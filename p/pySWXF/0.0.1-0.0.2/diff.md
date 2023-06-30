# Comparing `tmp/pyswxf-0.0.1.tar.gz` & `tmp/pyswxf-0.0.2.tar.gz`

## Comparing `pyswxf-0.0.1.tar` & `pyswxf-0.0.2.tar`

### file list

```diff
@@ -1,1522 +1,1521 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/src/pySWXF/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/src/pySWXF/n_to_rho.py
--rwxr-xr-x   0        0        0     3536 2020-02-02 00:00:00.000000 pyswxf-0.0.1/src/pySWXF/refl_funs.py
--rwxr-xr-x   0        0        0     3532 2020-02-02 00:00:00.000000 pyswxf-0.0.1/src/pySWXF/standing_wave.py
--rwxr-xr-x   0        0        0      914 2020-02-02 00:00:00.000000 pyswxf-0.0.1/src/pySWXF/xray_utils.py
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/pyvenv.cfg
--rwxr-xr-x   0        0        0     2273 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/activate
--rwxr-xr-x   0        0        0     1325 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/activate.csh
--rwxr-xr-x   0        0        0     2477 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/activate.fish
--rwxr-xr-x   0        0        0      324 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/docutils
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/easy_install
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/easy_install-3.7
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/keyring
--rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/markdown-it
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/normalizer
--rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/pip
--rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/pip3
--rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/pip3.10
--rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/pip3.7
--rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/pkginfo
--rwxr-xr-x   0        0        0      323 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/pygmentize
--rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/python3 -> /usr/bin/python3
--rwxr-xr-x   0        0        0      675 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2html.py
--rwxr-xr-x   0        0        0      797 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2html5.py
--rwxr-xr-x   0        0        0      874 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2latex.py
--rwxr-xr-x   0        0        0      697 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2man.py
--rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2odt.py
--rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      682 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2s5.py
--rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      683 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rst2xml.py
--rwxr-xr-x   0        0        0      751 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/bin/twine
--rwxr-xr-x   0        0        0   932624 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/_cffi_backend.cpython-37m-x86_64-linux-gnu.so
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/easy_install.py
--rwxr-xr-x   0        0        0   110349 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1504 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4027 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/METADATA
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0       14 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     3649 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/__init__.py
--rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/callbacks.py
--rwxr-xr-x   0        0        0     2526 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/css_sanitizer.py
--rwxr-xr-x   0        0        0    22779 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/html5lib_shim.py
--rwxr-xr-x   0        0        0    22350 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/linkifier.py
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/parse_shim.py
--rwxr-xr-x   0        0        0    21934 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/sanitizer.py
--rwxr-xr-x   0        0        0     2160 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/README.rst
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/__init__.py
--rwxr-xr-x   0        0        0    39023 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/parse.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/parse.py.SHA256SUM
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/vendor.txt
--rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/vendor_install.sh
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/__init__.py
--rwxr-xr-x   0        0        0    16728 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_ihatexml.py
--rwxr-xr-x   0        0        0    32300 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_inputstream.py
--rwxr-xr-x   0        0        0    77028 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_tokenizer.py
--rwxr-xr-x   0        0        0     4919 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_utils.py
--rwxr-xr-x   0        0        0    83464 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/constants.py
--rwxr-xr-x   0        0        0   117174 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/html5parser.py
--rwxr-xr-x   0        0        0    15747 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/serializer.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
--rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/_base.py
--rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/py.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/__init__.py
--rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/base.py
--rwxr-xr-x   0        0        0     2945 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
--rwxr-xr-x   0        0        0     3631 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/lint.py
--rwxr-xr-x   0        0        0    10588 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
--rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
--rwxr-xr-x   0        0        0     1214 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
--rwxr-xr-x   0        0        0     1715 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
--rwxr-xr-x   0        0        0     1776 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
--rwxr-xr-x   0        0        0     3592 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
--rwxr-xr-x   0        0        0    14553 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
--rwxr-xr-x   0        0        0     8925 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
--rwxr-xr-x   0        0        0    12824 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
--rwxr-xr-x   0        0        0    14754 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
--rwxr-xr-x   0        0        0     5719 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
--rwxr-xr-x   0        0        0     7476 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
--rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
--rwxr-xr-x   0        0        0     4539 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
--rwxr-xr-x   0        0        0     6345 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
--rwxr-xr-x   0        0        0     2309 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
--rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE
--rwxr-xr-x   0        0        0    16076 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA
--rwxr-xr-x   0        0        0     3486 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/REQUESTED
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      569 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0    29799 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     8456 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0    19190 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/__init__.py
--rwxr-xr-x   0        0        0    12200 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/__main__.py
--rwxr-xr-x   0        0        0    12636 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/env.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/py.typed
--rwxr-xr-x   0        0        0     1632 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/util.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4071 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1052 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/LICENSE
--rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/METADATA
--rwxr-xr-x   0        0        0     1006 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/WHEEL
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/__init__.py
--rwxr-xr-x   0        0        0     3908 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_errors.h
--rwxr-xr-x   0        0        0    14800 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_include.h
--rwxr-xr-x   0        0        0    17680 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/_embedding.h
--rwxr-xr-x   0        0        0    42064 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/api.py
--rwxr-xr-x   0        0        0    42454 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/backend_ctypes.py
--rwxr-xr-x   0        0        0     5724 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/cffi_opcode.py
--rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/commontypes.py
--rwxr-xr-x   0        0        0    44231 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/cparser.py
--rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/error.py
--rwxr-xr-x   0        0        0     4046 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/ffiplatform.py
--rwxr-xr-x   0        0        0      747 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/lock.py
--rwxr-xr-x   0        0        0    21768 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/model.py
--rwxr-xr-x   0        0        0     5976 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/parse_c_type.h
--rwxr-xr-x   0        0        0     4374 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/pkgconfig.py
--rwxr-xr-x   0        0        0    64598 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/recompiler.py
--rwxr-xr-x   0        0        0     8931 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/setuptools_ext.py
--rwxr-xr-x   0        0        0    43320 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/vengine_cpy.py
--rwxr-xr-x   0        0        0    26684 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/vengine_gen.py
--rwxr-xr-x   0        0        0    11253 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/verifier.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1294 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/LICENSE
--rwxr-xr-x   0        0        0     1144 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/METADATA
--rwxr-xr-x   0        0        0     2897 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/RECORD
--rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/__init__.py
--rwxr-xr-x   0        0        0    18624 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/api.py
--rwxr-xr-x   0        0        0    12554 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cd.py
--rwxr-xr-x   0        0        0    19101 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/constant.py
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/legacy.py
--rwxr-xr-x   0        0        0    17144 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.cpython-37m-x86_64-linux-gnu.so
--rwxr-xr-x   0        0        0    18258 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.py
--rwxr-xr-x   0        0        0   344664 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md__mypyc.cpython-37m-x86_64-linux-gnu.so
--rwxr-xr-x   0        0        0    11492 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/models.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/py.typed
--rwxr-xr-x   0        0        0    11544 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/utils.py
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/version.py
--rwxr-xr-x   0        0        0    20069 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/assets/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cli/__init__.py
--rwxr-xr-x   0        0        0     9744 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cli/normalizer.py
--rwxr-xr-x   0        0        0      445 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/__about__.py
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/__init__.py
--rwxr-xr-x   0        0        0     1118 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/exceptions.py
--rwxr-xr-x   0        0        0     6886 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/fernet.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/py.typed
--rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/utils.py
--rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/__init__.py
--rwxr-xr-x   0        0        0    14441 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/_oid.py
--rwxr-xr-x   0        0        0      361 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/__init__.py
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/__init__.py
--rwxr-xr-x   0        0        0    15967 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/aead.py
--rwxr-xr-x   0        0        0    73231 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/backend.py
--rwxr-xr-x   0        0        0    10358 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ciphers.py
--rwxr-xr-x   0        0        0     3035 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/cmac.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/decode_asn1.py
--rwxr-xr-x   0        0        0    11474 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ec.py
--rwxr-xr-x   0        0        0    21825 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/rsa.py
--rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/utils.py
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/__init__.py
--rwxr-xr-x   0        0        0 13408352 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust.abi3.so
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/__init__.pyi
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/_openssl.pyi
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/asn1.pyi
--rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/exceptions.pyi
--rwxr-xr-x   0        0        0      905 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/ocsp.pyi
--rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/pkcs7.pyi
--rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/x509.pyi
--rwxr-xr-x   0        0        0      970 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
--rwxr-xr-x   0        0        0      896 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
--rwxr-xr-x   0        0        0      764 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
--rwxr-xr-x   0        0        0      629 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
--rwxr-xr-x   0        0        0      603 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
--rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
--rwxr-xr-x   0        0        0      616 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
--rwxr-xr-x   0        0        0      590 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/__init__.py
--rwxr-xr-x   0        0        0     9098 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/_conditional.py
--rwxr-xr-x   0        0        0     6696 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/binding.py
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/__init__.py
--rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_asymmetric.py
--rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_cipheralgorithm.py
--rwxr-xr-x   0        0        0     5216 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_serialization.py
--rwxr-xr-x   0        0        0     2065 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/cmac.py
--rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/constant_time.py
--rwxr-xr-x   0        0        0     5115 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/hashes.py
--rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/hmac.py
--rwxr-xr-x   0        0        0     5678 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/keywrap.py
--rwxr-xr-x   0        0        0     6242 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/padding.py
--rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/poly1305.py
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/__init__.py
--rwxr-xr-x   0        0        0     7013 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dh.py
--rwxr-xr-x   0        0        0     8263 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dsa.py
--rwxr-xr-x   0        0        0    12867 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ec.py
--rwxr-xr-x   0        0        0     3489 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed25519.py
--rwxr-xr-x   0        0        0     3440 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed448.py
--rwxr-xr-x   0        0        0     2717 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/padding.py
--rwxr-xr-x   0        0        0    11623 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/rsa.py
--rwxr-xr-x   0        0        0     2996 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/types.py
--rwxr-xr-x   0        0        0      790 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/utils.py
--rwxr-xr-x   0        0        0     3437 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x25519.py
--rwxr-xr-x   0        0        0     3358 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x448.py
--rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/__init__.py
--rwxr-xr-x   0        0        0    12067 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/aead.py
--rwxr-xr-x   0        0        0     5000 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/algorithms.py
--rwxr-xr-x   0        0        0     8286 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/base.py
--rwxr-xr-x   0        0        0     8361 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/modes.py
--rwxr-xr-x   0        0        0      750 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/__init__.py
--rwxr-xr-x   0        0        0     3726 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/concatkdf.py
--rwxr-xr-x   0        0        0     3045 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/hkdf.py
--rwxr-xr-x   0        0        0     9232 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/kbkdf.py
--rwxr-xr-x   0        0        0     2012 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/pbkdf2.py
--rwxr-xr-x   0        0        0     2354 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/scrypt.py
--rwxr-xr-x   0        0        0     2002 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/x963kdf.py
--rwxr-xr-x   0        0        0     1653 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/__init__.py
--rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/base.py
--rwxr-xr-x   0        0        0     6767 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs12.py
--rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs7.py
--rwxr-xr-x   0        0        0    50088 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/ssh.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/__init__.py
--rwxr-xr-x   0        0        0     3010 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/hotp.py
--rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/totp.py
--rwxr-xr-x   0        0        0     7870 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/__init__.py
--rwxr-xr-x   0        0        0    35677 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/base.py
--rwxr-xr-x   0        0        0     2261 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/certificate_transparency.py
--rwxr-xr-x   0        0        0    68365 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/extensions.py
--rwxr-xr-x   0        0        0     7868 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/general_name.py
--rwxr-xr-x   0        0        0    14855 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/name.py
--rwxr-xr-x   0        0        0    18534 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/ocsp.py
--rwxr-xr-x   0        0        0      829 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/oid.py
--rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/COPYING.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     2817 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/METADATA
--rwxr-xr-x   0        0        0    28033 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0    30724 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/__init__.py
--rwxr-xr-x   0        0        0     2454 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_adapters.py
--rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_collections.py
--rwxr-xr-x   0        0        0     1735 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_compat.py
--rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_functools.py
--rwxr-xr-x   0        0        0     2068 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_itertools.py
--rwxr-xr-x   0        0        0     1615 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_meta.py
--rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_py39compat.py
--rwxr-xr-x   0        0        0     2166 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_text.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/py.typed
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0    11358 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4878 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     1952 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco/classes/__init__.py
--rwxr-xr-x   0        0        0     1464 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco/classes/ancestry.py
--rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco/classes/meta.py
--rwxr-xr-x   0        0        0     3996 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco/classes/properties.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE
--rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/METADATA
--rwxr-xr-x   0        0        0     1065 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/__init__.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/__main__.py
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/_compat.py
--rwxr-xr-x   0        0        0     3886 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/_properties_compat.py
--rwxr-xr-x   0        0        0     8100 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backend.py
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backend_complete.zsh
--rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/cli.py
--rwxr-xr-x   0        0        0     1324 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/completion.py
--rwxr-xr-x   0        0        0     5731 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/core.py
--rwxr-xr-x   0        0        0     1593 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/credentials.py
--rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/devpi_client.py
--rwxr-xr-x   0        0        0     1430 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/errors.py
--rwxr-xr-x   0        0        0     1231 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/http.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/py.typed
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/py312compat.py
--rwxr-xr-x   0        0        0     4692 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/SecretService.py
--rwxr-xr-x   0        0        0     5814 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/Windows.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/__init__.py
--rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/chainer.py
--rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/fail.py
--rwxr-xr-x   0        0        0     5830 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/kwallet.py
--rwxr-xr-x   0        0        0     5982 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/libsecret.py
--rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/null.py
--rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/__init__.py
--rwxr-xr-x   0        0        0     4341 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/api.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/testing/__init__.py
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/testing/backend.py
--rwxr-xr-x   0        0        0     1918 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/testing/util.py
--rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/util/__init__.py
--rwxr-xr-x   0        0        0     2215 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/util/platform_.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1023 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/LICENSE
--rwxr-xr-x   0        0        0    20512 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/METADATA
--rwxr-xr-x   0        0        0     4527 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/__init__.py
--rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/_compat.py
--rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/_punycode.py
--rwxr-xr-x   0        0        0    12228 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/main.py
--rwxr-xr-x   0        0        0     3662 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_block.py
--rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_core.py
--rwxr-xr-x   0        0        0     4130 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_inline.py
--rwxr-xr-x   0        0        0     2516 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/port.yaml
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/py.typed
--rwxr-xr-x   0        0        0    10041 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/renderer.py
--rwxr-xr-x   0        0        0     8376 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/ruler.py
--rwxr-xr-x   0        0        0     6374 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/token.py
--rwxr-xr-x   0        0        0    11052 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/tree.py
--rwxr-xr-x   0        0        0     3262 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/utils.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/cli/__init__.py
--rwxr-xr-x   0        0        0     2901 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/cli/parse.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/__init__.py
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/entities.py
--rwxr-xr-x   0        0        0      932 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_blocks.py
--rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_re.py
--rwxr-xr-x   0        0        0     2631 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/normalize_url.py
--rwxr-xr-x   0        0        0    10894 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/utils.py
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/__init__.py
--rwxr-xr-x   0        0        0     1953 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_destination.py
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_label.py
--rwxr-xr-x   0        0        0     1410 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_title.py
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/__init__.py
--rwxr-xr-x   0        0        0     2809 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/commonmark.py
--rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/default.py
--rwxr-xr-x   0        0        0     2006 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/zero.py
--rwxr-xr-x   0        0        0      553 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/__init__.py
--rwxr-xr-x   0        0        0     9057 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/blockquote.py
--rwxr-xr-x   0        0        0      886 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/code.py
--rwxr-xr-x   0        0        0     2704 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/fence.py
--rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/heading.py
--rwxr-xr-x   0        0        0     1309 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/hr.py
--rwxr-xr-x   0        0        0     2808 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/html_block.py
--rwxr-xr-x   0        0        0     2798 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/lheading.py
--rwxr-xr-x   0        0        0     9944 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/list.py
--rwxr-xr-x   0        0        0     1851 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/paragraph.py
--rwxr-xr-x   0        0        0     6323 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/reference.py
--rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/state_block.py
--rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/table.py
--rwxr-xr-x   0        0        0      344 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/__init__.py
--rwxr-xr-x   0        0        0      413 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/block.py
--rwxr-xr-x   0        0        0      325 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/inline.py
--rwxr-xr-x   0        0        0     4833 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/linkify.py
--rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/normalize.py
--rwxr-xr-x   0        0        0     3560 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/replacements.py
--rwxr-xr-x   0        0        0     7251 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/smartquotes.py
--rwxr-xr-x   0        0        0      584 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/state_core.py
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/__init__.py
--rwxr-xr-x   0        0        0     2131 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/autolink.py
--rwxr-xr-x   0        0        0     2112 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/backticks.py
--rwxr-xr-x   0        0        0     4062 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/balance_pairs.py
--rwxr-xr-x   0        0        0     2948 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/emphasis.py
--rwxr-xr-x   0        0        0     1653 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/entity.py
--rwxr-xr-x   0        0        0     1116 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/escape.py
--rwxr-xr-x   0        0        0     1019 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/html_inline.py
--rwxr-xr-x   0        0        0     4260 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/image.py
--rwxr-xr-x   0        0        0     4362 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/link.py
--rwxr-xr-x   0        0        0     1176 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/newline.py
--rwxr-xr-x   0        0        0     5388 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/state_inline.py
--rwxr-xr-x   0        0        0     3390 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/strikethrough.py
--rwxr-xr-x   0        0        0     1427 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text.py
--rwxr-xr-x   0        0        0     1491 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text_collapse.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1078 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it
--rwxr-xr-x   0        0        0     6812 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/METADATA
--rwxr-xr-x   0        0        0    10448 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     2338 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rwxr-xr-x   0        0        0     1638 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/METADATA
--rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/WHEEL
--rwxr-xr-x   0        0        0      501 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/__init__.py
--rwxr-xr-x   0        0        0     3266 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_elffile.py
--rwxr-xr-x   0        0        0     8926 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_manylinux.py
--rwxr-xr-x   0        0        0     2524 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_musllinux.py
--rwxr-xr-x   0        0        0    10194 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_parser.py
--rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_structures.py
--rwxr-xr-x   0        0        0     5292 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_tokenizer.py
--rwxr-xr-x   0        0        0     8208 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/markers.py
--rwxr-xr-x   0        0        0    16397 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/metadata.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/py.typed
--rwxr-xr-x   0        0        0     3287 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/requirements.py
--rwxr-xr-x   0        0        0    39206 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/specifiers.py
--rwxr-xr-x   0        0        0    18106 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/tags.py
--rwxr-xr-x   0        0        0     4355 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/utils.py
--rwxr-xr-x   0        0        0    16326 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/version.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE
--rwxr-xr-x   0        0        0    10174 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.APACHE
--rwxr-xr-x   0        0        0     1344 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.BSD
--rwxr-xr-x   0        0        0     3082 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/METADATA
--rwxr-xr-x   0        0        0     2461 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/__init__.py
--rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/__main__.py
--rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/__pip-runner__.py
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/py.typed
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/__init__.py
--rwxr-xr-x   0        0        0    10243 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/build_env.py
--rwxr-xr-x   0        0        0     9661 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cache.py
--rwxr-xr-x   0        0        0    13529 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/configuration.py
--rwxr-xr-x   0        0        0    23741 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/exceptions.py
--rwxr-xr-x   0        0        0      340 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/main.py
--rwxr-xr-x   0        0        0     7161 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/pyproject.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/self_outdated_check.py
--rwxr-xr-x   0        0        0    11842 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/wheel_builder.py
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/__init__.py
--rwxr-xr-x   0        0        0     6676 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/autocompletion.py
--rwxr-xr-x   0        0        0     8176 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/base_command.py
--rwxr-xr-x   0        0        0    30030 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/cmdoptions.py
--rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/command_context.py
--rwxr-xr-x   0        0        0     2816 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main.py
--rwxr-xr-x   0        0        0     4338 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main_parser.py
--rwxr-xr-x   0        0        0    10817 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/parser.py
--rwxr-xr-x   0        0        0     1968 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/progress_bars.py
--rwxr-xr-x   0        0        0    18328 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/req_command.py
--rwxr-xr-x   0        0        0     5118 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/spinners.py
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/status_codes.py
--rwxr-xr-x   0        0        0     3882 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/__init__.py
--rwxr-xr-x   0        0        0     7581 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/cache.py
--rwxr-xr-x   0        0        0     1684 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/check.py
--rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/completion.py
--rwxr-xr-x   0        0        0     9815 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/configuration.py
--rwxr-xr-x   0        0        0     6591 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/debug.py
--rwxr-xr-x   0        0        0     5182 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/download.py
--rwxr-xr-x   0        0        0     2951 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/freeze.py
--rwxr-xr-x   0        0        0     1703 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/hash.py
--rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/help.py
--rwxr-xr-x   0        0        0     4793 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/index.py
--rwxr-xr-x   0        0        0     3188 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/inspect.py
--rwxr-xr-x   0        0        0    28722 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/install.py
--rwxr-xr-x   0        0        0    12343 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/list.py
--rwxr-xr-x   0        0        0     5697 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/search.py
--rwxr-xr-x   0        0        0     6419 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/show.py
--rwxr-xr-x   0        0        0     3886 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/uninstall.py
--rwxr-xr-x   0        0        0     6324 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/wheel.py
--rwxr-xr-x   0        0        0      858 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/__init__.py
--rwxr-xr-x   0        0        0     1221 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/base.py
--rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/installed.py
--rwxr-xr-x   0        0        0     6494 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/sdist.py
--rwxr-xr-x   0        0        0     1164 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/wheel.py
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/__init__.py
--rwxr-xr-x   0        0        0    16504 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/collector.py
--rwxr-xr-x   0        0        0    37873 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/package_finder.py
--rwxr-xr-x   0        0        0     6556 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/sources.py
--rwxr-xr-x   0        0        0    15365 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/__init__.py
--rwxr-xr-x   0        0        0     6100 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_distutils.py
--rwxr-xr-x   0        0        0     7680 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_sysconfig.py
--rwxr-xr-x   0        0        0     2556 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/base.py
--rwxr-xr-x   0        0        0     4280 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/__init__.py
--rwxr-xr-x   0        0        0     2595 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/_json.py
--rwxr-xr-x   0        0        0    25277 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/base.py
--rwxr-xr-x   0        0        0     9773 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/pkg_resources.py
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/__init__.py
--rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_compat.py
--rwxr-xr-x   0        0        0     8181 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_dists.py
--rwxr-xr-x   0        0        0     7457 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_envs.py
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/__init__.py
--rwxr-xr-x   0        0        0      990 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/candidate.py
--rwxr-xr-x   0        0        0     6931 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/direct_url.py
--rwxr-xr-x   0        0        0     2520 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/format_control.py
--rwxr-xr-x   0        0        0     1030 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/index.py
--rwxr-xr-x   0        0        0     2619 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/installation_report.py
--rwxr-xr-x   0        0        0    18817 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/link.py
--rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/scheme.py
--rwxr-xr-x   0        0        0     4643 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/search_scope.py
--rwxr-xr-x   0        0        0     1907 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/selection_prefs.py
--rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/target_python.py
--rwxr-xr-x   0        0        0     3600 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/wheel.py
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/__init__.py
--rwxr-xr-x   0        0        0    20435 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/auth.py
--rwxr-xr-x   0        0        0     2145 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/cache.py
--rwxr-xr-x   0        0        0     6096 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/download.py
--rwxr-xr-x   0        0        0     7638 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/lazy_wheel.py
--rwxr-xr-x   0        0        0    18442 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/session.py
--rwxr-xr-x   0        0        0     4073 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/utils.py
--rwxr-xr-x   0        0        0     1791 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/xmlrpc.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/__init__.py
--rwxr-xr-x   0        0        0     5122 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/check.py
--rwxr-xr-x   0        0        0     9816 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/freeze.py
--rwxr-xr-x   0        0        0    27696 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/prepare.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/__init__.py
--rwxr-xr-x   0        0        0     4133 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/build_tracker.py
--rwxr-xr-x   0        0        0     1422 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata.py
--rwxr-xr-x   0        0        0     1474 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_editable.py
--rwxr-xr-x   0        0        0     2198 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rwxr-xr-x   0        0        0     1075 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel.py
--rwxr-xr-x   0        0        0     1417 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_editable.py
--rwxr-xr-x   0        0        0     3064 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/__init__.py
--rwxr-xr-x   0        0        0     1282 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/editable_legacy.py
--rwxr-xr-x   0        0        0    27475 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/wheel.py
--rwxr-xr-x   0        0        0     2738 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/__init__.py
--rwxr-xr-x   0        0        0    16610 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/constructors.py
--rwxr-xr-x   0        0        0    17872 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_file.py
--rwxr-xr-x   0        0        0    32782 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_install.py
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_set.py
--rwxr-xr-x   0        0        0    24678 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_uninstall.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/__init__.py
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/base.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/legacy/__init__.py
--rwxr-xr-x   0        0        0    24128 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/legacy/resolver.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rwxr-xr-x   0        0        0     5220 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/base.py
--rwxr-xr-x   0        0        0    18864 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rwxr-xr-x   0        0        0    27845 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rwxr-xr-x   0        0        0     5705 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rwxr-xr-x   0        0        0     9824 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rwxr-xr-x   0        0        0     3094 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rwxr-xr-x   0        0        0     5454 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rwxr-xr-x   0        0        0    11538 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/__init__.py
--rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_jaraco_text.py
--rwxr-xr-x   0        0        0     1015 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_log.py
--rwxr-xr-x   0        0        0     1665 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/appdirs.py
--rwxr-xr-x   0        0        0     1884 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compat.py
--rwxr-xr-x   0        0        0     5377 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compatibility_tags.py
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/datetime.py
--rwxr-xr-x   0        0        0     3627 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/deprecation.py
--rwxr-xr-x   0        0        0     3206 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/direct_url_helpers.py
--rwxr-xr-x   0        0        0     2118 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/egg_link.py
--rwxr-xr-x   0        0        0     1169 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/encoding.py
--rwxr-xr-x   0        0        0     3064 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/entrypoints.py
--rwxr-xr-x   0        0        0     5122 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filesystem.py
--rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filetypes.py
--rwxr-xr-x   0        0        0     3110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/glibc.py
--rwxr-xr-x   0        0        0     5118 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/hashes.py
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/inject_securetransport.py
--rwxr-xr-x   0        0        0    11632 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/logging.py
--rwxr-xr-x   0        0        0    22216 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/misc.py
--rwxr-xr-x   0        0        0     1193 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/models.py
--rwxr-xr-x   0        0        0     2108 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/packaging.py
--rwxr-xr-x   0        0        0     4435 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/setuptools_build.py
--rwxr-xr-x   0        0        0     9200 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/subprocess.py
--rwxr-xr-x   0        0        0     7702 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/temp_dir.py
--rwxr-xr-x   0        0        0     8821 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/unpacking.py
--rwxr-xr-x   0        0        0     1759 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/urls.py
--rwxr-xr-x   0        0        0     3456 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/virtualenv.py
--rwxr-xr-x   0        0        0     4549 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/wheel.py
--rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/__init__.py
--rwxr-xr-x   0        0        0     3519 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/bazaar.py
--rwxr-xr-x   0        0        0    18116 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/git.py
--rwxr-xr-x   0        0        0     5238 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/mercurial.py
--rwxr-xr-x   0        0        0    11729 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/subversion.py
--rwxr-xr-x   0        0        0    22811 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/versioncontrol.py
--rwxr-xr-x   0        0        0     4966 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/__init__.py
--rwxr-xr-x   0        0        0    34549 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/six.py
--rwxr-xr-x   0        0        0    84101 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/typing_extensions.py
--rwxr-xr-x   0        0        0      476 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/vendor.txt
--rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/__init__.py
--rwxr-xr-x   0        0        0     1379 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rwxr-xr-x   0        0        0     5033 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/adapter.py
--rwxr-xr-x   0        0        0     1535 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/cache.py
--rwxr-xr-x   0        0        0      778 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/compat.py
--rwxr-xr-x   0        0        0    16416 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/controller.py
--rwxr-xr-x   0        0        0     3946 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rwxr-xr-x   0        0        0     4154 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rwxr-xr-x   0        0        0     7105 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/serialize.py
--rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rwxr-xr-x   0        0        0     5271 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rwxr-xr-x   0        0        0     1033 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/__init__.py
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/__main__.py
--rwxr-xr-x   0        0        0   275233 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/cacert.pem
--rwxr-xr-x   0        0        0     4279 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/core.py
--rwxr-xr-x   0        0        0     4797 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/__init__.py
--rwxr-xr-x   0        0        0    31274 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5freq.py
--rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5prober.py
--rwxr-xr-x   0        0        0    10032 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/chardistribution.py
--rwxr-xr-x   0        0        0     3915 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rwxr-xr-x   0        0        0     5420 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetprober.py
--rwxr-xr-x   0        0        0     3732 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rwxr-xr-x   0        0        0      542 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cp949prober.py
--rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/enums.py
--rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escprober.py
--rwxr-xr-x   0        0        0    12176 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escsm.py
--rwxr-xr-x   0        0        0     3934 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/eucjpprober.py
--rwxr-xr-x   0        0        0    13566 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrfreq.py
--rwxr-xr-x   0        0        0     1753 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrprober.py
--rwxr-xr-x   0        0        0    36913 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwfreq.py
--rwxr-xr-x   0        0        0     1753 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwprober.py
--rwxr-xr-x   0        0        0    20735 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312freq.py
--rwxr-xr-x   0        0        0     1759 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312prober.py
--rwxr-xr-x   0        0        0    14537 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/hebrewprober.py
--rwxr-xr-x   0        0        0    25796 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jisfreq.py
--rwxr-xr-x   0        0        0    42498 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabfreq.py
--rwxr-xr-x   0        0        0     1752 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabprober.py
--rwxr-xr-x   0        0        0    27055 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jpcntx.py
--rwxr-xr-x   0        0        0   104562 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rwxr-xr-x   0        0        0    98484 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rwxr-xr-x   0        0        0    98196 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rwxr-xr-x   0        0        0   101363 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rwxr-xr-x   0        0        0   128035 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rwxr-xr-x   0        0        0   102774 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langthaimodel.py
--rwxr-xr-x   0        0        0    95372 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rwxr-xr-x   0        0        0     5380 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/latin1prober.py
--rwxr-xr-x   0        0        0     6077 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/macromanprober.py
--rwxr-xr-x   0        0        0     3715 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rwxr-xr-x   0        0        0     2131 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rwxr-xr-x   0        0        0    30391 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcssm.py
--rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/resultdict.py
--rwxr-xr-x   0        0        0     6400 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rwxr-xr-x   0        0        0     4137 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rwxr-xr-x   0        0        0     4007 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sjisprober.py
--rwxr-xr-x   0        0        0    14848 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/universaldetector.py
--rwxr-xr-x   0        0        0     8505 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf1632prober.py
--rwxr-xr-x   0        0        0     2812 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf8prober.py
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/version.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cli/__init__.py
--rwxr-xr-x   0        0        0     3242 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rwxr-xr-x   0        0        0    13560 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/languages.py
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/__init__.py
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansi.py
--rwxr-xr-x   0        0        0    11128 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansitowin32.py
--rwxr-xr-x   0        0        0     3325 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/initialise.py
--rwxr-xr-x   0        0        0     6181 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/win32.py
--rwxr-xr-x   0        0        0     7134 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/winterm.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/__init__.py
--rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rwxr-xr-x   0        0        0    10678 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rwxr-xr-x   0        0        0     6741 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/utils.py
--rwxr-xr-x   0        0        0     3709 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rwxr-xr-x   0        0        0      581 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/__init__.py
--rwxr-xr-x   0        0        0    41259 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/compat.py
--rwxr-xr-x   0        0        0    51697 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/database.py
--rwxr-xr-x   0        0        0    20834 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/index.py
--rwxr-xr-x   0        0        0    51991 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/locators.py
--rwxr-xr-x   0        0        0    14811 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/manifest.py
--rwxr-xr-x   0        0        0     5058 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/markers.py
--rwxr-xr-x   0        0        0    39801 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/metadata.py
--rwxr-xr-x   0        0        0    10820 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/resources.py
--rwxr-xr-x   0        0        0    18102 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64.exe
--rwxr-xr-x   0        0        0    66262 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/util.py
--rwxr-xr-x   0        0        0    23513 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64.exe
--rwxr-xr-x   0        0        0    43898 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/wheel.py
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/__init__.py
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/__main__.py
--rwxr-xr-x   0        0        0    49330 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/distro.py
--rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/__init__.py
--rwxr-xr-x   0        0        0     3374 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/codec.py
--rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/compat.py
--rwxr-xr-x   0        0        0    12950 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/core.py
--rwxr-xr-x   0        0        0    44375 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/idnadata.py
--rwxr-xr-x   0        0        0     1881 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/intranges.py
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/package_data.py
--rwxr-xr-x   0        0        0   206539 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/uts46data.py
--rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/__init__.py
--rwxr-xr-x   0        0        0     1081 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/exceptions.py
--rwxr-xr-x   0        0        0     6079 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/ext.py
--rwxr-xr-x   0        0        0    34544 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/fallback.py
--rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0    11488 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_manylinux.py
--rwxr-xr-x   0        0        0     4378 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_musllinux.py
--rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     8487 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4676 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    30110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0    15699 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/tags.py
--rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    14665 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0   109388 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pkg_resources/__init__.py
--rwxr-xr-x   0        0        0    18003 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__init__.py
--rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__main__.py
--rwxr-xr-x   0        0        0     4303 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/android.py
--rwxr-xr-x   0        0        0     5706 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/api.py
--rwxr-xr-x   0        0        0     2800 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/macos.py
--rwxr-xr-x   0        0        0     7448 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/unix.py
--rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/version.py
--rwxr-xr-x   0        0        0     7098 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/windows.py
--rwxr-xr-x   0        0        0     2999 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/__init__.py
--rwxr-xr-x   0        0        0      353 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/__main__.py
--rwxr-xr-x   0        0        0    23685 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/cmdline.py
--rwxr-xr-x   0        0        0     1697 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/console.py
--rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filter.py
--rwxr-xr-x   0        0        0     2917 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatter.py
--rwxr-xr-x   0        0        0    32064 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexer.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/modeline.py
--rwxr-xr-x   0        0        0     2591 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/plugin.py
--rwxr-xr-x   0        0        0     3072 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/regexopt.py
--rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/scanner.py
--rwxr-xr-x   0        0        0     6882 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/sphinxext.py
--rwxr-xr-x   0        0        0     6257 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/style.py
--rwxr-xr-x   0        0        0     6184 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/token.py
--rwxr-xr-x   0        0        0    63187 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/unistring.py
--rwxr-xr-x   0        0        0     9110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/util.py
--rwxr-xr-x   0        0        0    40386 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filters/__init__.py
--rwxr-xr-x   0        0        0     4800 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rwxr-xr-x   0        0        0     4104 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rwxr-xr-x   0        0        0     3314 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rwxr-xr-x   0        0        0     5086 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/groff.py
--rwxr-xr-x   0        0        0    35601 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/html.py
--rwxr-xr-x   0        0        0    21938 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/img.py
--rwxr-xr-x   0        0        0     4981 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/irc.py
--rwxr-xr-x   0        0        0    19351 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/latex.py
--rwxr-xr-x   0        0        0     5073 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/other.py
--rwxr-xr-x   0        0        0     2212 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rwxr-xr-x   0        0        0     5014 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rwxr-xr-x   0        0        0     7335 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/svg.py
--rwxr-xr-x   0        0        0     4674 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rwxr-xr-x   0        0        0    11753 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rwxr-xr-x   0        0        0    11164 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rwxr-xr-x   0        0        0    71556 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rwxr-xr-x   0        0        0    53572 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/python.py
--rwxr-xr-x   0        0        0     3419 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/styles/__init__.py
--rwxr-xr-x   0        0        0     9171 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/__init__.py
--rwxr-xr-x   0        0        0     6426 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/actions.py
--rwxr-xr-x   0        0        0    12936 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/common.py
--rwxr-xr-x   0        0        0   213344 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/core.py
--rwxr-xr-x   0        0        0     9023 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/exceptions.py
--rwxr-xr-x   0        0        0    39129 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/helpers.py
--rwxr-xr-x   0        0        0    25341 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/results.py
--rwxr-xr-x   0        0        0    13402 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/testing.py
--rwxr-xr-x   0        0        0    10787 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/unicode.py
--rwxr-xr-x   0        0        0     6805 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/util.py
--rwxr-xr-x   0        0        0    23685 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rwxr-xr-x   0        0        0      491 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rwxr-xr-x   0        0        0    11920 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rwxr-xr-x   0        0        0    10927 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rwxr-xr-x   0        0        0     5178 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/__init__.py
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/__version__.py
--rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/_internal_utils.py
--rwxr-xr-x   0        0        0    21443 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/adapters.py
--rwxr-xr-x   0        0        0     6377 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/api.py
--rwxr-xr-x   0        0        0    10187 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/auth.py
--rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/certs.py
--rwxr-xr-x   0        0        0     1286 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/compat.py
--rwxr-xr-x   0        0        0    18560 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/cookies.py
--rwxr-xr-x   0        0        0     3823 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/exceptions.py
--rwxr-xr-x   0        0        0     3879 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/help.py
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/hooks.py
--rwxr-xr-x   0        0        0    35288 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/models.py
--rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/packages.py
--rwxr-xr-x   0        0        0    30180 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/sessions.py
--rwxr-xr-x   0        0        0     4235 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/status_codes.py
--rwxr-xr-x   0        0        0     2912 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/structures.py
--rwxr-xr-x   0        0        0    33240 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/utils.py
--rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/__init__.py
--rwxr-xr-x   0        0        0     5871 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/providers.py
--rwxr-xr-x   0        0        0     1601 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/reporters.py
--rwxr-xr-x   0        0        0    20511 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/resolvers.py
--rwxr-xr-x   0        0        0     4963 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/structs.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rwxr-xr-x   0        0        0     6090 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__init__.py
--rwxr-xr-x   0        0        0     8478 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__main__.py
--rwxr-xr-x   0        0        0    10096 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_cell_widths.py
--rwxr-xr-x   0        0        0   140235 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_codes.py
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_replace.py
--rwxr-xr-x   0        0        0     2100 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_export_format.py
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_extension.py
--rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_fileno.py
--rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_inspect.py
--rwxr-xr-x   0        0        0     3225 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_log_render.py
--rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_loop.py
--rwxr-xr-x   0        0        0     1387 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_null_file.py
--rwxr-xr-x   0        0        0     7063 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_palettes.py
--rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_pick.py
--rwxr-xr-x   0        0        0     5472 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_ratio.py
--rwxr-xr-x   0        0        0    19919 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_spinners.py
--rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_stack.py
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_timer.py
--rwxr-xr-x   0        0        0    22820 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_win32_console.py
--rwxr-xr-x   0        0        0     1926 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows.py
--rwxr-xr-x   0        0        0     2783 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows_renderer.py
--rwxr-xr-x   0        0        0     1840 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_wrap.py
--rwxr-xr-x   0        0        0      890 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/abc.py
--rwxr-xr-x   0        0        0    10368 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/align.py
--rwxr-xr-x   0        0        0     6906 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/ansi.py
--rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/bar.py
--rwxr-xr-x   0        0        0     9842 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/box.py
--rwxr-xr-x   0        0        0     4509 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/cells.py
--rwxr-xr-x   0        0        0    18224 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color.py
--rwxr-xr-x   0        0        0     1054 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color_triplet.py
--rwxr-xr-x   0        0        0     7131 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/columns.py
--rwxr-xr-x   0        0        0    99195 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/console.py
--rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/constrain.py
--rwxr-xr-x   0        0        0     5497 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/containers.py
--rwxr-xr-x   0        0        0     6630 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/control.py
--rwxr-xr-x   0        0        0     8082 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/default_styles.py
--rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/diagnose.py
--rwxr-xr-x   0        0        0     2501 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/emoji.py
--rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/errors.py
--rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/file_proxy.py
--rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/filesize.py
--rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/highlighter.py
--rwxr-xr-x   0        0        0     5032 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/json.py
--rwxr-xr-x   0        0        0     3252 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/jupyter.py
--rwxr-xr-x   0        0        0    14007 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/layout.py
--rwxr-xr-x   0        0        0    14273 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live.py
--rwxr-xr-x   0        0        0     3667 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live_render.py
--rwxr-xr-x   0        0        0    11903 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/logging.py
--rwxr-xr-x   0        0        0     8198 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/markup.py
--rwxr-xr-x   0        0        0     5305 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/measure.py
--rwxr-xr-x   0        0        0     4970 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/padding.py
--rwxr-xr-x   0        0        0      828 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pager.py
--rwxr-xr-x   0        0        0     3396 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/palette.py
--rwxr-xr-x   0        0        0    10574 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/panel.py
--rwxr-xr-x   0        0        0    35852 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pretty.py
--rwxr-xr-x   0        0        0    59706 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress.py
--rwxr-xr-x   0        0        0     8165 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress_bar.py
--rwxr-xr-x   0        0        0    11303 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/prompt.py
--rwxr-xr-x   0        0        0     1391 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/protocol.py
--rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/region.py
--rwxr-xr-x   0        0        0     4431 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/repr.py
--rwxr-xr-x   0        0        0     4602 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/rule.py
--rwxr-xr-x   0        0        0     2843 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/scope.py
--rwxr-xr-x   0        0        0     1591 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/screen.py
--rwxr-xr-x   0        0        0    24247 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/segment.py
--rwxr-xr-x   0        0        0     4339 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/spinner.py
--rwxr-xr-x   0        0        0     4425 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/status.py
--rwxr-xr-x   0        0        0    27073 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/style.py
--rwxr-xr-x   0        0        0     1258 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/styled.py
--rwxr-xr-x   0        0        0    35153 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/syntax.py
--rwxr-xr-x   0        0        0    39684 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/table.py
--rwxr-xr-x   0        0        0     3370 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/terminal_theme.py
--rwxr-xr-x   0        0        0    45525 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/text.py
--rwxr-xr-x   0        0        0     3777 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/theme.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/themes.py
--rwxr-xr-x   0        0        0    29604 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/traceback.py
--rwxr-xr-x   0        0        0     9169 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/tree.py
--rwxr-xr-x   0        0        0    20493 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/__init__.py
--rwxr-xr-x   0        0        0     3551 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_asyncio.py
--rwxr-xr-x   0        0        0     2179 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_utils.py
--rwxr-xr-x   0        0        0     1682 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/after.py
--rwxr-xr-x   0        0        0     1562 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before.py
--rwxr-xr-x   0        0        0     2372 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before_sleep.py
--rwxr-xr-x   0        0        0     1383 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/nap.py
--rwxr-xr-x   0        0        0     8746 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/retry.py
--rwxr-xr-x   0        0        0     3086 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/stop.py
--rwxr-xr-x   0        0        0     2142 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rwxr-xr-x   0        0        0     8024 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/wait.py
--rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/__init__.py
--rwxr-xr-x   0        0        0    22633 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_parser.py
--rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_re.py
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_types.py
--rwxr-xr-x   0        0        0     3333 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/__init__.py
--rwxr-xr-x   0        0        0    10811 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/_collections.py
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/_version.py
--rwxr-xr-x   0        0        0    20300 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connection.py
--rwxr-xr-x   0        0        0    39128 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connectionpool.py
--rwxr-xr-x   0        0        0     8217 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/exceptions.py
--rwxr-xr-x   0        0        0     8579 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/fields.py
--rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/filepost.py
--rwxr-xr-x   0        0        0    19786 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/poolmanager.py
--rwxr-xr-x   0        0        0     5985 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/request.py
--rwxr-xr-x   0        0        0    30641 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/response.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rwxr-xr-x   0        0        0    11036 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rwxr-xr-x   0        0        0     4528 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rwxr-xr-x   0        0        0    17081 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rwxr-xr-x   0        0        0    34448 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rwxr-xr-x   0        0        0     7097 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rwxr-xr-x   0        0        0    17632 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rwxr-xr-x   0        0        0    13922 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rwxr-xr-x   0        0        0    34665 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/six.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rwxr-xr-x   0        0        0     1417 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rwxr-xr-x   0        0        0     1155 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/__init__.py
--rwxr-xr-x   0        0        0     4901 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/connection.py
--rwxr-xr-x   0        0        0     1605 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/proxy.py
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/queue.py
--rwxr-xr-x   0        0        0     3997 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/request.py
--rwxr-xr-x   0        0        0     3510 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/response.py
--rwxr-xr-x   0        0        0    22003 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/retry.py
--rwxr-xr-x   0        0        0    17177 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rwxr-xr-x   0        0        0     5758 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rwxr-xr-x   0        0        0     6895 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rwxr-xr-x   0        0        0    10168 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/timeout.py
--rwxr-xr-x   0        0        0    14296 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/url.py
--rwxr-xr-x   0        0        0     5403 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/wait.py
--rwxr-xr-x   0        0        0    10579 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/__init__.py
--rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/labels.py
--rwxr-xr-x   0        0        0     1305 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/mklabels.py
--rwxr-xr-x   0        0        0     6563 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/tests.py
--rwxr-xr-x   0        0        0     4307 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rwxr-xr-x   0        0        0     9953 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/METADATA
--rwxr-xr-x   0        0        0    76554 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/WHEEL
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/top_level.txt
--rwxr-xr-x   0        0        0   103551 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/__init__.py
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/py31compat.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/__init__.py
--rwxr-xr-x   0        0        0    22376 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/appdirs.py
--rwxr-xr-x   0        0        0   229871 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0    30098 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/six.py
--rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0      860 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rwxr-xr-x   0        0        0     1416 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     8248 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4355 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    28025 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    11556 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0     2487 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/extern/__init__.py
--rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/DESCRIPTION.rst
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/RECORD
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/metadata.json
--rwxr-xr-x   0        0        0     2959 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/__init__.py
--rwxr-xr-x   0        0        0      348 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/__main__.py
--rwxr-xr-x   0        0        0    23530 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/cmdline.py
--rwxr-xr-x   0        0        0     1697 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/console.py
--rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/filter.py
--rwxr-xr-x   0        0        0     4154 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatter.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/modeline.py
--rwxr-xr-x   0        0        0     2579 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/plugin.py
--rwxr-xr-x   0        0        0     3072 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/regexopt.py
--rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/scanner.py
--rwxr-xr-x   0        0        0     6816 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/sphinxext.py
--rwxr-xr-x   0        0        0     6245 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/style.py
--rwxr-xr-x   0        0        0     6184 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/token.py
--rwxr-xr-x   0        0        0    63223 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/unistring.py
--rwxr-xr-x   0        0        0    10230 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/util.py
--rwxr-xr-x   0        0        0    40338 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/filters/__init__.py
--rwxr-xr-x   0        0        0     5388 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/__init__.py
--rwxr-xr-x   0        0        0     4176 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/_mapping.py
--rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/bbcode.py
--rwxr-xr-x   0        0        0     5070 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/groff.py
--rwxr-xr-x   0        0        0    35574 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/html.py
--rwxr-xr-x   0        0        0    21914 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/img.py
--rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/irc.py
--rwxr-xr-x   0        0        0    19303 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/latex.py
--rwxr-xr-x   0        0        0     5025 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/other.py
--rwxr-xr-x   0        0        0     2200 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/pangomarkup.py
--rwxr-xr-x   0        0        0     4990 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/rtf.py
--rwxr-xr-x   0        0        0     7299 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/svg.py
--rwxr-xr-x   0        0        0     4626 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal.py
--rwxr-xr-x   0        0        0    11717 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal256.py
--rwxr-xr-x   0        0        0    12082 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/__init__.py
--rwxr-xr-x   0        0        0     1543 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_ada_builtins.py
--rwxr-xr-x   0        0        0    27287 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_asy_builtins.py
--rwxr-xr-x   0        0        0    13994 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cl_builtins.py
--rwxr-xr-x   0        0        0   105182 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cocoa_builtins.py
--rwxr-xr-x   0        0        0    18414 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_csound_builtins.py
--rwxr-xr-x   0        0        0    12446 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_css_builtins.py
--rwxr-xr-x   0        0        0    11883 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_julia_builtins.py
--rwxr-xr-x   0        0        0   134510 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lasso_builtins.py
--rwxr-xr-x   0        0        0   108094 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lilypond_builtins.py
--rwxr-xr-x   0        0        0     8116 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lua_builtins.py
--rwxr-xr-x   0        0        0    65633 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mapping.py
--rwxr-xr-x   0        0        0    24713 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mql_builtins.py
--rwxr-xr-x   0        0        0    25842 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mysql_builtins.py
--rwxr-xr-x   0        0        0    49398 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_openedge_builtins.py
--rwxr-xr-x   0        0        0   107930 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_php_builtins.py
--rwxr-xr-x   0        0        0    13355 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_postgres_builtins.py
--rwxr-xr-x   0        0        0    32564 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scheme_builtins.py
--rwxr-xr-x   0        0        0    52413 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scilab_builtins.py
--rwxr-xr-x   0        0        0    26781 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_sourcemod_builtins.py
--rwxr-xr-x   0        0        0    13445 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stan_builtins.py
--rwxr-xr-x   0        0        0    27227 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stata_builtins.py
--rwxr-xr-x   0        0        0    15460 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_tsql_builtins.py
--rwxr-xr-x   0        0        0     1658 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_usd_builtins.py
--rwxr-xr-x   0        0        0     4225 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vbscript_builtins.py
--rwxr-xr-x   0        0        0    57066 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vim_builtins.py
--rwxr-xr-x   0        0        0    11676 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/actionscript.py
--rwxr-xr-x   0        0        0     5320 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ada.py
--rwxr-xr-x   0        0        0      876 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/agile.py
--rwxr-xr-x   0        0        0     9873 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/algebra.py
--rwxr-xr-x   0        0        0     2606 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ambient.py
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/amdgpu.py
--rwxr-xr-x   0        0        0     4177 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ampl.py
--rwxr-xr-x   0        0        0    30766 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apdlexer.py
--rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apl.py
--rwxr-xr-x   0        0        0    11469 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/archetype.py
--rwxr-xr-x   0        0        0     3565 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arrow.py
--rwxr-xr-x   0        0        0    11417 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arturo.py
--rwxr-xr-x   0        0        0     1621 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asc.py
--rwxr-xr-x   0        0        0    41243 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asm.py
--rwxr-xr-x   0        0        0    19815 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/automation.py
--rwxr-xr-x   0        0        0     3915 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/boa.py
--rwxr-xr-x   0        0        0    28112 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/business.py
--rwxr-xr-x   0        0        0    29206 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/c_like.py
--rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/capnproto.py
--rwxr-xr-x   0        0        0     3231 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/carbon.py
--rwxr-xr-x   0        0        0     5182 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cddl.py
--rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/chapel.py
--rwxr-xr-x   0        0        0     6395 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/clean.py
--rwxr-xr-x   0        0        0     3156 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/comal.py
--rwxr-xr-x   0        0        0     1407 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/compiled.py
--rwxr-xr-x   0        0        0    42338 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/configs.py
--rwxr-xr-x   0        0        0     4148 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/console.py
--rwxr-xr-x   0        0        0     1390 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cplint.py
--rwxr-xr-x   0        0        0    15756 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/crystal.py
--rwxr-xr-x   0        0        0    16994 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/csound.py
--rwxr-xr-x   0        0        0    25322 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/css.py
--rwxr-xr-x   0        0        0     9875 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/d.py
--rwxr-xr-x   0        0        0     4607 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dalvik.py
--rwxr-xr-x   0        0        0    26940 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/data.py
--rwxr-xr-x   0        0        0     8099 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dax.py
--rwxr-xr-x   0        0        0     4020 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/devicetree.py
--rwxr-xr-x   0        0        0     5278 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/diff.py
--rwxr-xr-x   0        0        0    37623 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dotnet.py
--rwxr-xr-x   0        0        0    36774 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dsls.py
--rwxr-xr-x   0        0        0    10380 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dylan.py
--rwxr-xr-x   0        0        0     6372 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ecl.py
--rwxr-xr-x   0        0        0     3152 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elm.py
--rwxr-xr-x   0        0        0     6370 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elpi.py
--rwxr-xr-x   0        0        0     4742 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/email.py
--rwxr-xr-x   0        0        0    19170 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/erlang.py
--rwxr-xr-x   0        0        0    10396 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/esoteric.py
--rwxr-xr-x   0        0        0     3273 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ezhil.py
--rwxr-xr-x   0        0        0    19531 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/factor.py
--rwxr-xr-x   0        0        0    10197 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fantom.py
--rwxr-xr-x   0        0        0     9646 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/felix.py
--rwxr-xr-x   0        0        0     1621 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fift.py
--rwxr-xr-x   0        0        0     2668 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/floscript.py
--rwxr-xr-x   0        0        0     7194 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/forth.py
--rwxr-xr-x   0        0        0    10336 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fortran.py
--rwxr-xr-x   0        0        0    26212 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/foxpro.py
--rwxr-xr-x   0        0        0    26914 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/freefem.py
--rwxr-xr-x   0        0        0     3622 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/func.py
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/functional.py
--rwxr-xr-x   0        0        0     3732 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/futhark.py
--rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gcodelexer.py
--rwxr-xr-x   0        0        0     7543 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gdscript.py
--rwxr-xr-x   0        0        0     7980 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/grammar_notation.py
--rwxr-xr-x   0        0        0     3861 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graph.py
--rwxr-xr-x   0        0        0    39026 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphics.py
--rwxr-xr-x   0        0        0     1935 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphviz.py
--rwxr-xr-x   0        0        0     3991 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gsql.py
--rwxr-xr-x   0        0        0    32898 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haskell.py
--rwxr-xr-x   0        0        0    30976 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haxe.py
--rwxr-xr-x   0        0        0    22520 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/hdl.py
--rwxr-xr-x   0        0        0    15450 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/idl.py
--rwxr-xr-x   0        0        0    30631 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/igor.py
--rwxr-xr-x   0        0        0     3136 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/inferno.py
--rwxr-xr-x   0        0        0    13178 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/installers.py
--rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/iolang.py
--rwxr-xr-x   0        0        0    62859 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/javascript.py
--rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jmespath.py
--rwxr-xr-x   0        0        0     3701 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jslt.py
--rwxr-xr-x   0        0        0     5635 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jsonnet.py
--rwxr-xr-x   0        0        0    11646 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/julia.py
--rwxr-xr-x   0        0        0    72929 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jvm.py
--rwxr-xr-x   0        0        0    11406 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/kuin.py
--rwxr-xr-x   0        0        0   144039 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/lisp.py
--rwxr-xr-x   0        0        0    31914 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/macaulay2.py
--rwxr-xr-x   0        0        0     7618 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/make.py
--rwxr-xr-x   0        0        0    58129 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/markup.py
--rwxr-xr-x   0        0        0      676 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/math.py
--rwxr-xr-x   0        0        0     2716 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/maxima.py
--rwxr-xr-x   0        0        0     4337 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/meson.py
--rwxr-xr-x   0        0        0    13846 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/minecraft.py
--rwxr-xr-x   0        0        0     4604 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mips.py
--rwxr-xr-x   0        0        0    13524 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modeling.py
--rwxr-xr-x   0        0        0    53073 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modula2.py
--rwxr-xr-x   0        0        0     6290 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/monte.py
--rwxr-xr-x   0        0        0     9187 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mosel.py
--rwxr-xr-x   0        0        0    63962 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ncl.py
--rwxr-xr-x   0        0        0     2726 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nit.py
--rwxr-xr-x   0        0        0     4015 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nix.py
--rwxr-xr-x   0        0        0     4169 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/oberon.py
--rwxr-xr-x   0        0        0    22961 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/objective.py
--rwxr-xr-x   0        0        0     2982 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ooc.py
--rwxr-xr-x   0        0        0     1744 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/other.py
--rwxr-xr-x   0        0        0     2720 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parasail.py
--rwxr-xr-x   0        0        0    25904 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parsers.py
--rwxr-xr-x   0        0        0     8146 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pawn.py
--rwxr-xr-x   0        0        0    39170 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/perl.py
--rwxr-xr-x   0        0        0    23252 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/phix.py
--rwxr-xr-x   0        0        0    13040 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/php.py
--rwxr-xr-x   0        0        0     1975 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pointless.py
--rwxr-xr-x   0        0        0    12677 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/praat.py
--rwxr-xr-x   0        0        0     1156 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/procfile.py
--rwxr-xr-x   0        0        0    12351 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/prolog.py
--rwxr-xr-x   0        0        0     4715 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/promql.py
--rwxr-xr-x   0        0        0    53376 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/python.py
--rwxr-xr-x   0        0        0     6072 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/qvt.py
--rwxr-xr-x   0        0        0     6185 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/r.py
--rwxr-xr-x   0        0        0    15790 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rdf.py
--rwxr-xr-x   0        0        0    18248 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rebol.py
--rwxr-xr-x   0        0        0     2902 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/resource.py
--rwxr-xr-x   0        0        0     5056 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ride.py
--rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rita.py
--rwxr-xr-x   0        0        0     1973 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rnc.py
--rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/roboconf.py
--rwxr-xr-x   0        0        0    18449 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/robotframework.py
--rwxr-xr-x   0        0        0    22775 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ruby.py
--rwxr-xr-x   0        0        0     8216 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rust.py
--rwxr-xr-x   0        0        0     9400 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sas.py
--rwxr-xr-x   0        0        0     4645 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/savi.py
--rwxr-xr-x   0        0        0     2239 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scdoc.py
--rwxr-xr-x   0        0        0    70014 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scripting.py
--rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sgf.py
--rwxr-xr-x   0        0        0    36466 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/shell.py
--rwxr-xr-x   0        0        0     2441 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sieve.py
--rwxr-xr-x   0        0        0     8482 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/slash.py
--rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smalltalk.py
--rwxr-xr-x   0        0        0     2660 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smithy.py
--rwxr-xr-x   0        0        0     2773 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smv.py
--rwxr-xr-x   0        0        0     2732 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/snobol.py
--rwxr-xr-x   0        0        0     3127 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/solidity.py
--rwxr-xr-x   0        0        0     3330 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sophia.py
--rwxr-xr-x   0        0        0     3414 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/special.py
--rwxr-xr-x   0        0        0     2733 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/spice.py
--rwxr-xr-x   0        0        0    42086 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sql.py
--rwxr-xr-x   0        0        0     3698 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/supercollider.py
--rwxr-xr-x   0        0        0     2639 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tal.py
--rwxr-xr-x   0        0        0     5513 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tcl.py
--rwxr-xr-x   0        0        0     3523 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teal.py
--rwxr-xr-x   0        0        0    72610 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/templates.py
--rwxr-xr-x   0        0        0     9719 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teraterm.py
--rwxr-xr-x   0        0        0    10767 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/testing.py
--rwxr-xr-x   0        0        0     1029 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/text.py
--rwxr-xr-x   0        0        0     7609 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textedit.py
--rwxr-xr-x   0        0        0    15192 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textfmts.py
--rwxr-xr-x   0        0        0    20157 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/theorem.py
--rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/thingsdb.py
--rwxr-xr-x   0        0        0     1377 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tlb.py
--rwxr-xr-x   0        0        0    10457 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tnt.py
--rwxr-xr-x   0        0        0     1474 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/trafficscript.py
--rwxr-xr-x   0        0        0     8207 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/typoscript.py
--rwxr-xr-x   0        0        0     8956 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ul4.py
--rwxr-xr-x   0        0        0    18512 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/unicon.py
--rwxr-xr-x   0        0        0     6037 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/urbi.py
--rwxr-xr-x   0        0        0     3513 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/usd.py
--rwxr-xr-x   0        0        0     7273 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/varnish.py
--rwxr-xr-x   0        0        0     3885 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/verification.py
--rwxr-xr-x   0        0        0      894 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/web.py
--rwxr-xr-x   0        0        0     5699 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webassembly.py
--rwxr-xr-x   0        0        0    10517 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webidl.py
--rwxr-xr-x   0        0        0    40549 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webmisc.py
--rwxr-xr-x   0        0        0    11920 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wgsl.py
--rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/whiley.py
--rwxr-xr-x   0        0        0     4021 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wowtoc.py
--rwxr-xr-x   0        0        0     3239 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wren.py
--rwxr-xr-x   0        0        0     1920 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/x10.py
--rwxr-xr-x   0        0        0      902 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/xorg.py
--rwxr-xr-x   0        0        0     4500 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/yang.py
--rwxr-xr-x   0        0        0     3953 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/zig.py
--rwxr-xr-x   0        0        0      491 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/__init__.py
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_compat.py
--rwxr-xr-x   0        0        0    11920 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_impl.py
--rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/__init__.py
--rwxr-xr-x   0        0        0    10927 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/_in_process.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1081 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     1171 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0     1119 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/__about__.py
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/__init__.py
--rwxr-xr-x   0        0        0      625 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/__main__.py
--rwxr-xr-x   0        0        0     4290 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/clean.py
--rwxr-xr-x   0        0        0     3595 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/markdown.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/py.typed
--rwxr-xr-x   0        0        0     4460 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/rst.py
--rwxr-xr-x   0        0        0      823 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/txt.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     9694 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/LICENSE
--rwxr-xr-x   0        0        0     2669 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/METADATA
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     4963 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/__init__.py
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/__version__.py
--rwxr-xr-x   0        0        0     1495 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/_internal_utils.py
--rwxr-xr-x   0        0        0    19553 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/adapters.py
--rwxr-xr-x   0        0        0     6449 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/api.py
--rwxr-xr-x   0        0        0    10187 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/auth.py
--rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/certs.py
--rwxr-xr-x   0        0        0     1451 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/compat.py
--rwxr-xr-x   0        0        0    18560 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/cookies.py
--rwxr-xr-x   0        0        0     3811 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/exceptions.py
--rwxr-xr-x   0        0        0     3875 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/help.py
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/hooks.py
--rwxr-xr-x   0        0        0    35223 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/models.py
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/packages.py
--rwxr-xr-x   0        0        0    30373 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/sessions.py
--rwxr-xr-x   0        0        0     4235 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/status_codes.py
--rwxr-xr-x   0        0        0     2912 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/structures.py
--rwxr-xr-x   0        0        0    33448 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/utils.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0    10142 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4634 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     2743 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/__init__.py
--rwxr-xr-x   0        0        0     9260 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/_compat.py
--rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/exceptions.py
--rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/sessions.py
--rwxr-xr-x   0        0        0     4044 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/streaming_iterator.py
--rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/__init__.py
--rwxr-xr-x   0        0        0     7539 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/appengine.py
--rwxr-xr-x   0        0        0     1404 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/fingerprint.py
--rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/host_header_ssl.py
--rwxr-xr-x   0        0        0     4789 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/socket_options.py
--rwxr-xr-x   0        0        0     2608 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/source.py
--rwxr-xr-x   0        0        0     2399 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/ssl.py
--rwxr-xr-x   0        0        0     7854 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/x509.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/__init__.py
--rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
--rwxr-xr-x   0        0        0     4944 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/guess.py
--rwxr-xr-x   0        0        0     4407 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/handler.py
--rwxr-xr-x   0        0        0     3706 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/http_proxy_digest.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/cookies/__init__.py
--rwxr-xr-x   0        0        0      213 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/cookies/forgetful.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/__init__.py
--rwxr-xr-x   0        0        0     6024 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/stream.py
--rwxr-xr-x   0        0        0     4365 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/tee.py
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/__init__.py
--rwxr-xr-x   0        0        0     4861 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/decoder.py
--rwxr-xr-x   0        0        0    20769 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/encoder.py
--rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/__init__.py
--rwxr-xr-x   0        0        0     6628 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/pool.py
--rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/thread.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/__init__.py
--rwxr-xr-x   0        0        0     2558 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/deprecated.py
--rwxr-xr-x   0        0        0     6522 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/dump.py
--rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/formdata.py
--rwxr-xr-x   0        0        0     4524 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/user_agent.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0    14638 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     6044 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     1565 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/__init__.py
--rwxr-xr-x   0        0        0    13297 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/_mixin.py
--rwxr-xr-x   0        0        0     9048 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/abnf_regexp.py
--rwxr-xr-x   0        0        0     3862 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/api.py
--rwxr-xr-x   0        0        0    12709 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/builder.py
--rwxr-xr-x   0        0        0     1620 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/compat.py
--rwxr-xr-x   0        0        0     3614 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/exceptions.py
--rwxr-xr-x   0        0        0     5477 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/iri.py
--rwxr-xr-x   0        0        0     4114 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/misc.py
--rwxr-xr-x   0        0        0     5261 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/normalizers.py
--rwxr-xr-x   0        0        0    14599 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/parseresult.py
--rwxr-xr-x   0        0        0     5183 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/uri.py
--rwxr-xr-x   0        0        0    13676 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/validators.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      564 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     6630 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     2072 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/RECORD
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/__init__.py
--rwxr-xr-x   0        0        0     8334 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/__main__.py
--rwxr-xr-x   0        0        0    10096 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_cell_widths.py
--rwxr-xr-x   0        0        0   140235 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_emoji_codes.py
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_emoji_replace.py
--rwxr-xr-x   0        0        0     2100 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_export_format.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_extension.py
--rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_fileno.py
--rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_inspect.py
--rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_log_render.py
--rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_loop.py
--rwxr-xr-x   0        0        0     1387 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_null_file.py
--rwxr-xr-x   0        0        0     7063 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_palettes.py
--rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_pick.py
--rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_ratio.py
--rwxr-xr-x   0        0        0    19919 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_spinners.py
--rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_stack.py
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_timer.py
--rwxr-xr-x   0        0        0    22784 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_win32_console.py
--rwxr-xr-x   0        0        0     1902 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_windows.py
--rwxr-xr-x   0        0        0     2759 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_windows_renderer.py
--rwxr-xr-x   0        0        0     1840 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_wrap.py
--rwxr-xr-x   0        0        0      878 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/abc.py
--rwxr-xr-x   0        0        0    10320 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/align.py
--rwxr-xr-x   0        0        0     6906 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/ansi.py
--rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/bar.py
--rwxr-xr-x   0        0        0     9794 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/box.py
--rwxr-xr-x   0        0        0     4509 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/cells.py
--rwxr-xr-x   0        0        0    18224 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/color.py
--rwxr-xr-x   0        0        0     1054 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/color_triplet.py
--rwxr-xr-x   0        0        0     7131 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/columns.py
--rwxr-xr-x   0        0        0    99146 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/console.py
--rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/constrain.py
--rwxr-xr-x   0        0        0     5497 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/containers.py
--rwxr-xr-x   0        0        0     6606 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/control.py
--rwxr-xr-x   0        0        0     8046 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/default_styles.py
--rwxr-xr-x   0        0        0      924 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/diagnose.py
--rwxr-xr-x   0        0        0     2465 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/emoji.py
--rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/errors.py
--rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/file_proxy.py
--rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/filesize.py
--rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/highlighter.py
--rwxr-xr-x   0        0        0     5020 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/json.py
--rwxr-xr-x   0        0        0     3228 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/jupyter.py
--rwxr-xr-x   0        0        0    13947 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/layout.py
--rwxr-xr-x   0        0        0    14273 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/live.py
--rwxr-xr-x   0        0        0     3655 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/live_render.py
--rwxr-xr-x   0        0        0    11891 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/logging.py
--rwxr-xr-x   0        0        0    26245 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/markdown.py
--rwxr-xr-x   0        0        0     8174 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/markup.py
--rwxr-xr-x   0        0        0     5305 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/measure.py
--rwxr-xr-x   0        0        0     4958 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/padding.py
--rwxr-xr-x   0        0        0      828 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/pager.py
--rwxr-xr-x   0        0        0     3288 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/palette.py
--rwxr-xr-x   0        0        0    10574 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/panel.py
--rwxr-xr-x   0        0        0    35816 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/pretty.py
--rwxr-xr-x   0        0        0    59694 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/progress.py
--rwxr-xr-x   0        0        0     8165 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/progress_bar.py
--rwxr-xr-x   0        0        0    11291 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/prompt.py
--rwxr-xr-x   0        0        0     1367 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/protocol.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/py.typed
--rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/region.py
--rwxr-xr-x   0        0        0     4419 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/repr.py
--rwxr-xr-x   0        0        0     4590 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/rule.py
--rwxr-xr-x   0        0        0     2831 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/scope.py
--rwxr-xr-x   0        0        0     1579 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/screen.py
--rwxr-xr-x   0        0        0    24211 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/segment.py
--rwxr-xr-x   0        0        0     4339 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/spinner.py
--rwxr-xr-x   0        0        0     4425 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/status.py
--rwxr-xr-x   0        0        0    27073 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/style.py
--rwxr-xr-x   0        0        0     1234 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/styled.py
--rwxr-xr-x   0        0        0    35065 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/syntax.py
--rwxr-xr-x   0        0        0    39648 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/table.py
--rwxr-xr-x   0        0        0     3370 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/terminal_theme.py
--rwxr-xr-x   0        0        0    45513 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/text.py
--rwxr-xr-x   0        0        0     3777 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/theme.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/themes.py
--rwxr-xr-x   0        0        0    29532 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/traceback.py
--rwxr-xr-x   0        0        0     9109 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/tree.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/LICENSE
--rwxr-xr-x   0        0        0    18837 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/METADATA
--rwxr-xr-x   0        0        0     9572 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/RECORD
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/WHEEL
--rwxr-xr-x   0        0        0     5700 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/__init__.py
--rwxr-xr-x   0        0        0     6592 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/archive_util.py
--rwxr-xr-x   0        0        0     5671 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/cli.exe
--rwxr-xr-x   0        0        0    16381 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/config.py
--rwxr-xr-x   0        0        0      935 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/dep_util.py
--rwxr-xr-x   0        0        0     5837 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/depends.py
--rwxr-xr-x   0        0        0    42522 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/dist.py
--rwxr-xr-x   0        0        0     1729 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/extension.py
--rwxr-xr-x   0        0        0     3146 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/glibc.py
--rwxr-xr-x   0        0        0     5207 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/gui.exe
--rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/launch.py
--rwxr-xr-x   0        0        0     2013 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/lib2to3_ex.py
--rwxr-xr-x   0        0        0     5789 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/monkey.py
--rwxr-xr-x   0        0        0    40877 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/msvc.py
--rwxr-xr-x   0        0        0     3199 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/namespaces.py
--rwxr-xr-x   0        0        0    40153 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/package_index.py
--rwxr-xr-x   0        0        0    10882 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/pep425tags.py
--rwxr-xr-x   0        0        0      536 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py27compat.py
--rwxr-xr-x   0        0        0     1192 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py31compat.py
--rwxr-xr-x   0        0        0     1182 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py33compat.py
--rwxr-xr-x   0        0        0     2891 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py36compat.py
--rwxr-xr-x   0        0        0    14276 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/sandbox.py
--rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/script (dev).tmpl
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/script.tmpl
--rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/site-patch.py
--rwxr-xr-x   0        0        0     8492 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/ssl_support.py
--rwxr-xr-x   0        0        0      996 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/unicode_utils.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/version.py
--rwxr-xr-x   0        0        0     7230 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/wheel.py
--rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/windows_support.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/__init__.py
--rwxr-xr-x   0        0        0   229867 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0    30098 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/six.py
--rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0      860 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_compat.py
--rwxr-xr-x   0        0        0     1416 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     8239 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4343 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    28025 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    11556 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0      594 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/__init__.py
--rwxr-xr-x   0        0        0     2426 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/alias.py
--rwxr-xr-x   0        0        0    18185 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_egg.py
--rwxr-xr-x   0        0        0     1508 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_rpm.py
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_wininst.py
--rwxr-xr-x   0        0        0     4484 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_clib.py
--rwxr-xr-x   0        0        0    13173 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_ext.py
--rwxr-xr-x   0        0        0     9596 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_py.py
--rwxr-xr-x   0        0        0     8046 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/develop.py
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/dist_info.py
--rwxr-xr-x   0        0        0    89413 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/easy_install.py
--rwxr-xr-x   0        0        0    24808 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/egg_info.py
--rwxr-xr-x   0        0        0     4683 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install.py
--rwxr-xr-x   0        0        0     3195 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_egg_info.py
--rwxr-xr-x   0        0        0     5012 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_lib.py
--rwxr-xr-x   0        0        0     2439 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_scripts.py
--rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/launcher manifest.xml
--rwxr-xr-x   0        0        0     4986 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/py36compat.py
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/register.py
--rwxr-xr-x   0        0        0     2164 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/rotate.py
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/saveopts.py
--rwxr-xr-x   0        0        0     6711 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/sdist.py
--rwxr-xr-x   0        0        0     5085 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/setopt.py
--rwxr-xr-x   0        0        0     9214 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/test.py
--rwxr-xr-x   0        0        0     1172 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload.py
--rwxr-xr-x   0        0        0     7311 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload_docs.py
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/extern/__init__.py
--rwxr-xr-x   0        0        0     1422 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/DESCRIPTION.rst
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/METADATA
--rwxr-xr-x   0        0        0    11362 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/RECORD
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/dependency_links.txt
--rwxr-xr-x   0        0        0     2934 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/metadata.json
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/zip-safe
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/METADATA
--rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/RECORD
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli/__init__.py
--rwxr-xr-x   0        0        0    22633 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli/_parser.py
--rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli/_re.py
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli/_types.py
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli/py.typed
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/LICENSE
--rwxr-xr-x   0        0        0     8875 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/METADATA
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/__init__.py
--rwxr-xr-x   0        0        0     1475 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/__main__.py
--rwxr-xr-x   0        0        0     3129 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/auth.py
--rwxr-xr-x   0        0        0     3738 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/cli.py
--rwxr-xr-x   0        0        0     3814 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/exceptions.py
--rwxr-xr-x   0        0        0    11024 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/package.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/py.typed
--rwxr-xr-x   0        0        0     8713 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/repository.py
--rwxr-xr-x   0        0        0    12269 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/settings.py
--rwxr-xr-x   0        0        0    10867 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/utils.py
--rwxr-xr-x   0        0        0     3049 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/wheel.py
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/wininst.py
--rwxr-xr-x   0        0        0     1802 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/__init__.py
--rwxr-xr-x   0        0        0     5727 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/check.py
--rwxr-xr-x   0        0        0     2904 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/register.py
--rwxr-xr-x   0        0        0     7469 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/upload.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/LICENSE
--rwxr-xr-x   0        0        0     3259 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/METADATA
--rwxr-xr-x   0        0        0     2630 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/RECORD
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/REQUESTED
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/WHEEL
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/top_level.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0    13936 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/METADATA
--rwxr-xr-x   0        0        0      565 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0    10676 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp/__init__.py
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp/py310compat.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     3735 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/METADATA
--rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0        5 2020-02-02 00:00:00.000000 pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.0.1/LICENSE
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 pyswxf-0.0.1/README.md
--rwxr-xr-x   0        0        0      598 2020-02-02 00:00:00.000000 pyswxf-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pyswxf-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/src/pySWXF/__init__.py
+-rwxr-xr-x   0        0        0     3536 2020-02-02 00:00:00.000000 pyswxf-0.0.2/src/pySWXF/refl_funs.py
+-rwxr-xr-x   0        0        0     3532 2020-02-02 00:00:00.000000 pyswxf-0.0.2/src/pySWXF/standing_wave.py
+-rwxr-xr-x   0        0        0      914 2020-02-02 00:00:00.000000 pyswxf-0.0.2/src/pySWXF/xray_utils.py
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/pyvenv.cfg
+-rwxr-xr-x   0        0        0     2273 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/activate
+-rwxr-xr-x   0        0        0     1325 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/activate.csh
+-rwxr-xr-x   0        0        0     2477 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/activate.fish
+-rwxr-xr-x   0        0        0      324 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/docutils
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/easy_install
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/easy_install-3.7
+-rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/keyring
+-rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/markdown-it
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/normalizer
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/pip
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/pip3
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/pip3.10
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/pip3.7
+-rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/pkginfo
+-rwxr-xr-x   0        0        0      323 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/pygmentize
+-rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/python3 -> /usr/bin/python3
+-rwxr-xr-x   0        0        0      675 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2html.py
+-rwxr-xr-x   0        0        0      797 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      874 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      697 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2man.py
+-rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      682 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      683 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      751 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/bin/twine
+-rwxr-xr-x   0        0        0   932624 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/_cffi_backend.cpython-37m-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/easy_install.py
+-rwxr-xr-x   0        0        0   110349 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1504 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4027 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       14 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     3649 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/__init__.py
+-rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/callbacks.py
+-rwxr-xr-x   0        0        0     2526 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/css_sanitizer.py
+-rwxr-xr-x   0        0        0    22779 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/html5lib_shim.py
+-rwxr-xr-x   0        0        0    22350 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/linkifier.py
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/parse_shim.py
+-rwxr-xr-x   0        0        0    21934 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/sanitizer.py
+-rwxr-xr-x   0        0        0     2160 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/README.rst
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/__init__.py
+-rwxr-xr-x   0        0        0    39023 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/parse.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/parse.py.SHA256SUM
+-rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/vendor.txt
+-rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/vendor_install.sh
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/__init__.py
+-rwxr-xr-x   0        0        0    16728 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_ihatexml.py
+-rwxr-xr-x   0        0        0    32300 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_inputstream.py
+-rwxr-xr-x   0        0        0    77028 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_tokenizer.py
+-rwxr-xr-x   0        0        0     4919 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_utils.py
+-rwxr-xr-x   0        0        0    83464 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/constants.py
+-rwxr-xr-x   0        0        0   117174 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/html5parser.py
+-rwxr-xr-x   0        0        0    15747 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/serializer.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
+-rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/_base.py
+-rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/py.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/__init__.py
+-rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/base.py
+-rwxr-xr-x   0        0        0     2945 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
+-rwxr-xr-x   0        0        0     3631 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/lint.py
+-rwxr-xr-x   0        0        0    10588 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
+-rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
+-rwxr-xr-x   0        0        0     1214 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
+-rwxr-xr-x   0        0        0     1715 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
+-rwxr-xr-x   0        0        0     1776 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
+-rwxr-xr-x   0        0        0     3592 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
+-rwxr-xr-x   0        0        0    14553 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
+-rwxr-xr-x   0        0        0     8925 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
+-rwxr-xr-x   0        0        0    12824 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
+-rwxr-xr-x   0        0        0    14754 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
+-rwxr-xr-x   0        0        0     5719 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
+-rwxr-xr-x   0        0        0     7476 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
+-rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
+-rwxr-xr-x   0        0        0     4539 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
+-rwxr-xr-x   0        0        0     6345 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
+-rwxr-xr-x   0        0        0     2309 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
+-rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    16076 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0     3486 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/REQUESTED
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      569 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    29799 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     8456 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0    19190 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/__init__.py
+-rwxr-xr-x   0        0        0    12200 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/__main__.py
+-rwxr-xr-x   0        0        0    12636 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/env.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/py.typed
+-rwxr-xr-x   0        0        0     1632 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/util.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4071 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1052 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1006 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/__init__.py
+-rwxr-xr-x   0        0        0     3908 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_errors.h
+-rwxr-xr-x   0        0        0    14800 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_include.h
+-rwxr-xr-x   0        0        0    17680 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/_embedding.h
+-rwxr-xr-x   0        0        0    42064 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/api.py
+-rwxr-xr-x   0        0        0    42454 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/backend_ctypes.py
+-rwxr-xr-x   0        0        0     5724 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/cffi_opcode.py
+-rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/commontypes.py
+-rwxr-xr-x   0        0        0    44231 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/cparser.py
+-rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/error.py
+-rwxr-xr-x   0        0        0     4046 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/ffiplatform.py
+-rwxr-xr-x   0        0        0      747 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/lock.py
+-rwxr-xr-x   0        0        0    21768 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/model.py
+-rwxr-xr-x   0        0        0     5976 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/parse_c_type.h
+-rwxr-xr-x   0        0        0     4374 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/pkgconfig.py
+-rwxr-xr-x   0        0        0    64598 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/recompiler.py
+-rwxr-xr-x   0        0        0     8931 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/setuptools_ext.py
+-rwxr-xr-x   0        0        0    43320 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/vengine_cpy.py
+-rwxr-xr-x   0        0        0    26684 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/vengine_gen.py
+-rwxr-xr-x   0        0        0    11253 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/verifier.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1294 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1144 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2897 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/__init__.py
+-rwxr-xr-x   0        0        0    18624 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/api.py
+-rwxr-xr-x   0        0        0    12554 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cd.py
+-rwxr-xr-x   0        0        0    19101 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/constant.py
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/legacy.py
+-rwxr-xr-x   0        0        0    17144 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.cpython-37m-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    18258 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.py
+-rwxr-xr-x   0        0        0   344664 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md__mypyc.cpython-37m-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    11492 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/models.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/py.typed
+-rwxr-xr-x   0        0        0    11544 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/utils.py
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/version.py
+-rwxr-xr-x   0        0        0    20069 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/assets/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cli/__init__.py
+-rwxr-xr-x   0        0        0     9744 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cli/normalizer.py
+-rwxr-xr-x   0        0        0      445 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/__about__.py
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/__init__.py
+-rwxr-xr-x   0        0        0     1118 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/exceptions.py
+-rwxr-xr-x   0        0        0     6886 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/fernet.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/py.typed
+-rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/utils.py
+-rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/__init__.py
+-rwxr-xr-x   0        0        0    14441 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/_oid.py
+-rwxr-xr-x   0        0        0      361 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/__init__.py
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/__init__.py
+-rwxr-xr-x   0        0        0    15967 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/aead.py
+-rwxr-xr-x   0        0        0    73231 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/backend.py
+-rwxr-xr-x   0        0        0    10358 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ciphers.py
+-rwxr-xr-x   0        0        0     3035 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/cmac.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/decode_asn1.py
+-rwxr-xr-x   0        0        0    11474 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ec.py
+-rwxr-xr-x   0        0        0    21825 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/rsa.py
+-rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/utils.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/__init__.py
+-rwxr-xr-x   0        0        0 13408352 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust.abi3.so
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/__init__.pyi
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/_openssl.pyi
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/asn1.pyi
+-rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/exceptions.pyi
+-rwxr-xr-x   0        0        0      905 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/ocsp.pyi
+-rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/pkcs7.pyi
+-rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/x509.pyi
+-rwxr-xr-x   0        0        0      970 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
+-rwxr-xr-x   0        0        0      896 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
+-rwxr-xr-x   0        0        0      764 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
+-rwxr-xr-x   0        0        0      629 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
+-rwxr-xr-x   0        0        0      603 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
+-rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
+-rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
+-rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
+-rwxr-xr-x   0        0        0      616 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
+-rwxr-xr-x   0        0        0      590 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/__init__.py
+-rwxr-xr-x   0        0        0     9098 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/_conditional.py
+-rwxr-xr-x   0        0        0     6696 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/binding.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/__init__.py
+-rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_asymmetric.py
+-rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_cipheralgorithm.py
+-rwxr-xr-x   0        0        0     5216 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_serialization.py
+-rwxr-xr-x   0        0        0     2065 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/cmac.py
+-rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/constant_time.py
+-rwxr-xr-x   0        0        0     5115 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/hashes.py
+-rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/hmac.py
+-rwxr-xr-x   0        0        0     5678 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/keywrap.py
+-rwxr-xr-x   0        0        0     6242 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/padding.py
+-rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/poly1305.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/__init__.py
+-rwxr-xr-x   0        0        0     7013 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dh.py
+-rwxr-xr-x   0        0        0     8263 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dsa.py
+-rwxr-xr-x   0        0        0    12867 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ec.py
+-rwxr-xr-x   0        0        0     3489 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed25519.py
+-rwxr-xr-x   0        0        0     3440 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed448.py
+-rwxr-xr-x   0        0        0     2717 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/padding.py
+-rwxr-xr-x   0        0        0    11623 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/rsa.py
+-rwxr-xr-x   0        0        0     2996 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/types.py
+-rwxr-xr-x   0        0        0      790 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/utils.py
+-rwxr-xr-x   0        0        0     3437 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x25519.py
+-rwxr-xr-x   0        0        0     3358 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x448.py
+-rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/__init__.py
+-rwxr-xr-x   0        0        0    12067 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/aead.py
+-rwxr-xr-x   0        0        0     5000 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/algorithms.py
+-rwxr-xr-x   0        0        0     8286 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/base.py
+-rwxr-xr-x   0        0        0     8361 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/modes.py
+-rwxr-xr-x   0        0        0      750 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/__init__.py
+-rwxr-xr-x   0        0        0     3726 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/concatkdf.py
+-rwxr-xr-x   0        0        0     3045 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/hkdf.py
+-rwxr-xr-x   0        0        0     9232 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/kbkdf.py
+-rwxr-xr-x   0        0        0     2012 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/pbkdf2.py
+-rwxr-xr-x   0        0        0     2354 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/scrypt.py
+-rwxr-xr-x   0        0        0     2002 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/x963kdf.py
+-rwxr-xr-x   0        0        0     1653 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/__init__.py
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/base.py
+-rwxr-xr-x   0        0        0     6767 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs12.py
+-rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs7.py
+-rwxr-xr-x   0        0        0    50088 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/ssh.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/__init__.py
+-rwxr-xr-x   0        0        0     3010 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/hotp.py
+-rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/totp.py
+-rwxr-xr-x   0        0        0     7870 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/__init__.py
+-rwxr-xr-x   0        0        0    35677 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/base.py
+-rwxr-xr-x   0        0        0     2261 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/certificate_transparency.py
+-rwxr-xr-x   0        0        0    68365 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/extensions.py
+-rwxr-xr-x   0        0        0     7868 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/general_name.py
+-rwxr-xr-x   0        0        0    14855 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/name.py
+-rwxr-xr-x   0        0        0    18534 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/ocsp.py
+-rwxr-xr-x   0        0        0      829 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/oid.py
+-rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/COPYING.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     2817 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0    28033 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0    30724 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/__init__.py
+-rwxr-xr-x   0        0        0     2454 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_adapters.py
+-rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_collections.py
+-rwxr-xr-x   0        0        0     1735 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_compat.py
+-rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_functools.py
+-rwxr-xr-x   0        0        0     2068 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_itertools.py
+-rwxr-xr-x   0        0        0     1615 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_meta.py
+-rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_py39compat.py
+-rwxr-xr-x   0        0        0     2166 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_text.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/py.typed
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0    11358 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4878 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1952 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco/classes/__init__.py
+-rwxr-xr-x   0        0        0     1464 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco/classes/ancestry.py
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco/classes/meta.py
+-rwxr-xr-x   0        0        0     3996 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco/classes/properties.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1065 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/__init__.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/__main__.py
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/_compat.py
+-rwxr-xr-x   0        0        0     3886 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/_properties_compat.py
+-rwxr-xr-x   0        0        0     8100 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backend.py
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backend_complete.zsh
+-rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/cli.py
+-rwxr-xr-x   0        0        0     1324 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/completion.py
+-rwxr-xr-x   0        0        0     5731 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/core.py
+-rwxr-xr-x   0        0        0     1593 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/credentials.py
+-rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/devpi_client.py
+-rwxr-xr-x   0        0        0     1430 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/errors.py
+-rwxr-xr-x   0        0        0     1231 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/http.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/py.typed
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/py312compat.py
+-rwxr-xr-x   0        0        0     4692 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/SecretService.py
+-rwxr-xr-x   0        0        0     5814 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/Windows.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/__init__.py
+-rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/chainer.py
+-rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/fail.py
+-rwxr-xr-x   0        0        0     5830 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/kwallet.py
+-rwxr-xr-x   0        0        0     5982 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/libsecret.py
+-rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/null.py
+-rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/__init__.py
+-rwxr-xr-x   0        0        0     4341 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/api.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/testing/__init__.py
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/testing/backend.py
+-rwxr-xr-x   0        0        0     1918 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/testing/util.py
+-rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/util/__init__.py
+-rwxr-xr-x   0        0        0     2215 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/util/platform_.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1023 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    20512 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0     4527 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/__init__.py
+-rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/_compat.py
+-rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/_punycode.py
+-rwxr-xr-x   0        0        0    12228 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/main.py
+-rwxr-xr-x   0        0        0     3662 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_block.py
+-rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_core.py
+-rwxr-xr-x   0        0        0     4130 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_inline.py
+-rwxr-xr-x   0        0        0     2516 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/port.yaml
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/py.typed
+-rwxr-xr-x   0        0        0    10041 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/renderer.py
+-rwxr-xr-x   0        0        0     8376 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/ruler.py
+-rwxr-xr-x   0        0        0     6374 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/token.py
+-rwxr-xr-x   0        0        0    11052 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/tree.py
+-rwxr-xr-x   0        0        0     3262 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/utils.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/cli/__init__.py
+-rwxr-xr-x   0        0        0     2901 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/cli/parse.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/__init__.py
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/entities.py
+-rwxr-xr-x   0        0        0      932 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_blocks.py
+-rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_re.py
+-rwxr-xr-x   0        0        0     2631 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/normalize_url.py
+-rwxr-xr-x   0        0        0    10894 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/utils.py
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/__init__.py
+-rwxr-xr-x   0        0        0     1953 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_destination.py
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_label.py
+-rwxr-xr-x   0        0        0     1410 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_title.py
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/__init__.py
+-rwxr-xr-x   0        0        0     2809 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/commonmark.py
+-rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/default.py
+-rwxr-xr-x   0        0        0     2006 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/zero.py
+-rwxr-xr-x   0        0        0      553 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/__init__.py
+-rwxr-xr-x   0        0        0     9057 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/blockquote.py
+-rwxr-xr-x   0        0        0      886 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/code.py
+-rwxr-xr-x   0        0        0     2704 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/fence.py
+-rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/heading.py
+-rwxr-xr-x   0        0        0     1309 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/hr.py
+-rwxr-xr-x   0        0        0     2808 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/html_block.py
+-rwxr-xr-x   0        0        0     2798 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/lheading.py
+-rwxr-xr-x   0        0        0     9944 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/list.py
+-rwxr-xr-x   0        0        0     1851 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/paragraph.py
+-rwxr-xr-x   0        0        0     6323 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/reference.py
+-rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/state_block.py
+-rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/table.py
+-rwxr-xr-x   0        0        0      344 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/__init__.py
+-rwxr-xr-x   0        0        0      413 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/block.py
+-rwxr-xr-x   0        0        0      325 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/inline.py
+-rwxr-xr-x   0        0        0     4833 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/linkify.py
+-rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/normalize.py
+-rwxr-xr-x   0        0        0     3560 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/replacements.py
+-rwxr-xr-x   0        0        0     7251 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/smartquotes.py
+-rwxr-xr-x   0        0        0      584 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/state_core.py
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/__init__.py
+-rwxr-xr-x   0        0        0     2131 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/autolink.py
+-rwxr-xr-x   0        0        0     2112 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/backticks.py
+-rwxr-xr-x   0        0        0     4062 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rwxr-xr-x   0        0        0     2948 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/emphasis.py
+-rwxr-xr-x   0        0        0     1653 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/entity.py
+-rwxr-xr-x   0        0        0     1116 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/escape.py
+-rwxr-xr-x   0        0        0     1019 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/html_inline.py
+-rwxr-xr-x   0        0        0     4260 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/image.py
+-rwxr-xr-x   0        0        0     4362 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/link.py
+-rwxr-xr-x   0        0        0     1176 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/newline.py
+-rwxr-xr-x   0        0        0     5388 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/state_inline.py
+-rwxr-xr-x   0        0        0     3390 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/strikethrough.py
+-rwxr-xr-x   0        0        0     1427 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text.py
+-rwxr-xr-x   0        0        0     1491 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text_collapse.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1078 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it
+-rwxr-xr-x   0        0        0     6812 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0    10448 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     2338 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1638 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      501 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/__init__.py
+-rwxr-xr-x   0        0        0     3266 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_elffile.py
+-rwxr-xr-x   0        0        0     8926 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_manylinux.py
+-rwxr-xr-x   0        0        0     2524 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_musllinux.py
+-rwxr-xr-x   0        0        0    10194 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_parser.py
+-rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_structures.py
+-rwxr-xr-x   0        0        0     5292 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_tokenizer.py
+-rwxr-xr-x   0        0        0     8208 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/markers.py
+-rwxr-xr-x   0        0        0    16397 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/metadata.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/py.typed
+-rwxr-xr-x   0        0        0     3287 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/requirements.py
+-rwxr-xr-x   0        0        0    39206 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/specifiers.py
+-rwxr-xr-x   0        0        0    18106 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/tags.py
+-rwxr-xr-x   0        0        0     4355 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/utils.py
+-rwxr-xr-x   0        0        0    16326 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/version.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    10174 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.APACHE
+-rwxr-xr-x   0        0        0     1344 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.BSD
+-rwxr-xr-x   0        0        0     3082 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2461 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/__init__.py
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/__main__.py
+-rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/__pip-runner__.py
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/py.typed
+-rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/__init__.py
+-rwxr-xr-x   0        0        0    10243 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/build_env.py
+-rwxr-xr-x   0        0        0     9661 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cache.py
+-rwxr-xr-x   0        0        0    13529 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/configuration.py
+-rwxr-xr-x   0        0        0    23741 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/exceptions.py
+-rwxr-xr-x   0        0        0      340 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/main.py
+-rwxr-xr-x   0        0        0     7161 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/pyproject.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/self_outdated_check.py
+-rwxr-xr-x   0        0        0    11842 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/wheel_builder.py
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/__init__.py
+-rwxr-xr-x   0        0        0     6676 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/autocompletion.py
+-rwxr-xr-x   0        0        0     8176 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/base_command.py
+-rwxr-xr-x   0        0        0    30030 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/cmdoptions.py
+-rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/command_context.py
+-rwxr-xr-x   0        0        0     2816 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main.py
+-rwxr-xr-x   0        0        0     4338 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main_parser.py
+-rwxr-xr-x   0        0        0    10817 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/parser.py
+-rwxr-xr-x   0        0        0     1968 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/progress_bars.py
+-rwxr-xr-x   0        0        0    18328 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/req_command.py
+-rwxr-xr-x   0        0        0     5118 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/spinners.py
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/status_codes.py
+-rwxr-xr-x   0        0        0     3882 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/__init__.py
+-rwxr-xr-x   0        0        0     7581 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/cache.py
+-rwxr-xr-x   0        0        0     1684 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/check.py
+-rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/completion.py
+-rwxr-xr-x   0        0        0     9815 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/configuration.py
+-rwxr-xr-x   0        0        0     6591 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/debug.py
+-rwxr-xr-x   0        0        0     5182 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/download.py
+-rwxr-xr-x   0        0        0     2951 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/freeze.py
+-rwxr-xr-x   0        0        0     1703 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/hash.py
+-rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/help.py
+-rwxr-xr-x   0        0        0     4793 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/index.py
+-rwxr-xr-x   0        0        0     3188 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/inspect.py
+-rwxr-xr-x   0        0        0    28722 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/install.py
+-rwxr-xr-x   0        0        0    12343 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/list.py
+-rwxr-xr-x   0        0        0     5697 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/search.py
+-rwxr-xr-x   0        0        0     6419 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/show.py
+-rwxr-xr-x   0        0        0     3886 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/uninstall.py
+-rwxr-xr-x   0        0        0     6324 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/wheel.py
+-rwxr-xr-x   0        0        0      858 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/__init__.py
+-rwxr-xr-x   0        0        0     1221 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/base.py
+-rwxr-xr-x   0        0        0      729 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/installed.py
+-rwxr-xr-x   0        0        0     6494 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/sdist.py
+-rwxr-xr-x   0        0        0     1164 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/wheel.py
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/__init__.py
+-rwxr-xr-x   0        0        0    16504 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/collector.py
+-rwxr-xr-x   0        0        0    37873 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/package_finder.py
+-rwxr-xr-x   0        0        0     6556 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/sources.py
+-rwxr-xr-x   0        0        0    15365 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/__init__.py
+-rwxr-xr-x   0        0        0     6100 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_distutils.py
+-rwxr-xr-x   0        0        0     7680 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_sysconfig.py
+-rwxr-xr-x   0        0        0     2556 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/base.py
+-rwxr-xr-x   0        0        0     4280 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/__init__.py
+-rwxr-xr-x   0        0        0     2595 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/_json.py
+-rwxr-xr-x   0        0        0    25277 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/base.py
+-rwxr-xr-x   0        0        0     9773 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/pkg_resources.py
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rwxr-xr-x   0        0        0     8181 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rwxr-xr-x   0        0        0     7457 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/__init__.py
+-rwxr-xr-x   0        0        0      990 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/candidate.py
+-rwxr-xr-x   0        0        0     6931 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/direct_url.py
+-rwxr-xr-x   0        0        0     2520 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/format_control.py
+-rwxr-xr-x   0        0        0     1030 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/index.py
+-rwxr-xr-x   0        0        0     2619 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/installation_report.py
+-rwxr-xr-x   0        0        0    18817 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/link.py
+-rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/scheme.py
+-rwxr-xr-x   0        0        0     4643 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/search_scope.py
+-rwxr-xr-x   0        0        0     1907 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/selection_prefs.py
+-rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/target_python.py
+-rwxr-xr-x   0        0        0     3600 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/wheel.py
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/__init__.py
+-rwxr-xr-x   0        0        0    20435 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/auth.py
+-rwxr-xr-x   0        0        0     2145 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/cache.py
+-rwxr-xr-x   0        0        0     6096 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/download.py
+-rwxr-xr-x   0        0        0     7638 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/lazy_wheel.py
+-rwxr-xr-x   0        0        0    18442 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/session.py
+-rwxr-xr-x   0        0        0     4073 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/utils.py
+-rwxr-xr-x   0        0        0     1791 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/xmlrpc.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/__init__.py
+-rwxr-xr-x   0        0        0     5122 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/check.py
+-rwxr-xr-x   0        0        0     9816 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/freeze.py
+-rwxr-xr-x   0        0        0    27696 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/prepare.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/__init__.py
+-rwxr-xr-x   0        0        0     4133 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/build_tracker.py
+-rwxr-xr-x   0        0        0     1422 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata.py
+-rwxr-xr-x   0        0        0     1474 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rwxr-xr-x   0        0        0     2198 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rwxr-xr-x   0        0        0     1075 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel.py
+-rwxr-xr-x   0        0        0     1417 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rwxr-xr-x   0        0        0     3064 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/__init__.py
+-rwxr-xr-x   0        0        0     1282 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rwxr-xr-x   0        0        0    27475 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/wheel.py
+-rwxr-xr-x   0        0        0     2738 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/__init__.py
+-rwxr-xr-x   0        0        0    16610 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/constructors.py
+-rwxr-xr-x   0        0        0    17872 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_file.py
+-rwxr-xr-x   0        0        0    32782 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_install.py
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_set.py
+-rwxr-xr-x   0        0        0    24678 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_uninstall.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/__init__.py
+-rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/base.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rwxr-xr-x   0        0        0    24128 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rwxr-xr-x   0        0        0     5220 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rwxr-xr-x   0        0        0    18864 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rwxr-xr-x   0        0        0    27845 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rwxr-xr-x   0        0        0     5705 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rwxr-xr-x   0        0        0     9824 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rwxr-xr-x   0        0        0     3094 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rwxr-xr-x   0        0        0     5454 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rwxr-xr-x   0        0        0    11538 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/__init__.py
+-rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_jaraco_text.py
+-rwxr-xr-x   0        0        0     1015 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_log.py
+-rwxr-xr-x   0        0        0     1665 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/appdirs.py
+-rwxr-xr-x   0        0        0     1884 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compat.py
+-rwxr-xr-x   0        0        0     5377 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compatibility_tags.py
+-rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/datetime.py
+-rwxr-xr-x   0        0        0     3627 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/deprecation.py
+-rwxr-xr-x   0        0        0     3206 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rwxr-xr-x   0        0        0     2118 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/egg_link.py
+-rwxr-xr-x   0        0        0     1169 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/encoding.py
+-rwxr-xr-x   0        0        0     3064 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/entrypoints.py
+-rwxr-xr-x   0        0        0     5122 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filesystem.py
+-rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filetypes.py
+-rwxr-xr-x   0        0        0     3110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/glibc.py
+-rwxr-xr-x   0        0        0     5118 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/hashes.py
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/inject_securetransport.py
+-rwxr-xr-x   0        0        0    11632 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/logging.py
+-rwxr-xr-x   0        0        0    22216 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/misc.py
+-rwxr-xr-x   0        0        0     1193 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/models.py
+-rwxr-xr-x   0        0        0     2108 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/packaging.py
+-rwxr-xr-x   0        0        0     4435 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/setuptools_build.py
+-rwxr-xr-x   0        0        0     9200 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/subprocess.py
+-rwxr-xr-x   0        0        0     7702 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/temp_dir.py
+-rwxr-xr-x   0        0        0     8821 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/unpacking.py
+-rwxr-xr-x   0        0        0     1759 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/urls.py
+-rwxr-xr-x   0        0        0     3456 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/virtualenv.py
+-rwxr-xr-x   0        0        0     4549 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/wheel.py
+-rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/__init__.py
+-rwxr-xr-x   0        0        0     3519 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/bazaar.py
+-rwxr-xr-x   0        0        0    18116 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/git.py
+-rwxr-xr-x   0        0        0     5238 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/mercurial.py
+-rwxr-xr-x   0        0        0    11729 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/subversion.py
+-rwxr-xr-x   0        0        0    22811 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/versioncontrol.py
+-rwxr-xr-x   0        0        0     4966 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/__init__.py
+-rwxr-xr-x   0        0        0    34549 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/six.py
+-rwxr-xr-x   0        0        0    84101 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/typing_extensions.py
+-rwxr-xr-x   0        0        0      476 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/vendor.txt
+-rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rwxr-xr-x   0        0        0     1379 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rwxr-xr-x   0        0        0     5033 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rwxr-xr-x   0        0        0     1535 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/cache.py
+-rwxr-xr-x   0        0        0      778 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/compat.py
+-rwxr-xr-x   0        0        0    16416 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/controller.py
+-rwxr-xr-x   0        0        0     3946 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rwxr-xr-x   0        0        0     4154 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rwxr-xr-x   0        0        0     7105 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rwxr-xr-x   0        0        0     5271 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rwxr-xr-x   0        0        0     1033 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/__init__.py
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/__main__.py
+-rwxr-xr-x   0        0        0   275233 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/cacert.pem
+-rwxr-xr-x   0        0        0     4279 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/core.py
+-rwxr-xr-x   0        0        0     4797 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/__init__.py
+-rwxr-xr-x   0        0        0    31274 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5freq.py
+-rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5prober.py
+-rwxr-xr-x   0        0        0    10032 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/chardistribution.py
+-rwxr-xr-x   0        0        0     3915 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rwxr-xr-x   0        0        0     5420 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetprober.py
+-rwxr-xr-x   0        0        0     3732 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rwxr-xr-x   0        0        0      542 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cp949prober.py
+-rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/enums.py
+-rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escprober.py
+-rwxr-xr-x   0        0        0    12176 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escsm.py
+-rwxr-xr-x   0        0        0     3934 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rwxr-xr-x   0        0        0    13566 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rwxr-xr-x   0        0        0     1753 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrprober.py
+-rwxr-xr-x   0        0        0    36913 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rwxr-xr-x   0        0        0     1753 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwprober.py
+-rwxr-xr-x   0        0        0    20735 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rwxr-xr-x   0        0        0     1759 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rwxr-xr-x   0        0        0    14537 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rwxr-xr-x   0        0        0    25796 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jisfreq.py
+-rwxr-xr-x   0        0        0    42498 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabfreq.py
+-rwxr-xr-x   0        0        0     1752 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabprober.py
+-rwxr-xr-x   0        0        0    27055 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jpcntx.py
+-rwxr-xr-x   0        0        0   104562 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rwxr-xr-x   0        0        0    98484 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rwxr-xr-x   0        0        0    98196 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rwxr-xr-x   0        0        0   101363 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rwxr-xr-x   0        0        0   128035 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rwxr-xr-x   0        0        0   102774 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rwxr-xr-x   0        0        0    95372 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rwxr-xr-x   0        0        0     5380 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/latin1prober.py
+-rwxr-xr-x   0        0        0     6077 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/macromanprober.py
+-rwxr-xr-x   0        0        0     3715 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rwxr-xr-x   0        0        0     2131 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rwxr-xr-x   0        0        0    30391 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcssm.py
+-rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/resultdict.py
+-rwxr-xr-x   0        0        0     6400 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rwxr-xr-x   0        0        0     4137 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rwxr-xr-x   0        0        0     4007 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sjisprober.py
+-rwxr-xr-x   0        0        0    14848 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/universaldetector.py
+-rwxr-xr-x   0        0        0     8505 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rwxr-xr-x   0        0        0     2812 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf8prober.py
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/version.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rwxr-xr-x   0        0        0     3242 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rwxr-xr-x   0        0        0    13560 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/__init__.py
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansi.py
+-rwxr-xr-x   0        0        0    11128 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rwxr-xr-x   0        0        0     3325 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/initialise.py
+-rwxr-xr-x   0        0        0     6181 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/win32.py
+-rwxr-xr-x   0        0        0     7134 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/winterm.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rwxr-xr-x   0        0        0    10678 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rwxr-xr-x   0        0        0     6741 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/utils.py
+-rwxr-xr-x   0        0        0     3709 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rwxr-xr-x   0        0        0      581 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/__init__.py
+-rwxr-xr-x   0        0        0    41259 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/compat.py
+-rwxr-xr-x   0        0        0    51697 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/database.py
+-rwxr-xr-x   0        0        0    20834 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/index.py
+-rwxr-xr-x   0        0        0    51991 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/locators.py
+-rwxr-xr-x   0        0        0    14811 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/manifest.py
+-rwxr-xr-x   0        0        0     5058 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/markers.py
+-rwxr-xr-x   0        0        0    39801 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/metadata.py
+-rwxr-xr-x   0        0        0    10820 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/resources.py
+-rwxr-xr-x   0        0        0    18102 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64.exe
+-rwxr-xr-x   0        0        0    66262 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/util.py
+-rwxr-xr-x   0        0        0    23513 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64.exe
+-rwxr-xr-x   0        0        0    43898 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/wheel.py
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/__init__.py
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/__main__.py
+-rwxr-xr-x   0        0        0    49330 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/distro.py
+-rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/__init__.py
+-rwxr-xr-x   0        0        0     3374 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/codec.py
+-rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/compat.py
+-rwxr-xr-x   0        0        0    12950 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/core.py
+-rwxr-xr-x   0        0        0    44375 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/idnadata.py
+-rwxr-xr-x   0        0        0     1881 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/intranges.py
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/package_data.py
+-rwxr-xr-x   0        0        0   206539 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/uts46data.py
+-rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/__init__.py
+-rwxr-xr-x   0        0        0     1081 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/exceptions.py
+-rwxr-xr-x   0        0        0     6079 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/ext.py
+-rwxr-xr-x   0        0        0    34544 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/fallback.py
+-rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/__about__.py
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/__init__.py
+-rwxr-xr-x   0        0        0    11488 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_manylinux.py
+-rwxr-xr-x   0        0        0     4378 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_musllinux.py
+-rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_structures.py
+-rwxr-xr-x   0        0        0     8487 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/markers.py
+-rwxr-xr-x   0        0        0     4676 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/requirements.py
+-rwxr-xr-x   0        0        0    30110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/specifiers.py
+-rwxr-xr-x   0        0        0    15699 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/tags.py
+-rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/utils.py
+-rwxr-xr-x   0        0        0    14665 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/version.py
+-rwxr-xr-x   0        0        0   109388 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rwxr-xr-x   0        0        0    18003 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__init__.py
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__main__.py
+-rwxr-xr-x   0        0        0     4303 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/android.py
+-rwxr-xr-x   0        0        0     5706 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/api.py
+-rwxr-xr-x   0        0        0     2800 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/macos.py
+-rwxr-xr-x   0        0        0     7448 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/unix.py
+-rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/version.py
+-rwxr-xr-x   0        0        0     7098 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/windows.py
+-rwxr-xr-x   0        0        0     2999 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/__init__.py
+-rwxr-xr-x   0        0        0      353 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/__main__.py
+-rwxr-xr-x   0        0        0    23685 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/cmdline.py
+-rwxr-xr-x   0        0        0     1697 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/console.py
+-rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filter.py
+-rwxr-xr-x   0        0        0     2917 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatter.py
+-rwxr-xr-x   0        0        0    32064 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexer.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/modeline.py
+-rwxr-xr-x   0        0        0     2591 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/plugin.py
+-rwxr-xr-x   0        0        0     3072 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/regexopt.py
+-rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/scanner.py
+-rwxr-xr-x   0        0        0     6882 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/sphinxext.py
+-rwxr-xr-x   0        0        0     6257 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/style.py
+-rwxr-xr-x   0        0        0     6184 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/token.py
+-rwxr-xr-x   0        0        0    63187 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/unistring.py
+-rwxr-xr-x   0        0        0     9110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/util.py
+-rwxr-xr-x   0        0        0    40386 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rwxr-xr-x   0        0        0     4800 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rwxr-xr-x   0        0        0     4104 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rwxr-xr-x   0        0        0     3314 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rwxr-xr-x   0        0        0     5086 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rwxr-xr-x   0        0        0    35601 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/html.py
+-rwxr-xr-x   0        0        0    21938 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/img.py
+-rwxr-xr-x   0        0        0     4981 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rwxr-xr-x   0        0        0    19351 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rwxr-xr-x   0        0        0     5073 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/other.py
+-rwxr-xr-x   0        0        0     2212 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rwxr-xr-x   0        0        0     5014 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rwxr-xr-x   0        0        0     7335 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rwxr-xr-x   0        0        0     4674 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rwxr-xr-x   0        0        0    11753 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rwxr-xr-x   0        0        0    11164 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rwxr-xr-x   0        0        0    71556 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rwxr-xr-x   0        0        0    53572 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/python.py
+-rwxr-xr-x   0        0        0     3419 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rwxr-xr-x   0        0        0     9171 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/__init__.py
+-rwxr-xr-x   0        0        0     6426 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/actions.py
+-rwxr-xr-x   0        0        0    12936 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/common.py
+-rwxr-xr-x   0        0        0   213344 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/core.py
+-rwxr-xr-x   0        0        0     9023 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rwxr-xr-x   0        0        0    39129 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/helpers.py
+-rwxr-xr-x   0        0        0    25341 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/results.py
+-rwxr-xr-x   0        0        0    13402 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/testing.py
+-rwxr-xr-x   0        0        0    10787 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/unicode.py
+-rwxr-xr-x   0        0        0     6805 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/util.py
+-rwxr-xr-x   0        0        0    23685 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rwxr-xr-x   0        0        0      491 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rwxr-xr-x   0        0        0    11920 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rwxr-xr-x   0        0        0    10927 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rwxr-xr-x   0        0        0     5178 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/__init__.py
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/__version__.py
+-rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/_internal_utils.py
+-rwxr-xr-x   0        0        0    21443 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/adapters.py
+-rwxr-xr-x   0        0        0     6377 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/api.py
+-rwxr-xr-x   0        0        0    10187 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/auth.py
+-rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/certs.py
+-rwxr-xr-x   0        0        0     1286 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/compat.py
+-rwxr-xr-x   0        0        0    18560 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/cookies.py
+-rwxr-xr-x   0        0        0     3823 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/exceptions.py
+-rwxr-xr-x   0        0        0     3879 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/help.py
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/hooks.py
+-rwxr-xr-x   0        0        0    35288 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/models.py
+-rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/packages.py
+-rwxr-xr-x   0        0        0    30180 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/sessions.py
+-rwxr-xr-x   0        0        0     4235 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/status_codes.py
+-rwxr-xr-x   0        0        0     2912 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/structures.py
+-rwxr-xr-x   0        0        0    33240 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/utils.py
+-rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/__init__.py
+-rwxr-xr-x   0        0        0     5871 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/providers.py
+-rwxr-xr-x   0        0        0     1601 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/reporters.py
+-rwxr-xr-x   0        0        0    20511 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rwxr-xr-x   0        0        0     4963 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/structs.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rwxr-xr-x   0        0        0     6090 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__init__.py
+-rwxr-xr-x   0        0        0     8478 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__main__.py
+-rwxr-xr-x   0        0        0    10096 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_cell_widths.py
+-rwxr-xr-x   0        0        0   140235 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rwxr-xr-x   0        0        0     2100 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_export_format.py
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_extension.py
+-rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_fileno.py
+-rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_inspect.py
+-rwxr-xr-x   0        0        0     3225 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_log_render.py
+-rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_loop.py
+-rwxr-xr-x   0        0        0     1387 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_null_file.py
+-rwxr-xr-x   0        0        0     7063 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_palettes.py
+-rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_pick.py
+-rwxr-xr-x   0        0        0     5472 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_ratio.py
+-rwxr-xr-x   0        0        0    19919 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_spinners.py
+-rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_stack.py
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_timer.py
+-rwxr-xr-x   0        0        0    22820 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_win32_console.py
+-rwxr-xr-x   0        0        0     1926 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows.py
+-rwxr-xr-x   0        0        0     2783 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rwxr-xr-x   0        0        0     1840 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_wrap.py
+-rwxr-xr-x   0        0        0      890 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/abc.py
+-rwxr-xr-x   0        0        0    10368 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/align.py
+-rwxr-xr-x   0        0        0     6906 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/ansi.py
+-rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/bar.py
+-rwxr-xr-x   0        0        0     9842 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/box.py
+-rwxr-xr-x   0        0        0     4509 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/cells.py
+-rwxr-xr-x   0        0        0    18224 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color.py
+-rwxr-xr-x   0        0        0     1054 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color_triplet.py
+-rwxr-xr-x   0        0        0     7131 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/columns.py
+-rwxr-xr-x   0        0        0    99195 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/console.py
+-rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/constrain.py
+-rwxr-xr-x   0        0        0     5497 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/containers.py
+-rwxr-xr-x   0        0        0     6630 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/control.py
+-rwxr-xr-x   0        0        0     8082 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/default_styles.py
+-rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/diagnose.py
+-rwxr-xr-x   0        0        0     2501 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/emoji.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/errors.py
+-rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/file_proxy.py
+-rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/filesize.py
+-rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/highlighter.py
+-rwxr-xr-x   0        0        0     5032 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/json.py
+-rwxr-xr-x   0        0        0     3252 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/jupyter.py
+-rwxr-xr-x   0        0        0    14007 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/layout.py
+-rwxr-xr-x   0        0        0    14273 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live.py
+-rwxr-xr-x   0        0        0     3667 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live_render.py
+-rwxr-xr-x   0        0        0    11903 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/logging.py
+-rwxr-xr-x   0        0        0     8198 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/markup.py
+-rwxr-xr-x   0        0        0     5305 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/measure.py
+-rwxr-xr-x   0        0        0     4970 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/padding.py
+-rwxr-xr-x   0        0        0      828 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pager.py
+-rwxr-xr-x   0        0        0     3396 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/palette.py
+-rwxr-xr-x   0        0        0    10574 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/panel.py
+-rwxr-xr-x   0        0        0    35852 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pretty.py
+-rwxr-xr-x   0        0        0    59706 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress.py
+-rwxr-xr-x   0        0        0     8165 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress_bar.py
+-rwxr-xr-x   0        0        0    11303 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/prompt.py
+-rwxr-xr-x   0        0        0     1391 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/protocol.py
+-rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/region.py
+-rwxr-xr-x   0        0        0     4431 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/repr.py
+-rwxr-xr-x   0        0        0     4602 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/rule.py
+-rwxr-xr-x   0        0        0     2843 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/scope.py
+-rwxr-xr-x   0        0        0     1591 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/screen.py
+-rwxr-xr-x   0        0        0    24247 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/segment.py
+-rwxr-xr-x   0        0        0     4339 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/spinner.py
+-rwxr-xr-x   0        0        0     4425 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/status.py
+-rwxr-xr-x   0        0        0    27073 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/style.py
+-rwxr-xr-x   0        0        0     1258 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/styled.py
+-rwxr-xr-x   0        0        0    35153 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/syntax.py
+-rwxr-xr-x   0        0        0    39684 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/table.py
+-rwxr-xr-x   0        0        0     3370 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/terminal_theme.py
+-rwxr-xr-x   0        0        0    45525 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/text.py
+-rwxr-xr-x   0        0        0     3777 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/theme.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/themes.py
+-rwxr-xr-x   0        0        0    29604 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/traceback.py
+-rwxr-xr-x   0        0        0     9169 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/tree.py
+-rwxr-xr-x   0        0        0    20493 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/__init__.py
+-rwxr-xr-x   0        0        0     3551 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rwxr-xr-x   0        0        0     2179 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_utils.py
+-rwxr-xr-x   0        0        0     1682 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/after.py
+-rwxr-xr-x   0        0        0     1562 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before.py
+-rwxr-xr-x   0        0        0     2372 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rwxr-xr-x   0        0        0     1383 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/nap.py
+-rwxr-xr-x   0        0        0     8746 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/retry.py
+-rwxr-xr-x   0        0        0     3086 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/stop.py
+-rwxr-xr-x   0        0        0     2142 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rwxr-xr-x   0        0        0     8024 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/wait.py
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/__init__.py
+-rwxr-xr-x   0        0        0    22633 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_parser.py
+-rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_re.py
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_types.py
+-rwxr-xr-x   0        0        0     3333 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/__init__.py
+-rwxr-xr-x   0        0        0    10811 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/_collections.py
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/_version.py
+-rwxr-xr-x   0        0        0    20300 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connection.py
+-rwxr-xr-x   0        0        0    39128 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rwxr-xr-x   0        0        0     8217 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/exceptions.py
+-rwxr-xr-x   0        0        0     8579 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/fields.py
+-rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/filepost.py
+-rwxr-xr-x   0        0        0    19786 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rwxr-xr-x   0        0        0     5985 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/request.py
+-rwxr-xr-x   0        0        0    30641 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/response.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rwxr-xr-x   0        0        0    11036 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rwxr-xr-x   0        0        0     4528 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rwxr-xr-x   0        0        0    17081 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rwxr-xr-x   0        0        0    34448 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rwxr-xr-x   0        0        0     7097 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rwxr-xr-x   0        0        0    17632 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rwxr-xr-x   0        0        0    13922 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rwxr-xr-x   0        0        0    34665 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/six.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rwxr-xr-x   0        0        0     1417 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rwxr-xr-x   0        0        0     1155 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rwxr-xr-x   0        0        0     4901 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/connection.py
+-rwxr-xr-x   0        0        0     1605 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/queue.py
+-rwxr-xr-x   0        0        0     3997 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/request.py
+-rwxr-xr-x   0        0        0     3510 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/response.py
+-rwxr-xr-x   0        0        0    22003 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/retry.py
+-rwxr-xr-x   0        0        0    17177 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rwxr-xr-x   0        0        0     5758 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rwxr-xr-x   0        0        0     6895 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rwxr-xr-x   0        0        0    10168 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rwxr-xr-x   0        0        0    14296 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/url.py
+-rwxr-xr-x   0        0        0     5403 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/wait.py
+-rwxr-xr-x   0        0        0    10579 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/__init__.py
+-rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/labels.py
+-rwxr-xr-x   0        0        0     1305 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/mklabels.py
+-rwxr-xr-x   0        0        0     6563 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/tests.py
+-rwxr-xr-x   0        0        0     4307 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rwxr-xr-x   0        0        0     9953 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/METADATA
+-rwxr-xr-x   0        0        0    76554 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0   103551 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/__init__.py
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/py31compat.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/__init__.py
+-rwxr-xr-x   0        0        0    22376 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/appdirs.py
+-rwxr-xr-x   0        0        0   229871 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/pyparsing.py
+-rwxr-xr-x   0        0        0    30098 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/six.py
+-rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rwxr-xr-x   0        0        0      860 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rwxr-xr-x   0        0        0     1416 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rwxr-xr-x   0        0        0     8248 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rwxr-xr-x   0        0        0     4355 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rwxr-xr-x   0        0        0    28025 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rwxr-xr-x   0        0        0    11556 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/version.py
+-rwxr-xr-x   0        0        0     2487 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/extern/__init__.py
+-rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/DESCRIPTION.rst
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/metadata.json
+-rwxr-xr-x   0        0        0     2959 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/__init__.py
+-rwxr-xr-x   0        0        0      348 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/__main__.py
+-rwxr-xr-x   0        0        0    23530 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/cmdline.py
+-rwxr-xr-x   0        0        0     1697 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/console.py
+-rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/filter.py
+-rwxr-xr-x   0        0        0     4154 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatter.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/modeline.py
+-rwxr-xr-x   0        0        0     2579 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/plugin.py
+-rwxr-xr-x   0        0        0     3072 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/regexopt.py
+-rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/scanner.py
+-rwxr-xr-x   0        0        0     6816 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/sphinxext.py
+-rwxr-xr-x   0        0        0     6245 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/style.py
+-rwxr-xr-x   0        0        0     6184 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/token.py
+-rwxr-xr-x   0        0        0    63223 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/unistring.py
+-rwxr-xr-x   0        0        0    10230 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/util.py
+-rwxr-xr-x   0        0        0    40338 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/filters/__init__.py
+-rwxr-xr-x   0        0        0     5388 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/__init__.py
+-rwxr-xr-x   0        0        0     4176 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/_mapping.py
+-rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/bbcode.py
+-rwxr-xr-x   0        0        0     5070 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/groff.py
+-rwxr-xr-x   0        0        0    35574 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/html.py
+-rwxr-xr-x   0        0        0    21914 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/img.py
+-rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/irc.py
+-rwxr-xr-x   0        0        0    19303 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/latex.py
+-rwxr-xr-x   0        0        0     5025 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/other.py
+-rwxr-xr-x   0        0        0     2200 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/pangomarkup.py
+-rwxr-xr-x   0        0        0     4990 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/rtf.py
+-rwxr-xr-x   0        0        0     7299 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/svg.py
+-rwxr-xr-x   0        0        0     4626 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal.py
+-rwxr-xr-x   0        0        0    11717 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal256.py
+-rwxr-xr-x   0        0        0    12082 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/__init__.py
+-rwxr-xr-x   0        0        0     1543 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_ada_builtins.py
+-rwxr-xr-x   0        0        0    27287 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_asy_builtins.py
+-rwxr-xr-x   0        0        0    13994 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cl_builtins.py
+-rwxr-xr-x   0        0        0   105182 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cocoa_builtins.py
+-rwxr-xr-x   0        0        0    18414 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_csound_builtins.py
+-rwxr-xr-x   0        0        0    12446 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_css_builtins.py
+-rwxr-xr-x   0        0        0    11883 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_julia_builtins.py
+-rwxr-xr-x   0        0        0   134510 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lasso_builtins.py
+-rwxr-xr-x   0        0        0   108094 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lilypond_builtins.py
+-rwxr-xr-x   0        0        0     8116 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lua_builtins.py
+-rwxr-xr-x   0        0        0    65633 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mapping.py
+-rwxr-xr-x   0        0        0    24713 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mql_builtins.py
+-rwxr-xr-x   0        0        0    25842 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mysql_builtins.py
+-rwxr-xr-x   0        0        0    49398 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_openedge_builtins.py
+-rwxr-xr-x   0        0        0   107930 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_php_builtins.py
+-rwxr-xr-x   0        0        0    13355 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_postgres_builtins.py
+-rwxr-xr-x   0        0        0    32564 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scheme_builtins.py
+-rwxr-xr-x   0        0        0    52413 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scilab_builtins.py
+-rwxr-xr-x   0        0        0    26781 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rwxr-xr-x   0        0        0    13445 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stan_builtins.py
+-rwxr-xr-x   0        0        0    27227 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stata_builtins.py
+-rwxr-xr-x   0        0        0    15460 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_tsql_builtins.py
+-rwxr-xr-x   0        0        0     1658 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_usd_builtins.py
+-rwxr-xr-x   0        0        0     4225 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vbscript_builtins.py
+-rwxr-xr-x   0        0        0    57066 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vim_builtins.py
+-rwxr-xr-x   0        0        0    11676 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/actionscript.py
+-rwxr-xr-x   0        0        0     5320 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ada.py
+-rwxr-xr-x   0        0        0      876 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/agile.py
+-rwxr-xr-x   0        0        0     9873 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/algebra.py
+-rwxr-xr-x   0        0        0     2606 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ambient.py
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/amdgpu.py
+-rwxr-xr-x   0        0        0     4177 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ampl.py
+-rwxr-xr-x   0        0        0    30766 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apdlexer.py
+-rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apl.py
+-rwxr-xr-x   0        0        0    11469 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/archetype.py
+-rwxr-xr-x   0        0        0     3565 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arrow.py
+-rwxr-xr-x   0        0        0    11417 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arturo.py
+-rwxr-xr-x   0        0        0     1621 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asc.py
+-rwxr-xr-x   0        0        0    41243 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asm.py
+-rwxr-xr-x   0        0        0    19815 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/automation.py
+-rwxr-xr-x   0        0        0     3915 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/boa.py
+-rwxr-xr-x   0        0        0    28112 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/business.py
+-rwxr-xr-x   0        0        0    29206 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/c_like.py
+-rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/capnproto.py
+-rwxr-xr-x   0        0        0     3231 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/carbon.py
+-rwxr-xr-x   0        0        0     5182 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cddl.py
+-rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/chapel.py
+-rwxr-xr-x   0        0        0     6395 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/clean.py
+-rwxr-xr-x   0        0        0     3156 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/comal.py
+-rwxr-xr-x   0        0        0     1407 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/compiled.py
+-rwxr-xr-x   0        0        0    42338 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/configs.py
+-rwxr-xr-x   0        0        0     4148 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/console.py
+-rwxr-xr-x   0        0        0     1390 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cplint.py
+-rwxr-xr-x   0        0        0    15756 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/crystal.py
+-rwxr-xr-x   0        0        0    16994 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/csound.py
+-rwxr-xr-x   0        0        0    25322 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/css.py
+-rwxr-xr-x   0        0        0     9875 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/d.py
+-rwxr-xr-x   0        0        0     4607 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dalvik.py
+-rwxr-xr-x   0        0        0    26940 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/data.py
+-rwxr-xr-x   0        0        0     8099 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dax.py
+-rwxr-xr-x   0        0        0     4020 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/devicetree.py
+-rwxr-xr-x   0        0        0     5278 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/diff.py
+-rwxr-xr-x   0        0        0    37623 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dotnet.py
+-rwxr-xr-x   0        0        0    36774 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dsls.py
+-rwxr-xr-x   0        0        0    10380 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dylan.py
+-rwxr-xr-x   0        0        0     6372 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ecl.py
+-rwxr-xr-x   0        0        0     3152 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elm.py
+-rwxr-xr-x   0        0        0     6370 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elpi.py
+-rwxr-xr-x   0        0        0     4742 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/email.py
+-rwxr-xr-x   0        0        0    19170 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/erlang.py
+-rwxr-xr-x   0        0        0    10396 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/esoteric.py
+-rwxr-xr-x   0        0        0     3273 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ezhil.py
+-rwxr-xr-x   0        0        0    19531 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/factor.py
+-rwxr-xr-x   0        0        0    10197 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fantom.py
+-rwxr-xr-x   0        0        0     9646 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/felix.py
+-rwxr-xr-x   0        0        0     1621 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fift.py
+-rwxr-xr-x   0        0        0     2668 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/floscript.py
+-rwxr-xr-x   0        0        0     7194 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/forth.py
+-rwxr-xr-x   0        0        0    10336 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fortran.py
+-rwxr-xr-x   0        0        0    26212 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/foxpro.py
+-rwxr-xr-x   0        0        0    26914 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/freefem.py
+-rwxr-xr-x   0        0        0     3622 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/func.py
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/functional.py
+-rwxr-xr-x   0        0        0     3732 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/futhark.py
+-rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gcodelexer.py
+-rwxr-xr-x   0        0        0     7543 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gdscript.py
+-rwxr-xr-x   0        0        0     7980 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/grammar_notation.py
+-rwxr-xr-x   0        0        0     3861 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graph.py
+-rwxr-xr-x   0        0        0    39026 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphics.py
+-rwxr-xr-x   0        0        0     1935 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphviz.py
+-rwxr-xr-x   0        0        0     3991 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gsql.py
+-rwxr-xr-x   0        0        0    32898 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haskell.py
+-rwxr-xr-x   0        0        0    30976 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haxe.py
+-rwxr-xr-x   0        0        0    22520 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/hdl.py
+-rwxr-xr-x   0        0        0    15450 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/idl.py
+-rwxr-xr-x   0        0        0    30631 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/igor.py
+-rwxr-xr-x   0        0        0     3136 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/inferno.py
+-rwxr-xr-x   0        0        0    13178 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/installers.py
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/iolang.py
+-rwxr-xr-x   0        0        0    62859 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/javascript.py
+-rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jmespath.py
+-rwxr-xr-x   0        0        0     3701 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jslt.py
+-rwxr-xr-x   0        0        0     5635 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jsonnet.py
+-rwxr-xr-x   0        0        0    11646 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/julia.py
+-rwxr-xr-x   0        0        0    72929 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jvm.py
+-rwxr-xr-x   0        0        0    11406 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/kuin.py
+-rwxr-xr-x   0        0        0   144039 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/lisp.py
+-rwxr-xr-x   0        0        0    31914 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/macaulay2.py
+-rwxr-xr-x   0        0        0     7618 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/make.py
+-rwxr-xr-x   0        0        0    58129 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/markup.py
+-rwxr-xr-x   0        0        0      676 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/math.py
+-rwxr-xr-x   0        0        0     2716 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/maxima.py
+-rwxr-xr-x   0        0        0     4337 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/meson.py
+-rwxr-xr-x   0        0        0    13846 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/minecraft.py
+-rwxr-xr-x   0        0        0     4604 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mips.py
+-rwxr-xr-x   0        0        0    13524 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modeling.py
+-rwxr-xr-x   0        0        0    53073 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modula2.py
+-rwxr-xr-x   0        0        0     6290 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/monte.py
+-rwxr-xr-x   0        0        0     9187 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mosel.py
+-rwxr-xr-x   0        0        0    63962 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ncl.py
+-rwxr-xr-x   0        0        0     2726 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nit.py
+-rwxr-xr-x   0        0        0     4015 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nix.py
+-rwxr-xr-x   0        0        0     4169 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/oberon.py
+-rwxr-xr-x   0        0        0    22961 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/objective.py
+-rwxr-xr-x   0        0        0     2982 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ooc.py
+-rwxr-xr-x   0        0        0     1744 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/other.py
+-rwxr-xr-x   0        0        0     2720 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parasail.py
+-rwxr-xr-x   0        0        0    25904 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parsers.py
+-rwxr-xr-x   0        0        0     8146 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pawn.py
+-rwxr-xr-x   0        0        0    39170 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/perl.py
+-rwxr-xr-x   0        0        0    23252 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/phix.py
+-rwxr-xr-x   0        0        0    13040 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/php.py
+-rwxr-xr-x   0        0        0     1975 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pointless.py
+-rwxr-xr-x   0        0        0    12677 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/praat.py
+-rwxr-xr-x   0        0        0     1156 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/procfile.py
+-rwxr-xr-x   0        0        0    12351 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/prolog.py
+-rwxr-xr-x   0        0        0     4715 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/promql.py
+-rwxr-xr-x   0        0        0    53376 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/python.py
+-rwxr-xr-x   0        0        0     6072 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/qvt.py
+-rwxr-xr-x   0        0        0     6185 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/r.py
+-rwxr-xr-x   0        0        0    15790 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rdf.py
+-rwxr-xr-x   0        0        0    18248 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rebol.py
+-rwxr-xr-x   0        0        0     2902 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/resource.py
+-rwxr-xr-x   0        0        0     5056 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ride.py
+-rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rita.py
+-rwxr-xr-x   0        0        0     1973 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rnc.py
+-rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/roboconf.py
+-rwxr-xr-x   0        0        0    18449 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/robotframework.py
+-rwxr-xr-x   0        0        0    22775 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ruby.py
+-rwxr-xr-x   0        0        0     8216 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rust.py
+-rwxr-xr-x   0        0        0     9400 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sas.py
+-rwxr-xr-x   0        0        0     4645 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/savi.py
+-rwxr-xr-x   0        0        0     2239 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scdoc.py
+-rwxr-xr-x   0        0        0    70014 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scripting.py
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sgf.py
+-rwxr-xr-x   0        0        0    36466 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/shell.py
+-rwxr-xr-x   0        0        0     2441 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sieve.py
+-rwxr-xr-x   0        0        0     8482 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/slash.py
+-rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smalltalk.py
+-rwxr-xr-x   0        0        0     2660 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smithy.py
+-rwxr-xr-x   0        0        0     2773 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smv.py
+-rwxr-xr-x   0        0        0     2732 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/snobol.py
+-rwxr-xr-x   0        0        0     3127 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/solidity.py
+-rwxr-xr-x   0        0        0     3330 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sophia.py
+-rwxr-xr-x   0        0        0     3414 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/special.py
+-rwxr-xr-x   0        0        0     2733 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/spice.py
+-rwxr-xr-x   0        0        0    42086 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sql.py
+-rwxr-xr-x   0        0        0     3698 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/supercollider.py
+-rwxr-xr-x   0        0        0     2639 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tal.py
+-rwxr-xr-x   0        0        0     5513 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tcl.py
+-rwxr-xr-x   0        0        0     3523 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teal.py
+-rwxr-xr-x   0        0        0    72610 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/templates.py
+-rwxr-xr-x   0        0        0     9719 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teraterm.py
+-rwxr-xr-x   0        0        0    10767 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/testing.py
+-rwxr-xr-x   0        0        0     1029 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/text.py
+-rwxr-xr-x   0        0        0     7609 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textedit.py
+-rwxr-xr-x   0        0        0    15192 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textfmts.py
+-rwxr-xr-x   0        0        0    20157 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/theorem.py
+-rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/thingsdb.py
+-rwxr-xr-x   0        0        0     1377 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tlb.py
+-rwxr-xr-x   0        0        0    10457 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tnt.py
+-rwxr-xr-x   0        0        0     1474 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/trafficscript.py
+-rwxr-xr-x   0        0        0     8207 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/typoscript.py
+-rwxr-xr-x   0        0        0     8956 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ul4.py
+-rwxr-xr-x   0        0        0    18512 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/unicon.py
+-rwxr-xr-x   0        0        0     6037 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/urbi.py
+-rwxr-xr-x   0        0        0     3513 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/usd.py
+-rwxr-xr-x   0        0        0     7273 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/varnish.py
+-rwxr-xr-x   0        0        0     3885 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/verification.py
+-rwxr-xr-x   0        0        0      894 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/web.py
+-rwxr-xr-x   0        0        0     5699 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webassembly.py
+-rwxr-xr-x   0        0        0    10517 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webidl.py
+-rwxr-xr-x   0        0        0    40549 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webmisc.py
+-rwxr-xr-x   0        0        0    11920 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wgsl.py
+-rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/whiley.py
+-rwxr-xr-x   0        0        0     4021 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wowtoc.py
+-rwxr-xr-x   0        0        0     3239 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wren.py
+-rwxr-xr-x   0        0        0     1920 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/x10.py
+-rwxr-xr-x   0        0        0      902 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/xorg.py
+-rwxr-xr-x   0        0        0     4500 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/yang.py
+-rwxr-xr-x   0        0        0     3953 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/zig.py
+-rwxr-xr-x   0        0        0      491 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/__init__.py
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_compat.py
+-rwxr-xr-x   0        0        0    11920 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_impl.py
+-rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/__init__.py
+-rwxr-xr-x   0        0        0    10927 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/_in_process.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1081 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1171 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0     1119 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/__about__.py
+-rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/__init__.py
+-rwxr-xr-x   0        0        0      625 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/__main__.py
+-rwxr-xr-x   0        0        0     4290 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/clean.py
+-rwxr-xr-x   0        0        0     3595 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/markdown.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/py.typed
+-rwxr-xr-x   0        0        0     4460 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/rst.py
+-rwxr-xr-x   0        0        0      823 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/txt.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     9694 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     2669 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     4963 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/__init__.py
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/__version__.py
+-rwxr-xr-x   0        0        0     1495 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/_internal_utils.py
+-rwxr-xr-x   0        0        0    19553 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/adapters.py
+-rwxr-xr-x   0        0        0     6449 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/api.py
+-rwxr-xr-x   0        0        0    10187 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/auth.py
+-rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/certs.py
+-rwxr-xr-x   0        0        0     1451 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/compat.py
+-rwxr-xr-x   0        0        0    18560 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/cookies.py
+-rwxr-xr-x   0        0        0     3811 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/exceptions.py
+-rwxr-xr-x   0        0        0     3875 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/help.py
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/hooks.py
+-rwxr-xr-x   0        0        0    35223 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/models.py
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/packages.py
+-rwxr-xr-x   0        0        0    30373 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/sessions.py
+-rwxr-xr-x   0        0        0     4235 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/status_codes.py
+-rwxr-xr-x   0        0        0     2912 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/structures.py
+-rwxr-xr-x   0        0        0    33448 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/utils.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0    10142 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4634 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2743 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/__init__.py
+-rwxr-xr-x   0        0        0     9260 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/_compat.py
+-rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/exceptions.py
+-rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/sessions.py
+-rwxr-xr-x   0        0        0     4044 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/streaming_iterator.py
+-rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/__init__.py
+-rwxr-xr-x   0        0        0     7539 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/appengine.py
+-rwxr-xr-x   0        0        0     1404 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rwxr-xr-x   0        0        0     4789 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/socket_options.py
+-rwxr-xr-x   0        0        0     2608 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/source.py
+-rwxr-xr-x   0        0        0     2399 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/ssl.py
+-rwxr-xr-x   0        0        0     7854 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/x509.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/__init__.py
+-rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rwxr-xr-x   0        0        0     4944 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/guess.py
+-rwxr-xr-x   0        0        0     4407 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/handler.py
+-rwxr-xr-x   0        0        0     3706 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/cookies/__init__.py
+-rwxr-xr-x   0        0        0      213 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/cookies/forgetful.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rwxr-xr-x   0        0        0     6024 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/stream.py
+-rwxr-xr-x   0        0        0     4365 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/tee.py
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/__init__.py
+-rwxr-xr-x   0        0        0     4861 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/decoder.py
+-rwxr-xr-x   0        0        0    20769 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/encoder.py
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/__init__.py
+-rwxr-xr-x   0        0        0     6628 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/pool.py
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/thread.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/__init__.py
+-rwxr-xr-x   0        0        0     2558 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/deprecated.py
+-rwxr-xr-x   0        0        0     6522 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/dump.py
+-rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/formdata.py
+-rwxr-xr-x   0        0        0     4524 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/user_agent.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    14638 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     6044 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1565 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/__init__.py
+-rwxr-xr-x   0        0        0    13297 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/_mixin.py
+-rwxr-xr-x   0        0        0     9048 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/abnf_regexp.py
+-rwxr-xr-x   0        0        0     3862 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/api.py
+-rwxr-xr-x   0        0        0    12709 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/builder.py
+-rwxr-xr-x   0        0        0     1620 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/compat.py
+-rwxr-xr-x   0        0        0     3614 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/exceptions.py
+-rwxr-xr-x   0        0        0     5477 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/iri.py
+-rwxr-xr-x   0        0        0     4114 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/misc.py
+-rwxr-xr-x   0        0        0     5261 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/normalizers.py
+-rwxr-xr-x   0        0        0    14599 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/parseresult.py
+-rwxr-xr-x   0        0        0     5183 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/uri.py
+-rwxr-xr-x   0        0        0    13676 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/validators.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      564 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     6630 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2072 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/__init__.py
+-rwxr-xr-x   0        0        0     8334 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/__main__.py
+-rwxr-xr-x   0        0        0    10096 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_cell_widths.py
+-rwxr-xr-x   0        0        0   140235 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_emoji_codes.py
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_emoji_replace.py
+-rwxr-xr-x   0        0        0     2100 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_export_format.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_extension.py
+-rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_fileno.py
+-rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_inspect.py
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_log_render.py
+-rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_loop.py
+-rwxr-xr-x   0        0        0     1387 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_null_file.py
+-rwxr-xr-x   0        0        0     7063 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_palettes.py
+-rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_pick.py
+-rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_ratio.py
+-rwxr-xr-x   0        0        0    19919 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_spinners.py
+-rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_stack.py
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_timer.py
+-rwxr-xr-x   0        0        0    22784 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_win32_console.py
+-rwxr-xr-x   0        0        0     1902 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_windows.py
+-rwxr-xr-x   0        0        0     2759 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_windows_renderer.py
+-rwxr-xr-x   0        0        0     1840 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_wrap.py
+-rwxr-xr-x   0        0        0      878 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/abc.py
+-rwxr-xr-x   0        0        0    10320 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/align.py
+-rwxr-xr-x   0        0        0     6906 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/ansi.py
+-rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/bar.py
+-rwxr-xr-x   0        0        0     9794 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/box.py
+-rwxr-xr-x   0        0        0     4509 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/cells.py
+-rwxr-xr-x   0        0        0    18224 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/color.py
+-rwxr-xr-x   0        0        0     1054 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/color_triplet.py
+-rwxr-xr-x   0        0        0     7131 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/columns.py
+-rwxr-xr-x   0        0        0    99146 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/console.py
+-rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/constrain.py
+-rwxr-xr-x   0        0        0     5497 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/containers.py
+-rwxr-xr-x   0        0        0     6606 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/control.py
+-rwxr-xr-x   0        0        0     8046 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/default_styles.py
+-rwxr-xr-x   0        0        0      924 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/diagnose.py
+-rwxr-xr-x   0        0        0     2465 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/emoji.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/errors.py
+-rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/file_proxy.py
+-rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/filesize.py
+-rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/highlighter.py
+-rwxr-xr-x   0        0        0     5020 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/json.py
+-rwxr-xr-x   0        0        0     3228 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/jupyter.py
+-rwxr-xr-x   0        0        0    13947 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/layout.py
+-rwxr-xr-x   0        0        0    14273 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/live.py
+-rwxr-xr-x   0        0        0     3655 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/live_render.py
+-rwxr-xr-x   0        0        0    11891 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/logging.py
+-rwxr-xr-x   0        0        0    26245 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/markdown.py
+-rwxr-xr-x   0        0        0     8174 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/markup.py
+-rwxr-xr-x   0        0        0     5305 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/measure.py
+-rwxr-xr-x   0        0        0     4958 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/padding.py
+-rwxr-xr-x   0        0        0      828 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/pager.py
+-rwxr-xr-x   0        0        0     3288 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/palette.py
+-rwxr-xr-x   0        0        0    10574 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/panel.py
+-rwxr-xr-x   0        0        0    35816 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/pretty.py
+-rwxr-xr-x   0        0        0    59694 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/progress.py
+-rwxr-xr-x   0        0        0     8165 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/progress_bar.py
+-rwxr-xr-x   0        0        0    11291 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/prompt.py
+-rwxr-xr-x   0        0        0     1367 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/protocol.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/py.typed
+-rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/region.py
+-rwxr-xr-x   0        0        0     4419 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/repr.py
+-rwxr-xr-x   0        0        0     4590 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/rule.py
+-rwxr-xr-x   0        0        0     2831 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/scope.py
+-rwxr-xr-x   0        0        0     1579 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/screen.py
+-rwxr-xr-x   0        0        0    24211 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/segment.py
+-rwxr-xr-x   0        0        0     4339 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/spinner.py
+-rwxr-xr-x   0        0        0     4425 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/status.py
+-rwxr-xr-x   0        0        0    27073 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/style.py
+-rwxr-xr-x   0        0        0     1234 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/styled.py
+-rwxr-xr-x   0        0        0    35065 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/syntax.py
+-rwxr-xr-x   0        0        0    39648 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/table.py
+-rwxr-xr-x   0        0        0     3370 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/terminal_theme.py
+-rwxr-xr-x   0        0        0    45513 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/text.py
+-rwxr-xr-x   0        0        0     3777 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/theme.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/themes.py
+-rwxr-xr-x   0        0        0    29532 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/traceback.py
+-rwxr-xr-x   0        0        0     9109 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/tree.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    18837 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/METADATA
+-rwxr-xr-x   0        0        0     9572 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/RECORD
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0     5700 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/__init__.py
+-rwxr-xr-x   0        0        0     6592 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/archive_util.py
+-rwxr-xr-x   0        0        0     5671 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/build_meta.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/cli-32.exe
+-rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/cli-64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/cli.exe
+-rwxr-xr-x   0        0        0    16381 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/config.py
+-rwxr-xr-x   0        0        0      935 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/dep_util.py
+-rwxr-xr-x   0        0        0     5837 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/depends.py
+-rwxr-xr-x   0        0        0    42522 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/dist.py
+-rwxr-xr-x   0        0        0     1729 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/extension.py
+-rwxr-xr-x   0        0        0     3146 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/glibc.py
+-rwxr-xr-x   0        0        0     5207 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/glob.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/gui-32.exe
+-rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/gui-64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/gui.exe
+-rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/launch.py
+-rwxr-xr-x   0        0        0     2013 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/lib2to3_ex.py
+-rwxr-xr-x   0        0        0     5789 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/monkey.py
+-rwxr-xr-x   0        0        0    40877 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/msvc.py
+-rwxr-xr-x   0        0        0     3199 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/namespaces.py
+-rwxr-xr-x   0        0        0    40153 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/package_index.py
+-rwxr-xr-x   0        0        0    10882 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/pep425tags.py
+-rwxr-xr-x   0        0        0      536 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py27compat.py
+-rwxr-xr-x   0        0        0     1192 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py31compat.py
+-rwxr-xr-x   0        0        0     1182 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py33compat.py
+-rwxr-xr-x   0        0        0     2891 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py36compat.py
+-rwxr-xr-x   0        0        0    14276 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/sandbox.py
+-rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/script (dev).tmpl
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/script.tmpl
+-rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/site-patch.py
+-rwxr-xr-x   0        0        0     8492 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/ssl_support.py
+-rwxr-xr-x   0        0        0      996 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/unicode_utils.py
+-rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/version.py
+-rwxr-xr-x   0        0        0     7230 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/wheel.py
+-rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/windows_support.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/__init__.py
+-rwxr-xr-x   0        0        0   229867 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/pyparsing.py
+-rwxr-xr-x   0        0        0    30098 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/six.py
+-rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__about__.py
+-rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__init__.py
+-rwxr-xr-x   0        0        0      860 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_compat.py
+-rwxr-xr-x   0        0        0     1416 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_structures.py
+-rwxr-xr-x   0        0        0     8239 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/markers.py
+-rwxr-xr-x   0        0        0     4343 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/requirements.py
+-rwxr-xr-x   0        0        0    28025 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/utils.py
+-rwxr-xr-x   0        0        0    11556 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/version.py
+-rwxr-xr-x   0        0        0      594 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/__init__.py
+-rwxr-xr-x   0        0        0     2426 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/alias.py
+-rwxr-xr-x   0        0        0    18185 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_egg.py
+-rwxr-xr-x   0        0        0     1508 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_rpm.py
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_wininst.py
+-rwxr-xr-x   0        0        0     4484 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_clib.py
+-rwxr-xr-x   0        0        0    13173 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_ext.py
+-rwxr-xr-x   0        0        0     9596 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_py.py
+-rwxr-xr-x   0        0        0     8046 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/develop.py
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/dist_info.py
+-rwxr-xr-x   0        0        0    89413 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/easy_install.py
+-rwxr-xr-x   0        0        0    24808 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/egg_info.py
+-rwxr-xr-x   0        0        0     4683 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install.py
+-rwxr-xr-x   0        0        0     3195 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_egg_info.py
+-rwxr-xr-x   0        0        0     5012 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_lib.py
+-rwxr-xr-x   0        0        0     2439 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_scripts.py
+-rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/launcher manifest.xml
+-rwxr-xr-x   0        0        0     4986 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/py36compat.py
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/register.py
+-rwxr-xr-x   0        0        0     2164 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/rotate.py
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/saveopts.py
+-rwxr-xr-x   0        0        0     6711 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/sdist.py
+-rwxr-xr-x   0        0        0     5085 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/setopt.py
+-rwxr-xr-x   0        0        0     9214 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/test.py
+-rwxr-xr-x   0        0        0     1172 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload.py
+-rwxr-xr-x   0        0        0     7311 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload_docs.py
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/extern/__init__.py
+-rwxr-xr-x   0        0        0     1422 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/DESCRIPTION.rst
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0    11362 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/dependency_links.txt
+-rwxr-xr-x   0        0        0     2934 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/metadata.json
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/zip-safe
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli/__init__.py
+-rwxr-xr-x   0        0        0    22633 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli/_parser.py
+-rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli/_re.py
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli/_types.py
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli/py.typed
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     8875 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/__init__.py
+-rwxr-xr-x   0        0        0     1475 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/__main__.py
+-rwxr-xr-x   0        0        0     3129 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/auth.py
+-rwxr-xr-x   0        0        0     3738 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/cli.py
+-rwxr-xr-x   0        0        0     3814 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/exceptions.py
+-rwxr-xr-x   0        0        0    11024 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/package.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/py.typed
+-rwxr-xr-x   0        0        0     8713 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/repository.py
+-rwxr-xr-x   0        0        0    12269 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/settings.py
+-rwxr-xr-x   0        0        0    10867 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/utils.py
+-rwxr-xr-x   0        0        0     3049 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/wheel.py
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/wininst.py
+-rwxr-xr-x   0        0        0     1802 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/__init__.py
+-rwxr-xr-x   0        0        0     5727 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/check.py
+-rwxr-xr-x   0        0        0     2904 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/register.py
+-rwxr-xr-x   0        0        0     7469 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/upload.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     3259 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2630 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/RECORD
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/REQUESTED
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0    13936 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0      565 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0    10676 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp/__init__.py
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp/py310compat.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     3735 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        5 2020-02-02 00:00:00.000000 pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 pyswxf-0.0.2/README.md
+-rwxr-xr-x   0        0        0      598 2020-02-02 00:00:00.000000 pyswxf-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pyswxf-0.0.2/PKG-INFO
```

