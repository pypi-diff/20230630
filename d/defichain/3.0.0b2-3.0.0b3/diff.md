# Comparing `tmp/defichain-3.0.0b2.tar.gz` & `tmp/defichain-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defichain-3.0.0b2.tar", last modified: Wed Jun 14 18:19:06 2023, max compression
+gzip compressed data, was "defichain-3.0.0b3.tar", last modified: Fri Jun 30 10:39:22 2023, max compression
```

## Comparing `defichain-3.0.0b2.tar` & `defichain-3.0.0b3.tar`

### file list

```diff
@@ -1,207 +1,211 @@
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.093278 defichain-3.0.0b2/
--rw-rw-r--   0 executor  (1000) executor  (1000)     1066 2023-03-23 01:00:00.000000 defichain-3.0.0b2/LICENSE
--rw-rw-r--   0 executor  (1000) executor  (1000)      121 2022-12-10 21:33:06.000000 defichain-3.0.0b2/MANIFEST.in
--rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-06-14 18:19:06.093278 defichain-3.0.0b2/PKG-INFO
--rw-rw-r--   0 executor  (1000) executor  (1000)     2723 2022-12-10 21:33:06.000000 defichain-3.0.0b2/README.md
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain/
--rw-rw-r--   0 executor  (1000) executor  (1000)      406 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain/exceptions/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain/exceptions/hdwallet/
--rw-rw-r--   0 executor  (1000) executor  (1000)      427 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/hdwallet/DerivationError.py
--rw-rw-r--   0 executor  (1000) executor  (1000)       96 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/hdwallet/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/exceptions/http/
--rw-rw-r--   0 executor  (1000) executor  (1000)      199 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/BadMethod.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      249 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/BadRequest.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/Forbidden.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1978 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/HTTPStatusCode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      302 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/InternalServerError.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      240 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/NotFound.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3982 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/RPCErrorCode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      220 2023-05-13 11:11:51.000000 defichain-3.0.0b2/defichain/exceptions/http/ServiceUnavailable.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      306 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/Unauthorized.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/UnprocessableEntity.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      215 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/WrongParmeters.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      615 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/exceptions/transactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)      430 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      110 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/addresserror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/defitxerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      116 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/deserializeerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/inputerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      103 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/keyerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      114 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/notsupported.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      124 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/rawtransactionerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/tokenerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      112 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/txbuildererror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/verifyerror.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/hdwallet/
--rw-rw-r--   0 executor  (1000) executor  (1000)       93 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/hdwallet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2149 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/hdwallet/account.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3808 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/hdwallet/derivations.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1200 2023-05-31 20:38:49.000000 defichain-3.0.0b2/defichain/hdwallet/encryption.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10519 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/hdwallet/utils.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    55798 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/hdwallet/wallet.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/libs/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2222 2023-05-24 21:37:48.000000 defichain-3.0.0b2/defichain/libs/base58.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4356 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/libs/bech32.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14136 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/libs/ecc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5376 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/libs/ripemd160.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4660 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/logger.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/mnemonic/
--rw-rw-r--   0 executor  (1000) executor  (1000)       32 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10817 2023-03-14 21:50:04.000000 defichain-3.0.0b2/defichain/mnemonic/mnemonic.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.081278 defichain-3.0.0b2/defichain/mnemonic/wordlist/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_simplified.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_traditional.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    13116 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/english.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    16776 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/french.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    16033 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/italian.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    26423 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/japanese.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    37832 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/korean.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    13996 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/spanish.txt
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.081278 defichain-3.0.0b2/defichain/networks/
--rw-rw-r--   0 executor  (1000) executor  (1000)       84 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/networks/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4060 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/networks/networks.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.081278 defichain-3.0.0b2/defichain/node/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2990 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/node/RPCErrorHandler.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1081 2022-12-12 22:24:40.000000 defichain-3.0.0b2/defichain/node/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/node/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)    21262 2023-06-12 22:07:50.000000 defichain-3.0.0b2/defichain/node/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    53564 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/blockchain.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5563 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/control.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1843 2023-06-12 22:08:23.000000 defichain-3.0.0b2/defichain/node/modules/evm.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      856 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/generating.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14857 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/loan.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8435 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/masternodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    12054 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/mining.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    16833 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/network.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    12270 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    13718 2023-03-18 22:58:05.000000 defichain-3.0.0b2/defichain/node/modules/poolpair.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5632 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/proposals.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    40311 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/rawtransactions.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      144 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/spv.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2530 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/stats.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10291 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/tokens.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8691 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/util.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    15447 2023-04-24 23:36:41.000000 defichain-3.0.0b2/defichain/node/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    86413 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/wallet.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      848 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/zmq.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6967 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/node/node.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2680 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/node/rpc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4216 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/util.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/ocean/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2775 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/OceanErrorHandler.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      806 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2357 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/connection.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/ocean/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)     6077 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2458 2022-12-28 14:30:10.000000 defichain-3.0.0b2/defichain/ocean/modules/blocks.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2163 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/modules/consortium.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      641 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/fee.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5499 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/modules/governance.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6104 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/loan.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1464 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/masternodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2492 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     7224 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/poolpairs.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5362 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/prices.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1691 2023-02-14 10:46:13.000000 defichain-3.0.0b2/defichain/ocean/modules/rawTx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      697 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/rpc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2405 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/stats.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1588 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/tokens.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2360 2022-12-28 14:30:13.000000 defichain-3.0.0b2/defichain/ocean/modules/transactions.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2973 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/ocean.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/transactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/transactions/address/
--rw-rw-r--   0 executor  (1000) executor  (1000)      288 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/address/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4009 2023-04-29 17:23:24.000000 defichain-3.0.0b2/defichain/transactions/address/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2583 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/base58address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5750 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/baseaddress.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2317 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/bech32address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3828 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/p2pkh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2531 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/p2sh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3064 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/p2wpkh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1073 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/address/script.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/transactions/builder/
--rw-rw-r--   0 executor  (1000) executor  (1000)       33 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/builder/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/builder/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)      220 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2683 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3231 2023-05-31 20:59:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/data.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      963 2023-05-05 17:22:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/governance.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2228 2023-05-05 17:22:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/loans.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1541 2023-05-05 17:22:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/masternode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4685 2023-04-01 19:19:45.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/pool.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5305 2023-06-14 18:09:22.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/utxo.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:52:35.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6021 2023-06-14 18:09:22.000000 defichain-3.0.0b2/defichain/transactions/builder/rawtransactionbuilder.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     7025 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/builder/txbuilder.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/constants/
--rw-rw-r--   0 executor  (1000) executor  (1000)      440 2023-04-01 23:11:49.000000 defichain-3.0.0b2/defichain/transactions/constants/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      245 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:45:28.000000 defichain-3.0.0b2/defichain/transactions/constants/defitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      382 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/fees.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/constants/mainnet/
--rw-rw-r--   0 executor  (1000) executor  (1000)     8734 2023-04-29 16:23:23.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     9370 2023-03-26 16:27:39.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     5622 2023-03-26 16:27:39.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/LOAN_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     7346 2023-03-26 16:27:39.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/STANDARD_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-04-01 23:11:49.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3265 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/opcodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/rawtransactions.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/constants/testnet/
--rw-rw-r--   0 executor  (1000) executor  (1000)    18208 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/CUSTOM_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     1630 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)      598 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/LOAN_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     1623 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/STANDARD_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)      177 2023-04-01 23:11:49.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3321 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/tokens.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/defitx/
--rw-rw-r--   0 executor  (1000) executor  (1000)      300 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2010 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/builddefitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3173 2023-05-13 09:00:19.000000 defichain-3.0.0b2/defichain/transactions/defitx/defitx.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/defitx/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     9987 2023-05-13 09:19:42.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      672 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/basedefitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     7538 2023-04-13 22:18:28.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/baseinput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3779 2023-05-12 14:43:35.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/governance.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8707 2023-04-24 23:35:56.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/loans.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6082 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/masternode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      209 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    16975 2023-04-13 22:05:54.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/pool.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      204 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/token.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     9907 2023-04-29 16:23:24.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4808 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/keys.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/rawtransactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)      339 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      954 2023-06-12 21:35:44.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/fee.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1438 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/sign.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    21228 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/tx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4252 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/txbase.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14476 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/txinput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10971 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/txoutput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8572 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/witness.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/remotedata/
--rw-rw-r--   0 executor  (1000) executor  (1000)       89 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/remotedata/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1747 2023-04-30 09:04:11.000000 defichain-3.0.0b2/defichain/transactions/remotedata/node.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1332 2023-04-29 16:23:24.000000 defichain-3.0.0b2/defichain/transactions/remotedata/ocean.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1469 2023-05-01 20:06:53.000000 defichain-3.0.0b2/defichain/transactions/remotedata/remotedata.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.093278 defichain-3.0.0b2/defichain/transactions/utils/
--rw-rw-r--   0 executor  (1000) executor  (1000)      236 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/utils/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3970 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/utils/calculate.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2633 2023-06-12 21:37:02.000000 defichain-3.0.0b2/defichain/transactions/utils/converter.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3083 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/utils/token.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      987 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/utils/verify.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain.egg-info/
--rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/PKG-INFO
--rw-rw-r--   0 executor  (1000) executor  (1000)     7088 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/SOURCES.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/dependency_links.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       57 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/requires.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       10 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/top_level.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)      174 2022-12-10 21:33:06.000000 defichain-3.0.0b2/pyproject.toml
--rw-rw-r--   0 executor  (1000) executor  (1000)       56 2023-05-31 20:38:42.000000 defichain-3.0.0b2/requirements.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       38 2023-06-14 18:19:06.093278 defichain-3.0.0b2/setup.cfg
--rw-rw-r--   0 executor  (1000) executor  (1000)     2717 2023-06-12 22:06:26.000000 defichain-3.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.925680 defichain-3.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 10:39:12.000000 defichain-3.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 10:39:12.000000 defichain-3.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-30 10:39:22.925680 defichain-3.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-30 10:39:12.000000 defichain-3.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.905680 defichain-3.0.0b3/defichain/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.905680 defichain-3.0.0b3/defichain/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.905680 defichain-3.0.0b3/defichain/exceptions/hdwallet/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/hdwallet/DerivationError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/hdwallet/NetworkError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/hdwallet/WalletError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/hdwallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.909680 defichain-3.0.0b3/defichain/exceptions/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/BadMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/BadRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/Forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/HTTPStatusCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/InternalServerError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/NotFound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/RPCErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/ServiceUnavailable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/Unauthorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/UnprocessableEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/WrongParmeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.909680 defichain-3.0.0b3/defichain/exceptions/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/addresserror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/defitxerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/deserializeerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/inputerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/keyerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/notsupported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/rawtransactionerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/tokenerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/txbuildererror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/exceptions/transactions/verifyerror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.909680 defichain-3.0.0b3/defichain/hdwallet/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/hdwallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/hdwallet/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/hdwallet/derivations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/hdwallet/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/hdwallet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60000 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/hdwallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.909680 defichain-3.0.0b3/defichain/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/libs/base58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/libs/bech32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/libs/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/libs/ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.909680 defichain-3.0.0b3/defichain/mnemonic/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/mnemonic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.913680 defichain-3.0.0b3/defichain/mnemonic/wordlist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/chinese_simplified.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/chinese_traditional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/english.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/french.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/italian.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26423 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/japanese.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37832 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/korean.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/mnemonic/wordlist/spanish.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.913680 defichain-3.0.0b3/defichain/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/networks/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.913680 defichain-3.0.0b3/defichain/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/RPCErrorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.913680 defichain-3.0.0b3/defichain/node/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21262 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53564 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/masternodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16833 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/poolpair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/proposals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40311 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/rawtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/spv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86413 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/modules/zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/node/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.913680 defichain-3.0.0b3/defichain/ocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/OceanErrorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.917680 defichain-3.0.0b3/defichain/ocean/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/consortium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/governance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/masternodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/poolpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/prices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/rawTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/modules/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/ocean/ocean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.917680 defichain-3.0.0b3/defichain/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.917680 defichain-3.0.0b3/defichain/transactions/address/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/base58address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/baseaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/bech32address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/p2pkh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/p2sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/p2wpkh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/address/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.917680 defichain-3.0.0b3/defichain/transactions/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.921680 defichain-3.0.0b3/defichain/transactions/builder/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/governance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/loans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/masternode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/utxo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/modules/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/rawtransactionbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/builder/txbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.921680 defichain-3.0.0b3/defichain/transactions/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/defitx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/fees.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.921680 defichain-3.0.0b3/defichain/transactions/constants/mainnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/mainnet/LOAN_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/mainnet/STANDARD_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/mainnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/rawtransactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.921680 defichain-3.0.0b3/defichain/transactions/constants/testnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/testnet/CUSTOM_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/testnet/LOAN_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/testnet/STANDARD_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/testnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/constants/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.921680 defichain-3.0.0b3/defichain/transactions/defitx/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/builddefitx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/defitx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.921680 defichain-3.0.0b3/defichain/transactions/defitx/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/basedefitx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/baseinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/governance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/loans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/masternode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/defitx/modules/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.925680 defichain-3.0.0b3/defichain/transactions/rawtransactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/txbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/txinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/txoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/rawtransactions/witness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.925680 defichain-3.0.0b3/defichain/transactions/remotedata/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/remotedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/remotedata/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/remotedata/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/remotedata/remotedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.925680 defichain-3.0.0b3/defichain/transactions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/utils/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-30 10:39:12.000000 defichain-3.0.0b3/defichain/transactions/utils/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:39:22.905680 defichain-3.0.0b3/defichain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-30 10:39:22.000000 defichain-3.0.0b3/defichain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-30 10:39:22.000000 defichain-3.0.0b3/defichain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:39:22.000000 defichain-3.0.0b3/defichain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 10:39:22.000000 defichain-3.0.0b3/defichain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 10:39:22.000000 defichain-3.0.0b3/defichain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 10:39:12.000000 defichain-3.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 10:39:12.000000 defichain-3.0.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:39:22.925680 defichain-3.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 10:39:12.000000 defichain-3.0.0b3/setup.py
```

### Comparing `defichain-3.0.0b2/LICENSE` & `defichain-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/PKG-INFO` & `defichain-3.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defichain
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Defichain Python Library
 Home-page: https://github.com/eric-volz/DefichainPython
 Author: Intr0c
 Author-email: introc@volz.link
 Keywords: python,defichain,node,ocean,mnemonic,wallet,privateKey,transactions,raw transactions,P2PKH,P2SH,P2WPKH,DefiTx,custom transaction
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `defichain-3.0.0b2/README.md` & `defichain-3.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/exceptions/http/HTTPStatusCode.py` & `defichain-3.0.0b3/defichain/exceptions/http/HTTPStatusCode.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/exceptions/http/RPCErrorCode.py` & `defichain-3.0.0b3/defichain/exceptions/http/RPCErrorCode.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/exceptions/http/__init__.py` & `defichain-3.0.0b3/defichain/exceptions/http/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/hdwallet/account.py` & `defichain-3.0.0b3/defichain/hdwallet/account.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/hdwallet/derivations.py` & `defichain-3.0.0b3/defichain/hdwallet/derivations.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/hdwallet/encryption.py` & `defichain-3.0.0b3/defichain/hdwallet/encrypt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import base64
 import hashlib
-#from Crypto import Random
-#from Crypto.Cipher import AES
+from Crypto import Random
+from Crypto.Cipher import AES
 
 
 class AESCipher(object):
 
     def __init__(self, key):
-        self.bs = AES.block_size
-        self.key = hashlib.sha256(key.encode(,).digest()
+        self._bs = AES.block_size
+        self._key = hashlib.sha256(key.encode()).digest()
 
-    def encrypt(self, raw):
+    def get_block_size(self) -> int:
+        return self._bs
+
+    def get_key(self) -> str:
+        return self._key.hex()
+
+    def _get_bytes_key(self) -> bytes:
+        return self._key
+
+    def encrypt(self, raw:  str) -> str:
         raw = self._pad(raw)
         iv = Random.new().read(AES.block_size)
-        cipher = AES.new(self.key, AES.MODE_CBC, iv)
-        return base64.b64encode(iv + cipher.encrypt(raw.encode(,)).hex()
+        cipher = AES.new(self._get_bytes_key(), AES.MODE_CBC, iv)
+        return base64.b64encode(iv + cipher.encrypt(raw.encode())).hex()
 
-    def decrypt(self, enc):
+    def decrypt(self, enc: str) -> str:
         enc = base64.b64decode(bytes.fromhex(enc))
         iv = enc[:AES.block_size]
-        cipher = AES.new(self.key, AES.MODE_CBC, iv)
+        cipher = AES.new(self._get_bytes_key(), AES.MODE_CBC, iv)
         return self._unpad(cipher.decrypt(enc[AES.block_size:])).decode('utf-8')
 
     def _pad(self, s):
-        return s + (self.bs - len(s) % self.bs) * chr(self.bs - len(s) % self.bs)
+        return s + (self.get_block_size() - len(s) % self.get_block_size()) * \
+            chr(self.get_block_size() - len(s) % self.get_block_size())
 
     @staticmethod
     def _unpad(s):
         return s[:-ord(s[len(s)-1:])]
-
-
-if "__main__" == __name__:
-    aes = AESCipher("test")
-    print(aes.key)
-
-    e = aes.encrypt("expire moon few future amount auto energy trade amazing surge museum potato session action must music buddy solve venue media chronic casino armed physical")
-    print(e)
-
-    d = aes.decrypt(e)
-    print(d)
```

