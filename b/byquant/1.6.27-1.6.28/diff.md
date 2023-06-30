# Comparing `tmp/byquant-1.6.27.tar.gz` & `tmp/byquant-1.6.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.6.27.tar", last modified: Tue Jun 27 01:32:07 2023, max compression
+gzip compressed data, was "byquant-1.6.28.tar", last modified: Fri Jun 30 01:06:17 2023, max compression
```

## Comparing `byquant-1.6.27.tar` & `byquant-1.6.28.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.539946 byquant-1.6.27/
--rw-rw-rw-   0        0        0     1328 2023-06-27 01:32:07.539946 byquant-1.6.27/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.6.27/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.038142 byquant-1.6.27/byquant/
--rw-rw-rw-   0        0        0    21860 2023-06-25 06:21:22.000000 byquant-1.6.27/byquant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.069376 byquant-1.6.27/byquant/crypto/
--rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.6.27/byquant/crypto/__init__.py
--rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.6.27/byquant/crypto/broker.py
--rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.6.27/byquant/crypto/feed.py
--rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.6.27/byquant/crypto/store.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.538914 byquant-1.6.27/byquant/exchange/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.6.27/byquant/exchange/__init__.py
--rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.6.27/byquant/exchange/ace.py
--rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/alpaca.py
--rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/ascendex.py
--rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bequant.py
--rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bigone.py
--rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binance.py
--rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binancecoinm.py
--rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binanceus.py
--rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binanceusdm.py
--rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bit2c.py
--rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitbank.py
--rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitbay.py
--rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitbns.py
--rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitcoincom.py
--rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitfinex.py
--rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitfinex2.py
--rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitflyer.py
--rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitforex.py
--rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitget.py
--rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bithumb.py
--rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitmart.py
--rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitmex.py
--rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitopro.py
--rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitpanda.py
--rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitrue.py
--rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitso.py
--rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitstamp.py
--rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitstamp1.py
--rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bittrex.py
--rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitvavo.py
--rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bkex.py
--rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bl3p.py
--rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/blockchaincom.py
--rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcalpha.py
--rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcbox.py
--rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcex.py
--rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcmarkets.py
--rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btctradeua.py
--rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcturk.py
--rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/buda.py
--rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bybit.py
--rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/cex.py
--rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinbase.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinbaseprime.py
--rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinbasepro.py
--rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coincheck.py
--rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinex.py
--rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinfalcon.py
--rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinmate.py
--rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinone.py
--rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinsph.py
--rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinspot.py
--rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/cryptocom.py
--rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/currencycom.py
--rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/delta.py
--rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/deribit.py
--rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/digifinex.py
--rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/exmo.py
--rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/flowbtc.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/fmfwio.py
--rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/gate.py
--rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/gateio.py
--rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/gemini.py
--rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/hitbtc.py
--rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/hitbtc3.py
--rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/hollaex.py
--rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/huobi.py
--rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/huobijp.py
--rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/huobipro.py
--rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/idex.py
--rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/independentreserve.py
--rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/indodax.py
--rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/itbit.py
--rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kraken.py
--rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/krakenfutures.py
--rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kucoin.py
--rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kucoinfutures.py
--rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kuna.py
--rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/latoken.py
--rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/lbank.py
--rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/lbank2.py
--rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/luno.py
--rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/lykke.py
--rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/mercado.py
--rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/mexc.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/mexc3.py
--rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/ndax.py
--rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/novadax.py
--rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/oceanex.py
--rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/okcoin.py
--rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/okex.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/okex5.py
--rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.6.27/byquant/exchange/okx.py
--rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/paymium.py
--rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/phemex.py
--rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/poloniex.py
--rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/poloniexfutures.py
--rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/probit.py
--rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/ripio.py
--rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/stex.py
--rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/tidex.py
--rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/timex.py
--rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/tokocrypto.py
--rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/upbit.py
--rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/wavesexchange.py
--rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/wazirx.py
--rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/whitebit.py
--rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/woo.py
--rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/xt.py
--rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/yobit.py
--rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/zaif.py
--rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/zb.py
--rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/zonda.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.539946 byquant-1.6.27/byquant/tool/
--rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.6.27/byquant/tool/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.6.27/byquant/tool/tawPlus.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.069376 byquant-1.6.27/byquant.egg-info/
--rw-rw-rw-   0        0        0     1328 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3561 2023-06-27 01:32:07.000000 byquant-1.6.27/byquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.6.27/byquant.egg-info/zip-safe
--rw-rw-rw-   0        0        0      125 2023-06-27 01:29:04.000000 byquant-1.6.27/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 01:32:07.539946 byquant-1.6.27/setup.cfg
--rw-rw-rw-   0        0        0     2760 2023-06-27 01:28:02.000000 byquant-1.6.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:06:17.017108 byquant-1.6.28/
+-rw-rw-rw-   0        0        0     1328 2023-06-30 01:06:17.013118 byquant-1.6.28/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.6.28/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 01:06:16.354193 byquant-1.6.28/byquant/
+-rw-rw-rw-   0        0        0    21860 2023-06-25 06:21:22.000000 byquant-1.6.28/byquant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:06:16.403062 byquant-1.6.28/byquant/crypto/
+-rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.6.28/byquant/crypto/__init__.py
+-rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.6.28/byquant/crypto/broker.py
+-rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.6.28/byquant/crypto/feed.py
+-rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.6.28/byquant/crypto/store.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:06:17.002148 byquant-1.6.28/byquant/exchange/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.6.28/byquant/exchange/__init__.py
+-rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.6.28/byquant/exchange/ace.py
+-rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/alpaca.py
+-rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/ascendex.py
+-rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bequant.py
+-rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bigone.py
+-rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/binance.py
+-rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/binancecoinm.py
+-rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/binanceusdm.py
+-rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bit2c.py
+-rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitbank.py
+-rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitbay.py
+-rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitbns.py
+-rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitcoincom.py
+-rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitfinex.py
+-rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitfinex2.py
+-rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitflyer.py
+-rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitforex.py
+-rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitget.py
+-rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bithumb.py
+-rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitmart.py
+-rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitmex.py
+-rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitopro.py
+-rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitpanda.py
+-rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitrue.py
+-rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitso.py
+-rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitstamp.py
+-rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitstamp1.py
+-rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bittrex.py
+-rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bitvavo.py
+-rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bkex.py
+-rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bl3p.py
+-rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/blockchaincom.py
+-rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/btcalpha.py
+-rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/btcbox.py
+-rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/btcex.py
+-rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/btcmarkets.py
+-rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/btctradeua.py
+-rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/btcturk.py
+-rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/buda.py
+-rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/bybit.py
+-rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/cex.py
+-rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinbase.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinbaseprime.py
+-rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinbasepro.py
+-rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coincheck.py
+-rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinex.py
+-rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinfalcon.py
+-rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinmate.py
+-rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinone.py
+-rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinsph.py
+-rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/coinspot.py
+-rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/cryptocom.py
+-rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/currencycom.py
+-rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/delta.py
+-rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/deribit.py
+-rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/digifinex.py
+-rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/exmo.py
+-rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/flowbtc.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/fmfwio.py
+-rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/gate.py
+-rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/gateio.py
+-rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/gemini.py
+-rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/hitbtc.py
+-rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/hitbtc3.py
+-rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/hollaex.py
+-rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/huobi.py
+-rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/huobijp.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/huobipro.py
+-rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/idex.py
+-rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/independentreserve.py
+-rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/indodax.py
+-rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/itbit.py
+-rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/kraken.py
+-rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/krakenfutures.py
+-rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/kucoin.py
+-rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/kucoinfutures.py
+-rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/kuna.py
+-rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/latoken.py
+-rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/lbank.py
+-rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/lbank2.py
+-rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/luno.py
+-rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/lykke.py
+-rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/mercado.py
+-rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/mexc.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/mexc3.py
+-rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/ndax.py
+-rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/novadax.py
+-rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/oceanex.py
+-rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/okcoin.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/okex.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/okex5.py
+-rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.6.28/byquant/exchange/okx.py
+-rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/paymium.py
+-rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/phemex.py
+-rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/poloniex.py
+-rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/poloniexfutures.py
+-rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/probit.py
+-rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/ripio.py
+-rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/stex.py
+-rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/tidex.py
+-rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/timex.py
+-rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/tokocrypto.py
+-rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/upbit.py
+-rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/wavesexchange.py
+-rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/wazirx.py
+-rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/whitebit.py
+-rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/woo.py
+-rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/xt.py
+-rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/yobit.py
+-rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/zaif.py
+-rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/zb.py
+-rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.6.28/byquant/exchange/zonda.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:06:17.009129 byquant-1.6.28/byquant/tool/
+-rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.6.28/byquant/tool/__init__.py
+-rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.6.28/byquant/tool/tawPlus.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:06:16.384117 byquant-1.6.28/byquant.egg-info/
+-rw-rw-rw-   0        0        0     1328 2023-06-30 01:06:16.000000 byquant-1.6.28/byquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3561 2023-06-30 01:06:16.000000 byquant-1.6.28/byquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 01:06:16.000000 byquant-1.6.28/byquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-30 01:06:16.000000 byquant-1.6.28/byquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 01:06:16.000000 byquant-1.6.28/byquant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.6.28/byquant.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      156 2023-06-30 01:04:00.000000 byquant-1.6.28/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 01:06:17.017108 byquant-1.6.28/setup.cfg
+-rw-rw-rw-   0        0        0     2760 2023-06-30 01:03:16.000000 byquant-1.6.28/setup.py
```

### Comparing `byquant-1.6.27/PKG-INFO` & `byquant-1.6.28/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.6.27
+Version: 1.6.28
 Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.6.27/byquant/__init__.py` & `byquant-1.6.28/byquant/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/crypto/broker.py` & `byquant-1.6.28/byquant/crypto/broker.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/crypto/feed.py` & `byquant-1.6.28/byquant/crypto/feed.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/crypto/store.py` & `byquant-1.6.28/byquant/crypto/store.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/ace.py` & `byquant-1.6.28/byquant/exchange/ace.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/alpaca.py` & `byquant-1.6.28/byquant/exchange/alpaca.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/ascendex.py` & `byquant-1.6.28/byquant/exchange/ascendex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bequant.py` & `byquant-1.6.28/byquant/exchange/bequant.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bigone.py` & `byquant-1.6.28/byquant/exchange/bigone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/binance.py` & `byquant-1.6.28/byquant/exchange/binance.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/binancecoinm.py` & `byquant-1.6.28/byquant/exchange/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/binanceus.py` & `byquant-1.6.28/byquant/exchange/binanceus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/binanceusdm.py` & `byquant-1.6.28/byquant/exchange/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bit2c.py` & `byquant-1.6.28/byquant/exchange/bit2c.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitbank.py` & `byquant-1.6.28/byquant/exchange/bitbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitbns.py` & `byquant-1.6.28/byquant/exchange/bitbns.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitfinex.py` & `byquant-1.6.28/byquant/exchange/bitfinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitfinex2.py` & `byquant-1.6.28/byquant/exchange/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitflyer.py` & `byquant-1.6.28/byquant/exchange/bitflyer.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitforex.py` & `byquant-1.6.28/byquant/exchange/bitforex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitget.py` & `byquant-1.6.28/byquant/exchange/bitget.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bithumb.py` & `byquant-1.6.28/byquant/exchange/bithumb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitmart.py` & `byquant-1.6.28/byquant/exchange/bitmart.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitmex.py` & `byquant-1.6.28/byquant/exchange/bitmex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitopro.py` & `byquant-1.6.28/byquant/exchange/bitopro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitpanda.py` & `byquant-1.6.28/byquant/exchange/bitpanda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitrue.py` & `byquant-1.6.28/byquant/exchange/bitrue.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitso.py` & `byquant-1.6.28/byquant/exchange/bitso.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitstamp.py` & `byquant-1.6.28/byquant/exchange/bitstamp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitstamp1.py` & `byquant-1.6.28/byquant/exchange/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bittrex.py` & `byquant-1.6.28/byquant/exchange/bittrex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bitvavo.py` & `byquant-1.6.28/byquant/exchange/bitvavo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bkex.py` & `byquant-1.6.28/byquant/exchange/bkex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bl3p.py` & `byquant-1.6.28/byquant/exchange/bl3p.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/blockchaincom.py` & `byquant-1.6.28/byquant/exchange/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/btcalpha.py` & `byquant-1.6.28/byquant/exchange/btcalpha.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/btcbox.py` & `byquant-1.6.28/byquant/exchange/btcbox.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/btcex.py` & `byquant-1.6.28/byquant/exchange/btcex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/btcmarkets.py` & `byquant-1.6.28/byquant/exchange/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/btctradeua.py` & `byquant-1.6.28/byquant/exchange/btctradeua.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/btcturk.py` & `byquant-1.6.28/byquant/exchange/btcturk.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/buda.py` & `byquant-1.6.28/byquant/exchange/buda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/bybit.py` & `byquant-1.6.28/byquant/exchange/bybit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/cex.py` & `byquant-1.6.28/byquant/exchange/cex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinbase.py` & `byquant-1.6.28/byquant/exchange/coinbase.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinbaseprime.py` & `byquant-1.6.28/byquant/exchange/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinbasepro.py` & `byquant-1.6.28/byquant/exchange/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coincheck.py` & `byquant-1.6.28/byquant/exchange/coincheck.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinex.py` & `byquant-1.6.28/byquant/exchange/coinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinfalcon.py` & `byquant-1.6.28/byquant/exchange/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinmate.py` & `byquant-1.6.28/byquant/exchange/coinmate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinone.py` & `byquant-1.6.28/byquant/exchange/coinone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinsph.py` & `byquant-1.6.28/byquant/exchange/coinsph.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/coinspot.py` & `byquant-1.6.28/byquant/exchange/coinspot.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/cryptocom.py` & `byquant-1.6.28/byquant/exchange/cryptocom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/currencycom.py` & `byquant-1.6.28/byquant/exchange/currencycom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/delta.py` & `byquant-1.6.28/byquant/exchange/delta.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/deribit.py` & `byquant-1.6.28/byquant/exchange/deribit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/digifinex.py` & `byquant-1.6.28/byquant/exchange/digifinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/exmo.py` & `byquant-1.6.28/byquant/exchange/exmo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/flowbtc.py` & `byquant-1.6.28/byquant/exchange/flowbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/fmfwio.py` & `byquant-1.6.28/byquant/exchange/fmfwio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/gate.py` & `byquant-1.6.28/byquant/exchange/gate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/gemini.py` & `byquant-1.6.28/byquant/exchange/gemini.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/hitbtc.py` & `byquant-1.6.28/byquant/exchange/hitbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/hitbtc3.py` & `byquant-1.6.28/byquant/exchange/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/hollaex.py` & `byquant-1.6.28/byquant/exchange/hollaex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/huobi.py` & `byquant-1.6.28/byquant/exchange/huobi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/huobijp.py` & `byquant-1.6.28/byquant/exchange/huobijp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/huobipro.py` & `byquant-1.6.28/byquant/exchange/huobipro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/idex.py` & `byquant-1.6.28/byquant/exchange/idex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/independentreserve.py` & `byquant-1.6.28/byquant/exchange/independentreserve.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/indodax.py` & `byquant-1.6.28/byquant/exchange/indodax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/itbit.py` & `byquant-1.6.28/byquant/exchange/itbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/kraken.py` & `byquant-1.6.28/byquant/exchange/kraken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/krakenfutures.py` & `byquant-1.6.28/byquant/exchange/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/kucoin.py` & `byquant-1.6.28/byquant/exchange/kucoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/kucoinfutures.py` & `byquant-1.6.28/byquant/exchange/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/kuna.py` & `byquant-1.6.28/byquant/exchange/kuna.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/latoken.py` & `byquant-1.6.28/byquant/exchange/latoken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/lbank.py` & `byquant-1.6.28/byquant/exchange/lbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/lbank2.py` & `byquant-1.6.28/byquant/exchange/lbank2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/luno.py` & `byquant-1.6.28/byquant/exchange/luno.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/lykke.py` & `byquant-1.6.28/byquant/exchange/lykke.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/mercado.py` & `byquant-1.6.28/byquant/exchange/mercado.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/mexc.py` & `byquant-1.6.28/byquant/exchange/mexc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/ndax.py` & `byquant-1.6.28/byquant/exchange/ndax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/novadax.py` & `byquant-1.6.28/byquant/exchange/novadax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/oceanex.py` & `byquant-1.6.28/byquant/exchange/oceanex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/okcoin.py` & `byquant-1.6.28/byquant/exchange/okcoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/okx.py` & `byquant-1.6.28/byquant/exchange/okx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/paymium.py` & `byquant-1.6.28/byquant/exchange/paymium.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/phemex.py` & `byquant-1.6.28/byquant/exchange/phemex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/poloniex.py` & `byquant-1.6.28/byquant/exchange/poloniex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/poloniexfutures.py` & `byquant-1.6.28/byquant/exchange/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/probit.py` & `byquant-1.6.28/byquant/exchange/probit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/ripio.py` & `byquant-1.6.28/byquant/exchange/ripio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/stex.py` & `byquant-1.6.28/byquant/exchange/stex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/tidex.py` & `byquant-1.6.28/byquant/exchange/tidex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/timex.py` & `byquant-1.6.28/byquant/exchange/timex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/tokocrypto.py` & `byquant-1.6.28/byquant/exchange/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/upbit.py` & `byquant-1.6.28/byquant/exchange/upbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/wavesexchange.py` & `byquant-1.6.28/byquant/exchange/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/wazirx.py` & `byquant-1.6.28/byquant/exchange/wazirx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/whitebit.py` & `byquant-1.6.28/byquant/exchange/whitebit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/woo.py` & `byquant-1.6.28/byquant/exchange/woo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/xt.py` & `byquant-1.6.28/byquant/exchange/xt.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/yobit.py` & `byquant-1.6.28/byquant/exchange/yobit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/zaif.py` & `byquant-1.6.28/byquant/exchange/zaif.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/zb.py` & `byquant-1.6.28/byquant/exchange/zb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/exchange/zonda.py` & `byquant-1.6.28/byquant/exchange/zonda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant/tool/tawPlus.py` & `byquant-1.6.28/byquant/tool/tawPlus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/byquant.egg-info/PKG-INFO` & `byquant-1.6.28/byquant.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.6.27
+Version: 1.6.28
 Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.6.27/byquant.egg-info/SOURCES.txt` & `byquant-1.6.28/byquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byquant-1.6.27/setup.py` & `byquant-1.6.28/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 here = path.abspath(path.dirname(__file__))
 root = path.dirname(here)
 
 readme = path.join(here, 'README.md')
 package = {
   "name": "byquant",
-  "version": "1.6.27",
+  "version": "1.6.28",
   "description": "ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community",
   "type": "module",
   "readme": "README.md",
   "package_json": "package.json",
   "author": {
     "name": "Uakeey",
     "email": "uakee@outlook.com",
```

