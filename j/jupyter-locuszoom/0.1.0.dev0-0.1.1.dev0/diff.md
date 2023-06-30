# Comparing `tmp/jupyter_locuszoom-0.1.0.dev0.tar.gz` & `tmp/jupyter_locuszoom-0.1.1.dev0.tar.gz`

## Comparing `jupyter_locuszoom-0.1.0.dev0.tar` & `jupyter_locuszoom-0.1.1.dev0.tar`

### file list

```diff
@@ -1,138 +1,78 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/.prettierrc
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/MANIFEST.in
--rw-r--r--   0        0        0    13593 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/Untitled.ipynb
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/install.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jest.config.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom.json
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/package.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/pytest.ini
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/tsconfig.json
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/webpack.config.js
--rw-r--r--   0        0        0   346793 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/yarn.lock
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/css/widget.css
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/_frontend.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/_version.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/locus_zoom.py
--rw-r--r--   0        0        0    21318 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/build_log.json
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/package.json
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_index_js.1462f2843f4c04a52881.js
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_index_js.1462f2843f4c04a52881.js.map
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_index_js.d2339fe266cabc7f3ebc.js
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_index_js.d2339fe266cabc7f3ebc.js.map
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.68f86ed0f284bae73ee7.js
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.68f86ed0f284bae73ee7.js.map
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.7e633c522b2189389736.js
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.7e633c522b2189389736.js.map
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.abcb39077817d9f5e5c0.js
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.abcb39077817d9f5e5c0.js.map
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.031ff8058d8d31610ff4.js
--rw-r--r--   0        0        0    12520 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.031ff8058d8d31610ff4.js.map
--rw-r--r--   0        0        0    12832 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.0623db0f7d3c07125290.js
--rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.0623db0f7d3c07125290.js.map
--rw-r--r--   0        0        0    12834 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.19c75a6eec62583a7167.js
--rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.19c75a6eec62583a7167.js.map
--rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.1de32fa6eec660baca88.js
--rw-r--r--   0        0        0    12380 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.1de32fa6eec660baca88.js.map
--rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2b66441289369f8600c8.js
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2b66441289369f8600c8.js.map
--rw-r--r--   0        0        0    12535 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2bf13a2b62c6e59e7386.js
--rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2bf13a2b62c6e59e7386.js.map
--rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.4dd25bf992348c7ee2aa.js
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.4dd25bf992348c7ee2aa.js.map
--rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.606f97136d9daa583196.js
--rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.606f97136d9daa583196.js.map
--rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.64b17e31e6293d303ab7.js
--rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.64b17e31e6293d303ab7.js.map
--rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.6d9b779a0e9408e22a1d.js
--rw-r--r--   0        0        0    12379 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.6d9b779a0e9408e22a1d.js.map
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.6e425a6c4d8cfd3a31e0.js
--rw-r--r--   0        0        0    12517 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.6e425a6c4d8cfd3a31e0.js.map
--rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.81e08279fe4b0adaaf61.js
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.81e08279fe4b0adaaf61.js.map
--rw-r--r--   0        0        0    12862 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.918a8f0e01a3404fc095.js
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.918a8f0e01a3404fc095.js.map
--rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.9b2c61bbd001346eef96.js
--rw-r--r--   0        0        0    11064 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.9b2c61bbd001346eef96.js.map
--rw-r--r--   0        0        0    12425 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.9cddcf818523b2bcc6d9.js
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.9cddcf818523b2bcc6d9.js.map
--rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.a1298431a7d62cadbcf0.js
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.a1298431a7d62cadbcf0.js.map
--rw-r--r--   0        0        0    17305 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.a1664a9d7724f48c1ea5.js
--rw-r--r--   0        0        0    16485 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.a1664a9d7724f48c1ea5.js.map
--rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.cace536d8c00a83cb1c0.js
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.cace536d8c00a83cb1c0.js.map
--rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.d56b5082cb3b61badea2.js
--rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.d56b5082cb3b61badea2.js.map
--rw-r--r--   0        0        0    13042 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.de2f37af2c0d8baa33d7.js
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.de2f37af2c0d8baa33d7.js.map
--rw-r--r--   0        0        0    12218 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.e9372078d9076bd5c48d.js
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.e9372078d9076bd5c48d.js.map
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ea252ff7eb1fab502c50.js
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ea252ff7eb1fab502c50.js.map
--rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ea32ee74764dc488341a.js
--rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ea32ee74764dc488341a.js.map
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.eadf6ecf6ca0ff8a0a10.js
--rw-r--r--   0        0        0    12737 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.eadf6ecf6ca0ff8a0a10.js.map
--rw-r--r--   0        0        0    12778 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ec541c78db92f327b738.js
--rw-r--r--   0        0        0    12466 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ec541c78db92f327b738.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.1629023844841c0a9ae9.js.map
--rw-r--r--   0        0        0    28750 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.1aa611838b67c7e01bd2.js
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.1aa611838b67c7e01bd2.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.20eb474b851c8a21381e.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.2a585e92942f2727413c.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.3005a39789aa770403fd.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.32b5350f76df71fc343e.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.38f37b6bb3476b64bbf7.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.443305058db5a89036de.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.4c8488b4f7384b98d2aa.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.535a63d55ec89549b827.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.6e9b772671a8ef8348b1.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.8d9dc161c6a98ea0895a.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.9442631447559c5f3c1f.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.955e596c68116f7732f0.js.map
--rw-r--r--   0        0        0    25416 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.98859b7e603315a04340.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.9f53c0aff5b0e2a19fbc.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.a305fbf5b45accc4759c.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.a63bde28acfd4eb009be.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.a8af7ab576ef7d9b2d32.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.b68369816a614d790269.js.map
--rw-r--r--   0        0        0    25416 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.cf3065b6cb35f65ed995.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.dcc60fbe7c0f222be4db.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.dd9bd4de4c11dcd42857.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.e01ee10839c6d05ae3c4.js.map
--rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.e1ac7ed65b505e5dc83b.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/style.js
--rw-r--r--   0        0        0    32151 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js
--rw-r--r--   0        0        0    37977 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js.map
--rw-r--r--   0        0        0  1851079 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js
--rw-r--r--   0        0        0  1462234 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js.map
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/nbextension/extension.js
--rw-r--r--   0        0        0  1920857 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/nbextension/index.js
--rw-r--r--   0        0        0  1545476 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/tests/__init__.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/tests/conftest.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/tests/test_example.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/extension.ts
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/index.ts
--rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/locuszoom.d.ts
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/plugin.ts
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/utils.ts
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/version.ts
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/widget.ts
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/LICENSE.txt
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/README.md
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/.prettierrc
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/MANIFEST.in
+-rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/Untitled.ipynb
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/install.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jest.config.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom.json
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/package.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/pytest.ini
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/tsconfig.json
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/webpack.config.js
+-rw-r--r--   0        0        0   346793 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/yarn.lock
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/css/widget.css
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/_frontend.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/_version.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/locus_zoom.py
+-rw-r--r--   0        0        0    21317 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/build_log.json
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/package.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_index_js.1462f2843f4c04a52881.js
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_index_js.1462f2843f4c04a52881.js.map
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.7e633c522b2189389736.js
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.7e633c522b2189389736.js.map
+-rw-r--r--   0        0        0    14991 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.751b11392fdca570e288.js
+-rw-r--r--   0        0        0    14642 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.751b11392fdca570e288.js.map
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.b631ee8a6ff24aede47c.js
+-rw-r--r--   0        0        0    14476 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.b631ee8a6ff24aede47c.js.map
+-rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.d278f1d07325a0e4e5cb.js
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.d278f1d07325a0e4e5cb.js.map
+-rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.dc6697cf94dcc4cb14bc.js
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.dc6697cf94dcc4cb14bc.js.map
+-rw-r--r--   0        0        0    14953 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.e00d9776199cdb3b0918.js
+-rw-r--r--   0        0        0    14475 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.e00d9776199cdb3b0918.js.map
+-rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff0b505f89816ef2fa6c.js
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff0b505f89816ef2fa6c.js.map
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff612b296119c6362583.js
+-rw-r--r--   0        0        0    14476 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff612b296119c6362583.js.map
+-rw-r--r--   0        0        0    28750 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.03af74c81e37b8d85832.js
+-rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.03af74c81e37b8d85832.js.map
+-rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.32f59f51d40bf5ffa01e.js.map
+-rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.35a953c4bbbdf71b3939.js.map
+-rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.76e640dbe79737ef23c4.js.map
+-rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.844efee5a11f0506b968.js.map
+-rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.e1d041ac7fb699acd6d5.js.map
+-rw-r--r--   0        0        0    27502 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.e681d2c3e869ee437176.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/style.js
+-rw-r--r--   0        0        0    32151 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js
+-rw-r--r--   0        0        0    37977 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js.map
+-rw-r--r--   0        0        0  1851079 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js
+-rw-r--r--   0        0        0  1462234 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js.map
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/nbextension/extension.js
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/nbextension/index.js
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/tests/__init__.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/tests/conftest.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/tests/test_example.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/extension.ts
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/index.ts
+-rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/locuszoom.d.ts
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/plugin.ts
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/utils.ts
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/version.ts
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/widget.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/LICENSE.txt
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/README.md
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 jupyter_locuszoom-0.1.1.dev0/PKG-INFO
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/.eslintrc.js` & `jupyter_locuszoom-0.1.1.dev0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/MANIFEST.in` & `jupyter_locuszoom-0.1.1.dev0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/Untitled.ipynb` & `jupyter_locuszoom-0.1.1.dev0/Untitled.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883357242555831%*

 * *Differences: {"'cells'": "{0: {'execution_count': 28, 'metadata': {'execution': {'iopub.execute_input': "*

 * *            "'2023-06-30T09:49:17.064299Z', 'iopub.status.busy': '2023-06-30T09:49:17.063346Z', "*

 * *            "'iopub.status.idle': '2023-06-30T09:49:17.190090Z', 'shell.execute_reply': "*

 * *            "'2023-06-30T09:49:17.189138Z', 'shell.execute_reply.started': "*

 * *            "'2023-06-30T09:49:17.064247Z'}}, 'outputs': [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['The autore […]*

```diff
@@ -1,127 +1,124 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 28,
             "id": "57e7f19f-8932-4e0c-a81b-fd90398bbd47",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:07:19.505958Z",
-                    "iopub.status.busy": "2023-06-29T14:07:19.505630Z",
-                    "iopub.status.idle": "2023-06-29T14:07:19.541770Z",
-                    "shell.execute_reply": "2023-06-29T14:07:19.540820Z",
-                    "shell.execute_reply.started": "2023-06-29T14:07:19.505926Z"
+                    "iopub.execute_input": "2023-06-30T09:49:17.064299Z",
+                    "iopub.status.busy": "2023-06-30T09:49:17.063346Z",
+                    "iopub.status.idle": "2023-06-30T09:49:17.190090Z",
+                    "shell.execute_reply": "2023-06-30T09:49:17.189138Z",
+                    "shell.execute_reply.started": "2023-06-30T09:49:17.064247Z"
                 },
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "The autoreload extension is already loaded. To reload it, use:\n",
+                        "  %reload_ext autoreload\n"
+                    ]
+                }
+            ],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 29,
             "id": "f62b5722-27f6-43e8-95c3-83d2e9777735",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:07:19.545038Z",
-                    "iopub.status.busy": "2023-06-29T14:07:19.544253Z",
-                    "iopub.status.idle": "2023-06-29T14:07:19.562793Z",
-                    "shell.execute_reply": "2023-06-29T14:07:19.561846Z",
-                    "shell.execute_reply.started": "2023-06-29T14:07:19.545002Z"
+                    "iopub.execute_input": "2023-06-30T09:49:17.757422Z",
+                    "iopub.status.busy": "2023-06-30T09:49:17.756694Z",
+                    "iopub.status.idle": "2023-06-30T09:49:17.774696Z",
+                    "shell.execute_reply": "2023-06-30T09:49:17.773741Z",
+                    "shell.execute_reply.started": "2023-06-30T09:49:17.757388Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "#%pip install pandas zstandard"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 30,
             "id": "015ee7b4-744b-4be0-b5ab-048731598676",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:07:19.565411Z",
-                    "iopub.status.busy": "2023-06-29T14:07:19.564012Z",
-                    "iopub.status.idle": "2023-06-29T14:07:19.980948Z",
-                    "shell.execute_reply": "2023-06-29T14:07:19.979954Z",
-                    "shell.execute_reply.started": "2023-06-29T14:07:19.564970Z"
+                    "iopub.execute_input": "2023-06-30T09:49:18.164062Z",
+                    "iopub.status.busy": "2023-06-30T09:49:18.163175Z",
+                    "iopub.status.idle": "2023-06-30T09:49:18.181368Z",
+                    "shell.execute_reply": "2023-06-30T09:49:18.180434Z",
+                    "shell.execute_reply.started": "2023-06-30T09:49:18.164028Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import pandas as pd"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": null,
             "id": "6bf014c1-b378-49a1-8605-ae3a54fd9267",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:26:20.952367Z",
-                    "iopub.status.busy": "2023-06-29T14:26:20.951770Z",
-                    "iopub.status.idle": "2023-06-29T14:26:39.471377Z",
-                    "shell.execute_reply": "2023-06-29T14:26:39.470455Z",
-                    "shell.execute_reply.started": "2023-06-29T14:26:20.952331Z"
+                    "iopub.execute_input": "2023-06-30T09:49:50.207064Z",
+                    "iopub.status.busy": "2023-06-30T09:49:50.206689Z"
                 },
                 "tags": []
             },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/tmp/ipykernel_309284/3026281591.py:1: DtypeWarning: Columns (0) have mixed types. Specify dtype option on import or set low_memory=False.\n",
-                        "  assoc = pd.read_table('data/phenotype.NRS_Worst_period_pain_during_last_period.glm.linear.zst').rename({\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "assoc = pd.read_table('data/phenotype.NRS_Worst_period_pain_during_last_period.glm.linear.zst').drop(columns=['ID'])"
+                "assoc = pd.read_table('~/pelvic_pain/data/from_cluster/phenotype.NRS_Worst_period_pain_during_last_period.glm.linear.zst').drop(columns=['ID'])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 35,
             "id": "12ab90c5-65be-4fb9-b0f5-7a1970edd050",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:26:59.490065Z",
-                    "iopub.status.busy": "2023-06-29T14:26:59.489273Z",
-                    "iopub.status.idle": "2023-06-29T14:26:59.921950Z",
-                    "shell.execute_reply": "2023-06-29T14:26:59.921022Z",
-                    "shell.execute_reply.started": "2023-06-29T14:26:59.490016Z"
+                    "iopub.execute_input": "2023-06-30T09:50:19.806856Z",
+                    "iopub.status.busy": "2023-06-30T09:50:19.806373Z",
+                    "iopub.status.idle": "2023-06-30T09:50:20.261428Z",
+                    "shell.execute_reply": "2023-06-30T09:50:20.260699Z",
+                    "shell.execute_reply.started": "2023-06-30T09:50:19.806810Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "assoc = assoc.rename(columns={\n",
                 "    '#CHROM': 'CHROM'\n",
                 "})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 36,
             "id": "033b4b4c-9b64-4a0f-ba57-7c1a10811627",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:07:32.459260Z",
-                    "iopub.status.busy": "2023-06-29T14:07:32.458234Z",
-                    "iopub.status.idle": "2023-06-29T14:07:36.847332Z",
-                    "shell.execute_reply": "2023-06-29T14:07:36.846379Z",
-                    "shell.execute_reply.started": "2023-06-29T14:07:32.459212Z"
+                    "iopub.execute_input": "2023-06-30T09:50:20.263578Z",
+                    "iopub.status.busy": "2023-06-30T09:50:20.262949Z",
+                    "iopub.status.idle": "2023-06-30T09:50:24.120999Z",
+                    "shell.execute_reply": "2023-06-30T09:50:24.119886Z",
+                    "shell.execute_reply.started": "2023-06-30T09:50:20.263545Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
@@ -139,17 +136,16 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>#CHROM</th>\n",
+                            "      <th>CHROM</th>\n",
                             "      <th>POS</th>\n",
-                            "      <th>ID</th>\n",
                             "      <th>REF</th>\n",
                             "      <th>ALT</th>\n",
                             "      <th>A1</th>\n",
                             "      <th>TEST</th>\n",
                             "      <th>OBS_CT</th>\n",
                             "      <th>BETA</th>\n",
                             "      <th>SE</th>\n",
@@ -160,15 +156,14 @@
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>5144362</th>\n",
                             "      <td>15</td>\n",
                             "      <td>22609561</td>\n",
-                            "      <td>chr15:22609561:G:A</td>\n",
                             "      <td>G</td>\n",
                             "      <td>A</td>\n",
                             "      <td>A</td>\n",
                             "      <td>ADD</td>\n",
                             "      <td>626</td>\n",
                             "      <td>1.25594</td>\n",
                             "      <td>0.208805</td>\n",
@@ -177,15 +172,14 @@
                             "      <td>6.01486</td>\n",
                             "      <td>8.50923</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5144366</th>\n",
                             "      <td>15</td>\n",
                             "      <td>22613826</td>\n",
-                            "      <td>chr15:22613826:T:C</td>\n",
                             "      <td>T</td>\n",
                             "      <td>C</td>\n",
                             "      <td>C</td>\n",
                             "      <td>ADD</td>\n",
                             "      <td>626</td>\n",
                             "      <td>1.25594</td>\n",
                             "      <td>0.208805</td>\n",
@@ -194,15 +188,14 @@
                             "      <td>6.01486</td>\n",
                             "      <td>8.50923</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5144365</th>\n",
                             "      <td>15</td>\n",
                             "      <td>22611676</td>\n",
-                            "      <td>chr15:22611676:C:G</td>\n",
                             "      <td>C</td>\n",
                             "      <td>G</td>\n",
                             "      <td>G</td>\n",
                             "      <td>ADD</td>\n",
                             "      <td>626</td>\n",
                             "      <td>1.24663</td>\n",
                             "      <td>0.211012</td>\n",
@@ -211,15 +204,14 @@
                             "      <td>5.90787</td>\n",
                             "      <td>8.24043</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3590531</th>\n",
                             "      <td>9</td>\n",
                             "      <td>64851643</td>\n",
-                            "      <td>chr9:64851643:T:C</td>\n",
                             "      <td>T</td>\n",
                             "      <td>C</td>\n",
                             "      <td>C</td>\n",
                             "      <td>ADD</td>\n",
                             "      <td>626</td>\n",
                             "      <td>1.30305</td>\n",
                             "      <td>0.231133</td>\n",
@@ -228,15 +220,14 @@
                             "      <td>5.63768</td>\n",
                             "      <td>7.57978</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3590542</th>\n",
                             "      <td>9</td>\n",
                             "      <td>65067398</td>\n",
-                            "      <td>chr9:65067398:T:G</td>\n",
                             "      <td>T</td>\n",
                             "      <td>G</td>\n",
                             "      <td>G</td>\n",
                             "      <td>ADD</td>\n",
                             "      <td>626</td>\n",
                             "      <td>1.16528</td>\n",
                             "      <td>0.210540</td>\n",
@@ -246,99 +237,118 @@
                             "      <td>7.33495</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "        #CHROM       POS                  ID REF ALT A1 TEST  OBS_CT     BETA  \\\n",
-                            "5144362     15  22609561  chr15:22609561:G:A   G   A  A  ADD     626  1.25594   \n",
-                            "5144366     15  22613826  chr15:22613826:T:C   T   C  C  ADD     626  1.25594   \n",
-                            "5144365     15  22611676  chr15:22611676:C:G   C   G  G  ADD     626  1.24663   \n",
-                            "3590531      9  64851643   chr9:64851643:T:C   T   C  C  ADD     626  1.30305   \n",
-                            "3590542      9  65067398   chr9:65067398:T:G   T   G  G  ADD     626  1.16528   \n",
+                            "        CHROM       POS REF ALT A1 TEST  OBS_CT     BETA        SE       L95  \\\n",
+                            "5144362    15  22609561   G   A  A  ADD     626  1.25594  0.208805  0.846685   \n",
+                            "5144366    15  22613826   T   C  C  ADD     626  1.25594  0.208805  0.846685   \n",
+                            "5144365    15  22611676   C   G  G  ADD     626  1.24663  0.211012  0.833058   \n",
+                            "3590531     9  64851643   T   C  C  ADD     626  1.30305  0.231133  0.850041   \n",
+                            "3590542     9  65067398   T   G  G  ADD     626  1.16528  0.210540  0.752631   \n",
                             "\n",
-                            "               SE       L95      U95   T_STAT  LOG10_P  \n",
-                            "5144362  0.208805  0.846685  1.66519  6.01486  8.50923  \n",
-                            "5144366  0.208805  0.846685  1.66519  6.01486  8.50923  \n",
-                            "5144365  0.211012  0.833058  1.66021  5.90787  8.24043  \n",
-                            "3590531  0.231133  0.850041  1.75606  5.63768  7.57978  \n",
-                            "3590542  0.210540  0.752631  1.57793  5.53474  7.33495  "
+                            "             U95   T_STAT  LOG10_P  \n",
+                            "5144362  1.66519  6.01486  8.50923  \n",
+                            "5144366  1.66519  6.01486  8.50923  \n",
+                            "5144365  1.66021  5.90787  8.24043  \n",
+                            "3590531  1.75606  5.63768  7.57978  \n",
+                            "3590542  1.57793  5.53474  7.33495  "
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 36,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "assoc.sort_values('LOG10_P', ascending=False).head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 40,
             "id": "c0888990-7f2e-4130-8558-6833b48ffca9",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:27:11.263936Z",
-                    "iopub.status.busy": "2023-06-29T14:27:11.263442Z",
-                    "iopub.status.idle": "2023-06-29T14:27:11.281926Z",
-                    "shell.execute_reply": "2023-06-29T14:27:11.281024Z",
-                    "shell.execute_reply.started": "2023-06-29T14:27:11.263905Z"
+                    "iopub.execute_input": "2023-06-30T09:51:38.906978Z",
+                    "iopub.status.busy": "2023-06-30T09:51:38.906302Z",
+                    "iopub.status.idle": "2023-06-30T09:51:39.051066Z",
+                    "shell.execute_reply": "2023-06-30T09:51:39.050137Z",
+                    "shell.execute_reply.started": "2023-06-30T09:51:38.906946Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from jupyter_locuszoom import LocusZoom"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 41,
             "id": "2ab6371b-20f0-4a2f-8140-4b9cf37cbe88",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:27:11.449926Z",
-                    "iopub.status.busy": "2023-06-29T14:27:11.449299Z",
-                    "iopub.status.idle": "2023-06-29T14:27:11.470293Z",
-                    "shell.execute_reply": "2023-06-29T14:27:11.469251Z",
-                    "shell.execute_reply.started": "2023-06-29T14:27:11.449891Z"
+                    "iopub.execute_input": "2023-06-30T09:51:39.279165Z",
+                    "iopub.status.busy": "2023-06-30T09:51:39.278226Z",
+                    "iopub.status.idle": "2023-06-30T09:51:39.308916Z",
+                    "shell.execute_reply": "2023-06-30T09:51:39.307624Z",
+                    "shell.execute_reply.started": "2023-06-30T09:51:39.279116Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "'CHROM,POS,REF,ALT,A1,TEST,OBS_CT,BETA,SE,L95,U95,T_STAT,LOG10_P'"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 41,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "','.join(assoc.columns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 44,
             "id": "f7d7257b-1be8-4f01-bd05-ff905f2ba6d5",
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-29T14:27:11.603492Z",
-                    "iopub.status.busy": "2023-06-29T14:27:11.602674Z"
+                    "iopub.execute_input": "2023-06-30T10:05:18.401198Z",
+                    "iopub.status.busy": "2023-06-30T10:05:18.400867Z",
+                    "iopub.status.idle": "2023-06-30T10:05:28.795076Z",
+                    "shell.execute_reply": "2023-06-30T10:05:28.793965Z",
+                    "shell.execute_reply.started": "2023-06-30T10:05:18.401174Z"
                 },
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "9e4422318481465382299cdc89f8d35b",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "LocusZoom(position={'chr': '1', 'start': 13732560, 'end': 14232560})"
+                        ]
+                    },
+                    "execution_count": 44,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "LocusZoom(\n",
                 "    assoc,\n",
                 "    chrom='1',\n",
                 "    build='GRCh38'\n",
                 ")"
             ]
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/package.json` & `jupyter_locuszoom-0.1.1.dev0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -88,9 +88,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/tsconfig.json` & `jupyter_locuszoom-0.1.1.dev0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/webpack.config.js` & `jupyter_locuszoom-0.1.1.dev0/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/yarn.lock` & `jupyter_locuszoom-0.1.1.dev0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/__init__.py` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/locus_zoom.py` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/locus_zoom.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,16 +88,17 @@
         }
         # TODO check overlap
         associations = associations.rename(columns=tolerance)
         required_columns = ['ref_allele', 'ALT', 'chr', 'position']
         for required_column in required_columns:
             if required_column not in associations.columns:
               raise ValueError(f'Required column missing: {required_column}')