### Comparing `defichain-3.0.0b2/defichain/hdwallet/utils.py` & `defichain-3.0.0b3/defichain/hdwallet/utils.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/hdwallet/wallet.py` & `defichain-3.0.0b3/defichain/hdwallet/wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,37 @@
 from ecdsa.keys import SigningKey, VerifyingKey
 
 from ecdsa.ecdsa import int_to_string, string_to_int
 
 from binascii import hexlify, unhexlify
 
 from defichain.mnemonic import Mnemonic
+from defichain.hdwallet.encrypt import AESCipher
+from defichain.networks import DefichainMainnet, DefichainTestnet
 from hashlib import sha256
 from typing import Optional, Any, Union
 
 import hmac
 import ecdsa
 import struct
 import unicodedata
 import hashlib
 import base58
+import json
 
 from defichain.libs.ripemd160 import ripemd160
 from defichain.libs.ecc import S256Point, G
 from defichain.libs.bech32 import encode
 from defichain.libs.base58 import check_encode, check_decode, ensure_string
 
 from defichain.networks.networks import Network
 
 from .derivations import Derivation
 
-from defichain.exceptions.hdwallet.DerivationError import DerivationError
+from defichain.exceptions.hdwallet import DerivationError, NetworkError, WalletError
 
 from .utils import (
     get_bytes, is_entropy, is_mnemonic, get_entropy_strength, _unhexlify,
     get_mnemonic_language, get_mnemonic_strength, get_semantic
 )
 
 MIN_ENTROPY_LEN: int = 128