### Comparing `pyswxf-0.0.1/src/pySWXF/refl_funs.py` & `pyswxf-0.0.2/src/pySWXF/refl_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/src/pySWXF/standing_wave.py` & `pyswxf-0.0.2/src/pySWXF/standing_wave.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/src/pySWXF/xray_utils.py` & `pyswxf-0.0.2/src/pySWXF/xray_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/activate` & `pyswxf-0.0.2/tutorial_env/bin/activate`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/activate.csh` & `pyswxf-0.0.2/tutorial_env/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/activate.fish` & `pyswxf-0.0.2/tutorial_env/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2html.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2html4.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2html5.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2latex.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2man.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2odt.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2odt_prepstyles.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2pseudoxml.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2s5.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2xetex.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rst2xml.py` & `pyswxf-0.0.2/tutorial_env/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/bin/rstpep2html.py` & `pyswxf-0.0.2/tutorial_env/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/_cffi_backend.cpython-37m-x86_64-linux-gnu.so` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/_cffi_backend.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/SecretStorage-3.3.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/callbacks.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/css_sanitizer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/css_sanitizer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/html5lib_shim.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/html5lib_shim.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/linkifier.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/linkifier.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/sanitizer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/sanitizer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/README.rst` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/README.rst`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/parse.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/parse.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_ihatexml.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_inputstream.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_tokenizer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/constants.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/html5parser.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/serializer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/_base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/py.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/lint.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/whitespace.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/bleach-6.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/__main__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/__main__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/env.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/env.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build/util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build/util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/build-0.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/certifi-2023.5.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_errors.h` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_errors.h`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_include.h` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/_cffi_include.h`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/_embedding.h` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/_embedding.h`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/api.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/api.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/backend_ctypes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/backend_ctypes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/cffi_opcode.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/cffi_opcode.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/commontypes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/commontypes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/cparser.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/cparser.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/error.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/error.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/ffiplatform.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/ffiplatform.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/lock.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/lock.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/model.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/model.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/parse_c_type.h` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/parse_c_type.h`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/pkgconfig.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/recompiler.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/recompiler.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/setuptools_ext.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/setuptools_ext.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/vengine_cpy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/vengine_cpy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/vengine_gen.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/vengine_gen.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi/verifier.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi/verifier.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cffi-1.15.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/api.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cd.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/constant.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/legacy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.cpython-37m-x86_64-linux-gnu.so` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md__mypyc.cpython-37m-x86_64-linux-gnu.so` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/md__mypyc.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/models.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/assets/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cli/normalizer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/fernet.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/fernet.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/_oid.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/_oid.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/aead.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/aead.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/backend.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/backend.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ciphers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ciphers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/cmac.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/cmac.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/decode_asn1.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/decode_asn1.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ec.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/ec.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/rsa.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/rsa.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/backends/openssl/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust.abi3.so` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust.abi3.so`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/__init__.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/asn1.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/asn1.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/exceptions.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/ocsp.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/x509.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/x509.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dh.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dh.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x448.pyi` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/_rust/openssl/x448.pyi`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/_conditional.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/_conditional.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/binding.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/bindings/openssl/binding.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_asymmetric.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_asymmetric.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_cipheralgorithm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_cipheralgorithm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_serialization.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/_serialization.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/cmac.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/cmac.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/hashes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/hashes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/keywrap.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/keywrap.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/padding.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/padding.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dh.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dh.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dsa.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/dsa.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ec.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ec.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed25519.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed25519.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed448.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/ed448.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/padding.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/padding.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/rsa.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/rsa.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/types.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/types.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x25519.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x25519.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x448.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/asymmetric/x448.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/aead.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/aead.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/algorithms.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/algorithms.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/modes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/ciphers/modes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/concatkdf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/concatkdf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/hkdf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/hkdf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/kbkdf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/kbkdf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/pbkdf2.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/scrypt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/scrypt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/x963kdf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/kdf/x963kdf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs12.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs12.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs7.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/pkcs7.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/ssh.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/serialization/ssh.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/hotp.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/hotp.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/totp.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/hazmat/primitives/twofactor/totp.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/certificate_transparency.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/certificate_transparency.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/extensions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/extensions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/general_name.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/general_name.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/name.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/name.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/ocsp.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/ocsp.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/cryptography/x509/oid.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/cryptography/x509/oid.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/COPYING.txt` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/docutils-0.20.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_adapters.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_collections.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_functools.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_itertools.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_meta.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_py39compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_text.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/importlib_metadata-6.7.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco/classes/ancestry.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco/classes/ancestry.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco/classes/meta.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco/classes/meta.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco/classes/properties.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco/classes/properties.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/jaraco.classes-3.2.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/_properties_compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/_properties_compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backend.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backend.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/cli.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/cli.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/completion.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/completion.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/core.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/core.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/credentials.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/credentials.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/devpi_client.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/devpi_client.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/errors.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/errors.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/http.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/http.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/SecretService.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/SecretService.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/Windows.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/Windows.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/chainer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/chainer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/fail.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/fail.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/kwallet.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/kwallet.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/libsecret.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/libsecret.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/api.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/backends/macOS/api.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/testing/backend.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/testing/backend.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/testing/util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/testing/util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/util/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring/util/platform_.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring/util/platform_.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/keyring-24.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/_punycode.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/_punycode.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/main.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/main.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_block.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_block.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_core.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_core.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_inline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/parser_inline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/port.yaml` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/renderer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/renderer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/ruler.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/ruler.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/token.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/token.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/tree.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/tree.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/cli/parse.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/cli/parse.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_blocks.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_blocks.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_re.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/html_re.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/normalize_url.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/normalize_url.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/common/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/common/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_destination.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_destination.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_label.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_label.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_title.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/helpers/parse_link_title.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/commonmark.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/commonmark.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/default.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/default.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/zero.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/presets/zero.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/blockquote.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/blockquote.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/code.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/code.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/fence.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/fence.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/heading.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/heading.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/hr.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/hr.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/html_block.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/html_block.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/lheading.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/lheading.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/list.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/list.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/paragraph.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/reference.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/reference.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/state_block.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/state_block.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/table.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_block/table.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/linkify.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/linkify.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/replacements.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/replacements.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/smartquotes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/smartquotes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/state_core.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_core/state_core.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/autolink.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/autolink.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/backticks.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/backticks.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/balance_pairs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/balance_pairs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/emphasis.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/emphasis.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/entity.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/entity.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/escape.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/escape.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/html_inline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/html_inline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/image.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/image.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/link.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/link.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/newline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/newline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/state_inline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/state_inline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/strikethrough.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/strikethrough.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text_collapse.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it/rules_inline/text_collapse.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/markdown_it_py-2.2.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/mdurl-0.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_elffile.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_manylinux.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_musllinux.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_parser.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_structures.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/_tokenizer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/markers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/metadata.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/requirements.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/specifiers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/tags.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging/version.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.APACHE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.BSD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/packaging-23.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/__main__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/__pip-runner__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/build_env.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cache.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/configuration.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/pyproject.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/self_outdated_check.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/wheel_builder.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/autocompletion.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/base_command.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/cmdoptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/command_context.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main_parser.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/parser.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/progress_bars.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/req_command.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/spinners.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/cache.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/check.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/completion.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/configuration.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/debug.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/download.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/freeze.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/hash.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/help.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/index.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/inspect.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/install.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/list.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/search.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/show.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/uninstall.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/installed.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/sdist.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/collector.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/package_finder.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/sources.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_distutils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_sysconfig.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/_json.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/pkg_resources.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_dists.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_envs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/candidate.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/direct_url.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/format_control.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/index.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/installation_report.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/link.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/scheme.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/search_scope.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/selection_prefs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/target_python.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/auth.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/cache.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/download.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/lazy_wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/session.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/xmlrpc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/check.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/freeze.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/prepare.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/build_tracker.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_editable.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_editable.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/editable_legacy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/constructors.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_file.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_install.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_set.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_uninstall.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/legacy/resolver.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/base.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_jaraco_text.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_log.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/appdirs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compatibility_tags.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/deprecation.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/direct_url_helpers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/egg_link.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/encoding.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/entrypoints.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filesystem.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filetypes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/glibc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/hashes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/inject_securetransport.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/logging.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/misc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/models.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/packaging.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/setuptools_build.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/subprocess.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/temp_dir.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/unpacking.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/urls.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/virtualenv.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/bazaar.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/git.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/mercurial.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/subversion.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/versioncontrol.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/six.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/typing_extensions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/adapter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/cache.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/controller.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/serialize.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/cacert.pem` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/core.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5freq.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5prober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/chardistribution.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cp949prober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/enums.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escsm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/eucjpprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrfreq.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwfreq.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312freq.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312prober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/hebrewprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jisfreq.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabfreq.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jpcntx.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langthaimodel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/latin1prober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/macromanprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcssm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sjisprober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/universaldetector.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf1632prober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf8prober.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/languages.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansitowin32.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/initialise.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/win32.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/winterm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/database.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/index.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/locators.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/manifest.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/markers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/metadata.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/resources.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/scripts.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t32.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64-arm.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/version.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w32.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64-arm.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/distro.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/codec.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/core.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/idnadata.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/intranges.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/uts46data.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/ext.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/fallback.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/__about__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_manylinux.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_musllinux.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_structures.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/markers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/requirements.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/specifiers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/tags.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/version.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pkg_resources/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__main__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/android.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/api.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/macos.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/unix.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/windows.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/cmdline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/console.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/modeline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/plugin.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/regexopt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/scanner.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/sphinxext.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/style.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/token.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/unistring.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filters/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/groff.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/html.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/img.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/irc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/latex.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/other.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/svg.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/python.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/styles/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/actions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/common.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/core.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/helpers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/results.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/testing.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/unicode.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/_internal_utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/adapters.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/api.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/auth.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/certs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/cookies.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/help.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/hooks.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/models.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/packages.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/sessions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/status_codes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/structures.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/providers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/reporters.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/resolvers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/structs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__main__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_cell_widths.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_codes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_replace.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_export_format.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_fileno.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_inspect.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_log_render.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_loop.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_null_file.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_palettes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_ratio.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_spinners.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_win32_console.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows_renderer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_wrap.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/abc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/align.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/ansi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/bar.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/box.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/cells.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color_triplet.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/columns.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/console.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/constrain.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/containers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/control.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/default_styles.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/diagnose.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/emoji.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/errors.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/file_proxy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/filesize.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/highlighter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/json.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/jupyter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/layout.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live_render.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/logging.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/markup.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/measure.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/padding.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pager.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/palette.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/panel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pretty.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress_bar.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/prompt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/protocol.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/repr.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/rule.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/scope.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/screen.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/segment.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/spinner.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/status.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/style.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/styled.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/syntax.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/table.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/terminal_theme.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/text.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/theme.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/traceback.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/tree.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_asyncio.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/after.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before_sleep.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/nap.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/retry.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/stop.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/wait.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_parser.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_re.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/_collections.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connection.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connectionpool.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/fields.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/filepost.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/poolmanager.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/request.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/response.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/six.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/connection.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/proxy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/request.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/response.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/retry.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/timeout.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/url.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/wait.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/labels.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/mklabels.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/tests.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pip-23.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/py31compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/appdirs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/pyparsing.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/six.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/markers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/version.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources/extern/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pkg_resources-0.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/cmdline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/console.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/filter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/modeline.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/plugin.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/regexopt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/scanner.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/sphinxext.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/style.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/token.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/unistring.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/filters/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/_mapping.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/bbcode.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/groff.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/html.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/img.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/irc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/latex.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/other.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/pangomarkup.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/rtf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/svg.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal256.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_ada_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_ada_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_asy_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cl_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cocoa_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_csound_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_css_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_css_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_julia_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_julia_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lasso_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lilypond_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lilypond_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lua_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mapping.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mql_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mysql_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_mysql_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_openedge_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_php_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_postgres_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scheme_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scheme_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scilab_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_sourcemod_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stan_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stata_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_tsql_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_usd_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_usd_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vbscript_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vim_builtins.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/actionscript.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ada.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ada.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/agile.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/algebra.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ambient.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/amdgpu.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/amdgpu.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ampl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apdlexer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apdlexer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/archetype.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arrow.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arrow.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arturo.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/arturo.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/automation.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/boa.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/business.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/c_like.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/capnproto.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/carbon.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/carbon.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cddl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cddl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/chapel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/clean.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/comal.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/comal.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/compiled.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/configs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/console.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cplint.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/cplint.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/crystal.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/csound.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/css.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/d.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dalvik.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/data.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dax.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dax.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/devicetree.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/devicetree.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/diff.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dotnet.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dsls.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dylan.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ecl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elpi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/elpi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/email.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/erlang.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/esoteric.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ezhil.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/factor.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fantom.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/felix.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fift.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fift.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/floscript.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/forth.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fortran.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/foxpro.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/freefem.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/func.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/func.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/functional.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/futhark.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/futhark.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gcodelexer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gcodelexer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gdscript.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gdscript.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/grammar_notation.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graph.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphics.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphviz.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/graphviz.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gsql.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/gsql.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haskell.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haxe.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/hdl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/idl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/igor.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/inferno.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/installers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/iolang.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/javascript.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jmespath.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jmespath.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jslt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jslt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jsonnet.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/julia.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jvm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/kuin.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/kuin.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/lisp.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/macaulay2.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/macaulay2.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/make.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/markup.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/math.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/maxima.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/maxima.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/meson.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/meson.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/minecraft.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/minecraft.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mips.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mips.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modeling.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modula2.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/monte.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mosel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/mosel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ncl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nit.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nix.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/oberon.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/objective.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ooc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/other.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parasail.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parsers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pawn.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/perl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/phix.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/phix.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/php.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pointless.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/pointless.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/praat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/procfile.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/procfile.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/prolog.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/promql.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/promql.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/python.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/qvt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/r.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rdf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rebol.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/resource.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ride.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ride.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rita.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rita.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rnc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/roboconf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/robotframework.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ruby.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rust.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sas.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/savi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/savi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scdoc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scripting.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sgf.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/shell.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sieve.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sieve.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/slash.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smalltalk.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smithy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smithy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smv.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/snobol.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/solidity.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sophia.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sophia.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/special.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/spice.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/spice.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sql.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/supercollider.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tal.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tal.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tcl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teal.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teal.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/templates.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teraterm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/testing.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/text.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textedit.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textfmts.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/theorem.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/thingsdb.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/thingsdb.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tlb.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tlb.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tnt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/tnt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/trafficscript.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/typoscript.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ul4.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/ul4.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/unicon.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/urbi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/usd.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/usd.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/varnish.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/verification.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/web.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webassembly.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webassembly.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webidl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webidl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webmisc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wgsl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wgsl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/whiley.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wowtoc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wowtoc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wren.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/wren.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/x10.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/xorg.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/yang.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/yang.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pygments/lexers/zig.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_impl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/_in_process.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/__about__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/__about__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/__main__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/__main__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/clean.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/clean.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/markdown.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/markdown.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/rst.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/rst.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer/txt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer/txt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/readme_renderer-37.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/_internal_utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/adapters.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/api.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/auth.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/cookies.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/help.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/hooks.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/models.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/packages.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/sessions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/status_codes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/structures.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests-2.31.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/_compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/_compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/sessions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/sessions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/streaming_iterator.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/appengine.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/appengine.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/fingerprint.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/fingerprint.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/host_header_ssl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/host_header_ssl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/socket_options.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/socket_options.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/source.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/source.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/ssl.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/ssl.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/x509.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/adapters/x509.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/_digest_auth_compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/_digest_auth_compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/guess.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/guess.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/handler.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/handler.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/http_proxy_digest.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/auth/http_proxy_digest.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/stream.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/stream.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/tee.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/downloadutils/tee.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/decoder.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/encoder.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/pool.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/pool.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/thread.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/threaded/thread.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/deprecated.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/dump.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/dump.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/formdata.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/formdata.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/user_agent.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/_mixin.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/_mixin.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/abnf_regexp.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/abnf_regexp.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/api.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/api.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/builder.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/builder.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/iri.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/iri.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/misc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/misc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/normalizers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/normalizers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/parseresult.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/parseresult.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/uri.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/uri.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986/validators.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986/validators.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rfc3986-2.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/__main__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_cell_widths.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_emoji_codes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_emoji_replace.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_export_format.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_fileno.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_inspect.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_log_render.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_loop.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_null_file.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_palettes.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_ratio.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_spinners.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_win32_console.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_windows.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_windows_renderer.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/_wrap.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/abc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/align.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/align.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/ansi.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/bar.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/box.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/box.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/cells.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/color.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/color.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/color_triplet.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/columns.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/console.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/console.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/constrain.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/containers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/control.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/control.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/default_styles.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/diagnose.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/emoji.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/errors.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/file_proxy.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/filesize.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/highlighter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/json.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/json.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/jupyter.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/layout.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/live.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/live.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/live_render.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/logging.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/markdown.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/markup.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/measure.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/padding.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/pager.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/palette.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/panel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/pretty.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/progress.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/progress_bar.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/prompt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/protocol.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/repr.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/rule.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/scope.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/screen.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/segment.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/spinner.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/status.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/status.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/style.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/style.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/styled.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/syntax.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/table.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/table.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/terminal_theme.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/text.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/text.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/theme.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/traceback.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich/tree.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/rich-13.4.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/archive_util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/build_meta.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/cli-32.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/cli-64.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/cli.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/config.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/dep_util.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/depends.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/dist.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/extension.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/glibc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/glibc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/glob.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/gui-32.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/gui-64.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/gui.exe` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/launch.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/lib2to3_ex.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/monkey.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/msvc.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/namespaces.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/package_index.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/pep425tags.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/pep425tags.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py27compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py27compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py31compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py31compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py33compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py33compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/py36compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/py36compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/sandbox.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/site-patch.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/site-patch.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/ssl_support.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/ssl_support.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/unicode_utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/windows_support.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/pyparsing.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/six.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__about__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_structures.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/markers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/requirements.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/specifiers.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/version.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/alias.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_egg.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_rpm.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_wininst.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_clib.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_ext.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_py.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/develop.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/dist_info.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/easy_install.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/egg_info.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_egg_info.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_lib.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_scripts.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/launcher manifest.xml` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/py36compat.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/rotate.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/saveopts.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/sdist.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/setopt.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/test.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload_docs.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools/extern/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/DESCRIPTION.rst` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/entry_points.txt` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/metadata.json` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/setuptools-39.0.1.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/six-1.16.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli/_parser.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli/_re.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/tomli-2.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/__main__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/__main__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/auth.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/auth.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/cli.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/cli.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/exceptions.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/package.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/package.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/repository.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/repository.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/settings.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/settings.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/utils.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/wheel.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/wheel.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/wininst.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/wininst.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/check.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/check.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/register.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/register.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine/commands/upload.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine/commands/upload.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/twine-4.0.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/typing_extensions-4.7.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp/__init__.py` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/LICENSE` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/METADATA` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/RECORD` & `pyswxf-0.0.2/tutorial_env/lib/python3.7/site-packages/zipp-3.15.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/LICENSE` & `pyswxf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.0.1/pyproject.toml` & `pyswxf-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "pySWXF"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
 	{name="Laurence Lurio", email="llurio@niu.edu" },
 ]
 description = "Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity"
 readme = "README.md"
 requires-python = ">3.7"
 classifiers = [
```

### Comparing `pyswxf-0.0.1/PKG-INFO` & `pyswxf-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySWXF
-Version: 0.0.1
+Version: 0.0.2
 Summary: Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Laurence Lurio <llurio@niu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