-        # harmonise type
+        # harmonise type - TODO do not cast if already string
         associations['chr'] = associations['chr'].astype(str)
+        # TODO: coerce position to integer if not already
         if 'log_pvalue' not in associations.columns:
             if 'pvalue' in associations.columns:
                 from math import log10
                 associations['log_pvalue'] = -associations['pvalue'].apply(log10)
             else:
                 raise ValueError('Neither `pvalue` nor log_pvalue (recommended) is in columns')
 
@@ -106,26 +107,31 @@
             + ':' + associations['position'].apply(str)
             + '_' + associations['ref_allele']
             + '/' + associations['ALT']
         )
         # not needed, but could be fun to implement multi-analysis
         # associations['analysis'] = 0
         self._associations = associations
+        self._by_chrom = associations.groupby('chr')
         #self._update_view();
 
     def _update_view(self):
         # TODO use tabix?
-        filtered = self._associations[
-          (self._associations.chr == self.position['chr'])
+        query_range = self.position
+        df = self._by_chrom.get_group(query_range['chr'])
+        filtered = df[
+          (df.position >= query_range['start'])
           &
-          (self._associations.position >= self.position['start'])
-          &
-          (self._associations.position <= self.position['end'])
+          (df.position <= query_range['end'])
         ]
-        self._associations_view = filtered.to_dict(orient='list')
+        data_dict = {
+          'data': filtered.to_dict(orient='list'),
+          'range': query_range
+        }
+        self._associations_view = data_dict
 
     _associations_view = Dict().tag(sync=True)
     build = Unicode('GRCh38').tag(sync=True)
     position: DictType = Dict(
       {},
       per_key_traits={'chr': Unicode(), 'start': Integer(), 'end': Integer()}
     ).tag(sync=True)
@@ -169,8 +175,8 @@
 
     @chrom.setter
     def chrom(self, value):
         self.position = {
           **self.position,
           'chr': value
         }
-    """
+    """
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/build_log.json` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {'0': "{'bail': True}"}*

```diff
@@ -1,10 +1,10 @@
 [
     {
-        "bail": false,
+        "bail": true,
         "devtool": "source-map",
         "entry": {},
         "mode": "development",
         "module": {
             "rules": [
                 {
                     "test": {},
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/package.json` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990234375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.03af74c81e37b8d85832.js'}}"}*

```diff
@@ -47,15 +47,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/krassowski/jupyter-locuszoom",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1aa611838b67c7e01bd2.js"
+            "load": "static/remoteEntry.03af74c81e37b8d85832.js"
         },
         "extension": "lib/plugin",
         "outputDir": "jupyter_locuszoom/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_index_js.1462f2843f4c04a52881.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_index_js.1462f2843f4c04a52881.js`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.68f86ed0f284bae73ee7.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.7e633c522b2189389736.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -46,25 +46,25 @@
                     value: true
                 }));
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const widgetExports = __importStar(__webpack_require__( /*! ./widget */ "./lib/widget.js"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
                 const EXTENSION_ID = 'jupyter-locuszoom:plugin';
                 /**
-                 * The example plugin.
+                 * The widget plugin.
                  */
-                const examplePlugin = {
+                const plugin = {
                     id: EXTENSION_ID,
                     requires: [base_1.IJupyterWidgetRegistry],
                     activate: activateWidgetExtension,
                     autoStart: true,
                 };
                 // the "as unknown as ..." typecast above is solely to support JupyterLab 1
                 // and 2 in the same codebase and should be removed when we migrate to Lumino.
-                exports["default"] = examplePlugin;
+                exports["default"] = plugin;
                 /**
                  * Activate the widget extension.
                  */
                 function activateWidgetExtension(app, registry) {
                     registry.registerWidget({
                         name: version_1.MODULE_NAME,
                         version: version_1.MODULE_VERSION,
@@ -74,8 +74,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_plugin_js.68f86ed0f284bae73ee7.js.map
+//# sourceMappingURL=lib_plugin_js.7e633c522b2189389736.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.68f86ed0f284bae73ee7.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_plugin_js.7e633c522b2189389736.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'lib_plugin_js.7e633c522b2189389736.js'",*

 * * "'mappings'": "';;;;;;;;;;AAAA,kCAAkC;AAClC,2DAA2D;;;;;;;;;;;;;;;;;;;;;AAM3D,yHAA+D;AAE/D,2FAA0C;AAE1C,2EAAwD;AAExD,MAAM,YAAY,GAAG,0BAA0B,CAAC;AAEhD;;GAEG;AACH,MAAM,MAAM,GAAuC;IACjD,EAAE,EAAE,YAAY;IAChB,QAAQ,EAAE,CAAC,6BAAsB,CAAC;IAClC,QAAQ,EAAE,uBAAuB;IACjC,SAAS,EAAE,IAAI;CACiC,CAAC;AACnD,2EAA2E;AAC3E,8EAA8E;AAE9E,qBAAe,MAAM,CAAC;AAEtB;;GAEG;AACH,SAAS,uBAAuB,CAC9B,GAAwB,EACxB,QAAgC;IAEhC,QAAQ,CAAC,cAAc,CAAC;QACtB,IAAI,EAAE,qBAAW;QACjB,OAAO,EAAE,wBAAc;Q […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "lib_plugin_js.68f86ed0f284bae73ee7.js",
-    "mappings": ";;;;;;;;;;AAAA,kCAAkC;AAClC,2DAA2D;;;;;;;;;;;;;;;;;;;;;AAM3D,yHAA+D;AAE/D,2FAA0C;AAE1C,2EAAwD;AAExD,MAAM,YAAY,GAAG,0BAA0B,CAAC;AAEhD;;GAEG;AACH,MAAM,aAAa,GAAuC;IACxD,EAAE,EAAE,YAAY;IAChB,QAAQ,EAAE,CAAC,6BAAsB,CAAC;IAClC,QAAQ,EAAE,uBAAuB;IACjC,SAAS,EAAE,IAAI;CACiC,CAAC;AACnD,2EAA2E;AAC3E,8EAA8E;AAE9E,qBAAe,aAAa,CAAC;AAE7B;;GAEG;AACH,SAAS,uBAAuB,CAC9B,GAAwB,EACxB,QAAgC;IAEhC,QAAQ,CAAC,cAAc,CAAC;QACtB,IAAI,EAAE,qBAAW;QACjB,OAAO,EAAE,wBAAc;QACvB,OAAO,EAAE,aAAa;KACvB,CAAC,CAAC;AACL,CAAC",
+    "file": "lib_plugin_js.7e633c522b2189389736.js",
+    "mappings": ";;;;;;;;;;AAAA,kCAAkC;AAClC,2DAA2D;;;;;;;;;;;;;;;;;;;;;AAM3D,yHAA+D;AAE/D,2FAA0C;AAE1C,2EAAwD;AAExD,MAAM,YAAY,GAAG,0BAA0B,CAAC;AAEhD;;GAEG;AACH,MAAM,MAAM,GAAuC;IACjD,EAAE,EAAE,YAAY;IAChB,QAAQ,EAAE,CAAC,6BAAsB,CAAC;IAClC,QAAQ,EAAE,uBAAuB;IACjC,SAAS,EAAE,IAAI;CACiC,CAAC;AACnD,2EAA2E;AAC3E,8EAA8E;AAE9E,qBAAe,MAAM,CAAC;AAEtB;;GAEG;AACH,SAAS,uBAAuB,CAC9B,GAAwB,EACxB,QAAgC;IAEhC,QAAQ,CAAC,cAAc,CAAC;QACtB,IAAI,EAAE,qBAAW;QACjB,OAAO,EAAE,wBAAc;QACvB,OAAO,EAAE,aAAa;KACvB,CAAC,CAAC;AACL,CAAC",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./src/plugin.ts"
     ],
     "sourcesContent": [
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport { Application, IPlugin } from '@lumino/application';\n\nimport { Widget } from '@lumino/widgets';\n\nimport { IJupyterWidgetRegistry } from '@jupyter-widgets/base';\n\nimport * as widgetExports from './widget';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n\nconst EXTENSION_ID = 'jupyter-locuszoom:plugin';\n\n/**\n * The widget plugin.\n */\nconst plugin: IPlugin<Application<Widget>, void> = {\n  id: EXTENSION_ID,\n  requires: [IJupyterWidgetRegistry],\n  activate: activateWidgetExtension,\n  autoStart: true,\n} as unknown as IPlugin<Application<Widget>, void>;\n// the \"as unknown as ...\" typecast above is solely to support JupyterLab 1\n// and 2 in the same codebase and should be removed when we migrate to Lumino.\n\nexport default plugin;\n\n/**\n * Activate the widget extension.\n */\nfunction activateWidgetExtension(\n  app: Application<Widget>,\n  registry: IJupyterWidgetRegistry\n): void {\n  registry.registerWidget({\n    name: MODULE_NAME,\n    version: MODULE_VERSION,\n    exports: widgetExports,\n  });\n}\n"
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.031ff8058d8d31610ff4.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff612b296119c6362583.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,88 @@
                 module.exports = exports;
 
 
                 /***/
             }),
 
         /***/
+        "./lib/utils.js":
+            /*!**********************!*\
+              !*** ./lib/utils.js ***!
+              \**********************/
+            /***/
+            (function(__unused_webpack_module, exports) {
+
+                "use strict";
+
+                var __awaiter = (this && this.__awaiter) || function(thisArg, _arguments, P, generator) {
+                    function adopt(value) {
+                        return value instanceof P ? value : new P(function(resolve) {
+                            resolve(value);
+                        });
+                    }
+                    return new(P || (P = Promise))(function(resolve, reject) {
+                        function fulfilled(value) {
+                            try {
+                                step(generator.next(value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function rejected(value) {
+                            try {
+                                step(generator["throw"](value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function step(result) {
+                            result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected);
+                        }
+                        step((generator = generator.apply(thisArg, _arguments || [])).next());
+                    });
+                };
+                Object.defineProperty(exports, "__esModule", ({
+                    value: true
+                }));
+                exports.untilReady = void 0;
+
+                function sleep(timeout) {
+                    return __awaiter(this, void 0, void 0, function*() {
+                        return new Promise((resolve) => {
+                            setTimeout(() => {
+                                resolve();
+                            }, timeout);
+                        });
+                    });
+                }
+
+                function untilReady(isReady, maxRetrials = 15, interval = 75, intervalModifier = (i) => i) {
+                    return (() => __awaiter(this, void 0, void 0, function*() {
+                        let i = 0;
+                        while (isReady() !== true) {
+                            i += 1;
+                            if (maxRetrials !== -1 && i > maxRetrials) {
+                                throw Error('Too many retrials');
+                            }
+                            interval = intervalModifier(interval);
+                            yield sleep(interval);
+                        }
+                        return isReady;
+                    }))();
+                }
+                exports.untilReady = untilReady;
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/version.js":
             /*!************************!*\
               !*** ./lib/version.js ***!
               \************************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
@@ -107,15 +181,15 @@
                     value: true
                 }));
                 exports.LocusZoomView = exports.LocusZoomModel = void 0;
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const coreutils_1 = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 const locuszoom_1 = __importDefault(__webpack_require__( /*! locuszoom */ "webpack/sharing/consume/default/locuszoom/locuszoom"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
-                //import { untilReady } from './utils';
+                const utils_1 = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 // Import the CSS
                 __webpack_require__( /*! locuszoom/dist/locuszoom.css */ "./node_modules/locuszoom/dist/locuszoom.css");
                 __webpack_require__( /*! ../css/widget.css */ "./css/widget.css");
                 class LocusZoomModel extends base_1.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: LocusZoomModel.model_name,
@@ -126,15 +200,21 @@
                             _view_module_version: LocusZoomModel.view_module_version,
                             build: 'GRCh38',
                             position: {
                                 chr: '1',
                                 start: 0,
                                 end: 5000000,
                             },
-                            _associations_view: {}
+                            _associations_view: {
+                                range: {
+                                    chr: '1',
+                                    start: 0,
+                                    end: 5000000,
+                                },
+                            }
                         });
                     }
                 }
                 exports.LocusZoomModel = LocusZoomModel;
                 LocusZoomModel.serializers = Object.assign({}, base_1.DOMWidgetModel.serializers);
                 LocusZoomModel.model_name = 'LocusZoomModel';
                 LocusZoomModel.model_module = version_1.MODULE_NAME;
@@ -147,32 +227,22 @@
                     constructor(config) {
                         super({});
                         this.model = config.model;
                     }
                     _performRequest(options) {
                         return __awaiter(this, void 0, void 0, function*() {
                             // TODO: find a way to fetch view properly
-                            /**
-                            console.log('performing request', options);
-                            await untilReady(() => {
-                              const position = this.model.get('position');
-                              return (
-                                position.chr === options.chr
-                                &&
-                                position.start === options.start
-                                &&
-                                position.end === options.end
-                                )
-                            })
-                            console.log('got it!');
-                            */
-                            return {
-                                data: this.model.get('_associations_view'),
-                                lastPage: 100
-                            };
+                            yield utils_1.untilReady(() => {
+                                const view = this.model.get('_associations_view');
+                                const position = view.range;
+                                return (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end);
+                            });
+                            return this.model.get('_associations_view');
                         });
                     }
                 }
                 // A custom adapter should be added to the registry before using it
                 locuszoom_1.default.Adapters.add('ModelAssociation', ModelAssociation);
                 class LocusZoomView extends base_1.DOMWidgetView {
                     constructor(options) {
@@ -187,80 +257,89 @@
                             case 'resize':
                                 console.log('resize message');
                                 window.requestAnimationFrame(() => this.plot.rescaleSVG());
                                 break;
                         }
                     }
                     processPhosphorMessage(msg) {
-                        this._processLuminoMessage(msg, super.processLuminoMessage);
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this._processLuminoMessage(msg, super.processPhosphorMessage);
                     }
                     processLuminoMessage(msg) {
                         this._processLuminoMessage(msg, super.processLuminoMessage);
                     }
                     render() {
-                        const apiBase = "https://portaldev.sph.umich.edu/api/v1/";
+                        const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
                         const build = this.model.get('build');
-                        var dataSources = new locuszoom_1.default.DataSources();
+                        const dataSources = new locuszoom_1.default.DataSources();
                         dataSources
-                            .add("assoc", ["ModelAssociation", {
+                            .add('assoc', ['ModelAssociation', {
                                 model: this.model
                             }])
-                            .add("ld", ["LDServer", {
-                                url: "https://portaldev.sph.umich.edu/ld/",
-                                source: '1000G',
-                                build,
-                                population: 'ALL'
-                            }])
-                            .add("gene", ["GeneLZ", {
-                                url: apiBase + "annotation/genes/",
+                            .add('ld', [
+                                'LDServer', {
+                                    url: 'https://portaldev.sph.umich.edu/ld/',
+                                    source: '1000G',
+                                    build,
+                                    population: 'ALL',
+                                },
+                            ])
+                            .add('gene', ['GeneLZ', {
+                                url: apiBase + 'annotation/genes/',
                                 build
                             }])
-                            .add("recomb", ["RecombLZ", {
-                                url: apiBase + "annotation/recomb/results/",
-                                build
-                            }])
-                            .add("constraint", ["GeneConstraintLZ", {
-                                url: "https://gnomad.broadinstitute.org/api/",
-                                build
-                            }]);
+                            .add('recomb', [
+                                'RecombLZ', {
+                                    url: apiBase + 'annotation/recomb/results/',
+                                    build
+                                },
+                            ])
+                            .add('constraint', [
+                                'GeneConstraintLZ', {
+                                    url: 'https://gnomad.broadinstitute.org/api/',
+                                    build
+                                },
+                            ]);
+                        // TODO:
+                        //.add("phewas", ["PheWASLZ", {url: "https://portaldev.sph.umich.edu/" + "api/v1/statistic/phewas/", build: [build]}])
                         const initialState = this.positionState;
                         console.log(initialState);
-                        const layout = locuszoom_1.default.Layouts.get("plot", "standard_association", {
-                            state: initialState
+                        const layout = locuszoom_1.default.Layouts.get('plot', 'standard_association', {
+                            state: initialState,
                         });
                         // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.
                         const attached = this.el.parentElement !== null;
                         if (!attached) {
                             document.body.appendChild(this.el);
                         }
-                        const plot = locuszoom_1.default.populate("#" + this.container.id, dataSources, layout);
+                        const plot = locuszoom_1.default.populate('#' + this.container.id, dataSources, layout);
                         if (!attached) {
                             document.body.removeChild(this.el);
                         }
                         this.plot = plot;
                         plot.on('state_changed', () => {
-                            console.log('state changed');
                             const position = this.model.get('position');
-                            if (plot.state.start == position.start &&
-                                plot.state.end == position.end &&
-                                plot.state.chr == position.chr) {
+                            if (plot.state.start === position.start &&
+                                plot.state.end === position.end &&
+                                plot.state.chr === position.chr) {
                                 return;
                             }
                             console.log('plot state changed, will set kernel state to', plot.state);
                             this.model.set('position', {
                                 start: plot.state.start,
                                 end: plot.state.end,
-                                chr: plot.state.chr
+                                chr: plot.state.chr,
                             });
                             this.model.save_changes();
                         });
                         const updateState = () => {
                             console.log('kernel state changed, will set state to ', this.positionState);
                             plot.applyState(Object.assign(Object.assign({}, this.positionState), {
-                                ldrefvar: ""
+                                ldrefvar: ''
                             }));
                         };
                         // listen to changes of state in kernel and update view accordingly
                         this.model.on('change:position', updateState);
                         this.displayed.then(() => {
                             this.plot.rescaleSVG();
                         });
@@ -320,8 +399,8 @@
                 module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.0","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.031ff8058d8d31610ff4.js.map
+//# sourceMappingURL=lib_widget_js.ff612b296119c6362583.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.031ff8058d8d31610ff4.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.e00d9776199cdb3b0918.js.map`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071428571428572%*

 * *Differences: {"'file'": "'lib_widget_js.e00d9776199cdb3b0918.js'",*

 * * "'mappings'": "';;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE; […]*

```diff
@@ -1,19 +1,21 @@
 {
-    "file": "lib_widget_js.031ff8058d8d31610ff4.js",
-    "mappings": ";;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;ACNA,kCAAkC;AAClC,2DAA2D;;;AAE3D,6DAA6D;AAC7D,aAAa;AACb,8DAA8D;AAC9D,MAAM,IAAI,GAAG,mBAAO,CAAC,uCAAiB,CAAC,CAAC;AAExC;;;;;GAKG;AACU,sBAAc,GAAG,IAAI,CAAC,OAAO,CAAC;AAE3C;;GAEG;AACU,mBAAW,GAAG,IAAI,CAAC,IAAI,CAAC;;;;;;;;;;;;;ACnBrC,kCAAkC;AAClC,2DAA2D;;;;;;;;;;;;;;;AAE3D,yHAI+B;AAC/B,sHAAyC;AAGzC,iIAAkC;AAElC,2EAAwD;AACxD,uCAAuC;AAEvC,iBAAiB;AACjB,uGAAsC;AACtC,iEAA2B;AAE3B,MAAa,cAAe,SAAQ,qBAAc;IAChD,QAAQ;QACN,uCACK,KAAK,CAAC,QAAQ,EAAE,KACnB,WAAW,EAAE,cAAc,CAAC,UAAU,EACtC,aAAa,EAAE,cAAc,CAAC,YAAY,EAC1C,qBAAqB,EAAE,cAAc,CAAC,oBAAoB,EAC1D,UAAU,EAAE,cAAc,CAAC,SAAS,EACpC,YAAY,EAAE,cAAc,CAAC,WAAW,EACxC,oBAAoB,EAAE,cAAc,CAAC,mBAAmB,EACxD,KAAK,EAAE,QAAQ,EACf,QAAQ,EAAE;gBACR,GAAG,EAAE,GAAG;gBACR,KAAK,EAAE,CAAC;gBACR,GAAG,EAAE,OAAO;aACb,EACD,kBAAkB,EAAE,EAAE,IACtB;IACJ,CAAC;;AAlBH,wCA+BC;AAXQ,0BAAW,qBACb,qBAAc,CAAC,WAAW,EAE7B;AAEK,yBAAU,GAAG,gBAAgB,CAAC;AAC9B,2BAAY,GAAG,qBAAW,CAAC;AAC3B,mCAAoB,GAAG,wBAAc,CAAC;AACtC,wBAAS,GAAG,eAAe,CAAC,CAAC,yBAAyB;AACtD,0BAAW,GAAG,qBAAW,CAAC,CAAC,yBAAyB;AACpD,kCAAmB,GAAG,wBAAc,CAAC;AAS9C,MAAM,aAAa,GAAG,mBAAS,CAAC,QAAQ,CAAC,GAAG,CAAC,eAAe,CAAC,CAAC;AAG9D,MAAM,gBAAiB,SAAQ,aAAa;IAE1C,YAAY,MAA+B;QACzC,KAAK,CAAC,EAAE,CAAC,CAAC;QACV,IAAI,CAAC,KAAK,GAAG,MAAM,CAAC,KAAK,CAAC;IAC5B,CAAC;IAEK,eAAe,CAAC,OAAwB;;YAC5C,0CAA0C;YAC1C;;;;;;;;;;;;;cAaE;YACF,OAAO;gBACL,IAAI,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,oBAAoB,CAAC;gBAC1C,QAAQ,EAAE,GAAG;aACd,CAAC;QACJ,CAAC;KAAA;CACF;AACD,mEAAmE;AACnE,mBAAS,CAAC,QAAQ,CAAC,GAAG,CAAC,kBAAkB,EAAE,gBAAgB,CAAC,CAAC;AAG7D,MAAa,aAAc,SAAQ,oBAAa;IAG9C,YAAY,OAAY;QACtB,KAAK,CAAC,OAAO,CAAC,CAAC;QACf,IAAI,CAAC,SAAS,GAAG,QAAQ,CAAC,aAAa,CAAC,KAAK,CAAC,CAAC;QAC/C,IAAI,CAAC,SAAS,CAAC,EAAE,GAAG,aAAa,GAAG,gBAAI,CAAC,KAAK,EAAE,CAAC;QACjD,IAAI,CAAC,EAAE,CAAC,WAAW,CAAC,IAAI,CAAC,SAAS,CAAC,CAAC;IACtC,CAAC;IACA,qBAAqB,CAAC,GAAY,EAAE,MAA8B;QAC9D,MAAM,CAAC,IAAI,CAAC,IAAI,EAAE,GAAG,CAAC,CAAC;QACvB,QAAQ,GAAG,CAAC,IAAI,EAAE;YAChB,KAAK,QAAQ;gBACX,OAAO,CAAC,GAAG,CAAC,gBAAgB,CAAC;gBAC7B,MAAM,CAAC,qBAAqB,CAAC,GAAG,EAAE,CAAC,IAAI,CAAC,IAAI,CAAC,UAAU,EAAE,CAAC,CAAC;gBAC3D,MAAM;SACT;IACN,CAAC;IACD,sBAAsB,CAAC,GAAY;QAChC,IAAI,CAAC,qBAAqB,CAAC,GAAG,EAAE,KAAK,CAAC,oBAAoB,CAAC,CAAC;IAChE,CAAC;IAED,oBAAoB,CAAC,GAAY;QAC7B,IAAI,CAAC,qBAAqB,CAAC,GAAG,EAAE,KAAK,CAAC,oBAAoB,CAAC,CAAC;IAChE,CAAC;IACA,MAAM;QACJ,MAAM,OAAO,GAAG,yCAAyC,CAAC;QAC1D,MAAM,KAAK,GAAG,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,OAAO,CAAC,CAAC;QAEtC,IAAI,WAAW,GAAG,IAAI,mBAAS,CAAC,WAAW,EAAE,CAAC;QAC9C,WAAW;aACR,GAAG,CAAC,OAAO,EAAE,CAAC,kBAAkB,EAAE,EAAE,KAAK,EAAE,IAAI,CAAC,KAAK,EAAE,CAAC,CAAC;aACzD,GAAG,CAAC,IAAI,EAAE,CAAC,UAAU,EAAE,EAAE,GAAG,EAAE,qCAAqC,EAAE,MAAM,EAAE,OAAO,EAAE,KAAK,EAAE,UAAU,EAAE,KAAK,EAAE,CAAC,CAAC;aAClH,GAAG,CAAC,MAAM,EAAE,CAAC,QAAQ,EAAE,EAAE,GAAG,EAAE,OAAO,GAAG,mBAAmB,EAAE,KAAK,EAAE,CAAC,CAAC;aACtE,GAAG,CAAC,QAAQ,EAAE,CAAC,UAAU,EAAE,EAAE,GAAG,EAAE,OAAO,GAAG,4BAA4B,EAAE,KAAK,EAAE,CAAC,CAAC;aACnF,GAAG,CAAC,YAAY,EAAE,CAAC,kBAAkB,EAAE,EAAE,GAAG,EAAE,wCAAwC,EAAE,KAAK,EAAE,CAAC,CAAC,CAGnG;QAED,MAAM,YAAY,GAAG,IAAI,CAAC,aAAa,CAAC;QACxC,OAAO,CAAC,GAAG,CAAC,YAAY,CAAC,CAAC;QAC1B,MAAM,MAAM,GAAG,mBAAS,CAAC,OAAO,CAAC,GAAG,CAAC,MAAM,EAAE,sBAAsB,EAAE,EAAC,KAAK,EAAE,YAAY,EAAC,CAAC,CAAC;QAE5F,8FAA8F;QAC9F,MAAM,QAAQ,GAAG,IAAI,CAAC,EAAE,CAAC,aAAa,KAAK,IAAI,CAAC;QAChD,IAAI,CAAC,QAAQ,EAAE;YACb,QAAQ,CAAC,IAAI,CAAC,WAAW,CAAC,IAAI,CAAC,EAAE,CAAC,CAAC;SACpC;QACD,MAAM,IAAI,GAAG,mBAAS,CAAC,QAAQ,CAAC,GAAG,GAAG,IAAI,CAAC,SAAS,CAAC,EAAE,EAAE,WAAW,EAAE,MAAM,CAAC,CAAC;QAC9E,IAAI,CAAC,QAAQ,EAAE;YACb,QAAQ,CAAC,IAAI,CAAC,WAAW,CAAC,IAAI,CAAC,EAAE,CAAC,CAAC;SACpC;QACD,IAAI,CAAC,IAAI,GAAG,IAAI,CAAC;QAEjB,IAAI,CAAC,EAAE,CAAC,eAAe,EAAE,GAAG,EAAE;YAC5B,OAAO,CAAC,GAAG,CAAC,eAAe,CAAC,CAAC;YAC7B,MAAM,QAAQ,GAAG,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,UAAU,CAAC,CAAC;YAC5C,IACE,IAAI,CAAC,KAAK,CAAC,KAAK,IAAI,QAAQ,CAAC,KAAK;;oBAElC,IAAI,CAAC,KAAK,CAAC,GAAG,IAAI,QAAQ,CAAC,GAAG;;oBAE9B,IAAI,CAAC,KAAK,CAAC,GAAG,IAAI,QAAQ,CAAC,GAAG,EAC9B;gBACA,OAAO;aACR;YACD,OAAO,CAAC,GAAG,CAAC,8CAA8C,EAAG,IAAI,CAAC,KAAK,CAAC;YACxE,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,UAAU,EAAE,EAAC,KAAK,EAAE,IAAI,CAAC,KAAK,CAAC,KAAK,EAAE,GAAG,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG,EAAE,GAAG,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG,EAAC,CAAC,CAAC;YAChG,IAAI,CAAC,KAAK,CAAC,YAAY,EAAE,CAAC;QAC5B,CAAC,CAAC,CAAC;QAEH,MAAM,WAAW,GAAG,GAAG,EAAE;YACvB,OAAO,CAAC,GAAG,CAAC,0CAA0C,EAAE,IAAI,CAAC,aAAa,CAAC,CAAC;YAC5E,IAAI,CAAC,UAAU,iCAAM,IAAI,CAAC,aAAa,KAAE,QAAQ,EAAE,EAAE,IAAG,CAAC;QAC3D,CAAC;QAED,mEAAmE;QACnE,IAAI,CAAC,KAAK,CAAC,EAAE,CAAC,iBAAiB,EAAE,WAAW,CAAC,CAAC;QAC9C,IAAI,CAAC,SAAS,CAAC,IAAI,CAAC,GAAG,EAAE;YACvB,IAAI,CAAC,IAAI,CAAC,UAAU,EAAE,CAAC;QACzB,CAAC,CAAC,CAAC;IACL,CAAC;IAED,IAAI,aAAa;QACf,OAAO,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,UAAU,CAAC,CAAC;IACpC,CAAC;CACF;AAvFD,sCAuFC;;;;;;;;;;;ACtLD,UAAU,mBAAO,CAAC,oJAAwE;AAC1F,0BAA0B,mBAAO,CAAC,qHAAuD;;AAEzF;;AAEA;AACA;AACA;;AAEA;;AAEA;AACA;;AAEA;;;;AAIA",
+    "file": "lib_widget_js.e00d9776199cdb3b0918.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./css/widget.css",
+        "webpack://jupyter-locuszoom/./src/utils.ts",
         "webpack://jupyter-locuszoom/./src/version.ts",
         "webpack://jupyter-locuszoom/./src/widget.ts",
         "webpack://jupyter-locuszoom/./css/widget.css?a195"
     ],
     "sourcesContent": [
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
+        "async function sleep(timeout: number): Promise<void> {\n  return new Promise<void>((resolve) => {\n    setTimeout(() => {\n      resolve();\n    }, timeout);\n  });\n}\n\nexport function untilReady(\n  isReady: CallableFunction,\n  maxRetrials = 15,\n  interval = 75,\n  intervalModifier = (i: number) => i\n): Promise<CallableFunction> {\n  return (async () => {\n    let i = 0;\n    while (isReady() !== true) {\n      i += 1;\n      if (maxRetrials !== -1 && i > maxRetrials) {\n        throw Error('Too many retrials');\n      }\n      interval = intervalModifier(interval);\n      await sleep(interval);\n    }\n    return isReady;\n  })();\n}\n",
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n//import { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {}\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: {model: LocusZoomModel}) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    /**\n    console.log('performing request', options);\n    await untilReady(() => {\n      const position = this.model.get('position');\n      return (\n        position.chr === options.chr\n        &&\n        position.start === options.start\n        &&\n        position.end === options.end\n        )\n    })\n    console.log('got it!');\n    */\n    return {\n      data: this.model.get('_associations_view'),\n      lastPage: 100\n    };\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n   _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n       _super.call(this, msg);\n       switch (msg.type) {\n         case 'resize':\n           console.log('resize message')\n           window.requestAnimationFrame(() => this.plot.rescaleSVG());\n           break;\n       }\n  }\n  processPhosphorMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n\n processLuminoMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n  render() {\n    const apiBase = \"https://portaldev.sph.umich.edu/api/v1/\";\n    const build = this.model.get('build');\n\n    var dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add(\"assoc\", [\"ModelAssociation\", { model: this.model }])\n      .add(\"ld\", [\"LDServer\", { url: \"https://portaldev.sph.umich.edu/ld/\", source: '1000G', build, population: 'ALL' }])\n      .add(\"gene\", [\"GeneLZ\", { url: apiBase + \"annotation/genes/\", build }])\n      .add(\"recomb\", [\"RecombLZ\", { url: apiBase + \"annotation/recomb/results/\", build }])\n      .add(\"constraint\", [\"GeneConstraintLZ\", { url: \"https://gnomad.broadinstitute.org/api/\", build }])\n      // TODO:\n      //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n    ;\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get(\"plot\", \"standard_association\", {state: initialState});\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\"#\" + this.container.id, dataSources, layout);\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      console.log('state changed');\n      const position = this.model.get('position');\n      if (\n        plot.state.start == position.start\n        &&\n        plot.state.end == position.end\n        &&\n        plot.state.chr == position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to',  plot.state)\n      this.model.set('position', {start: plot.state.start, end: plot.state.end, chr: plot.state.chr});\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log('kernel state changed, will set state to ', this.positionState);\n      plot.applyState({ ...this.positionState, ldrefvar: \"\" });\n    }\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
+        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {\n        range: {\n          chr: '1',\n          start: 0,\n          end: 5000000,\n        }\n      },\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: { model: LocusZoomModel }) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    await untilReady(() => {\n      const view = this.model.get('_associations_view');\n      const position = view.range;\n      return (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      );\n    });\n    return this.model.get('_associations_view');\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n  _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n    _super.call(this, msg);\n    switch (msg.type) {\n      case 'resize':\n        console.log('resize message');\n        window.requestAnimationFrame(() => this.plot.rescaleSVG());\n        break;\n    }\n  }\n  processPhosphorMessage(msg: Message): void {\n    // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n    // @ts-ignore\n    this._processLuminoMessage(msg, super.processPhosphorMessage);\n  }\n\n  processLuminoMessage(msg: Message): void {\n    this._processLuminoMessage(msg, super.processLuminoMessage);\n  }\n  render() {\n    const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';\n    const build = this.model.get('build');\n\n    const dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add('assoc', ['ModelAssociation', { model: this.model }])\n      .add('ld', [\n        'LDServer',\n        {\n          url: 'https://portaldev.sph.umich.edu/ld/',\n          source: '1000G',\n          build,\n          population: 'ALL',\n        },\n      ])\n      .add('gene', ['GeneLZ', { url: apiBase + 'annotation/genes/', build }])\n      .add('recomb', [\n        'RecombLZ',\n        { url: apiBase + 'annotation/recomb/results/', build },\n      ])\n      .add('constraint', [\n        'GeneConstraintLZ',\n        { url: 'https://gnomad.broadinstitute.org/api/', build },\n      ]);\n    // TODO:\n    //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get('plot', 'standard_association', {\n      state: initialState,\n    });\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\n      '#' + this.container.id,\n      dataSources,\n      layout\n    );\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      const position = this.model.get('position');\n      if (\n        plot.state.start === position.start &&\n        plot.state.end === position.end &&\n        plot.state.chr === position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to', plot.state);\n      this.model.set('position', {\n        start: plot.state.start,\n        end: plot.state.end,\n        chr: plot.state.chr,\n      });\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log(\n        'kernel state changed, will set state to ',\n        this.positionState\n      );\n      plot.applyState({ ...this.positionState, ldrefvar: '' });\n    };\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.0623db0f7d3c07125290.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.b631ee8a6ff24aede47c.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,88 @@
                 module.exports = exports;
 
 
                 /***/
             }),
 
         /***/
+        "./lib/utils.js":
+            /*!**********************!*\
+              !*** ./lib/utils.js ***!
+              \**********************/
+            /***/
+            (function(__unused_webpack_module, exports) {
+
+                "use strict";
+
+                var __awaiter = (this && this.__awaiter) || function(thisArg, _arguments, P, generator) {
+                    function adopt(value) {
+                        return value instanceof P ? value : new P(function(resolve) {
+                            resolve(value);
+                        });
+                    }
+                    return new(P || (P = Promise))(function(resolve, reject) {
+                        function fulfilled(value) {
+                            try {
+                                step(generator.next(value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function rejected(value) {
+                            try {
+                                step(generator["throw"](value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function step(result) {
+                            result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected);
+                        }
+                        step((generator = generator.apply(thisArg, _arguments || [])).next());
+                    });
+                };
+                Object.defineProperty(exports, "__esModule", ({
+                    value: true
+                }));
+                exports.untilReady = void 0;
+
+                function sleep(timeout) {
+                    return __awaiter(this, void 0, void 0, function*() {
+                        return new Promise((resolve) => {
+                            setTimeout(() => {
+                                resolve();
+                            }, timeout);
+                        });
+                    });
+                }
+
+                function untilReady(isReady, maxRetrials = 15, interval = 75, intervalModifier = (i) => i) {
+                    return (() => __awaiter(this, void 0, void 0, function*() {
+                        let i = 0;
+                        while (isReady() !== true) {
+                            i += 1;
+                            if (maxRetrials !== -1 && i > maxRetrials) {
+                                throw Error('Too many retrials');
+                            }
+                            interval = intervalModifier(interval);
+                            yield sleep(interval);
+                        }
+                        return isReady;
+                    }))();
+                }
+                exports.untilReady = untilReady;
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/version.js":
             /*!************************!*\
               !*** ./lib/version.js ***!
               \************************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
@@ -107,34 +181,40 @@
                     value: true
                 }));
                 exports.LocusZoomView = exports.LocusZoomModel = void 0;
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const coreutils_1 = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 const locuszoom_1 = __importDefault(__webpack_require__( /*! locuszoom */ "webpack/sharing/consume/default/locuszoom/locuszoom"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
-                //import { untilReady } from './utils';
+                const utils_1 = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 // Import the CSS
                 __webpack_require__( /*! locuszoom/dist/locuszoom.css */ "./node_modules/locuszoom/dist/locuszoom.css");
                 __webpack_require__( /*! ../css/widget.css */ "./css/widget.css");
                 class LocusZoomModel extends base_1.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: LocusZoomModel.model_name,
                             _model_module: LocusZoomModel.model_module,
                             _model_module_version: LocusZoomModel.model_module_version,
                             _view_name: LocusZoomModel.view_name,
                             _view_module: LocusZoomModel.view_module,
                             _view_module_version: LocusZoomModel.view_module_version,
                             build: 'GRCh38',
                             position: {
-                                chrom: '1',
+                                chr: '1',
                                 start: 0,
                                 end: 5000000,
                             },
-                            _associations_view: {}
+                            _associations_view: {
+                                range: {
+                                    chr: '1',
+                                    start: 0,
+                                    end: 5000000,
+                                },
+                            }
                         });
                     }
                 }
                 exports.LocusZoomModel = LocusZoomModel;
                 LocusZoomModel.serializers = Object.assign({}, base_1.DOMWidgetModel.serializers);
                 LocusZoomModel.model_name = 'LocusZoomModel';
                 LocusZoomModel.model_module = version_1.MODULE_NAME;
@@ -146,32 +226,23 @@
                 class ModelAssociation extends AssociationLZ {
                     constructor(config) {
                         super({});
                         this.model = config.model;
                     }
                     _performRequest(options) {
                         return __awaiter(this, void 0, void 0, function*() {
-                            /**
-                            console.log('performing request', options);
-                            await untilReady(() => {
-                              const position = this.model.get('position');
-                              return (
-                                position.chr === options.chr
-                                &&
-                                position.start === options.start
-                                &&
-                                position.end === options.end
-                                )
-                            })
-                            console.log('got it!');
-                            */
-                            return {
-                                data: this.model.get('_associations_view'),
-                                lastPage: 100
-                            };
+                            // TODO: find a way to fetch view properly
+                            yield utils_1.untilReady(() => {
+                                const view = this.model.get('_associations_view');
+                                const position = view.range;
+                                return (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end);
+                            });
+                            return this.model.get('_associations_view');
                         });
                     }
                 }
                 // A custom adapter should be added to the registry before using it
                 locuszoom_1.default.Adapters.add('ModelAssociation', ModelAssociation);
                 class LocusZoomView extends base_1.DOMWidgetView {
                     constructor(options) {
@@ -186,88 +257,96 @@
                             case 'resize':
                                 console.log('resize message');
                                 window.requestAnimationFrame(() => this.plot.rescaleSVG());
                                 break;
                         }
                     }
                     processPhosphorMessage(msg) {
-                        this._processLuminoMessage(msg, super.processLuminoMessage);
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this._processLuminoMessage(msg, super.processPhosphorMessage);
                     }
                     processLuminoMessage(msg) {
                         this._processLuminoMessage(msg, super.processLuminoMessage);
                     }
                     render() {
-                        const apiBase = "https://portaldev.sph.umich.edu/api/v1/";
+                        const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
                         const build = this.model.get('build');
-                        var dataSources = new locuszoom_1.default.DataSources();
+                        const dataSources = new locuszoom_1.default.DataSources();
                         dataSources
-                            .add("assoc", ["ModelAssociation", {
+                            .add('assoc', ['ModelAssociation', {
                                 model: this.model
                             }])
-                            .add("ld", ["LDServer", {
-                                url: "https://portaldev.sph.umich.edu/ld/",
-                                source: '1000G',
-                                build,
-                                population: 'ALL'
-                            }])
-                            .add("gene", ["GeneLZ", {
-                                url: apiBase + "annotation/genes/",
+                            .add('ld', [
+                                'LDServer', {
+                                    url: 'https://portaldev.sph.umich.edu/ld/',
+                                    source: '1000G',
+                                    build,
+                                    population: 'ALL',
+                                },
+                            ])
+                            .add('gene', ['GeneLZ', {
+                                url: apiBase + 'annotation/genes/',
                                 build
                             }])
-                            .add("recomb", ["RecombLZ", {
-                                url: apiBase + "annotation/recomb/results/",
-                                build
-                            }])
-                            .add("constraint", ["GeneConstraintLZ", {
-                                url: "https://gnomad.broadinstitute.org/api/",
-                                build
-                            }]);
+                            .add('recomb', [
+                                'RecombLZ', {
+                                    url: apiBase + 'annotation/recomb/results/',
+                                    build
+                                },
+                            ])
+                            .add('constraint', [
+                                'GeneConstraintLZ', {
+                                    url: 'https://gnomad.broadinstitute.org/api/',
+                                    build
+                                },
+                            ]);
+                        // TODO:
+                        //.add("phewas", ["PheWASLZ", {url: "https://portaldev.sph.umich.edu/" + "api/v1/statistic/phewas/", build: [build]}])
                         const initialState = this.positionState;
                         console.log(initialState);
-                        const layout = locuszoom_1.default.Layouts.get("plot", "standard_association", {
-                            state: initialState
+                        const layout = locuszoom_1.default.Layouts.get('plot', 'standard_association', {
+                            state: initialState,
                         });
                         // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.
                         const attached = this.el.parentElement !== null;
                         if (!attached) {
                             document.body.appendChild(this.el);
                         }
-                        const plot = locuszoom_1.default.populate("#" + this.container.id, dataSources, layout);
+                        const plot = locuszoom_1.default.populate('#' + this.container.id, dataSources, layout);
                         if (!attached) {
                             document.body.removeChild(this.el);
                         }
                         this.plot = plot;
                         plot.on('state_changed', () => {
-                            console.log('state changed');
                             const position = this.model.get('position');
-                            if (plot.state.start == position.start &&
-                                plot.state.end == position.end &&
-                                plot.state.chr == position.chr) {
+                            if (plot.state.start === position.start &&
+                                plot.state.end === position.end &&
+                                plot.state.chr === position.chr) {
                                 return;
                             }
                             console.log('plot state changed, will set kernel state to', plot.state);
                             this.model.set('position', {
                                 start: plot.state.start,
                                 end: plot.state.end,
-                                chr: plot.state.chr
+                                chr: plot.state.chr,
                             });
                             this.model.save_changes();
                         });
                         const updateState = () => {
                             console.log('kernel state changed, will set state to ', this.positionState);
                             plot.applyState(Object.assign(Object.assign({}, this.positionState), {
-                                ldrefvar: ""
+                                ldrefvar: ''
                             }));
                         };
                         // listen to changes of state in kernel and update view accordingly
                         this.model.on('change:position', updateState);
                         this.displayed.then(() => {
                             this.plot.rescaleSVG();
                         });
-                        //this.model.on('change:_associations_view', updateState);
                     }
                     get positionState() {
                         return this.model.get('position');
                     }
                 }
                 exports.LocusZoomView = LocusZoomView;
 
@@ -313,15 +392,15 @@
             /*!**********************!*\
               !*** ./package.json ***!
               \**********************/
             /***/
             ((module) => {
 
                 "use strict";
-                module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.0","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
+                module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.1","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.0623db0f7d3c07125290.js.map
+//# sourceMappingURL=lib_widget_js.b631ee8a6ff24aede47c.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.0623db0f7d3c07125290.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.b631ee8a6ff24aede47c.js.map`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071428571428572%*

 * *Differences: {"'file'": "'lib_widget_js.b631ee8a6ff24aede47c.js'",*

 * * "'mappings'": "';;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE; […]*

```diff
@@ -1,19 +1,21 @@
 {
-    "file": "lib_widget_js.0623db0f7d3c07125290.js",
-    "mappings": "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",
+    "file": "lib_widget_js.b631ee8a6ff24aede47c.js",
+    "mappings": ";;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE;QACjB,IAAI,CAAC,GAAG,CAAC,CAAC;QACV,OAAO,OAAO,EAAE,KAAK,IAAI,EAAE;YACzB,CAAC,IAAI,CAAC,CAAC;YACP,IAAI,WAAW,KAAK,CAAC,CAAC,IAAI,CAAC,GAAG,WAAW,EAAE;gBACzC,MAAM,KAAK,CAAC,mBAAmB,CAAC,CAAC;aAClC;YACD,QAAQ,GAAG,gBAAgB,CAAC,QAAQ,CAAC,CAAC;YACtC,MAAM,KAAK,CAAC,QAAQ,CAAC,CAAC;SACvB;QACD,OAAO,OAAO,CAAC;IACjB,CAAC,EAAC,EAAE,CAAC;AACP,CAAC;AAlBD,gCAkBC;;;;;;;;;;;;;AC1BD,kCAAkC;AAClC,2DAA2D;;;AAE3D,6DAA6D;AAC7D,aAAa;AACb,8DAA8D;AAC9D,MAAM,IAAI,GAAG,mBAAO,CAAC,uCAAiB,CAAC,CAAC;AAExC;;;;;GAKG;AACU,sBAAc,GAAG,IAAI,CAAC,OAAO,CAAC;AAE3C;;GAEG;AACU,mBAAW,GAAG,IAAI,CAAC,IAAI,CAAC;;;;;;;;;;;;;ACnBrC,kCAAkC;AAClC,2DAA2D;;;;;;;;;;;;;;;AAE3D,yHAI+B;AAC/B,sHAAyC;AAGzC,iIAAkC;AAElC,2EAAwD;AACxD,qEAAqC;AAErC,iBAAiB;AACjB,uGAAsC;AACtC,iEAA2B;AAE3B,MAAa,cAAe,SAAQ,qBAAc;IAChD,QAAQ;QACN,uCACK,KAAK,CAAC,QAAQ,EAAE,KACnB,WAAW,EAAE,cAAc,CAAC,UAAU,EACtC,aAAa,EAAE,cAAc,CAAC,YAAY,EAC1C,qBAAqB,EAAE,cAAc,CAAC,oBAAoB,EAC1D,UAAU,EAAE,cAAc,CAAC,SAAS,EACpC,YAAY,EAAE,cAAc,CAAC,WAAW,EACxC,oBAAoB,EAAE,cAAc,CAAC,mBAAmB,EACxD,KAAK,EAAE,QAAQ,EACf,QAAQ,EAAE;gBACR,GAAG,EAAE,GAAG;gBACR,KAAK,EAAE,CAAC;gBACR,GAAG,EAAE,OAAO;aACb,EACD,kBAAkB,EAAE;gBAClB,KAAK,EAAE;oBACL,GAAG,EAAE,GAAG;oBACR,KAAK,EAAE,CAAC;oBACR,GAAG,EAAE,OAAO;iBACb;aACF,IACD;IACJ,CAAC;;AAxBH,wCAqCC;AAXQ,0BAAW,qBACb,qBAAc,CAAC,WAAW,EAE7B;AAEK,yBAAU,GAAG,gBAAgB,CAAC;AAC9B,2BAAY,GAAG,qBAAW,CAAC;AAC3B,mCAAoB,GAAG,wBAAc,CAAC;AACtC,wBAAS,GAAG,eAAe,CAAC,CAAC,yBAAyB;AACtD,0BAAW,GAAG,qBAAW,CAAC,CAAC,yBAAyB;AACpD,kCAAmB,GAAG,wBAAc,CAAC;AAS9C,MAAM,aAAa,GAAG,mBAAS,CAAC,QAAQ,CAAC,GAAG,CAAC,eAAe,CAAC,CAAC;AAE9D,MAAM,gBAAiB,SAAQ,aAAa;IAE1C,YAAY,MAAiC;QAC3C,KAAK,CAAC,EAAE,CAAC,CAAC;QACV,IAAI,CAAC,KAAK,GAAG,MAAM,CAAC,KAAK,CAAC;IAC5B,CAAC;IAEK,eAAe,CAAC,OAAwB;;YAC5C,0CAA0C;YAC1C,MAAM,kBAAU,CAAC,GAAG,EAAE;gBACpB,MAAM,IAAI,GAAG,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,oBAAoB,CAAC,CAAC;gBAClD,MAAM,QAAQ,GAAG,IAAI,CAAC,KAAK,CAAC;gBAC5B,OAAO,CACL,QAAQ,CAAC,GAAG,KAAK,OAAO,CAAC,GAAG;oBAC5B,QAAQ,CAAC,KAAK,KAAK,OAAO,CAAC,KAAK;oBAChC,QAAQ,CAAC,GAAG,KAAK,OAAO,CAAC,GAAG,CAC7B,CAAC;YACJ,CAAC,CAAC,CAAC;YACH,OAAO,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,oBAAoB,CAAC,CAAC;QAC9C,CAAC;KAAA;CACF;AACD,mEAAmE;AACnE,mBAAS,CAAC,QAAQ,CAAC,GAAG,CAAC,kBAAkB,EAAE,gBAAgB,CAAC,CAAC;AAE7D,MAAa,aAAc,SAAQ,oBAAa;IAG9C,YAAY,OAAY;QACtB,KAAK,CAAC,OAAO,CAAC,CAAC;QACf,IAAI,CAAC,SAAS,GAAG,QAAQ,CAAC,aAAa,CAAC,KAAK,CAAC,CAAC;QAC/C,IAAI,CAAC,SAAS,CAAC,EAAE,GAAG,aAAa,GAAG,gBAAI,CAAC,KAAK,EAAE,CAAC;QACjD,IAAI,CAAC,EAAE,CAAC,WAAW,CAAC,IAAI,CAAC,SAAS,CAAC,CAAC;IACtC,CAAC;IACD,qBAAqB,CAAC,GAAY,EAAE,MAA8B;QAChE,MAAM,CAAC,IAAI,CAAC,IAAI,EAAE,GAAG,CAAC,CAAC;QACvB,QAAQ,GAAG,CAAC,IAAI,EAAE;YAChB,KAAK,QAAQ;gBACX,OAAO,CAAC,GAAG,CAAC,gBAAgB,CAAC,CAAC;gBAC9B,MAAM,CAAC,qBAAqB,CAAC,GAAG,EAAE,CAAC,IAAI,CAAC,IAAI,CAAC,UAAU,EAAE,CAAC,CAAC;gBAC3D,MAAM;SACT;IACH,CAAC;IACD,sBAAsB,CAAC,GAAY;QACjC,6DAA6D;QAC7D,aAAa;QACb,IAAI,CAAC,qBAAqB,CAAC,GAAG,EAAE,KAAK,CAAC,sBAAsB,CAAC,CAAC;IAChE,CAAC;IAED,oBAAoB,CAAC,GAAY;QAC/B,IAAI,CAAC,qBAAqB,CAAC,GAAG,EAAE,KAAK,CAAC,oBAAoB,CAAC,CAAC;IAC9D,CAAC;IACD,MAAM;QACJ,MAAM,OAAO,GAAG,yCAAyC,CAAC;QAC1D,MAAM,KAAK,GAAG,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,OAAO,CAAC,CAAC;QAEtC,MAAM,WAAW,GAAG,IAAI,mBAAS,CAAC,WAAW,EAAE,CAAC;QAChD,WAAW;aACR,GAAG,CAAC,OAAO,EAAE,CAAC,kBAAkB,EAAE,EAAE,KAAK,EAAE,IAAI,CAAC,KAAK,EAAE,CAAC,CAAC;aACzD,GAAG,CAAC,IAAI,EAAE;YACT,UAAU;YACV;gBACE,GAAG,EAAE,qCAAqC;gBAC1C,MAAM,EAAE,OAAO;gBACf,KAAK;gBACL,UAAU,EAAE,KAAK;aAClB;SACF,CAAC;aACD,GAAG,CAAC,MAAM,EAAE,CAAC,QAAQ,EAAE,EAAE,GAAG,EAAE,OAAO,GAAG,mBAAmB,EAAE,KAAK,EAAE,CAAC,CAAC;aACtE,GAAG,CAAC,QAAQ,EAAE;YACb,UAAU;YACV,EAAE,GAAG,EAAE,OAAO,GAAG,4BAA4B,EAAE,KAAK,EAAE;SACvD,CAAC;aACD,GAAG,CAAC,YAAY,EAAE;YACjB,kBAAkB;YAClB,EAAE,GAAG,EAAE,wCAAwC,EAAE,KAAK,EAAE;SACzD,CAAC,CAAC;QACL,QAAQ;QACR,sHAAsH;QAEtH,MAAM,YAAY,GAAG,IAAI,CAAC,aAAa,CAAC;QACxC,OAAO,CAAC,GAAG,CAAC,YAAY,CAAC,CAAC;QAC1B,MAAM,MAAM,GAAG,mBAAS,CAAC,OAAO,CAAC,GAAG,CAAC,MAAM,EAAE,sBAAsB,EAAE;YACnE,KAAK,EAAE,YAAY;SACpB,CAAC,CAAC;QAEH,8FAA8F;QAC9F,MAAM,QAAQ,GAAG,IAAI,CAAC,EAAE,CAAC,aAAa,KAAK,IAAI,CAAC;QAChD,IAAI,CAAC,QAAQ,EAAE;YACb,QAAQ,CAAC,IAAI,CAAC,WAAW,CAAC,IAAI,CAAC,EAAE,CAAC,CAAC;SACpC;QACD,MAAM,IAAI,GAAG,mBAAS,CAAC,QAAQ,CAC7B,GAAG,GAAG,IAAI,CAAC,SAAS,CAAC,EAAE,EACvB,WAAW,EACX,MAAM,CACP,CAAC;QACF,IAAI,CAAC,QAAQ,EAAE;YACb,QAAQ,CAAC,IAAI,CAAC,WAAW,CAAC,IAAI,CAAC,EAAE,CAAC,CAAC;SACpC;QACD,IAAI,CAAC,IAAI,GAAG,IAAI,CAAC;QAEjB,IAAI,CAAC,EAAE,CAAC,eAAe,EAAE,GAAG,EAAE;YAC5B,MAAM,QAAQ,GAAG,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,UAAU,CAAC,CAAC;YAC5C,IACE,IAAI,CAAC,KAAK,CAAC,KAAK,KAAK,QAAQ,CAAC,KAAK;gBACnC,IAAI,CAAC,KAAK,CAAC,GAAG,KAAK,QAAQ,CAAC,GAAG;gBAC/B,IAAI,CAAC,KAAK,CAAC,GAAG,KAAK,QAAQ,CAAC,GAAG,EAC/B;gBACA,OAAO;aACR;YACD,OAAO,CAAC,GAAG,CAAC,8CAA8C,EAAE,IAAI,CAAC,KAAK,CAAC,CAAC;YACxE,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,UAAU,EAAE;gBACzB,KAAK,EAAE,IAAI,CAAC,KAAK,CAAC,KAAK;gBACvB,GAAG,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG;gBACnB,GAAG,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG;aACpB,CAAC,CAAC;YACH,IAAI,CAAC,KAAK,CAAC,YAAY,EAAE,CAAC;QAC5B,CAAC,CAAC,CAAC;QAEH,MAAM,WAAW,GAAG,GAAG,EAAE;YACvB,OAAO,CAAC,GAAG,CACT,0CAA0C,EAC1C,IAAI,CAAC,aAAa,CACnB,CAAC;YACF,IAAI,CAAC,UAAU,iCAAM,IAAI,CAAC,aAAa,KAAE,QAAQ,EAAE,EAAE,IAAG,CAAC;QAC3D,CAAC,CAAC;QAEF,mEAAmE;QACnE,IAAI,CAAC,KAAK,CAAC,EAAE,CAAC,iBAAiB,EAAE,WAAW,CAAC,CAAC;QAC9C,IAAI,CAAC,SAAS,CAAC,IAAI,CAAC,GAAG,EAAE;YACvB,IAAI,CAAC,IAAI,CAAC,UAAU,EAAE,CAAC;QACzB,CAAC,CAAC,CAAC;IACL,CAAC;IAED,IAAI,aAAa;QACf,OAAO,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,UAAU,CAAC,CAAC;IACpC,CAAC;CACF;AAhHD,sCAgHC;;;;;;;;;;;AC3MD,UAAU,mBAAO,CAAC,oJAAwE;AAC1F,0BAA0B,mBAAO,CAAC,qHAAuD;;AAEzF;;AAEA;AACA;AACA;;AAEA;;AAEA;AACA;;AAEA;;;;AAIA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./css/widget.css",
+        "webpack://jupyter-locuszoom/./src/utils.ts",
         "webpack://jupyter-locuszoom/./src/version.ts",
         "webpack://jupyter-locuszoom/./src/widget.ts",
         "webpack://jupyter-locuszoom/./css/widget.css?a195"
     ],
     "sourcesContent": [
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
+        "async function sleep(timeout: number): Promise<void> {\n  return new Promise<void>((resolve) => {\n    setTimeout(() => {\n      resolve();\n    }, timeout);\n  });\n}\n\nexport function untilReady(\n  isReady: CallableFunction,\n  maxRetrials = 15,\n  interval = 75,\n  intervalModifier = (i: number) => i\n): Promise<CallableFunction> {\n  return (async () => {\n    let i = 0;\n    while (isReady() !== true) {\n      i += 1;\n      if (maxRetrials !== -1 && i > maxRetrials) {\n        throw Error('Too many retrials');\n      }\n      interval = intervalModifier(interval);\n      await sleep(interval);\n    }\n    return isReady;\n  })();\n}\n",
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n//import { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chrom: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {}\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: {model: LocusZoomModel}) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    /**\n    console.log('performing request', options);\n    await untilReady(() => {\n      const position = this.model.get('position');\n      return (\n        position.chr === options.chr\n        &&\n        position.start === options.start\n        &&\n        position.end === options.end\n        )\n    })\n    console.log('got it!');\n    */\n    return{\n      data: this.model.get('_associations_view'),\n      lastPage: 100\n    };\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n   _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n       _super.call(this, msg);\n       switch (msg.type) {\n         case 'resize':\n           console.log('resize message')\n           window.requestAnimationFrame(() => this.plot.rescaleSVG());\n           break;\n       }\n  }\n  processPhosphorMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n\n processLuminoMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n  render() {\n    const apiBase = \"https://portaldev.sph.umich.edu/api/v1/\";\n    const build = this.model.get('build');\n\n    var dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add(\"assoc\", [\"ModelAssociation\", { model: this.model }])\n      .add(\"ld\", [\"LDServer\", { url: \"https://portaldev.sph.umich.edu/ld/\", source: '1000G', build, population: 'ALL' }])\n      .add(\"gene\", [\"GeneLZ\", { url: apiBase + \"annotation/genes/\", build }])\n      .add(\"recomb\", [\"RecombLZ\", { url: apiBase + \"annotation/recomb/results/\", build }])\n      .add(\"constraint\", [\"GeneConstraintLZ\", { url: \"https://gnomad.broadinstitute.org/api/\", build }]);\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get(\"plot\", \"standard_association\", {state: initialState});\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\"#\" + this.container.id, dataSources, layout);\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      console.log('state changed');\n      const position = this.model.get('position');\n      if (\n        plot.state.start == position.start\n        &&\n        plot.state.end == position.end\n        &&\n        plot.state.chr == position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to',  plot.state)\n      this.model.set('position', {start: plot.state.start, end: plot.state.end, chr: plot.state.chr});\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log('kernel state changed, will set state to ', this.positionState);\n      plot.applyState({ ...this.positionState, ldrefvar: \"\" });\n    }\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n    //this.model.on('change:_associations_view', updateState);\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
+        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {\n        range: {\n          chr: '1',\n          start: 0,\n          end: 5000000,\n        },\n      },\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: { model: LocusZoomModel }) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    await untilReady(() => {\n      const view = this.model.get('_associations_view');\n      const position = view.range;\n      return (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      );\n    });\n    return this.model.get('_associations_view');\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n  _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n    _super.call(this, msg);\n    switch (msg.type) {\n      case 'resize':\n        console.log('resize message');\n        window.requestAnimationFrame(() => this.plot.rescaleSVG());\n        break;\n    }\n  }\n  processPhosphorMessage(msg: Message): void {\n    // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n    // @ts-ignore\n    this._processLuminoMessage(msg, super.processPhosphorMessage);\n  }\n\n  processLuminoMessage(msg: Message): void {\n    this._processLuminoMessage(msg, super.processLuminoMessage);\n  }\n  render() {\n    const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';\n    const build = this.model.get('build');\n\n    const dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add('assoc', ['ModelAssociation', { model: this.model }])\n      .add('ld', [\n        'LDServer',\n        {\n          url: 'https://portaldev.sph.umich.edu/ld/',\n          source: '1000G',\n          build,\n          population: 'ALL',\n        },\n      ])\n      .add('gene', ['GeneLZ', { url: apiBase + 'annotation/genes/', build }])\n      .add('recomb', [\n        'RecombLZ',\n        { url: apiBase + 'annotation/recomb/results/', build },\n      ])\n      .add('constraint', [\n        'GeneConstraintLZ',\n        { url: 'https://gnomad.broadinstitute.org/api/', build },\n      ]);\n    // TODO:\n    //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get('plot', 'standard_association', {\n      state: initialState,\n    });\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\n      '#' + this.container.id,\n      dataSources,\n      layout\n    );\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      const position = this.model.get('position');\n      if (\n        plot.state.start === position.start &&\n        plot.state.end === position.end &&\n        plot.state.chr === position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to', plot.state);\n      this.model.set('position', {\n        start: plot.state.start,\n        end: plot.state.end,\n        chr: plot.state.chr,\n      });\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log(\n        'kernel state changed, will set state to ',\n        this.positionState\n      );\n      plot.applyState({ ...this.positionState, ldrefvar: '' });\n    };\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.19c75a6eec62583a7167.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.e00d9776199cdb3b0918.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,88 @@
                 module.exports = exports;
 
 
                 /***/
             }),
 
         /***/
+        "./lib/utils.js":
+            /*!**********************!*\
+              !*** ./lib/utils.js ***!
+              \**********************/
+            /***/
+            (function(__unused_webpack_module, exports) {
+
+                "use strict";
+
+                var __awaiter = (this && this.__awaiter) || function(thisArg, _arguments, P, generator) {
+                    function adopt(value) {
+                        return value instanceof P ? value : new P(function(resolve) {
+                            resolve(value);
+                        });
+                    }
+                    return new(P || (P = Promise))(function(resolve, reject) {
+                        function fulfilled(value) {
+                            try {
+                                step(generator.next(value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function rejected(value) {
+                            try {
+                                step(generator["throw"](value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function step(result) {
+                            result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected);
+                        }
+                        step((generator = generator.apply(thisArg, _arguments || [])).next());
+                    });
+                };
+                Object.defineProperty(exports, "__esModule", ({
+                    value: true
+                }));
+                exports.untilReady = void 0;
+
+                function sleep(timeout) {
+                    return __awaiter(this, void 0, void 0, function*() {
+                        return new Promise((resolve) => {
+                            setTimeout(() => {
+                                resolve();
+                            }, timeout);
+                        });
+                    });
+                }
+
+                function untilReady(isReady, maxRetrials = 15, interval = 75, intervalModifier = (i) => i) {
+                    return (() => __awaiter(this, void 0, void 0, function*() {
+                        let i = 0;
+                        while (isReady() !== true) {
+                            i += 1;
+                            if (maxRetrials !== -1 && i > maxRetrials) {
+                                throw Error('Too many retrials');
+                            }
+                            interval = intervalModifier(interval);
+                            yield sleep(interval);
+                        }
+                        return isReady;
+                    }))();
+                }
+                exports.untilReady = untilReady;
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/version.js":
             /*!************************!*\
               !*** ./lib/version.js ***!
               \************************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
@@ -107,34 +181,40 @@
                     value: true
                 }));
                 exports.LocusZoomView = exports.LocusZoomModel = void 0;
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const coreutils_1 = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 const locuszoom_1 = __importDefault(__webpack_require__( /*! locuszoom */ "webpack/sharing/consume/default/locuszoom/locuszoom"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
-                //import { untilReady } from './utils';
+                const utils_1 = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 // Import the CSS
                 __webpack_require__( /*! locuszoom/dist/locuszoom.css */ "./node_modules/locuszoom/dist/locuszoom.css");
                 __webpack_require__( /*! ../css/widget.css */ "./css/widget.css");
                 class LocusZoomModel extends base_1.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: LocusZoomModel.model_name,
                             _model_module: LocusZoomModel.model_module,
                             _model_module_version: LocusZoomModel.model_module_version,
                             _view_name: LocusZoomModel.view_name,
                             _view_module: LocusZoomModel.view_module,
                             _view_module_version: LocusZoomModel.view_module_version,
                             build: 'GRCh38',
                             position: {
-                                chrom: '1',
+                                chr: '1',
                                 start: 0,
                                 end: 5000000,
                             },
-                            _associations_view: {}
+                            _associations_view: {
+                                range: {
+                                    chr: '1',
+                                    start: 0,
+                                    end: 5000000,
+                                }
+                            }
                         });
                     }
                 }
                 exports.LocusZoomModel = LocusZoomModel;
                 LocusZoomModel.serializers = Object.assign({}, base_1.DOMWidgetModel.serializers);
                 LocusZoomModel.model_name = 'LocusZoomModel';
                 LocusZoomModel.model_module = version_1.MODULE_NAME;
@@ -146,32 +226,23 @@
                 class ModelAssociation extends AssociationLZ {
                     constructor(config) {
                         super({});
                         this.model = config.model;
                     }
                     _performRequest(options) {
                         return __awaiter(this, void 0, void 0, function*() {
-                            /**
-                            console.log('performing request', options);
-                            await untilReady(() => {
-                              const position = this.model.get('position');
-                              return (
-                                position.chr === options.chr
-                                &&
-                                position.start === options.start
-                                &&
-                                position.end === options.end
-                                )
-                            })
-                            console.log('got it!');
-                            */
-                            return {
-                                data: this.model.get('_associations_view'),
-                                lastPage: 100
-                            };
+                            // TODO: find a way to fetch view properly
+                            yield utils_1.untilReady(() => {
+                                const view = this.model.get('_associations_view');
+                                const position = view.range;
+                                return (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end);
+                            });
+                            return this.model.get('_associations_view');
                         });
                     }
                 }
                 // A custom adapter should be added to the registry before using it
                 locuszoom_1.default.Adapters.add('ModelAssociation', ModelAssociation);
                 class LocusZoomView extends base_1.DOMWidgetView {
                     constructor(options) {
@@ -186,88 +257,96 @@
                             case 'resize':
                                 console.log('resize message');
                                 window.requestAnimationFrame(() => this.plot.rescaleSVG());
                                 break;
                         }
                     }
                     processPhosphorMessage(msg) {
-                        this._processLuminoMessage(msg, super.processLuminoMessage);
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this._processLuminoMessage(msg, super.processPhosphorMessage);
                     }
                     processLuminoMessage(msg) {
                         this._processLuminoMessage(msg, super.processLuminoMessage);
                     }
                     render() {
-                        const apiBase = "https://portaldev.sph.umich.edu/api/v1/";
+                        const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
                         const build = this.model.get('build');
-                        var dataSources = new locuszoom_1.default.DataSources();
+                        const dataSources = new locuszoom_1.default.DataSources();
                         dataSources
-                            .add("assoc", ["ModelAssociation", {
+                            .add('assoc', ['ModelAssociation', {
                                 model: this.model
                             }])
-                            .add("ld", ["LDServer", {
-                                url: "https://portaldev.sph.umich.edu/ld/",
-                                source: '1000G',
-                                build,
-                                population: 'ALL'
-                            }])
-                            .add("gene", ["GeneLZ", {
-                                url: apiBase + "annotation/genes/",
+                            .add('ld', [
+                                'LDServer', {
+                                    url: 'https://portaldev.sph.umich.edu/ld/',
+                                    source: '1000G',
+                                    build,
+                                    population: 'ALL',
+                                },
+                            ])
+                            .add('gene', ['GeneLZ', {
+                                url: apiBase + 'annotation/genes/',
                                 build
                             }])
-                            .add("recomb", ["RecombLZ", {
-                                url: apiBase + "annotation/recomb/results/",
-                                build
-                            }])
-                            .add("constraint", ["GeneConstraintLZ", {
-                                url: "https://gnomad.broadinstitute.org/api/",
-                                build
-                            }]);
+                            .add('recomb', [
+                                'RecombLZ', {
+                                    url: apiBase + 'annotation/recomb/results/',
+                                    build
+                                },
+                            ])
+                            .add('constraint', [
+                                'GeneConstraintLZ', {
+                                    url: 'https://gnomad.broadinstitute.org/api/',
+                                    build
+                                },
+                            ]);
+                        // TODO:
+                        //.add("phewas", ["PheWASLZ", {url: "https://portaldev.sph.umich.edu/" + "api/v1/statistic/phewas/", build: [build]}])
                         const initialState = this.positionState;
                         console.log(initialState);
-                        const layout = locuszoom_1.default.Layouts.get("plot", "standard_association", {
-                            state: initialState
+                        const layout = locuszoom_1.default.Layouts.get('plot', 'standard_association', {
+                            state: initialState,
                         });
                         // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.
                         const attached = this.el.parentElement !== null;
                         if (!attached) {
                             document.body.appendChild(this.el);
                         }
-                        const plot = locuszoom_1.default.populate("#" + this.container.id, dataSources, layout);
+                        const plot = locuszoom_1.default.populate('#' + this.container.id, dataSources, layout);
                         if (!attached) {
                             document.body.removeChild(this.el);
                         }
                         this.plot = plot;
                         plot.on('state_changed', () => {
-                            console.log('state changed');
                             const position = this.model.get('position');
-                            if (plot.state.start == position.start &&
-                                plot.state.end == position.end &&
-                                plot.state.chr == position.chrom) {
+                            if (plot.state.start === position.start &&
+                                plot.state.end === position.end &&
+                                plot.state.chr === position.chr) {
                                 return;
                             }
                             console.log('plot state changed, will set kernel state to', plot.state);
                             this.model.set('position', {
                                 start: plot.state.start,
                                 end: plot.state.end,
-                                chr: plot.state.chr
+                                chr: plot.state.chr,
                             });
                             this.model.save_changes();
                         });
                         const updateState = () => {
                             console.log('kernel state changed, will set state to ', this.positionState);
                             plot.applyState(Object.assign(Object.assign({}, this.positionState), {
-                                ldrefvar: ""
+                                ldrefvar: ''
                             }));
                         };
                         // listen to changes of state in kernel and update view accordingly
                         this.model.on('change:position', updateState);
                         this.displayed.then(() => {
                             this.plot.rescaleSVG();
                         });
-                        //this.model.on('change:_associations_view', updateState);
                     }
                     get positionState() {
                         return this.model.get('position');
                     }
                 }
                 exports.LocusZoomView = LocusZoomView;
 
@@ -320,8 +399,8 @@
                 module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.0","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.19c75a6eec62583a7167.js.map
+//# sourceMappingURL=lib_widget_js.e00d9776199cdb3b0918.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.19c75a6eec62583a7167.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff612b296119c6362583.js.map`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071428571428572%*

 * *Differences: {"'file'": "'lib_widget_js.ff612b296119c6362583.js'",*

 * * "'mappings'": "';;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE; […]*

```diff
@@ -1,19 +1,21 @@
 {
-    "file": "lib_widget_js.19c75a6eec62583a7167.js",
-    "mappings": "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",
+    "file": "lib_widget_js.ff612b296119c6362583.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./css/widget.css",
+        "webpack://jupyter-locuszoom/./src/utils.ts",
         "webpack://jupyter-locuszoom/./src/version.ts",
         "webpack://jupyter-locuszoom/./src/widget.ts",
         "webpack://jupyter-locuszoom/./css/widget.css?a195"
     ],
     "sourcesContent": [
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
+        "async function sleep(timeout: number): Promise<void> {\n  return new Promise<void>((resolve) => {\n    setTimeout(() => {\n      resolve();\n    }, timeout);\n  });\n}\n\nexport function untilReady(\n  isReady: CallableFunction,\n  maxRetrials = 15,\n  interval = 75,\n  intervalModifier = (i: number) => i\n): Promise<CallableFunction> {\n  return (async () => {\n    let i = 0;\n    while (isReady() !== true) {\n      i += 1;\n      if (maxRetrials !== -1 && i > maxRetrials) {\n        throw Error('Too many retrials');\n      }\n      interval = intervalModifier(interval);\n      await sleep(interval);\n    }\n    return isReady;\n  })();\n}\n",
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n//import { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chrom: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {}\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: {model: LocusZoomModel}) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    /**\n    console.log('performing request', options);\n    await untilReady(() => {\n      const position = this.model.get('position');\n      return (\n        position.chr === options.chr\n        &&\n        position.start === options.start\n        &&\n        position.end === options.end\n        )\n    })\n    console.log('got it!');\n    */\n    return{\n      data: this.model.get('_associations_view'),\n      lastPage: 100\n    };\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n   _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n       _super.call(this, msg);\n       switch (msg.type) {\n         case 'resize':\n           console.log('resize message')\n           window.requestAnimationFrame(() => this.plot.rescaleSVG());\n           break;\n       }\n  }\n  processPhosphorMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n\n processLuminoMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n  render() {\n    const apiBase = \"https://portaldev.sph.umich.edu/api/v1/\";\n    const build = this.model.get('build');\n\n    var dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add(\"assoc\", [\"ModelAssociation\", { model: this.model }])\n      .add(\"ld\", [\"LDServer\", { url: \"https://portaldev.sph.umich.edu/ld/\", source: '1000G', build, population: 'ALL' }])\n      .add(\"gene\", [\"GeneLZ\", { url: apiBase + \"annotation/genes/\", build }])\n      .add(\"recomb\", [\"RecombLZ\", { url: apiBase + \"annotation/recomb/results/\", build }])\n      .add(\"constraint\", [\"GeneConstraintLZ\", { url: \"https://gnomad.broadinstitute.org/api/\", build }]);\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get(\"plot\", \"standard_association\", {state: initialState});\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\"#\" + this.container.id, dataSources, layout);\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      console.log('state changed');\n      const position = this.model.get('position');\n      if (\n        plot.state.start == position.start\n        &&\n        plot.state.end == position.end\n        &&\n        plot.state.chr == position.chrom\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to',  plot.state)\n      this.model.set('position', {start: plot.state.start, end: plot.state.end, chr: plot.state.chr});\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log('kernel state changed, will set state to ', this.positionState);\n      plot.applyState({ ...this.positionState, ldrefvar: \"\" });\n    }\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n    //this.model.on('change:_associations_view', updateState);\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
+        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {\n        range: {\n          chr: '1',\n          start: 0,\n          end: 5000000,\n        },\n      },\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: { model: LocusZoomModel }) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    await untilReady(() => {\n      const view = this.model.get('_associations_view');\n      const position = view.range;\n      return (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      );\n    });\n    return this.model.get('_associations_view');\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n  _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n    _super.call(this, msg);\n    switch (msg.type) {\n      case 'resize':\n        console.log('resize message');\n        window.requestAnimationFrame(() => this.plot.rescaleSVG());\n        break;\n    }\n  }\n  processPhosphorMessage(msg: Message): void {\n    // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n    // @ts-ignore\n    this._processLuminoMessage(msg, super.processPhosphorMessage);\n  }\n\n  processLuminoMessage(msg: Message): void {\n    this._processLuminoMessage(msg, super.processLuminoMessage);\n  }\n  render() {\n    const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';\n    const build = this.model.get('build');\n\n    const dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add('assoc', ['ModelAssociation', { model: this.model }])\n      .add('ld', [\n        'LDServer',\n        {\n          url: 'https://portaldev.sph.umich.edu/ld/',\n          source: '1000G',\n          build,\n          population: 'ALL',\n        },\n      ])\n      .add('gene', ['GeneLZ', { url: apiBase + 'annotation/genes/', build }])\n      .add('recomb', [\n        'RecombLZ',\n        { url: apiBase + 'annotation/recomb/results/', build },\n      ])\n      .add('constraint', [\n        'GeneConstraintLZ',\n        { url: 'https://gnomad.broadinstitute.org/api/', build },\n      ]);\n    // TODO:\n    //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get('plot', 'standard_association', {\n      state: initialState,\n    });\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\n      '#' + this.container.id,\n      dataSources,\n      layout\n    );\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      const position = this.model.get('position');\n      if (\n        plot.state.start === position.start &&\n        plot.state.end === position.end &&\n        plot.state.chr === position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to', plot.state);\n      this.model.set('position', {\n        start: plot.state.start,\n        end: plot.state.end,\n        chr: plot.state.chr,\n      });\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log(\n        'kernel state changed, will set state to ',\n        this.positionState\n      );\n      plot.applyState({ ...this.positionState, ldrefvar: '' });\n    };\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.1de32fa6eec660baca88.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.751b11392fdca570e288.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,88 @@
                 module.exports = exports;
 
 
                 /***/
             }),
 
         /***/
+        "./lib/utils.js":
+            /*!**********************!*\
+              !*** ./lib/utils.js ***!
+              \**********************/
+            /***/
+            (function(__unused_webpack_module, exports) {
+
+                "use strict";
+
+                var __awaiter = (this && this.__awaiter) || function(thisArg, _arguments, P, generator) {
+                    function adopt(value) {
+                        return value instanceof P ? value : new P(function(resolve) {
+                            resolve(value);
+                        });
+                    }
+                    return new(P || (P = Promise))(function(resolve, reject) {
+                        function fulfilled(value) {
+                            try {
+                                step(generator.next(value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function rejected(value) {
+                            try {
+                                step(generator["throw"](value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function step(result) {
+                            result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected);
+                        }
+                        step((generator = generator.apply(thisArg, _arguments || [])).next());
+                    });
+                };
+                Object.defineProperty(exports, "__esModule", ({
+                    value: true
+                }));
+                exports.untilReady = void 0;
+
+                function sleep(timeout) {
+                    return __awaiter(this, void 0, void 0, function*() {
+                        return new Promise((resolve) => {
+                            setTimeout(() => {
+                                resolve();
+                            }, timeout);
+                        });
+                    });
+                }
+
+                function untilReady(isReady, maxRetrials = 10, interval = 75, intervalModifier = (i) => i) {
+                    return (() => __awaiter(this, void 0, void 0, function*() {
+                        let i = 0;
+                        while (isReady() !== true) {
+                            i += 1;
+                            if (maxRetrials !== -1 && i > maxRetrials) {
+                                throw Error('Too many retrials');
+                            }
+                            interval = intervalModifier(interval);
+                            yield sleep(interval);
+                        }
+                        return isReady;
+                    }))();
+                }
+                exports.untilReady = untilReady;
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/version.js":
             /*!************************!*\
               !*** ./lib/version.js ***!
               \************************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
@@ -107,15 +181,15 @@
                     value: true
                 }));
                 exports.LocusZoomView = exports.LocusZoomModel = void 0;
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const coreutils_1 = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 const locuszoom_1 = __importDefault(__webpack_require__( /*! locuszoom */ "webpack/sharing/consume/default/locuszoom/locuszoom"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
-                //import { untilReady } from './utils';
+                const utils_1 = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 // Import the CSS
                 __webpack_require__( /*! locuszoom/dist/locuszoom.css */ "./node_modules/locuszoom/dist/locuszoom.css");
                 __webpack_require__( /*! ../css/widget.css */ "./css/widget.css");
                 class LocusZoomModel extends base_1.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: LocusZoomModel.model_name,
@@ -146,32 +220,26 @@
                 class ModelAssociation extends AssociationLZ {
                     constructor(config) {
                         super({});
                         this.model = config.model;
                     }
                     _performRequest(options) {
                         return __awaiter(this, void 0, void 0, function*() {
-                            /**
-                            console.log('performing request', options);
-                            await untilReady(() => {
-                              const position = this.model.get('position');
-                              return (
-                                position.chr === options.chr
-                                &&
-                                position.start === options.start
-                                &&
-                                position.end === options.end
-                                )
-                            })
-                            console.log('got it!');
-                            */
-                            return {
-                                data: this.model.get('_associations_view'),
-                                lastPage: 100
-                            };
+                            // TODO: find a way to fetch view properly
+                            yield utils_1.untilReady(() => {
+                                const view = this.model.get('_associations_view');
+                                const position = view.range;
+                                console.log(position, options, (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end));
+                                return (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end);
+                            });
+                            return this.model.get('_associations_view');
                         });
                     }
                 }
                 // A custom adapter should be added to the registry before using it
                 locuszoom_1.default.Adapters.add('ModelAssociation', ModelAssociation);
                 class LocusZoomView extends base_1.DOMWidgetView {
                     constructor(options) {
@@ -186,88 +254,96 @@
                             case 'resize':
                                 console.log('resize message');
                                 window.requestAnimationFrame(() => this.plot.rescaleSVG());
                                 break;
                         }
                     }
                     processPhosphorMessage(msg) {
-                        this._processLuminoMessage(msg, super.processLuminoMessage);
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this._processLuminoMessage(msg, super.processPhosphorMessage);
                     }
                     processLuminoMessage(msg) {
                         this._processLuminoMessage(msg, super.processLuminoMessage);
                     }
                     render() {
-                        const apiBase = "https://portaldev.sph.umich.edu/api/v1/";
+                        const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
                         const build = this.model.get('build');
-                        var dataSources = new locuszoom_1.default.DataSources();
+                        const dataSources = new locuszoom_1.default.DataSources();
                         dataSources
-                            .add("assoc", ["ModelAssociation", {
+                            .add('assoc', ['ModelAssociation', {
                                 model: this.model
                             }])
-                            .add("ld", ["LDServer", {
-                                url: "https://portaldev.sph.umich.edu/ld/",
-                                source: '1000G',
-                                build,
-                                population: 'ALL'
-                            }])
-                            .add("gene", ["GeneLZ", {
-                                url: apiBase + "annotation/genes/",
+                            .add('ld', [
+                                'LDServer', {
+                                    url: 'https://portaldev.sph.umich.edu/ld/',
+                                    source: '1000G',
+                                    build,
+                                    population: 'ALL',
+                                },
+                            ])
+                            .add('gene', ['GeneLZ', {
+                                url: apiBase + 'annotation/genes/',
                                 build
                             }])
-                            .add("recomb", ["RecombLZ", {
-                                url: apiBase + "annotation/recomb/results/",
-                                build
-                            }])
-                            .add("constraint", ["GeneConstraintLZ", {
-                                url: "https://gnomad.broadinstitute.org/api/",
-                                build
-                            }]);
+                            .add('recomb', [
+                                'RecombLZ', {
+                                    url: apiBase + 'annotation/recomb/results/',
+                                    build
+                                },
+                            ])
+                            .add('constraint', [
+                                'GeneConstraintLZ', {
+                                    url: 'https://gnomad.broadinstitute.org/api/',
+                                    build
+                                },
+                            ]);
+                        // TODO:
+                        //.add("phewas", ["PheWASLZ", {url: "https://portaldev.sph.umich.edu/" + "api/v1/statistic/phewas/", build: [build]}])
                         const initialState = this.positionState;
                         console.log(initialState);
-                        const layout = locuszoom_1.default.Layouts.get("plot", "standard_association", {
-                            state: initialState
+                        const layout = locuszoom_1.default.Layouts.get('plot', 'standard_association', {
+                            state: initialState,
                         });
                         // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.
                         const attached = this.el.parentElement !== null;
                         if (!attached) {
                             document.body.appendChild(this.el);
                         }
-                        const plot = locuszoom_1.default.populate("#" + this.container.id, dataSources, layout);
+                        const plot = locuszoom_1.default.populate('#' + this.container.id, dataSources, layout);
                         if (!attached) {
                             document.body.removeChild(this.el);
                         }
                         this.plot = plot;
                         plot.on('state_changed', () => {
-                            console.log('state changed');
                             const position = this.model.get('position');
-                            if (plot.state.start == position.start &&
-                                plot.state.end == position.end &&
-                                plot.state.chr == position.chr) {
+                            if (plot.state.start === position.start &&
+                                plot.state.end === position.end &&
+                                plot.state.chr === position.chr) {
                                 return;
                             }
                             console.log('plot state changed, will set kernel state to', plot.state);
                             this.model.set('position', {
                                 start: plot.state.start,
                                 end: plot.state.end,
-                                chr: plot.state.chr
+                                chr: plot.state.chr,
                             });
                             this.model.save_changes();
                         });
                         const updateState = () => {
                             console.log('kernel state changed, will set state to ', this.positionState);
                             plot.applyState(Object.assign(Object.assign({}, this.positionState), {
-                                ldrefvar: ""
+                                ldrefvar: ''
                             }));
                         };
                         // listen to changes of state in kernel and update view accordingly
                         this.model.on('change:position', updateState);
                         this.displayed.then(() => {
                             this.plot.rescaleSVG();
                         });
-                        //this.model.on('change:_associations_view', updateState);
                     }
                     get positionState() {
                         return this.model.get('position');
                     }
                 }
                 exports.LocusZoomView = LocusZoomView;
 
@@ -320,8 +396,8 @@
                 module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.0","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.1de32fa6eec660baca88.js.map
+//# sourceMappingURL=lib_widget_js.751b11392fdca570e288.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.1de32fa6eec660baca88.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.751b11392fdca570e288.js.map`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071428571428572%*

 * *Differences: {"'file'": "'lib_widget_js.751b11392fdca570e288.js'",*

 * * "'mappings'": "';;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE; […]*

```diff
@@ -1,19 +1,21 @@
 {
-    "file": "lib_widget_js.1de32fa6eec660baca88.js",
-    "mappings": "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",
+    "file": "lib_widget_js.751b11392fdca570e288.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./css/widget.css",
+        "webpack://jupyter-locuszoom/./src/utils.ts",
         "webpack://jupyter-locuszoom/./src/version.ts",
         "webpack://jupyter-locuszoom/./src/widget.ts",
         "webpack://jupyter-locuszoom/./css/widget.css?a195"
     ],
     "sourcesContent": [
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
+        "async function sleep(timeout: number): Promise<void> {\n  return new Promise<void>((resolve) => {\n    setTimeout(() => {\n      resolve();\n    }, timeout);\n  });\n}\n\nexport function untilReady(\n  isReady: CallableFunction,\n  maxRetrials = 10,\n  interval = 75,\n  intervalModifier = (i: number) => i\n): Promise<CallableFunction> {\n  return (async () => {\n    let i = 0;\n    while (isReady() !== true) {\n      i += 1;\n      if (maxRetrials !== -1 && i > maxRetrials) {\n        throw Error('Too many retrials');\n      }\n      interval = intervalModifier(interval);\n      await sleep(interval);\n    }\n    return isReady;\n  })();\n}\n",
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n//import { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {}\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: {model: LocusZoomModel}) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    /**\n    console.log('performing request', options);\n    await untilReady(() => {\n      const position = this.model.get('position');\n      return (\n        position.chr === options.chr\n        &&\n        position.start === options.start\n        &&\n        position.end === options.end\n        )\n    })\n    console.log('got it!');\n    */\n    return {\n      data: this.model.get('_associations_view'),\n      lastPage: 100\n    };\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n   _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n       _super.call(this, msg);\n       switch (msg.type) {\n         case 'resize':\n           console.log('resize message')\n           window.requestAnimationFrame(() => this.plot.rescaleSVG());\n           break;\n       }\n  }\n  processPhosphorMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n\n processLuminoMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n  render() {\n    const apiBase = \"https://portaldev.sph.umich.edu/api/v1/\";\n    const build = this.model.get('build');\n\n    var dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add(\"assoc\", [\"ModelAssociation\", { model: this.model }])\n      .add(\"ld\", [\"LDServer\", { url: \"https://portaldev.sph.umich.edu/ld/\", source: '1000G', build, population: 'ALL' }])\n      .add(\"gene\", [\"GeneLZ\", { url: apiBase + \"annotation/genes/\", build }])\n      .add(\"recomb\", [\"RecombLZ\", { url: apiBase + \"annotation/recomb/results/\", build }])\n      .add(\"constraint\", [\"GeneConstraintLZ\", { url: \"https://gnomad.broadinstitute.org/api/\", build }]);\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get(\"plot\", \"standard_association\", {state: initialState});\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\"#\" + this.container.id, dataSources, layout);\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      console.log('state changed');\n      const position = this.model.get('position');\n      if (\n        plot.state.start == position.start\n        &&\n        plot.state.end == position.end\n        &&\n        plot.state.chr == position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to',  plot.state)\n      this.model.set('position', {start: plot.state.start, end: plot.state.end, chr: plot.state.chr});\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log('kernel state changed, will set state to ', this.positionState);\n      plot.applyState({ ...this.positionState, ldrefvar: \"\" });\n    }\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n    //this.model.on('change:_associations_view', updateState);\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
+        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {},\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: { model: LocusZoomModel }) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    await untilReady(() => {\n      const view = this.model.get('_associations_view');\n      const position = view.range;\n      console.log(position, options, (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      ))\n      return (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      );\n    });\n    return this.model.get('_associations_view');\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n  _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n    _super.call(this, msg);\n    switch (msg.type) {\n      case 'resize':\n        console.log('resize message');\n        window.requestAnimationFrame(() => this.plot.rescaleSVG());\n        break;\n    }\n  }\n  processPhosphorMessage(msg: Message): void {\n    // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n    // @ts-ignore\n    this._processLuminoMessage(msg, super.processPhosphorMessage);\n  }\n\n  processLuminoMessage(msg: Message): void {\n    this._processLuminoMessage(msg, super.processLuminoMessage);\n  }\n  render() {\n    const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';\n    const build = this.model.get('build');\n\n    const dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add('assoc', ['ModelAssociation', { model: this.model }])\n      .add('ld', [\n        'LDServer',\n        {\n          url: 'https://portaldev.sph.umich.edu/ld/',\n          source: '1000G',\n          build,\n          population: 'ALL',\n        },\n      ])\n      .add('gene', ['GeneLZ', { url: apiBase + 'annotation/genes/', build }])\n      .add('recomb', [\n        'RecombLZ',\n        { url: apiBase + 'annotation/recomb/results/', build },\n      ])\n      .add('constraint', [\n        'GeneConstraintLZ',\n        { url: 'https://gnomad.broadinstitute.org/api/', build },\n      ]);\n    // TODO:\n    //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get('plot', 'standard_association', {\n      state: initialState,\n    });\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\n      '#' + this.container.id,\n      dataSources,\n      layout\n    );\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      const position = this.model.get('position');\n      if (\n        plot.state.start === position.start &&\n        plot.state.end === position.end &&\n        plot.state.chr === position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to', plot.state);\n      this.model.set('position', {\n        start: plot.state.start,\n        end: plot.state.end,\n        chr: plot.state.chr,\n      });\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log(\n        'kernel state changed, will set state to ',\n        this.positionState\n      );\n      plot.applyState({ ...this.positionState, ldrefvar: '' });\n    };\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2b66441289369f8600c8.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.d278f1d07325a0e4e5cb.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,88 @@
                 module.exports = exports;
 
 
                 /***/
             }),
 
         /***/
+        "./lib/utils.js":
+            /*!**********************!*\
+              !*** ./lib/utils.js ***!
+              \**********************/
+            /***/
+            (function(__unused_webpack_module, exports) {
+
+                "use strict";
+
+                var __awaiter = (this && this.__awaiter) || function(thisArg, _arguments, P, generator) {
+                    function adopt(value) {
+                        return value instanceof P ? value : new P(function(resolve) {
+                            resolve(value);
+                        });
+                    }
+                    return new(P || (P = Promise))(function(resolve, reject) {
+                        function fulfilled(value) {
+                            try {
+                                step(generator.next(value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function rejected(value) {
+                            try {
+                                step(generator["throw"](value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function step(result) {
+                            result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected);
+                        }
+                        step((generator = generator.apply(thisArg, _arguments || [])).next());
+                    });
+                };
+                Object.defineProperty(exports, "__esModule", ({
+                    value: true
+                }));
+                exports.untilReady = void 0;
+
+                function sleep(timeout) {
+                    return __awaiter(this, void 0, void 0, function*() {
+                        return new Promise((resolve) => {
+                            setTimeout(() => {
+                                resolve();
+                            }, timeout);
+                        });
+                    });
+                }
+
+                function untilReady(isReady, maxRetrials = 15, interval = 75, intervalModifier = (i) => i) {
+                    return (() => __awaiter(this, void 0, void 0, function*() {
+                        let i = 0;
+                        while (isReady() !== true) {
+                            i += 1;
+                            if (maxRetrials !== -1 && i > maxRetrials) {
+                                throw Error('Too many retrials');
+                            }
+                            interval = intervalModifier(interval);
+                            yield sleep(interval);
+                        }
+                        return isReady;
+                    }))();
+                }
+                exports.untilReady = untilReady;
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/version.js":
             /*!************************!*\
               !*** ./lib/version.js ***!
               \************************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
@@ -107,34 +181,40 @@
                     value: true
                 }));
                 exports.LocusZoomView = exports.LocusZoomModel = void 0;
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const coreutils_1 = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 const locuszoom_1 = __importDefault(__webpack_require__( /*! locuszoom */ "webpack/sharing/consume/default/locuszoom/locuszoom"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
-                //import { untilReady } from './utils';
+                const utils_1 = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 // Import the CSS
                 __webpack_require__( /*! locuszoom/dist/locuszoom.css */ "./node_modules/locuszoom/dist/locuszoom.css");
                 __webpack_require__( /*! ../css/widget.css */ "./css/widget.css");
                 class LocusZoomModel extends base_1.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: LocusZoomModel.model_name,
                             _model_module: LocusZoomModel.model_module,
                             _model_module_version: LocusZoomModel.model_module_version,
                             _view_name: LocusZoomModel.view_name,
                             _view_module: LocusZoomModel.view_module,
                             _view_module_version: LocusZoomModel.view_module_version,
                             build: 'GRCh38',
                             position: {
-                                chrom: '1',
+                                chr: '1',
                                 start: 0,
                                 end: 5000000,
                             },
-                            _associations_view: {}
+                            _associations_view: {
+                                range: {
+                                    chr: '1',
+                                    start: 0,
+                                    end: 5000000,
+                                }
+                            }
                         });
                     }
                 }
                 exports.LocusZoomModel = LocusZoomModel;
                 LocusZoomModel.serializers = Object.assign({}, base_1.DOMWidgetModel.serializers);
                 LocusZoomModel.model_name = 'LocusZoomModel';
                 LocusZoomModel.model_module = version_1.MODULE_NAME;
@@ -146,109 +226,130 @@
                 class ModelAssociation extends AssociationLZ {
                     constructor(config) {
                         super({});
                         this.model = config.model;
                     }
                     _performRequest(options) {
                         return __awaiter(this, void 0, void 0, function*() {
-                            /**
-                            console.log('performing request', options);
-                            await untilReady(() => {
-                              const position = this.model.get('position');
-                              return (
-                                position.chr === options.chr
-                                &&
-                                position.start === options.start
-                                &&
-                                position.end === options.end
-                                )
-                            })
-                            console.log('got it!');
-                            */
-                            return {
-                                data: this.model.get('_associations_view'),
-                                lastPage: 100
-                            };
+                            // TODO: find a way to fetch view properly
+                            yield utils_1.untilReady(() => {
+                                const view = this.model.get('_associations_view');
+                                const position = view.range;
+                                console.log(position, options, (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end));
+                                return (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end);
+                            });
+                            return this.model.get('_associations_view');
                         });
                     }
                 }
                 // A custom adapter should be added to the registry before using it
                 locuszoom_1.default.Adapters.add('ModelAssociation', ModelAssociation);
                 class LocusZoomView extends base_1.DOMWidgetView {
                     constructor(options) {
                         super(options);
                         this.container = document.createElement('div');
                         this.container.id = 'locus-zoom-' + coreutils_1.UUID.uuid4();
                         this.el.appendChild(this.container);
                     }
+                    _processLuminoMessage(msg, _super) {
+                        _super.call(this, msg);
+                        switch (msg.type) {
+                            case 'resize':
+                                console.log('resize message');
+                                window.requestAnimationFrame(() => this.plot.rescaleSVG());
+                                break;
+                        }
+                    }
+                    processPhosphorMessage(msg) {
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this._processLuminoMessage(msg, super.processPhosphorMessage);
+                    }
+                    processLuminoMessage(msg) {
+                        this._processLuminoMessage(msg, super.processLuminoMessage);
+                    }
                     render() {
-                        const apiBase = "https://portaldev.sph.umich.edu/api/v1/";
+                        const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
                         const build = this.model.get('build');
-                        var dataSources = new locuszoom_1.default.DataSources();
+                        const dataSources = new locuszoom_1.default.DataSources();
                         dataSources
-                            .add("assoc", ["ModelAssociation", {
+                            .add('assoc', ['ModelAssociation', {
                                 model: this.model
                             }])
-                            .add("ld", ["LDServer", {
-                                url: "https://portaldev.sph.umich.edu/ld/",
-                                source: '1000G',
-                                build,
-                                population: 'ALL'
-                            }])
-                            .add("gene", ["GeneLZ", {
-                                url: apiBase + "annotation/genes/",
+                            .add('ld', [
+                                'LDServer', {
+                                    url: 'https://portaldev.sph.umich.edu/ld/',
+                                    source: '1000G',
+                                    build,
+                                    population: 'ALL',
+                                },
+                            ])
+                            .add('gene', ['GeneLZ', {
+                                url: apiBase + 'annotation/genes/',
                                 build
                             }])
-                            .add("recomb", ["RecombLZ", {
-                                url: apiBase + "annotation/recomb/results/",
-                                build
-                            }])
-                            .add("constraint", ["GeneConstraintLZ", {
-                                url: "https://gnomad.broadinstitute.org/api/",
-                                build
-                            }]);
+                            .add('recomb', [
+                                'RecombLZ', {
+                                    url: apiBase + 'annotation/recomb/results/',
+                                    build
+                                },
+                            ])
+                            .add('constraint', [
+                                'GeneConstraintLZ', {
+                                    url: 'https://gnomad.broadinstitute.org/api/',
+                                    build
+                                },
+                            ]);
+                        // TODO:
+                        //.add("phewas", ["PheWASLZ", {url: "https://portaldev.sph.umich.edu/" + "api/v1/statistic/phewas/", build: [build]}])
                         const initialState = this.positionState;
                         console.log(initialState);
-                        const layout = locuszoom_1.default.Layouts.get("plot", "standard_association", {
-                            state: initialState
+                        const layout = locuszoom_1.default.Layouts.get('plot', 'standard_association', {
+                            state: initialState,
                         });
                         // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.
                         const attached = this.el.parentElement !== null;
                         if (!attached) {
                             document.body.appendChild(this.el);
                         }
-                        const plot = locuszoom_1.default.populate("#" + this.container.id, dataSources, layout);
+                        const plot = locuszoom_1.default.populate('#' + this.container.id, dataSources, layout);
                         if (!attached) {
                             document.body.removeChild(this.el);
                         }
+                        this.plot = plot;
                         plot.on('state_changed', () => {
-                            console.log('state changed');
                             const position = this.model.get('position');
-                            if (plot.state.start == position.start &&
-                                plot.state.end == position.end &&
-                                plot.state.chr == position.chrom) {
+                            if (plot.state.start === position.start &&
+                                plot.state.end === position.end &&
+                                plot.state.chr === position.chr) {
                                 return;
                             }
                             console.log('plot state changed, will set kernel state to', plot.state);
                             this.model.set('position', {
                                 start: plot.state.start,
                                 end: plot.state.end,
-                                chr: plot.state.chr
+                                chr: plot.state.chr,
                             });
                             this.model.save_changes();
                         });
                         const updateState = () => {
                             console.log('kernel state changed, will set state to ', this.positionState);
                             plot.applyState(Object.assign(Object.assign({}, this.positionState), {
-                                ldrefvar: ""
+                                ldrefvar: ''
                             }));
                         };
                         // listen to changes of state in kernel and update view accordingly
                         this.model.on('change:position', updateState);
-                        //this.model.on('change:_associations_view', updateState);
+                        this.displayed.then(() => {
+                            this.plot.rescaleSVG();
+                        });
                     }
                     get positionState() {
                         return this.model.get('position');
                     }
                 }
                 exports.LocusZoomView = LocusZoomView;
 
@@ -301,8 +402,8 @@
                 module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.0","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.2b66441289369f8600c8.js.map
+//# sourceMappingURL=lib_widget_js.d278f1d07325a0e4e5cb.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2b66441289369f8600c8.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.d278f1d07325a0e4e5cb.js.map`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071428571428572%*

 * *Differences: {"'file'": "'lib_widget_js.d278f1d07325a0e4e5cb.js'",*

 * * "'mappings'": "';;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE; […]*

```diff
@@ -1,19 +1,21 @@
 {
-    "file": "lib_widget_js.2b66441289369f8600c8.js",
-    "mappings": "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",
+    "file": "lib_widget_js.d278f1d07325a0e4e5cb.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./css/widget.css",
+        "webpack://jupyter-locuszoom/./src/utils.ts",
         "webpack://jupyter-locuszoom/./src/version.ts",
         "webpack://jupyter-locuszoom/./src/widget.ts",
         "webpack://jupyter-locuszoom/./css/widget.css?a195"
     ],
     "sourcesContent": [
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
+        "async function sleep(timeout: number): Promise<void> {\n  return new Promise<void>((resolve) => {\n    setTimeout(() => {\n      resolve();\n    }, timeout);\n  });\n}\n\nexport function untilReady(\n  isReady: CallableFunction,\n  maxRetrials = 15,\n  interval = 75,\n  intervalModifier = (i: number) => i\n): Promise<CallableFunction> {\n  return (async () => {\n    let i = 0;\n    while (isReady() !== true) {\n      i += 1;\n      if (maxRetrials !== -1 && i > maxRetrials) {\n        throw Error('Too many retrials');\n      }\n      interval = intervalModifier(interval);\n      await sleep(interval);\n    }\n    return isReady;\n  })();\n}\n",
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n//import { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chrom: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {}\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: {model: LocusZoomModel}) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    /**\n    console.log('performing request', options);\n    await untilReady(() => {\n      const position = this.model.get('position');\n      return (\n        position.chr === options.chr\n        &&\n        position.start === options.start\n        &&\n        position.end === options.end\n        )\n    })\n    console.log('got it!');\n    */\n    return{\n      data: this.model.get('_associations_view'),\n      lastPage: 100\n    };\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n   _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n       _super.call(this, msg);\n       switch (msg.type) {\n         case 'resize':\n             this.resize();\n             break;\n       }\n  }\n  render() {\n    const apiBase = \"https://portaldev.sph.umich.edu/api/v1/\";\n    const build = this.model.get('build');\n\n    var dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add(\"assoc\", [\"ModelAssociation\", { model: this.model }])\n      .add(\"ld\", [\"LDServer\", { url: \"https://portaldev.sph.umich.edu/ld/\", source: '1000G', build, population: 'ALL' }])\n      .add(\"gene\", [\"GeneLZ\", { url: apiBase + \"annotation/genes/\", build }])\n      .add(\"recomb\", [\"RecombLZ\", { url: apiBase + \"annotation/recomb/results/\", build }])\n      .add(\"constraint\", [\"GeneConstraintLZ\", { url: \"https://gnomad.broadinstitute.org/api/\", build }]);\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get(\"plot\", \"standard_association\", {state: initialState});\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\"#\" + this.container.id, dataSources, layout);\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n\n    plot.on('state_changed', () => {\n      console.log('state changed');\n      const position = this.model.get('position');\n      if (\n        plot.state.start == position.start\n        &&\n        plot.state.end == position.end\n        &&\n        plot.state.chr == position.chrom\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to',  plot.state)\n      this.model.set('position', {start: plot.state.start, end: plot.state.end, chr: plot.state.chr});\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log('kernel state changed, will set state to ', this.positionState);\n      plot.applyState({ ...this.positionState, ldrefvar: \"\" });\n    }\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    //this.model.on('change:_associations_view', updateState);\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
+        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {\n        range: {\n          chr: '1',\n          start: 0,\n          end: 5000000,\n        }\n      },\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: { model: LocusZoomModel }) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    await untilReady(() => {\n      const view = this.model.get('_associations_view');\n      const position = view.range;\n      console.log(position, options, (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      ))\n      return (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      );\n    });\n    return this.model.get('_associations_view');\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n  _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n    _super.call(this, msg);\n    switch (msg.type) {\n      case 'resize':\n        console.log('resize message');\n        window.requestAnimationFrame(() => this.plot.rescaleSVG());\n        break;\n    }\n  }\n  processPhosphorMessage(msg: Message): void {\n    // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n    // @ts-ignore\n    this._processLuminoMessage(msg, super.processPhosphorMessage);\n  }\n\n  processLuminoMessage(msg: Message): void {\n    this._processLuminoMessage(msg, super.processLuminoMessage);\n  }\n  render() {\n    const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';\n    const build = this.model.get('build');\n\n    const dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add('assoc', ['ModelAssociation', { model: this.model }])\n      .add('ld', [\n        'LDServer',\n        {\n          url: 'https://portaldev.sph.umich.edu/ld/',\n          source: '1000G',\n          build,\n          population: 'ALL',\n        },\n      ])\n      .add('gene', ['GeneLZ', { url: apiBase + 'annotation/genes/', build }])\n      .add('recomb', [\n        'RecombLZ',\n        { url: apiBase + 'annotation/recomb/results/', build },\n      ])\n      .add('constraint', [\n        'GeneConstraintLZ',\n        { url: 'https://gnomad.broadinstitute.org/api/', build },\n      ]);\n    // TODO:\n    //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get('plot', 'standard_association', {\n      state: initialState,\n    });\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\n      '#' + this.container.id,\n      dataSources,\n      layout\n    );\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      const position = this.model.get('position');\n      if (\n        plot.state.start === position.start &&\n        plot.state.end === position.end &&\n        plot.state.chr === position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to', plot.state);\n      this.model.set('position', {\n        start: plot.state.start,\n        end: plot.state.end,\n        chr: plot.state.chr,\n      });\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log(\n        'kernel state changed, will set state to ',\n        this.positionState\n      );\n      plot.applyState({ ...this.positionState, ldrefvar: '' });\n    };\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2bf13a2b62c6e59e7386.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.dc6697cf94dcc4cb14bc.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,88 @@
                 module.exports = exports;
 
 
                 /***/
             }),
 
         /***/
+        "./lib/utils.js":
+            /*!**********************!*\
+              !*** ./lib/utils.js ***!
+              \**********************/
+            /***/
+            (function(__unused_webpack_module, exports) {
+
+                "use strict";
+
+                var __awaiter = (this && this.__awaiter) || function(thisArg, _arguments, P, generator) {
+                    function adopt(value) {
+                        return value instanceof P ? value : new P(function(resolve) {
+                            resolve(value);
+                        });
+                    }
+                    return new(P || (P = Promise))(function(resolve, reject) {
+                        function fulfilled(value) {
+                            try {
+                                step(generator.next(value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function rejected(value) {
+                            try {
+                                step(generator["throw"](value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function step(result) {
+                            result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected);
+                        }
+                        step((generator = generator.apply(thisArg, _arguments || [])).next());
+                    });
+                };
+                Object.defineProperty(exports, "__esModule", ({
+                    value: true
+                }));
+                exports.untilReady = void 0;
+
+                function sleep(timeout) {
+                    return __awaiter(this, void 0, void 0, function*() {
+                        return new Promise((resolve) => {
+                            setTimeout(() => {
+                                resolve();
+                            }, timeout);
+                        });
+                    });
+                }
+
+                function untilReady(isReady, maxRetrials = 20, interval = 75, intervalModifier = (i) => i) {
+                    return (() => __awaiter(this, void 0, void 0, function*() {
+                        let i = 0;
+                        while (isReady() !== true) {
+                            i += 1;
+                            if (maxRetrials !== -1 && i > maxRetrials) {
+                                throw Error('Too many retrials');
+                            }
+                            interval = intervalModifier(interval);
+                            yield sleep(interval);
+                        }
+                        return isReady;
+                    }))();
+                }
+                exports.untilReady = untilReady;
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/version.js":
             /*!************************!*\
               !*** ./lib/version.js ***!
               \************************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
@@ -107,34 +181,40 @@
                     value: true
                 }));
                 exports.LocusZoomView = exports.LocusZoomModel = void 0;
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const coreutils_1 = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 const locuszoom_1 = __importDefault(__webpack_require__( /*! locuszoom */ "webpack/sharing/consume/default/locuszoom/locuszoom"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
-                //import { untilReady } from './utils';
+                const utils_1 = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 // Import the CSS
                 __webpack_require__( /*! locuszoom/dist/locuszoom.css */ "./node_modules/locuszoom/dist/locuszoom.css");
                 __webpack_require__( /*! ../css/widget.css */ "./css/widget.css");
                 class LocusZoomModel extends base_1.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: LocusZoomModel.model_name,
                             _model_module: LocusZoomModel.model_module,
                             _model_module_version: LocusZoomModel.model_module_version,
                             _view_name: LocusZoomModel.view_name,
                             _view_module: LocusZoomModel.view_module,
                             _view_module_version: LocusZoomModel.view_module_version,
                             build: 'GRCh38',
                             position: {
-                                chrom: '1',
+                                chr: '1',
                                 start: 0,
                                 end: 5000000,
                             },
-                            _associations_view: {}
+                            _associations_view: {
+                                range: {
+                                    chr: '1',
+                                    start: 0,
+                                    end: 5000000,
+                                }
+                            }
                         });
                     }
                 }
                 exports.LocusZoomModel = LocusZoomModel;
                 LocusZoomModel.serializers = Object.assign({}, base_1.DOMWidgetModel.serializers);
                 LocusZoomModel.model_name = 'LocusZoomModel';
                 LocusZoomModel.model_module = version_1.MODULE_NAME;
@@ -146,32 +226,26 @@
                 class ModelAssociation extends AssociationLZ {
                     constructor(config) {
                         super({});
                         this.model = config.model;
                     }
                     _performRequest(options) {
                         return __awaiter(this, void 0, void 0, function*() {
-                            /**
-                            console.log('performing request', options);
-                            await untilReady(() => {
-                              const position = this.model.get('position');
-                              return (
-                                position.chr === options.chr
-                                &&
-                                position.start === options.start
-                                &&
-                                position.end === options.end
-                                )
-                            })
-                            console.log('got it!');
-                            */
-                            return {
-                                data: this.model.get('_associations_view'),
-                                lastPage: 100
-                            };
+                            // TODO: find a way to fetch view properly
+                            yield utils_1.untilReady(() => {
+                                const view = this.model.get('_associations_view');
+                                const position = view.range;
+                                console.log(position, options, (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end));
+                                return (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end);
+                            });
+                            return this.model.get('_associations_view');
                         });
                     }
                 }
                 // A custom adapter should be added to the registry before using it
                 locuszoom_1.default.Adapters.add('ModelAssociation', ModelAssociation);
                 class LocusZoomView extends base_1.DOMWidgetView {
                     constructor(options) {
@@ -180,87 +254,102 @@
                         this.container.id = 'locus-zoom-' + coreutils_1.UUID.uuid4();
                         this.el.appendChild(this.container);
                     }
                     _processLuminoMessage(msg, _super) {
                         _super.call(this, msg);
                         switch (msg.type) {
                             case 'resize':
-                                this.plot.rescaleSVG();
+                                console.log('resize message');
+                                window.requestAnimationFrame(() => this.plot.rescaleSVG());
                                 break;
                         }
                     }
+                    processPhosphorMessage(msg) {
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this._processLuminoMessage(msg, super.processPhosphorMessage);
+                    }
+                    processLuminoMessage(msg) {
+                        this._processLuminoMessage(msg, super.processLuminoMessage);
+                    }
                     render() {
-                        const apiBase = "https://portaldev.sph.umich.edu/api/v1/";
+                        const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
                         const build = this.model.get('build');
-                        var dataSources = new locuszoom_1.default.DataSources();
+                        const dataSources = new locuszoom_1.default.DataSources();
                         dataSources
-                            .add("assoc", ["ModelAssociation", {
+                            .add('assoc', ['ModelAssociation', {
                                 model: this.model
                             }])
-                            .add("ld", ["LDServer", {
-                                url: "https://portaldev.sph.umich.edu/ld/",
-                                source: '1000G',
-                                build,
-                                population: 'ALL'
-                            }])
-                            .add("gene", ["GeneLZ", {
-                                url: apiBase + "annotation/genes/",
+                            .add('ld', [
+                                'LDServer', {
+                                    url: 'https://portaldev.sph.umich.edu/ld/',
+                                    source: '1000G',
+                                    build,
+                                    population: 'ALL',
+                                },
+                            ])
+                            .add('gene', ['GeneLZ', {
+                                url: apiBase + 'annotation/genes/',
                                 build
                             }])
-                            .add("recomb", ["RecombLZ", {
-                                url: apiBase + "annotation/recomb/results/",
-                                build
-                            }])
-                            .add("constraint", ["GeneConstraintLZ", {
-                                url: "https://gnomad.broadinstitute.org/api/",
-                                build
-                            }]);
+                            .add('recomb', [
+                                'RecombLZ', {
+                                    url: apiBase + 'annotation/recomb/results/',
+                                    build
+                                },
+                            ])
+                            .add('constraint', [
+                                'GeneConstraintLZ', {
+                                    url: 'https://gnomad.broadinstitute.org/api/',
+                                    build
+                                },
+                            ]);
+                        // TODO:
+                        //.add("phewas", ["PheWASLZ", {url: "https://portaldev.sph.umich.edu/" + "api/v1/statistic/phewas/", build: [build]}])
                         const initialState = this.positionState;
                         console.log(initialState);
-                        const layout = locuszoom_1.default.Layouts.get("plot", "standard_association", {
-                            state: initialState
+                        const layout = locuszoom_1.default.Layouts.get('plot', 'standard_association', {
+                            state: initialState,
                         });
                         // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.
                         const attached = this.el.parentElement !== null;
                         if (!attached) {
                             document.body.appendChild(this.el);
                         }
-                        const plot = locuszoom_1.default.populate("#" + this.container.id, dataSources, layout);
+                        const plot = locuszoom_1.default.populate('#' + this.container.id, dataSources, layout);
                         if (!attached) {
                             document.body.removeChild(this.el);
                         }
                         this.plot = plot;
                         plot.on('state_changed', () => {
-                            console.log('state changed');
                             const position = this.model.get('position');
-                            if (plot.state.start == position.start &&
-                                plot.state.end == position.end &&
-                                plot.state.chr == position.chrom) {
+                            if (plot.state.start === position.start &&
+                                plot.state.end === position.end &&
+                                plot.state.chr === position.chr) {
                                 return;
                             }
                             console.log('plot state changed, will set kernel state to', plot.state);
                             this.model.set('position', {
                                 start: plot.state.start,
                                 end: plot.state.end,
-                                chr: plot.state.chr
+                                chr: plot.state.chr,
                             });
                             this.model.save_changes();
                         });
                         const updateState = () => {
                             console.log('kernel state changed, will set state to ', this.positionState);
                             plot.applyState(Object.assign(Object.assign({}, this.positionState), {
-                                ldrefvar: ""
+                                ldrefvar: ''
                             }));
                         };
                         // listen to changes of state in kernel and update view accordingly
                         this.model.on('change:position', updateState);
                         this.displayed.then(() => {
                             this.plot.rescaleSVG();
                         });
-                        //this.model.on('change:_associations_view', updateState);
                     }
                     get positionState() {
                         return this.model.get('position');
                     }
                 }
                 exports.LocusZoomView = LocusZoomView;
 
@@ -313,8 +402,8 @@
                 module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.0","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.2bf13a2b62c6e59e7386.js.map
+//# sourceMappingURL=lib_widget_js.dc6697cf94dcc4cb14bc.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.2bf13a2b62c6e59e7386.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff0b505f89816ef2fa6c.js.map`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071428571428572%*

 * *Differences: {"'file'": "'lib_widget_js.ff0b505f89816ef2fa6c.js'",*

 * * "'mappings'": "';;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE; […]*

```diff
@@ -1,19 +1,21 @@
 {
-    "file": "lib_widget_js.2bf13a2b62c6e59e7386.js",
-    "mappings": "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",
+    "file": "lib_widget_js.ff0b505f89816ef2fa6c.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./css/widget.css",
+        "webpack://jupyter-locuszoom/./src/utils.ts",
         "webpack://jupyter-locuszoom/./src/version.ts",
         "webpack://jupyter-locuszoom/./src/widget.ts",
         "webpack://jupyter-locuszoom/./css/widget.css?a195"
     ],
     "sourcesContent": [
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
+        "async function sleep(timeout: number): Promise<void> {\n  return new Promise<void>((resolve) => {\n    setTimeout(() => {\n      resolve();\n    }, timeout);\n  });\n}\n\nexport function untilReady(\n  isReady: CallableFunction,\n  maxRetrials = 10,\n  interval = 75,\n  intervalModifier = (i: number) => i\n): Promise<CallableFunction> {\n  return (async () => {\n    let i = 0;\n    while (isReady() !== true) {\n      i += 1;\n      if (maxRetrials !== -1 && i > maxRetrials) {\n        throw Error('Too many retrials');\n      }\n      interval = intervalModifier(interval);\n      await sleep(interval);\n    }\n    return isReady;\n  })();\n}\n",
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n//import { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chrom: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {}\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: {model: LocusZoomModel}) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    /**\n    console.log('performing request', options);\n    await untilReady(() => {\n      const position = this.model.get('position');\n      return (\n        position.chr === options.chr\n        &&\n        position.start === options.start\n        &&\n        position.end === options.end\n        )\n    })\n    console.log('got it!');\n    */\n    return{\n      data: this.model.get('_associations_view'),\n      lastPage: 100\n    };\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n   _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n       _super.call(this, msg);\n       switch (msg.type) {\n         case 'resize':\n             this.plot.rescaleSVG();\n             break;\n       }\n  }\n  render() {\n    const apiBase = \"https://portaldev.sph.umich.edu/api/v1/\";\n    const build = this.model.get('build');\n\n    var dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add(\"assoc\", [\"ModelAssociation\", { model: this.model }])\n      .add(\"ld\", [\"LDServer\", { url: \"https://portaldev.sph.umich.edu/ld/\", source: '1000G', build, population: 'ALL' }])\n      .add(\"gene\", [\"GeneLZ\", { url: apiBase + \"annotation/genes/\", build }])\n      .add(\"recomb\", [\"RecombLZ\", { url: apiBase + \"annotation/recomb/results/\", build }])\n      .add(\"constraint\", [\"GeneConstraintLZ\", { url: \"https://gnomad.broadinstitute.org/api/\", build }]);\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get(\"plot\", \"standard_association\", {state: initialState});\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\"#\" + this.container.id, dataSources, layout);\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      console.log('state changed');\n      const position = this.model.get('position');\n      if (\n        plot.state.start == position.start\n        &&\n        plot.state.end == position.end\n        &&\n        plot.state.chr == position.chrom\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to',  plot.state)\n      this.model.set('position', {start: plot.state.start, end: plot.state.end, chr: plot.state.chr});\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log('kernel state changed, will set state to ', this.positionState);\n      plot.applyState({ ...this.positionState, ldrefvar: \"\" });\n    }\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n    //this.model.on('change:_associations_view', updateState);\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
+        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {\n        range: {\n          chr: '1',\n          start: 0,\n          end: 5000000,\n        }\n      },\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: { model: LocusZoomModel }) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    await untilReady(() => {\n      const view = this.model.get('_associations_view');\n      const position = view.range;\n      console.log(position, options, (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      ))\n      return (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      );\n    });\n    return this.model.get('_associations_view');\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n  _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n    _super.call(this, msg);\n    switch (msg.type) {\n      case 'resize':\n        console.log('resize message');\n        window.requestAnimationFrame(() => this.plot.rescaleSVG());\n        break;\n    }\n  }\n  processPhosphorMessage(msg: Message): void {\n    // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n    // @ts-ignore\n    this._processLuminoMessage(msg, super.processPhosphorMessage);\n  }\n\n  processLuminoMessage(msg: Message): void {\n    this._processLuminoMessage(msg, super.processLuminoMessage);\n  }\n  render() {\n    const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';\n    const build = this.model.get('build');\n\n    const dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add('assoc', ['ModelAssociation', { model: this.model }])\n      .add('ld', [\n        'LDServer',\n        {\n          url: 'https://portaldev.sph.umich.edu/ld/',\n          source: '1000G',\n          build,\n          population: 'ALL',\n        },\n      ])\n      .add('gene', ['GeneLZ', { url: apiBase + 'annotation/genes/', build }])\n      .add('recomb', [\n        'RecombLZ',\n        { url: apiBase + 'annotation/recomb/results/', build },\n      ])\n      .add('constraint', [\n        'GeneConstraintLZ',\n        { url: 'https://gnomad.broadinstitute.org/api/', build },\n      ]);\n    // TODO:\n    //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get('plot', 'standard_association', {\n      state: initialState,\n    });\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\n      '#' + this.container.id,\n      dataSources,\n      layout\n    );\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      const position = this.model.get('position');\n      if (\n        plot.state.start === position.start &&\n        plot.state.end === position.end &&\n        plot.state.chr === position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to', plot.state);\n      this.model.set('position', {\n        start: plot.state.start,\n        end: plot.state.end,\n        chr: plot.state.chr,\n      });\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log(\n        'kernel state changed, will set state to ',\n        this.positionState\n      );\n      plot.applyState({ ...this.positionState, ldrefvar: '' });\n    };\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.4dd25bf992348c7ee2aa.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.ff0b505f89816ef2fa6c.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,88 @@
                 module.exports = exports;
 
 
                 /***/
             }),
 
         /***/
+        "./lib/utils.js":
+            /*!**********************!*\
+              !*** ./lib/utils.js ***!
+              \**********************/
+            /***/
+            (function(__unused_webpack_module, exports) {
+
+                "use strict";
+
+                var __awaiter = (this && this.__awaiter) || function(thisArg, _arguments, P, generator) {
+                    function adopt(value) {
+                        return value instanceof P ? value : new P(function(resolve) {
+                            resolve(value);
+                        });
+                    }
+                    return new(P || (P = Promise))(function(resolve, reject) {
+                        function fulfilled(value) {
+                            try {
+                                step(generator.next(value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function rejected(value) {
+                            try {
+                                step(generator["throw"](value));
+                            } catch (e) {
+                                reject(e);
+                            }
+                        }
+
+                        function step(result) {
+                            result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected);
+                        }
+                        step((generator = generator.apply(thisArg, _arguments || [])).next());
+                    });
+                };
+                Object.defineProperty(exports, "__esModule", ({
+                    value: true
+                }));
+                exports.untilReady = void 0;
+
+                function sleep(timeout) {
+                    return __awaiter(this, void 0, void 0, function*() {
+                        return new Promise((resolve) => {
+                            setTimeout(() => {
+                                resolve();
+                            }, timeout);
+                        });
+                    });
+                }
+
+                function untilReady(isReady, maxRetrials = 10, interval = 75, intervalModifier = (i) => i) {
+                    return (() => __awaiter(this, void 0, void 0, function*() {
+                        let i = 0;
+                        while (isReady() !== true) {
+                            i += 1;
+                            if (maxRetrials !== -1 && i > maxRetrials) {
+                                throw Error('Too many retrials');
+                            }
+                            interval = intervalModifier(interval);
+                            yield sleep(interval);
+                        }
+                        return isReady;
+                    }))();
+                }
+                exports.untilReady = untilReady;
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/version.js":
             /*!************************!*\
               !*** ./lib/version.js ***!
               \************************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
@@ -107,34 +181,40 @@
                     value: true
                 }));
                 exports.LocusZoomView = exports.LocusZoomModel = void 0;
                 const base_1 = __webpack_require__( /*! @jupyter-widgets/base */ "webpack/sharing/consume/default/@jupyter-widgets/base");
                 const coreutils_1 = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 const locuszoom_1 = __importDefault(__webpack_require__( /*! locuszoom */ "webpack/sharing/consume/default/locuszoom/locuszoom"));
                 const version_1 = __webpack_require__( /*! ./version */ "./lib/version.js");
-                //import { untilReady } from './utils';
+                const utils_1 = __webpack_require__( /*! ./utils */ "./lib/utils.js");
                 // Import the CSS
                 __webpack_require__( /*! locuszoom/dist/locuszoom.css */ "./node_modules/locuszoom/dist/locuszoom.css");
                 __webpack_require__( /*! ../css/widget.css */ "./css/widget.css");
                 class LocusZoomModel extends base_1.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: LocusZoomModel.model_name,
                             _model_module: LocusZoomModel.model_module,
                             _model_module_version: LocusZoomModel.model_module_version,
                             _view_name: LocusZoomModel.view_name,
                             _view_module: LocusZoomModel.view_module,
                             _view_module_version: LocusZoomModel.view_module_version,
                             build: 'GRCh38',
                             position: {
-                                chrom: '1',
+                                chr: '1',
                                 start: 0,
                                 end: 5000000,
                             },
-                            _associations_view: {}
+                            _associations_view: {
+                                range: {
+                                    chr: '1',
+                                    start: 0,
+                                    end: 5000000,
+                                }
+                            }
                         });
                     }
                 }
                 exports.LocusZoomModel = LocusZoomModel;
                 LocusZoomModel.serializers = Object.assign({}, base_1.DOMWidgetModel.serializers);
                 LocusZoomModel.model_name = 'LocusZoomModel';
                 LocusZoomModel.model_module = version_1.MODULE_NAME;
@@ -146,32 +226,26 @@
                 class ModelAssociation extends AssociationLZ {
                     constructor(config) {
                         super({});
                         this.model = config.model;
                     }
                     _performRequest(options) {
                         return __awaiter(this, void 0, void 0, function*() {
-                            /**
-                            console.log('performing request', options);
-                            await untilReady(() => {
-                              const position = this.model.get('position');
-                              return (
-                                position.chr === options.chr
-                                &&
-                                position.start === options.start
-                                &&
-                                position.end === options.end
-                                )
-                            })
-                            console.log('got it!');
-                            */
-                            return {
-                                data: this.model.get('_associations_view'),
-                                lastPage: 100
-                            };
+                            // TODO: find a way to fetch view properly
+                            yield utils_1.untilReady(() => {
+                                const view = this.model.get('_associations_view');
+                                const position = view.range;
+                                console.log(position, options, (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end));
+                                return (position.chr === options.chr &&
+                                    position.start === options.start &&
+                                    position.end === options.end);
+                            });
+                            return this.model.get('_associations_view');
                         });
                     }
                 }
                 // A custom adapter should be added to the registry before using it
                 locuszoom_1.default.Adapters.add('ModelAssociation', ModelAssociation);
                 class LocusZoomView extends base_1.DOMWidgetView {
                     constructor(options) {
@@ -185,83 +259,97 @@
                         switch (msg.type) {
                             case 'resize':
                                 console.log('resize message');
                                 window.requestAnimationFrame(() => this.plot.rescaleSVG());
                                 break;
                         }
                     }
+                    processPhosphorMessage(msg) {
+                        // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+                        // @ts-ignore
+                        this._processLuminoMessage(msg, super.processPhosphorMessage);
+                    }
+                    processLuminoMessage(msg) {
+                        this._processLuminoMessage(msg, super.processLuminoMessage);
+                    }
                     render() {
-                        const apiBase = "https://portaldev.sph.umich.edu/api/v1/";
+                        const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
                         const build = this.model.get('build');
-                        var dataSources = new locuszoom_1.default.DataSources();
+                        const dataSources = new locuszoom_1.default.DataSources();
                         dataSources
-                            .add("assoc", ["ModelAssociation", {
+                            .add('assoc', ['ModelAssociation', {
                                 model: this.model
                             }])
-                            .add("ld", ["LDServer", {
-                                url: "https://portaldev.sph.umich.edu/ld/",
-                                source: '1000G',
-                                build,
-                                population: 'ALL'
-                            }])
-                            .add("gene", ["GeneLZ", {
-                                url: apiBase + "annotation/genes/",
+                            .add('ld', [
+                                'LDServer', {
+                                    url: 'https://portaldev.sph.umich.edu/ld/',
+                                    source: '1000G',
+                                    build,
+                                    population: 'ALL',
+                                },
+                            ])
+                            .add('gene', ['GeneLZ', {
+                                url: apiBase + 'annotation/genes/',
                                 build
                             }])
-                            .add("recomb", ["RecombLZ", {
-                                url: apiBase + "annotation/recomb/results/",
-                                build
-                            }])
-                            .add("constraint", ["GeneConstraintLZ", {
-                                url: "https://gnomad.broadinstitute.org/api/",
-                                build
-                            }]);
+                            .add('recomb', [
+                                'RecombLZ', {
+                                    url: apiBase + 'annotation/recomb/results/',
+                                    build
+                                },
+                            ])
+                            .add('constraint', [
+                                'GeneConstraintLZ', {
+                                    url: 'https://gnomad.broadinstitute.org/api/',
+                                    build
+                                },
+                            ]);
+                        // TODO:
+                        //.add("phewas", ["PheWASLZ", {url: "https://portaldev.sph.umich.edu/" + "api/v1/statistic/phewas/", build: [build]}])
                         const initialState = this.positionState;
                         console.log(initialState);
-                        const layout = locuszoom_1.default.Layouts.get("plot", "standard_association", {
-                            state: initialState
+                        const layout = locuszoom_1.default.Layouts.get('plot', 'standard_association', {
+                            state: initialState,
                         });
                         // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.
                         const attached = this.el.parentElement !== null;
                         if (!attached) {
                             document.body.appendChild(this.el);
                         }
-                        const plot = locuszoom_1.default.populate("#" + this.container.id, dataSources, layout);
+                        const plot = locuszoom_1.default.populate('#' + this.container.id, dataSources, layout);
                         if (!attached) {
                             document.body.removeChild(this.el);
                         }
                         this.plot = plot;
                         plot.on('state_changed', () => {
-                            console.log('state changed');
                             const position = this.model.get('position');
-                            if (plot.state.start == position.start &&
-                                plot.state.end == position.end &&
-                                plot.state.chr == position.chrom) {
+                            if (plot.state.start === position.start &&
+                                plot.state.end === position.end &&
+                                plot.state.chr === position.chr) {
                                 return;
                             }
                             console.log('plot state changed, will set kernel state to', plot.state);
                             this.model.set('position', {
                                 start: plot.state.start,
                                 end: plot.state.end,
-                                chr: plot.state.chr
+                                chr: plot.state.chr,
                             });
                             this.model.save_changes();
                         });
                         const updateState = () => {
                             console.log('kernel state changed, will set state to ', this.positionState);
                             plot.applyState(Object.assign(Object.assign({}, this.positionState), {
-                                ldrefvar: ""
+                                ldrefvar: ''
                             }));
                         };
                         // listen to changes of state in kernel and update view accordingly
                         this.model.on('change:position', updateState);
                         this.displayed.then(() => {
                             this.plot.rescaleSVG();
                         });
-                        //this.model.on('change:_associations_view', updateState);
                     }
                     get positionState() {
                         return this.model.get('position');
                     }
                 }
                 exports.LocusZoomView = LocusZoomView;
 
@@ -314,8 +402,8 @@
                 module.exports = JSON.parse('{"name":"jupyter-locuszoom","version":"0.1.0","description":"Jupyter Widget for LocusZoom","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/krassowski/jupyter-locuszoom","bugs":{"url":"https://github.com/krassowski/jupyter-locuszoom/issues"},"license":"BSD-3-Clause","author":{"name":"Michał Krassowski","email":"me@me.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/krassowski/jupyter-locuszoom"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf jupyter_locuszoom/labextension","clean:nbextension":"rimraf jupyter_locuszoom/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","locuszoom":"^0.14.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"jupyter_locuszoom/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.4dd25bf992348c7ee2aa.js.map
+//# sourceMappingURL=lib_widget_js.ff0b505f89816ef2fa6c.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.4dd25bf992348c7ee2aa.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/lib_widget_js.dc6697cf94dcc4cb14bc.js.map`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071428571428572%*

 * *Differences: {"'file'": "'lib_widget_js.dc6697cf94dcc4cb14bc.js'",*

 * * "'mappings'": "';;;;;;;;AAAA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,0CAA0C,oCAAoC,qBAAqB,GAAG;AACtG;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACNA,SAAe,KAAK,CAAC,OAAe;;QAClC,OAAO,IAAI,OAAO,CAAO,CAAC,OAAO,EAAE,EAAE;YACnC,UAAU,CAAC,GAAG,EAAE;gBACd,OAAO,EAAE,CAAC;YACZ,CAAC,EAAE,OAAO,CAAC,CAAC;QACd,CAAC,CAAC,CAAC;IACL,CAAC;CAAA;AAED,SAAgB,UAAU,CACxB,OAAyB,EACzB,WAAW,GAAG,EAAE,EAChB,QAAQ,GAAG,EAAE,EACb,mBAAmB,CAAC,CAAS,EAAE,EAAE,CAAC,CAAC;IAEnC,OAAO,CAAC,GAAS,EAAE; […]*

```diff
@@ -1,19 +1,21 @@
 {
-    "file": "lib_widget_js.4dd25bf992348c7ee2aa.js",
-    "mappings": "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",
+    "file": "lib_widget_js.dc6697cf94dcc4cb14bc.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/./css/widget.css",
+        "webpack://jupyter-locuszoom/./src/utils.ts",
         "webpack://jupyter-locuszoom/./src/version.ts",
         "webpack://jupyter-locuszoom/./src/widget.ts",
         "webpack://jupyter-locuszoom/./css/widget.css?a195"
     ],
     "sourcesContent": [
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
+        "async function sleep(timeout: number): Promise<void> {\n  return new Promise<void>((resolve) => {\n    setTimeout(() => {\n      resolve();\n    }, timeout);\n  });\n}\n\nexport function untilReady(\n  isReady: CallableFunction,\n  maxRetrials = 20,\n  interval = 75,\n  intervalModifier = (i: number) => i\n): Promise<CallableFunction> {\n  return (async () => {\n    let i = 0;\n    while (isReady() !== true) {\n      i += 1;\n      if (maxRetrials !== -1 && i > maxRetrials) {\n        throw Error('Too many retrials');\n      }\n      interval = intervalModifier(interval);\n      await sleep(interval);\n    }\n    return isReady;\n  })();\n}\n",
         "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n//import { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chrom: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {}\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: {model: LocusZoomModel}) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    /**\n    console.log('performing request', options);\n    await untilReady(() => {\n      const position = this.model.get('position');\n      return (\n        position.chr === options.chr\n        &&\n        position.start === options.start\n        &&\n        position.end === options.end\n        )\n    })\n    console.log('got it!');\n    */\n    return{\n      data: this.model.get('_associations_view'),\n      lastPage: 100\n    };\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n   _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n       _super.call(this, msg);\n       switch (msg.type) {\n         case 'resize':\n           console.log('resize message')\n           window.requestAnimationFrame(() => this.plot.rescaleSVG());\n           break;\n       }\n  }\n  processPhosphorMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processPhosphorMessage);\n }\n\n processLuminoMessage(msg: Message): void {\n     this._processLuminoMessage(msg, super.processLuminoMessage);\n }\n  render() {\n    const apiBase = \"https://portaldev.sph.umich.edu/api/v1/\";\n    const build = this.model.get('build');\n\n    var dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add(\"assoc\", [\"ModelAssociation\", { model: this.model }])\n      .add(\"ld\", [\"LDServer\", { url: \"https://portaldev.sph.umich.edu/ld/\", source: '1000G', build, population: 'ALL' }])\n      .add(\"gene\", [\"GeneLZ\", { url: apiBase + \"annotation/genes/\", build }])\n      .add(\"recomb\", [\"RecombLZ\", { url: apiBase + \"annotation/recomb/results/\", build }])\n      .add(\"constraint\", [\"GeneConstraintLZ\", { url: \"https://gnomad.broadinstitute.org/api/\", build }]);\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get(\"plot\", \"standard_association\", {state: initialState});\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\"#\" + this.container.id, dataSources, layout);\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      console.log('state changed');\n      const position = this.model.get('position');\n      if (\n        plot.state.start == position.start\n        &&\n        plot.state.end == position.end\n        &&\n        plot.state.chr == position.chrom\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to',  plot.state)\n      this.model.set('position', {start: plot.state.start, end: plot.state.end, chr: plot.state.chr});\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log('kernel state changed, will set state to ', this.positionState);\n      plot.applyState({ ...this.positionState, ldrefvar: \"\" });\n    }\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n    //this.model.on('change:_associations_view', updateState);\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
+        "// Copyright (c) Micha\u0142 Krassowski\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n} from '@jupyter-widgets/base';\nimport { UUID } from '@lumino/coreutils';\nimport { Message } from '@lumino/messaging';\n\nimport LocusZoom from 'locuszoom';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\nimport { untilReady } from './utils';\n\n// Import the CSS\nimport 'locuszoom/dist/locuszoom.css';\nimport '../css/widget.css';\n\nexport class LocusZoomModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: LocusZoomModel.model_name,\n      _model_module: LocusZoomModel.model_module,\n      _model_module_version: LocusZoomModel.model_module_version,\n      _view_name: LocusZoomModel.view_name,\n      _view_module: LocusZoomModel.view_module,\n      _view_module_version: LocusZoomModel.view_module_version,\n      build: 'GRCh38',\n      position: {\n        chr: '1',\n        start: 0,\n        end: 5000000,\n      },\n      _associations_view: {\n        range: {\n          chr: '1',\n          start: 0,\n          end: 5000000,\n        }\n      },\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // Add any extra serializers here\n  };\n\n  static model_name = 'LocusZoomModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'LocusZoomView'; // Set to null if no view\n  static view_module = MODULE_NAME; // Set to null if no view\n  static view_module_version = MODULE_VERSION;\n}\n\ninterface IRequestOptions {\n  chr: string;\n  start: number;\n  end: number;\n}\n\nconst AssociationLZ = LocusZoom.Adapters.get('AssociationLZ');\n\nclass ModelAssociation extends AssociationLZ {\n  model: LocusZoomModel;\n  constructor(config: { model: LocusZoomModel }) {\n    super({});\n    this.model = config.model;\n  }\n\n  async _performRequest(options: IRequestOptions) {\n    // TODO: find a way to fetch view properly\n    await untilReady(() => {\n      const view = this.model.get('_associations_view');\n      const position = view.range;\n      console.log(position, options, (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      ))\n      return (\n        position.chr === options.chr &&\n        position.start === options.start &&\n        position.end === options.end\n      );\n    });\n    return this.model.get('_associations_view');\n  }\n}\n// A custom adapter should be added to the registry before using it\nLocusZoom.Adapters.add('ModelAssociation', ModelAssociation);\n\nexport class LocusZoomView extends DOMWidgetView {\n  container: HTMLDivElement;\n  plot: any;\n  constructor(options: any) {\n    super(options);\n    this.container = document.createElement('div');\n    this.container.id = 'locus-zoom-' + UUID.uuid4();\n    this.el.appendChild(this.container);\n  }\n  _processLuminoMessage(msg: Message, _super: (msg: Message) => void): void {\n    _super.call(this, msg);\n    switch (msg.type) {\n      case 'resize':\n        console.log('resize message');\n        window.requestAnimationFrame(() => this.plot.rescaleSVG());\n        break;\n    }\n  }\n  processPhosphorMessage(msg: Message): void {\n    // eslint-disable-next-line @typescript-eslint/ban-ts-comment\n    // @ts-ignore\n    this._processLuminoMessage(msg, super.processPhosphorMessage);\n  }\n\n  processLuminoMessage(msg: Message): void {\n    this._processLuminoMessage(msg, super.processLuminoMessage);\n  }\n  render() {\n    const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';\n    const build = this.model.get('build');\n\n    const dataSources = new LocusZoom.DataSources();\n    dataSources\n      .add('assoc', ['ModelAssociation', { model: this.model }])\n      .add('ld', [\n        'LDServer',\n        {\n          url: 'https://portaldev.sph.umich.edu/ld/',\n          source: '1000G',\n          build,\n          population: 'ALL',\n        },\n      ])\n      .add('gene', ['GeneLZ', { url: apiBase + 'annotation/genes/', build }])\n      .add('recomb', [\n        'RecombLZ',\n        { url: apiBase + 'annotation/recomb/results/', build },\n      ])\n      .add('constraint', [\n        'GeneConstraintLZ',\n        { url: 'https://gnomad.broadinstitute.org/api/', build },\n      ]);\n    // TODO:\n    //.add(\"phewas\", [\"PheWASLZ\", {url: \"https://portaldev.sph.umich.edu/\" + \"api/v1/statistic/phewas/\", build: [build]}])\n\n    const initialState = this.positionState;\n    console.log(initialState);\n    const layout = LocusZoom.Layouts.get('plot', 'standard_association', {\n      state: initialState,\n    });\n\n    // d3 assumes the node is already in the DOM and will fail if we do not attach it temporarily.\n    const attached = this.el.parentElement !== null;\n    if (!attached) {\n      document.body.appendChild(this.el);\n    }\n    const plot = LocusZoom.populate(\n      '#' + this.container.id,\n      dataSources,\n      layout\n    );\n    if (!attached) {\n      document.body.removeChild(this.el);\n    }\n    this.plot = plot;\n\n    plot.on('state_changed', () => {\n      const position = this.model.get('position');\n      if (\n        plot.state.start === position.start &&\n        plot.state.end === position.end &&\n        plot.state.chr === position.chr\n      ) {\n        return;\n      }\n      console.log('plot state changed, will set kernel state to', plot.state);\n      this.model.set('position', {\n        start: plot.state.start,\n        end: plot.state.end,\n        chr: plot.state.chr,\n      });\n      this.model.save_changes();\n    });\n\n    const updateState = () => {\n      console.log(\n        'kernel state changed, will set state to ',\n        this.positionState\n      );\n      plot.applyState({ ...this.positionState, ldrefvar: '' });\n    };\n\n    // listen to changes of state in kernel and update view accordingly\n    this.model.on('change:position', updateState);\n    this.displayed.then(() => {\n      this.plot.rescaleSVG();\n    });\n  }\n\n  get positionState() {\n    return this.model.get('position');\n  }\n}\n",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};"
     ],
     "version": 3
 }
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.1629023844841c0a9ae9.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.35a953c4bbbdf71b3939.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.35a953c4bbbdf71b3939.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_locuszoom_dist_locuszoom_css":"ece39b50ae745565006a","lib_widget_js":"ff0b505f89816ef2fa6c","lib_index_js":"1462f2843f4c04a52881","lib_plugin_js":"7e633c5 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.1629023844841c0a9ae9.js",
+    "file": "remoteEntry.35a953c4bbbdf71b3939.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oQAAoQ;WAClS;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/webpack/container-entry",
         "webpack://jupyter-locuszoom/webpack/bootstrap",
         "webpack://jupyter-locuszoom/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"4dd25bf992348c7ee2aa\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"ff0b505f89816ef2fa6c\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-locuszoom:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter-locuszoom\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-locuszoom\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"locuszoom\", \"0.14.0\", () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/locuszoom/esm/index.js */ \"./node_modules/locuszoom/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.1aa611838b67c7e01bd2.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.03af74c81e37b8d85832.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -180,15 +180,15 @@
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
                 "vendors-node_modules_locuszoom_dist_locuszoom_css": "ece39b50ae745565006a",
-                "lib_widget_js": "eadf6ecf6ca0ff8a0a10",
+                "lib_widget_js": "b631ee8a6ff24aede47c",
                 "lib_index_js": "1462f2843f4c04a52881",
                 "lib_plugin_js": "7e633c522b2189389736",
                 "vendors-node_modules_locuszoom_esm_index_js": "5de6f7d98777bdb8af3e"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -1088,8 +1088,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyter-locuszoom");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyter-locuszoom"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.1aa611838b67c7e01bd2.js.map
+//# sourceMappingURL=remoteEntry.03af74c81e37b8d85832.js.map
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.1aa611838b67c7e01bd2.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.e1d041ac7fb699acd6d5.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.e1d041ac7fb699acd6d5.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_locuszoom_dist_locuszoom_css":"ece39b50ae745565006a","lib_widget_js":"751b11392fdca570e288","lib_index_js":"1462f2843f4c04a52881","lib_plugin_js":"7e633c5 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.1aa611838b67c7e01bd2.js",
+    "file": "remoteEntry.e1d041ac7fb699acd6d5.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oQAAoQ;WAClS;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/webpack/container-entry",
         "webpack://jupyter-locuszoom/webpack/bootstrap",
         "webpack://jupyter-locuszoom/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"eadf6ecf6ca0ff8a0a10\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"751b11392fdca570e288\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-locuszoom:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter-locuszoom\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-locuszoom\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"locuszoom\", \"0.14.0\", () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/locuszoom/esm/index.js */ \"./node_modules/locuszoom/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.20eb474b851c8a21381e.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.e681d2c3e869ee437176.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.e681d2c3e869ee437176.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_locuszoom_dist_locuszoom_css":"ece39b50ae745565006a","lib_widget_js":"ff612b296119c6362583","lib_index_js":"1462f2843f4c04a52881","lib_plugin_js":"7e633c5 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.20eb474b851c8a21381e.js",
+    "file": "remoteEntry.e681d2c3e869ee437176.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oQAAoQ;WAClS;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/webpack/container-entry",
         "webpack://jupyter-locuszoom/webpack/bootstrap",
         "webpack://jupyter-locuszoom/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"19c75a6eec62583a7167\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"ff612b296119c6362583\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-locuszoom:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter-locuszoom\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-locuszoom\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"locuszoom\", \"0.14.0\", () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/locuszoom/esm/index.js */ \"./node_modules/locuszoom/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.2a585e92942f2727413c.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.844efee5a11f0506b968.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.844efee5a11f0506b968.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_locuszoom_dist_locuszoom_css":"ece39b50ae745565006a","lib_widget_js":"dc6697cf94dcc4cb14bc","lib_index_js":"1462f2843f4c04a52881","lib_plugin_js":"7e633c5 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.2a585e92942f2727413c.js",
+    "file": "remoteEntry.844efee5a11f0506b968.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oQAAoQ;WAClS;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/webpack/container-entry",
         "webpack://jupyter-locuszoom/webpack/bootstrap",
         "webpack://jupyter-locuszoom/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"de2f37af2c0d8baa33d7\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"dc6697cf94dcc4cb14bc\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-locuszoom:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter-locuszoom\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-locuszoom\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"locuszoom\", \"0.14.0\", () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/locuszoom/esm/index.js */ \"./node_modules/locuszoom/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.3005a39789aa770403fd.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.03af74c81e37b8d85832.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.03af74c81e37b8d85832.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_locuszoom_dist_locuszoom_css":"ece39b50ae745565006a","lib_widget_js":"b631ee8a6ff24aede47c","lib_index_js":"1462f2843f4c04a52881","lib_plugin_js":"7e633c5 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.3005a39789aa770403fd.js",
+    "file": "remoteEntry.03af74c81e37b8d85832.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oQAAoQ;WAClS;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/webpack/container-entry",
         "webpack://jupyter-locuszoom/webpack/bootstrap",
         "webpack://jupyter-locuszoom/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"9b2c61bbd001346eef96\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"b631ee8a6ff24aede47c\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-locuszoom:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter-locuszoom\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-locuszoom\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"locuszoom\", \"0.14.0\", () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/locuszoom/esm/index.js */ \"./node_modules/locuszoom/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.32b5350f76df71fc343e.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.32f59f51d40bf5ffa01e.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.32f59f51d40bf5ffa01e.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_locuszoom_dist_locuszoom_css":"ece39b50ae745565006a","lib_widget_js":"d278f1d07325a0e4e5cb","lib_index_js":"1462f2843f4c04a52881","lib_plugin_js":"7e633c5 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.32b5350f76df71fc343e.js",
+    "file": "remoteEntry.32f59f51d40bf5ffa01e.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oQAAoQ;WAClS;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/webpack/container-entry",
         "webpack://jupyter-locuszoom/webpack/bootstrap",
         "webpack://jupyter-locuszoom/webpack/runtime/compat get default export",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"0623db0f7d3c07125290\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"d278f1d07325a0e4e5cb\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-locuszoom:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter-locuszoom\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-locuszoom\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"locuszoom\", \"0.14.0\", () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/locuszoom/esm/index.js */ \"./node_modules/locuszoom/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyter-locuszoom\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyter_locuszoom\"] = self[\"webpackChunkjupyter_locuszoom\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyter-locuszoom\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/remoteEntry.38f37b6bb3476b64bbf7.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/remoteEntry.76e640dbe79737ef23c4.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.76e640dbe79737ef23c4.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_locuszoom_dist_locuszoom_css":"ece39b50ae745565006a","lib_widget_js":"e00d9776199cdb3b0918","lib_index_js":"1462f2843f4c04a52881","lib_plugin_js":"7e633c5 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.38f37b6bb3476b64bbf7.js",
+    "file": "remoteEntry.76e640dbe79737ef23c4.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oQAAoQ;WAClS;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-locuszoom/webpack/container-entry",
         "webpack://jupyter-locuszoom/webpack/bootstrap",
         "webpack://jupyter-locuszoom/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"1de32fa6eec660baca88\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_locuszoom_dist_locuszoom_css\":\"ece39b50ae745565006a\",\"lib_widget_js\":\"e00d9776199cdb3b0918\",\"lib_index_js\":\"1462f2843f4c04a52881\",\"lib_plugin_js\":\"7e633c522b2189389736\",\"vendors-node_modules_locuszoom_esm_index_js\":\"5de6f7d98777bdb8af3e\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-locuszoom:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter-locuszoom\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-locuszoom\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_locuszoom_dist_locuszoom_css\"), __webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"locuszoom\", \"0.14.0\", () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/locuszoom/esm/index.js */ \"./node_modules/locuszoom/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/locuszoom/locuszoom\": () => (loadStrictVersionCheckFallback(\"default\", \"locuszoom\", [2,0,14,0], () => (__webpack_require__.e(\"vendors-node_modules_locuszoom_esm_index_js\").then(() => (() => (__webpack_require__(/*! locuszoom */ \"./node_modules/locuszoom/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/locuszoom/locuszoom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_dist_locuszoom_css.ece39b50ae745565006a.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js.map` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/labextension/static/vendors-node_modules_locuszoom_esm_index_js.5de6f7d98777bdb8af3e.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/jupyter_locuszoom/tests/conftest.py` & `jupyter_locuszoom-0.1.1.dev0/jupyter_locuszoom/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/src/extension.ts` & `jupyter_locuszoom-0.1.1.dev0/src/extension.ts`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/src/locuszoom.d.ts` & `jupyter_locuszoom-0.1.1.dev0/src/locuszoom.d.ts`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/src/plugin.ts` & `jupyter_locuszoom-0.1.1.dev0/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/src/utils.ts` & `jupyter_locuszoom-0.1.1.dev0/src/utils.ts`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
       resolve();
     }, timeout);
   });
 }
 
 export function untilReady(
   isReady: CallableFunction,
-  maxRetrials = 35,
-  interval = 50,
+  maxRetrials = 15,
+  interval = 75,
   intervalModifier = (i: number) => i
 ): Promise<CallableFunction> {
   return (async () => {
     let i = 0;
     while (isReady() !== true) {
       i += 1;
       if (maxRetrials !== -1 && i > maxRetrials) {
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/src/version.ts` & `jupyter_locuszoom-0.1.1.dev0/src/version.ts`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/src/widget.ts` & `jupyter_locuszoom-0.1.1.dev0/src/widget.ts`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 } from '@jupyter-widgets/base';
 import { UUID } from '@lumino/coreutils';
 import { Message } from '@lumino/messaging';
 
 import LocusZoom from 'locuszoom';
 
 import { MODULE_NAME, MODULE_VERSION } from './version';
-//import { untilReady } from './utils';
+import { untilReady } from './utils';
 
 // Import the CSS
 import 'locuszoom/dist/locuszoom.css';
 import '../css/widget.css';
 
 export class LocusZoomModel extends DOMWidgetModel {
   defaults() {
@@ -30,15 +30,21 @@
       _view_module_version: LocusZoomModel.view_module_version,
       build: 'GRCh38',
       position: {
         chr: '1',
         start: 0,
         end: 5000000,
       },
-      _associations_view: {},
+      _associations_view: {
+        range: {
+          chr: '1',
+          start: 0,
+          end: 5000000,
+        },
+      },
     };
   }
 
   static serializers: ISerializers = {
     ...DOMWidgetModel.serializers,
     // Add any extra serializers here
   };
@@ -64,32 +70,24 @@
   constructor(config: { model: LocusZoomModel }) {
     super({});
     this.model = config.model;
   }
 
   async _performRequest(options: IRequestOptions) {
     // TODO: find a way to fetch view properly
-    /**
-    console.log('performing request', options);
     await untilReady(() => {
-      const position = this.model.get('position');
+      const view = this.model.get('_associations_view');
+      const position = view.range;
       return (
-        position.chr === options.chr
-        &&
-        position.start === options.start
-        &&
+        position.chr === options.chr &&
+        position.start === options.start &&
         position.end === options.end
-        )
-    })
-    console.log('got it!');
-    */
-    return {
-      data: this.model.get('_associations_view'),
-      lastPage: 100,
-    };
+      );
+    });
+    return this.model.get('_associations_view');
   }
 }
 // A custom adapter should be added to the registry before using it
 LocusZoom.Adapters.add('ModelAssociation', ModelAssociation);
 
 export class LocusZoomView extends DOMWidgetView {
   container: HTMLDivElement;
@@ -106,15 +104,17 @@
       case 'resize':
         console.log('resize message');
         window.requestAnimationFrame(() => this.plot.rescaleSVG());
         break;
     }
   }
   processPhosphorMessage(msg: Message): void {
-    this._processLuminoMessage(msg, super.processLuminoMessage);
+    // eslint-disable-next-line @typescript-eslint/ban-ts-comment
+    // @ts-ignore
+    this._processLuminoMessage(msg, super.processPhosphorMessage);
   }
 
   processLuminoMessage(msg: Message): void {
     this._processLuminoMessage(msg, super.processLuminoMessage);
   }
   render() {
     const apiBase = 'https://portaldev.sph.umich.edu/api/v1/';
@@ -162,15 +162,14 @@
     );
     if (!attached) {
       document.body.removeChild(this.el);
     }
     this.plot = plot;
 
     plot.on('state_changed', () => {
-      console.log('state changed');
       const position = this.model.get('position');
       if (
         plot.state.start === position.start &&
         plot.state.end === position.end &&
         plot.state.chr === position.chr
       ) {
         return;
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/src/__tests__/utils.ts` & `jupyter_locuszoom-0.1.1.dev0/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/.gitignore` & `jupyter_locuszoom-0.1.1.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/LICENSE.txt` & `jupyter_locuszoom-0.1.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_locuszoom-0.1.0.dev0/README.md` & `jupyter_locuszoom-0.1.1.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     chrom='15',    # optional (if not given top locus will be shown)
     start=0,       # optional (if nto given top locus on given chromosome will be shown)
     end=100_000,   # optional, but has to be given if start was given
     build='GRCh38'
 )
 ```
 
-![Screenshot from 2023-06-29 15-30-43](https://github.com/krassowski/jupyter-locuszoom/assets/5832902/42fb1adf-825e-4afb-a915-f0efbfaf4d10)
+![Example](https://github.com/krassowski/jupyter-locuszoom/assets/5832902/f7ee35fc-7024-477c-b411-c28670eed8cc)
 
 Alternatively, center on a specific position:
 
 ```python
 LocusZoom(
     assoc,
     chrom='15',
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/pyproject.toml` & `jupyter_locuszoom-0.1.1.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
 ]
-version = "0.1.0.dev0"
+version = "0.1.1.dev0"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `jupyter_locuszoom-0.1.0.dev0/PKG-INFO` & `jupyter_locuszoom-0.1.1.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-locuszoom
-Version: 0.1.0.dev0
+Version: 0.1.1.dev0
 Summary: Jupyter Widget for LocusZoom
 Project-URL: Homepage, https://github.com/krassowski/jupyter-locuszoom
 Author: Michał Krassowski
 License: Copyright (c) 2023 Michał Krassowski
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -88,15 +88,15 @@
     chrom='15',    # optional (if not given top locus will be shown)
     start=0,       # optional (if nto given top locus on given chromosome will be shown)
     end=100_000,   # optional, but has to be given if start was given
     build='GRCh38'
 )
 ```
 
-![Screenshot from 2023-06-29 15-30-43](https://github.com/krassowski/jupyter-locuszoom/assets/5832902/42fb1adf-825e-4afb-a915-f0efbfaf4d10)
+![Example](https://github.com/krassowski/jupyter-locuszoom/assets/5832902/f7ee35fc-7024-477c-b411-c28670eed8cc)
 
 Alternatively, center on a specific position:
 
 ```python
 LocusZoom(
     assoc,
     chrom='15',
```