@@ -52,14 +55,78 @@
     :type semantic: str
     :param use_default_path: Use default derivation path, defaults to ``False``.
     :type use_default_path: bool
 
     :returns: Wallet -- Hierarchical Deterministic Wallet instance.
     """
 
+    @staticmethod
+    def decrypt(passphrase: str, data: str = None, filename: str = None) -> "Wallet":
+        """
+        Decrypt a wallet, witch is stored as a string
+
+        >>> from defichain import Wallet
+        >>> from defichain.networks import DefichainMainnet
+        >>> Wallet.decrypt("password", filename="wallet.hd")
+
+        :param passphrase: (required) the passphrase / key to decrypt the data
+        :type passphrase: str
+        :param data: (optional) encrypted data
+        :type data: str
+        :param filename: (optional) filename, where the encrypted data is stored
+        :type filename: str
+        :return: Wallet
+        """
+        # Decryption module
+        aes = AESCipher(passphrase)
+
+        # Check if only one attribute is specified
+        if data and filename:
+            raise AttributeError("Only one of the parameters may be given: data or filename")
+
+        # Copy data from file if specified
+        if filename:
+            with open(filename, "r") as f:
+                data = f.read()
+
+        # Decrypt
+        wallet_data = json.loads(aes.decrypt(data))
+
+        # Select Network
+        networkType = wallet_data.get("network")
+        if networkType == "mainnet":
+            network = DefichainMainnet
+        elif networkType == "testnet":
+            network = DefichainTestnet
+        else:
+            raise NotImplementedError("Only defichain mainnet and testnet is supported")
+
+        # Build Wallet
+        language = wallet_data.get("language")
+        wallet_passphrase = wallet_data.get("passphrase")
+
+        wallet = Wallet(network)
+
+        if wallet_data.get("entropy"):
+            wallet.from_entropy(entropy=wallet_data.get("entropy"), language=language, passphrase=wallet_passphrase)
+        elif wallet_data.get("mnemonic"):
+            wallet.from_mnemonic(mnemonic=wallet_data.get("mnemonic"), language=language, passphrase=wallet_passphrase)
+        elif wallet_data.get("seed"):
+            wallet.from_seed(wallet_data.get("seed"))
+        elif wallet_data.get("wif"):
+            wallet.from_wif(wallet_data.get("wif"))
+        elif wallet_data.get("private_key"):
+            wallet.from_private_key(wallet_data.get("private_key"))
+        elif wallet_data.get("public_key"):
+            wallet.from_public_key(wallet_data.get("public_key"))
+        else:
+            raise WalletError("The necessary information to restore the wallet is not given")
+
+        return wallet
+
     def __init__(self, network: Any, semantic: Optional[str] = None, use_default_path: bool = True):
         self._cryptocurrency: Any = None
         if network:
             if not issubclass(network, Network):
                 raise TypeError("Invalid Network type, the sub class must be Network instance.")
             self._cryptocurrency: Any = network
 
@@ -1240,14 +1307,29 @@
         "KxGKLeymbFrSY7t3X31FMaDgQDUQGYvhUACLe4o1LXokvWtMs1WU"
         """
 
         return check_encode(
             _unhexlify(self._cryptocurrency.WIF_SECRET_KEY) + self._key.to_string() + b"\x01") if self._key else None
 
     def get_account(self, index: int = 0, prefix: str = "m/1129/0/0/"):
+        """
+        Returns the account of the specified prefix and index
+
+        >>> from defichain import Wallet
+        >>> from defichain.networks import DefichainMainnet
+        >>> wallet = Wallet(network=DefichainMainnet)
+        >>> wallet.from_mnemonic(mnemonic="venture fitness paper little blush april rigid where find volcano fetch crack label polar dash", passphrase="password")
+        >>> wallet.get_account(0)
+
+        :param index: (optional) number of account
+        :type index: int
+        :param prefix: (optional) prefix from which the account is to be derived
+        :type prefix: str
+        :return: Account
+        """
         from .account import Account
         previousPath = self.path()
         path = prefix + str(index)
 
         if self.seed():
             self.from_path(path)
 
@@ -1255,14 +1337,38 @@
             acc = Account(self._cryptocurrency, self.private_key())
         else:
             acc = Account(self._cryptocurrency, self.public_key())
         if self.seed():
             self.from_path(previousPath)
         return acc
 
+    def encrypt(self, passphrase: str, filename: str = None) -> str:
+        """
+        Encrypts the wallet into a string
+
+        >>> from defichain import Wallet
+        >>> from defichain.networks import DefichainMainnet
+        >>> wallet = Wallet(network=DefichainMainnet)
+        >>> wallet.from_mnemonic(mnemonic="venture fitness paper little blush april rigid where find volcano fetch crack label polar dash", passphrase="password")
+        >>> wallet.encrypt("password")
+
+        :param passphrase: (required) the passphrase / key to encrypt the data
+        :type passphrase: str
+        :param filename: (required) filename, where the encrypted data should be stored
+        :type filename: str
+        :return: str -- encrypted string
+        """
+        aes = AESCipher(passphrase)
+        e = aes.encrypt(json.dumps(self.dumps()))
+
+        if filename:
+            with open(filename, "w") as f:
+                f.write(e)
+        return e
+
     def dumps(self) -> dict:
         """
         Get All Wallet imformations.
 
         :returns: dict -- All Wallet imformations.
 
         >>> from defichain import Wallet
```

### Comparing `defichain-3.0.0b2/defichain/libs/base58.py` & `defichain-3.0.0b3/defichain/libs/base58.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/libs/bech32.py` & `defichain-3.0.0b3/defichain/libs/bech32.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/libs/ecc.py` & `defichain-3.0.0b3/defichain/libs/ecc.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/libs/ripemd160.py` & `defichain-3.0.0b3/defichain/libs/ripemd160.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/logger.py` & `defichain-3.0.0b3/defichain/logger.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/mnemonic.py` & `defichain-3.0.0b3/defichain/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_simplified.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_traditional.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/english.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/french.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/italian.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/japanese.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/korean.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/korean.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/mnemonic/wordlist/spanish.txt` & `defichain-3.0.0b3/defichain/mnemonic/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/networks/networks.py` & `defichain-3.0.0b3/defichain/networks/networks.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/RPCErrorHandler.py` & `defichain-3.0.0b3/defichain/node/RPCErrorHandler.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/__init__.py` & `defichain-3.0.0b3/defichain/node/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/accounts.py` & `defichain-3.0.0b3/defichain/node/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/blockchain.py` & `defichain-3.0.0b3/defichain/node/modules/blockchain.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/control.py` & `defichain-3.0.0b3/defichain/node/modules/control.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/generating.py` & `defichain-3.0.0b3/defichain/node/modules/generating.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/loan.py` & `defichain-3.0.0b3/defichain/node/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/masternodes.py` & `defichain-3.0.0b3/defichain/node/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/mining.py` & `defichain-3.0.0b3/defichain/node/modules/mining.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/network.py` & `defichain-3.0.0b3/defichain/node/modules/network.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/oracles.py` & `defichain-3.0.0b3/defichain/node/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/poolpair.py` & `defichain-3.0.0b3/defichain/node/modules/poolpair.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/proposals.py` & `defichain-3.0.0b3/defichain/node/modules/proposals.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/rawtransactions.py` & `defichain-3.0.0b3/defichain/node/modules/rawtransactions.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/stats.py` & `defichain-3.0.0b3/defichain/node/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/tokens.py` & `defichain-3.0.0b3/defichain/node/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/util.py` & `defichain-3.0.0b3/defichain/node/modules/util.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/vault.py` & `defichain-3.0.0b3/defichain/node/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/wallet.py` & `defichain-3.0.0b3/defichain/node/modules/wallet.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/modules/zmq.py` & `defichain-3.0.0b3/defichain/node/modules/zmq.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/node.py` & `defichain-3.0.0b3/defichain/node/node.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/rpc.py` & `defichain-3.0.0b3/defichain/node/rpc.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/node/util.py` & `defichain-3.0.0b3/defichain/node/util.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/OceanErrorHandler.py` & `defichain-3.0.0b3/defichain/ocean/OceanErrorHandler.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/__init__.py` & `defichain-3.0.0b3/defichain/ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/connection.py` & `defichain-3.0.0b3/defichain/ocean/connection.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/address.py` & `defichain-3.0.0b3/defichain/ocean/modules/address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/blocks.py` & `defichain-3.0.0b3/defichain/ocean/modules/blocks.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/consortium.py` & `defichain-3.0.0b3/defichain/ocean/modules/consortium.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/fee.py` & `defichain-3.0.0b3/defichain/ocean/modules/fee.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/governance.py` & `defichain-3.0.0b3/defichain/ocean/modules/governance.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/loan.py` & `defichain-3.0.0b3/defichain/ocean/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/masternodes.py` & `defichain-3.0.0b3/defichain/ocean/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/oracles.py` & `defichain-3.0.0b3/defichain/ocean/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/poolpairs.py` & `defichain-3.0.0b3/defichain/ocean/modules/poolpairs.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/prices.py` & `defichain-3.0.0b3/defichain/ocean/modules/prices.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/rawTx.py` & `defichain-3.0.0b3/defichain/ocean/modules/rawTx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/rpc.py` & `defichain-3.0.0b3/defichain/ocean/modules/rpc.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/stats.py` & `defichain-3.0.0b3/defichain/ocean/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/tokens.py` & `defichain-3.0.0b3/defichain/ocean/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/modules/transactions.py` & `defichain-3.0.0b3/defichain/ocean/modules/transactions.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/ocean/ocean.py` & `defichain-3.0.0b3/defichain/ocean/ocean.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,24 @@
             >>> blocks = ocaen.blocks.list()  #  returns the latest 30 blocks
             >>> print(blocks)
     """
 
     def __init__(self, url: str = "https://ocean.defichain.com", version: str = "v0",
                  network: str = "mainnet", logger: Logger = None) -> "Ocean":
 
+        if url != "https://ocean.defichain.com":
+            pass
+        elif network == "mainnet":
+            url = "https://ocean.defichain.com"
+        elif network == "testnet":
+            url = "https://testnet.ocean.jellyfishsdk.com"
+        else:
+            raise Exception("The network that is specified is not available. Use one of these networks: 'mainnet', "
+                            "'testnet'")
+
         self._attachedURL = url + "/" + version + "/" + network + "/"
         self._test_connection()
 
         self._conn = Connection(self._attachedURL, logger)
 
         self.address = Address(self)
         self.blocks = Blocks(self)
```

### Comparing `defichain-3.0.0b2/defichain/transactions/address/address.py` & `defichain-3.0.0b3/defichain/transactions/address/address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/address/base58address.py` & `defichain-3.0.0b3/defichain/transactions/address/base58address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/address/baseaddress.py` & `defichain-3.0.0b3/defichain/transactions/address/baseaddress.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/address/bech32address.py` & `defichain-3.0.0b3/defichain/transactions/address/bech32address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/address/p2pkh.py` & `defichain-3.0.0b3/defichain/transactions/address/p2pkh.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/address/p2sh.py` & `defichain-3.0.0b3/defichain/transactions/address/p2sh.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/address/p2wpkh.py` & `defichain-3.0.0b3/defichain/transactions/address/p2wpkh.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/address/script.py` & `defichain-3.0.0b3/defichain/transactions/address/script.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/modules/accounts.py` & `defichain-3.0.0b3/defichain/transactions/builder/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/modules/data.py` & `defichain-3.0.0b3/defichain/transactions/builder/modules/data.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/modules/governance.py` & `defichain-3.0.0b3/defichain/transactions/builder/modules/governance.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/modules/loans.py` & `defichain-3.0.0b3/defichain/transactions/builder/modules/loans.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/modules/pool.py` & `defichain-3.0.0b3/defichain/transactions/builder/modules/pool.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/modules/utxo.py` & `defichain-3.0.0b3/defichain/transactions/builder/modules/utxo.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/modules/vault.py` & `defichain-3.0.0b3/defichain/transactions/builder/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/rawtransactionbuilder.py` & `defichain-3.0.0b3/defichain/transactions/builder/rawtransactionbuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from defichain import Account
 from defichain.exceptions.transactions import TxBuilderError, NotYetSupportedError
 
 from defichain.transactions.address import Address
 from defichain.transactions.constants import AddressTypes, DefiTxType
 from defichain.networks import Network
 from defichain.transactions.remotedata.remotedata import RemoteData
-from defichain.transactions.rawtransactions import Transaction, TxInput, TxP2WPKHInput, TxP2SHInput, TxAddressOutput, \
-    TxDefiOutput, estimate_fee
+from defichain.transactions.rawtransactions import Transaction, TxInput, TxP2PKHInput, TxP2WPKHInput, TxP2SHInput, \
+    TxAddressOutput, TxDefiOutput, estimate_fee
 from defichain.transactions.defitx.modules.basedefitx import BaseDefiTx
 
 
 class RawTransactionBuilder:
 
     @staticmethod
     def new_transaction() -> Transaction:
@@ -30,25 +30,25 @@
         if inputs or self.get_dataSource() is None:
             tx.set_inputs(inputs)
         else:
             for input in self.get_dataSource().get_unspent(self.get_address()):
                 address = Address.from_scriptPublicKey(self.get_account().get_network(), input["scriptPubKey"])
                 # Build P2PKH Input
                 if address.get_addressType() == AddressTypes.P2PKH:
-                    raise NotYetSupportedError()
+                    tx.add_input(TxP2PKHInput(input["txid"], input["vout"], self.get_address(), input["value"]))
                 # Build P2SH Input
                 elif address.get_addressType() == AddressTypes.P2SH:
                     tx.add_input(TxP2SHInput(input["txid"], input["vout"], self.get_account().get_p2wpkh(),
                                              input["value"]))
                 # Build P2WPKH Input
                 elif address.get_addressType() == AddressTypes.P2WPKH:
                     tx.add_input(TxP2WPKHInput(input["txid"], input["vout"], self.get_address(), input["value"]))
             # Check Inputs for masternode collateral
             tx.set_inputs(self.checkMasternodeInputs(tx.get_inputs()))
-        if tx.get_inputs() == []:
+        if not tx.get_inputs():
             raise TxBuilderError(f"Given address: {self._address} has no unspent inputs. Check your builder object!")
         return tx
 
     def build_defiTx(self, value: int, defiTx: BaseDefiTx, inputs=[], **additionalData) -> Transaction:
         tx = self.build_transactionInputs(inputs)
 
         # Check for errors in Inputs
```

### Comparing `defichain-3.0.0b2/defichain/transactions/builder/txbuilder.py` & `defichain-3.0.0b3/defichain/transactions/builder/txbuilder.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/defitx.py` & `defichain-3.0.0b3/defichain/transactions/constants/defitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/mainnet/CUSTOM_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/mainnet/CUSTOM_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/mainnet/LOAN_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/mainnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/mainnet/STANDARD_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/mainnet/STANDARD_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/opcodes.py` & `defichain-3.0.0b3/defichain/transactions/constants/opcodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/testnet/CUSTOM_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/testnet/CUSTOM_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/testnet/LOAN_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/testnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/testnet/STANDARD_tokens.json` & `defichain-3.0.0b3/defichain/transactions/constants/testnet/STANDARD_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/constants/tokens.py` & `defichain-3.0.0b3/defichain/transactions/constants/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/builddefitx.py` & `defichain-3.0.0b3/defichain/transactions/defitx/builddefitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/defitx.py` & `defichain-3.0.0b3/defichain/transactions/defitx/defitx.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
             return PaybackLoan.deserialize(network, hex[position:])
 
         # Masternode
         elif DefiTxType.OP_DEFI_TX_CREATE_MASTER_NODE == defiTxType:
             return CreateMasternode.deserialize(network, hex[position:])
         elif DefiTxType.OP_DEFI_TX_RESIGN_MASTER_NODE == defiTxType:
             return ResignMasternode.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_UPDATE_MASTER_NODE == defiTxType:
+            return UpdateMasternode.deserialize(network, hex[position:])
 
         # Pool
         elif DefiTxType.OP_DEFI_TX_POOL_SWAP == defiTxType:
             return PoolSwap.deserialize(network, hex[position:])
         elif DefiTxType.OP_DEFI_TX_COMPOSITE_SWAP == defiTxType:
             return CompositeSwap.deserialize(network, hex[position:])
         elif DefiTxType.OP_DEFI_TX_POOL_ADD_LIQUIDITY == defiTxType:
```

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/modules/accounts.py` & `defichain-3.0.0b3/defichain/transactions/defitx/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/modules/basedefitx.py` & `defichain-3.0.0b3/defichain/transactions/defitx/modules/basedefitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/modules/baseinput.py` & `defichain-3.0.0b3/defichain/transactions/defitx/modules/baseinput.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Any
 
 from defichain.exceptions.transactions import AddressError
 from defichain.transactions.utils import Token, Verify, BuildAddressAmounts
 from defichain.transactions.address import Address
 from defichain.transactions.utils import Converter, Calculate
+from defichain.transactions.constants import AddressTypes
 
 
 class BaseInput(ABC):
 
     @staticmethod
     @abstractmethod
     def deserialize(network: Any, hex: str) -> "BaseInput":
@@ -163,17 +164,19 @@
         numberOfReceivers = Converter.hex_to_int(hex[position: position + 2])
         position += 2
 
         scriptBalances = []
 
         for _ in range(numberOfReceivers):
             length_addressTo = Converter.hex_to_int(hex[position: position + 2]) * 2
-            numberOfAmounts = Converter.hex_to_int(hex[position + 2 + length_addressTo: position + 2 + length_addressTo + 2])
+            numberOfAmounts = Converter.hex_to_int(
+                hex[position + 2 + length_addressTo: position + 2 + length_addressTo + 2])
 
-            scriptBalance = ScriptBalances.deserialize(network, hex[position: position + 2 + length_addressTo + 2 + numberOfAmounts * TokenBalanceInt32.estimated_size()])
+            scriptBalance = ScriptBalances.deserialize(network, hex[
+                                                                position: position + 2 + length_addressTo + 2 + numberOfAmounts * TokenBalanceInt32.estimated_size()])
             scriptBalances.append(scriptBalance)
 
             position += 2 + length_addressTo + 2 + numberOfAmounts * TokenBalanceInt32.estimated_size()
         return scriptBalances
 
     @staticmethod
     def to_json(scriptBalances: []) -> {}:
@@ -210,7 +213,70 @@
 
     def get_script(self) -> str:
         return Address.from_address(self._address).get_scriptPublicKey()
 
     def get_bytes_script(self) -> bytes:
         return Converter.hex_to_bytes(self.get_script())
 
+
+class MasternodeUpdates(BaseInput):
+    """
+    Update Types: 1 byte, 1 = OwnerAddress, 2 = OperatorAddress, 3 = SetRewardAddress, 4 = RemRewardAddress
+    Address Types: 1 byte, 1 = p2pkh, 4 = p2wpkh, 0 to remove reward address
+    """
+
+    @staticmethod
+    def deserialize(network: Any, hex: str):
+        pass
+
+    def __init__(self, updateType: int, address: str):
+        self._updateType, self._address, self._addressType = None, None, None
+        self.set_updateType(updateType)
+        self.set_address(address)
+
+    def __bytes__(self) -> bytes:
+        # Convert to Bytes
+        updateType = Converter.int_to_bytes(self.get_updateType(), 1)
+        addressType = Converter.int_to_bytes(self._addressType, 1)
+        if self.get_address() == "":
+            addressPubKeyHash = Converter.hex_to_bytes("")
+        else:
+            addressPubKeyHash = Converter.hex_to_bytes(Address.from_address(self.get_address()).get_publicKeyHash())
+
+        sizeAddressPubKeyHash = Converter.int_to_bytes(len(addressPubKeyHash), 1)
+
+        # Build UpdateMasternodeDefiTx
+        result = updateType
+        result += addressType
+        result += sizeAddressPubKeyHash
+        result += addressPubKeyHash
+
+        return result
+
+    # Get Information
+    def get_updateType(self) -> int:
+        return self._updateType
+
+    def get_address(self) -> str:
+        return self._address
+
+    def get_addressType(self) -> int:
+        return self._addressType
+
+    # Set Information
+    def set_updateType(self, updateType: int):
+        self._updateType = updateType
+
+    def set_address(self, address: str):
+        if address == "":
+            self._addressType = 0
+            self._address = address
+        else:
+            addressType = Address.from_address(address).get_addressType()
+            if addressType == AddressTypes.P2PKH:
+                self._addressType = 1
+            elif addressType == AddressTypes.P2WPKH:
+                self._addressType = 4
+            else:
+                raise AddressError("Only P2PKH and P2WPKH can be used to update the masternode")
+            self._address = address
+
```

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/modules/governance.py` & `defichain-3.0.0b3/defichain/transactions/defitx/modules/governance.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/modules/loans.py` & `defichain-3.0.0b3/defichain/transactions/defitx/modules/loans.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/modules/pool.py` & `defichain-3.0.0b3/defichain/transactions/defitx/modules/pool.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/defitx/modules/vault.py` & `defichain-3.0.0b3/defichain/transactions/defitx/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/keys.py` & `defichain-3.0.0b3/defichain/transactions/keys.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/rawtransactions/fee.py` & `defichain-3.0.0b3/defichain/transactions/rawtransactions/fee.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/rawtransactions/sign.py` & `defichain-3.0.0b3/defichain/transactions/rawtransactions/sign.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 from binascii import hexlify, unhexlify
 import struct
 from hashlib import sha256
 from ecdsa import SigningKey, SECP256k1
-from ecdsa.util import sigencode_der
+from ecdsa.util import sigencode_der, sigencode_der_canonize
 
 from defichain.transactions.constants import ORDER
+from defichain.transactions.utils import Converter
 
 
-def sign_input(privateKey: str, data: bytes) -> str:
+def sign_legacy_input(privateKey: str, data: bytes, sigHash: bytes) -> str:
+    """
+    Signs the given data with a given private key in a deterministic way
+
+    :param privateKey: (required) private key to sign the input
+    :type privateKey: str
+    :param data: (required) data that has to be signed
+    :type data: bytes
+    :param sigHash: (required) sigHash to be signed with
+    :type sigHash: bytes
+    :return: "hex" - signature of data
+    """
+    sk = SigningKey.from_string(unhexlify(privateKey), curve=SECP256k1)
+    s = sk.sign_deterministic(data, hashfunc=sha256, sigencode=sigencode_der_canonize)
+    signature = Converter.bytes_to_hex(s) + Converter.bytes_to_hex(sigHash)[:2]  # SIGHASH_ALL
+    return signature
+
+
+def sign_segwit_input(privateKey: str, data: bytes) -> str:
     """
     Signs the given data with a given private key in a deterministic way
 
     :param privateKey: (required) private key to sign the input
     :type privateKey: str
     :param data: (required) data that has to be signed
     :type data: bytes
```

### Comparing `defichain-3.0.0b2/defichain/transactions/rawtransactions/tx.py` & `defichain-3.0.0b3/defichain/transactions/rawtransactions/tx.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import ABC, abstractmethod
 from typing import Any
+from hashlib import sha256
 
 from defichain.exceptions.transactions import RawTransactionError, NotYetSupportedError, DeserializeError
 from defichain.networks import Network
 from defichain.transactions.address import Address
 from defichain.transactions.keys import PrivateKey, KeyError, PublicKey
 from defichain.transactions.utils import Converter, Calculate
 from defichain.transactions.constants import SIGHASH, AddressTypes
 
 from .txbase import TxBase
 from .txinput import TxBaseInput, TxInput, TxP2PKHInput, TxP2SHInput, TxP2WPKHInput, TxCoinbaseInput
 from .txoutput import TxBaseOutput, TxOutput, TxAddressOutput, TxDataOutput, TxDefiOutput, TxCoinbaseOutput
 from .witness import WitnessHash, Witness
-from .sign import sign_input
+from .sign import sign_segwit_input, sign_legacy_input
 
 
 class BaseTransaction(TxBase, ABC):
 
     def __init__(self, inputs: [], outputs: [], lockTime: int = 0):
         self._version, self._marker, self._flag, self._sigHash, self._inputs, self._outputs, self._lockTime = None, None, None, None, [], [], None
         self._signed = False
@@ -31,14 +32,17 @@
     def sign(self, network: Any, private_keys: [str]) -> "Transaction":
         pass
 
     @abstractmethod
     def _analyse(self):
         pass
 
+    def unsigned(self) -> str:
+        return Converter.bytes_to_hex(self.bytes_unsigned())
+
     def bytes_unsigned(self) -> bytes:
         # Version
         result = self.get_bytes_version()
 
         # Inputs
         result += Calculate.write_compactSize(len(self.get_inputs()), "bytes")
         for input in self.get_inputs():
@@ -59,19 +63,16 @@
         result += self.get_bytes_lockTime()
         return result
 
     # Calculated Information
     def get_inputsValue(self) -> "int | None":
         result = 0
         for input in self.get_inputs():
-            if isinstance(input, TxP2PKHInput) or isinstance(input, TxCoinbaseInput):
+            if input.get_value() is None:
                 return None
-            elif isinstance(input, TxP2WPKHInput) or isinstance(input, TxP2SHInput):
-                if input.get_value() is None:
-                    return None
             result += input.get_value()
         return result
 
     def get_outputsValue(self) -> int:
         result = 0
         for outputs in self.get_outputs():
             result += outputs.get_value()
@@ -126,16 +127,15 @@
     def get_lockTime(self) -> int:
         return self._lockTime
 
     def get_txid(self) -> str:
         return Converter.bytes_to_hex(bytes(reversed(Calculate.dHash256(self.bytes_unsigned()))))
 
     def get_hash(self):
-        hash = Calculate.dHash256(self.bytes())
-        return Converter.bytes_to_hex(bytes(reversed(hash)))
+        return Converter.bytes_to_hex(bytes(reversed(Calculate.dHash256(self.bytes()))))
 
     def get_bytes_version(self) -> bytes:
         return Converter.int_to_bytes(self.get_version(), 4)
 
     def get_bytes_marker(self) -> bytes:
         return Converter.int_to_bytes(self.get_marker(), 1)
 
@@ -310,28 +310,30 @@
                     if hex[position: position + 2] == "00":
                         if len(hex) - position <= 8:
                             break
                         position += 2
                     elif hex[position: position + 2] == "02":
                         position += 2
                         length_signature = Converter.hex_to_int(hex[position: position + 2]) * 2
-                        length_publicKey = Converter.hex_to_int(hex[position + 2 + length_signature: position + 2 + length_signature + 2]) * 2
+                        length_publicKey = Converter.hex_to_int(
+                            hex[position + 2 + length_signature: position + 2 + length_signature + 2]) * 2
                         length_witness = 2 + length_signature + 2 + length_publicKey
                         witness = Witness.deserialize(network, hex[position: position + length_witness])
                         witnesses.append(witness)
                         position += length_witness
                         tx._signed = True
 
             # Match all witnisses with the corresponding input
             if tx.is_signed():
                 count_witness = 0
                 count_inputs = 0
                 for input in inputs:
                     if isinstance(input, TxP2SHInput):
-                        publicKey_address = PublicKey(network, witnesses[count_witness].get_publicKey()).p2wpkh_address()
+                        publicKey_address = PublicKey(network,
+                                                      witnesses[count_witness].get_publicKey()).p2wpkh_address()
                         script_address = Address.from_scriptPublicKey(network, input.get_scriptSig()[2:]).get_address()
                         if publicKey_address == script_address:
                             input.set_witness(witnesses[count_witness])
                             count_witness += 1
                         else:
                             raise DeserializeError("The given p2sh input script signature does not correspond with the "
                                                    "given witness")
@@ -344,15 +346,14 @@
 
             tx.set_inputs(inputs)
             tx.set_outputs(outputs)
             tx.set_witness(witnesses)
 
             # Coinbase Transaction
             if tx.is_coinbase():
-
                 numberOfCoinbaseElements = Converter.hex_to_int(hex[position: position + 2])
                 position += 2
 
                 length_coinbase = Converter.hex_to_int(hex[position: position + 2]) * 2
                 position += 2
 
                 coinbaseElement = Converter.hex_to_int(hex[position: position + length_coinbase])
@@ -449,50 +450,70 @@
         order as the inputs
         :type private_keys: [str]
         :return: Transaction
         """
         if not isinstance(private_keys, list):
             raise RawTransactionError("The given private keys have to be parsed in a list: [key, key, ...]")
 
-        # Check if wif and calc hexadecimal private key
+        # Check if wif and calc hexadecimal private key and public key
         keys = []
         for key in private_keys:
             if PrivateKey.is_privateKey(network, key):
                 key = PrivateKey(network, privateKey=key)
             elif PrivateKey.is_wif(network, key):
                 key = PrivateKey(network, wif=key)
             else:
                 raise KeyError("Given private key is not valid")
             keys.append({"private": key.get_privateKey(), "public": key.get_publicKey()})
 
-        # Sign
         index = 0
+        scriptSignatures = []
         for input in self.get_inputs():
-            if isinstance(input, TxP2PKHInput):
-                raise NotYetSupportedError()
-            elif isinstance(input, TxP2WPKHInput) or isinstance(input, TxP2SHInput):
-                if len(private_keys) == 1:
-                    privKey = keys[0]["private"]
-                    pubKey = keys[0]["public"]
+            # Check Keys for Input
+            if len(private_keys) == 1:
+                privKey = keys[0]["private"]
+                pubKey = keys[0]["public"]
+            else:
+                if len(private_keys) <= index:
+                    raise RawTransactionError("The transaction could not from be signed. Not enough private keys "
+                                              "were provided in the list")
                 else:
-                    if len(private_keys) <= index:
-                        raise RawTransactionError("The transaction could not from be signed. Not enough private keys "
-                                                  "were provided in the list")
-                    else:
-                        privKey = keys[index]["private"]
-                        pubKey = keys[index]["public"]
+                    privKey = keys[index]["private"]
+                    pubKey = keys[index]["public"]
+
+            # Sign different Inputs
+            if isinstance(input, TxP2PKHInput):
+                SIGHASH_ALL = Converter.int_to_bytes(SIGHASH, 4)
 
+                input.set_scriptSig(Address.from_address(input.get_address()).get_scriptPublicKey())
+                h = sha256(self.bytes() + SIGHASH_ALL).digest()
+
+                signature = sign_legacy_input(privKey, h, SIGHASH_ALL)
+                scriptSignature = Converter.int_to_hex(int(len(signature) / 2), 1) + signature + \
+                                  Converter.int_to_hex(int(len(pubKey) / 2), 1) + pubKey
+                input.set_scriptSig("")
+                scriptSignatures.append(scriptSignature)
+
+            elif isinstance(input, TxP2WPKHInput) or isinstance(input, TxP2SHInput):
                 witness_hash = WitnessHash(self, input)
-                signature = sign_input(privKey, witness_hash.bytes_hash())
+                signature = sign_segwit_input(privKey, witness_hash.bytes_hash())
                 witness = Witness(signature, pubKey)
                 input.set_witness(witness)
 
             else:
                 raise NotYetSupportedError()
             index += 1
+
+        # Assign ScriptSignatures to P2PKH Inputs after signing
+        index = 0
+        for input in self.get_inputs():
+            if isinstance(input, TxP2PKHInput):
+                input.set_scriptSig(scriptSignatures[index])
+            index += 1
+
         self._signed = True
 
         return self
 
     def _analyse(self):
         # Analyse Inputs
         signed = None
```

### Comparing `defichain-3.0.0b2/defichain/transactions/rawtransactions/txbase.py` & `defichain-3.0.0b3/defichain/transactions/rawtransactions/txbase.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/rawtransactions/txinput.py` & `defichain-3.0.0b3/defichain/transactions/rawtransactions/txinput.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC
 from typing import Any
 
 from .txbase import TxBase
+from defichain.transactions.keys import PublicKey
 from defichain.exceptions.transactions import AddressError, DeserializeError
 from defichain.transactions.constants import SEQUENCE
 from defichain.transactions.utils import Converter
 from defichain.networks import Network
 from defichain.transactions.address import Address
 from defichain.transactions.constants import AddressTypes
 
@@ -90,15 +91,17 @@
     def get_bytes_address(self) -> bytes:
         return Converter.hex_to_bytes(self.get_address())
 
     def get_bytes_value(self) -> bytes:
         return Converter.int_to_bytes(self.get_value(), 8)
 
     def get_bytes_unsignedInput(self) -> bytes:
-        return self.get_bytes_txid() + self.get_bytes_vout() + Converter.int_to_bytes(0, 1) + self.get_bytes_sequence()
+        scriptSigLength = len(self.get_bytes_scriptSig())
+        return self.get_bytes_txid() + self.get_bytes_vout() + Converter.int_to_bytes(scriptSigLength, 1) + \
+            self.get_bytes_scriptSig() + self.get_bytes_sequence()
 
     # Set Information
     def set_txid(self, txid: str) -> None:
         self._txid = txid
 
     def set_vout(self, vout: int) -> None:
         self._vout = vout
@@ -186,16 +189,17 @@
         json.update({"inputType": "unsigned"})
         json.update({"txid": self.get_txid()})
         json.update({"vout": self.get_vout()})
         json.update({"scriptSig": self.get_scriptSig()})
         json.update({"sequence": self.get_sequence()})
         return json
 
-    def to_p2pkhInput(self) -> "TxP2PKHInput":
-        return TxP2PKHInput(self.get_txid(), self.get_vout(), self.get_scriptSig(), self.get_sequence())
+    def to_p2pkhInput(self, network: Any) -> "TxP2PKHInput":
+        address = Address.from_scriptPublicKey(network, self.get_scriptSig()).get_address()
+        return TxP2PKHInput(self.get_txid(), self.get_vout(), address, None, self.get_sequence())
 
     def to_p2shInput(self, network: Any) -> "TxP2SHInput":
         address = Address.from_scriptPublicKey(network, self.get_scriptSig()).get_address()
         return TxP2SHInput(self.get_txid(), self.get_vout(), address, None, self.get_sequence())
 
     def to_p2wpkhInput(self) -> "TxP2WPKHInput":
         return TxP2WPKHInput(self.get_txid(), self.get_vout(), "", None, self.get_sequence())
@@ -215,29 +219,36 @@
     :type sequence: str
     """
 
     @staticmethod
     def deserialize(network: Any, hex: str) -> "TxP2PKHInput":
         input = TxBaseInput.deserialize(network, hex)
         if input.get_scriptSig() != "":
-            if len(input.get_scriptSig()) < 23:
+            if len(input.get_scriptSig()) < 214:
                 raise DeserializeError("The given input to decode is not an p2pkh input")
-
-        return TxP2PKHInput(input.get_txid(), input.get_vout(), input.get_scriptSig(), input.get_sequence())
-
-    def __init__(self, txid: str, vout: int, scriptSig: str = "", sequence: str = SEQUENCE):
-        super().__init__(txid, vout, scriptSig, sequence)
+        publicKey = input.get_scriptSig()[-66:]
+        address = PublicKey(network, publicKey).p2pkh_address()
+        resultInput = TxP2PKHInput(input.get_txid(), input.get_vout(), address, input.get_value(), input.get_sequence())
+        resultInput.set_scriptSig(input.get_scriptSig())
+        return resultInput
+
+    def __init__(self, txid: str, vout: int, address: str = "", value: int = None, sequence: str = SEQUENCE):
+        super().__init__(txid, vout, "", sequence)
+        self.set_value(value)
+        self.set_address(address)
 
     def to_json(self) -> {}:
         json = {}
         json.update({"inputType": AddressTypes.P2PKH})
         json.update({"txid": self.get_txid()})
         json.update({"vout": self.get_vout()})
         json.update({"scriptSig": self.get_scriptSig()})
         json.update({"sequence": self.get_sequence()})
+        json.update({"address": self.get_address()})
+        json.update({"value": self.get_value()})
         return json
 
 
 class TxP2SHInput(TxInput):
     """
     Input to spend from P2SH address
```

### Comparing `defichain-3.0.0b2/defichain/transactions/rawtransactions/txoutput.py` & `defichain-3.0.0b3/defichain/transactions/rawtransactions/txoutput.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/rawtransactions/witness.py` & `defichain-3.0.0b3/defichain/transactions/rawtransactions/witness.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/remotedata/node.py` & `defichain-3.0.0b3/defichain/transactions/remotedata/node.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/remotedata/ocean.py` & `defichain-3.0.0b3/defichain/transactions/remotedata/ocean.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/remotedata/remotedata.py` & `defichain-3.0.0b3/defichain/transactions/remotedata/remotedata.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/utils/calculate.py` & `defichain-3.0.0b3/defichain/transactions/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/utils/converter.py` & `defichain-3.0.0b3/defichain/transactions/utils/converter.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/utils/token.py` & `defichain-3.0.0b3/defichain/transactions/utils/token.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain/transactions/utils/verify.py` & `defichain-3.0.0b3/defichain/transactions/utils/verify.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b2/defichain.egg-info/PKG-INFO` & `defichain-3.0.0b3/defichain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defichain
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Defichain Python Library
 Home-page: https://github.com/eric-volz/DefichainPython
 Author: Intr0c
 Author-email: introc@volz.link
 Keywords: python,defichain,node,ocean,mnemonic,wallet,privateKey,transactions,raw transactions,P2PKH,P2SH,P2WPKH,DefiTx,custom transaction
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `defichain-3.0.0b2/defichain.egg-info/SOURCES.txt` & `defichain-3.0.0b3/defichain.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 defichain.egg-info/PKG-INFO
 defichain.egg-info/SOURCES.txt
 defichain.egg-info/dependency_links.txt
 defichain.egg-info/requires.txt
 defichain.egg-info/top_level.txt
 defichain/exceptions/__init__.py
 defichain/exceptions/hdwallet/DerivationError.py
+defichain/exceptions/hdwallet/NetworkError.py
+defichain/exceptions/hdwallet/WalletError.py
 defichain/exceptions/hdwallet/__init__.py
 defichain/exceptions/http/BadMethod.py
 defichain/exceptions/http/BadRequest.py
 defichain/exceptions/http/Forbidden.py
 defichain/exceptions/http/HTTPStatusCode.py
 defichain/exceptions/http/InternalServerError.py
 defichain/exceptions/http/NotFound.py
@@ -36,17 +38,18 @@
 defichain/exceptions/transactions/rawtransactionerror.py
 defichain/exceptions/transactions/tokenerror.py
 defichain/exceptions/transactions/txbuildererror.py
 defichain/exceptions/transactions/verifyerror.py
 defichain/hdwallet/__init__.py
 defichain/hdwallet/account.py
 defichain/hdwallet/derivations.py
-defichain/hdwallet/encryption.py
+defichain/hdwallet/encrypt.py
 defichain/hdwallet/utils.py
 defichain/hdwallet/wallet.py
+defichain/libs/__init__.py
 defichain/libs/base58.py
 defichain/libs/bech32.py
 defichain/libs/ecc.py
 defichain/libs/ripemd160.py
 defichain/mnemonic/__init__.py
 defichain/mnemonic/mnemonic.py
 defichain/mnemonic/wordlist/__init__.py
@@ -61,18 +64,18 @@
 defichain/networks/__init__.py
 defichain/networks/networks.py
 defichain/node/RPCErrorHandler.py
 defichain/node/__init__.py
 defichain/node/node.py
 defichain/node/rpc.py
 defichain/node/util.py
+defichain/node/modules/__init__.py
 defichain/node/modules/accounts.py
 defichain/node/modules/blockchain.py
 defichain/node/modules/control.py
-defichain/node/modules/evm.py
 defichain/node/modules/generating.py
 defichain/node/modules/loan.py
 defichain/node/modules/masternodes.py
 defichain/node/modules/mining.py
 defichain/node/modules/network.py
 defichain/node/modules/oracles.py
 defichain/node/modules/poolpair.py
@@ -85,14 +88,15 @@
 defichain/node/modules/vault.py
 defichain/node/modules/wallet.py
 defichain/node/modules/zmq.py
 defichain/ocean/OceanErrorHandler.py
 defichain/ocean/__init__.py
 defichain/ocean/connection.py
 defichain/ocean/ocean.py
+defichain/ocean/modules/__init__.py
 defichain/ocean/modules/address.py
 defichain/ocean/modules/blocks.py
 defichain/ocean/modules/consortium.py
 defichain/ocean/modules/fee.py
 defichain/ocean/modules/governance.py
 defichain/ocean/modules/loan.py
 defichain/ocean/modules/masternodes.py
```

