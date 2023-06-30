# Comparing `tmp/bbot-1.0.5.1665rc0.tar.gz` & `tmp/bbot-1.0.5.1793rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1665rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1793rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1665rc0.tar` & `bbot-1.0.5.1793rc0.tar`

### file list

```diff
@@ -1,182 +1,277 @@
--rw-r--r--   0        0        0    32473 2023-05-06 00:17:42.480626 bbot-1.0.5.1665rc0/LICENSE
--rw-r--r--   0        0        0    51011 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/README.md
--rw-r--r--   0        0        0      211 2023-05-06 00:18:05.401001 bbot-1.0.5.1665rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     6536 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      376 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    13693 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8920 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     4261 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      632 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    30910 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1498 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3644 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1256 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     2875 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     6940 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    13841 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     8540 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    29454 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     4286 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5435 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1414 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    29037 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14848 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9574 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     2919 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/queueing.py
--rw-r--r--   0        0        0     1890 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     8474 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/threadpool.py
--rw-r--r--   0        0        0     3987 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3193 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0     9324 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    10967 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     7859 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3794 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1371 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3461 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2350 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    26022 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2197 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1225 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5502 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1065 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      847 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1167 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2169 2023-05-06 00:17:42.484626 bbot-1.0.5.1665rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4550 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5107 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1116 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     5432 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      732 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     5001 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1160 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13578 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15617 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5763 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2516 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2954 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2862 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      866 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11117 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2164 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1093 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7290 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     2723 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10120 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      658 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7395 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5490 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7748 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     1944 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9438 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      298 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16587 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     4773 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1274 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2037 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0      707 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11237 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    14828 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4245 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     4867 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11137 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1379 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2595 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1809 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1836 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1047 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1255 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      204 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3649 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     1747 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1532 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1620 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5360 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1533 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1310 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      746 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1584 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8262 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      742 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2255 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2578 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1071 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1198 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1432 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1607 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1527 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     8014 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6077 2023-05-06 00:17:42.488626 bbot-1.0.5.1665rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11235 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      566 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3819 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2759 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2458 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1158 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1569 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1169 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2190 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2095 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      427 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    26264 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    22025 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4038 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    18609 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0      559 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0     2545 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/helpers.py
--rw-r--r--   0        0        0    74299 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/modules_test_classes.py
--rw-r--r--   0        0        0       15 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/pytest.ini
--rwxr-xr-x   0        0        0      578 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0      904 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_1/test_before_patching.py
--rw-r--r--   0        0        0     5859 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_1/test_modules_full.py
--rw-r--r--   0        0        0        0 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0      588 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_agent.py
--rw-r--r--   0        0        0     4739 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_cli.py
--rw-r--r--   0        0        0      932 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_cloud_helpers.py
--rw-r--r--   0        0        0      462 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_config.py
--rw-r--r--   0        0        0      722 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_depsinstaller.py
--rw-r--r--   0        0        0    15064 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_events.py
--rw-r--r--   0        0        0    34798 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_helpers.py
--rw-r--r--   0        0        0     7171 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_manager.py
--rw-r--r--   0        0        0    11616 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_modules_basic.py
--rw-r--r--   0        0        0      789 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_python_api.py
--rw-r--r--   0        0        0     3215 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_scan.py
--rw-r--r--   0        0        0     1395 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_scope.py
--rw-r--r--   0        0        0     2163 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_target.py
--rw-r--r--   0        0        0      707 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_threadpool.py
--rw-r--r--   0        0        0      476 2023-05-06 00:17:42.492627 bbot-1.0.5.1665rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-05-06 00:17:42.500627 bbot-1.0.5.1665rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-05-06 00:17:42.500627 bbot-1.0.5.1665rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-05-06 00:17:42.500627 bbot-1.0.5.1665rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-05-06 00:17:42.500627 bbot-1.0.5.1665rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1338 2023-05-06 00:18:05.401001 bbot-1.0.5.1665rc0/pyproject.toml
--rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1665rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/LICENSE
+-rw-r--r--   0        0        0    51778 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/README.md
+-rw-r--r--   0        0        0      211 2023-06-30 15:28:26.133301 bbot-1.0.5.1793rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14606 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8720 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5150 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31058 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1496 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     1993 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5022 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9234 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    27284 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4373 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    32311 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14831 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     1929 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-06-30 15:28:02.769189 bbot-1.0.5.1793rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3192 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    13205 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8300 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3786 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3491 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2600 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25482 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5461 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4760 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5125 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     2636 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      680 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5520 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13670 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15857 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2539 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11304 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1307 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      807 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7437 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5749 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7754 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9552 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16933 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5124 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1292 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    15167 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4269 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     5248 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     4993 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-06-30 15:28:02.773189 bbot-1.0.5.1793rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11391 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1820 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1426 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1493 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5331 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8302 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2273 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1744 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7882 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11359 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3843 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1711 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2291 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    24694 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27042 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10812 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     2668 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1086 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0    15109 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    24751 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7959 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     7688 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     2664 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     6570 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 15:28:02.777189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     1886 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1949 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     2069 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     1770 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      555 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0      972 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1726 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0      419 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
+-rw-r--r--   0        0        0      659 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1116 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     1160 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     1614 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0     1596 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     1673 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      611 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     5562 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2370 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-06-30 15:28:02.781189 bbot-1.0.5.1793rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-06-30 15:28:02.789189 bbot-1.0.5.1793rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-06-30 15:28:02.789189 bbot-1.0.5.1793rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-06-30 15:28:02.789189 bbot-1.0.5.1793rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-06-30 15:28:02.789189 bbot-1.0.5.1793rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1537 2023-06-30 15:28:26.133301 bbot-1.0.5.1793rc0/pyproject.toml
+-rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1793rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1665rc0/LICENSE` & `bbot-1.0.5.1793rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/README.md` & `bbot-1.0.5.1793rc0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,44 @@
-![bbot_banner](https://user-images.githubusercontent.com/20261699/158000235-6c1ace81-a267-4f8e-90a1-f4c16884ebac.png)
-
 # BEE·bot
 ### OSINT automation for hackers.
 
-~~~bash
-pip install bbot
-~~~
+[![Python Version](https://img.shields.io/badge/python-3.9+-FF8400)](https://www.python.org) [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License](https://img.shields.io/badge/license-GPLv3-FF8400.svg)](https://github.com/blacklanternsecurity/bbot/blob/dev/LICENSE) [![Tests](https://github.com/blacklanternsecurity/bbot/actions/workflows/tests.yml/badge.svg?branch=stable)](https://github.com/blacklanternsecurity/bbot/actions?query=workflow%3A"tests") [![Codecov](https://codecov.io/gh/blacklanternsecurity/bbot/branch/dev/graph/badge.svg?token=IR5AZBDM5K)](https://codecov.io/gh/blacklanternsecurity/bbot) [![Discord](https://img.shields.io/discord/859164869970362439)](https://discord.com/invite/PZqkgxu5SA)
 
-[![Python Version](https://img.shields.io/badge/python-3.9+-FF8400)](https://www.python.org) [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License](https://img.shields.io/badge/license-GPLv3-FF8400.svg)](https://github.com/blacklanternsecurity/bbot/blob/dev/LICENSE) [![Tests](https://github.com/blacklanternsecurity/bbot/actions/workflows/tests.yml/badge.svg?branch=stable)](https://github.com/blacklanternsecurity/bbot/actions?query=workflow%3A"tests") [![Codecov](https://codecov.io/gh/blacklanternsecurity/bbot/branch/dev/graph/badge.svg?token=IR5AZBDM5K)](https://codecov.io/gh/blacklanternsecurity/bbot)
+BBOT is a powerful and modular OSINT (Open Source Intelligence) framework designed to map the attack surface of an organization. With BBOT, you can execute the entire OSINT workflow with just a single command.
 
-![bbot-demo](https://user-images.githubusercontent.com/20261699/217346759-d5bf56c3-3936-43f7-ad14-4d73d2cd1417.gif)
+![bbot_banner](https://user-images.githubusercontent.com/20261699/158000235-6c1ace81-a267-4f8e-90a1-f4c16884ebac.png)
+
+BBOT is inspired by [Spiderfoot](https://github.com/smicallef/spiderfoot) but takes it to the next level with features like multi-target scans, lightning-fast asyncio performance, and NLP-powered subdomain mutations. It offers a wide range of functionality, including subdomain enumeration, port scanning, web screenshots, vulnerability scanning, and much more. BBOT has over 80 modules and counting.
 
-### **BBOT** is a **recursive**, **modular** OSINT framework inspired by Spiderfoot.
+Whether you're a pentester, security researcher, or bug bounty hunter, BBOT simplifies and automates the OSINT process so you can focus on the fun part: hacking!
 
-BBOT can execute the entire OSINT process in a single command: subdomain enumeration, port scans, web screenshots (with `gowitness`), vulnerability scanning (with `nuclei`), and much more. BBOT has over **80 modules** and counting.
+https://github.com/blacklanternsecurity/bbot/assets/20261699/ebf2a81e-7530-4a9e-922d-4e62eb949f35
 
-Read our [blog post](https://blog.blacklanternsecurity.com/p/subdomain-enumeration-tool-face-off) to find out why BBOT is the most thorough subdomain enumeration tool available.
+Visualization courtesy of [VivaGraphJS](https://github.com/blacklanternsecurity/bbot-vivagraphjs)
 
-![graphs-small](https://user-images.githubusercontent.com/20261699/199602154-14c71a93-57aa-4ac0-ad81-87ce64fbffc7.png)
+# Getting Started
 
 ## Installation ([pip](https://pypi.org/project/bbot/))
-Note: installing in a virtualenv (e.g. via `pipx`) is recommended
+Note: installing in a virtualenv (e.g. via `pipx`) is recommended. If you need help with installation, please refer to the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#installation).
 ~~~bash
+# Prerequisites:
+# - Linux (Windows and macOS are *not* supported)
+# - Python 3.9 or newer
+
 # stable version
 pip install bbot
 
 # bleeding edge (dev branch)
 pip install --pre bbot
 
 bbot --help
 ~~~
-Prerequisites:
-- Linux (Windows and macOS are *not* supported)
-- Python 3.9 or newer
-
-## Installation ([Docker](https://hub.docker.com/r/blacklanternsecurity/bbot))
-~~~bash
-# bleeding edge (dev)
-docker run -it blacklanternsecurity/bbot --help
-
-# stable
-docker run -it blacklanternsecurity/bbot:stable --help
-
-# note: alternatively there is a helper script that will map docker volumes to persist your BBOT scan data:
-./bbot-docker.sh --help
-~~~
 
-If you need help with installation, please refer to the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#installation).
-
-See also: [Release History](https://github.com/blacklanternsecurity/bbot/wiki/Release-History)
-
-## Scanning with BBOT
-
-### Examples
+## Example Commands
+Note: Scan output, logs, etc. are saved to `~/.bbot`.
 ~~~bash
 # subdomains
 bbot -t evilcorp.com -f subdomain-enum
 
 # subdomains (passive only)
 bbot -t evilcorp.com -f subdomain-enum -rf passive
 
@@ -73,15 +55,39 @@
 # subdomains + emails + cloud + port scan + non-intrusive web + web screenshots + nuclei
 bbot -t evilcorp.com -f subdomain-enum email-enum cloud-enum web-basic -m naabu gowitness nuclei --allow-deadly
 
 # list modules
 bbot -l
 ~~~
 
-### Targets
+## Using BBOT as a Python library
+**Synchronous**
+~~~python
+from bbot.scanner import Scanner
+
+# any number of targets can be specified
+scan = Scanner("example.com", "scanme.nmap.org", modules=["nmap", "sslcert"])
+for event in scan.start():
+    print(event.json())
+~~~
+
+**Asynchronous**
+~~~python
+from bbot.scanner import Scanner
+
+async def main():
+    scan = Scanner("example.com", "scanme.nmap.org", modules=["nmap", "sslcert"])
+    async for event in scan.async_start():
+        print(event.json())
+
+import asyncio
+asyncio.run(main())
+~~~
+
+## Targets
 
 Targets seed a scan with initial data. You can specify an unlimited number of targets, either directly on the command line or in files (or both!). Targets can be any of the following:
 
 - DNS_NAME (`evilcorp.com`)
 - IP_ADDRESS (`1.2.3.4`)
 - IP_RANGE (`1.2.3.0/24`)
 - URL (`https://www.evilcorp.com`)
@@ -90,122 +96,82 @@
 For example, the following scan is totally valid:
 
 ~~~bash
 # multiple targets
 bbot -t evilcorp.com evilcorp.co.uk http://www.evilcorp.cn 1.2.3.0/24 other_targets.txt
 ~~~
 
-#### Whitelists / Blacklists
-
-BBOT's whitelist determines what's considered to be in-scope. By default, the whitelist is simply your target. But if you want more granular scope control, you can override it with `--whitelist` (or add a `--blacklist`).
-
-~~~bash
-# seed a scan with two domains, but only consider assets to be in scope if they are inside 1.2.3.0/24
-bbot -t evilcorp.com evilcorp.co.uk --whitelist 1.2.3.0/24 --blacklist test.evilcorp.com 1.2.3.4 blacklist.txt
-~~~
-
 Visit the wiki for more [tips and tricks](https://github.com/blacklanternsecurity/bbot/wiki#tips-and-tricks).
 
-## Using BBOT as a Python library
-~~~python
-from bbot.scanner import Scanner
-
-# any number of targets can be specified
-scan = Scanner("evilcorp.com", "evilcorp.co.uk", modules=["httpx", "sslcert"])
-for event in scan.start():
-    print(event.json())
-~~~
-
-# Output
-By default, BBOT saves its output in TXT, JSON, and CSV formats. To enable more output modules, you can use `--output-module`.
+## [Docker](https://hub.docker.com/r/blacklanternsecurity/bbot)
+BBOT provides docker images, along with helper script `bbot-docker.sh` to persist your BBOT scan data.
 ~~~bash
-# tee to a file
-bbot -f subdomain-enum -t evilcorp.com | tee evilcorp.txt
+# helper script
+./bbot-docker.sh --help
 
-# output to JSON
-bbot --output-module json -f subdomain-enum -t evilcorp.com | jq
+# bleeding edge (dev)
+docker run -it blacklanternsecurity/bbot --help
 
-# output asset inventory in current directory
-bbot -o . --output-module asset_inventory -f subdomain-enum -t evilcorp.com
+# stable
+docker run -it blacklanternsecurity/bbot:stable --help
 ~~~
-For every scan, BBOT generates a unique and mildly-entertaining name like `demonic_jimmy`. Output for that scan, including the word cloud and any gowitness screenshots, etc., are saved to a folder by that name in `~/.bbot/scans`. The most recent 20 scans are kept, and older ones are removed. You can change the location of BBOT's output with `--output`, and you can also pick a custom scan name with `--name`.
 
-If you reuse a scan name, it will append to its original output files and leverage the previous word cloud.
-
-# Neo4j
-Neo4j is the funnest (and prettiest) way to view and interact with BBOT data.
-
-![neo4j](https://user-images.githubusercontent.com/20261699/182398274-729f3c48-c23c-4db0-8c2e-8b403c1bf790.png)
-
-- You can get Neo4j up and running with a single docker command:
-~~~bash
-docker run -p 7687:7687 -p 7474:7474 -v "$(pwd)/data/:/data/" -e NEO4J_AUTH=neo4j/bbotislife neo4j
-~~~
-- After that, run bbot with `--output-modules neo4j`
-~~~bash
-bbot -f subdomain-enum -t evilcorp.com --output-modules neo4j
-~~~
-- Browse data at http://localhost:7474
 
 # Usage
 ~~~
 $ bbot --help
-usage: bbot [-h] [--help-all] [-t TARGET [TARGET ...]] [-w WHITELIST [WHITELIST ...]] [-b BLACKLIST [BLACKLIST ...]] [--strict-scope] [-n SCAN_NAME] [-m MODULE [MODULE ...]] [-l] [-em MODULE [MODULE ...]]
-            [-f FLAG [FLAG ...]] [-rf FLAG [FLAG ...]] [-ef FLAG [FLAG ...]] [-om MODULE [MODULE ...]] [-o DIR] [-c [CONFIG ...]] [--allow-deadly] [-v] [-d] [-s] [--force] [-y] [--dry-run] [--current-config]
-            [--save-wordcloud FILE] [--load-wordcloud FILE] [--no-deps | --force-deps | --retry-deps | --ignore-failed-deps | --install-all-deps] [-a] [--version]
+usage: bbot [-h] [--help-all] [-t TARGET [TARGET ...]] [-w WHITELIST [WHITELIST ...]] [-b BLACKLIST [BLACKLIST ...]] [--strict-scope] [-m MODULE [MODULE ...]] [-l]
+            [-em MODULE [MODULE ...]] [-f FLAG [FLAG ...]] [-rf FLAG [FLAG ...]] [-ef FLAG [FLAG ...]] [-om MODULE [MODULE ...]] [--allow-deadly] [-n SCAN_NAME] [-o DIR] [-c [CONFIG ...]]
+            [-v] [-d] [-s] [--force] [-y] [--dry-run] [--current-config] [--no-deps | --force-deps | --retry-deps | --ignore-failed-deps | --install-all-deps] [-a] [--version]
 
 Bighuge BLS OSINT Tool
 
 options:
   -h, --help            show this help message and exit
   --help-all            Display full help including module config options
-  -n SCAN_NAME, --name SCAN_NAME
-                        Name of scan (default: random)
+
+Target:
+  -t TARGET [TARGET ...], --targets TARGET [TARGET ...]
+                        Targets to seed the scan
+  -w WHITELIST [WHITELIST ...], --whitelist WHITELIST [WHITELIST ...]
+                        What's considered in-scope (by default it's the same as --targets)
+  -b BLACKLIST [BLACKLIST ...], --blacklist BLACKLIST [BLACKLIST ...]
+                        Don't touch these things
+  --strict-scope        Don't consider subdomains of target/whitelist to be in-scope
+
+Modules:
   -m MODULE [MODULE ...], --modules MODULE [MODULE ...]
-                        Modules to enable. Choices: affiliates,anubisdb,asn,azure_tenant,badsecrets,bevigil,binaryedge,bucket_aws,bucket_azure,bucket_digitalocean,bucket_firebase,bucket_gcp,builtwith,bypass403,c99,censys,certspotter,crobat,crt,dnscommonsrv,dnsdumpster,dnszonetransfer,emailformat,ffuf,ffuf_shortnames,fingerprintx,fullhunt,generic_ssrf,github,gowitness,hackertarget,host_header,httpx,hunt,hunterio,iis_shortnames,ipneighbor,ipstack,leakix,masscan,massdns,naabu,ntlm,nuclei,otx,paramminer_cookies,paramminer_getparams,paramminer_headers,passivetotal,pgp,rapiddns,riddler,robots,secretsdb,securitytrails,shodan_dns,skymem,smuggler,social,sslcert,subdomain_hijack,sublist3r,telerik,threatminer,url_manipulation,urlscan,vhost,viewdns,virustotal,wafw00f,wappalyzer,wayback,zoomeye
+                        Modules to enable. Choices: affiliates,anubisdb,asn,azure_tenant,badsecrets,bevigil,binaryedge,bucket_aws,bucket_azure,bucket_digitalocean,bucket_firebase,bucket_gcp,builtwith,bypass403,c99,censys,certspotter,crobat,crt,dnscommonsrv,dnsdumpster,dnszonetransfer,emailformat,ffuf,ffuf_shortnames,fingerprintx,fullhunt,generic_ssrf,github,gowitness,hackertarget,host_header,httpx,hunt,hunterio,iis_shortnames,ipneighbor,ipstack,leakix,masscan,massdns,naabu,nmap,ntlm,nuclei,otx,paramminer_cookies,paramminer_getparams,paramminer_headers,passivetotal,pgp,rapiddns,riddler,robots,secretsdb,securitytrails,shodan_dns,skymem,smuggler,social,sslcert,subdomain_hijack,sublist3r,telerik,threatminer,url_manipulation,urlscan,vhost,viewdns,virustotal,wafw00f,wappalyzer,wayback,zoomeye
   -l, --list-modules    List available modules.
   -em MODULE [MODULE ...], --exclude-modules MODULE [MODULE ...]
                         Exclude these modules.
   -f FLAG [FLAG ...], --flags FLAG [FLAG ...]
                         Enable modules by flag. Choices: active,affiliates,aggressive,cloud-enum,deadly,email-enum,iis-shortnames,passive,portscan,report,safe,service-enum,slow,social-enum,subdomain-enum,subdomain-hijack,web-basic,web-paramminer,web-screenshots,web-thorough
   -rf FLAG [FLAG ...], --require-flags FLAG [FLAG ...]
-                        Disable modules that don't have these flags (e.g. -rf passive)
+                        Only enable modules with these flags (e.g. -rf passive)
   -ef FLAG [FLAG ...], --exclude-flags FLAG [FLAG ...]
                         Disable modules with these flags. (e.g. -ef aggressive)
   -om MODULE [MODULE ...], --output-modules MODULE [MODULE ...]
                         Output module(s). Choices: asset_inventory,csv,http,human,json,neo4j,python,web_report,websocket
+  --allow-deadly        Enable the use of highly aggressive modules
+
+Scan:
+  -n SCAN_NAME, --name SCAN_NAME
+                        Name of scan (default: random)
   -o DIR, --output-dir DIR
   -c [CONFIG ...], --config [CONFIG ...]
                         custom config file, or configuration options in key=value format: 'modules.shodan.api_key=1234'
-  --allow-deadly        Enable the use of highly aggressive modules
   -v, --verbose         Be more verbose
   -d, --debug           Enable debugging
   -s, --silent          Be quiet
   --force               Run scan even if module setups fail
   -y, --yes             Skip scan confirmation prompt
   --dry-run             Abort before executing scan
   --current-config      Show current config in YAML format
 
-Target:
-  -t TARGET [TARGET ...], --targets TARGET [TARGET ...]
-                        Targets to seed the scan
-  -w WHITELIST [WHITELIST ...], --whitelist WHITELIST [WHITELIST ...]
-                        What's considered in-scope (by default it's the same as --targets)
-  -b BLACKLIST [BLACKLIST ...], --blacklist BLACKLIST [BLACKLIST ...]
-                        Don't touch these things
-  --strict-scope        Don't consider subdomains of target/whitelist to be in-scope
-
-Word cloud:
-  Save/load wordlist of common words gathered during a scan
-
-  --save-wordcloud FILE
-                        Output wordcloud to custom file when the scan completes
-  --load-wordcloud FILE
-                        Load wordcloud from a custom file
-
 Module dependencies:
   Control how modules install their dependencies
 
   --no-deps             Don't install module dependencies
   --force-deps          Force install all module dependencies
   --retry-deps          Try again to install failed module dependencies
   --ignore-failed-deps  Run modules even if they have failed dependencies
@@ -216,20 +182,21 @@
 
   -a, --agent-mode      Start in agent mode
 
 Misc:
   --version             show BBOT version and exit
 ~~~
 
+
 # BBOT Config
-BBOT loads its config from these places in the following order:
+Additional config options (such as API keys, rate limits, user-agent, etc.) can be passed to BBOT via its YAML config. BBOT loads its config beginning from `~/.config/bbot`:
 
 - `~/.config/bbot/bbot.yml` <-- Use this one as your main config
 - `~/.config/bbot/secrets.yml` <-- Use this one for sensitive stuff like API keys
-- command line (`--config`)
+- command line (`--config`) <-- Use this to specify a custom `.yml` or override individual config options
 
 These config files will be automatically created for you when you first run BBOT.
 
 Command-line arguments take precedence over all others. You can give BBOT a custom config file with `--config myconf.yml`, or individual arguments like this: `--config http_proxy=http://127.0.0.1:8080 modules.shodan_dns.api_key=1234`. To display the full and current BBOT config, including any command-line arguments, use `bbot --current-config`.
 
 Note that placing the following in `bbot.yml`:
 ```yaml
@@ -240,14 +207,47 @@
 Is the same as:
 ```bash
 bbot --config modules.shodan.api_key=deadbeef
 ```
 
 For explanations of config options, see `defaults.yml` or the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#yaml-config)
 
+
+# Output
+By default, BBOT saves its output in TXT, JSON, and CSV formats. You can enable other output modules with `--output-module`.
+~~~bash
+# tee to a file
+bbot -f subdomain-enum -t evilcorp.com | tee evilcorp.txt
+
+# output to JSON
+bbot --output-module json -f subdomain-enum -t evilcorp.com | jq
+
+# output asset inventory in current directory
+bbot -o . --output-module asset_inventory -f subdomain-enum -t evilcorp.com
+~~~
+For every scan, BBOT generates a unique and mildly-entertaining name like `demonic_jimmy`. Output for that scan, including scan stats and any gowitness screenshots, etc., are saved to a folder by that name in `~/.bbot/scans`. The most recent 20 scans are kept, and older ones are removed. You can change the location of BBOT's output with `--output`, and you can also pick a custom scan name with `--name`.
+
+If you reuse a scan name, it will append to its original output files and leverage the previous.
+
+## Neo4j
+Neo4j is the funnest (and prettiest) way to view and interact with BBOT data.
+
+![neo4j](https://user-images.githubusercontent.com/20261699/182398274-729f3c48-c23c-4db0-8c2e-8b403c1bf790.png)
+
+- You can get Neo4j up and running with a single docker command:
+~~~bash
+docker run -p 7687:7687 -p 7474:7474 -v "$(pwd)/data/:/data/" -e NEO4J_AUTH=neo4j/bbotislife neo4j
+~~~
+- After that, run bbot with `--output-modules neo4j`
+~~~bash
+bbot -f subdomain-enum -t evilcorp.com --output-modules neo4j
+~~~
+- Browse data at http://localhost:7474
+
+
 # Modules
 
 ### Note: You can find more fun and interesting modules at the [Module Playground](https://github.com/blacklanternsecurity/bbot-module-playground). For instructions on how to install these other modules, see the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#module-playground).
 
 To see modules' options (how to change wordlists, thread count, etc.), use `--help-all`.
 
 ~~~
@@ -304,14 +304,16 @@
 | iis_shortnames       | scan     |         | Check for IIS shortname vulnerability    | active,iis-shortnames,safe,web-          | URL_HINT                                 |
 |                      |          |         |                                          | basic,web-thorough                       |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | masscan              | scan     |         | Port scan IP subnets with masscan        | active,aggressive,portscan               | OPEN_TCP_PORT                            |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | naabu                | scan     |         | Execute port scans with naabu            | active,aggressive,portscan,web-thorough  | OPEN_TCP_PORT                            |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
+| nmap                 | scan     |         | Execute port scans with nmap             | active,aggressive,portscan,web-thorough  | OPEN_TCP_PORT                            |
++----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | ntlm                 | scan     |         | Watch for HTTP endpoints that support    | active,safe,web-basic,web-thorough       | DNS_NAME,FINDING                         |
 |                      |          |         | NTLM authentication                      |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | nuclei               | scan     |         | Fast and customisable vulnerability      | active,aggressive,deadly                 | FINDING,VULNERABILITY                    |
 |                      |          |         | scanner                                  |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | paramminer_cookies   | scan     |         | Smart brute-force to check for common    | active,aggressive,slow,web-paramminer    | FINDING                                  |
@@ -349,15 +351,15 @@
 | vhost                | scan     |         | Fuzz for virtual hosts                   | active,aggressive,deadly,slow            | DNS_NAME,VHOST                           |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | wafw00f              | scan     |         | Web Application Firewall Fingerprinting  | active,aggressive                        | WAF                                      |
 |                      |          |         | Tool                                     |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | wappalyzer           | scan     |         | Extract technologies from web responses  | active,safe,web-basic,web-thorough       | TECHNOLOGY                               |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
-| affiliates           | scan     |         | Summarize affiliate domains at the end   | passive,report,safe                      |                                          |
+| affiliates           | scan     |         | Summarize affiliate domains at the end   | affiliates,passive,report,safe           |                                          |
 |                      |          |         | of a scan                                |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | anubisdb             | scan     |         | Query jldc.me's database for subdomains  | passive,safe,subdomain-enum              | DNS_NAME                                 |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | asn                  | scan     |         | Query ripe and bgpview.io for ASNs       | passive,report,safe,subdomain-enum       | ASN                                      |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | azure_tenant         | scan     |         | Query Azure for tenant sister domains    | affiliates,passive,safe,subdomain-enum   | DNS_NAME                                 |
@@ -438,15 +440,15 @@
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | virustotal           | scan     | X       | Query VirusTotal's API for subdomains    | passive,safe,subdomain-enum              | DNS_NAME                                 |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | wayback              | scan     |         | Query archive.org's API for subdomains   | passive,safe,subdomain-enum              | DNS_NAME,URL_UNVERIFIED                  |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | zoomeye              | scan     | X       | Query ZoomEye's API for subdomains       | affiliates,passive,safe,subdomain-enum   | DNS_NAME                                 |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
-| asset_inventory      | output   |         | Output to an asset inventory style       |                                          |                                          |
+| asset_inventory      | output   |         | Output to an asset inventory style       |                                          | IP_ADDRESS,OPEN_TCP_PORT                 |
 |                      |          |         | flattened CSV file                       |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | csv                  | output   |         | Output to CSV                            |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | http                 | output   |         | Send every event to a custom URL via a   |                                          |                                          |
 |                      |          |         | web request                              |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
@@ -469,16 +471,29 @@
 |                      |          |         | scan data                                |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | speculate            | internal |         | Derive certain event types from others   | passive                                  | DNS_NAME,FINDING,IP_ADDRESS,OPEN_TCP_POR |
 |                      |          |         | by common sense                          |                                          | T                                        |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 ~~~
 
-# Credit
 
-BBOT is written by @TheTechromancer. Web hacking in BBOT is made possible by @liquidsec, who wrote most of the web modules and helpers.
+# Acknowledgements
 
-Very special thanks to the following people who made BBOT possible:
+Thanks to all these amazing people for contributing to BBOT! :heart:
 
-- @kerrymilan for his Neo4j and Ansible expertise
+If you have an idea for a feature or run into bugs of any kind, please submit an issue or a PR. We welcome contributions!
+
+<p align="center">
+<a href="https://github.com/blacklanternsecurity/bbot/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=blacklanternsecurity/bbot&max=500">
+</a>
+</p>
+
+Special thanks to the following people who made BBOT possible:
+
+- @TheTechromancer for creating BBOT
+- @liquidsec for his extensive work on BBOT's web hacking features
 - Steve Micallef (@smicallef) for creating Spiderfoot
+- @kerrymilan for his Neo4j and Ansible expertise
 - Aleksei Kornev (@alekseiko) for allowing us ownership of the bbot Pypi repository <3
+
+See also: [Release History](https://github.com/blacklanternsecurity/bbot/wiki/Release-History)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/agent/agent.py` & `bbot-1.0.5.1793rc0/bbot/agent/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,186 +1,195 @@
 import json
+import asyncio
 import logging
-import threading
 import traceback
-import websocket
-from time import sleep
+import websockets
 from omegaconf import OmegaConf
 
 from . import messages
 import bbot.core.errors
 from bbot.scanner import Scanner
 from bbot.scanner.dispatcher import Dispatcher
+from bbot.core.helpers.misc import urlparse, split_host_port
+from bbot.core.configurator.environ import prepare_environment
 
 log = logging.getLogger("bbot.core.agent")
 
 
 class Agent:
     def __init__(self, config):
         self.config = config
+        prepare_environment(self.config)
         self.url = self.config.get("agent_url", "")
+        self.parsed_url = urlparse(self.url)
+        self.host, self.port = split_host_port(self.parsed_url.netloc)
         self.token = self.config.get("agent_token", "")
         self.scan = None
-        self.thread = None
-        self._scan_lock = threading.Lock()
+        self.task = None
+        self._ws = None
+        self._scan_lock = asyncio.Lock()
 
         self.dispatcher = Dispatcher()
         self.dispatcher.on_status = self.on_scan_status
         self.dispatcher.on_finish = self.on_scan_finish
 
     def setup(self):
-        websocket.enableTrace(False)
         if not self.url:
             log.error(f"Must specify agent_url")
             return False
         if not self.token:
             log.error(f"Must specify agent_token")
             return False
-        self.ws = websocket.WebSocketApp(
-            f"{self.url}/control/",
-            on_open=self.on_open,
-            on_message=self.on_message,
-            on_error=self.on_error,
-            on_close=self.on_close,
-            header={"Authorization": f"Bearer {self.token}"},
-        )
         return True
 
-    def start(self):
-        not_keyboardinterrupt = False
+    async def ws(self, rebuild=False):
+        if self._ws is None or rebuild:
+            kwargs = {"close_timeout": 0.5}
+            if self.token:
+                kwargs.update({"extra_headers": {"Authorization": f"Bearer {self.token}"}})
+            verbs = ("Building", "Built")
+            if rebuild:
+                verbs = ("Rebuilding", "Rebuilt")
+            log.debug(f"{verbs[0]} websocket connection to {self.url}")
+            self._ws = await websockets.connect(self.url, **kwargs)
+            log.debug(f"{verbs[1]} websocket connection to {self.url}")
+        return self._ws
+
+    async def start(self):
+        rebuild = False
         while 1:
-            not_keyboardinterrupt = self.ws.run_forever()
-            if not not_keyboardinterrupt:
-                break
-            sleep(1)
+            ws = await self.ws(rebuild=rebuild)
+            rebuild = False
+            try:
+                message = await ws.recv()
+                log.debug(f"Got message: {message}")
+                try:
+                    message = json.loads(message)
+                    message = messages.Message(**message)
+
+                    if message.command == "ping":
+                        if self.scan is None:
+                            await self.send({"conversation": str(message.conversation), "message_type": "pong"})
+
+                    command_type = getattr(messages, message.command, None)
+                    if command_type is None:
+                        log.warning(f'Invalid command: "{message.command}"')
+                        continue
+
+                    command_args = command_type(**message.arguments)
+                    command_fn = getattr(self, message.command)
+                    response = await self.err_handle(command_fn, **command_args.dict())
+                    log.info(str(response))
+                    await self.send({"conversation": str(message.conversation), "message": response})
+
+                except json.decoder.JSONDecodeError as e:
+                    log.warning(f'Failed to decode message "{message}": {e}')
+                    log.trace(traceback.format_exc())
+                    continue
+            except Exception as e:
+                log.debug(f"Error receiving message: {e}")
+                log.debug(traceback.format_exc())
+                await asyncio.sleep(1)
+                rebuild = True
 
-    def send(self, message):
+    async def send(self, message):
+        rebuild = False
         while 1:
             try:
-                self.ws.send(json.dumps(message))
+                ws = await self.ws(rebuild=rebuild)
+                j = json.dumps(message)
+                log.debug(f"Sending message of length {len(message)}")
+                await ws.send(j)
+                rebuild = False
                 break
             except Exception as e:
-                if getattr(self.scan, "stopping", True):
-                    break
                 log.warning(f"Error sending message: {e}, retrying")
                 log.trace(traceback.format_exc())
-                sleep(1)
+                await asyncio.sleep(1)
+                # rebuild = True
 
-    def on_message(self, ws, message):
-        try:
-            message = json.loads(message)
-        except Exception as e:
-            log.warning(f'Failed to JSON-decode message "{message}": {e}')
-            return
-        message = messages.Message(**message)
-
-        if message.command == "ping":
-            if self.scan is None:
-                self.send({"conversation": str(message.conversation), "message_type": "pong"})
-            return
-
-        command_type = None
-        try:
-            command_type = getattr(messages, message.command)
-        except AttributeError:
-            log.warning(f'Invalid command: "{message.command}"')
-
-        command_args = command_type(**message.arguments)
-        command_fn = getattr(self, message.command)
-        response = self.err_handle(command_fn, **command_args.dict())
-        log.info(str(response))
-        self.send({"conversation": str(message.conversation), "message": response})
-
-    def on_error(self, ws, error):
-        log.warning(f"on_error: {error}")
-
-    def on_close(self, ws, close_status_code, close_msg):
-        log.warning("Closed connection")
-
-    def on_open(self, ws):
-        log.success("Opened connection")
-
-    def start_scan(self, scan_id="", targets=[], modules=[], output_modules=[], config={}):
-        with self._scan_lock:
+    async def start_scan(self, scan_id, name=None, targets=[], modules=[], output_modules=[], config={}):
+        async with self._scan_lock:
             if self.scan is None:
                 log.success(
                     f"Starting scan with targets={targets}, modules={modules}, output_modules={output_modules}"
                 )
                 output_module_config = OmegaConf.create(
                     {"output_modules": {"websocket": {"url": f"{self.url}/scan/{scan_id}/", "token": self.token}}}
                 )
                 config = OmegaConf.create(config)
                 config = OmegaConf.merge(self.config, config, output_module_config)
                 output_modules = list(set(output_modules + ["websocket"]))
-                self.scan = Scanner(
+                scan = Scanner(
                     *targets,
                     scan_id=scan_id,
+                    name=name,
                     modules=modules,
                     output_modules=output_modules,
                     config=config,
                     dispatcher=self.dispatcher,
                 )
-                self.thread = threading.Thread(target=self._start_scan, args=(self.scan,), daemon=True)
-                self.thread.start()
+                self.task = asyncio.create_task(self._start_scan_task(scan))
 
-                return {"success": f"Started scan", "scan_id": self.scan.id}
+                return {"success": f"Started scan", "scan_id": scan.id}
             else:
                 msg = f"Scan {self.scan.id} already in progress"
                 log.warning(msg)
                 return {"error": msg, "scan_id": self.scan.id}
 
-    def stop_scan(self):
+    async def _start_scan_task(self, scan):
+        self.scan = scan
+        try:
+            await scan.async_start_without_generator()
+        except bbot.core.errors.ScanError as e:
+            log.error(f"Scan error: {e}")
+            log.trace(traceback.format_exc())
+        except Exception:
+            log.critical(f"Encountered error: {traceback.format_exc()}")
+            self.on_scan_status("FAILED", scan.id)
+        finally:
+            self.task = None
+
+    async def stop_scan(self):
         log.warning("Stopping scan")
         try:
-            with self._scan_lock:
+            async with self._scan_lock:
                 if self.scan is None:
                     msg = "Scan not in progress"
                     log.warning(msg)
                     return {"error": msg}
                 scan_id = str(self.scan.id)
-                self.scan.stop(wait=True)
+                self.scan.stop()
                 msg = f"Stopped scan {scan_id}"
                 log.warning(msg)
                 self.scan = None
                 return {"success": msg, "scan_id": scan_id}
         except Exception as e:
             log.warning(f"Error while stopping scan: {e}")
             log.trace(traceback.format_exc())
         finally:
             self.scan = None
-            self.thread = None
+            self.task = None
 
-    def scan_status(self):
-        with self._scan_lock:
+    async def scan_status(self):
+        async with self._scan_lock:
             if self.scan is None:
-                self.thread = None
                 msg = "Scan not in progress"
                 log.warning(msg)
                 return {"error": msg}
         return {"success": "Polled scan", "scan_status": self.scan.status}
 
-    def on_scan_status(self, status, scan_id):
-        self.send({"message_type": "scan_status_change", "status": str(status), "scan_id": scan_id})
+    async def on_scan_status(self, status, scan_id):
+        await self.send({"message_type": "scan_status_change", "status": str(status), "scan_id": scan_id})
 
-    def on_scan_finish(self, scan):
+    async def on_scan_finish(self, scan):
         self.scan = None
-        self.thread = None
+        self.task = None
 
-    @staticmethod
-    def err_handle(callback, *args, **kwargs):
+    async def err_handle(self, callback, *args, **kwargs):
         try:
-            return callback(*args, **kwargs)
+            return await callback(*args, **kwargs)
         except Exception as e:
             msg = f"Error in {callback.__qualname__}(): {e}"
             log.error(msg)
             log.trace(traceback.format_exc())
             return {"error": msg}
-
-    def _start_scan(self, scan):
-        try:
-            scan.start_without_generator()
-        except bbot.core.errors.ScanError as e:
-            log.error(f"Scan error: {e}")
-            log.trace(traceback.format_exc())
-        except Exception:
-            log.critical(f"Encountered error: {traceback.format_exc()}")
-            self.on_scan_status("FAILED", scan.id)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/cli.py` & `bbot-1.0.5.1793rc0/bbot/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import os
 import sys
+import asyncio
 import logging
 import threading
 import traceback
 from omegaconf import OmegaConf
 from contextlib import suppress
 
 # fix tee buffering
@@ -15,29 +16,58 @@
 from bbot.core.logger import get_log_level, toggle_log_level
 
 import bbot.core.errors
 from bbot import __version__
 from bbot.modules import module_loader
 from bbot.core.configurator.args import parser
 from bbot.core.helpers.logger import log_to_stderr
-from bbot.core.configurator import ensure_config_files, check_cli_args
+from bbot.core.configurator import ensure_config_files, check_cli_args, environ
 
 log = logging.getLogger("bbot.cli")
 sys.stdout.reconfigure(line_buffering=True)
 
 
 log_level = get_log_level()
 
 
 from . import config
 
 
-def main():
-    err = False
-    scan_name = ""
+err = False
+scan_name = ""
+
+
+async def _main():
+    global err
+    global scan_name
+    environ.cli_execution = True
+
+    # async def monitor_tasks():
+    #     in_row = 0
+    #     while 1:
+    #         try:
+    #             print('looooping')
+    #             tasks = asyncio.all_tasks()
+    #             current_task = asyncio.current_task()
+    #             if len(tasks) == 1 and list(tasks)[0] == current_task:
+    #                 print('no tasks')
+    #                 in_row += 1
+    #             else:
+    #                 in_row = 0
+    #             for t in tasks:
+    #                 print(t)
+    #             if in_row > 2:
+    #                 break
+    #             await asyncio.sleep(1)
+    #         except BaseException as e:
+    #             print(traceback.format_exc())
+    #             with suppress(BaseException):
+    #                 await asyncio.sleep(.1)
+
+    # monitor_tasks_task = asyncio.create_task(monitor_tasks())
 
     ensure_config_files()
 
     try:
         if len(sys.argv) == 1:
             parser.print_help()
             sys.exit(1)
@@ -61,15 +91,15 @@
 
         if options.agent_mode:
             from bbot.agent import Agent
 
             agent = Agent(config)
             success = agent.setup()
             if success:
-                agent.start()
+                await agent.start()
 
         else:
             from bbot.scanner import Scanner
 
             try:
                 module_filtering = False
                 if (options.list_modules or options.help_all) and not any([options.flags, options.modules]):
@@ -91,20 +121,16 @@
                 default_output_modules = ["human", "json", "csv"]
 
                 # Make a list of the modules which can be output to the console
                 consoleable_output_modules = [
                     k for k, v in module_loader.preloaded(type="output").items() if "console" in v["config"]
                 ]
 
-                # If no options are specified, use the default set
-                if not options.output_modules:
-                    options.output_modules = default_output_modules
-
                 # if none of the output modules provided on the command line are consoleable, don't turn off the defaults. Instead, just add the one specified to the defaults.
-                elif not any(o in consoleable_output_modules for o in options.output_modules):
+                if not any(o in consoleable_output_modules for o in options.output_modules):
                     options.output_modules += default_output_modules
 
                 scanner = Scanner(
                     *options.targets,
                     modules=list(modules),
                     output_modules=options.output_modules,
                     config=config,
@@ -114,17 +140,17 @@
                     strict_scope=options.strict_scope,
                     force_start=options.force,
                 )
 
                 if options.install_all_deps:
                     all_modules = list(module_loader.preloaded())
                     scanner.helpers.depsinstaller.force_deps = True
-                    scanner.helpers.depsinstaller.install(*all_modules)
+                    succeeded, failed = await scanner.helpers.depsinstaller.install(*all_modules)
                     log.info("Finished installing module dependencies")
-                    return
+                    return False if failed else True
 
                 scan_name = str(scanner.name)
 
                 # enable modules by dependency
                 # this is only a basic surface-level check
                 # todo: recursive dependency graph with networkx or topological sort?
                 all_modules = list(set(scanner._scan_modules + scanner._internal_modules + scanner._output_modules))
@@ -234,15 +260,15 @@
                         if "slow" in m[-1]["flags"]:
                             slow_modules.append(m[0])
                 if scanner._scan_modules:
                     if deadly_modules and not options.allow_deadly:
                         log.hugewarning(f"You enabled the following deadly modules: {','.join(deadly_modules)}")
                         log.hugewarning(f"Deadly modules are highly intrusive")
                         log.hugewarning(f"Please specify --allow-deadly to continue")
-                        return
+                        return False
                     if active_modules:
                         if active_modules:
                             if active_aggressive_modules:
                                 log.hugewarning(
                                     "This is an (aggressive) active scan! Intrusive connections will be made to target"
                                 )
                             else:
@@ -252,17 +278,17 @@
                     else:
                         log.hugeinfo("This is a passive scan. No connections will be made to target")
                     if slow_modules:
                         log.warning(
                             f"You have enabled the following slow modules: {','.join(slow_modules)}. Scan may take longer than usual"
                         )
 
-                scanner.helpers.word_cloud.load(options.load_wordcloud)
+                scanner.helpers.word_cloud.load()
 
-                scanner.prep()
+                await scanner.prep()
 
                 if not options.dry_run:
                     if not options.agent_mode and not options.yes and sys.stdin.isatty():
                         log.hugesuccess(f"Scan ready. Press enter to execute {scanner.name}")
                         input()
 
                     def keyboard_listen():
@@ -272,63 +298,63 @@
                             try:
                                 keyboard_input = input()
                                 allowed_errors = 10
                             except Exception:
                                 allowed_errors -= 1
                             if not keyboard_input:
                                 toggle_log_level(logger=log)
+                                scanner.manager.modules_status(_log=True)
                             if allowed_errors <= 0:
                                 break
 
                     keyboard_listen_thread = threading.Thread(target=keyboard_listen, daemon=True)
                     keyboard_listen_thread.start()
 
-                    scanner.start_without_generator()
+                    await scanner.async_start_without_generator()
 
             except bbot.core.errors.ScanError as e:
                 log_to_stderr(str(e), level="ERROR")
             except Exception:
                 raise
-            finally:
-                with suppress(NameError):
-                    scanner.cleanup()
 
     except bbot.core.errors.BBOTError as e:
         log_to_stderr(f"{e} (--debug for details)", level="ERROR")
         if log_level <= logging.DEBUG:
             log_to_stderr(traceback.format_exc(), level="DEBUG")
         err = True
 
     except Exception:
         log_to_stderr(f"Encountered unknown error: {traceback.format_exc()}", level="ERROR")
         err = True
 
-    except KeyboardInterrupt:
-        msg = "Interrupted"
-        if scan_name:
-            msg = f"You killed {scan_name}"
-        log_to_stderr(msg, level="ERROR")
-        err = True
-
     finally:
         # save word cloud
         with suppress(BaseException):
-            save_success, filename = scanner.helpers.word_cloud.save(options.save_wordcloud)
+            save_success, filename = scanner.helpers.word_cloud.save()
             if save_success:
                 log_to_stderr(f"Saved word cloud ({len(scanner.helpers.word_cloud):,} words) to {filename}")
         # remove output directory if empty
         with suppress(BaseException):
             scanner.home.rmdir()
         if err:
             os._exit(1)
 
-        # debug troublesome modules
-        """
-        from time import sleep
-        while 1:
-            scanner.manager.modules_status(_log=True)
-            sleep(1)
-        """
+
+def main():
+    global scan_name
+    try:
+        asyncio.run(_main())
+    except asyncio.CancelledError:
+        if get_log_level() <= logging.DEBUG:
+            log_to_stderr(traceback.format_exc(), level="DEBUG")
+    except KeyboardInterrupt:
+        msg = "Interrupted"
+        if scan_name:
+            msg = f"You killed {scan_name}"
+        log_to_stderr(msg, level="WARNING")
+        if get_log_level() <= logging.DEBUG:
+            log_to_stderr(traceback.format_exc(), level="DEBUG")
+        exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1793rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1793rc0/bbot/core/configurator/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,88 +100,85 @@
     )
     target.add_argument("-b", "--blacklist", nargs="+", default=[], help="Don't touch these things")
     target.add_argument(
         "--strict-scope",
         action="store_true",
         help="Don't consider subdomains of target/whitelist to be in-scope",
     )
-    p.add_argument("-n", "--name", help="Name of scan (default: random)", metavar="SCAN_NAME")
-    p.add_argument(
+    modules = p.add_argument_group(title="Modules")
+    modules.add_argument(
         "-m",
         "--modules",
         nargs="+",
         default=[],
         help=f'Modules to enable. Choices: {",".join(module_choices)}',
         metavar="MODULE",
     )
-    p.add_argument("-l", "--list-modules", action="store_true", help=f"List available modules.")
-    p.add_argument("-em", "--exclude-modules", nargs="+", default=[], help=f"Exclude these modules.", metavar="MODULE")
-    p.add_argument(
+    modules.add_argument("-l", "--list-modules", action="store_true", help=f"List available modules.")
+    modules.add_argument(
+        "-em", "--exclude-modules", nargs="+", default=[], help=f"Exclude these modules.", metavar="MODULE"
+    )
+    modules.add_argument(
         "-f",
         "--flags",
         nargs="+",
         default=[],
         help=f'Enable modules by flag. Choices: {",".join(sorted(flag_choices))}',
         metavar="FLAG",
     )
-    p.add_argument(
+    modules.add_argument(
         "-rf",
         "--require-flags",
         nargs="+",
         default=[],
         help=f"Only enable modules with these flags (e.g. -rf passive)",
         metavar="FLAG",
     )
-    p.add_argument(
+    modules.add_argument(
         "-ef",
         "--exclude-flags",
         nargs="+",
         default=[],
         help=f"Disable modules with these flags. (e.g. -ef aggressive)",
         metavar="FLAG",
     )
-    p.add_argument(
+    modules.add_argument(
         "-om",
         "--output-modules",
         nargs="+",
         default=["human", "json", "csv"],
         help=f'Output module(s). Choices: {",".join(output_module_choices)}',
         metavar="MODULE",
     )
-    p.add_argument(
+    modules.add_argument("--allow-deadly", action="store_true", help="Enable the use of highly aggressive modules")
+    scan = p.add_argument_group(title="Scan")
+    scan.add_argument("-n", "--name", help="Name of scan (default: random)", metavar="SCAN_NAME")
+    scan.add_argument(
         "-o",
         "--output-dir",
         metavar="DIR",
     )
-    p.add_argument(
+    scan.add_argument(
         "-c",
         "--config",
         nargs="*",
         help="custom config file, or configuration options in key=value format: 'modules.shodan.api_key=1234'",
         metavar="CONFIG",
     )
-    p.add_argument("--allow-deadly", action="store_true", help="Enable the use of highly aggressive modules")
-    p.add_argument("-v", "--verbose", action="store_true", help="Be more verbose")
-    p.add_argument("-d", "--debug", action="store_true", help="Enable debugging")
-    p.add_argument("-s", "--silent", action="store_true", help="Be quiet")
-    p.add_argument("--force", action="store_true", help="Run scan even if module setups fail")
-    p.add_argument("-y", "--yes", action="store_true", help="Skip scan confirmation prompt")
-    p.add_argument("--dry-run", action="store_true", help=f"Abort before executing scan")
-    p.add_argument(
+    scan.add_argument("-v", "--verbose", action="store_true", help="Be more verbose")
+    scan.add_argument("-d", "--debug", action="store_true", help="Enable debugging")
+    scan.add_argument("-s", "--silent", action="store_true", help="Be quiet")
+    scan.add_argument("--force", action="store_true", help="Run scan even if module setups fail")
+    scan.add_argument("-y", "--yes", action="store_true", help="Skip scan confirmation prompt")
+    scan.add_argument("--dry-run", action="store_true", help=f"Abort before executing scan")
+    scan.add_argument(
         "--current-config",
         action="store_true",
         help="Show current config in YAML format",
     )
-    wordcloud = p.add_argument_group(
-        title="Word cloud", description="Save/load wordlist of common words gathered during a scan"
-    )
-    wordcloud.add_argument(
-        "--save-wordcloud", help="Output wordcloud to custom file when the scan completes", metavar="FILE"
-    )
-    wordcloud.add_argument("--load-wordcloud", help="Load wordcloud from a custom file", metavar="FILE")
     deps = p.add_argument_group(
         title="Module dependencies", description="Control how modules install their dependencies"
     )
     g2 = deps.add_mutually_exclusive_group()
     g2.add_argument("--no-deps", action="store_true", help="Don't install module dependencies")
     g2.add_argument("--force-deps", action="store_true", help="Force install all module dependencies")
     g2.add_argument("--retry-deps", action="store_true", help="Try again to install failed module dependencies")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1793rc0/bbot/core/configurator/environ.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,36 @@
 from pathlib import Path
 
 from . import args
 from ...modules import module_loader
 from ..helpers.misc import cpu_architecture, os_platform, os_platform_friendly
 
 
+# keep track of whether BBOT is being executed via the CLI
+cli_execution = False
+
+
+def increase_limit(new_limit):
+    try:
+        import resource
+
+        # Get current limit
+        soft_limit, hard_limit = resource.getrlimit(resource.RLIMIT_NOFILE)
+
+        new_limit = min(new_limit, hard_limit)
+
+        # Attempt to set new limit
+        resource.setrlimit(resource.RLIMIT_NOFILE, (new_limit, hard_limit))
+    except Exception as e:
+        sys.stderr.write(f"Failed to set new ulimit: {e}\n")
+
+
+increase_limit(65535)
+
+
 def flatten_config(config, base="bbot"):
     """
     Flatten a JSON-like config into a list of environment variables:
         {"modules": [{"httpx": {"timeout": 5}}]} --> "BBOT_MODULES_HTTPX_TIMEOUT=5"
     """
     if type(config) == omegaconf.dictconfig.DictConfig:
         for k, v in config.items():
@@ -72,26 +94,37 @@
 
     # platform variables
     os.environ["BBOT_OS_PLATFORM"] = os_platform()
     os.environ["BBOT_OS"] = os_platform_friendly()
     os.environ["BBOT_CPU_ARCH"] = cpu_architecture()
 
     # exchange certain options between CLI args and config
-    if args.cli_options is not None:
+    if cli_execution and args.cli_options is not None:
         # deps
         bbot_config["retry_deps"] = args.cli_options.retry_deps
         bbot_config["force_deps"] = args.cli_options.force_deps
         bbot_config["no_deps"] = args.cli_options.no_deps
         bbot_config["ignore_failed_deps"] = args.cli_options.ignore_failed_deps
         # debug
         bbot_config["debug"] = args.cli_options.debug
         bbot_config["silent"] = args.cli_options.silent
         if args.cli_options.output_dir:
             bbot_config["output_dir"] = args.cli_options.output_dir
 
+    import logging
+
+    log = logging.getLogger()
+    if bbot_config.get("debug", False):
+        global _log_level_override
+        bbot_config["silent"] = False
+        _log_level_override = logging.DEBUG
+        log = logging.getLogger("bbot")
+        log.setLevel(logging.DEBUG)
+        logging.getLogger("asyncio").setLevel(logging.DEBUG)
+
     # copy config to environment
     bbot_environ = flatten_config(bbot_config)
     os.environ.update(bbot_environ)
 
     # handle HTTP proxy
     http_proxy = bbot_config.get("http_proxy", "")
     if http_proxy:
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1793rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/core/errors.py` & `bbot-1.0.5.1793rc0/bbot/core/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-from requests.exceptions import RequestException  # noqa F401
+from httpx import RequestError, ReadTimeout  # noqa
 
 
 class BBOTError(Exception):
     pass
 
 
 class ScanError(BBOTError):
     pass
 
 
-class ScanCancelledError(BBOTError):
-    pass
-
-
 class ValidationError(BBOTError):
     pass
 
 
 class ConfigLoadError(BBOTError):
     pass
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/event/base.py` & `bbot-1.0.5.1793rc0/bbot/core/event/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
+import asyncio
 import logging
 import ipaddress
 import traceback
 from typing import Optional
 from datetime import datetime
 from contextlib import suppress
 from pydantic import BaseModel, validator
-from threading import Event as ThreadingEvent
 
 from .helpers import *
 from bbot.core.errors import *
 from bbot.core.helpers import (
     extract_words,
     split_host_port,
     host_in_host,
@@ -121,16 +121,16 @@
 
         # internal events are not ingested by output modules
         if not self._dummy:
             # removed this second part because it was making certain sslcert events internal
             if _internal:  # or source._internal:
                 self.make_internal()
 
-        # a threading event indicating whether the event has undergone DNS resolution yet
-        self._resolved = ThreadingEvent()
+        # an event indicating whether the event has undergone DNS resolution
+        self._resolved = asyncio.Event()
 
     @property
     def data(self):
         return self._data
 
     @property
     def resolved_hosts(self):
@@ -305,32 +305,36 @@
             self._internal = False
             self._made_internal = False
         if force_output is True:
             self._force_output = True
         if force_output == "trail_only":
             force_output = True
 
+        # if our source event is internal, unmake it too
         if getattr(self.source, "_internal", False):
             source_scope_distance = None
             if set_scope_distance is not None:
                 source_scope_distance = set_scope_distance + 1
             source_trail += self.source.unmake_internal(
                 set_scope_distance=source_scope_distance, force_output=force_output
             )
             source_trail.append(self.source)
 
         return source_trail
 
-    def make_in_scope(self, set_scope_distance=0):
+    def set_scope_distance(self, d=0):
+        """
+        Set the scope of an event and its parents
+        """
         source_trail = []
         # keep the event internal if the module requests so, unless it's a DNS_NAME
         if getattr(self.module, "_scope_shepherding", True) or self.type in ("DNS_NAME",):
-            source_trail = self.unmake_internal(set_scope_distance=set_scope_distance, force_output="trail_only")
-        self.scope_distance = set_scope_distance
-        if set_scope_distance == 0:
+            source_trail = self.unmake_internal(set_scope_distance=d, force_output="trail_only")
+        self.scope_distance = d
+        if d == 0:
             self.add_tag("in-scope")
         return source_trail
 
     def _host(self):
         return ""
 
     def _sanitize_data(self, data):
@@ -583,30 +587,31 @@
         if isinstance(data, str):
             return json.loads(data)
         return data
 
 
 class DictHostEvent(DictEvent):
     def _host(self):
-        return make_ip_type(self.data["host"])
+        if isinstance(self.data, dict) and "host" in self.data:
+            return make_ip_type(self.data["host"])
+        else:
+            parsed = getattr(self, "parsed")
+            if parsed is not None:
+                return make_ip_type(parsed.hostname)
 
 
 class ASN(DictEvent):
     _always_emit = True
 
 
 class CODE_REPOSITORY(DictHostEvent):
     class _data_validator(BaseModel):
         url: str
         _validate_url = validator("url", allow_reuse=True)(validators.validate_url)
 
-    def _host(self):
-        self.parsed = validators.validate_url_parsed(self.data["url"])
-        return make_ip_type(self.parsed.hostname)
-
     def _pretty_string(self):
         return self.data["url"]
 
 
 class IP_ADDRESS(BaseEvent):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -802,14 +807,15 @@
     def _words(self):
         return extract_words(self.host_stem)
 
 
 class HTTP_RESPONSE(URL_UNVERIFIED, DictEvent):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        # count number of consecutive redirects
         self.num_redirects = getattr(self.source, "num_redirects", 0)
         if str(self.data.get("status_code", 0)).startswith("3"):
             self.num_redirects += 1
 
     def sanitize_data(self, data):
         url = data.get("url", "")
         self.parsed = validators.validate_url_parsed(url)
@@ -822,14 +828,15 @@
                 v = v.lstrip()
                 header_dict[k] = v
         data["header-dict"] = header_dict
         # move URL to the front of the dictionary for visibility
         data = dict(data)
         new_data = {"url": data.pop("url")}
         new_data.update(data)
+
         return new_data
 
     def _words(self):
         return set()
 
     def _pretty_string(self):
         return f'{self.data["hash"]["header_mmh3"]}:{self.data["hash"]["body_mmh3"]}'
@@ -920,15 +927,15 @@
     _always_emit = True
 
 
 class SOCIAL(DictEvent):
     _always_emit = True
 
 
-class WEBSCREENSHOT(BaseEvent):
+class WEBSCREENSHOT(DictHostEvent):
     _always_emit = True
 
 
 def make_event(
     data,
     event_type=None,
     source=None,
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1793rc0/bbot/core/event/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import ipaddress
 from contextlib import suppress
 
 from bbot.core.errors import ValidationError
 from bbot.core.helpers import sha1, smart_decode, smart_decode_punycode
-from bbot.core.helpers.regexes import event_type_regexes, event_id_regex, _hostname_regex
+from bbot.core.helpers.regexes import event_type_regexes, event_id_regex, hostname_regex
 
 
 log = logging.getLogger("bbot.core.event.helpers")
 
 
 def get_event_type(data):
     """
@@ -32,15 +32,15 @@
         for r in regexes:
             if r.match(data):
                 if t == "URL":
                     return "URL_UNVERIFIED"
                 return t
 
     # Assume DNS_NAME for basic words
-    if _hostname_regex.match(data):
+    if hostname_regex.match(data):
         return "DNS_NAME"
 
     raise ValidationError(f'Unable to autodetect event type from "{data}"')
 
 
 def is_event_id(s):
     if event_id_regex.match(str(s)):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import time
 import logging
-import threading
 from contextlib import suppress
 from collections import OrderedDict
 
 from .misc import sha1
 
 log = logging.getLogger("bbot.core.helpers.cache")
 
@@ -62,40 +61,37 @@
 class CacheDict:
     """
     Dictionary to store cached values, with a maximum size limit
     """
 
     def __init__(self, max_size=1000):
         self._cache = OrderedDict()
-        self._lock = threading.Lock()
         self._max_size = int(max_size)
 
     def get(self, name, fallback=_sentinel):
         name_hash = self._hash(name)
-        with self._lock:
-            try:
-                return self._cache[name_hash]
-            except KeyError:
-                if fallback is not _sentinel:
-                    return fallback
-                raise
-            finally:
-                with suppress(KeyError):
-                    self._cache.move_to_end(name_hash)
-                self._truncate()
+        try:
+            return self._cache[name_hash]
+        except KeyError:
+            if fallback is not _sentinel:
+                return fallback
+            raise
+        finally:
+            with suppress(KeyError):
+                self._cache.move_to_end(name_hash)
+            self._truncate()
 
     def put(self, name, value):
         name_hash = self._hash(name)
-        with self._lock:
-            try:
-                self._cache[name_hash] = value
-            finally:
-                with suppress(KeyError):
-                    self._cache.move_to_end(name_hash)
-                self._truncate()
+        try:
+            self._cache[name_hash] = value
+        finally:
+            with suppress(KeyError):
+                self._cache.move_to_end(name_hash)
+            self._truncate()
 
     def _truncate(self):
         if not self or len(self) <= self._max_size:
             return
         for nh in list(self._cache.keys()):
             try:
                 del self._cache[nh]
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,13 +21,17 @@
         self.providers = {}
         for provider_class in provider_list:
             provider_name = str(provider_class.__name__).lower()
             provider = provider_class(self.parent_helper)
             self.providers[provider_name] = provider
             setattr(self, provider_name, provider)
 
-    def excavate(self, event, http_body):
+    def excavate(self, *args, **kwargs):
         for provider in self.providers.values():
-            provider.excavate(event, http_body)
+            provider.excavate(*args, **kwargs)
+
+    def speculate(self, *args, **kwargs):
+        for provider in self.providers.values():
+            provider.speculate(*args, **kwargs)
 
     def __iter__(self):
         yield from self.providers.values()
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/cloud/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,38 +37,63 @@
                     if not match in found:
                         found.add(match)
                         if event_type == "STORAGE_BUCKET":
                             self.emit_bucket(match, **kwargs)
                         else:
                             self.emit_event(**kwargs)
 
+    def speculate(self, event):
+        base_kwargs = dict(source=event, tags=self.base_tags)
+
+        if event.type.startswith("DNS_NAME"):
+            # check for DNS_NAMEs that are buckets
+            for event_type, sigs in self.signatures.items():
+                found = set()
+                for sig in sigs:
+                    match = sig.match(event.data)
+                    if match:
+                        kwargs = dict(base_kwargs)
+                        kwargs["event_type"] = event_type
+                        if not event.data in found:
+                            found.add(event.data)
+                            if event_type == "STORAGE_BUCKET":
+                                self.emit_bucket(match.groups(), **kwargs)
+                            else:
+                                self.emit_event(**kwargs)
+
     def emit_bucket(self, match, **kwargs):
         bucket_name, bucket_domain = match
         kwargs["data"] = {"name": bucket_name, "url": f"https://{bucket_name}.{bucket_domain}"}
         self.emit_event(**kwargs)
 
     def emit_event(self, *args, **kwargs):
         excavate_module = self.parent_helper.scan.modules.get("excavate", None)
         if excavate_module:
             event = self.dummy_module.make_event(*args, **kwargs)
-            excavate_module.emit_event(event)
+            if event:
+                excavate_module.emit_event(event)
 
     def is_valid_bucket(self, bucket_name):
         return self.bucket_name_regex.match(bucket_name)
 
     def tag_event(self, event):
         # tag the event if
         if event.host:
             # its host directly matches this cloud provider's domains
             if isinstance(event.host, str) and self.domain_match(event.host):
                 event.tags.update(self.base_tags)
-                return
-            # or it has a CNAME that matches this cloud provider's domains
-            for rh in event.resolved_hosts:
-                if not self.parent_helper.is_ip(rh) and self.domain_match(rh):
-                    event.tags.update(self.base_tags)
+                # tag as buckets, etc.
+                for event_type, sigs in self.signatures.items():
+                    for sig in sigs:
+                        if sig.match(event.host):
+                            event.add_tag(f"cloud-{event_type}")
+            else:
+                # or it has a CNAME that matches this cloud provider's domains
+                for rh in event.resolved_hosts:
+                    if not self.parent_helper.is_ip(rh) and self.domain_match(rh):
+                        event.tags.update(self.base_tags)
 
     def domain_match(self, s):
         for r in self.domain_regexes:
             if r.match(s):
                 return True
         return False
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         self.parent_helper = parent_helper
 
         # respect BBOT's http timeout
         http_timeout = self.parent_helper.config.get("http_timeout", 30)
         os.environ["ANSIBLE_TIMEOUT"] = str(http_timeout)
 
         self.askpass_filename = "sudo_askpass.py"
+        self._installed_sudo_askpass = False
         self._sudo_password = os.environ.get("BBOT_SUDO_PASS", None)
         if self._sudo_password is None:
             if configurator.bbot_sudo_pass is not None:
                 self._sudo_password = configurator.bbot_sudo_pass
             elif can_sudo_without_password():
                 self._sudo_password = ""
         self.data_dir = self.parent_helper.cache_dir / "depsinstaller"
@@ -51,15 +52,15 @@
         if sys.prefix != sys.base_prefix:
             self.venv = sys.prefix
 
         self.all_modules_preloaded = module_loader.preloaded()
 
         self.ensure_root_lock = Lock()
 
-    def install(self, *modules):
+    async def install(self, *modules):
         self.install_core_deps()
         succeeded = []
         failed = []
         try:
             notified = False
             for m in modules:
                 # assume success if we're ignoring dependencies
@@ -91,15 +92,15 @@
                         if not notified:
                             log.hugeinfo(f"Installing module dependencies. Please be patient, this may take a while.")
                             notified = True
                         log.verbose(f'Installing dependencies for module "{m}"')
                         # get sudo access if we need it
                         if preloaded.get("sudo", False) == True:
                             self.ensure_root(f'Module "{m}" needs root privileges to install its dependencies.')
-                        success = self.install_module(m)
+                        success = await self.install_module(m)
                         self.setup_status[module_hash] = success
                         if success or self.ignore_failed_deps:
                             log.debug(f'Setup succeeded for module "{m}"')
                             succeeded.append(m)
                         else:
                             log.warning(f'Setup failed for module "{m}"')
                             failed.append(m)
@@ -118,15 +119,15 @@
         finally:
             self.write_setup_status()
 
         succeeded.sort()
         failed.sort()
         return succeeded, failed
 
-    def install_module(self, module):
+    async def install_module(self, module):
         success = True
         preloaded = self.all_modules_preloaded[module]
 
         # ansible tasks
         ansible_tasks = preloaded["deps"]["ansible"]
         if ansible_tasks:
             success &= self.tasks(module, ansible_tasks)
@@ -141,36 +142,36 @@
         if deps_shell:
             success &= self.shell(module, deps_shell)
 
         # pip
         deps_pip = preloaded["deps"]["pip"]
         deps_pip_constraints = preloaded["deps"]["pip_constraints"]
         if deps_pip:
-            success &= self.pip_install(deps_pip, constraints=deps_pip_constraints)
+            success &= await self.pip_install(deps_pip, constraints=deps_pip_constraints)
 
         return success
 
-    def pip_install(self, packages, constraints=None):
+    async def pip_install(self, packages, constraints=None):
         packages_str = ",".join(packages)
         log.info(f"Installing the following pip packages: {packages_str}")
 
         command = [sys.executable, "-m", "pip", "install", "--upgrade"] + packages
 
         if constraints:
             contraints_tempfile = self.parent_helper.tempfile(constraints, pipe=False)
             command.append("--constraint")
             command.append(contraints_tempfile)
 
         process = None
         try:
-            process = self.parent_helper.run(command, check=True)
+            process = await self.parent_helper.run(command, check=True)
             message = f'Successfully installed pip packages "{packages_str}"'
-            output = process.stdout.splitlines()[-1]
-            if output:
-                message = output
+            output = process.stdout
+            if output is not None:
+                message = output.splitlines()[-1]
             log.info(message)
             return True
         except CalledProcessError as err:
             log.warning(f"Failed to install pip packages {packages_str} (return code {err.returncode}): {err.stderr}")
         return False
 
     def apt_install(self, packages):
@@ -293,14 +294,15 @@
         return setup_status
 
     def write_setup_status(self):
         with open(self.setup_status_cache, "w") as f:
             json.dump(self.setup_status, f)
 
     def ensure_root(self, message=""):
+        self._install_sudo_askpass()
         with self.ensure_root_lock:
             if os.geteuid() != 0 and self._sudo_password is None:
                 if message:
                     log.warning(message)
                 while not self._sudo_password:
                     # sleep for a split second to flush previous log messages
                     sleep(0.1)
@@ -310,22 +312,27 @@
                         self._sudo_password = password
                         configurator.bbot_sudo_pass = password
                     else:
                         log.warning("Incorrect password")
 
     def install_core_deps(self):
         to_install = set()
-        # install custom askpass script
-        askpass_src = Path(__file__).resolve().parent / self.askpass_filename
-        askpass_dst = self.parent_helper.tools_dir / self.askpass_filename
-        shutil.copy(askpass_src, askpass_dst)
-        askpass_dst.chmod(askpass_dst.stat().st_mode | stat.S_IEXEC)
+        self._install_sudo_askpass()
         # ensure tldextract data is cached
         self.parent_helper.tldextract("evilcorp.co.uk")
         # command: package_name
         core_deps = {"unzip": "unzip", "curl": "curl"}
         for command, package_name in core_deps.items():
             if not self.parent_helper.which(command):
                 to_install.add(package_name)
         if to_install:
             self.ensure_root()
             self.apt_install(list(to_install))
+
+    def _install_sudo_askpass(self):
+        if not self._installed_sudo_askpass:
+            self._installed_sudo_askpass = True
+            # install custom askpass script
+            askpass_src = Path(__file__).resolve().parent / self.askpass_filename
+            askpass_dst = self.parent_helper.tools_dir / self.askpass_filename
+            shutil.copy(askpass_src, askpass_dst)
+            askpass_dst.chmod(askpass_dst.stat().st_mode | stat.S_IEXEC)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,95 @@
 import logging
 import xmltodict
-from time import sleep
 from deepdiff import DeepDiff
 from contextlib import suppress
 from xml.parsers.expat import ExpatError
 from bbot.core.errors import HttpCompareError
 
 log = logging.getLogger("bbot.core.helpers.diff")
 
 
 class HttpCompare:
     def __init__(self, baseline_url, parent_helper, method="GET", allow_redirects=False, include_cache_buster=True):
         self.parent_helper = parent_helper
         self.baseline_url = baseline_url
         self.include_cache_buster = include_cache_buster
+        self.method = method
+        self.allow_redirects = allow_redirects
+        self._baselined = False
+
+    async def _baseline(self):
+        if not self._baselined:
+            self._baselined = True
+            # vanilla URL
+            if self.include_cache_buster:
+                url_1 = self.parent_helper.add_get_params(self.baseline_url, self.gen_cache_buster()).geturl()
+            else:
+                url_1 = self.baseline_url
+            baseline_1 = await self.parent_helper.request(
+                url_1, follow_redirects=self.allow_redirects, method=self.method
+            )
+            await self.parent_helper.sleep(1)
+            # put random parameters in URL, headers, and cookies
+            get_params = {self.parent_helper.rand_string(6): self.parent_helper.rand_string(6)}
+
+            if self.include_cache_buster:
+                get_params.update(self.gen_cache_buster())
+            url_2 = self.parent_helper.add_get_params(self.baseline_url, get_params).geturl()
+            baseline_2 = await self.parent_helper.request(
+                url_2,
+                headers={self.parent_helper.rand_string(6): self.parent_helper.rand_string(6)},
+                cookies={self.parent_helper.rand_string(6): self.parent_helper.rand_string(6)},
+                follow_redirects=self.allow_redirects,
+                method=self.method,
+            )
 
-        # vanilla URL
-        if self.include_cache_buster:
-            url_1 = self.parent_helper.add_get_params(self.baseline_url, self.gen_cache_buster()).geturl()
-        else:
-            url_1 = self.baseline_url
-        baseline_1 = self.parent_helper.request(url_1, allow_redirects=allow_redirects, method=method)
-        sleep(1)
-        # put random parameters in URL, headers, and cookies
-        get_params = {self.parent_helper.rand_string(6): self.parent_helper.rand_string(6)}
-
-        if self.include_cache_buster:
-            get_params.update(self.gen_cache_buster())
-        url_2 = self.parent_helper.add_get_params(self.baseline_url, get_params).geturl()
-        baseline_2 = self.parent_helper.request(
-            url_2,
-            headers={self.parent_helper.rand_string(6): self.parent_helper.rand_string(6)},
-            cookies={self.parent_helper.rand_string(6): self.parent_helper.rand_string(6)},
-            allow_redirects=allow_redirects,
-            method=method,
-        )
-
-        self.baseline = baseline_1
-
-        if baseline_1 is None or baseline_2 is None:
-            log.debug("HTTP error while establishing baseline, aborting")
-            raise HttpCompareError("Can't get baseline from source URL")
-        if baseline_1.status_code != baseline_2.status_code:
-            log.debug("Status code not stable during baseline, aborting")
-            raise HttpCompareError("Can't get baseline from source URL")
-        try:
-            baseline_1_json = xmltodict.parse(baseline_1.text)
-            baseline_2_json = xmltodict.parse(baseline_2.text)
-        except ExpatError:
-            log.debug(f"Cant HTML parse for {baseline_url}. Switching to text parsing as a backup")
-            baseline_1_json = baseline_1.text.split("\n")
-            baseline_2_json = baseline_2.text.split("\n")
-
-        ddiff = DeepDiff(baseline_1_json, baseline_2_json, ignore_order=True, view="tree")
-        self.ddiff_filters = []
-
-        for k, v in ddiff.items():
-            for x in list(ddiff[k]):
-                log.debug(f"Added {k} filter for path: {x.path()}")
-                self.ddiff_filters.append(x.path())
-
-        self.baseline_json = baseline_1_json
+            self.baseline = baseline_1
 
-        self.baseline_ignore_headers = [
-            h.lower()
-            for h in [
-                "date",
-                "last-modified",
-                "content-length",
-                "ETag",
-                "X-Pad",
-                "X-Backside-Transport",
+            if baseline_1 is None or baseline_2 is None:
+                log.debug("HTTP error while establishing baseline, aborting")
+                raise HttpCompareError(
+                    f"Can't get baseline from source URL: {url_1}:{baseline_1} / {url_2}:{baseline_2}"
+                )
+            if baseline_1.status_code != baseline_2.status_code:
+                log.debug("Status code not stable during baseline, aborting")
+                raise HttpCompareError("Can't get baseline from source URL")
+            try:
+                baseline_1_json = xmltodict.parse(baseline_1.text)
+                baseline_2_json = xmltodict.parse(baseline_2.text)
+            except ExpatError:
+                log.debug(f"Cant HTML parse for {self.baseline_url}. Switching to text parsing as a backup")
+                baseline_1_json = baseline_1.text.split("\n")
+                baseline_2_json = baseline_2.text.split("\n")
+
+            ddiff = DeepDiff(baseline_1_json, baseline_2_json, ignore_order=True, view="tree")
+            self.ddiff_filters = []
+
+            for k, v in ddiff.items():
+                for x in list(ddiff[k]):
+                    log.debug(f"Added {k} filter for path: {x.path()}")
+                    self.ddiff_filters.append(x.path())
+
+            self.baseline_json = baseline_1_json
+
+            self.baseline_ignore_headers = [
+                h.lower()
+                for h in [
+                    "date",
+                    "last-modified",
+                    "content-length",
+                    "ETag",
+                    "X-Pad",
+                    "X-Backside-Transport",
+                ]
             ]
-        ]
-        dynamic_headers = self.compare_headers(baseline_1.headers, baseline_2.headers)
+            dynamic_headers = self.compare_headers(baseline_1.headers, baseline_2.headers)
 
-        self.baseline_ignore_headers += [x.lower() for x in dynamic_headers]
-        self.baseline_body_distance = self.compare_body(baseline_1_json, baseline_2_json)
+            self.baseline_ignore_headers += [x.lower() for x in dynamic_headers]
+            self.baseline_body_distance = self.compare_body(baseline_1_json, baseline_2_json)
 
     def gen_cache_buster(self):
         return {self.parent_helper.rand_string(6): "1"}
 
     def compare_headers(self, headers_1, headers_2):
         differing_headers = []
 
@@ -110,34 +119,35 @@
 
         if len(ddiff.keys()) == 0:
             return True
         else:
             log.debug(ddiff)
             return False
 
-    def compare(
+    async def compare(
         self, subject, headers=None, cookies=None, check_reflection=False, method="GET", allow_redirects=False
     ):
         """
         Compares a URL with the baseline, with optional headers or cookies added
 
         Returns (match (bool), reason (str), reflection (bool),subject_response (requests response object))
             where "match" is whether the content matched against the baseline, and
                 "reason" is the location of the change ("code", "body", "header", or None), and
                 "reflection" is whether the value was reflected in the HTTP response
         """
+        await self._baseline()
 
         reflection = False
         if self.include_cache_buster:
             cache_key, cache_value = list(self.gen_cache_buster().items())[0]
             url = self.parent_helper.add_get_params(subject, {cache_key: cache_value}).geturl()
         else:
             url = subject
-        subject_response = self.parent_helper.request(
-            url, headers=headers, cookies=cookies, allow_redirects=allow_redirects, method=method
+        subject_response = await self.parent_helper.request(
+            url, headers=headers, cookies=cookies, follow_redirects=allow_redirects, method=method
         )
 
         if not subject_response:
             # this can be caused by a WAF not liking the header, so we really arent interested in it
             return (True, "403", reflection, subject_response)
 
         if check_reflection:
@@ -180,31 +190,34 @@
             diff_reasons.append("body")
 
         if not diff_reasons:
             return (True, [], False, None)
         else:
             return (False, diff_reasons, reflection, subject_response)
 
-    def canary_check(self, url, mode, rounds=6):
+    async def canary_check(self, url, mode, rounds=6):
         """
         test detection using a canary to find hosts giving bad results
         """
+        await self._baseline()
         headers = None
         cookies = None
         for i in range(0, rounds):
             random_params = {self.parent_helper.rand_string(7): self.parent_helper.rand_string(6)}
             new_url = str(url)
             if mode == "getparam":
                 new_url = self.parent_helper.add_get_params(url, random_params).geturl()
             elif mode == "header":
                 headers = random_params
             elif mode == "cookie":
                 cookies = random_params
             else:
                 raise ValueError(f'Invalid mode: "{mode}", choose from: getparam, header, cookie')
 
-            match, reasons, reflection, subject_response = self.compare(new_url, headers=headers, cookies=cookies)
+            match, reasons, reflection, subject_response = await self.compare(
+                new_url, headers=headers, cookies=cookies
+            )
 
             # a nonsense header "caused" a difference, we need to abort
             if match == False:
                 return False
         return True
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/dns.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-import json
+import asyncio
 import logging
 import ipaddress
 import traceback
-import dns.resolver
+import contextlib
 import dns.exception
-from threading import Lock
-from contextlib import suppress
+import dns.asyncresolver
 
 from .regexes import dns_name_regex
+from bbot.core.helpers.ratelimiter import RateLimiter
+from bbot.core.helpers.async_helpers import NamedLock
 from bbot.core.errors import ValidationError, DNSError
-from .threadpool import NamedLock, PatchedThreadPoolExecutor
-from .misc import is_ip, is_domain, domain_parents, parent_domain, rand_string, cloudcheck
+from .misc import is_ip, is_domain, is_dns_name, domain_parents, parent_domain, rand_string, cloudcheck
 
 log = logging.getLogger("bbot.core.helpers.dns")
 
 
 class DNSHelper:
     """
     For automatic wildcard detection, nameserver validation, etc.
     """
 
-    nameservers_url = "https://public-dns.info/nameserver/nameservers.json"
     all_rdtypes = ["A", "AAAA", "SRV", "MX", "NS", "SOA", "CNAME", "TXT"]
 
     def __init__(self, parent_helper):
         self.parent_helper = parent_helper
         try:
-            self.resolver = dns.resolver.Resolver()
+            self.resolver = dns.asyncresolver.Resolver()
         except Exception as e:
             raise DNSError(f"Failed to create BBOT DNS resolver: {e}")
         self.timeout = self.parent_helper.config.get("dns_timeout", 5)
         self.retries = self.parent_helper.config.get("dns_retries", 1)
         self.abort_threshold = self.parent_helper.config.get("dns_abort_threshold", 5)
         self.max_dns_resolve_distance = self.parent_helper.config.get("max_dns_resolve_distance", 4)
         self.resolver.timeout = self.timeout
@@ -44,135 +43,121 @@
         self.wildcard_tests = self.parent_helper.config.get("dns_wildcard_tests", 5)
         self._wildcard_cache = dict()
         # since wildcard detection takes some time, This is to prevent multiple
         # modules from kicking off wildcard detection for the same domain at the same time
         self._wildcard_lock = NamedLock()
         # keeps track of warnings issued for wildcard detection to prevent duplicate warnings
         self._dns_warnings = set()
-
         self._errors = dict()
-        self._error_lock = Lock()
-
         self.fallback_nameservers_file = self.parent_helper.wordlist_dir / "nameservers.txt"
-
-        # we need our own threadpool because using the shared one can lead to deadlocks
-        max_workers = self.parent_helper.config.get("max_dns_threads", 100)
-        self._thread_pool = PatchedThreadPoolExecutor(max_workers=max_workers)
-
+        self.dns_queries_per_second = self.parent_helper.config.get("dns_queries_per_second", 100)
+        self.dns_rate_limiter = RateLimiter(self.dns_queries_per_second, "DNS")
         self._debug = self.parent_helper.config.get("dns_debug", False)
-
         self._dummy_modules = dict()
-        self._dummy_modules_lock = Lock()
-
         self._dns_cache = self.parent_helper.CacheDict(max_size=100000)
-
         self._event_cache = self.parent_helper.CacheDict(max_size=10000)
-        self._event_cache_lock = Lock()
         self._event_cache_locks = NamedLock()
 
         # copy the system's current resolvers to a text file for tool use
         self.system_resolvers = dns.resolver.Resolver().nameservers
         self.resolver_file = self.parent_helper.tempfile(self.system_resolvers, pipe=False)
 
         self.filter_bad_ptrs = self.parent_helper.config.get("dns_filter_ptrs", True)
 
-    def resolve(self, query, **kwargs):
+    async def resolve(self, query, **kwargs):
         """
         "1.2.3.4" --> {
             "evilcorp.com",
         }
         "evilcorp.com" --> {
             "1.2.3.4",
             "dead::beef"
         }
         """
         results = set()
-        raw_results, errors = self.resolve_raw(query, **kwargs)
-        for rdtype, answers in raw_results:
-            for answer in answers:
-                for _, t in self.extract_targets(answer):
-                    results.add(t)
+        r = await self.resolve_raw(query, **kwargs)
+        if r:
+            raw_results, errors = r
+            for rdtype, answers in raw_results:
+                for answer in answers:
+                    for _, t in self.extract_targets(answer):
+                        results.add(t)
         return results
 
-    def resolve_raw(self, query, **kwargs):
+    async def resolve_raw(self, query, **kwargs):
         # DNS over TCP is more reliable
         # But setting this breaks DNS resolution on Ubuntu because systemd-resolve doesn't support TCP
         # kwargs["tcp"] = True
+        results = []
+        errors = []
         query = str(query).strip()
-        if is_ip(query):
-            kwargs.pop("type", None)
-            kwargs.pop("rdtype", None)
-            results, errors = self._resolve_ip(query, **kwargs)
-            return [("PTR", results)], [("PTR", e) for e in errors]
-        else:
-            results = []
-            errors = []
-            types = ["A", "AAAA"]
-            kwargs.pop("rdtype", None)
-            if "type" in kwargs:
-                t = kwargs.pop("type")
-                if isinstance(t, str):
-                    if t.strip().lower() in ("any", "all", "*"):
-                        types = self.all_rdtypes
-                    else:
-                        types = [t.strip().upper()]
-                elif any([isinstance(t, x) for x in (list, tuple)]):
-                    types = [str(_).strip().upper() for _ in t]
-            for t in types:
-                r, e = self._resolve_hostname(query, rdtype=t, **kwargs)
-                if r:
-                    results.append((t, r))
-                for error in e:
-                    errors.append((t, error))
-
-            return (results, errors)
-
-    def submit_task(self, *args, **kwargs):
         try:
-            return self._thread_pool.submit(*args, **kwargs)
+            if is_ip(query):
+                kwargs.pop("type", None)
+                kwargs.pop("rdtype", None)
+                results, errors = await self._resolve_ip(query, **kwargs)
+                return [("PTR", results)], [("PTR", e) for e in errors]
+            else:
+                types = ["A", "AAAA"]
+                kwargs.pop("rdtype", None)
+                if "type" in kwargs:
+                    t = kwargs.pop("type")
+                    if isinstance(t, str):
+                        if t.strip().lower() in ("any", "all", "*"):
+                            types = self.all_rdtypes
+                        else:
+                            types = [t.strip().upper()]
+                    elif any([isinstance(t, x) for x in (list, tuple)]):
+                        types = [str(_).strip().upper() for _ in t]
+                for t in types:
+                    r, e = await self._resolve_hostname(query, rdtype=t, **kwargs)
+                    if r:
+                        results.append((t, r))
+                    for error in e:
+                        errors.append((t, error))
         except RuntimeError as e:
-            log.debug(f"Error submitting DNS thread task: {e}")
+            log.debug(f"Error in resolve_raw({query}, kwargs={kwargs}): {e}")
+            log.trace(traceback.format_exc())
+
+        return (results, errors)
 
-    def _resolve_hostname(self, query, **kwargs):
+    async def _resolve_hostname(self, query, **kwargs):
         self.debug(f"Resolving {query} with kwargs={kwargs}")
         results = []
         errors = []
         parent = self.parent_helper.parent_domain(query)
         rdtype = kwargs.get("rdtype", "A")
         retries = kwargs.pop("retries", self.retries)
         cache_result = kwargs.pop("cache_result", False)
         tries_left = int(retries) + 1
         parent_hash = hash(f"{parent}:{rdtype}")
         dns_cache_hash = hash(f"{query}:{rdtype}")
         while tries_left > 0:
-            if self.parent_helper.scan_stopping:
-                break
             try:
                 try:
                     results = self._dns_cache[dns_cache_hash]
                 except KeyError:
                     error_count = self._errors.get(parent_hash, 0)
                     if error_count >= self.abort_threshold:
                         log.verbose(
                             f'Aborting query "{query}" because failed {rdtype} queries for "{parent}" ({error_count:,}) exceeded abort threshold ({self.abort_threshold:,})'
                         )
                         return results, errors
-                    results = list(self._catch(self.resolver.resolve, query, **kwargs))
+                    async with self.dns_rate_limiter:
+                        results = await self._catch(self.resolver.resolve, query, **kwargs)
                     if cache_result:
                         self._dns_cache[dns_cache_hash] = results
-                    with self._error_lock:
-                        if parent_hash in self._errors:
-                            self._errors[parent_hash] = 0
+                    if parent_hash in self._errors:
+                        self._errors[parent_hash] = 0
                 break
             except (dns.resolver.NoNameservers, dns.exception.Timeout, dns.resolver.LifetimeTimeout) as e:
-                with self._error_lock:
-                    try:
-                        self._errors[parent_hash] += 1
-                    except KeyError:
-                        self._errors[parent_hash] = 1
+                try:
+                    self._errors[parent_hash] += 1
+                except KeyError:
+                    self._errors[parent_hash] = 1
                 errors.append(e)
                 # don't retry if we get a SERVFAIL
                 if isinstance(e, dns.resolver.NoNameservers):
                     break
                 tries_left -= 1
                 err_msg = (
                     f'DNS error or timeout for {rdtype} query "{query}" ({self._errors[parent_hash]:,} so far): {e}'
@@ -180,94 +165,94 @@
                 if tries_left > 0:
                     retry_num = (retries + 1) - tries_left
                     self.debug(err_msg)
                     self.debug(f"Retry (#{retry_num}) resolving {query} with kwargs={kwargs}")
                 else:
                     log.verbose(err_msg)
 
-        self.debug(f"Results for {query} with kwargs={kwargs}: {results}")
         return results, errors
 
-    def _resolve_ip(self, query, **kwargs):
+    async def _resolve_ip(self, query, **kwargs):
         self.debug(f"Reverse-resolving {query} with kwargs={kwargs}")
         retries = kwargs.pop("retries", 0)
         cache_result = kwargs.pop("cache_result", False)
         tries_left = int(retries) + 1
         results = []
         errors = []
         dns_cache_hash = hash(f"{query}:PTR")
         while tries_left > 0:
-            if self.parent_helper.scan_stopping:
-                break
             try:
-                if dns_cache_hash in self._dns_cache:
-                    result = self._dns_cache[dns_cache_hash]
-                else:
-                    result = list(self._catch(self.resolver.resolve_address, query, **kwargs))
+                try:
+                    results = self._dns_cache[dns_cache_hash]
+                except KeyError:
+                    async with self.dns_rate_limiter:
+                        results = await self._catch(self.resolver.resolve_address, query, **kwargs)
                     if cache_result:
-                        self._dns_cache[dns_cache_hash] = result
-                return result, errors
+                        self._dns_cache[dns_cache_hash] = results
+                break
             except (dns.exception.Timeout, dns.resolver.LifetimeTimeout, dns.resolver.NoNameservers) as e:
                 errors.append(e)
                 # don't retry if we get a SERVFAIL
                 if isinstance(e, dns.resolver.NoNameservers):
                     self.debug(f"{e} (query={query}, kwargs={kwargs})")
                     break
                 else:
                     tries_left -= 1
                     if tries_left > 0:
                         retry_num = (retries + 2) - tries_left
                         self.debug(f"Retrying (#{retry_num}) {query} with kwargs={kwargs}")
         self.debug(f"Results for {query} with kwargs={kwargs}: {results}")
         return results, errors
 
-    def handle_wildcard_event(self, event, children):
+    async def handle_wildcard_event(self, event, children):
         event_host = str(event.host)
         # wildcard checks
         if not is_ip(event.host):
             # check if this domain is using wildcard dns
             event_target = "target" in event.tags
-            for hostname, wildcard_domain_rdtypes in self.is_wildcard_domain(
-                event_host, log_info=event_target
+            for hostname, wildcard_domain_rdtypes in (
+                await self.is_wildcard_domain(event_host, log_info=event_target)
             ).items():
                 if wildcard_domain_rdtypes:
                     event.add_tag("wildcard-domain")
                     for rdtype, ips in wildcard_domain_rdtypes.items():
                         event.add_tag(f"{rdtype.lower()}-wildcard-domain")
             # check if the dns name itself is a wildcard entry
-            wildcard_rdtypes = self.is_wildcard(event_host)
+            wildcard_rdtypes = await self.is_wildcard(event_host)
             for rdtype, (is_wildcard, wildcard_host) in wildcard_rdtypes.items():
                 wildcard_tag = "error"
                 if is_wildcard == True:
                     event.add_tag("wildcard")
                     wildcard_tag = "wildcard"
                 event.add_tag(f"{rdtype.lower()}-{wildcard_tag}")
 
         # wildcard event modification (www.evilcorp.com --> _wildcard.evilcorp.com)
-        if not is_ip(event.host) and children and wildcard_rdtypes:
+        if not is_ip(event.host) and wildcard_rdtypes and children:
             # these are the rdtypes that successfully resolve
             resolved_rdtypes = set([c.upper() for c in children])
             # these are the rdtypes that have wildcards
             wildcard_rdtypes_set = set(wildcard_rdtypes)
             # consider the event a full wildcard if all its records are wildcards
             event_is_wildcard = False
             if resolved_rdtypes:
                 event_is_wildcard = all(r in wildcard_rdtypes_set for r in resolved_rdtypes)
-            if event_is_wildcard and event.type in ("DNS_NAME",) and not "_wildcard" in event.data.split("."):
-                wildcard_parent = self.parent_helper.parent_domain(event_host)
-                for rdtype, (_is_wildcard, _parent_domain) in wildcard_rdtypes.items():
-                    if _is_wildcard:
-                        wildcard_parent = _parent_domain
-                        break
-                wildcard_data = f"_wildcard.{wildcard_parent}"
-                if wildcard_data != event.data:
-                    log.debug(f'Wildcard detected, changing event.data "{event.data}" --> "{wildcard_data}"')
-                    event.data = wildcard_data
+            # if event_is_wildcard and event.type in ("DNS_NAME",) and not "_wildcard" in event.data.split("."):
+            if event_is_wildcard:
+                if event.type in ("DNS_NAME",) and not "_wildcard" in event.data.split("."):
+                    wildcard_parent = self.parent_helper.parent_domain(event_host)
+                    for rdtype, (_is_wildcard, _parent_domain) in wildcard_rdtypes.items():
+                        if _is_wildcard:
+                            wildcard_parent = _parent_domain
+                            break
+                    wildcard_data = f"_wildcard.{wildcard_parent}"
+                    if wildcard_data != event.data:
+                        log.debug(f'Wildcard detected, changing event.data "{event.data}" --> "{wildcard_data}"')
+                        event.data = wildcard_data
 
-    def resolve_event(self, event, minimal=False):
+    async def resolve_event(self, event, minimal=False):
         """
         Tag event with appropriate dns record types
         Optionally create child events from dns resolutions
         """
         log.debug(f"Resolving {event}")
         event_host = str(event.host)
         event_tags = set()
@@ -275,15 +260,15 @@
         event_whitelisted = False
         event_blacklisted = False
 
         if not event.host or event.type in ("IP_RANGE",):
             return event_tags, event_whitelisted, event_blacklisted, dns_children
 
         # lock to ensure resolution of the same host doesn't start while we're working here
-        with self._event_cache_locks.get_lock(event_host):
+        async with self._event_cache_locks.lock(event_host):
             # try to get data from cache
             _event_tags, _event_whitelisted, _event_blacklisted, _dns_children = self.event_cache_get(event_host)
             event_tags.update(_event_tags)
             # if we found it, return it
             if _event_whitelisted is not None:
                 return event_tags, _event_whitelisted, _event_blacklisted, _dns_children
 
@@ -295,25 +280,17 @@
             else:
                 if event.type == "DNS_NAME" and not minimal:
                     types = self.all_rdtypes
                 else:
                     types = ("A", "AAAA")
 
             if types:
-                futures = {}
-                for t in types:
-                    future = self.submit_task(
-                        self._catch_keyboardinterrupt, self.resolve_raw, event_host, type=t, cache_result=True
-                    )
-                    if future is None:
-                        break
-                    futures[future] = t
-
-                for future in self.parent_helper.as_completed(futures):
-                    resolved_raw, errors = future.result()
+                tasks = [asyncio.create_task(self.resolve_raw(event_host, type=t, cache_result=True)) for t in types]
+                for task in asyncio.as_completed(tasks):
+                    resolved_raw, errors = await task
                     for rdtype, e in errors:
                         if rdtype not in resolved_raw:
                             event_tags.add(f"{rdtype.lower()}-error")
                     for rdtype, records in resolved_raw:
                         rdtype = str(rdtype).upper()
                         if records:
                             event_tags.add("resolved")
@@ -322,19 +299,19 @@
                         # whitelisting and blacklisting of IPs
                         for r in records:
                             for _, t in self.extract_targets(r):
                                 if t:
                                     ip = self.parent_helper.make_ip_type(t)
 
                                     if rdtype in ("A", "AAAA", "CNAME"):
-                                        with suppress(ValidationError):
+                                        with contextlib.suppress(ValidationError):
                                             if self.parent_helper.is_ip(ip):
                                                 if self.parent_helper.scan.whitelisted(ip):
                                                     event_whitelisted = True
-                                        with suppress(ValidationError):
+                                        with contextlib.suppress(ValidationError):
                                             if self.parent_helper.scan.blacklisted(ip):
                                                 event_blacklisted = True
 
                                     if self.filter_bad_ptrs and rdtype in ("PTR") and self.parent_helper.is_ptr(t):
                                         self.debug(f"Filtering out bad PTR: {t}")
                                         continue
 
@@ -376,30 +353,33 @@
 
     def event_cache_get(self, host):
         try:
             return self._event_cache[host]
         except KeyError:
             return set(), None, None, set()
 
-    def resolve_batch(self, queries, **kwargs):
+    async def _resolve_batch_coro_wrapper(self, q, **kwargs):
         """
-        resolve_batch("www.evilcorp.com", "evilcorp.com") --> [
+        Helps us correlate task results back to their original arguments
+        """
+        result = await self.resolve(q, **kwargs)
+        return (q, result)
+
+    async def resolve_batch(self, queries, **kwargs):
+        """
+        await resolve_batch(["www.evilcorp.com", "evilcorp.com"]) --> [
             ("www.evilcorp.com", {"1.1.1.1"}),
             ("evilcorp.com", {"2.2.2.2"})
         ]
         """
-        futures = dict()
-        for query in queries:
-            future = self.submit_task(self._catch_keyboardinterrupt, self.resolve, query, **kwargs)
-            if future is None:
-                break
-            futures[future] = query
-        for future in self.parent_helper.as_completed(futures):
-            query = futures[future]
-            yield (query, future.result())
+
+        for task in asyncio.as_completed(
+            [asyncio.create_task(self._resolve_batch_coro_wrapper(q, **kwargs)) for q in queries]
+        ):
+            yield await task
 
     def extract_targets(self, record):
         """
         Extract whatever hostnames/IPs a DNS records points to
         """
         results = set()
         rdtype = str(record.rdtype.name).upper()
@@ -420,64 +400,33 @@
                     results.add((rdtype, host))
         else:
             log.warning(f'Unknown DNS record type "{rdtype}"')
         return results
 
     @staticmethod
     def _clean_dns_record(record):
-        with suppress(Exception):
+        if not isinstance(record, str):
             record = str(record.to_text())
         return str(record).rstrip(".").lower()
 
-    def get_valid_resolvers(self, min_reliability=0.99):
-        nameservers = set()
-        nameservers_file = self.parent_helper.download(self.nameservers_url, cache_hrs=72)
-        if nameservers_file is None:
-            log.warning(f"Failed to download nameservers from {self.nameservers_url}")
-        else:
-            nameservers_json = []
-            try:
-                nameservers_json = json.loads(open(nameservers_file).read())
-            except Exception as e:
-                log.warning(f"Failed to load nameserver list from {nameservers_file}: {e}")
-                nameservers_file.unlink()
-            for entry in nameservers_json:
-                try:
-                    ip = str(entry.get("ip", "")).strip()
-                except Exception:
-                    continue
-                try:
-                    reliability = float(entry.get("reliability", 0))
-                except ValueError:
-                    continue
-                if reliability >= min_reliability and is_ip(ip, version=4):
-                    nameservers.add(ip)
-            log.verbose(f"Loaded {len(nameservers):,} nameservers from {self.nameservers_url}")
-        if not nameservers:
-            log.info(f"Loading fallback nameservers from {self.fallback_nameservers_file}")
-            lines = self.parent_helper.read_file(self.fallback_nameservers_file)
-            nameservers = set([l for l in lines if not l.startswith("#")])
-        resolver_list = self.verify_nameservers(nameservers)
-        return resolver_list
-
-    def _catch(self, callback, *args, **kwargs):
+    async def _catch(self, callback, *args, **kwargs):
         try:
-            return callback(*args, **kwargs)
+            return await callback(*args, **kwargs)
         except dns.resolver.NoNameservers:
             raise
         except (dns.exception.Timeout, dns.resolver.LifetimeTimeout):
             log.debug(f"DNS query with args={args}, kwargs={kwargs} timed out after {self.timeout} seconds")
             raise
         except dns.exception.DNSException as e:
             self.debug(f"{e} (args={args}, kwargs={kwargs})")
         except Exception:
             log.warning(f"Error in {callback.__qualname__}() with args={args}, kwargs={kwargs}")
-        return list()
+        return []
 
-    def is_wildcard(self, query, ips=None, rdtype=None):
+    async def is_wildcard(self, query, ips=None, rdtype=None):
         """
         Use this method to check whether a *host* is a wildcard entry
 
         This can reliably tell the difference between a valid DNS record and a wildcard inside a wildcard domain.
 
         If you want to know whether a domain is using wildcard DNS, use is_wildcard_domain() instead.
 
@@ -485,57 +434,61 @@
             {rdtype: (is_wildcard, wildcard_parent)}
 
             is_wildcard("www.github.io") --> {"A": (True, "github.io"), "AAAA": (True, "github.io")}
 
         Note that is_wildcard can be True, False, or None (indicating that wildcard detection was inconclusive)
         """
         result = {}
+
+        if not is_dns_name(query):
+            return {}
+
+        # skip check if the query's parent domain is excluded in the config
+        for d in self.wildcard_ignore:
+            if self.parent_helper.host_in_host(query, d):
+                log.debug(f"Skipping wildcard detection on {query} because it is excluded in the config")
+                return {}
+
         if rdtype is None:
             rdtype = "ANY"
 
         query = self._clean_dns_record(query)
         # skip check if it's an IP
         if is_ip(query) or not "." in query:
             return {}
         # skip check if the query is a domain
         if is_domain(query):
             return {}
-        # skip check if the query's parent domain is excluded in the config
-        for d in self.wildcard_ignore:
-            if self.parent_helper.host_in_host(query, d):
-                return {}
 
         parent = parent_domain(query)
         parents = list(domain_parents(query))
 
-        futures = []
+        wildcard_tasks = {t: [] for t in self.all_rdtypes}
         base_query_ips = dict()
         # if the caller hasn't already done the work of resolving the IPs
         if ips is None:
             # then resolve the query for all rdtypes
             for _rdtype in self.all_rdtypes:
                 # resolve the base query
-                future = self.submit_task(
-                    self._catch_keyboardinterrupt, self.resolve_raw, query, type=_rdtype, cache_result=True
+                wildcard_tasks[_rdtype].append(
+                    asyncio.create_task(self.resolve_raw(query, type=_rdtype, cache_result=True))
                 )
-                if future is None:
-                    break
-                futures.append(future)
 
-            for future in self.parent_helper.as_completed(futures):
-                raw_results, errors = future.result()
-                if errors and not raw_results:
-                    self.debug(f"Failed to resolve {query} ({_rdtype}) during wildcard detection")
-                    result[_rdtype] = (None, parent)
-                    continue
-                for _rdtype, answers in raw_results:
-                    base_query_ips[_rdtype] = set()
-                    for answer in answers:
-                        for _, t in self.extract_targets(answer):
-                            base_query_ips[_rdtype].add(t)
+            for _rdtype, tasks in wildcard_tasks.items():
+                for task in asyncio.as_completed(tasks):
+                    raw_results, errors = await task
+                    if errors and not raw_results:
+                        self.debug(f"Failed to resolve {query} ({_rdtype}) during wildcard detection")
+                        result[_rdtype] = (None, parent)
+                        continue
+                    for __rdtype, answers in raw_results:
+                        base_query_ips[__rdtype] = set()
+                        for answer in answers:
+                            for _, t in self.extract_targets(answer):
+                                base_query_ips[__rdtype].add(t)
         else:
             # otherwise, we can skip all that
             base_query_ips[rdtype] = set([self._clean_dns_record(ip) for ip in ips])
         if not base_query_ips:
             return result
 
         # once we've resolved the base query and have IP addresses to work with
@@ -546,116 +499,100 @@
             query_ips = base_query_ips.get("ANY", base_query_ips.get(_rdtype, set()))
             if not query_ips:
                 continue
             # for every parent domain, starting with the longest
             for host in parents[::-1]:
                 host_hash = hash(host)
                 # make sure we've checked that domain for wildcards
-                self.is_wildcard_domain(host)
+                await self.is_wildcard_domain(host)
                 if host_hash in self._wildcard_cache:
                     # then get its IPs from our wildcard cache
                     wildcard_rdtypes = self._wildcard_cache[host_hash]
                     # then check to see if our IPs match the wildcard ones
                     if _rdtype in wildcard_rdtypes:
                         wildcard_ips = wildcard_rdtypes[_rdtype]
                         # if our IPs match the wildcard ones, then ladies and gentlemen we have a wildcard
                         is_wildcard = any(r in wildcard_ips for r in query_ips)
                         if is_wildcard:
                             result[_rdtype] = (True, host)
                             break
 
         return result
 
-    def is_wildcard_domain(self, domain, log_info=False):
+    async def is_wildcard_domain(self, domain, log_info=False):
         """
         Check whether a domain is using wildcard DNS
 
         Returns a dictionary containing any DNS record types that are wildcards, and their associated IPs
             is_wildcard_domain("github.io") --> {"A": {"1.2.3.4",}, "AAAA": {"dead::beef",}}
         """
         wildcard_domain_results = {}
         domain = self._clean_dns_record(domain)
 
+        if not is_dns_name(domain):
+            return {}
+
+        # skip check if the query's parent domain is excluded in the config
+        for d in self.wildcard_ignore:
+            if self.parent_helper.host_in_host(domain, d):
+                log.debug(f"Skipping wildcard detection on {domain} because it is excluded in the config")
+                return {}
+
         # make a list of its parents
         parents = list(domain_parents(domain, include_self=True))
         # and check each of them, beginning with the highest parent (i.e. the root domain)
         for i, host in enumerate(parents[::-1]):
             # have we checked this host before?
             host_hash = hash(host)
-            with self._wildcard_lock.get_lock(host_hash):
+            async with self._wildcard_lock.lock(host_hash):
                 # if we've seen this host before
                 if host_hash in self._wildcard_cache:
                     wildcard_domain_results[host] = self._wildcard_cache[host_hash]
                     continue
 
                 # determine if this is a wildcard domain
-                wildcard_futures = {}
+                wildcard_tasks = {t: [] for t in self.all_rdtypes}
                 # resolve a bunch of random subdomains of the same parent
                 for rdtype in self.all_rdtypes:
                     # continue if a wildcard was already found for this rdtype
                     # if rdtype in self._wildcard_cache[host_hash]:
                     #     continue
                     for _ in range(self.wildcard_tests):
                         rand_query = f"{rand_string(digits=False, length=10)}.{host}"
-                        future = self.submit_task(
-                            self._catch_keyboardinterrupt,
-                            self.resolve,
-                            rand_query,
-                            type=rdtype,
-                            cache_result=False,
+                        wildcard_tasks[rdtype].append(
+                            asyncio.create_task(self.resolve(rand_query, type=rdtype, cache_result=False))
                         )
-                        if future is None:
-                            break
-                        wildcard_futures[future] = rdtype
 
                 # combine the random results
                 is_wildcard = False
                 wildcard_results = dict()
-                for future in self.parent_helper.as_completed(wildcard_futures):
-                    results = future.result()
-                    rdtype = wildcard_futures[future]
-                    if results:
-                        is_wildcard = True
-                    if results:
-                        if not rdtype in wildcard_results:
-                            wildcard_results[rdtype] = set()
-                        wildcard_results[rdtype].update(results)
+                for rdtype, tasks in wildcard_tasks.items():
+                    for task in asyncio.as_completed(tasks):
+                        results = await task
+                        if results:
+                            is_wildcard = True
+                            if not rdtype in wildcard_results:
+                                wildcard_results[rdtype] = set()
+                            wildcard_results[rdtype].update(results)
 
                 self._wildcard_cache.update({host_hash: wildcard_results})
                 wildcard_domain_results.update({host: wildcard_results})
                 if is_wildcard:
                     wildcard_rdtypes_str = ",".join(sorted([t.upper() for t, r in wildcard_results.items() if r]))
                     log_fn = log.verbose
                     if log_info:
                         log_fn = log.info
                     log_fn(f"Encountered domain with wildcard DNS ({wildcard_rdtypes_str}): {host}")
 
         return wildcard_domain_results
 
-    def _catch_keyboardinterrupt(self, callback, *args, **kwargs):
-        try:
-            return callback(*args, **kwargs)
-        except Exception as e:
-            log.error(f"Error in {callback.__qualname__}(): {e}")
-            log.trace(traceback.format_exc())
-        except KeyboardInterrupt:
-            if self.parent_helper.scan:
-                self.parent_helper.scan.stop()
-
     def debug(self, *args, **kwargs):
         if self._debug:
             log.debug(*args, **kwargs)
 
     def _get_dummy_module(self, name):
-        with self._dummy_modules_lock:
-            try:
-                dummy_module = self._dummy_modules[name]
-            except KeyError:
-                dummy_module = self.parent_helper._make_dummy_module(name=name, _type="DNS")
-                self._dummy_modules[name] = dummy_module
+        try:
+            dummy_module = self._dummy_modules[name]
+        except KeyError:
+            dummy_module = self.parent_helper._make_dummy_module(name=name, _type="DNS")
+            self._dummy_modules[name] = dummy_module
         return dummy_module
-
-    def dns_warning(self, msg):
-        msg_hash = hash(msg)
-        if msg_hash not in self._dns_warnings:
-            log.warning(msg)
-            self._dns_warnings.add(msg_hash)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
 import logging
 from pathlib import Path
 from threading import Lock
 
 from . import misc
 from .dns import DNSHelper
+from .web import WebHelper
 from .diff import HttpCompare
 from .wordcloud import WordCloud
 from .cloud import CloudProviders
 from .interactsh import Interactsh
-from .threadpool import as_completed
 from ...scanner.target import Target
 from ...modules.base import BaseModule
 from .depsinstaller import DepsInstaller
 
 
 log = logging.getLogger("bbot.core.helpers")
 
 
 class ConfigAwareHelper:
-    from .web import wordlist, request, download, api_page_iter, curl
-    from .cache import cache_get, cache_put, cache_filename, is_cached, CacheDict
-    from .command import run, run_live, _prepare_command_kwargs, tempfile, feed_pipe, _feed_pipe, tempfile_tail
     from . import ntlm
     from . import regexes
     from . import validators
+    from .files import tempfile, feed_pipe, _feed_pipe, tempfile_tail
+    from .command import run, run_live, _spawn_proc, _prepare_command_kwargs
+    from .cache import cache_get, cache_put, cache_filename, is_cached, CacheDict
 
     def __init__(self, config, scan=None):
         self.config = config
         self._scan = scan
         self.bbot_home = Path(self.config.get("home", "~/.bbot")).expanduser().resolve()
         self.cache_dir = self.bbot_home / "cache"
         self.temp_dir = self.bbot_home / "temp"
@@ -42,32 +42,36 @@
         self.mkdir(self.temp_dir)
         self.mkdir(self.tools_dir)
         self.mkdir(self.lib_dir)
         self._futures = set()
         self._future_lock = Lock()
 
         self.dns = DNSHelper(self)
+        self.web = WebHelper(self)
         self.depsinstaller = DepsInstaller(self)
         self.word_cloud = WordCloud(self)
         self.dummy_modules = {}
 
         # cloud helpers
         self.cloud = CloudProviders(self)
 
     def interactsh(self):
         return Interactsh(self)
 
     def http_compare(self, url, allow_redirects=False, include_cache_buster=True):
         return HttpCompare(url, self, allow_redirects=allow_redirects, include_cache_buster=include_cache_buster)
 
-    def temp_filename(self):
+    def temp_filename(self, extension=None):
         """
         temp_filename() --> Path("/home/user/.bbot/temp/pgxml13bov87oqrvjz7a")
         """
-        return self.temp_dir / self.rand_string(20)
+        filename = self.rand_string(20)
+        if extension is not None:
+            filename = f"{filename}.{extension}"
+        return self.temp_dir / filename
 
     def clean_old_scans(self):
         _filter = lambda x: x.is_dir() and self.regexes.scan_name_regex.match(x.name)
         self.clean_old(self.scans_dir, keep=self.keep_old_scans, filter=_filter)
 
     def make_target(self, events):
         return Target(self.scan, *events)
@@ -77,25 +81,17 @@
         if self._scan is None:
             from bbot.scanner import Scanner
 
             self._scan = Scanner()
         return self._scan
 
     @property
-    def scan_stopping(self):
-        return getattr(self.scan, "stopping", False)
-
-    @property
     def in_tests(self):
         return os.environ.get("BBOT_TESTING", "") == "True"
 
-    @staticmethod
-    def as_completed(*args, **kwargs):
-        return as_completed(*args, **kwargs)
-
     def _make_dummy_module(self, name, _type="scan"):
         """
         Construct a dummy module, for attachment to events
         """
         try:
             return self.dummy_modules[name]
         except KeyError:
@@ -115,16 +111,20 @@
                 # then try misc
                 return getattr(misc, attr)
             except AttributeError:
                 try:
                     # then try dns
                     return getattr(self.dns, attr)
                 except AttributeError:
-                    # then die
-                    raise AttributeError(f'Helper has no attribute "{attr}"')
+                    try:
+                        # then try web
+                        return getattr(self.web, attr)
+                    except AttributeError:
+                        # then die
+                        raise AttributeError(f'Helper has no attribute "{attr}"')
 
 
 class DummyModule(BaseModule):
     _priority = 4
 
     def __init__(self, *args, **kwargs):
         self._name = kwargs.pop("name")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/interactsh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # based on https://github.com/ElSicarius/interactsh-python/blob/main/sources/interactsh.py
 import json
 import base64
 import random
+import asyncio
 import logging
 import traceback
-from time import sleep
 from uuid import uuid4
-from threading import Thread
 
 from Crypto.Hash import SHA256
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import AES, PKCS1_OAEP
 
 from bbot.core.errors import InteractshError
 
@@ -22,17 +21,17 @@
 class Interactsh:
     def __init__(self, parent_helper):
         self.parent_helper = parent_helper
         self.server = None
         self.correlation_id = None
         self.custom_server = self.parent_helper.config.get("interactsh_server", None)
         self.token = self.parent_helper.config.get("interactsh_token", None)
-        self._thread = None
+        self._poll_task = None
 
-    def register(self, callback=None):
+    async def register(self, callback=None):
         rsa = RSA.generate(1024)
 
         self.public_key = rsa.publickey().exportKey()
         self.private_key = rsa.exportKey()
 
         encoded_public_key = base64.b64encode(self.public_key).decode("utf8")
 
@@ -53,15 +52,17 @@
         for server in self.server_list:
             log.info(f"Registering with interact.sh server: {server}")
             data = {
                 "public-key": encoded_public_key,
                 "secret-key": self.secret,
                 "correlation-id": self.correlation_id,
             }
-            r = self.parent_helper.request(f"https://{server}/register", headers=headers, json=data, method="POST")
+            r = await self.parent_helper.request(
+                f"https://{server}/register", headers=headers, json=data, method="POST"
+            )
             if r is None:
                 continue
             try:
                 msg = r.json().get("message", "")
                 assert "registration successful" in msg
             except Exception:
                 log.debug(f"Failed to register with interactsh server {self.server}")
@@ -74,73 +75,81 @@
             raise InteractshError(f"Failed to register with an interactsh server")
 
         log.info(
             f"Successfully registered to interactsh server {self.server} with correlation_id {self.correlation_id} [{self.domain}]"
         )
 
         if callable(callback):
-            self._thread = Thread(target=self.poll_loop, args=(callback,), daemon=True)
-            self._thread.start()
+            self._poll_task = asyncio.create_task(self.poll_loop(callback))
 
         return self.domain
 
-    def deregister(self):
+    async def deregister(self):
         if not self.server or not self.correlation_id or not self.secret:
             raise InteractshError(f"Missing required information to deregister")
 
         headers = {}
         if self.token:
             headers["Authorization"] = self.token
 
         data = {"secret-key": self.secret, "correlation-id": self.correlation_id}
 
-        r = self.parent_helper.request(f"https://{self.server}/deregister", headers=headers, json=data, method="POST")
+        r = await self.parent_helper.request(
+            f"https://{self.server}/deregister", headers=headers, json=data, method="POST"
+        )
+
+        if self._poll_task is not None:
+            self._poll_task.cancel()
+
         if "success" not in getattr(r, "text", ""):
             raise InteractshError(f"Failed to de-register with interactsh server {self.server}")
 
-    def poll(self):
+    async def poll(self):
         if not self.server or not self.correlation_id or not self.secret:
             raise InteractshError(f"Missing required information to poll")
 
         headers = {}
         if self.token:
             headers["Authorization"] = self.token
 
-        r = self.parent_helper.request(
+        r = await self.parent_helper.request(
             f"https://{self.server}/poll?id={self.correlation_id}&secret={self.secret}", headers=headers
         )
 
+        ret = []
         data_list = r.json().get("data", None)
         if data_list:
             aes_key = r.json()["aes_key"]
 
             for data in data_list:
                 decrypted_data = self.decrypt(aes_key, data)
-                yield decrypted_data
+                ret.append(decrypted_data)
+        return ret
 
-    def poll_loop(self, callback):
-        return self.parent_helper.scan.manager.catch(self._poll_loop, callback, _force=True)
+    async def poll_loop(self, callback):
+        async with self.parent_helper.scan.acatch(context=self._poll_loop):
+            return await self._poll_loop(callback)
 
-    def _poll_loop(self, callback):
+    async def _poll_loop(self, callback):
         while 1:
             if self.parent_helper.scan.stopping:
-                sleep(1)
+                await asyncio.sleep(1)
                 continue
             data_list = []
             try:
-                data_list = list(self.poll())
+                data_list = await self.poll()
             except InteractshError as e:
                 log.warning(e)
                 log.trace(traceback.format_exc())
             if not data_list:
-                sleep(10)
+                await asyncio.sleep(10)
                 continue
             for data in data_list:
                 if data:
-                    callback(data)
+                    await self.parent_helper.execute_sync_or_async(callback, data)
 
     def decrypt(self, aes_key, data):
         private_key = RSA.importKey(self.private_key)
         cipher = PKCS1_OAEP.new(private_key, hashAlgo=SHA256)
         aes_plain_key = cipher.decrypt(base64.b64decode(aes_key))
         decode = base64.b64decode(data)
         bs = AES.block_size
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     levelname = level.upper()
     if not any(x in sys.argv for x in ("-s", "--silent")):
         levelshort = f"[{loglevel_mapping.get(level, 'INFO')}]"
         levelshort = f"{colorize(levelshort, level=levelname)}"
         if levelname == "CRITICAL" or levelname.startswith("HUGE"):
             msg = colorize(msg, level=levelname)
         if logname:
-            msg = f"{levelshort} bbot: {msg}"
+            msg = f"{levelshort} {msg}"
         print(msg, file=sys.stderr)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import atexit
 import codecs
 import psutil
 import random
 import shutil
 import signal
 import string
+import asyncio
 import difflib
 import inspect
 import logging
 import platform
 import ipaddress
 import traceback
 import subprocess as sp
@@ -21,16 +22,18 @@
 from itertools import islice
 from datetime import datetime
 from tabulate import tabulate
 import wordninja as _wordninja
 from contextlib import suppress
 import cloudcheck as _cloudcheck
 import tldextract as _tldextract
+from collections.abc import Mapping
 from hashlib import sha1 as hashlib_sha1
 from urllib.parse import urlparse, quote, unquote, urlunparse  # noqa F401
+from asyncio import as_completed, create_task, sleep, wait_for  # noqa
 
 from .url import *  # noqa F401
 from . import regexes
 from .. import errors
 from .punycode import *  # noqa F401
 from .logger import log_to_stderr
 from .names_generator import random_name, names, adjectives  # noqa F401
@@ -39,25 +42,27 @@
 
 
 def is_domain(d):
     """
     "evilcorp.co.uk" --> True
     "www.evilcorp.co.uk" --> False
     """
+    d, _ = split_host_port(d)
     extracted = tldextract(d)
     if extracted.domain and not extracted.subdomain:
         return True
     return False
 
 
 def is_subdomain(d):
     """
     "www.evilcorp.co.uk" --> True
     "evilcorp.co.uk" --> False
     """
+    d, _ = split_host_port(d)
     extracted = tldextract(d)
     if extracted.domain and extracted.subdomain:
         return True
     return False
 
 
 def is_ptr(d):
@@ -103,33 +108,35 @@
     if not "://" in d:
         d = f"d://{d}"
     parsed = urlparse(d)
     port = None
     host = None
     with suppress(ValueError):
         if parsed.port is None:
-            if parsed.scheme == "https":
+            if parsed.scheme in ("https", "wss"):
                 port = 443
-            elif parsed.scheme == "http":
+            elif parsed.scheme in ("http", "ws"):
                 port = 80
         else:
             port = int(parsed.port)
     with suppress(ValueError):
         host = parsed.hostname
     return make_ip_type(host), port
 
 
 def parent_domain(d):
     """
     "www.internal.evilcorp.co.uk" --> "internal.evilcorp.co.uk"
+    "www.internal.evilcorp.co.uk:8080" --> "internal.evilcorp.co.uk:8080"
     "www.evilcorp.co.uk" --> "evilcorp.co.uk"
     "evilcorp.co.uk" --> "evilcorp.co.uk"
     """
+    host, port = split_host_port(d)
     if is_subdomain(d):
-        return ".".join(str(d).split(".")[1:])
+        return make_netloc(".".join(str(host).split(".")[1:]), port)
     return d
 
 
 def domain_parents(d, include_self=False):
     """
     "test.www.evilcorp.co.uk" --> ["www.evilcorp.co.uk", "evilcorp.co.uk"]
     """
@@ -204,14 +211,25 @@
 
 
 def is_port(p):
     p = str(p)
     return p and p.isdigit() and 0 <= int(p) <= 65535
 
 
+def is_dns_name(d):
+    if is_ip(d):
+        return False
+    d = smart_decode(d)
+    if regexes.hostname_regex.match(d):
+        return True
+    if regexes.dns_name_regex.match(d):
+        return True
+    return False
+
+
 def is_ip(d, version=None):
     """
     "192.168.1.1" --> True
     "bad::c0de" --> True
     "evilcorp.com" --> False
     """
     if type(d) in (ipaddress.IPv4Address, ipaddress.IPv6Address):
@@ -528,18 +546,21 @@
         for p in range(1, padding + 1):
             results.add(str(i).zfill(p))
     return results
 
 
 def make_netloc(host, port):
     """
+    ("192.168.1.1", None) --> "192.168.1.1"
     ("192.168.1.1", 443) --> "192.168.1.1:443"
     ("evilcorp.com", 80) --> "evilcorp.com:80"
     ("dead::beef", 443) --> "[dead::beef]:443"
     """
+    if port is None:
+        return host
     if is_ip(host, version=6):
         host = f"[{host}]"
     return f"{host}:{port}"
 
 
 def which(*executables):
     """
@@ -564,25 +585,26 @@
     elif isinstance(d, list):
         for v in d:
             yield from search_dict_by_key(key, v)
 
 
 def search_format_dict(d, **kwargs):
     """
-    Recursively .format() string values in dictionary keys
-    search_format_dict({"test": "{name} is awesome"}, name="keanu")
+    Recursively .format() string values in dictionary values
+    search_format_dict({"test": "#{name} is awesome"}, name="keanu")
         --> {"test": "keanu is awesome"}
     """
     if isinstance(d, dict):
         return {k: search_format_dict(v, **kwargs) for k, v in d.items()}
     elif isinstance(d, list):
         return [search_format_dict(v, **kwargs) for v in d]
     elif isinstance(d, str):
-        for k, v in kwargs.items():
-            d = d.replace("#{" + str(k) + "}", v)
+        for find, replace in kwargs.items():
+            find = "#{" + str(find) + "}"
+            d = d.replace(find, replace)
     return d
 
 
 def filter_dict(d, *key_names, fuzzy=False, invert=False, exclude_keys=None, prev_key=None):
     """
     Recursively filter a dictionary based on key names
     filter_dict({"key1": "test", "key2": "asdf"}, "key2")
@@ -916,22 +938,22 @@
         return "macOS"
     return p
 
 
 tag_filter_regex = re.compile(r"[^a-z0-9]+")
 
 
-def tagify(s):
+def tagify(s, maxlen=None):
     """
     Sanitize a string into a tag-friendly format
 
     tagify("HTTP Web Title") --> "http-web-title"
     """
     ret = str(s).lower()
-    return tag_filter_regex.sub("-", ret).strip("-")
+    return tag_filter_regex.sub("-", ret)[:maxlen].strip("-")
 
 
 def memory_status():
     """
     Return statistics on system memory consumption
 
     Example: to get available memory (not including swap):
@@ -954,50 +976,52 @@
         swap_status().used
     """
     return psutil.swap_memory()
 
 
 def get_size(obj, max_depth=5, seen=None):
     """
-    Recursively get size of object in bytes
+    Rough recursive measurement of a python object's memory footprint
     """
-    size = 0
-    if max_depth <= 0:
-        return size
+    # If seen is not provided, initialize an empty set
+    if seen is None:
+        seen = set()
+    # Get the id of the object
+    obj_id = id(obj)
+    # Decrease the maximum depth for the next recursion
     new_max_depth = max_depth - 1
-    try:
-        size = sys.getsizeof(obj)
-        if seen is None:
-            seen = set()
-        obj_id = id(obj)
-        if obj_id in seen:
-            return 0
-        # Important mark as seen *before* entering recursion to gracefully handle
-        # self-referential objects
-        seen.add(obj_id)
-        if hasattr(obj, "__dict__"):
-            for _cls in obj.__class__.__mro__:
-                if "__dict__" in _cls.__dict__:
-                    d = _cls.__dict__["__dict__"]
-                    if inspect.isgetsetdescriptor(d) or inspect.ismemberdescriptor(d):
-                        size += get_size(obj.__dict__, max_depth=new_max_depth, seen=seen)
-                    break
-        if isinstance(obj, dict):
-            size += sum((get_size(v, max_depth=new_max_depth, seen=seen) for v in obj.values()))
-            size += sum((get_size(k, max_depth=new_max_depth, seen=seen) for k in obj.keys()))
-        # elif hasattr(obj, "__iter__") and not isinstance(obj, (str, bytes, bytearray)):
-        #     size += sum((get_size(i, seen) for i in obj))
-        if hasattr(obj, "__slots__"):  # can have __slots__ with __dict__
-            size += sum(
-                get_size(getattr(obj, s), max_depth=new_max_depth, seen=seen) for s in obj.__slots__ if hasattr(obj, s)
-            )
-    except Exception as e:
-        log.debug(f"Error getting size of {obj}: {e}")
-        log.trace(traceback.format_exc())
-
+    # If the object has already been seen or we've reached the maximum recursion depth, return 0
+    if obj_id in seen or new_max_depth <= 0:
+        return 0
+    # Get the size of the object
+    size = sys.getsizeof(obj)
+    # Add the object's id to the set of seen objects
+    seen.add(obj_id)
+    # If the object has a __dict__ attribute, we want to measure its size
+    if hasattr(obj, "__dict__"):
+        # Iterate over the Method Resolution Order (MRO) of the class of the object
+        for cls in obj.__class__.__mro__:
+            # If the class's __dict__ contains a __dict__ key
+            if "__dict__" in cls.__dict__:
+                for k, v in obj.__dict__.items():
+                    size += get_size(k, new_max_depth, seen)
+                    size += get_size(v, new_max_depth, seen)
+                break
+    # If the object is a mapping (like a dictionary), we want to measure the size of its items
+    if isinstance(obj, Mapping):
+        with suppress(StopIteration):
+            k, v = next(iter(obj.items()))
+            size += (get_size(k, new_max_depth, seen) + get_size(v, new_max_depth, seen)) * len(obj)
+    # If the object is a container (like a list or tuple) but not a string or bytes-like object
+    elif isinstance(obj, (list, tuple, set)):
+        with suppress(StopIteration):
+            size += get_size(next(iter(obj)), new_max_depth, seen) * len(obj)
+    # If the object has __slots__, we want to measure the size of the attributes in __slots__
+    if hasattr(obj, "__slots__"):
+        size += sum(get_size(getattr(obj, s), new_max_depth, seen) for s in obj.__slots__ if hasattr(obj, s))
     return size
 
 
 def is_file(f):
     with suppress(Exception):
         return Path(f).is_file()
     return False
@@ -1016,7 +1040,82 @@
         print(subnet) # IPv4Network('168.62.0.0/19')
     """
     provider, provider_type, subnet = _cloudcheck.check(ip)
     if provider:
         with suppress(KeyError):
             provider = provider_map[provider.lower()]
     return provider, provider_type, subnet
+
+
+def is_async_function(f):
+    return inspect.iscoroutinefunction(f)
+
+
+async def execute_sync_or_async(callback, *args, **kwargs):
+    if is_async_function(callback):
+        return await callback(*args, **kwargs)
+    else:
+        return callback(*args, **kwargs)
+
+
+def get_exception_chain(e):
+    """
+    Get the full chain of exceptions that led to the current one
+    """
+    exception_chain = []
+    current_exception = e
+    while current_exception is not None:
+        exception_chain.append(current_exception)
+        current_exception = getattr(current_exception, "__context__", None)
+    return exception_chain
+
+
+def get_traceback_details(e):
+    tb = traceback.extract_tb(e.__traceback__)
+    last_frame = tb[-1]  # Get the last frame in the traceback (the one where the exception was raised)
+    filename = last_frame.filename
+    lineno = last_frame.lineno
+    funcname = last_frame.name
+    return filename, lineno, funcname
+
+
+async def cancel_tasks(tasks):
+    current_task = asyncio.current_task()
+    tasks = [t for t in tasks if t != current_task]
+    for task in tasks:
+        log.debug(f"Cancelling task: {task}")
+        task.cancel()
+    for task in tasks:
+        try:
+            await task
+        except asyncio.CancelledError:
+            log.trace(traceback.format_exc())
+
+
+def cancel_tasks_sync(tasks):
+    current_task = asyncio.current_task()
+    for task in tasks:
+        if task != current_task:
+            log.debug(f"Cancelling task: {task}")
+            task.cancel()
+
+
+def weighted_shuffle(items, weights):
+    # Create a list of tuples where each tuple is (item, weight)
+    pool = list(zip(items, weights))
+
+    shuffled_items = []
+
+    # While there are still items to be chosen...
+    while pool:
+        # Normalize weights
+        total = sum(weight for item, weight in pool)
+        weights = [weight / total for item, weight in pool]
+
+        # Choose an index based on weight
+        chosen_index = random.choices(range(len(pool)), weights=weights, k=1)[0]
+
+        # Add the chosen item to the shuffled list
+        chosen_item, chosen_weight = pool.pop(chosen_index)
+        shuffled_items.append(chosen_item)
+
+    return shuffled_items
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 import sys
 import importlib
+import traceback
 from pathlib import Path
 from omegaconf import OmegaConf
 from contextlib import suppress
 
 from .misc import list_files, sha1, search_dict_by_key, search_format_dict, make_table, os_platform
 
 
@@ -37,16 +38,14 @@
                     preloaded["flags"] = list(set(preloaded["flags"] + [module_dir.name]))
                 preloaded["type"] = module_type
                 preloaded["namespace"] = namespace
                 config = OmegaConf.create(preloaded.get("config", {}))
                 self._configs[module_file.stem] = config
                 self._preloaded[module_file.stem] = preloaded
             except Exception:
-                import traceback
-
                 print(f"[CRIT] Error preloading {module_file}\n\n{traceback.format_exc()}")
                 print(f"[CRIT] Error in {module_file.name}")
                 sys.exit(1)
 
         return self.preloaded
 
     def preloaded(self, type=None):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/names_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     "benevolent",
     "bewildered",
     "bighuge",
     "black",
     "blazed",
     "bloodshot",
     "brown",
-    "carbonated",
     "cheeky",
     "childish",
     "chiseled",
     "cold",
     "considerate",
     "constipated",
     "contentious",
@@ -40,14 +39,15 @@
     "cuddly",
     "cute",
     "dark",
     "dastardly",
     "decrypted",
     "deep",
     "delicious",
+    "demented",
     "demonic",
     "depraved",
     "depressed",
     "deranged",
     "derogatory",
     "despicable",
     "devilish",
@@ -73,14 +73,15 @@
     "euphoric",
     "evil",
     "exquisite",
     "extreme",
     "ferocious",
     "fiendish",
     "fierce",
+    "flamboyant",
     "fleecy",
     "flirtatious",
     "flustered",
     "foreboding",
     "frenetic",
     "frolicking",
     "frothy",
@@ -123,14 +124,15 @@
     "intoxicated",
     "inventive",
     "irritable",
     "large",
     "liquid",
     "loveable",
     "lovely",
+    "lucid",
     "malevolent",
     "malfunctioning",
     "malicious",
     "manic",
     "masochistic",
     "medicated",
     "mediocre",
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/regexes.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 word_regex = re.compile(r"[^\d\W_]+")
 word_num_regex = re.compile(r"[^\W_]+")
 num_regex = re.compile(r"\d+")
 _ipv6_regex = r"[A-F0-9:]*:[A-F0-9:]*:[A-F0-9:]*"
 ipv6_regex = re.compile(_ipv6_regex, re.I)
 _dns_name_regex = r"(?:(?:[\w-]+)\.)+(?:[^\W_0-9]{2,20})"
-_hostname_regex = re.compile(r"^[\w-]+$")
+_hostname_regex = r"^[\w-]+$"
 _email_regex = r"(?:[^\W_][\w\-\.\+]{,100})@(?:\w[\w\-\._]{,100})\.(?:[^\W_0-9]{2,8})"
 email_regex = re.compile(_email_regex, re.I)
 _ptr_regex = r"(?:[0-9]{1,3}[-_\.]){3}[0-9]{1,3}"
 ptr_regex = re.compile(_ptr_regex)
 
 event_type_regexes = OrderedDict(
     [
@@ -57,7 +57,8 @@
         ]
     ]
 )
 
 event_id_regex = re.compile(r"[0-9a-f]{40}:[A-Z0-9_]+")
 dns_name_regex = re.compile(_dns_name_regex, re.I)
 scan_name_regex = re.compile(r"[a-z]{3,20}_[a-z]{3,20}")
+hostname_regex = re.compile(_hostname_regex, re.I)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/url.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,24 @@
 
     http://evilcorp.com:80 --> http://evilcorp.com/
     http://eViLcORp.com/ --> http://evilcorp.com/
     http://evilcorp.com/api?user=bob#place --> http://evilcorp.com/api
     """
     parsed = parse_url(url)
     parsed = parsed._replace(netloc=str(parsed.netloc).lower(), fragment="", query="")
+    try:
+        scheme = parsed.scheme
+    except ValueError:
+        scheme = "https"
+    try:
+        port = parsed.port
+    except ValueError:
+        port = 80 if scheme == "http" else 443
     # remove ports if they're redundant
-    if (parsed.scheme == "http" and parsed.port == 80) or (parsed.scheme == "https" and parsed.port == 443):
+    if (scheme == "http" and port == 80) or (scheme == "https" and port == 443):
         hostname = parsed.hostname
         # special case for IPv6 URLs
         if parsed.netloc.startswith("["):
             hostname = f"[{hostname}]"
         # punycode
         hostname = smart_decode_punycode(hostname)
         parsed = parsed._replace(netloc=hostname)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             # finally, try DNS_NAME
             host = smart_decode_punycode(host)
             # clean asterisks and clinging dashes
             host = host.strip("*.-").replace("*", "")
             for r in regexes.event_type_regexes["DNS_NAME"]:
                 if r.match(host):
                     return host
-            if regexes._hostname_regex.match(host):
+            if regexes.hostname_regex.match(host):
                 return host
     assert False, f'Invalid hostname: "{host}"'
 
 
 @validator
 def validate_url(url):
     return validate_url_parsed(url).geturl()
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/web.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,282 +1,356 @@
+import re
+import ssl
+import httpx
 import logging
-import requests
-from time import sleep
+import traceback
 from pathlib import Path
-from requests_cache import CachedSession
-from requests.adapters import HTTPAdapter
-from requests_cache.backends import SQLiteCache
-from requests.exceptions import RequestException
+from bs4 import BeautifulSoup
 
 from bbot.core.errors import WordlistError, CurlError
+from bbot.core.helpers.ratelimiter import RateLimiter
 
 log = logging.getLogger("bbot.core.helpers.web")
 
 
-def wordlist(self, path, lines=None, **kwargs):
-    if not path:
-        raise WordlistError(f"Invalid wordlist: {path}")
-    if not "cache_hrs" in kwargs:
-        kwargs["cache_hrs"] = 720
-    if self.is_url(path):
-        filename = self.download(str(path), **kwargs)
-        if filename is None:
-            raise WordlistError(f"Unable to retrieve wordlist from {path}")
-    else:
-        filename = Path(path).resolve()
-        if not filename.is_file():
-            raise WordlistError(f"Unable to find wordlist at {path}")
-
-    if lines is None:
-        return filename
-    else:
-        lines = int(lines)
-        with open(filename) as f:
-            read_lines = f.readlines()
-        cache_key = f"{filename}:{lines}"
-        truncated_filename = self.cache_filename(cache_key)
-        with open(truncated_filename, "w") as f:
-            for line in read_lines[:lines]:
-                f.write(line)
-        return truncated_filename
+class BBOTAsyncClient(httpx.AsyncClient):
+    def __init__(self, *args, **kwargs):
+        self._bbot_scan = kwargs.pop("_bbot_scan")
 
+        # timeout
+        http_timeout = self._bbot_scan.config.get("http_timeout", 20)
+        if not "timeout" in kwargs:
+            kwargs["timeout"] = http_timeout
 
-def download(self, url, **kwargs):
-    """
-    Downloads file, returns full path of filename
-    If download failed, returns None
+        # headers
+        headers = kwargs.get("headers", None)
+        if headers is None:
+            headers = {}
+        user_agent = self._bbot_scan.config.get("user_agent", "BBOT")
+        if "User-Agent" not in headers:
+            headers["User-Agent"] = user_agent
+        kwargs["headers"] = headers
 
-    Caching supported via "cache_hrs"
-    """
-    success = False
-    filename = self.cache_filename(url)
-    cache_hrs = float(kwargs.pop("cache_hrs", -1))
-    log.debug(f"Downloading file from {url} with cache_hrs={cache_hrs}")
-    if cache_hrs > 0 and self.is_cached(url):
-        log.debug(f"{url} is cached")
-        success = True
-    else:
-        method = kwargs.get("method", "GET")
-        try:
-            with self.request(method=method, url=url, stream=True, raise_error=True, **kwargs) as response:
-                status_code = getattr(response, "status_code", 0)
-                log.debug(f"Download result: HTTP {status_code}")
-                if status_code != 0:
-                    response.raise_for_status()
-                    with open(filename, "wb") as f:
-                        for chunk in response.iter_content(chunk_size=8192):
-                            f.write(chunk)
-                    success = True
-        except RequestException as e:
-            log.warning(f"Failed to download {url}: {e}")
-            return
-        except AttributeError:
-            return
+        super().__init__(*args, **kwargs)
 
-    if success:
-        return filename.resolve()
+    def build_request(self, *args, **kwargs):
+        request = super().build_request(*args, **kwargs)
+        # add custom headers if the URL is in-scope
+        if self._bbot_scan.in_scope(str(request.url)):
+            for hk, hv in self._bbot_scan.config.get("http_headers", {}).items():
+                # don't clobber headers
+                if hk not in request.headers:
+                    request.headers[hk] = hv
+        return request
 
 
-def request(self, *args, **kwargs):
+class WebHelper:
     """
-    Multipurpose function for making web requests
-
-    Supports custom sessions
-        session Request.Session()
-
-    Arguments
-        cache_for (Union[None, int, float, str, datetime, timedelta]): Cache response for <int> seconds
-        raise_error (bool): Whether to raise exceptions (default: False)
+    For making HTTP requests
     """
 
-    # we handle our own retries
-    retries = kwargs.pop("retries", self.config.get("http_retries", 1))
-    if getattr(self, "retry_adapter", None) is None:
-        self.retry_adapter = HTTPAdapter(max_retries=0)
-
-    raise_error = kwargs.pop("raise_error", False)
-
-    cache_for = kwargs.pop("cache_for", None)
-    if cache_for is not None:
-        log.debug(f"Caching HTTP session with expire_after={cache_for}")
-        db_path = str(self.cache_dir / "requests-cache.sqlite")
-        backend = SQLiteCache(db_path=db_path)
-        session = CachedSession(expire_after=cache_for, backend=backend)
-        session.mount("http://", self.retry_adapter)
-        session.mount("https://", self.retry_adapter)
-    elif kwargs.get("session", None) is not None:
-        session = kwargs.pop("session", None)
-        session.mount("http://", self.retry_adapter)
-        session.mount("https://", self.retry_adapter)
-    else:
-        session = requests.Session()
-        session.mount("http://", self.retry_adapter)
-        session.mount("https://", self.retry_adapter)
-
-    http_timeout = self.config.get("http_timeout", 20)
-    user_agent = self.config.get("user_agent", "BBOT")
-
-    # in case of URL only, assume GET request
-    if len(args) == 1:
-        kwargs["url"] = args[0]
-        args = []
-
-    url = kwargs.get("url", "")
-
-    if not args and "method" not in kwargs:
-        kwargs["method"] = "GET"
-
-    if not "timeout" in kwargs:
-        kwargs["timeout"] = http_timeout
-
-    headers = kwargs.get("headers", None)
-
-    if headers is None:
-        headers = {}
-    if "User-Agent" not in headers:
-        headers.update({"User-Agent": user_agent})
-    # only add custom headers if the URL is in-scope
-    if self.scan.in_scope(url):
-        for hk, hv in self.scan.config.get("http_headers", {}).items():
-            # don't clobber headers
-            if hk not in headers:
-                headers[hk] = hv
-    kwargs["headers"] = headers
-
-    http_debug = self.config.get("http_debug", False)
-    while retries == "infinite" or retries >= 0:
-        try:
-            if http_debug:
-                logstr = f"Web request: {str(args)}, {str(kwargs)}"
-                log.debug(logstr)
-            if session is not None:
-                response = session.request(*args, **kwargs)
+    client_options = (
+        "auth",
+        "params",
+        "headers",
+        "retries",
+        "cookies",
+        "verify",
+        "timeout",
+        "follow_redirects",
+        "max_redirects",
+    )
+
+    def __init__(self, parent_helper):
+        self.parent_helper = parent_helper
+        self.ssl_verify = self.parent_helper.config.get("ssl_verify", False)
+        self.web_requests_per_second = self.parent_helper.config.get("web_requests_per_second", 50)
+        self.web_rate_limiter = RateLimiter(self.web_requests_per_second, "Web")
+
+    def AsyncClient(self, *args, **kwargs):
+        kwargs["_bbot_scan"] = self.parent_helper.scan
+        retries = kwargs.pop("retries", self.parent_helper.config.get("http_retries", 1))
+        kwargs["transport"] = httpx.AsyncHTTPTransport(retries=retries, verify=self.ssl_verify)
+        return BBOTAsyncClient(*args, **kwargs)
+
+    async def request(self, *args, **kwargs):
+        raise_error = kwargs.pop("raise_error", False)
+        # TODO: use this
+        cache_for = kwargs.pop("cache_for", None)  # noqa
+
+        # allow vs follow, httpx why??
+        allow_redirects = kwargs.pop("allow_redirects", None)
+        if allow_redirects is not None and "follow_redirects" not in kwargs:
+            kwargs["follow_redirects"] = allow_redirects
+
+        # in case of URL only, assume GET request
+        if len(args) == 1:
+            kwargs["url"] = args[0]
+            args = []
+
+        if not args and "method" not in kwargs:
+            kwargs["method"] = "GET"
+
+        http_debug = self.parent_helper.config.get("http_debug", False)
+
+        client_kwargs = {}
+        for k in list(kwargs):
+            if k in self.client_options:
+                v = kwargs.pop(k)
+                client_kwargs[k] = v
+        async with self.AsyncClient(**client_kwargs) as client:
+            try:
+                if http_debug:
+                    logstr = f"Web request: {str(args)}, {str(kwargs)}"
+                    log.debug(logstr)
+                async with self.web_rate_limiter:
+                    response = await client.request(*args, **kwargs)
+                if http_debug:
+                    log.debug(
+                        f"Web response: {response} (Length: {len(response.content)}) headers: {response.headers}"
+                    )
+                return response
+            except httpx.RequestError as e:
+                log.debug(f"Error with request: {e}")
+                if raise_error:
+                    raise
+            except ssl.SSLError as e:
+                log.debug(f"SSL error with request: {e}")
+
+    async def download(self, url, **kwargs):
+        """
+        Downloads file, returns full path of filename
+        If download failed, returns None
+
+        Caching supported via "cache_hrs"
+        """
+        success = False
+        filename = self.parent_helper.cache_filename(url)
+        cache_hrs = float(kwargs.pop("cache_hrs", -1))
+        log.debug(f"Downloading file from {url} with cache_hrs={cache_hrs}")
+        if cache_hrs > 0 and self.parent_helper.is_cached(url):
+            log.debug(f"{url} is cached at {self.parent_helper.cache_filename(url)}")
+            success = True
+        else:
+            # kwargs["raise_error"] = True
+            # kwargs["stream"] = True
+            if not "method" in kwargs:
+                kwargs["method"] = "GET"
+            try:
+                async with self.AsyncClient().stream(url=url, **kwargs) as response:
+                    status_code = getattr(response, "status_code", 0)
+                    log.debug(f"Download result: HTTP {status_code}")
+                    if status_code != 0:
+                        response.raise_for_status()
+                        with open(filename, "wb") as f:
+                            async for chunk in response.aiter_bytes(chunk_size=8192):
+                                f.write(chunk)
+                        success = True
+            except httpx.HTTPError as e:
+                log.warning(f"Failed to download {url}: {e}")
+                return
+
+        if success:
+            return filename.resolve()
+
+    async def wordlist(self, path, lines=None, **kwargs):
+        if not path:
+            raise WordlistError(f"Invalid wordlist: {path}")
+        if not "cache_hrs" in kwargs:
+            kwargs["cache_hrs"] = 720
+        if self.parent_helper.is_url(path):
+            filename = await self.download(str(path), **kwargs)
+            if filename is None:
+                raise WordlistError(f"Unable to retrieve wordlist from {path}")
+        else:
+            filename = Path(path).resolve()
+            if not filename.is_file():
+                raise WordlistError(f"Unable to find wordlist at {path}")
+
+        if lines is None:
+            return filename
+        else:
+            lines = int(lines)
+            with open(filename) as f:
+                read_lines = f.readlines()
+            cache_key = f"{filename}:{lines}"
+            truncated_filename = self.parent_helper.cache_filename(cache_key)
+            with open(truncated_filename, "w") as f:
+                for line in read_lines[:lines]:
+                    f.write(line)
+            return truncated_filename
+
+    async def api_page_iter(self, url, page_size=100, json=True, next_key=None, **requests_kwargs):
+        """
+        An async generator to fetch and loop through API pages.
+
+        This function keeps calling the API with the provided URL, increasing the page number each time, and spits out
+        the results one page at a time. It's perfect for APIs that split their data across multiple pages.
+
+        Args:
+            url (str): The API endpoint. May contain placeholders for 'page' and 'page_size'.
+            page_size (int, optional): How many items you want per page. Defaults to 100.
+            json (bool, optional): If True, we'll try to convert the response to JSON. Defaults to True.
+            next_key (callable, optional): If your API has a weird way to get to the next page, give us a function
+                                           that takes the response and spits out the new URL. Defaults to None.
+            **requests_kwargs: Any other stuff you want to pass to the request.
+
+        Yields:
+            If 'json' is True, you'll get a dict with the API's response, else you'll get the raw response.
+
+        Note:
+            You MUST break out of the loop when you stop getting useful results! Otherwise it will loop forever.
+
+        Example:
+            Here's a quick example of how to use this:
+            ```
+            agen = api_page_iter('https://api.example.com/data?page={page}&page_size={page_size}')
+            try:
+                async for page in agen:
+                    subdomains = json["subdomains"]
+                    self.hugesuccess(subdomains)
+                    if not subdomains:
+                        break
+            finally:
+                agen.aclose()
+            ```
+        """
+        page = 1
+        offset = 0
+        result = None
+        while 1:
+            if result and callable(next_key):
+                try:
+                    new_url = next_key(result)
+                except Exception as e:
+                    log.debug(f"Failed to extract next page of results from {url}: {e}")
+                    log.debug(traceback.formate_exc())
             else:
-                response = requests.request(*args, **kwargs)
-            if http_debug:
-                log.debug(f"Web response: {response} (Length: {len(response.content)}) headers: {response.headers}")
-            return response
-        except RequestException as e:
-            log.debug(f"Error with request: {e}")
-            if self.parent_helper.scan_stopping:
+                new_url = url.format(page=page, page_size=page_size, offset=offset)
+            result = await self.request(new_url, **requests_kwargs)
+            try:
+                if json:
+                    result = result.json()
+                yield result
+            except Exception:
+                log.warning(f'Error in api_page_iter() for url: "{new_url}"')
+                log.trace(traceback.format_exc())
                 break
-            if retries != "infinite":
-                retries -= 1
-            if retries == "infinite" or retries >= 0:
-                log.verbose(f'Error requesting "{url}" ({e}), retrying...')
-                sleep(1)
-            else:
-                if raise_error:
-                    raise e
+            finally:
+                offset += page_size
+                page += 1
 
+    async def curl(self, *args, **kwargs):
+        url = kwargs.get("url", "")
 
-def api_page_iter(self, url, page_size=100, json=True, **requests_kwargs):
-    page = 1
-    offset = 0
-    while 1:
-        new_url = url.format(page=page, page_size=page_size, offset=offset)
-        result = self.request(new_url, **requests_kwargs)
-        try:
-            if json:
-                result = result.json()
-            yield result
-        except Exception:
-            import traceback
-
-            log.warning(f'Error in api_page_iter() for url: "{new_url}"')
-            log.trace(traceback.format_exc())
-            break
-        finally:
-            offset += page_size
-            page += 1
-
-
-def curl(self, *args, **kwargs):
-    url = kwargs.get("url", "")
-
-    if not url:
-        raise CurlError("No URL supplied to CURL helper")
-
-    curl_command = ["curl", url, "-s"]
-
-    raw_path = kwargs.get("raw_path", False)
-    if raw_path:
-        curl_command.append("--path-as-is")
-
-    # respect global ssl verify settings
-    ssl_verify = self.config.get("ssl_verify")
-    if ssl_verify == False:
-        curl_command.append("-k")
-
-    headers = kwargs.get("headers", {})
-
-    ignore_bbot_global_settings = kwargs.get("ignore_bbot_global_settings", False)
-
-    if ignore_bbot_global_settings:
-        log.debug("ignore_bbot_global_settings enabled. Global settings will not be applied")
-    else:
-        http_timeout = self.config.get("http_timeout", 20)
-        user_agent = self.config.get("user_agent", "BBOT")
+        if not url:
+            raise CurlError("No URL supplied to CURL helper")
 
-        if "User-Agent" not in headers:
-            headers["User-Agent"] = user_agent
+        curl_command = ["curl", url, "-s"]
 
-        # only add custom headers if the URL is in-scope
-        if self.scan.in_scope(url):
-            for hk, hv in self.scan.config.get("http_headers", {}).items():
-                headers[hk] = hv
+        raw_path = kwargs.get("raw_path", False)
+        if raw_path:
+            curl_command.append("--path-as-is")
 
-        # add the timeout
-        if not "timeout" in kwargs:
-            timeout = http_timeout
+        # respect global ssl verify settings
+        if self.ssl_verify == False:
+            curl_command.append("-k")
 
-        curl_command.append("-m")
-        curl_command.append(str(timeout))
+        headers = kwargs.get("headers", {})
 
-    for k, v in headers.items():
-        if isinstance(v, list):
-            for x in v:
-                curl_command.append("-H")
-                curl_command.append(f"{k}: {x}")
+        ignore_bbot_global_settings = kwargs.get("ignore_bbot_global_settings", False)
 
+        if ignore_bbot_global_settings:
+            log.debug("ignore_bbot_global_settings enabled. Global settings will not be applied")
         else:
-            curl_command.append("-H")
-            curl_command.append(f"{k}: {v}")
+            http_timeout = self.parent_helper.config.get("http_timeout", 20)
+            user_agent = self.parent_helper.config.get("user_agent", "BBOT")
+
+            if "User-Agent" not in headers:
+                headers["User-Agent"] = user_agent
+
+            # only add custom headers if the URL is in-scope
+            if self.parent_helper.scan.in_scope(url):
+                for hk, hv in self.parent_helper.scan.config.get("http_headers", {}).items():
+                    headers[hk] = hv
+
+            # add the timeout
+            if not "timeout" in kwargs:
+                timeout = http_timeout
+
+            curl_command.append("-m")
+            curl_command.append(str(timeout))
+
+        for k, v in headers.items():
+            if isinstance(v, list):
+                for x in v:
+                    curl_command.append("-H")
+                    curl_command.append(f"{k}: {x}")
+
+            else:
+                curl_command.append("-H")
+                curl_command.append(f"{k}: {v}")
 
-    post_data = kwargs.get("post_data", {})
-    if len(post_data.items()) > 0:
-        curl_command.append("-d")
-        post_data_str = ""
-        for k, v in post_data.items():
-            post_data_str += f"&{k}={v}"
-        curl_command.append(post_data_str.lstrip("&"))
-
-    method = kwargs.get("method", "")
-    if method:
-        curl_command.append("-X")
-        curl_command.append(method)
-
-    cookies = kwargs.get("cookies", "")
-    if cookies:
-        curl_command.append("-b")
-        cookies_str = ""
-        for k, v in cookies.items():
-            cookies_str += f"{k}={v}; "
-        curl_command.append(f'{cookies_str.rstrip(" ")}')
-
-    path_override = kwargs.get("path_override", None)
-    if path_override:
-        curl_command.append("--request-target")
-        curl_command.append(f"{path_override}")
-
-    head_mode = kwargs.get("head_mode", None)
-    if head_mode:
-        curl_command.append("-I")
-
-    raw_body = kwargs.get("raw_body", None)
-    if raw_body:
-        curl_command.append("-d")
-        curl_command.append(raw_body)
-
-    output_bytes = self.run(curl_command, text=False).stdout
-    output = self.smart_decode(output_bytes)
-    return output
+        post_data = kwargs.get("post_data", {})
+        if len(post_data.items()) > 0:
+            curl_command.append("-d")
+            post_data_str = ""
+            for k, v in post_data.items():
+                post_data_str += f"&{k}={v}"
+            curl_command.append(post_data_str.lstrip("&"))
+
+        method = kwargs.get("method", "")
+        if method:
+            curl_command.append("-X")
+            curl_command.append(method)
+
+        cookies = kwargs.get("cookies", "")
+        if cookies:
+            curl_command.append("-b")
+            cookies_str = ""
+            for k, v in cookies.items():
+                cookies_str += f"{k}={v}; "
+            curl_command.append(f'{cookies_str.rstrip(" ")}')
+
+        path_override = kwargs.get("path_override", None)
+        if path_override:
+            curl_command.append("--request-target")
+            curl_command.append(f"{path_override}")
+
+        head_mode = kwargs.get("head_mode", None)
+        if head_mode:
+            curl_command.append("-I")
+
+        raw_body = kwargs.get("raw_body", None)
+        if raw_body:
+            curl_command.append("-d")
+            curl_command.append(raw_body)
+
+        output = (await self.parent_helper.run(curl_command)).stdout
+        return output
+
+
+user_keywords = [re.compile(r, re.I) for r in ["user", "login", "email"]]
+pass_keywords = [re.compile(r, re.I) for r in ["pass"]]
+
+
+def is_login_page(html):
+    try:
+        soup = BeautifulSoup(html, "html.parser")
+    except Exception as e:
+        log.debug(f"Error parsing html: {e}")
+        return False
+
+    forms = soup.find_all("form")
+
+    # first, check for obvious password fields
+    for form in forms:
+        if form.find_all("input", {"type": "password"}):
+            return True
+
+    # next, check for forms that have both a user-like and password-like field
+    for form in forms:
+        user_fields = sum(bool(form.find_all("input", {"name": r})) for r in user_keywords)
+        pass_fields = sum(bool(form.find_all("input", {"name": r})) for r in pass_keywords)
+        if user_fields and pass_fields:
+            return True
+    return False
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1793rc0/bbot/core/helpers/wordcloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -245,22 +245,20 @@
             self[mutation] = 1
 
     def add_word(self, word):
         pass
 
 
 class DNSMutator(Mutator):
-    word_regex = re.compile(r"[^_\W]+")
     extract_word_regexes = [
         re.compile(r, re.I)
         for r in [
             r"[a-z]+",
+            r"[a-z_-]+",
             r"[a-z0-9]+",
-            r"[a-z0-9-]+",
-            r"[a-z0-9_]+",
             r"[a-z0-9_-]+",
         ]
     ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         wordlist_dir = Path(__file__).parent.parent.parent / "wordlists"
@@ -273,26 +271,34 @@
         new_words = set()
         for word in words:
             for e in extract_words(word, acronyms=False, model=self.model, word_regexes=self.extract_word_regexes):
                 new_words.add(e)
         return super().mutations(new_words, max_mutations=max_mutations)
 
     def add_word(self, word):
-        for match in self.word_regex.finditer(word):
-            start, end = match.span()
+        spans = set()
+        mutations = set()
+        for r in self.extract_word_regexes:
+            for match in r.finditer(word):
+                span = match.span()
+                if span not in spans:
+                    spans.add(span)
+        for start, end in spans:
             match_str = word[start:end]
             # skip digits
             if match_str.isdigit():
                 continue
             before = word[:start]
             after = word[end:]
-            basic_mutation = [before, None, after]
-            self._add_mutation(basic_mutation)
+            basic_mutation = (before, None, after)
+            mutations.add(basic_mutation)
             match_str_split = self.model.split(match_str)
             if len(match_str_split) > 1:
                 for i, s in enumerate(match_str_split):
                     if s.isdigit():
                         continue
                     split_before = "".join(match_str_split[:i])
                     split_after = "".join(match_str_split[i + 1 :])
-                    wordninja_mutation = [before + split_before, None, split_after + after]
-                    self._add_mutation(wordninja_mutation)
+                    wordninja_mutation = (before + split_before, None, split_after + after)
+                    mutations.add(wordninja_mutation)
+        for m in mutations:
+            self._add_mutation(m)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1793rc0/bbot/core/logger/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,43 @@
 from ..helpers.misc import mkdir, error_and_exit
 from ..helpers.logger import colorize, loglevel_mapping
 
 
 _log_level_override = None
 
 
+# Log to stderr
+stderr_handler = logging.StreamHandler(sys.stderr)
+
+# Log to stdout
+stdout_handler = logging.StreamHandler(sys.stdout)
+
+log_listener = None
+
+
 class ColoredFormatter(logging.Formatter):
     """
     Pretty colors for terminal
     """
 
+    formatter = logging.Formatter("%(levelname)s %(message)s")
+    module_formatter = logging.Formatter("%(levelname)s %(name)s: %(message)s")
+
     def format(self, record):
         colored_record = copy(record)
         levelname = colored_record.levelname
         levelshort = loglevel_mapping.get(levelname, "INFO")
         colored_record.levelname = colorize(f"[{levelshort}]", level=levelname)
         if levelname == "CRITICAL" or levelname.startswith("HUGE"):
             colored_record.msg = colorize(colored_record.msg, level=levelname)
-        return logging.Formatter.format(self, colored_record)
+        # remove name
+        if colored_record.name.startswith("bbot.modules."):
+            colored_record.name = colored_record.name.split("bbot.modules.")[-1]
+            return self.module_formatter.format(colored_record)
+        return self.formatter.format(colored_record)
 
 
 def addLoggingLevel(levelName, levelNum, methodName=None):
     """
     Comprehensively adds a new logging level to the `logging` module and the
     currently configured logging class.
 
@@ -116,20 +132,14 @@
 
 
 def log_listener_setup(logging_queue):
     log_dir = Path(config["home"]) / "logs"
     if not mkdir(log_dir, raise_error=False):
         error_and_exit(f"Failure creating or error writing to BBOT logs directory ({log_dir})")
 
-    # Log to stderr
-    stderr_handler = logging.StreamHandler(sys.stderr)
-
-    # Log to stdout
-    stdout_handler = logging.StreamHandler(sys.stdout)
-
     # Main log file
     main_handler = logging.handlers.TimedRotatingFileHandler(
         f"{log_dir}/bbot.log", when="d", interval=1, backupCount=14
     )
 
     # Separate log file for debugging
     debug_handler = logging.handlers.TimedRotatingFileHandler(
@@ -162,14 +172,15 @@
     debug_handler.setFormatter(debug_format)
     main_handler.setFormatter(debug_format)
     stderr_handler.setFormatter(ColoredFormatter("%(levelname)s %(name)s: %(message)s"))
     stdout_handler.setFormatter(logging.Formatter("%(message)s"))
 
     handlers = [stdout_handler, stderr_handler, main_handler, debug_handler]
 
+    global log_listener
     log_listener = QueueListener(logging_queue, *handlers)
     log_listener.start()
     atexit.register(stop_listener, log_listener)
     return {
         "stderr": stderr_handler,
         "stdout": stdout_handler,
         "file_debug": debug_handler,
@@ -217,14 +228,15 @@
     global _log_level_override
     if logger is not None:
         logger.hugeinfo(f"Setting log level to {logging.getLevelName(level)}")
     config["silent"] = False
     _log_level_override = level
     log = logging.getLogger("bbot")
     log.setLevel(level)
+    logging.getLogger("asyncio").setLevel(level)
 
 
 def toggle_log_level(logger=None):
     log_level = get_log_level()
     if log_level in verbosity_levels_toggle:
         for i, level in enumerate(verbosity_levels_toggle):
             if log_level == level:
```

### Comparing `bbot-1.0.5.1665rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1793rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/defaults.yml` & `bbot-1.0.5.1793rc0/bbot/defaults.yml`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 # 1 == 1 hope away from main scope
 # 0 == in scope only
 scope_report_distance: 0
 # Generate new DNS_NAME and IP_ADDRESS events through DNS resolution
 dns_resolution: true
 # Limit the number of BBOT threads
 max_threads: 25
-# Limit the number of DNS threads (this should be approximately 4x max_threads)
-max_dns_threads: 100
+# Rate-limit DNS
+dns_queries_per_second: 1000
+# Rate-limit HTTP
+web_requests_per_second: 100
+# Interval for displaying status messages
+status_frequency: 15
 # HTTP proxy
 http_proxy: 
 # Web user-agent
 user_agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.79 Safari/537.36
 
 
 ### ADVANCED OPTIONS ###
@@ -71,16 +75,14 @@
 dns_abort_threshold: 10
 # Don't show PTR records containing IP addresses
 dns_filter_ptrs: true
 # Enable/disable debug messages for dns queries
 dns_debug: false
 # Whether to verify SSL certificates
 ssl_verify: false
-# Interval for displaying status messages
-status_frequency: 15
 # How many scan results to keep before cleaning up the older ones
 keep_scans: 20
 # Completely ignore URLs with these extensions
 url_extension_blacklist:
     # images
     - png
     - jpg
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1793rc0/bbot/modules/anubisdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,33 +6,33 @@
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     meta = {"description": "Query jldc.me's database for subdomains"}
 
     base_url = "https://jldc.me/anubis/subdomains"
     dns_abort_depth = 5
 
-    def request_url(self, query):
+    async def request_url(self, query):
         url = f"{self.base_url}/{self.helpers.quote(query)}"
-        return self.request_with_fail_count(url)
+        return await self.request_with_fail_count(url)
 
     def abort_if_pre(self, hostname):
         """
         Discards results that are longer than 5 segments, e.g. a.b.c.d.evilcorp.com
         This exists because of the _disgusting_ amount of garbage data in this API
         """
         dns_depth = hostname.count(".") + 1
         if dns_depth > self.dns_abort_depth:
             return True
         return False
 
-    def abort_if(self, event):
+    async def abort_if(self, event):
         # abort if dns name is unresolved
         if not "resolved" in event.tags:
             return True, "DNS name is unresolved"
-        return super().abort_if(event)
+        return await super().abort_if(event)
 
     def parse_results(self, r, query):
         results = set()
         json = r.json()
         if json:
             for hostname in json:
                 hostname = str(hostname).lower()
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1793rc0/bbot/modules/azure_tenant.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "subdomain-enum", "passive", "safe"]
     meta = {"description": "Query Azure for tenant sister domains"}
 
     base_url = "https://autodiscover-s.outlook.com"
     in_scope_only = True
 
-    def setup(self):
+    async def setup(self):
         self.processed = set()
         self.d_xml_regex = re.compile(r"<Domain>([^<>/]*)</Domain>", re.I)
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         _, query = self.helpers.split_domain(event.data)
-        domains, _ = self.query(query)
+        domains, _ = await self.query(query)
         if domains:
             self.success(f'Found {len(domains):,} domains under tenant for "{query}"')
         for domain in domains:
             if domain != query:
                 self.emit_event(domain, "DNS_NAME", source=event, tags=["affiliate"])
         # todo: tenants?
 
-    def query(self, domain):
+    async def query(self, domain):
         url = f"{self.base_url}/autodiscover/autodiscover.svc"
         data = f"""<?xml version="1.0" encoding="utf-8"?>
 <soap:Envelope xmlns:exm="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:ext="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:a="http://www.w3.org/2005/08/addressing" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
     <soap:Header>
         <a:Action soap:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformation</a:Action>
         <a:To soap:mustUnderstand="1">https://autodiscover-s.outlook.com/autodiscover/autodiscover.svc</a:To>
         <a:ReplyTo>
@@ -52,15 +52,15 @@
             "SOAPAction": '"http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformation"',
             "User-Agent": "AutodiscoverClient",
             "Accept-Encoding": "identity",
         }
 
         self.debug(f"Retrieving tenant domains at {url}")
 
-        r = self.request_with_fail_count(url, method="POST", headers=headers, data=data)
+        r = await self.request_with_fail_count(url, method="POST", headers=headers, data=data)
         status_code = getattr(r, "status_code", 0)
         if status_code not in (200, 421):
             self.warning(f'Error retrieving azure_tenant domains for "{domain}" (status code: {status_code})')
             return set(), set()
         found_domains = list(set(self.d_xml_regex.findall(r.text)))
         domains = set()
         tenantnames = set()
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1793rc0/bbot/modules/badsecrets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+import multiprocessing
+
 from .base import BaseModule
 
 from badsecrets.base import carve_all_modules
 
 
 class badsecrets(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
     meta = {"description": "Library for detecting known or weak secrets across many web frameworks"}
     max_event_handlers = 2
-    deps_pip = ["badsecrets~=0.1.287"]
+    deps_pip = ["badsecrets~=0.3.351"]
+
+    @property
+    def _max_event_handlers(self):
+        return multiprocessing.cpu_count()
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         resp_body = event.data.get("body", None)
         resp_headers = event.data.get("header", None)
         resp_cookies = {}
         if resp_headers:
             resp_cookies_raw = resp_headers.get("set_cookie", None)
             if resp_cookies_raw:
                 if "," in resp_cookies_raw:
@@ -23,25 +29,27 @@
                 else:
                     resp_cookies_list = [resp_cookies_raw]
                 for c in resp_cookies_list:
                     c2 = c.lstrip(";").strip().split(";")[0].split("=")
                     if len(c2) == 2:
                         resp_cookies[c2[0]] = c2[1]
         if resp_body or resp_cookies:
-            r_list = carve_all_modules(body=resp_body, cookies=resp_cookies)
+            r_list = await self.scan.run_in_executor_mp(
+                carve_all_modules, body=resp_body, cookies=resp_cookies, url=event.data.get("url", None)
+            )
             if r_list:
                 for r in r_list:
                     if r["type"] == "SecretFound":
                         data = {
                             "severity": "HIGH",
-                            "description": f"Known Secret Found. Secret Type: [{r['description']['Secret']}] Secret: [{r['secret']}] Product Type: [{r['description']['Product']}] Product: [{r['source']}] Detecting Module: [{r['detecting_module']}]",
+                            "description": f"Known Secret Found. Secret Type: [{r['description']['secret']}] Secret: [{r['secret']}] Product Type: [{r['description']['product']}] Product: [{r['product']}] Detecting Module: [{r['detecting_module']}] Details: [{r['details']}]",
                             "url": event.data["url"],
                             "host": str(event.host),
                         }
                         self.emit_event(data, "VULNERABILITY", event)
                     elif r["type"] == "IdentifyOnly":
                         data = {
-                            "description": f"Cryptographic Product identified. Product Type: [{r['description']['Product']}] Product: [{r['source']}] Detecting Module: [{r['detecting_module']}]",
+                            "description": f"Cryptographic Product identified. Product Type: [{r['description']['product']}] Product: [{r['product']}] Detecting Module: [{r['detecting_module']}]",
                             "url": event.data["url"],
                             "host": str(event.host),
                         }
                         self.emit_event(data, "FINDING", event)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/base.py` & `bbot-1.0.5.1793rc0/bbot/modules/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import queue
+import asyncio
 import logging
-import threading
 import traceback
 from sys import exc_info
 from contextlib import suppress
 
 from ..core.helpers.misc import get_size
-from ..core.helpers.threadpool import ThreadPoolWrapper, TaskCounter
-from ..core.errors import ScanCancelledError, ValidationError, WordlistError
+from ..core.helpers.async_helpers import TaskCounter
+from ..core.errors import ValidationError, WordlistError
 
 
 class BaseModule:
     # Event types to watch
     watched_events = []
     # Event types to produce
     produced_events = []
@@ -63,126 +62,124 @@
     # Use in conjunction with .request_with_fail_count() to set_error_state() after this many failed HTTP requests
     failed_request_abort_threshold = 5
     # When set to false, prevents events generated by this module from being automatically marked as in-scope
     # Useful for low-confidence modules like speculate and ipneighbor
     _scope_shepherding = True
     # Exclude from scan statistics
     _stats_exclude = False
-    # outgoing queue size (None == infinite)
-    _qsize = None
+    # outgoing queue size (0 == infinite)
+    _qsize = 0
     # Priority of events raised by this module, 1-5, lower numbers == higher priority
     _priority = 3
     # Name, overridden automatically
     _name = "base"
     # Type, for differentiating between normal modules and output modules, etc.
     _type = "scan"
 
-    _report_lock = threading.Lock()
-
     def __init__(self, scan):
         self.scan = scan
         self.errored = False
         self._log = None
         self._incoming_event_queue = None
         # seconds since we've submitted a batch
+        self._outgoing_event_queue = None
+        # seconds since we've submitted a batch
         self._last_submitted_batch = None
-        # wrapper around shared thread pool to ensure that a single module doesn't hog more than its share
-        self.thread_pool = ThreadPoolWrapper(self.scan._thread_pool)
-        self._internal_thread_pool = ThreadPoolWrapper(
-            self.scan._internal_thread_pool.executor, max_workers=self.max_event_handlers
-        )
         # additional callbacks to be executed alongside self.cleanup()
         self.cleanup_callbacks = []
         self._cleanedup = False
         self._watched_events = None
 
-        self._lock = threading.RLock()
-        self._running_counter = TaskCounter()
-        self.event_received = threading.Condition(self._lock)
+        self._task_counter = TaskCounter()
 
         # string constant
         self._custom_filter_criteria_msg = "it did not meet custom filter criteria"
 
         # track number of failures (for .request_with_fail_count())
         self._request_failures = 0
 
-    def setup(self):
+        self._tasks = []
+        self._event_received = asyncio.Condition()
+        self._event_queued = asyncio.Condition()
+        self._event_dequeued = asyncio.Condition()
+
+    async def setup(self):
         """
         Perform setup functions at the beginning of the scan.
         Optionally override this method.
 
         Must return True or False based on whether the setup was successful
         """
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         """
         Override this method if batch_size == 1.
         """
         pass
 
     def handle_batch(self, *events):
         """
         Override this method if batch_size > 1.
         """
         pass
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         """
         Accept/reject events based on custom criteria
 
         Override this method if you need more granular control
         over which events are distributed to your module
         """
         return True
 
-    def finish(self):
+    async def finish(self):
         """
         Perform final functions when scan is nearing completion
 
         For example,  if your module relies on the word cloud, you may choose to wait until
         the scan is finished (and the word cloud is most complete) before running an operation.
 
         Note that this method may be called multiple times, because it may raise events.
         Optionally override this method.
         """
         return
 
-    def report(self):
+    async def report(self):
         """
         Perform a final task when the scan is finished, but before cleanup happens
 
         This is useful for modules that aggregate data and raise summary events at the end of a scan
         """
         return
 
-    def cleanup(self):
+    async def cleanup(self):
         """
         Perform final cleanup after the scan has finished
         This method is called only once, and may not raise events.
         Optionally override this method.
         """
         return
 
-    def require_api_key(self):
+    async def require_api_key(self):
         """
         Use in setup() to ensure the module is configured with an API key
         """
         self.api_key = self.config.get("api_key", "")
         if self.auth_secret:
             try:
-                self.ping()
+                await self.ping()
                 self.hugesuccess(f"API is ready")
                 return True
             except Exception as e:
                 return None, f"Error with API ({str(e).strip()})"
         else:
             return None, "No API key set"
 
-    def ping(self):
+    async def ping(self):
         """
         Used in conjuction with require_api_key to ensure an API is up and responding
 
         Requires the use of an assert statement.
 
         E.g. if your API has a "/ping" endpoint, you can use it like this:
             def ping(self):
@@ -203,64 +200,34 @@
         """
         Override if you need your watched_events to be dynamic
         """
         if self._watched_events is None:
             self._watched_events = set(self.watched_events)
         return self._watched_events
 
-    def submit_task(self, *args, **kwargs):
-        kwargs["_block"] = False
-        return self.thread_pool.submit_task(self.catch, *args, **kwargs)
-
-    def catch(self, *args, **kwargs):
-        return self.scan.manager.catch(*args, **kwargs)
-
-    def _postcheck_and_run(self, callback, event):
-        acceptable, reason = self._event_postcheck(event)
-        if not acceptable:
-            if reason:
-                self.debug(f"Not accepting {event} because {reason}")
-            return
-        self.scan.stats.event_consumed(event, self)
-        return callback(event)
-
-    def _register_running(self, callback, *args, **kwargs):
-        with self._running_counter:
-            return callback(*args, **kwargs)
-
-    def _handle_batch(self, force=False):
+    async def _handle_batch(self):
+        submitted = False
         if self.batch_size <= 1:
             return
-        if self.num_queued_events > 0 and (force or self.num_queued_events >= self.batch_size):
-            on_finish_callback = None
-            events, finish, report = self.events_waiting
-            if finish:
-                on_finish_callback = self.finish
-            elif report:
-                on_finish_callback = self.report
-            checked_events = []
-            for e in events:
-                acceptable, reason = self._event_postcheck(e)
-                if not acceptable:
-                    if reason:
-                        self.debug(f"Not accepting {e} because {reason}")
-                    continue
-                checked_events.append(e)
-            if checked_events:
+        if self.num_incoming_events > 0:
+            events, finish, report = await self.events_waiting()
+            if not self.errored:
                 self.debug(f"Handling batch of {len(events):,} events")
-                if not self.errored:
-                    self._internal_thread_pool.submit_task(
-                        self.catch,
-                        self._register_running,
-                        self.handle_batch,
-                        *checked_events,
-                        _on_finish_callback=on_finish_callback,
-                    )
-                return True
-        return False
+                if events:
+                    submitted = True
+                    async with self.scan.acatch(context=f"{self.name}.handle_batch"):
+                        with self._task_counter:
+                            await self.handle_batch(*events)
+                if finish:
+                    async with self.scan.acatch(context=f"{self.name}.finish"):
+                        await self.finish()
+                elif report:
+                    async with self.scan.acatch(context=f"{self.name}.report"):
+                        await self.report()
+        return submitted
 
     def make_event(self, *args, **kwargs):
         raise_error = kwargs.pop("raise_error", False)
         try:
             event = self.scan.make_event(*args, **kwargs)
         except ValidationError as e:
             if raise_error:
@@ -269,156 +236,137 @@
             return
         if not event.module:
             event.module = self
         return event
 
     def emit_event(self, *args, **kwargs):
         event_kwargs = dict(kwargs)
+        emit_kwargs = {}
         for o in ("on_success_callback", "abort_if", "quick"):
-            event_kwargs.pop(o, None)
+            v = event_kwargs.pop(o, None)
+            if v is not None:
+                emit_kwargs[o] = v
         event = self.make_event(*args, **event_kwargs)
-        if event is None:
-            return
-        # nerf event's priority if it's likely not to be in scope
-        if event.scope_distance > 0:
-            event_in_scope = self.scan.whitelisted(event) and not self.scan.blacklisted(event)
-            if not event_in_scope:
-                event.module_priority += event.scope_distance
         if event:
-            # Wait for parent event to resolve (in case its scope distance changes)
-            while 1:
-                if self.scan.stopping:
-                    return
-                resolved = event.source._resolved.wait(timeout=0.1)
-                if resolved:
-                    # update event's scope distance based on its parent
-                    event.scope_distance = event.source.scope_distance + 1
-                    break
-            self.scan.manager.incoming_event_queue.put((event, kwargs))
+            self.queue_outgoing_event(event, **emit_kwargs)
 
-    @property
-    def events_waiting(self):
+    async def events_waiting(self):
         """
         yields all events in queue, up to maximum batch size
         """
         events = []
         finish = False
         report = False
         while self.incoming_event_queue:
             if len(events) > self.batch_size:
                 break
             try:
                 event = self.incoming_event_queue.get_nowait()
-                if event.type == "FINISHED":
-                    finish = True
-                else:
-                    events.append(event)
-            except queue.Empty:
+                self.debug(f"Got {event} from {getattr(event, 'module', 'unknown_module')}")
+                acceptable, reason = await self._event_postcheck(event)
+                if acceptable:
+                    if event.type == "FINISHED":
+                        finish = True
+                    else:
+                        events.append(event)
+                        self.scan.stats.event_consumed(event, self)
+                elif reason:
+                    self.debug(f"Not accepting {event} because {reason}")
+            except asyncio.queues.QueueEmpty:
                 break
         return events, finish, report
 
     @property
-    def num_queued_events(self):
+    def num_incoming_events(self):
         ret = 0
         if self.incoming_event_queue:
             ret = self.incoming_event_queue.qsize()
         return ret
 
+    @property
+    def _max_event_handlers(self):
+        return self.max_event_handlers
+
     def start(self):
-        self.thread = threading.Thread(target=self._worker, daemon=True)
-        self.thread.start()
+        self._tasks = [asyncio.create_task(self._worker()) for _ in range(self._max_event_handlers)]
 
-    def _setup(self):
+    async def _setup(self):
         status_codes = {False: "hard-fail", None: "soft-fail", True: "success"}
 
         status = False
         self.debug(f"Setting up module {self.name}")
         try:
-            result = self.setup()
+            result = await self.setup()
             if type(result) == tuple and len(result) == 2:
                 status, msg = result
             else:
                 status = result
                 msg = status_codes[status]
             self.debug(f"Finished setting up module {self.name}")
         except Exception as e:
             self.set_error_state()
+            # soft-fail if it's only a wordlist error
             if isinstance(e, WordlistError):
                 status = None
             msg = f"{e}"
             self.trace()
-        return status, str(msg)
+        return self.name, status, str(msg)
 
-    @property
-    def _force_batch(self):
-        """
-        Determine whether a batch should be forcefully submitted
-        """
-        # if we're below our maximum threading potential
-        return self._internal_thread_pool.num_tasks < self.max_event_handlers
-
-    def _worker(self):
-        try:
+    async def _worker(self):
+        async with self.scan.acatch(context=self._worker):
             while not self.scan.stopping:
                 # hold the reigns if our outgoing queue is full
-                if self._qsize and self.outgoing_event_queue_qsize >= self._qsize:
-                    with self.event_received:
-                        self.event_received.wait(timeout=0.1)
+                if self._qsize > 0 and self.outgoing_event_queue.qsize() >= self._qsize:
+                    await asyncio.sleep(0.1)
                     continue
 
                 if self.batch_size > 1:
-                    submitted = self._handle_batch(force=self._force_batch)
+                    submitted = await self._handle_batch()
                     if not submitted:
-                        with self.event_received:
-                            self.event_received.wait(timeout=0.1)
+                        async with self._event_received:
+                            await self._event_received.wait()
 
                 else:
                     try:
                         if self.incoming_event_queue:
-                            e = self.incoming_event_queue.get(timeout=0.1)
+                            event = await self.incoming_event_queue.get()
                         else:
                             self.debug(f"Event queue is in bad state")
                             return
-                    except queue.Empty:
+                    except asyncio.queues.QueueEmpty:
                         continue
-                    self.debug(f"Got {e} from {getattr(e, 'module', e)}")
-                    # if we receive the special "FINISHED" event
-                    if e.type == "FINISHED":
-                        self._internal_thread_pool.submit_task(self.catch, self._register_running, self.finish)
-                    else:
-                        if self._type == "output":
-                            self.catch(self._register_running, self._postcheck_and_run, self.handle_event, e)
+                    self.debug(f"Got {event} from {getattr(event, 'module', 'unknown_module')}")
+                    acceptable, reason = await self._event_postcheck(event)
+                    if not acceptable:
+                        self.debug(f"Not accepting {event} because {reason}")
+                    if acceptable:
+                        if event.type == "FINISHED":
+                            async with self.scan.acatch(context=f"{self.name}.finish"):
+                                with self._task_counter:
+                                    await self.finish()
                         else:
-                            self._internal_thread_pool.submit_task(
-                                self.catch, self._register_running, self._postcheck_and_run, self.handle_event, e
-                            )
-
-        except KeyboardInterrupt:
-            self.debug(f"Interrupted")
-            self.scan.stop()
-        except ScanCancelledError as e:
-            self.verbose(f"Scan cancelled, {e}")
-        except Exception as e:
-            self.set_error_state(f"Exception ({e.__class__.__name__}) in module {self.name}:\n{e}")
-            self.trace()
+                            self.scan.stats.event_consumed(event, self)
+                            async with self.scan.acatch(context=f"{self.name}.handle_event"):
+                                with self._task_counter:
+                                    await self.handle_event(event)
 
     @property
     def max_scope_distance(self):
         if self.in_scope_only or self.target_only:
             return 0
         return max(0, self.scan.scope_search_distance + self.scope_distance_modifier)
 
     def _event_precheck(self, event):
         """
         Check if an event should be accepted by the module
         Used when putting an event INTO the modules' queue
         """
         # special signal event types
         if event.type in ("FINISHED",):
-            return True, ""
+            return True, "its type is FINISHED"
         if self.errored:
             return False, f"module is in error state"
         # exclude non-watched types
         if not any(t in self.get_watched_events() for t in ("*", event.type)):
             return False, "its type is not in watched_events"
         if self.target_only:
             if "target" not in event.tags:
@@ -435,94 +383,122 @@
             and self.name != "speculate"
         ):
             # and the current module listens for both ranges and CIDRs
             if all([x in self.watched_events for x in ("IP_RANGE", "IP_ADDRESS")]):
                 # then skip the event.
                 # this helps avoid double-portscanning both an individual IP and its parent CIDR.
                 return False, "module consumes IP ranges directly"
-        return True, ""
+        return True, "precheck succeeded"
 
-    def _event_postcheck(self, event):
+    async def _event_postcheck(self, event):
         """
         Check if an event should be accepted by the module
         Used when taking an event FROM the module's queue (immediately before it's handled)
         """
+        # special exception for "FINISHED" event
         if event.type in ("FINISHED",):
             return True, ""
 
+        # reject out-of-scope events for active modules
+        # TODO: reconsider this
         if "active" in self.flags and "target" in event.tags and event not in self.scan.whitelist:
             return False, "it is not in whitelist and module has active flag"
 
+        # check scope distance
         if self._type != "output":
             if self.in_scope_only:
                 if event.scope_distance > 0:
                     return False, "it did not meet in_scope_only filter criteria"
             if self.scope_distance_modifier is not None:
                 if event.scope_distance < 0:
                     return False, f"its scope_distance ({event.scope_distance}) is invalid."
                 elif event.scope_distance > self.max_scope_distance:
                     return (
                         False,
                         f"its scope_distance ({event.scope_distance}) exceeds the maximum allowed by the scan ({self.scan.scope_search_distance}) + the module ({self.scope_distance_modifier}) == {self.max_scope_distance}",
                     )
 
         # custom filtering
-        try:
-            filter_result = self.filter_event(event)
+        async with self.scan.acatch(context=self.filter_event):
+            filter_result = await self.filter_event(event)
             msg = str(self._custom_filter_criteria_msg)
             with suppress(ValueError, TypeError):
                 filter_result, reason = filter_result
                 msg += f": {reason}"
             if not filter_result:
                 return False, msg
-        except ScanCancelledError:
-            return False, "Scan cancelled"
-        except Exception as e:
-            self.error(f"Error in filter_event({event}): {e}")
-            self.trace()
 
         if self._type == "output" and not event._stats_recorded:
             event._stats_recorded = True
             self.scan.stats.event_produced(event)
 
+        self.debug(f"{event} passed post-check")
         return True, ""
 
-    def _cleanup(self):
+    async def _cleanup(self):
         if not self._cleanedup:
             self._cleanedup = True
             for callback in [self.cleanup] + self.cleanup_callbacks:
                 if callable(callback):
-                    self.catch(self._register_running, callback, _force=True)
+                    async with self.scan.acatch(context=self.name):
+                        with self._task_counter:
+                            await self.helpers.execute_sync_or_async(callback)
 
-    def queue_event(self, event):
+    async def queue_event(self, event):
+        """
+        Queue (incoming) event with module
+        """
         if self.incoming_event_queue in (None, False):
-            self.debug(f"Not in an acceptable state to queue event")
+            self.debug(f"Not in an acceptable state to queue incoming event")
             return
         acceptable, reason = self._event_precheck(event)
         if not acceptable:
             if reason and reason != "its type is not in watched_events":
                 self.debug(f"Not accepting {event} because {reason}")
             return
+        else:
+            self.debug(f"Accepting {event} because {reason}")
         try:
-            self.incoming_event_queue.put(event)
+            self.incoming_event_queue.put_nowait(event)
+            async with self._event_received:
+                self._event_received.notify()
+            if event.type != "FINISHED":
+                self.scan.manager._new_activity = True
         except AttributeError:
-            self.debug(f"Not in an acceptable state to queue event")
-        with self.event_received:
-            self.event_received.notify()
+            self.debug(f"Not in an acceptable state to queue incoming event")
+
+    def queue_outgoing_event(self, event, **kwargs):
+        """
+        Queue (outgoing) event with module
+        """
+        try:
+            self.outgoing_event_queue.put_nowait((event, kwargs))
+        except AttributeError:
+            self.debug(f"Not in an acceptable state to queue outgoing event")
+
+    async def dequeue_outgoing_event(self):
+        await self.outgoing_event_queue.get()
+        with self._event_dequeued:
+            self._event_dequeued.notify()
+
+    def dequeue_outgoing_event_nowait(self):
+        return self.outgoing_event_queue.get_nowait()
+        with self._event_dequeued:
+            self._event_dequeued.notify()
 
     def set_error_state(self, message=None):
         if not self.errored:
             if message is not None:
                 self.warning(str(message))
             self.debug(f"Setting error state for module {self.name}")
             self.errored = True
             # clear incoming queue
             if self.incoming_event_queue:
                 self.debug(f"Emptying event_queue")
-                with suppress(queue.Empty):
+                with suppress(asyncio.queues.QueueEmpty):
                     while 1:
                         self.incoming_event_queue.get_nowait()
                 # set queue to None to prevent its use
                 # if there are leftover objects in the queue, the scan will hang.
                 self._incoming_event_queue = False
 
     @property
@@ -531,45 +507,38 @@
 
     @property
     def helpers(self):
         return self.scan.helpers
 
     @property
     def status(self):
-        main_pool = self.thread_pool.num_tasks
-        internal_pool = self._internal_thread_pool.num_tasks
-        pool_total = main_pool + internal_pool
-        incoming_qsize = 0
-        if self.incoming_event_queue:
-            incoming_qsize = self.incoming_event_queue.qsize()
         status = {
-            "events": {"incoming": incoming_qsize, "outgoing": self.outgoing_event_queue_qsize},
-            "tasks": {"main_pool": main_pool, "internal_pool": internal_pool, "total": pool_total},
+            "events": {"incoming": self.num_incoming_events, "outgoing": self.outgoing_event_queue.qsize()},
+            "tasks": self._task_counter.value,
             "errored": self.errored,
         }
         status["running"] = self.running
-        status["active"] = self._is_active(status)
         return status
 
-    @staticmethod
-    def _is_active(status):
-        if status["running"]:
-            return True
-        total = status["tasks"]["total"] + status["events"]["incoming"] + status["events"]["outgoing"]
-        return total > 0
-
     @property
     def running(self):
         """
         Indicates whether the module is currently processing data.
         """
-        return self._running_counter.value > 0
+        return self._task_counter.value > 0
 
-    def request_with_fail_count(self, *args, **kwargs):
-        r = self.helpers.request(*args, **kwargs)
+    @property
+    def finished(self):
+        """
+        Indicates whether the module is finished (not running and nothing in queues)
+        """
+        return not self.running and self.num_incoming_events <= 0 and self.outgoing_event_queue.qsize() <= 0
+
+    async def request_with_fail_count(self, *args, **kwargs):
+        r = await self.helpers.request(*args, **kwargs)
         if r is None:
             self._request_failures += 1
         else:
             self._request_failures = 0
         if self._request_failures >= self.failed_request_abort_threshold:
             self.set_error_state(f"Setting error state due to {self._request_failures:,} failed HTTP requests")
         return r
@@ -589,20 +558,22 @@
         if config is None:
             config = {}
         return config
 
     @property
     def incoming_event_queue(self):
         if self._incoming_event_queue is None:
-            self._incoming_event_queue = queue.PriorityQueue()
+            self._incoming_event_queue = asyncio.PriorityQueue()
         return self._incoming_event_queue
 
     @property
-    def outgoing_event_queue_qsize(self):
-        return self.scan.manager.incoming_event_queue.modules.get(str(self), 0)
+    def outgoing_event_queue(self):
+        if self._outgoing_event_queue is None:
+            self._outgoing_event_queue = asyncio.PriorityQueue()
+        return self._outgoing_event_queue
 
     @property
     def priority(self):
         return int(max(1, min(5, self._priority)))
 
     @property
     def auth_required(self):
@@ -615,72 +586,88 @@
         return self._log
 
     @property
     def memory_usage(self):
         """
         Return how much memory the module is currently using in bytes
         """
-        seen = set(self.scan.pools.values())
-        seen.update({self.scan, self.helpers, self.log})
+        seen = {self.scan, self.helpers, self.log}
         return get_size(self, max_depth=3, seen=seen)
 
     def __str__(self):
         return self.name
 
     def log_table(self, *args, **kwargs):
-        with self._report_lock:
-            table_name = kwargs.pop("table_name", None)
-            table = self.helpers.make_table(*args, **kwargs)
-            for line in table.splitlines():
-                self.info(line)
-            if table_name is not None:
-                date = self.helpers.make_date()
-                filename = self.scan.home / f"{self.helpers.tagify(table_name)}-table-{date}.txt"
-                with open(filename, "w") as f:
-                    f.write(table)
-                self.verbose(f"Wrote {table_name} to {filename}")
-            return table
+        table_name = kwargs.pop("table_name", None)
+        table = self.helpers.make_table(*args, **kwargs)
+        for line in table.splitlines():
+            self.info(line)
+        if table_name is not None:
+            date = self.helpers.make_date()
+            filename = self.scan.home / f"{self.helpers.tagify(table_name)}-table-{date}.txt"
+            with open(filename, "w") as f:
+                f.write(table)
+            self.verbose(f"Wrote {table_name} to {filename}")
+        return table
 
     def stdout(self, *args, **kwargs):
         self.log.stdout(*args, extra={"scan_id": self.scan.id}, **kwargs)
 
-    def debug(self, *args, **kwargs):
+    def debug(self, *args, trace=False, **kwargs):
         self.log.debug(*args, extra={"scan_id": self.scan.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def verbose(self, *args, **kwargs):
+    def verbose(self, *args, trace=False, **kwargs):
         self.log.verbose(*args, extra={"scan_id": self.scan.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def hugeverbose(self, *args, **kwargs):
+    def hugeverbose(self, *args, trace=False, **kwargs):
         self.log.hugeverbose(*args, extra={"scan_id": self.scan.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def info(self, *args, **kwargs):
+    def info(self, *args, trace=False, **kwargs):
         self.log.info(*args, extra={"scan_id": self.scan.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def hugeinfo(self, *args, **kwargs):
+    def hugeinfo(self, *args, trace=False, **kwargs):
         self.log.hugeinfo(*args, extra={"scan_id": self.scan.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def success(self, *args, **kwargs):
+    def success(self, *args, trace=False, **kwargs):
         self.log.success(*args, extra={"scan_id": self.scan.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def hugesuccess(self, *args, **kwargs):
+    def hugesuccess(self, *args, trace=False, **kwargs):
         self.log.hugesuccess(*args, extra={"scan_id": self.scan.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def warning(self, *args, **kwargs):
+    def warning(self, *args, trace=True, **kwargs):
         self.log.warning(*args, extra={"scan_id": self.scan.id}, **kwargs)
-        self.trace()
+        if trace:
+            self.trace()
 
-    def hugewarning(self, *args, **kwargs):
+    def hugewarning(self, *args, trace=True, **kwargs):
         self.log.hugewarning(*args, extra={"scan_id": self.scan.id}, **kwargs)
-        self.trace()
+        if trace:
+            self.trace()
 
-    def error(self, *args, **kwargs):
+    def error(self, *args, trace=True, **kwargs):
         self.log.error(*args, extra={"scan_id": self.scan.id}, **kwargs)
-        self.trace()
+        if trace:
+            self.trace()
 
     def trace(self):
         e_type, e_val, e_traceback = exc_info()
         if e_type is not None:
             self.log.trace(traceback.format_exc())
 
-    def critical(self, *args, **kwargs):
+    def critical(self, *args, trace=True, **kwargs):
         self.log.critical(*args, extra={"scan_id": self.scan.id}, **kwargs)
-        self.trace()
+        if trace:
+            self.trace()
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1793rc0/bbot/modules/bevigil.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,43 +11,43 @@
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Retrieve OSINT data from mobile applications using BeVigil", "auth_required": True}
     options = {"api_key": "", "urls": False}
     options_desc = {"api_key": "BeVigil OSINT API Key", "urls": "Emit URLs in addition to DNS_NAMEs"}
 
     base_url = "https://osint.bevigil.com/api"
 
-    def setup(self):
+    async def setup(self):
         self.api_key = self.config.get("api_key", "")
         self.headers = {"X-Access-Token": self.api_key}
         self.urls = self.config.get("urls", False)
-        return super().setup()
+        return await super().setup()
 
-    def ping(self):
+    async def ping(self):
         pass
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        subdomains = self.query(query, request_fn=self.request_subdomains, parse_fn=self.parse_subdomains)
+        subdomains = await self.query(query, request_fn=self.request_subdomains, parse_fn=self.parse_subdomains)
         if subdomains:
             for subdomain in subdomains:
                 self.emit_event(subdomain, "DNS_NAME", source=event)
 
         if self.urls:
-            urls = self.query(query, request_fn=self.request_urls, parse_fn=self.parse_urls)
+            urls = await self.query(query, request_fn=self.request_urls, parse_fn=self.parse_urls)
             if urls:
                 for parsed_url in self.helpers.collapse_urls(urls):
                     self.emit_event(parsed_url.geturl(), "URL_UNVERIFIED", source=event)
 
-    def request_subdomains(self, query):
+    async def request_subdomains(self, query):
         url = f"{self.base_url}/{self.helpers.quote(query)}/subdomains/"
-        return self.request_with_fail_count(url, headers=self.headers)
+        return await self.request_with_fail_count(url, headers=self.headers)
 
-    def request_urls(self, query):
+    async def request_urls(self, query):
         url = f"{self.base_url}/{self.helpers.quote(query)}/urls/"
-        return self.request_with_fail_count(url, headers=self.headers)
+        return await self.request_with_fail_count(url, headers=self.headers)
 
     def parse_subdomains(self, r, query=None):
         results = set()
         subdomains = r.json().get("subdomains")
         if subdomains:
             results.update(subdomains)
         return results
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1793rc0/bbot/modules/binaryedge.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,25 +10,25 @@
     options_desc = {
         "api_key": "BinaryEdge API key",
         "max_records": "Limit results to help prevent exceeding API quota",
     }
 
     base_url = "https://api.binaryedge.io/v2"
 
-    def setup(self):
+    async def setup(self):
         self.max_records = self.config.get("max_records", 1000)
         self.headers = {"X-Key": self.config.get("api_key", "")}
-        return super().setup()
+        return await super().setup()
 
-    def ping(self):
+    async def ping(self):
         url = f"{self.base_url}/user/subscription"
-        j = self.request_with_fail_count(url, headers=self.headers).json()
+        j = (await self.request_with_fail_count(url, headers=self.headers)).json()
         assert j.get("requests_left", 0) > 0
 
-    def request_url(self, query):
+    async def request_url(self, query):
         # todo: host query (certs + services)
         url = f"{self.base_url}/query/domains/subdomain/{self.helpers.quote(query)}"
-        return self.request_with_fail_count(url, headers=self.headers)
+        return await self.request_with_fail_count(url, headers=self.headers)
 
     def parse_results(self, r, query):
         j = r.json()
         return j.get("events", [])
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1793rc0/bbot/modules/bucket_aws.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,113 +2,110 @@
 
 
 class bucket_aws(BaseModule):
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "cloud-enum", "web-basic", "web-thorough"]
     meta = {"description": "Check for S3 buckets related to target"}
-    options = {"max_threads": 10, "permutations": False}
+    options = {"permutations": False}
     options_desc = {
-        "max_threads": "Maximum number of threads for HTTP requests",
         "permutations": "Whether to try permutations",
     }
     scope_distance_modifier = 3
 
     cloud_helper_name = "aws"
     delimiters = ("", ".", "-")
     base_domains = ["s3.amazonaws.com"]
     regions = [None]
     supports_open_check = True
 
-    def setup(self):
+    async def setup(self):
         self.buckets_tried = set()
         self.cloud_helper = getattr(self.helpers.cloud, self.cloud_helper_name)
         self.permutations = self.config.get("permutations", False)
         return True
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if event.type == "DNS_NAME" and event.scope_distance > 0:
             return False, "only accepts in-scope DNS_NAMEs"
         if event.type == "STORAGE_BUCKET":
             if f"cloud-{self.cloud_helper_name}" not in event.tags:
                 return False, "bucket belongs to a different cloud provider"
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         if event.type == "DNS_NAME":
-            self.handle_dns_name(event)
+            await self.handle_dns_name(event)
         elif event.type == "STORAGE_BUCKET":
-            self.handle_storage_bucket(event)
+            await self.handle_storage_bucket(event)
 
-    def handle_dns_name(self, event):
+    async def handle_dns_name(self, event):
         buckets = set()
         base = event.data
         stem = self.helpers.domain_stem(base)
         for b in [base, stem]:
             split = b.split(".")
             for d in self.delimiters:
                 buckets.add(d.join(split))
-        for bucket_name, url, tags in self.brute_buckets(buckets, permutations=self.permutations):
+        async for bucket_name, url, tags in self.brute_buckets(buckets, permutations=self.permutations):
             self.emit_event({"name": bucket_name, "url": url}, "STORAGE_BUCKET", source=event, tags=tags)
 
-    def handle_storage_bucket(self, event):
+    async def handle_storage_bucket(self, event):
         url = event.data["url"]
         bucket_name = event.data["name"]
         if self.supports_open_check:
-            description, tags = self._check_bucket_open(bucket_name, url)
+            description, tags = await self._check_bucket_open(bucket_name, url)
             if description:
                 event_data = {"host": event.host, "url": url, "description": description}
                 self.emit_event(event_data, "FINDING", source=event, tags=tags)
 
-        for bucket_name, url, tags in self.brute_buckets(
+        async for bucket_name, url, tags in self.brute_buckets(
             [bucket_name], permutations=self.permutations, omit_base=True
         ):
             self.emit_event({"name": bucket_name, "url": url}, "STORAGE_BUCKET", source=event, tags=tags)
 
-    def brute_buckets(self, buckets, permutations=False, omit_base=False):
+    async def brute_buckets(self, buckets, permutations=False, omit_base=False):
         buckets = set(buckets)
         new_buckets = set(buckets)
         if permutations:
             for b in buckets:
                 for mutation in self.helpers.word_cloud.mutations(b, cloud=False):
                     for d in self.delimiters:
                         new_buckets.add(d.join(mutation))
         if omit_base:
             new_buckets = new_buckets - buckets
         new_buckets = [b for b in new_buckets if self.valid_bucket_name(b)]
-        futures = {}
+        tasks = []
         for base_domain in self.base_domains:
             for region in self.regions:
                 for bucket_name in new_buckets:
                     url = self.build_url(bucket_name, base_domain, region)
-                    future = self.submit_task(self._check_bucket_exists, bucket_name, url)
-                    futures[future] = (bucket_name, url)
-        for future in self.helpers.as_completed(futures):
-            bucket_name, url = futures[future]
-            existent_bucket, tags = future.result()
+                    tasks.append(self.helpers.create_task(self._check_bucket_exists(bucket_name, url)))
+        for task in self.helpers.as_completed(tasks):
+            existent_bucket, tags, bucket_name, url = await task
             if existent_bucket:
                 yield bucket_name, url, tags
 
-    def _check_bucket_exists(self, bucket_name, url):
+    async def _check_bucket_exists(self, bucket_name, url):
         self.debug(f'Checking if bucket exists: "{bucket_name}"')
-        return self.check_bucket_exists(bucket_name, url)
+        return await self.check_bucket_exists(bucket_name, url)
 
-    def check_bucket_exists(self, bucket_name, url):
-        response = self.helpers.request(url)
+    async def check_bucket_exists(self, bucket_name, url):
+        response = await self.helpers.request(url)
         tags = self.gen_tags_exists(response)
         status_code = getattr(response, "status_code", 404)
         existent_bucket = status_code != 404
-        return (existent_bucket, tags)
+        return (existent_bucket, tags, bucket_name, url)
 
-    def _check_bucket_open(self, bucket_name, url):
+    async def _check_bucket_open(self, bucket_name, url):
         self.debug(f'Checking if bucket is misconfigured: "{bucket_name}"')
-        return self.check_bucket_open(bucket_name, url)
+        return await self.check_bucket_open(bucket_name, url)
 
-    def check_bucket_open(self, bucket_name, url):
-        response = self.helpers.request(url)
+    async def check_bucket_open(self, bucket_name, url):
+        response = await self.helpers.request(url)
         tags = self.gen_tags_exists(response)
         status_code = getattr(response, "status_code", 404)
         content = getattr(response, "text", "")
         open_bucket = status_code == 200 and "Contents" in content
         msg = ""
         if open_bucket:
             msg = "Open storage bucket"
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1793rc0/bbot/modules/bucket_azure.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 
 class bucket_azure(bucket_aws):
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "cloud-enum", "web-basic", "web-thorough"]
     meta = {"description": "Check for Azure storage blobs related to target"}
-    options = {"max_threads": 10, "permutations": False}
+    options = {"permutations": False}
     options_desc = {
-        "max_threads": "Maximum number of threads for HTTP requests",
         "permutations": "Whether to try permutations",
     }
 
     cloud_helper_name = "azure"
     delimiters = ("", "-")
     base_domains = ["blob.core.windows.net"]
     # Dirbusting is required to know whether a bucket is public
     supports_open_check = False
 
-    def check_bucket_exists(self, bucket_name, url):
+    async def check_bucket_exists(self, bucket_name, url):
         url = url.strip("/") + f"/{bucket_name}?restype=container"
-        response = self.helpers.request(url, retries=0)
+        response = await self.helpers.request(url, retries=0)
         status_code = getattr(response, "status_code", 0)
         existent_bucket = status_code != 0
-        return (existent_bucket, set())
+        return existent_bucket, set(), bucket_name, url
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1793rc0/bbot/modules/bucket_digitalocean.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 
 class bucket_digitalocean(bucket_aws):
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "slow", "cloud-enum", "web-thorough"]
     meta = {"description": "Check for DigitalOcean spaces related to target"}
-    options = {"max_threads": 10, "permutations": False}
+    options = {"permutations": False}
     options_desc = {
-        "max_threads": "Maximum number of threads for HTTP requests",
         "permutations": "Whether to try permutations",
     }
 
     cloud_helper_name = "digitalocean"
     delimiters = ("", "-")
     base_domains = ["digitaloceanspaces.com"]
     regions = ["ams3", "fra1", "nyc3", "sfo2", "sfo3", "sgp1"]
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1793rc0/bbot/modules/bucket_gcp.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,16 @@
     Adapted from https://github.com/RhinoSecurityLabs/GCPBucketBrute/blob/master/gcpbucketbrute.py
     """
 
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "cloud-enum", "web-basic", "web-thorough"]
     meta = {"description": "Check for Google object storage related to target"}
-    options = {"max_threads": 10, "permutations": False}
+    options = {"permutations": False}
     options_desc = {
-        "max_threads": "Maximum number of threads for HTTP requests",
         "permutations": "Whether to try permutations",
     }
 
     cloud_helper_name = "gcp"
     delimiters = ("", "-", ".", "_")
     base_domains = ["storage.googleapis.com"]
     bad_permissions = [
@@ -25,29 +24,29 @@
         "storage.objects.get",
         "storage.objects.create",
     ]
 
     def build_url(self, bucket_name, base_domain, region):
         return f"https://www.googleapis.com/storage/v1/b/{bucket_name}"
 
-    def check_bucket_open(self, bucket_name, url):
+    async def check_bucket_open(self, bucket_name, url):
         bad_permissions = []
         try:
             list_permissions = "&".join(["=".join(("permissions", p)) for p in self.bad_permissions])
             url = f"https://www.googleapis.com/storage/v1/b/{bucket_name}/iam/testPermissions?" + list_permissions
-            response = self.helpers.request(url)
+            response = await self.helpers.request(url)
             permissions = response.json()
             if isinstance(permissions, dict):
                 bad_permissions = list(permissions.get("permissions", {}))
         except Exception as e:
-            self.warning(f'Failed to enumerate permissions for bucket "{bucket_name}": {e}')
+            self.info(f'Failed to enumerate permissions for bucket "{bucket_name}": {e}')
         msg = ""
         if bad_permissions:
             perms_str = ",".join(bad_permissions)
             msg = f"Open permissions on storage bucket ({perms_str})"
         return (msg, set())
 
-    def check_bucket_exists(self, bucket_name, url):
-        response = self.helpers.request(url)
+    async def check_bucket_exists(self, bucket_name, url):
+        response = await self.helpers.request(url)
         status_code = getattr(response, "status_code", 0)
         existent_bucket = status_code not in (0, 400, 404)
-        return existent_bucket, set()
+        return existent_bucket, set(), bucket_name, url
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1793rc0/bbot/modules/builtwith.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,66 +18,70 @@
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "subdomain-enum", "passive", "safe"]
     meta = {"description": "Query Builtwith.com for subdomains", "auth_required": True}
     options = {"api_key": "", "redirects": True}
     options_desc = {"api_key": "Builtwith API key", "redirects": "Also look up inbound and outbound redirects"}
     base_url = "https://api.builtwith.com"
 
-    def ping(self):
+    async def ping(self):
         # builtwith does not have a ping feature, so we skip it to save API credits
         return
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
         # domains
-        subdomains = self.query(query, parse_fn=self.parse_domains, request_fn=self.request_domains)
+        subdomains = await self.query(query, parse_fn=self.parse_domains, request_fn=self.request_domains)
         if subdomains:
             for s in subdomains:
                 if s != event:
                     self.emit_event(s, "DNS_NAME", source=event)
         # redirects
         if self.config.get("redirects", True):
-            redirects = self.query(query, parse_fn=self.parse_redirects, request_fn=self.request_redirects)
+            redirects = await self.query(query, parse_fn=self.parse_redirects, request_fn=self.request_redirects)
             if redirects:
                 for r in redirects:
                     if r != event:
                         self.emit_event(r, "DNS_NAME", source=event, tags=["affiliate"])
 
-    def request_domains(self, query):
+    async def request_domains(self, query):
         url = f"{self.base_url}/v20/api.json?KEY={self.api_key}&LOOKUP={query}&NOMETA=yes&NOATTR=yes&HIDETEXT=yes&HIDEDL=yes"
-        return self.request_with_fail_count(url)
+        return await self.request_with_fail_count(url)
 
-    def request_redirects(self, query):
+    async def request_redirects(self, query):
         url = f"{self.base_url}/redirect1/api.json?KEY={self.api_key}&LOOKUP={query}"
-        return self.request_with_fail_count(url)
+        return await self.request_with_fail_count(url)
 
     def parse_domains(self, r, query):
         """
-        This method yields subdomains.
+        This method returns a set of subdomains.
         Each subdomain is an "FQDN" that was reported in the "Detailed Technology Profile" page on builtwith.com
 
         Parameters
         ----------
         r (requests Response): The raw requests response from the API
         query (string): The query used against the API
         """
+        results_set = set()
         json = r.json()
         if json:
-            for result in json.get("Results", []):
-                for chunk in result.get("Result", {}).get("Paths", []):
-                    domain = chunk.get("Domain", "")
-                    subdomain = chunk.get("SubDomain", "")
-                    if domain:
-                        if subdomain:
-                            domain = f"{subdomain}.{domain}"
-                        yield domain
+            results = json.get("Results", [])
+            if results:
+                for result in results:
+                    for chunk in result.get("Result", {}).get("Paths", []):
+                        domain = chunk.get("Domain", "")
+                        subdomain = chunk.get("SubDomain", "")
+                        if domain:
+                            if subdomain:
+                                domain = f"{subdomain}.{domain}"
+                            results_set.add(domain)
             else:
                 error = json.get("Errors", [{}])[0].get("Message", "Unknown Error")
                 if error:
                     self.verbose(f"No results for {query}: {error}")
+        return results_set
 
     def parse_redirects(self, r, query):
         """
         This method creates a set.
         Each entry in the set is either an Inbound or Outbound Redirect reported in the "Redirect Profile" page on builtwith.com
 
         Parameters
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1793rc0/bbot/modules/bypass403.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,28 +77,28 @@
 class bypass403(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "web-thorough"]
     meta = {"description": "Check 403 pages for common bypasses"}
     in_scope_only = True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         try:
             compare_helper = self.helpers.http_compare(event.data, allow_redirects=True)
         except HttpCompareError as e:
             self.debug(e)
             return
 
         for sig in signatures:
             sig = self.format_signature(sig, event)
             if sig[2] != None:
                 headers = dict(sig[2])
             else:
                 headers = None
-            match, reasons, reflection, subject_response = compare_helper.compare(
+            match, reasons, reflection, subject_response = await compare_helper.compare(
                 sig[1], headers=headers, method=sig[0], allow_redirects=True
             )
 
             # In some cases WAFs will respond with a 200 code which causes a false positive
             if subject_response != None:
                 for ws in waf_strings:
                     if ws in subject_response.text:
@@ -117,15 +117,15 @@
                         {"description": description, "host": str(event.host), "url": event.data},
                         "FINDING",
                         source=event,
                     )
                 else:
                     self.debug(f"Status code changed to {str(subject_response.status_code)}, ignoring")
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if ("status-403" in event.tags) or ("status-401" in event.tags):
             return True
         return False
 
     def format_signature(self, sig, event):
         if sig[3] == True:
             cleaned_path = event.parsed.path.strip("/")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/c99.py` & `bbot-1.0.5.1793rc0/bbot/modules/c99.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Query the C99 API for subdomains", "auth_required": True}
     options = {"api_key": ""}
     options_desc = {"api_key": "c99.nl API key"}
 
     base_url = "https://api.c99.nl"
 
-    def ping(self):
+    async def ping(self):
         url = f"{self.base_url}/randomnumber?key={self.api_key}&between=1,100&json"
-        response = self.request_with_fail_count(url)
+        response = await self.request_with_fail_count(url)
         assert response.json()["success"] == True
 
-    def request_url(self, query):
+    async def request_url(self, query):
         url = f"{self.base_url}/subdomainfinder?key={self.api_key}&domain={self.helpers.quote(query)}&json"
-        return self.request_with_fail_count(url)
+        return await self.request_with_fail_count(url)
 
     def parse_results(self, r, query):
         j = r.json()
         if isinstance(j, dict):
             subdomains = j.get("subdomains", [])
             if subdomains:
                 for s in subdomains:
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/censys.py` & `bbot-1.0.5.1793rc0/bbot/modules/httpx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,155 @@
-from contextlib import suppress
+import json
+import subprocess
+from bbot.modules.base import BaseModule
+from bbot.core.helpers.web import is_login_page
 
-from censys.common import exceptions
-from censys.search import CensysHosts
-from censys.search import CensysCertificates
 
-from bbot.modules.shodan_dns import shodan_dns
+class httpx(BaseModule):
+    watched_events = ["OPEN_TCP_PORT", "URL_UNVERIFIED", "URL"]
+    produced_events = ["URL", "HTTP_RESPONSE"]
+    flags = ["active", "safe", "web-basic", "web-thorough", "social-enum", "subdomain-enum", "cloud-enum"]
+    meta = {"description": "Visit webpages. Many other modules rely on httpx"}
 
-
-class censys(shodan_dns):
-    watched_events = ["DNS_NAME"]
-    produced_events = ["DNS_NAME", "EMAIL_ADDRESS", "IP_ADDRESS", "OPEN_PORT", "PROTOCOL"]
-    flags = ["subdomain-enum", "email-enum", "passive", "safe"]
-    meta = {"description": "Query the Censys API", "auth_required": True}
-    options = {"api_id": "", "api_secret": "", "max_records": 1000}
+    batch_size = 500
+    options = {"threads": 50, "in_scope_only": True, "version": "1.2.5", "max_response_size": 5242880}
     options_desc = {
-        "api_id": "Censys.io API ID",
-        "api_secret": "Censys.io API Secret",
-        "max_records": "Limit results to help prevent exceeding API quota",
+        "threads": "Number of httpx threads to use",
+        "in_scope_only": "Only visit web resources that are in scope.",
+        "version": "httpx version",
+        "max_response_size": "Max response size in bytes",
     }
+    deps_ansible = [
+        {
+            "name": "Download httpx",
+            "unarchive": {
+                "src": "https://github.com/projectdiscovery/httpx/releases/download/v#{BBOT_MODULES_HTTPX_VERSION}/httpx_#{BBOT_MODULES_HTTPX_VERSION}_#{BBOT_OS}_#{BBOT_CPU_ARCH}.zip",
+                "include": "httpx",
+                "dest": "#{BBOT_TOOLS}",
+                "remote_src": True,
+            },
+        }
+    ]
+
+    scope_distance_modifier = 1
+    _priority = 2
+
+    async def setup(self):
+        self.threads = self.config.get("threads", 50)
+        self.timeout = self.scan.config.get("httpx_timeout", 5)
+        self.retries = self.scan.config.get("httpx_retries", 1)
+        self.max_response_size = self.config.get("max_response_size", 5242880)
+        self.visited = set()
+        return True
+
+    async def filter_event(self, event):
+        if "_wildcard" in str(event.host).split("."):
+            return False, "event is wildcard"
+
+        if "unresolved" in event.tags:
+            return False, "event is unresolved"
+
+        if event.module == self:
+            return False, "event is from self"
+
+        if "spider-danger" in event.tags:
+            return False, "event has spider danger"
+
+        # scope filtering
+        in_scope_only = self.config.get("in_scope_only", True)
+        safe_to_visit = "httpx-safe" in event.tags
+        if not safe_to_visit and (in_scope_only and not self.scan.in_scope(event)):
+            return False, "event is not in scope"
+        # reject base URLs to avoid visiting a resource twice
+        # note: speculate makes open ports from
+        return True
+
+    async def handle_batch(self, *events):
+        stdin = {}
+        for e in events:
+            url_hash = None
+            if e.type.startswith("URL"):
+                # we NEED the port, otherwise httpx will try HTTPS even for HTTP URLs
+                url = e.with_port().geturl()
+                if e.parsed.path == "/":
+                    url_hash = hash((e.host, e.port))
+            else:
+                url = str(e.data)
+                url_hash = hash((e.host, e.port))
+
+            if url_hash not in self.visited:
+                stdin[url] = e
+                if url_hash is not None:
+                    self.visited.add(url_hash)
+
+        if not stdin:
+            return
+
+        command = [
+            "httpx",
+            "-silent",
+            "-json",
+            "-include-response",
+            "-threads",
+            self.threads,
+            "-timeout",
+            self.timeout,
+            "-retries",
+            self.retries,
+            "-header",
+            f"User-Agent: {self.scan.useragent}",
+            "-response-size-to-read",
+            f"{self.max_response_size}",
+            # "-r",
+            # self.helpers.resolver_file,
+        ]
+        for hk, hv in self.scan.config.get("http_headers", {}).items():
+            command += ["-header", f"{hk}: {hv}"]
+        proxy = self.scan.config.get("http_proxy", "")
+        if proxy:
+            command += ["-http-proxy", proxy]
+        async for line in self.helpers.run_live(command, input=list(stdin), stderr=subprocess.DEVNULL):
+            try:
+                j = json.loads(line)
+            except json.decoder.JSONDecodeError:
+                self.debug(f"Failed to decode line: {line}")
+                continue
+
+            url = j.get("url", "")
+            status_code = int(j.get("status_code", 0))
+            if status_code == 0:
+                self.debug(f'No HTTP status code for "{url}"')
+                continue
 
-    deps_pip = ["censys~=2.1.9"]
+            source_event = stdin.get(j.get("input", ""), None)
 
-    def setup(self):
-        self.max_records = self.config.get("max_records", 1000)
-        self.api_id = self.config.get("api_id", "")
-        self.api_secret = self.config.get("api_secret", "")
-        self._cert_name_threshold = 20
-        with suppress(Exception):
-            self.hosts = CensysHosts(api_id=self.api_id, api_secret=self.api_secret)
-        with suppress(Exception):
-            self.certificates = CensysCertificates(api_id=self.api_id, api_secret=self.api_secret)
-        return super().setup()
-
-    def ping(self):
-        quota = self.certificates.quota()
-        used = int(quota["used"])
-        allowance = int(quota["allowance"])
-        assert used < allowance, "No quota remaining"
-
-    def query(self, query):
-        emails = set()
-        dns_names = set()
-        ip_addresses = dict()
-        try:
-            # certificates
-            certificate_query = f"parsed.names: {query}"
-            certificate_fields = ["parsed.names", "parsed.issuer_dn", "parsed.subject_dn"]
-            for result in self.certificates.search(
-                certificate_query, fields=certificate_fields, max_records=self.max_records
-            ):
-                parsed_names = result.get("parsed.names", [])
-                # helps filter out third-party certs with a lot of garbage names
-                _filter = lambda x: True
-                domain = self.helpers.tldextract(query).domain
-                if len(parsed_names) > self._cert_name_threshold:
-                    _filter = lambda x: domain in str(x.lower())
-                parsed_names = list(filter(_filter, parsed_names))
-                dns_names.update(set([n.lstrip(".*").rstrip(".").lower() for n in parsed_names]))
-                emails.update(set(self.helpers.extract_emails(result.get("parsed.issuer_dn", ""))))
-                emails.update(set(self.helpers.extract_emails(result.get("parsed.subject_dn", ""))))
-
-            # hosts
-            per_page = 100
-            pages = max(1, int(self.max_records / per_page))
-            hosts_query = f"services.tls.certificates.leaf_data.names: {query} or services.tls.certificates.leaf_data.subject.email_address: {query}"
-            for i, page in enumerate(self.hosts.search(hosts_query, per_page=per_page, pages=pages)):
-                for result in page:
-                    ip = result.get("ip", "")
-                    if not ip:
-                        continue
-                    ip_addresses[ip] = []
-                    services = result.get("services", [])
-                    for service in services:
-                        port = service.get("port")
-                        service_name = service.get("service_name", "")
-                        transport_protocol = service.get("transport_protocol", "")
-                        if not port or not transport_protocol:
-                            continue
-                        ip_addresses[ip].append((port, service_name, transport_protocol))
-                if self.scan.stopping:
-                    break
-
-        except exceptions.CensysRateLimitExceededException:
-            self.warning("Exceeded Censys account limits")
-        except exceptions.CensysException as e:
-            self.warning(f"Error with API: {e}")
-        except Exception as e:
-            self.warning(f"Unknown error: {e}")
-
-        return emails, dns_names, ip_addresses
-
-    def handle_event(self, event):
-        query = self.make_query(event)
-        emails, dns_names, ip_addresses = self.query(query)
-        for email in emails:
-            self.emit_event(email, "EMAIL_ADDRESS", source=event)
-        for dns_name in dns_names:
-            self.emit_event(dns_name, "DNS_NAME", source=event)
-        for ip, services in ip_addresses.items():
-            ip_event = self.make_event(ip, "IP_ADDRESS", source=event)
-            if not ip_event:
+            if source_event is None:
+                self.warning(f"Unable to correlate source event from: {line}")
                 continue
-            self.emit_event(ip_event)
-            for port, service_name, transport_protocol in services:
-                port_data = self.helpers.make_netloc(ip, port)
-                port_type = f"OPEN_{transport_protocol.upper()}_PORT"
-                port_event = self.make_event(port_data, port_type, source=ip_event)
-                if not port_event:
-                    continue
-                self.emit_event(port_event)
-                if service_name:
-                    service_name = str(service_name).upper()
-                    protocol_data = {"host": port_data, "protocol": service_name}
-                    self.emit_event(protocol_data, "PROTOCOL", source=port_event)
-
-    @property
-    def auth_secret(self):
-        return self.api_id and self.api_secret
+
+            # discard 404s from unverified URLs
+            if source_event.type == "URL_UNVERIFIED" and status_code in (404,):
+                self.debug(f'Discarding 404 from "{url}"')
+                continue
+
+            # main URL
+            httpx_ip = j.get("host", "unknown")
+            tags = [f"status-{status_code}", f"ip-{httpx_ip}"]
+            # detect login pages
+            if is_login_page(j.get("body", "")):
+                tags.append("login-page")
+            # grab title
+            title = self.helpers.tagify(j.get("title", ""), maxlen=30)
+            if title:
+                tags.append(f"http-title-{title}")
+            url_event = self.make_event(url, "URL", source_event, tags=tags)
+            if url_event:
+                if url_event != source_event:
+                    self.emit_event(url_event)
+                else:
+                    url_event._resolved.set()
+                # HTTP response
+                self.emit_event(j, "HTTP_RESPONSE", url_event, tags=url_event.tags, internal=True)
+
+    async def cleanup(self):
+        resume_file = self.helpers.current_dir / "resume.cfg"
+        resume_file.unlink(missing_ok=True)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1793rc0/bbot/modules/columbus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from bbot.modules.crobat import crobat
+from .crobat import crobat
 
 
-class certspotter(crobat):
+class columbus(crobat):
+    flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query Certspotter's API for subdomains"}
+    meta = {"description": "Query the Columbus Project API for subdomains"}
 
-    base_url = "https://api.certspotter.com/v1"
+    base_url = "https://columbus.elmasy.com/api/lookup"
 
-    def request_url(self, query):
-        url = f"{self.base_url}/issuances?domain={self.helpers.quote(query)}&include_subdomains=true&expand=dns_names"
-        return self.request_with_fail_count(url)
+    async def request_url(self, query):
+        url = f"{self.base_url}/{self.helpers.quote(query)}"
+        return await self.request_with_fail_count(url)
 
     def parse_results(self, r, query):
+        results = set()
         json = r.json()
-        if json:
-            for r in json:
-                for dns_name in r.get("dns_names", []):
-                    yield dns_name.lstrip(".*").rstrip(".")
+        if json and isinstance(json, list):
+            return set([f"{s.lower()}.{query}" for s in json])
+        return results
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1793rc0/bbot/modules/crobat.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,44 +18,45 @@
     abort_after_failures = 5
     # whether to reject wildcard DNS_NAMEs
     reject_wildcards = "strict"
     # this helps combat rate limiting by ensuring that a query doesn't execute
     # until the queue is ready to receive its results
     _qsize = 1
 
-    def setup(self):
+    async def setup(self):
         self.processed = set()
         self.http_timeout = self.scan.config.get("http_timeout", 10)
         self._failures = 0
         return True
 
-    def _is_wildcard(self, query):
-        for domain, wildcard_rdtypes in self.helpers.is_wildcard_domain(query).items():
-            if any(t in wildcard_rdtypes for t in ("A", "AAAA", "CNAME")):
-                return True
+    async def _is_wildcard(self, query):
+        if self.helpers.is_dns_name(query):
+            for domain, wildcard_rdtypes in (await self.helpers.is_wildcard_domain(query)).items():
+                if any(t in wildcard_rdtypes for t in ("A", "AAAA", "CNAME")):
+                    return True
         return False
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         """
         This filter_event is used across many modules
         """
         query = self.make_query(event)
         # reject if already processed
         if self.already_processed(query):
             return False, "Event was already processed"
-        eligible, reason = self.eligible_for_enumeration(event)
+        eligible, reason = await self.eligible_for_enumeration(event)
         if eligible:
             self.processed.add(hash(query))
             return True, reason
         return False, reason
 
-    def eligible_for_enumeration(self, event):
+    async def eligible_for_enumeration(self, event):
         query = self.make_query(event)
         # check if wildcard
-        is_wildcard = self._is_wildcard(query)
+        is_wildcard = await self._is_wildcard(query)
         # check if cloud
         is_cloud = False
         if any(t.startswith("cloud-") for t in event.tags):
             is_cloud = True
         # reject if it's a cloud resource and not in our target
         if is_cloud and event not in self.scan.target:
             return False, "Event is a cloud resource and not a direct target"
@@ -73,59 +74,67 @@
 
     def already_processed(self, hostname):
         for parent in self.helpers.domain_parents(hostname, include_self=True):
             if hash(parent) in self.processed:
                 return True
         return False
 
-    def abort_if(self, event):
+    async def abort_if(self, event):
         # this helps weed out unwanted results when scanning IP_RANGES and wildcard domains
         if "in-scope" not in event.tags:
             return True
-        if self._is_wildcard(event.data):
+        if await self._is_wildcard(event.data):
             return True
         return False
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        results = self.query(query)
+        results = await self.query(query)
         if results:
             for hostname in set(results):
                 if hostname:
                     try:
                         hostname = self.helpers.validators.validate_host(hostname)
                     except ValueError as e:
                         self.verbose(e)
                         continue
                     if hostname and hostname.endswith(f".{query}") and not hostname == event.data:
                         self.emit_event(hostname, "DNS_NAME", event, abort_if=self.abort_if)
 
-    def request_url(self, query):
+    async def request_url(self, query):
         url = f"{self.base_url}/subdomains/{self.helpers.quote(query)}"
-        return self.request_with_fail_count(url)
+        return await self.request_with_fail_count(url)
 
     def make_query(self, event):
         if "target" in event.tags:
             query = str(event.data)
         else:
             query = self.helpers.parent_domain(event.data).lower()
         return ".".join([s for s in query.split(".") if s != "_wildcard"])
 
     def parse_results(self, r, query=None):
         json = r.json()
         if json:
             for hostname in json:
                 yield hostname
 
-    def query(self, query, parse_fn=None, request_fn=None):
+    async def query(self, query, parse_fn=None, request_fn=None):
         if parse_fn is None:
             parse_fn = self.parse_results
         if request_fn is None:
             request_fn = self.request_url
         try:
-            results = list(parse_fn(request_fn(query), query))
+            response = await request_fn(query)
+            try:
+                results = list(parse_fn(response, query))
+            except Exception as e:
+                if response:
+                    self.info(f'Status code {response.status_code} for query "{query}"')
+                    self.debug(response.text)
+                else:
+                    self.info(f'Error parsing results for "{query}": {e}', trace=True)
+                return
             if results:
                 return results
             self.debug(f'No results for "{query}"')
         except Exception as e:
-            self.info(f"Error retrieving results for {query}: {e}")
-            self.trace()
+            self.info(f"Error retrieving results for {query}: {e}", trace=True)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/crt.py` & `bbot-1.0.5.1793rc0/bbot/modules/crt.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     meta = {"description": "Query crt.sh (certificate transparency) for subdomains"}
 
     base_url = "https://crt.sh"
     reject_wildcards = False
 
-    def setup(self):
+    async def setup(self):
         self.cert_ids = set()
-        return super().setup()
+        return await super().setup()
 
-    def request_url(self, query):
+    async def request_url(self, query):
         params = {"q": f"%.{query}", "output": "json"}
         url = self.helpers.add_get_params(self.base_url, params).geturl()
-        return self.request_with_fail_count(url, timeout=self.http_timeout + 10)
+        return await self.request_with_fail_count(url, timeout=self.http_timeout + 30)
 
     def parse_results(self, r, query):
         j = r.json()
         for cert_info in j:
             if not type(cert_info) == dict:
                 continue
             cert_id = cert_info.get("id")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1793rc0/bbot/modules/deadly/ffuf.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,28 +42,26 @@
 
     banned_characters = [" "]
 
     blacklist = ["images", "css", "image"]
 
     in_scope_only = True
 
-    def setup(self):
+    async def setup(self):
         self.canary = "".join(random.choice(string.ascii_lowercase) for i in range(10))
         wordlist_url = self.config.get("wordlist", "")
         self.debug(f"Using wordlist [{wordlist_url}]")
-        self.wordlist = self.helpers.wordlist(wordlist_url)
-        f = open(self.wordlist, "r")
-        self.wordlist_lines = f.readlines()
-        f.close()
+        self.wordlist = await self.helpers.wordlist(wordlist_url)
+        self.wordlist_lines = list(self.helpers.read_file(self.wordlist))
         self.tempfile, tempfile_len = self.generate_templist()
         self.verbose(f"Generated dynamic wordlist with length [{str(tempfile_len)}]")
-        self.extensions = self.config.get("extensions")
+        self.extensions = self.config.get("extensions", "")
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         if self.helpers.url_depth(event.data) > self.config.get("max_depth"):
             self.debug(f"Exceeded max depth, aborting event")
             return
 
         # only FFUF against a directory
         if "." in event.parsed.path.split("/")[-1]:
             self.debug("Aborting FFUF as period was detected in right-most path segment (likely a file)")
@@ -73,40 +71,40 @@
             fixed_url = event.data.rstrip("/") + "/"
 
         exts = ["", "/"]
         if self.extensions:
             for ext in self.extensions.split(","):
                 exts.append(f".{ext}")
 
-        filters = self.baseline_ffuf(fixed_url, exts=exts)
-        for r in self.execute_ffuf(self.tempfile, fixed_url, exts=exts, filters=filters):
+        filters = await self.baseline_ffuf(fixed_url, exts=exts)
+        async for r in self.execute_ffuf(self.tempfile, fixed_url, exts=exts, filters=filters):
             self.emit_event(r["url"], "URL_UNVERIFIED", source=event, tags=[f"status-{r['status']}"])
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if "endpoint" in event.tags:
             self.debug(f"rejecting URL [{event.data}] because we don't ffuf endpoints")
             return False
         return True
 
-    def baseline_ffuf(self, url, exts=[""], prefix="", suffix="", mode="normal"):
+    async def baseline_ffuf(self, url, exts=[""], prefix="", suffix="", mode="normal"):
         filters = {}
         for ext in exts:
             self.debug(f"running baseline for URL [{url}] with ext [{ext}]")
             # For each "extension", we will attempt to build a baseline using 4 requests
 
             canary_results = []
 
             canary_length = 4
             canary_list = []
             for i in range(0, 4):
                 canary_list.append("".join(random.choice(string.ascii_lowercase) for i in range(canary_length)))
                 canary_length += 2
 
             canary_temp_file = self.helpers.tempfile(canary_list, pipe=False)
-            for canary_r in self.execute_ffuf(
+            async for canary_r in self.execute_ffuf(
                 canary_temp_file,
                 url,
                 prefix=prefix,
                 suffix=suffix,
                 mode=mode,
                 baseline=True,
                 apply_filters=False,
@@ -190,15 +188,15 @@
                 continue
 
             # if even the line count isn't stable, we can only reliably count on the result if the code is different
             filters[ext] = ["-fc", f"{str(canary_results[0]['status'])}"]
 
         return filters
 
-    def execute_ffuf(
+    async def execute_ffuf(
         self,
         tempfile,
         url,
         prefix="",
         suffix="",
         exts=[""],
         filters={},
@@ -257,15 +255,15 @@
 
                     else:
                         command += filters[ext]
             else:
                 command.append("-mc")
                 command.append("all")
 
-            for found in self.helpers.run_live(command):
+            async for found in self.helpers.run_live(command):
                 try:
                     found_json = json.loads(found)
                     input_json = found_json.get("input", {})
                     if type(input_json) != dict:
                         self.debug("Error decoding JSON from ffuf")
                         continue
                     encoded_input = input_json.get("FUZZ", "")
@@ -276,29 +274,30 @@
                         if input_val.rstrip() == self.canary:
                             self.debug("Found canary! aborting...")
                             return
                         else:
                             if mode == "normal":
                                 # before emitting, we are going to send another baseline. This will immediately catch things like a WAF flipping blocking on us mid-scan
                                 if baseline == False:
-                                    pre_emit_temp_canary = list(
-                                        self.execute_ffuf(
+                                    pre_emit_temp_canary = [
+                                        f
+                                        async for f in self.execute_ffuf(
                                             self.helpers.tempfile(
                                                 ["".join(random.choice(string.ascii_lowercase) for i in range(4))],
                                                 pipe=False,
                                             ),
                                             url,
                                             prefix=prefix,
                                             suffix=suffix,
                                             mode=mode,
                                             exts=[ext],
                                             baseline=True,
                                             filters=filters,
                                         )
-                                    )
+                                    ]
                                     if len(pre_emit_temp_canary) == 0:
                                         yield found_json
                                     else:
                                         self.warning(
                                             "Baseline changed mid-scan. This is probably due to a WAF turning on a block against you."
                                         )
                                         self.warning(f"Aborting the current run against [{url}]")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1793rc0/bbot/modules/deadly/nuclei.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "aggressive"]
     meta = {"description": "Fast and customisable vulnerability scanner"}
 
     batch_size = 25
 
     options = {
-        "version": "2.8.9",
+        "version": "2.9.4",
         "tags": "",
         "templates": "",
         "severity": "",
         "ratelimit": 150,
         "concurrency": 25,
         "mode": "manual",
         "etags": "",
@@ -46,19 +46,19 @@
                 "remote_src": True,
             },
         }
     ]
     deps_pip = ["pyyaml~=6.0"]
     in_scope_only = True
 
-    def setup(self):
+    async def setup(self):
         # attempt to update nuclei templates
         self.nuclei_templates_dir = self.helpers.tools_dir / "nuclei-templates"
         self.info("Updating Nuclei templates")
-        update_results = self.helpers.run(
+        update_results = await self.helpers.run(
             ["nuclei", "-update-template-dir", self.nuclei_templates_dir, "-update-templates"]
         )
         if update_results.stderr:
             if "Successfully downloaded nuclei-templates" in update_results.stderr:
                 self.success("Successfully updated nuclei templates")
             elif "No new updates found for nuclei templates" in update_results.stderr:
                 self.info("Nuclei templates already up-to-date")
@@ -123,18 +123,18 @@
             )
             self.info(
                 f"Template Severity: Critical [{self.nucleibudget.severity_stats['critical']}] High [{self.nucleibudget.severity_stats['high']}] Medium [{self.nucleibudget.severity_stats['medium']}] Low [{self.nucleibudget.severity_stats['low']}] Info [{self.nucleibudget.severity_stats['info']}] Unknown [{self.nucleibudget.severity_stats['unknown']}]"
             )
 
         return True
 
-    def handle_batch(self, *events):
+    async def handle_batch(self, *events):
         temp_target = self.helpers.make_target(events)
         nuclei_input = [str(e.data) for e in events]
-        for severity, template, host, url, name, extracted_results in self.execute_nuclei(nuclei_input):
+        async for severity, template, host, url, name, extracted_results in self.execute_nuclei(nuclei_input):
             # this is necessary because sometimes nuclei is inconsistent about the data returned in the host field
             cleaned_host = temp_target.get(host)
             source_event = self.correlate_event(events, cleaned_host)
 
             if url == "":
                 url = str(source_event.data)
 
@@ -166,18 +166,18 @@
 
     def correlate_event(self, events, host):
         for event in events:
             if host in event:
                 return event
         self.warning("Failed to correlate nuclei result with event")
 
-    def execute_nuclei(self, nuclei_input):
+    async def execute_nuclei(self, nuclei_input):
         command = [
             "nuclei",
-            "-json",
+            "-jsonl",
             "-update-template-dir",
             self.nuclei_templates_dir,
             "-rate-limit",
             self.ratelimit,
             "-concurrency",
             self.concurrency,
             "-disable-update-check",
@@ -203,15 +203,15 @@
         if self.mode == "budget":
             command.append("-t")
             command.append(self.budget_templates_file)
 
         stats_file = self.helpers.tempfile_tail(callback=self.log_nuclei_status)
         try:
             with open(stats_file, "w") as stats_fh:
-                for line in self.helpers.run_live(command, input=nuclei_input, stderr=stats_fh):
+                async for line in self.helpers.run_live(command, input=nuclei_input, stderr=stats_fh):
                     try:
                         j = json.loads(line)
                     except json.decoder.JSONDecodeError:
                         self.debug(f"Failed to decode line: {line}")
                         continue
 
                     template = j.get("template-id", "")
@@ -254,30 +254,31 @@
         requests = line.get("requests", "")
         rps = line.get("rps", "")
         templates = line.get("templates", "")
         total = line.get("total", "")
         status = f"[{duration}] | Templates: {templates} | Hosts: {hosts} | RPS: {rps} | Matched: {matched} | Errors: {errors} | Requests: {requests}/{total} ({percent}%)"
         self.info(status)
 
-    def cleanup(self):
+    async def cleanup(self):
         resume_file = self.helpers.current_dir / "resume.cfg"
         resume_file.unlink(missing_ok=True)
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if self.config.get("directory_only", True):
             if "endpoint" in event.tags:
                 self.debug(
                     f"rejecting URL [{str(event.data)}] because directory_only is true and event has endpoint tag"
                 )
                 return False
         return True
 
 
 class NucleiBudget:
     def __init__(self, budget, templates_dir):
+        self._yaml_files = {}
         self.templates_dir = templates_dir
         self.yaml_list = self.get_yaml_list()
         self.budget_paths = self.find_budget_paths(budget)
         self.collapsable_templates, self.severity_stats = self.find_collapsable_templates()
 
     def get_yaml_list(self):
         return list(self.templates_dir.rglob("*.yaml"))
@@ -295,15 +296,15 @@
                             path_frequency[path] = 1
 
         sorted_dict = dict(sorted(path_frequency.items(), key=lambda item: item[1], reverse=True))
         return list(dict(islice(sorted_dict.items(), budget)).keys())
 
     def get_yaml_request_attr(self, yf, attr):
         p = self.parse_yaml(yf)
-        requests = p.get("requests", [])
+        requests = p.get("http", [])
         for r in requests:
             raw = r.get("raw")
             if not raw:
                 res = r.get(attr)
                 yield res
 
     def get_yaml_info_attr(self, yf, attr):
@@ -353,13 +354,16 @@
                             if severity in severity_dict.keys():
                                 severity_dict[severity] += 1
                             else:
                                 severity_dict[severity] = 1
         return collapsable_templates, severity_dict
 
     def parse_yaml(self, yamlfile):
-        with open(yamlfile, "r") as stream:
-            try:
-                y = yaml.safe_load(stream)
-                return y
-            except yaml.YAMLError as e:
-                self.debug(f"failed to read yaml file: {e}")
+        if yamlfile not in self._yaml_files:
+            with open(yamlfile, "r") as stream:
+                try:
+                    y = yaml.safe_load(stream)
+                    self._yaml_files[yamlfile] = y
+                except yaml.YAMLError as e:
+                    self.warning(f"failed to load yaml file: {e}")
+                    return {}
+        return self._yaml_files[yamlfile]
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1793rc0/bbot/modules/deadly/vhost.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from bbot.modules.deadly.ffuf import ffuf
-
-from urllib.parse import urlparse
-import random
-import string
 import base64
+from urllib.parse import urlparse
+
+from bbot.modules.deadly.ffuf import ffuf
 
 
 class vhost(ffuf):
     watched_events = ["URL"]
     produced_events = ["VHOST", "DNS_NAME"]
     flags = ["active", "aggressive", "slow"]
     meta = {"description": "Fuzz for virtual hosts"}
@@ -34,82 +32,67 @@
                 "remote_src": True,
             },
         }
     ]
 
     in_scope_only = True
 
-    def setup(self):
-        self.canary = "".join(random.choice(string.ascii_lowercase) for i in range(10))
+    async def setup(self):
         self.scanned_hosts = {}
         self.wordcloud_tried_hosts = set()
-        self.wordlist = self.helpers.wordlist(self.config.get("wordlist"))
-        f = open(self.wordlist, "r")
-        self.wordlist_lines = f.readlines()
-        f.close()
-        self.ignore_redirects = True
-        self.tempfile, tempfile_len = self.generate_templist()
-        return True
-
-    @staticmethod
-    def get_parent_domain(domain):
-        domain_parts = domain.split(".")
-
-        if len(domain_parts) >= 3:
-            parent_domain = ".".join(domain_parts[1:])
-            return parent_domain
-        else:
-            return domain
+        return await super().setup()
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         if not self.helpers.is_ip(event.host) or self.config.get("force_basehost"):
             host = f"{event.parsed.scheme}://{event.parsed.netloc}"
             if host in self.scanned_hosts.keys():
                 return
             else:
                 self.scanned_hosts[host] = event
 
             # subdomain vhost check
             self.verbose("Main vhost bruteforce")
             if self.config.get("force_basehost"):
                 basehost = self.config.get("force_basehost")
             else:
-                basehost = self.get_parent_domain(event.parsed.netloc)
+                basehost = self.helpers.parent_domain(event.parsed.netloc)
 
             self.debug(f"Using basehost: {basehost}")
-            for vhost in self.ffuf_vhost(host, f".{basehost}", event):
+            async for vhost in self.ffuf_vhost(host, f".{basehost}", event):
                 self.verbose(f"Starting mutations check for {vhost}")
-                for vhost in self.ffuf_vhost(host, f".{basehost}", event, wordlist=self.mutations_check(vhost)):
+                async for vhost in self.ffuf_vhost(host, f".{basehost}", event, wordlist=self.mutations_check(vhost)):
                     pass
 
             # check existing host for mutations
             self.verbose("Checking for vhost mutations on main host")
-            for vhost in self.ffuf_vhost(
+            async for vhost in self.ffuf_vhost(
                 host, f".{basehost}", event, wordlist=self.mutations_check(event.parsed.netloc.split(".")[0])
             ):
                 pass
 
             # special vhost list
             self.verbose("Checking special vhost list")
-            for vhost in self.ffuf_vhost(
+            async for vhost in self.ffuf_vhost(
                 host,
                 "",
                 event,
                 wordlist=self.helpers.tempfile(self.special_vhost_list, pipe=False),
                 skip_dns_host=True,
             ):
                 pass
 
-    def ffuf_vhost(self, host, basehost, event, wordlist=None, skip_dns_host=False):
-        filters = self.baseline_ffuf(f"{host}/", exts=[""], suffix=basehost, mode="hostheader")
+    async def ffuf_vhost(self, host, basehost, event, wordlist=None, skip_dns_host=False):
+        filters = await self.baseline_ffuf(f"{host}/", exts=[""], suffix=basehost, mode="hostheader")
         self.debug(f"Baseline completed and returned these filters:")
         self.debug(filters)
         if not wordlist:
             wordlist = self.tempfile
-        for r in self.execute_ffuf(wordlist, host, exts=[""], suffix=basehost, filters=filters, mode="hostheader"):
+        async for r in self.execute_ffuf(
+            wordlist, host, exts=[""], suffix=basehost, filters=filters, mode="hostheader"
+        ):
             found_vhost_b64 = r["input"]["FUZZ"]
             vhost_dict = {"host": str(event.host), "url": host, "vhost": base64.b64decode(found_vhost_b64).decode()}
             if f"{vhost_dict['vhost']}{basehost}" != event.parsed.netloc:
                 self.emit_event(vhost_dict, "VHOST", source=event)
                 if skip_dns_host == False:
                     self.emit_event(f"{vhost_dict['vhost']}{basehost}", "DNS_NAME", source=event, tags=["vhost"])
 
@@ -119,25 +102,25 @@
         mutations_list = []
         for mutation in self.helpers.word_cloud.mutations(vhost):
             for i in ["", ".", "-"]:
                 mutations_list.append(i.join(mutation))
         mutations_list_file = self.helpers.tempfile(mutations_list, pipe=False)
         return mutations_list_file
 
-    def finish(self):
+    async def finish(self):
         # check existing hosts with wordcloud
         tempfile = self.helpers.tempfile(list(self.helpers.word_cloud.keys()), pipe=False)
 
         for host, event in self.scanned_hosts.items():
             if host not in self.wordcloud_tried_hosts:
                 event.parsed = urlparse(host)
 
                 self.verbose("Checking main host with wordcloud")
                 if self.config.get("force_basehost"):
                     basehost = self.config.get("force_basehost")
                 else:
-                    basehost = self.get_parent_domain(event.parsed.netloc)
+                    basehost = self.helpers.parent_domain(event.parsed.netloc)
 
-                for vhost in self.ffuf_vhost(host, f".{basehost}", event, wordlist=tempfile):
+                async for vhost in self.ffuf_vhost(host, f".{basehost}", event, wordlist=tempfile):
                     pass
 
                 self.wordcloud_tried_hosts.add(host)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1793rc0/bbot/modules/dnscommonsrv.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,20 +90,20 @@
 
 
 class dnscommonsrv(BaseModule):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Check for common SRV records"}
-    max_event_handlers = 10
+    max_event_handlers = 5
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         # skip SRV wildcards
-        if "SRV" in self.helpers.is_wildcard(event.host):
+        if "SRV" in await self.helpers.is_wildcard(event.host):
             return False
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         queries = [event.data] + [f"{srv}.{event.data}" for srv in common_srvs]
-        for query, results in self.helpers.resolve_batch(queries, type="srv"):
+        async for query, results in self.helpers.resolve_batch(queries, type="srv"):
             if results:
                 self.emit_event(query, "DNS_NAME", tags=["srv-record"], source=event)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1793rc0/bbot/modules/dnsdumpster.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 
 class dnsdumpster(crobat):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Query dnsdumpster for subdomains"}
 
-    deps_pip = ["bs4", "lxml~=4.9.2"]
-
     base_url = "https://dnsdumpster.com"
 
-    def query(self, domain):
+    async def query(self, domain):
         ret = []
         # first, get the CSRF tokens
-        res1 = self.request_with_fail_count(self.base_url)
+        res1 = await self.request_with_fail_count(self.base_url)
         status_code = getattr(res1, "status_code", 0)
         if status_code in [429]:
             self.verbose(f'Too many requests "{status_code}"')
             return ret
         elif status_code not in [200]:
             self.verbose(f'Bad response code "{status_code}" from DNSDumpster')
             return ret
         else:
             self.debug(f'Valid response code "{status_code}" from DNSDumpster')
-        html = BeautifulSoup(res1.content, features="lxml")
+        html = BeautifulSoup(res1.content, "html.parser")
         csrftoken = None
         csrfmiddlewaretoken = None
         try:
             for cookie in res1.headers.get("set-cookie", "").split(";"):
                 try:
                     k, v = cookie.split("=", 1)
                 except ValueError:
@@ -52,15 +50,15 @@
             self.debug("Successfully obtained CSRF tokens")
 
         if self.scan.stopping:
             return
 
         # Otherwise, do the needful
         subdomains = set()
-        res2 = self.request_with_fail_count(
+        res2 = await self.request_with_fail_count(
             f"{self.base_url}/",
             method="POST",
             cookies={"csrftoken": csrftoken},
             data={
                 "csrfmiddlewaretoken": csrfmiddlewaretoken,
                 "targetip": str(domain).lower(),
                 "user": "free",
@@ -71,14 +69,14 @@
             },
         )
         status_code = getattr(res2, "status_code", 0)
         if status_code not in [200]:
             self.verbose(f'Bad response code "{status_code}" from DNSDumpster')
             return ret
 
-        html = BeautifulSoup(res2.content, features="lxml")
+        html = BeautifulSoup(res2.content, "html.parser")
         escaped_domain = re.escape(domain)
         match_pattern = re.compile(r"^[\w\.-]+\." + escaped_domain + r"$")
         for subdomain in html.findAll(text=match_pattern):
             subdomains.add(str(subdomain).strip().lower())
 
         return list(subdomains)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1793rc0/bbot/modules/dnszonetransfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,40 +10,42 @@
     produced_events = ["DNS_NAME"]
     meta = {"description": "Attempt DNS zone transfers"}
     options = {"timeout": 10}
     options_desc = {"timeout": "Max seconds to wait before timing out"}
     max_event_handlers = 5
     suppress_dupes = False
 
-    def setup(self):
+    async def setup(self):
         self.timeout = self.config.get("timeout", 10)
         return True
 
-    def filter_event(self, event):
-        if any([x in event.tags for x in ("ns_record", "soa_record")]):
+    async def filter_event(self, event):
+        if any([x in event.tags for x in ("ns-record", "soa-record")]):
             return True
         return False
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         domain = event.data
         self.debug("Finding nameservers with NS/SOA query")
-        nameservers = list(self.helpers.resolve(event.data, type=("NS", "SOA")))
+        nameservers = list(await self.helpers.resolve(event.data, type=("NS", "SOA")))
         nameserver_ips = set()
         for n in nameservers:
-            nameserver_ips.update(self.helpers.resolve(n))
+            nameserver_ips.update(await self.helpers.resolve(n))
         self.debug(f"Found {len(nameservers):} nameservers for domain {domain}")
         for nameserver in nameserver_ips:
             if self.scan.stopping:
                 break
             try:
                 self.debug(f"Attempting zone transfer against {nameserver} for domain {domain}")
-                xfr_answer = dns.query.xfr(nameserver, domain, timeout=self.timeout, lifetime=self.timeout)
+                xfr_answer = await self.scan.run_in_executor(
+                    dns.query.xfr, nameserver, domain, timeout=self.timeout, lifetime=self.timeout
+                )
                 zone = dns.zone.from_xfr(xfr_answer)
             except Exception as e:
-                self.debug(f"Error retrieving zone: {e}")
+                self.debug(f"Error retrieving zone for {domain}: {e}")
                 continue
             self.hugesuccess(f"Successful zone transfer against {nameserver} for domain {domain}!")
             finding_description = f"Successful DNS zone transfer against {nameserver} for {domain}"
             self.emit_event({"host": str(event.host), "description": finding_description}, "FINDING", source=event)
             for name, ttl, rdata in zone.iterate_rdatas():
                 if str(name) == "@":
                     parent_data = domain
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1793rc0/bbot/modules/ffuf_shortnames.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,30 +68,28 @@
                 "remote_src": True,
             },
         }
     ]
 
     in_scope_only = True
 
-    def setup(self):
+    async def setup(self):
         self.canary = "".join(random.choice(string.ascii_lowercase) for i in range(10))
         wordlist = self.config.get("wordlist", "")
         if not wordlist:
             wordlist = f"{self.helpers.wordlist_dir}/ffuf_shortname_candidates.txt"
         self.debug(f"Using [{wordlist}] for shortname candidate list")
-        self.wordlist = self.helpers.wordlist(wordlist)
-        f = open(self.wordlist, "r")
-        self.wordlist_lines = f.readlines()
-        f.close()
+        self.wordlist = await self.helpers.wordlist(wordlist)
+        self.wordlist_lines = list(self.helpers.read_file(self.wordlist))
 
         wordlist_extensions = self.config.get("wordlist_extensions", "")
         if not wordlist_extensions:
             wordlist_extensions = f"{self.helpers.wordlist_dir}/raft-small-extensions-lowercase_CLEANED.txt"
         self.debug(f"Using [{wordlist_extensions}] for shortname candidate extension list")
-        self.wordlist_extensions = self.helpers.wordlist(wordlist_extensions)
+        self.wordlist_extensions = await self.helpers.wordlist(wordlist_extensions)
         self.extensions = self.config.get("extensions")
         self.ignore_redirects = self.config.get("ignore_redirects")
 
         self.per_host_collection = {}
         self.shortname_to_event = {}
         return True
 
@@ -112,18 +110,18 @@
         delimeters = ["_", "-"]
         for d in delimeters:
             if d in hint:
                 if not hint.startswith(d) and not hint.endswith(d):
                     return d, hint.split(d)[0], hint.split(d)[1]
         return None
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         if event.source.type == "URL":
             filename_hint = re.sub(r"~\d", "", event.parsed.path.rsplit(".", 1)[0].split("/")[-1]).lower()
 
             host = f"{event.source.parsed.scheme}://{event.source.parsed.netloc}/"
             if host not in self.per_host_collection.keys():
                 self.per_host_collection[host] = [(filename_hint, event.source.data)]
 
@@ -147,47 +145,49 @@
             else:
                 tempfile = self.helpers.tempfile([filename_hint], pipe=False)
                 tempfile_len = 1
 
             if tempfile_len > 0:
                 if "shortname-file" in event.tags:
                     for ext in used_extensions:
-                        for r in self.execute_ffuf(tempfile, root_url, suffix=f".{ext}"):
+                        async for r in self.execute_ffuf(tempfile, root_url, suffix=f".{ext}"):
                             self.emit_event(r["url"], "URL_UNVERIFIED", source=event, tags=[f"status-{r['status']}"])
 
                 elif "shortname-directory" in event.tags:
-                    for r in self.execute_ffuf(tempfile, root_url, exts=["/"]):
+                    async for r in self.execute_ffuf(tempfile, root_url, exts=["/"]):
                         r_url = f"{r['url'].rstrip('/')}/"
                         self.emit_event(r_url, "URL_UNVERIFIED", source=event, tags=[f"status-{r['status']}"])
 
             if self.config.get("find_delimeters"):
                 if "shortname-directory" in event.tags:
                     delimeter_r = self.find_delimeter(filename_hint)
                     if delimeter_r:
                         delimeter, prefix, partial_hint = delimeter_r
                         self.verbose(f"Detected delimeter [{delimeter}] in hint [{filename_hint}]")
                         tempfile, tempfile_len = self.generate_templist(prefix=partial_hint)
-                        for r in self.execute_ffuf(tempfile, root_url, prefix=f"{prefix}{delimeter}", exts=["/"]):
+                        async for r in self.execute_ffuf(
+                            tempfile, root_url, prefix=f"{prefix}{delimeter}", exts=["/"]
+                        ):
                             self.emit_event(r["url"], "URL_UNVERIFIED", source=event, tags=[f"status-{r['status']}"])
 
                 elif "shortname-file" in event.tags:
                     for ext in used_extensions:
                         delimeter_r = self.find_delimeter(filename_hint)
                         if delimeter_r:
                             delimeter, prefix, partial_hint = delimeter_r
                             self.verbose(f"Detected delimeter [{delimeter}] in hint [{filename_hint}]")
                             tempfile, tempfile_len = self.generate_templist(prefix=partial_hint)
-                            for r in self.execute_ffuf(
+                            async for r in self.execute_ffuf(
                                 tempfile, root_url, prefix=f"{prefix}{delimeter}", suffix=f".{ext}"
                             ):
                                 self.emit_event(
                                     r["url"], "URL_UNVERIFIED", source=event, tags=[f"status-{r['status']}"]
                                 )
 
-    def finish(self):
+    async def finish(self):
         if self.config.get("find_common_prefixes"):
             per_host_collection = dict(self.per_host_collection)
             self.per_host_collection.clear()
 
             for host, hint_tuple_list in per_host_collection.items():
                 hint_list = [x[0] for x in hint_tuple_list]
 
@@ -204,28 +204,30 @@
                                 tempfile, tempfile_len = self.generate_templist(prefix=partial_hint)
 
                                 if "shortname-directory" in self.shortname_to_event[hint].tags:
                                     self.verbose(
                                         f"Running common prefix check for URL_HINT: {hint} with prefix: {prefix} and partial_hint: {partial_hint}"
                                     )
 
-                                    for r in self.execute_ffuf(tempfile, url, prefix=prefix, exts=["/"]):
+                                    async for r in self.execute_ffuf(tempfile, url, prefix=prefix, exts=["/"]):
                                         self.emit_event(
                                             r["url"],
                                             "URL_UNVERIFIED",
                                             source=self.shortname_to_event[hint],
                                             tags=[f"status-{r['status']}"],
                                         )
                                 elif "shortname-file" in self.shortname_to_event[hint].tags:
                                     used_extensions = self.build_extension_list(self.shortname_to_event[hint])
 
                                     for ext in used_extensions:
                                         self.verbose(
                                             f"Running common prefix check for URL_HINT: {hint} with prefix: {prefix}, extension: .{ext}, and partial_hint: {partial_hint}"
                                         )
-                                        for r in self.execute_ffuf(tempfile, url, prefix=prefix, suffix=f".{ext}"):
+                                        async for r in self.execute_ffuf(
+                                            tempfile, url, prefix=prefix, suffix=f".{ext}"
+                                        ):
                                             self.emit_event(
                                                 r["url"],
                                                 "URL_UNVERIFIED",
                                                 source=self.shortname_to_event[hint],
                                                 tags=[f"status-{r['status']}"],
                                             )
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1793rc0/bbot/modules/fingerprintx.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,18 @@
                 "include": "fingerprintx",
                 "dest": "#{BBOT_TOOLS}",
                 "remote_src": True,
             },
         },
     ]
 
-    def handle_batch(self, *events):
+    async def handle_batch(self, *events):
         _input = {e.data: e for e in events}
         command = ["fingerprintx", "--json"]
-        for line in self.helpers.run_live(command, input=list(_input), stderr=subprocess.DEVNULL):
+        async for line in self.helpers.run_live(command, input=list(_input), stderr=subprocess.DEVNULL):
             try:
                 j = json.loads(line)
             except Exception as e:
                 self.debug(f'Error parsing line "{line}" as JSON: {e}')
                 break
             ip = j.get("ip", "")
             host = j.get("host", ip)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1793rc0/bbot/modules/fullhunt.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,25 @@
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Query the fullhunt.io API for subdomains", "auth_required": True}
     options = {"api_key": ""}
     options_desc = {"api_key": "FullHunt API Key"}
 
     base_url = "https://fullhunt.io/api/v1"
 
-    def setup(self):
+    async def setup(self):
         self.api_key = self.config.get("api_key", "")
         self.headers = {"x-api-key": self.api_key}
-        return super().setup()
+        return await super().setup()
 
-    def ping(self):
+    async def ping(self):
         url = f"{self.base_url}/auth/status"
-        j = self.request_with_fail_count(url, headers=self.headers).json()
+        j = (await self.request_with_fail_count(url, headers=self.headers)).json()
         remaining = j["user_credits"]["remaining_credits"]
         assert remaining > 0, "No credits remaining"
 
-    def request_url(self, query):
+    async def request_url(self, query):
         url = f"{self.base_url}/domain/{self.helpers.quote(query)}/subdomains"
-        return self.request_with_fail_count(url, headers=self.headers)
+        response = await self.request_with_fail_count(url, headers=self.headers)
+        return response
 
     def parse_results(self, r, query):
         return r.json().get("hosts", [])
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1793rc0/bbot/modules/generic_ssrf.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,25 +45,25 @@
 
     def set_base_url(self, event):
         return f"{event.parsed.scheme}://{event.parsed.netloc}"
 
     def create_paths(self):
         return self.paths
 
-    def test(self, event):
+    async def test(self, event):
         base_url = self.set_base_url(event)
 
         for test_path in self.test_paths:
             subdomain_tag = self.parent_module.helpers.rand_string(4)
             test_path_prepared = test_path.replace(
                 "SSRF_CANARY", f"{subdomain_tag}.{self.parent_module.interactsh_domain}"
             )
             test_url = f"{base_url}{test_path_prepared}"
             self.parent_module.debug(f"Sending request to URL: {test_url}")
-            r = self.parent_module.helpers.curl(url=test_url)
+            r = await self.parent_module.helpers.curl(url=test_url)
             if r:
                 self.process(event, r, subdomain_tag)
 
     def process(self, event, r, subdomain_tag):
         response_token = self.parent_module.interactsh_domain.split(".")[0][::-1]
         if response_token in r:
             read_response = True
@@ -100,15 +100,15 @@
 class Generic_SSRF_POST(BaseSubmodule):
     technique_description = "Generic SSRF (POST)"
     severity = "HIGH"
 
     def set_base_url(self, event):
         return event.data
 
-    def test(self, event):
+    async def test(self, event):
         test_url = f"{event.data}"
 
         subdomain_tag = self.parent_module.helpers.rand_string(4, digits=False)
         post_data = {}
         for param in ssrf_params:
             post_data[param] = f"http://{subdomain_tag}.{self.parent_module.interactsh_domain}"
 
@@ -117,35 +117,35 @@
             k.lower(): f"http://{subdomain_tag_lower}.{self.parent_module.interactsh_domain}"
             for k, v in post_data.items()
         }
 
         post_data_list = [(subdomain_tag, post_data), (subdomain_tag_lower, post_data_lower)]
 
         for tag, pd in post_data_list:
-            r = self.parent_module.helpers.curl(url=test_url, method="POST", post_data=pd)
+            r = await self.parent_module.helpers.curl(url=test_url, method="POST", post_data=pd)
             self.process(event, r, tag)
 
 
 class Generic_XXE(BaseSubmodule):
     technique_description = "Generic XXE"
     severity = "HIGH"
     paths = None
 
-    def test(self, event):
+    async def test(self, event):
         rand_entity = self.parent_module.helpers.rand_string(4, digits=False)
         subdomain_tag = self.parent_module.helpers.rand_string(4, digits=False)
 
         post_body = f"""<?xml version="1.0" encoding="ISO-8859-1"?>
 <!DOCTYPE foo [
 <!ELEMENT foo ANY >
 <!ENTITY % {rand_entity} SYSTEM "http://{subdomain_tag}.{self.parent_module.interactsh_domain}" >
 ]>
 <foo>&{rand_entity};</foo>"""
         test_url = f"{event.parsed.scheme}://{event.parsed.netloc}/"
-        r = self.parent_module.helpers.curl(
+        r = await self.parent_module.helpers.curl(
             url=test_url, method="POST", raw_body=post_body, headers={"Content-type": "application/xml"}
         )
         if r:
             self.process(event, r, subdomain_tag)
 
 
 class generic_ssrf(BaseModule):
@@ -153,24 +153,24 @@
     produced_events = ["VULNERABILITY"]
     flags = ["active", "aggressive", "web-thorough"]
     meta = {"description": "Check for generic SSRFs"}
     in_scope_only = True
 
     deps_apt = ["curl"]
 
-    def setup(self):
+    async def setup(self):
         self.submodules = {}
         self.interactsh_subdomain_tags = {}
         self.severity = None
         self.generic_only = self.config.get("generic_only", False)
 
         if self.scan.config.get("interactsh_disable", False) == False:
             try:
                 self.interactsh_instance = self.helpers.interactsh()
-                self.interactsh_domain = self.interactsh_instance.register(callback=self.interactsh_callback)
+                self.interactsh_domain = await self.interactsh_instance.register(callback=self.interactsh_callback)
             except InteractshError as e:
                 self.warning(f"Interactsh failure: {e}")
                 return False
         else:
             self.warning(
                 "The generic_ssrf module is completely dependent on interactsh to function, but it is disabled globally. Aborting."
             )
@@ -180,20 +180,17 @@
         for m in BaseSubmodule.__subclasses__():
             if m.__name__.startswith("Generic_"):
                 self.verbose(f"Starting generic_ssrf submodule: {m.__name__}")
                 self.submodules[m.__name__] = m(self)
 
         return True
 
-    def handle_event(self, event):
-        self.test_submodules(self.submodules, event)
-
-    def test_submodules(self, submodules, event, **kwargs):
-        for s in submodules.values():
-            s.test(event, **kwargs)
+    async def handle_event(self, event):
+        for s in self.submodules.values():
+            await s.test(event)
 
     def interactsh_callback(self, r):
         full_id = r.get("full-id", None)
         if full_id:
             if "." in full_id:
                 match = self.interactsh_subdomain_tags.get(full_id.split(".")[0])
                 if not match:
@@ -213,17 +210,25 @@
                     "VULNERABILITY",
                     matched_event,
                 )
             else:
                 # this is likely caused by something trying to resolve the base domain first and can be ignored
                 self.debug("skipping result because subdomain tag was missing")
 
-    def finish(self):
-        from time import sleep
-
-        sleep(5)
+    async def cleanup(self):
+        if self.scan.config.get("interactsh_disable", False) == False:
+            try:
+                await self.interactsh_instance.deregister()
+                self.debug(
+                    f"successfully deregistered interactsh session with correlation_id {self.interactsh_instance.correlation_id}"
+                )
+            except InteractshError as e:
+                self.warning(f"Interactsh failure: {e}")
 
-        try:
-            for r in self.interactsh_instance.poll():
-                self.interactsh_callback(r)
-        except InteractshError as e:
-            self.debug(f"Error in interact.sh: {e}")
+    async def finish(self):
+        if self.scan.config.get("interactsh_disable", False) == False:
+            await self.helpers.sleep(5)
+            try:
+                for r in await self.interactsh_instance.poll():
+                    self.interactsh_callback(r)
+            except InteractshError as e:
+                self.debug(f"Error in interact.sh: {e}")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/github.py` & `bbot-1.0.5.1793rc0/bbot/modules/github.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,63 +7,67 @@
     flags = ["passive", "subdomain-enum", "safe"]
     meta = {"description": "Query Github's API for related repositories", "auth_required": True}
     options = {"api_key": ""}
     options_desc = {"api_key": "Github token"}
 
     base_url = "https://api.github.com"
 
-    def setup(self):
-        ret = super().setup()
+    async def setup(self):
+        ret = await super().setup()
         self.headers = {"Authorization": f"token {self.api_key}"}
         return ret
 
-    def ping(self):
+    async def ping(self):
         url = f"{self.base_url}/zen"
-        response = self.helpers.request(url)
+        response = await self.helpers.request(url)
         assert getattr(response, "status_code", 0) == 200
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        for repo_url, raw_urls in self.query(query).items():
+        for repo_url, raw_urls in (await self.query(query)).items():
             repo_event = self.make_event({"url": repo_url}, "CODE_REPOSITORY", source=event)
             if repo_event is None:
                 continue
             self.emit_event(repo_event)
             for raw_url in raw_urls:
                 url_event = self.make_event(raw_url, "URL_UNVERIFIED", source=repo_event, tags=["httpx-safe"])
                 if not url_event:
                     continue
                 url_event.scope_distance = repo_event.scope_distance
                 self.emit_event(url_event)
 
-    def query(self, query):
+    async def query(self, query):
         repos = {}
         url = f"{self.base_url}/search/code?per_page=100&type=Code&q={self.helpers.quote(query)}&page=" + "{page}"
-        for r in self.helpers.api_page_iter(url, headers=self.headers, json=False):
-            if r is None:
-                continue
-            status_code = getattr(r, "status_code", 0)
-            if status_code == 429:
-                "Github is rate-limiting us (HTTP status: 429)"
-                break
-            try:
-                j = r.json()
-            except Exception as e:
-                self.warning(f"Failed to decode JSON for {r.url} (HTTP status: {status_code}): {e}")
-                continue
-            items = j.get("items", [])
-            if not items:
-                break
-            for item in items:
-                htlm_url = item.get("html_url", "")
-                raw_url = self.raw_url(htlm_url)
-                repo_url = item.get("repository", {}).get("html_url", "")
-                if raw_url and repo_url:
-                    try:
-                        repos[repo_url].append(raw_url)
-                    except KeyError:
-                        repos[repo_url] = [raw_url]
+        agen = self.helpers.api_page_iter(url, headers=self.headers, json=False)
+        try:
+            async for r in agen:
+                if r is None:
+                    break
+                status_code = getattr(r, "status_code", 0)
+                if status_code == 429:
+                    "Github is rate-limiting us (HTTP status: 429)"
+                    break
+                try:
+                    j = r.json()
+                except Exception as e:
+                    self.warning(f"Failed to decode JSON for {r.url} (HTTP status: {status_code}): {e}")
+                    break
+                items = j.get("items", [])
+                if not items:
+                    break
+                for item in items:
+                    htlm_url = item.get("html_url", "")
+                    raw_url = self.raw_url(htlm_url)
+                    repo_url = item.get("repository", {}).get("html_url", "")
+                    if raw_url and repo_url:
+                        try:
+                            repos[repo_url].append(raw_url)
+                        except KeyError:
+                            repos[repo_url] = [raw_url]
+        finally:
+            agen.aclose()
         return repos
 
     @staticmethod
     def raw_url(url):
         return url.replace("https://github.com/", "https://raw.githubusercontent.com/").replace("/blob/", "/")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1793rc0/bbot/modules/gowitness.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             },
         },
     ]
     # visit up to and including the scan's configured search distance plus one
     # this is one hop further than the default
     scope_distance_modifier = 1
 
-    def setup(self):
+    async def setup(self):
         self.timeout = self.config.get("timeout", 10)
         self.threads = self.config.get("threads", 4)
         self.proxy = self.scan.config.get("http_proxy", "")
         self.resolution_x = self.config.get("resolution_x")
         self.resolution_y = self.config.get("resolution_y")
         output_path = self.config.get("output_path")
         if output_path:
@@ -109,29 +109,29 @@
             self.helpers.mkdir(self.screenshot_path)
             self.db_path.touch()
             with suppress(Exception):
                 copyfile(self.helpers.tools_dir / "gowitness", self.base_path / "gowitness")
                 copymode(self.helpers.tools_dir / "gowitness", self.base_path / "gowitness")
             self.prepped = True
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         # Ignore URLs that are redirects
         if any(t.startswith("status-30") for t in event.tags):
             return False, "URL is a redirect"
         # ignore events from self
         if event.type == "URL" and event.module == self:
             return False, "event is from self"
         return True
 
-    def handle_batch(self, *events):
+    async def handle_batch(self, *events):
         self.prep()
         stdin = "\n".join([str(e.data) for e in events])
         events = {e.data: e for e in events}
 
-        for line in self.helpers.run_live(self.command, input=stdin):
+        async for line in self.helpers.run_live(self.command, input=stdin):
             self.debug(line)
 
         # emit web screenshots
         for filename, screenshot in self.new_screenshots.items():
             url = screenshot["url"]
             final_url = screenshot["final_url"]
             filename = screenshot["filename"]
@@ -235,19 +235,17 @@
         return technologies
 
     def cur_execute(self, cur, query):
         try:
             return cur.execute(query)
         except sqlite3.OperationalError as e:
             self.warning(f"Error executing query: {query}: {e}")
-            self.trace()
             return []
 
-    def report(self):
-        with self._report_lock:
-            if self.screenshots_taken:
-                self.success(f"{len(self.screenshots_taken):,} web screenshots captured. To view:")
-                self.success(f"    - Start gowitness")
-                self.success(f"        - cd {self.base_path} && ./gowitness server")
-                self.success(f"    - Browse to http://localhost:7171")
-            else:
-                self.info(f"No web screenshots captured")
+    async def report(self):
+        if self.screenshots_taken:
+            self.success(f"{len(self.screenshots_taken):,} web screenshots captured. To view:")
+            self.success(f"    - Start gowitness")
+            self.success(f"        - cd {self.base_path} && ./gowitness server")
+            self.success(f"    - Browse to http://localhost:7171")
+        else:
+            self.info(f"No web screenshots captured")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1793rc0/bbot/modules/hackertarget.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,20 @@
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Query the hackertarget.com API for subdomains"}
 
     base_url = "https://api.hackertarget.com"
 
-    def request_url(self, query):
-        return self.request_with_fail_count(f"{self.base_url}/hostsearch/?q={self.helpers.quote(query)}")
+    async def request_url(self, query):
+        url = f"{self.base_url}/hostsearch/?q={self.helpers.quote(query)}"
+        response = await self.request_with_fail_count(url)
+        return response
 
     def parse_results(self, r, query):
         for line in r.text.splitlines():
             host = line.split(",")[0]
-            if self.helpers.validators.validate_host(host):
+            try:
+                self.helpers.validators.validate_host(host)
                 yield host
+            except ValueError:
+                self.set_error_state(host)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1793rc0/bbot/modules/host_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     flags = ["active", "aggressive", "web-thorough"]
     meta = {"description": "Try common HTTP Host header spoofing techniques"}
 
     in_scope_only = True
 
     deps_apt = ["curl"]
 
-    def setup(self):
+    async def setup(self):
         self.scanned_hosts = set()
 
         self.subdomain_tags = {}
         if self.scan.config.get("interactsh_disable", False) == False:
             try:
                 self.interactsh_instance = self.helpers.interactsh()
-                self.domain = self.interactsh_instance.register(callback=self.interactsh_callback)
+                self.domain = await self.interactsh_instance.register(callback=self.interactsh_callback)
             except InteractshError as e:
                 self.warning(f"Interactsh failure: {e}")
                 return False
         else:
             self.warning("Interactsh is disabled globally. Interaction based detections will be disabled.")
             self.domain = f"{self.rand_string(12, digits=False)}.com"
         return True
@@ -50,33 +50,34 @@
                     "FINDING",
                     matched_event,
                 )
             else:
                 # this is likely caused by something trying to resolve the base domain first and can be ignored
                 self.debug("skipping results because subdomain tag was missing")
 
-    def finish(self):
+    async def finish(self):
         if self.scan.config.get("interactsh_disable", False) == False:
+            await self.helpers.sleep(5)
             try:
-                for r in self.interactsh_instance.poll():
+                for r in await self.interactsh_instance.poll():
                     self.interactsh_callback(r)
             except InteractshError as e:
                 self.debug(f"Error in interact.sh: {e}")
 
-    def cleanup(self):
+    async def cleanup(self):
         if self.scan.config.get("interactsh_disable", False) == False:
             try:
-                self.interactsh_instance.deregister()
+                await self.interactsh_instance.deregister()
                 self.debug(
                     f"successfully deregistered interactsh session with correlation_id {self.interactsh_instance.correlation_id}"
                 )
             except InteractshError as e:
                 self.warning(f"Interactsh failure: {e}")
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         host = f"{event.parsed.scheme}://{event.parsed.netloc}/"
         host_hash = hash(host)
         if host_hash in self.scanned_hosts:
             self.debug(f"Host {host} was already scanned, exiting")
             return
         else:
             self.scanned_hosts.add(host_hash)
@@ -96,41 +97,40 @@
         domain_reflections = []
 
         # host header replacement
         technique_description = "standard"
         self.debug(f"Performing {technique_description} case")
         subdomain_tag = self.rand_string(4, digits=False)
         self.subdomain_tags[subdomain_tag] = (event, technique_description)
-        output = self.helpers.curl(
+        output = await self.helpers.curl(
             url=event.data["url"],
             headers={"Host": f"{subdomain_tag}.{self.domain}"},
             ignore_bbot_global_settings=True,
             cookies=added_cookies,
         )
         if self.domain in output:
             domain_reflections.append(technique_description)
 
         # absolute URL / Host header transposition
         technique_description = "absolute URL transposition"
         self.debug(f"Performing {technique_description} case")
         subdomain_tag = self.rand_string(4, digits=False)
         self.subdomain_tags[subdomain_tag] = (event, technique_description)
-        output = self.helpers.curl(
+        output = await self.helpers.curl(
             url=event.data["url"],
-            headers={"Host": f"{subdomain_tag}.{self.domain}"},
             path_override=event.data["url"],
             cookies=added_cookies,
         )
 
         if self.domain in output:
             domain_reflections.append(technique_description)
 
         # duplicate host header tolerance
         technique_description = "duplicate host header tolerance"
-        output = self.helpers.curl(
+        output = await self.helpers.curl(
             url=event.data["url"],
             # Sending a blank HOST first as a hack to trick curl. This makes it no longer an "internal header", thereby allowing for duplicates
             # The fact that it's accepting two host headers is rare enough to note on its own, and not too noisy. Having the 3rd header be an interactsh would result in false negatives for the slightly less interesting cases.
             headers={"Host": ["", str(event.host), str(event.host)]},
             cookies=added_cookies,
             head_mode=True,
         )
@@ -163,15 +163,15 @@
             "X-HTTP-Host-Override",
             "Forwarded",
         ]
         override_headers = {}
         for oh in override_headers_list:
             override_headers[oh] = f"{subdomain_tag}.{self.domain}"
 
-        output = self.helpers.curl(
+        output = await self.helpers.curl(
             url=event.data["url"],
             headers=override_headers,
             cookies=added_cookies,
         )
         if self.domain in output:
             domain_reflections.append(technique_description)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1793rc0/bbot/modules/internal/speculate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,128 @@
-import json
-import subprocess
-from bbot.modules.base import BaseModule
+import random
+import ipaddress
 
+from bbot.modules.internal.base import BaseInternalModule
 
-class httpx(BaseModule):
-    watched_events = ["OPEN_TCP_PORT", "URL_UNVERIFIED", "URL"]
-    produced_events = ["URL", "HTTP_RESPONSE"]
-    flags = ["active", "safe", "web-basic", "web-thorough", "social-enum", "subdomain-enum", "cloud-enum"]
-    meta = {"description": "Visit webpages. Many other modules rely on httpx"}
 
-    batch_size = 500
-    options = {"threads": 50, "in_scope_only": True, "version": "1.2.5", "max_response_size": 5242880}
-    options_desc = {
-        "threads": "Number of httpx threads to use",
-        "in_scope_only": "Only visit web resources that are in scope.",
-        "version": "httpx version",
-        "max_response_size": "Max response size in bytes",
-    }
-    deps_ansible = [
-        {
-            "name": "Download httpx",
-            "unarchive": {
-                "src": "https://github.com/projectdiscovery/httpx/releases/download/v#{BBOT_MODULES_HTTPX_VERSION}/httpx_#{BBOT_MODULES_HTTPX_VERSION}_#{BBOT_OS}_#{BBOT_CPU_ARCH}.zip",
-                "include": "httpx",
-                "dest": "#{BBOT_TOOLS}",
-                "remote_src": True,
-            },
-        }
+class speculate(BaseInternalModule):
+    """
+    Bridge the gap between ranges and ips, or ips and open ports
+    in situations where e.g. a port scanner isn't enabled
+    """
+
+    watched_events = [
+        "IP_RANGE",
+        "URL",
+        "URL_UNVERIFIED",
+        "DNS_NAME",
+        "DNS_NAME_UNRESOLVED",
+        "IP_ADDRESS",
+        "HTTP_RESPONSE",
+        "STORAGE_BUCKET",
     ]
+    produced_events = ["DNS_NAME", "OPEN_TCP_PORT", "IP_ADDRESS", "FINDING"]
+    flags = ["passive"]
+    meta = {"description": "Derive certain event types from others by common sense"}
 
+    options = {"max_hosts": 65536, "ports": [80, 443]}
+    options_desc = {
+        "max_hosts": "Max number of IP_RANGE hosts to convert into IP_ADDRESS events",
+        "ports": "The set of ports to speculate on",
+    }
+    max_event_handlers = 5
     scope_distance_modifier = 1
-    _priority = 2
+    _scope_shepherding = False
+    _priority = 4
 
-    def setup(self):
-        self.threads = self.config.get("threads", 50)
-        self.timeout = self.scan.config.get("httpx_timeout", 5)
-        self.retries = self.scan.config.get("httpx_retries", 1)
-        self.max_response_size = self.config.get("max_response_size", 5242880)
-        self.visited = set()
-        return True
+    async def setup(self):
+        self.open_port_consumers = any(["OPEN_TCP_PORT" in m.watched_events for m in self.scan.modules.values()])
+        self.portscanner_enabled = any(["portscan" in m.flags for m in self.scan.modules.values()])
+        self.range_to_ip = True
+        self.dns_resolution = self.scan.config.get("dns_resolution", True)
+
+        self.ports = self.config.get("ports", [80, 443])
+        if isinstance(self.ports, int):
+            self.ports = [self.ports]
+        if not self.portscanner_enabled:
+            self.info(f"No portscanner enabled. Assuming open ports: {', '.join(str(x) for x in self.ports)}")
+
+        target_len = len(self.scan.target)
+        if target_len > self.config.get("max_hosts", 65536):
+            if not self.portscanner_enabled:
+                self.hugewarning(
+                    f"Selected target ({target_len:,} hosts) is too large, skipping IP_RANGE --> IP_ADDRESS speculation"
+                )
+                self.hugewarning(f"Enabling a port scanner (naabu or masscan) module is highly recommended")
+            self.range_to_ip = False
 
-    def filter_event(self, event):
-        if "_wildcard" in str(event.host).split("."):
-            return False, "event is wildcard"
-
-        if "unresolved" in event.tags:
-            return False, "event is unresolved"
-
-        if event.module == self:
-            return False, "event is from self"
-
-        if "spider-danger" in event.tags:
-            return False, "event has spider danger"
-
-        # scope filtering
-        in_scope_only = self.config.get("in_scope_only", True)
-        safe_to_visit = "httpx-safe" in event.tags
-        if not safe_to_visit and (in_scope_only and not self.scan.in_scope(event)):
-            return False, "event is not in scope"
-        # reject base URLs to avoid visiting a resource twice
-        # note: speculate makes open ports from
         return True
 
-    def handle_batch(self, *events):
-        stdin = {}
-        for e in events:
-            url_hash = None
-            if e.type.startswith("URL"):
-                # we NEED the port, otherwise httpx will try HTTPS even for HTTP URLs
-                url = e.with_port().geturl()
-                if e.parsed.path == "/":
-                    url_hash = hash((e.host, e.port))
-            else:
-                url = str(e.data)
-                url_hash = hash((e.host, e.port))
-
-            if url_hash not in self.visited:
-                stdin[url] = e
-                if url_hash is not None:
-                    self.visited.add(url_hash)
-
-        if not stdin:
-            return
-
-        command = [
-            "httpx",
-            "-silent",
-            "-json",
-            "-include-response",
-            "-threads",
-            self.threads,
-            "-timeout",
-            self.timeout,
-            "-retries",
-            self.retries,
-            "-header",
-            f"User-Agent: {self.scan.useragent}",
-            "-response-size-to-read",
-            f"{self.max_response_size}",
-            # "-r",
-            # self.helpers.resolver_file,
-        ]
-        for hk, hv in self.scan.config.get("http_headers", {}).items():
-            command += ["-header", f"{hk}: {hv}"]
-        proxy = self.scan.config.get("http_proxy", "")
-        if proxy:
-            command += ["-http-proxy", proxy]
-        for line in self.helpers.run_live(command, input=list(stdin), stderr=subprocess.DEVNULL):
-            try:
-                j = json.loads(line)
-            except json.decoder.JSONDecodeError:
-                self.debug(f"Failed to decode line: {line}")
-                continue
-
-            url = j.get("url", "")
-            status_code = int(j.get("status_code", 0))
-            if status_code == 0:
-                self.debug(f'No HTTP status code for "{url}"')
-                continue
-
-            source_event = stdin.get(j.get("input", ""), None)
-
-            if source_event is None:
-                self.warning(f"Unable to correlate source event from: {line}")
-                continue
-
-            # discard 404s from unverified URLs
-            if source_event.type == "URL_UNVERIFIED" and status_code in (404,):
-                self.debug(f'Discarding 404 from "{url}"')
-                continue
-
-            # main URL
-            httpx_ip = j.get("host", "unknown")
-            tags = [f"status-{status_code}", f"ip-{httpx_ip}"]
-            title = self.helpers.tagify(j.get("title", ""))
-            if title:
-                tags.append(f"http-title-{title}")
-            url_event = self.make_event(url, "URL", source_event, tags=tags)
-            if url_event:
-                if url_event != source_event:
+    async def handle_event(self, event):
+        # generate individual IP addresses from IP range
+        if event.type == "IP_RANGE" and self.range_to_ip:
+            net = ipaddress.ip_network(event.data)
+            ips = list(net)
+            random.shuffle(ips)
+            for ip in ips:
+                self.emit_event(ip, "IP_ADDRESS", source=event, internal=True)
+
+        # parent domains
+        if event.type == "DNS_NAME":
+            parent = self.helpers.parent_domain(event.data)
+            if parent != event.data:
+                self.emit_event(parent, "DNS_NAME", source=event, internal=True)
+
+        # generate open ports
+        emit_open_ports = self.open_port_consumers and not self.portscanner_enabled
+        # from URLs
+        if event.type == "URL" or (event.type == "URL_UNVERIFIED" and emit_open_ports):
+            if event.host and event.port not in self.ports:
+                self.emit_event(
+                    self.helpers.make_netloc(event.host, event.port),
+                    "OPEN_TCP_PORT",
+                    source=event,
+                    internal=True,
+                    quick=(event.type == "URL"),
+                )
+
+        # generate sub-directory URLS from URLS
+        if event.type == "URL":
+            url_parents = self.helpers.url_parents(event.data)
+            for up in url_parents:
+                url_event = self.make_event(f"{up}/", "URL_UNVERIFIED", source=event)
+                if url_event is not None:
+                    # inherit web spider distance from parent (don't increment)
+                    source_web_spider_distance = getattr(event, "web_spider_distance", 0)
+                    url_event.web_spider_distance = source_web_spider_distance
                     self.emit_event(url_event)
-                else:
-                    url_event._resolved.set()
-                # HTTP response
-                self.emit_event(j, "HTTP_RESPONSE", url_event, internal=True)
-
-    def cleanup(self):
-        resume_file = self.helpers.current_dir / "resume.cfg"
-        resume_file.unlink(missing_ok=True)
+
+        # from hosts
+        if emit_open_ports:
+            # don't act on unresolved DNS_NAMEs
+            usable_dns = False
+            if event.type == "DNS_NAME":
+                if (not self.dns_resolution) or ("a-record" in event.tags or "aaaa-record" in event.tags):
+                    usable_dns = True
+
+            if event.type == "IP_ADDRESS" or usable_dns:
+                for port in self.ports:
+                    self.emit_event(
+                        self.helpers.make_netloc(event.data, port),
+                        "OPEN_TCP_PORT",
+                        source=event,
+                        internal=True,
+                        quick=True,
+                    )
+
+        # storage buckets etc.
+        self.helpers.cloud.speculate(event)
+
+    async def filter_event(self, event):
+        # don't accept IP_RANGE --> IP_ADDRESS events from self
+        if str(event.module) == "speculate":
+            if not (event.type == "IP_ADDRESS" and str(getattr(event.source, "type")) == "IP_RANGE"):
+                return False
+        # don't accept errored DNS_NAMEs
+        if any(t in event.tags for t in ("unresolved", "a-error", "aaaa-error")):
+            return False
+        return True
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1793rc0/bbot/modules/hunt.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                     i = url.split("?")[1].split("&")
                 for x in i:
                     s = x.split("=")[0]
 
                     self.debug(f"FOUND PARAM ({s}) IN A TAG GET PARAMS")
                     yield s
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         body = event.data.get("body", "")
         for p in self.extract_params(body):
             for k in hunt_param_dict.keys():
                 if p.lower() in hunt_param_dict[k]:
                     description = f"Found potential {k.upper()} parameter [{p}]"
                     data = {"host": str(event.host), "description": description}
                     url = event.data.get("url", "")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1793rc0/bbot/modules/hunterio.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,46 +6,48 @@
     produced_events = ["EMAIL_ADDRESS", "DNS_NAME", "URL_UNVERIFIED"]
     flags = ["passive", "email-enum", "subdomain-enum", "safe"]
     meta = {"description": "Query hunter.io for emails", "auth_required": True}
     options = {"api_key": ""}
     options_desc = {"api_key": "Hunter.IO API key"}
 
     base_url = "https://api.hunter.io/v2"
+    limit = 100
 
-    def setup(self):
-        self.limit = 100
-        return super().setup()
-
-    def ping(self):
-        r = self.helpers.request(f"{self.base_url}/account?api_key={self.api_key}")
+    async def ping(self):
+        url = f"{self.base_url}/account?api_key={self.api_key}"
+        r = await self.helpers.request(url)
         resp_content = getattr(r, "text", "")
         assert getattr(r, "status_code", 0) == 200, resp_content
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        for entry in self.query(query):
+        for entry in await self.query(query):
             email = entry.get("value", "")
             sources = entry.get("sources", [])
             if email:
                 email_event = self.make_event(email, "EMAIL_ADDRESS", event)
                 if email_event:
                     self.emit_event(email_event)
                     for source in sources:
                         domain = source.get("domain", "")
                         if domain:
                             self.emit_event(domain, "DNS_NAME", email_event)
                         url = source.get("uri", "")
                         if url:
                             self.emit_event(url, "URL_UNVERIFIED", email_event)
 
-    def query(self, query):
+    async def query(self, query):
         emails = []
         url = (
             f"{self.base_url}/domain-search?domain={query}&api_key={self.api_key}"
             + "&limit={page_size}&offset={offset}"
         )
-        for j in self.helpers.api_page_iter(url, page_size=self.limit):
-            new_emails = j.get("data", {}).get("emails", [])
-            if not new_emails:
-                break
-            emails += new_emails
+        agen = self.helpers.api_page_iter(url, page_size=self.limit)
+        try:
+            async for j in agen:
+                new_emails = j.get("data", {}).get("emails", [])
+                if not new_emails:
+                    break
+                emails += new_emails
+        finally:
+            agen.aclose()
         return emails
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1793rc0/bbot/modules/iis_shortnames.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,139 +20,139 @@
         "detect_only": "Only detect the vulnerability and do not run the shortname scanner",
         "max_node_count": "Limit how many nodes to attempt to resolve on any given recursion branch",
     }
     in_scope_only = True
 
     max_event_handlers = 8
 
-    def detect(self, target):
+    async def detect(self, target):
         technique = None
         detections = []
         random_string = self.helpers.rand_string(8)
         control_url = f"{target}{random_string}*~1*/a.aspx"
         test_url = f"{target}*~1*/a.aspx"
 
         for method in ["GET", "POST", "OPTIONS", "DEBUG", "HEAD", "TRACE"]:
-            control = self.helpers.request(method=method, url=control_url, allow_redirects=False, timeout=10)
-            test = self.helpers.request(method=method, url=test_url, allow_redirects=False, timeout=10)
+            control = await self.helpers.request(method=method, url=control_url, allow_redirects=False, timeout=10)
+            test = await self.helpers.request(method=method, url=test_url, allow_redirects=False, timeout=10)
             if (control != None) and (test != None):
                 if control.status_code != test.status_code:
                     technique = f"{str(control.status_code)}/{str(test.status_code)} HTTP Code"
                     detections.append((method, test.status_code, technique))
 
                 elif ("Error Code</th><td>0x80070002" in control.text) and (
                     "Error Code</th><td>0x00000000" in test.text
                 ):
                     detections.append((method, 0, technique))
                     technique = "HTTP Body Error Message"
         return detections
 
-    def setup(self):
+    async def setup(self):
         self.scanned_tracker_lock = Lock()
         self.scanned_tracker = set()
         return True
 
     @staticmethod
     def normalize_url(url):
         return str(url.rstrip("/") + "/").lower()
 
-    def directory_confirm(self, target, method, url_hint, affirmative_status_code):
+    async def directory_confirm(self, target, method, url_hint, affirmative_status_code):
         payload = encode_all(f"{url_hint}")
         url = f"{target}{payload}"
-        directory_confirm_result = self.helpers.request(
+        directory_confirm_result = await self.helpers.request(
             method=method, url=url, allow_redirects=False, retries=2, timeout=10
         )
 
         if directory_confirm_result.status_code == affirmative_status_code:
             return True
         else:
             return False
 
-    def duplicate_check(self, target, method, url_hint, affirmative_status_code):
+    async def duplicate_check(self, target, method, url_hint, affirmative_status_code):
         duplicates = []
         count = 2
         base_hint = re.sub(r"~\d", "", url_hint)
-        suffix = "\\a.aspx"
+        suffix = "/a.aspx"
 
         while 1:
             payload = encode_all(f"{base_hint}~{str(count)}*")
             url = f"{target}{payload}{suffix}"
 
-            duplicate_check_results = self.helpers.request(
+            duplicate_check_results = await self.helpers.request(
                 method=method, url=url, allow_redirects=False, retries=2, timeout=10
             )
             if duplicate_check_results.status_code != affirmative_status_code:
                 break
             else:
                 duplicates.append(f"{base_hint}~{str(count)}")
                 count += 1
 
             if count > 5:
                 self.warning("Found more than 5 files with the same shortname. Will stop further duplicate checking.")
                 break
 
         return duplicates
 
-    def threaded_request(self, method, url, affirmative_status_code):
-        r = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2, timeout=10)
+    async def threaded_request(self, method, url, affirmative_status_code, c):
+        r = await self.helpers.request(method=method, url=url, allow_redirects=False, retries=2, timeout=10)
         if r is not None:
             if r.status_code == affirmative_status_code:
-                return True
+                return True, c
+        return None, c
 
-    def solve_shortname_recursive(
+    async def solve_shortname_recursive(
         self, method, target, prefix, affirmative_status_code, extension_mode=False, node_count=0
     ):
         url_hint_list = []
         found_results = False
 
-        futures = {}
+        tasks = []
         for c in valid_chars:
-            suffix = "\\a.aspx"
+            suffix = "/a.aspx"
             wildcard = "*" if extension_mode else "*~1*"
             payload = encode_all(f"{prefix}{c}{wildcard}")
             url = f"{target}{payload}{suffix}"
-            future = self.submit_task(self.threaded_request, method, url, affirmative_status_code)
-            futures[future] = c
+            task = self.helpers.create_task(self.threaded_request(method, url, affirmative_status_code, c))
+            tasks.append(task)
 
-        for future in self.helpers.as_completed(futures):
-            c = futures[future]
-            result = future.result()
+        for task in self.helpers.as_completed(tasks):
+            result, c = await task
             if result:
                 found_results = True
                 node_count += 1
                 self.verbose(f"node_count: {str(node_count)} for node: {target}")
                 if node_count > self.config.get("max_node_count"):
                     self.warning(
                         f"iis_shortnames: max_node_count ({str(self.config.get('max_node_count'))}) exceeded for node: {target}. Affected branch will be terminated."
                     )
                     return url_hint_list
 
                 # check to make sure the file isn't shorter than 6 characters
                 wildcard = "~1*"
                 payload = encode_all(f"{prefix}{c}{wildcard}")
                 url = f"{target}{payload}{suffix}"
-                r = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2, timeout=10)
+                r = await self.helpers.request(method=method, url=url, allow_redirects=False, retries=2, timeout=10)
                 if r is not None:
                     if r.status_code == affirmative_status_code:
                         url_hint_list.append(f"{prefix}{c}")
 
-                url_hint_list += self.solve_shortname_recursive(
+                url_hint_list += await self.solve_shortname_recursive(
                     method, target, f"{prefix}{c}", affirmative_status_code, extension_mode, node_count=node_count
                 )
         if len(prefix) > 0 and found_results == False:
             url_hint_list.append(f"{prefix}")
             self.verbose(f"Found new (possibly partial) URL_HINT: {prefix} from node {target}")
         return url_hint_list
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         normalized_url = self.normalize_url(event.data)
         with self.scanned_tracker_lock:
             self.scanned_tracker.add(normalized_url)
 
-        detections = self.detect(normalized_url)
+        detections = await self.detect(normalized_url)
 
         technique_strings = []
         if detections:
             for detection in detections:
                 method, affirmative_status_code, technique = detection
                 technique_strings.append(f"{method} ({technique})")
 
@@ -167,40 +167,39 @@
                     method, affirmative_status_code, technique = detection
                     valid_method_confirmed = False
 
                     if valid_method_confirmed:
                         break
 
                     file_name_hints = list(
-                        set(self.solve_shortname_recursive(method, normalized_url, "", affirmative_status_code))
+                        set(await self.solve_shortname_recursive(method, normalized_url, "", affirmative_status_code))
                     )
                     if len(file_name_hints) == 0:
                         continue
                     else:
                         valid_method_confirmed = True
 
                     file_name_hints = [f"{x}~1" for x in file_name_hints]
                     url_hint_list = []
 
                     file_name_hints_dedupe = file_name_hints[:]
 
                     for x in file_name_hints_dedupe:
-                        duplicates = self.duplicate_check(normalized_url, method, x, affirmative_status_code)
+                        duplicates = await self.duplicate_check(normalized_url, method, x, affirmative_status_code)
                         if duplicates:
                             file_name_hints += duplicates
 
                     # check for the case of a folder and file with the same filename
-
                     for d in file_name_hints:
-                        if self.directory_confirm(normalized_url, method, d, affirmative_status_code):
+                        if await self.directory_confirm(normalized_url, method, d, affirmative_status_code):
                             self.verbose(f"Confirmed Directory URL_HINT: {d} from node {normalized_url}")
                             url_hint_list.append(d)
 
                     for y in file_name_hints:
-                        file_name_extension_hints = self.solve_shortname_recursive(
+                        file_name_extension_hints = await self.solve_shortname_recursive(
                             method, normalized_url, f"{y}.", affirmative_status_code, extension_mode=True
                         )
                         for z in file_name_extension_hints:
                             if z.endswith("."):
                                 z = z.rstrip(".")
                             self.verbose(f"Found new file URL_HINT: {z} from node {normalized_url}")
                             url_hint_list.append(z)
@@ -208,14 +207,14 @@
                     for url_hint in url_hint_list:
                         if "." in url_hint:
                             hint_type = "shortname-file"
                         else:
                             hint_type = "shortname-directory"
                         self.emit_event(f"{normalized_url}/{url_hint}", "URL_HINT", event, tags=[hint_type])
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if "dir" in event.tags:
             with self.scanned_tracker_lock:
                 if self.normalize_url(event.data) not in self.scanned_tracker:
                     return True
                 return False
         return False
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1793rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1793rc0/bbot/modules/internal/excavate.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 
     def __init__(self, excavate):
         self.excavate = excavate
         self.compiled_regexes = {}
         for rname, r in self.regexes.items():
             self.compiled_regexes[rname] = re.compile(r)
 
-    def search(self, content, event, **kwargs):
+    async def search(self, content, event, **kwargs):
         results = set()
-        for result, name in self._search(content, event, **kwargs):
+        async for result, name in self._search(content, event, **kwargs):
             results.add(result)
         for result in results:
             self.report(result, name, event, **kwargs)
 
-    def _search(self, content, event, **kwargs):
+    async def _search(self, content, event, **kwargs):
         for name, regex in self.compiled_regexes.items():
+            # yield to event loop
+            await self.excavate.helpers.sleep(0)
             for result in regex.findall(content):
                 yield result, name
 
     def report(self, result, name, event):
         pass
 
 
@@ -62,32 +64,34 @@
 
     prefix_blacklist = ["javascript:", "mailto:", "tel:", "data:", "vbscript:", "about:", "file:"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.web_spider_links_per_page = self.excavate.scan.config.get("web_spider_links_per_page", 20)
 
-    def search(self, content, event, **kwargs):
+    async def search(self, content, event, **kwargs):
         result_hashes = set()
         results = []
-        for result in self._search(content, event, **kwargs):
+        async for result in self._search(content, event, **kwargs):
             result_hash = hash(result)
             if result_hash not in result_hashes:
                 result_hashes.add(result_hash)
                 results.append(result)
         for i, (result, name) in enumerate(results):
             new_kwargs = dict(kwargs)
             if i > self.web_spider_links_per_page:
                 # self.excavate.critical(f"SPIDER DANGER: {result}")
                 new_kwargs["exceeded_max_links"] = True
             self.report(result, name, event, **new_kwargs)
 
-    def _search(self, content, event, **kwargs):
+    async def _search(self, content, event, **kwargs):
         parsed = getattr(event, "parsed", None)
         for name, regex in self.compiled_regexes.items():
+            # yield to event loop
+            await self.excavate.helpers.sleep(0)
             for result in regex.findall(content):
                 if name == "fullurl":
                     protocol, other = result
                     result = f"{protocol}://{other}"
 
                 elif name in ("a-tag", "script-tag") and parsed:
                     path = html.unescape(result[1])
@@ -272,15 +276,15 @@
         "possible_creds_var": r"(?:password|passwd|pwd|pass)\s*=+\s*['\"][^\s'\"]{1,60}['\"]",
     }
 
     def report(self, result, name, event, **kwargs):
         # ensure that basic auth matches aren't false positives
         if name == "authorization_basic":
             try:
-                b64test = base64.b64decode(result.split(" ")[1].encode())
+                b64test = base64.b64decode(result.split(" ", 1)[-1].encode())
                 if b":" not in b64test:
                     return
             except (base64.binascii.Error, UnicodeDecodeError):
                 return
 
         self.excavate.debug(f"Found Possible Secret in Javascript [{result}]")
         description = f"Possible secret in JS [{result}] Signature [{name}]"
@@ -293,68 +297,69 @@
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["URL_UNVERIFIED"]
     flags = ["passive"]
     meta = {"description": "Passively extract juicy tidbits from scan data"}
 
     scope_distance_modifier = None
 
-    deps_pip = ["pyjwt~=2.6.0"]
-
-    def setup(self):
+    async def setup(self):
         self.hostname = HostnameExtractor(self)
         self.url = URLExtractor(self)
         self.email = EmailExtractor(self)
         self.error_extractor = ErrorExtractor(self)
         self.jwt = JWTExtractor(self)
         self.javascript = JavascriptExtractor(self)
         self.serialization = SerializationExtractor(self)
         self.functionality = FunctionalityExtractor(self)
         self.max_redirects = self.scan.config.get("http_max_redirects", 5)
 
         return True
 
-    def search(self, source, extractors, event, **kwargs):
+    async def search(self, source, extractors, event, **kwargs):
         for e in extractors:
-            e.search(source, event, **kwargs)
+            await e.search(source, event, **kwargs)
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         data = event.data
 
         # HTTP_RESPONSE is a special case
         if event.type == "HTTP_RESPONSE":
             # handle redirects
             web_spider_distance = getattr(event, "web_spider_distance", 0)
             num_redirects = max(getattr(event, "num_redirects", 0), web_spider_distance)
             location = event.data.get("location", "")
             host = event.host
+            # if it's a redirect
             if location:
+                # get the url scheme
                 scheme = self.helpers.is_uri(location, return_scheme=True)
+                # if there's no scheme (i.e. it's a relative redirect)
                 if not scheme:
-                    location_parsed = event.parsed._replace(path=location)
-                    host, _ = self.helpers.split_host_port(location_parsed.netloc)
-                    location = location_parsed.geturl()
+                    # then join the location with the current url
+                    location = urljoin(event.parsed.geturl(), location)
                     scheme = self.helpers.is_uri(location, return_scheme=True)
                 if scheme in ("http", "https"):
                     if num_redirects <= self.max_redirects:
                         url_event = self.make_event(location, "URL_UNVERIFIED", event)
-                        # inherit web spider distance from parent (don't increment)
-                        source_web_spider_distance = getattr(event, "web_spider_distance", 0)
-                        url_event.web_spider_distance = source_web_spider_distance
-                        self.emit_event(url_event)
+                        if url_event is not None:
+                            # inherit web spider distance from parent (don't increment)
+                            source_web_spider_distance = getattr(event, "web_spider_distance", 0)
+                            url_event.web_spider_distance = source_web_spider_distance
+                            self.emit_event(url_event)
                     else:
                         self.verbose(f"Exceeded max HTTP redirects ({self.max_redirects}): {location}")
                 elif scheme:
                     # we ran into a scheme that's not HTTP or HTTPS
                     data = {"host": host, "description": f"Non-standard URI scheme: {scheme}://", "url": location}
                     self.emit_event(data, "FINDING", event)
 
             body = self.helpers.recursive_decode(event.data.get("body", ""))
             # Cloud extractors
             self.helpers.cloud.excavate(event, body)
-            self.search(
+            await self.search(
                 body,
                 [
                     self.hostname,
                     self.url,
                     self.email,
                     self.error_extractor,
                     self.jwt,
@@ -363,20 +368,20 @@
                     self.functionality,
                 ],
                 event,
                 consider_spider_danger=True,
             )
 
             headers = self.helpers.recursive_decode(event.data.get("raw_header", ""))
-            self.search(
+            await self.search(
                 headers,
                 [self.hostname, self.url, self.email, self.error_extractor, self.jwt, self.serialization],
                 event,
                 consider_spider_danger=False,
             )
 
         else:
-            self.search(
+            await self.search(
                 str(data),
                 [self.hostname, self.url, self.email, self.error_extractor, self.jwt, self.serialization],
                 event,
             )
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1793rc0/bbot/modules/ntlm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,160 @@
-import random
-import ipaddress
-
-from bbot.modules.internal.base import BaseInternalModule
-
-
-class speculate(BaseInternalModule):
-    """
-    Bridge the gap between ranges and ips, or ips and open ports
-    in situations where e.g. a port scanner isn't enabled
-    """
-
-    watched_events = ["IP_RANGE", "URL", "URL_UNVERIFIED", "DNS_NAME", "IP_ADDRESS", "HTTP_RESPONSE", "STORAGE_BUCKET"]
-    produced_events = ["DNS_NAME", "OPEN_TCP_PORT", "IP_ADDRESS", "FINDING"]
-    flags = ["passive"]
-    meta = {"description": "Derive certain event types from others by common sense"}
-
-    options = {"max_hosts": 65536, "ports": [80, 443]}
-    options_desc = {
-        "max_hosts": "Max number of IP_RANGE hosts to convert into IP_ADDRESS events",
-        "ports": "The set of ports to speculate on",
-    }
-    max_event_handlers = 5
-    scope_distance_modifier = 1
-    _scope_shepherding = False
-    _priority = 4
-
-    def setup(self):
-        self.open_port_consumers = any(["OPEN_TCP_PORT" in m.watched_events for m in self.scan.modules.values()])
-        self.portscanner_enabled = any(["portscan" in m.flags for m in self.scan.modules.values()])
-        self.range_to_ip = True
-
-        self.ports = self.config.get("ports", [80, 443])
-        if isinstance(self.ports, int):
-            self.ports = [self.ports]
-        if not self.portscanner_enabled:
-            self.info(f"No portscanner enabled. Assuming open ports: {', '.join(str(x) for x in self.ports)}")
-
-        target_len = len(self.scan.target)
-        if target_len > self.config.get("max_hosts", 65536):
-            if not self.portscanner_enabled:
-                self.hugewarning(
-                    f"Selected target ({target_len:,} hosts) is too large, skipping IP_RANGE --> IP_ADDRESS speculation"
-                )
-                self.hugewarning(f"Enabling a port scanner (naabu or masscan) module is highly recommended")
-            self.range_to_ip = False
+from bbot.modules.base import BaseModule
+from bbot.core.errors import NTLMError, RequestError, ReadTimeout
 
+ntlm_discovery_endpoints = [
+    "",
+    "autodiscover/autodiscover.xml",
+    "ecp/",
+    "ews/",
+    "ews/exchange.asmx",
+    "exchange/",
+    "exchweb/",
+    "oab/",
+    "owa/",
+    "_windows/default.aspx?ReturnUrl=/",
+    "abs/",
+    "adfs/ls/wia",
+    "adfs/services/trust/2005/windowstransport",
+    "aspnet_client/",
+    "autodiscover/",
+    "autoupdate/",
+    "certenroll/",
+    "certprov/",
+    "certsrv/",
+    "conf/",
+    "debug/",
+    "deviceupdatefiles_ext/",
+    "deviceupdatefiles_int/",
+    "dialin/",
+    "etc/",
+    "groupexpansion/",
+    "hybridconfig/",
+    "iwa/authenticated.aspx",
+    "iwa/iwa_test.aspx",
+    "mcx/",
+    "mcx/mcxservice.svc",
+    "meet/",
+    "meeting/",
+    "microsoft-server-activesync/",
+    "ocsp/",
+    "persistentchat/",
+    "phoneconferencing/",
+    "powershell/",
+    "public/",
+    "reach/sip.svc",
+    "remoteDesktopGateway/",
+    "requesthandler/",
+    "requesthandlerext/",
+    "rgs/",
+    "rgsclients/",
+    "rpc/",
+    "rpcwithcert/",
+    "scheduler/",
+    "ucwa/",
+    "unifiedmessaging/",
+    "webticket/",
+    "webticket/webticketservice.svc",
+]
+
+NTLM_test_header = {"Authorization": "NTLM TlRMTVNTUAABAAAAl4II4gAAAAAAAAAAAAAAAAAAAAAKAGFKAAAADw=="}
+
+
+class ntlm(BaseModule):
+    watched_events = ["URL", "HTTP_RESPONSE"]
+    produced_events = ["FINDING", "DNS_NAME"]
+    flags = ["active", "safe", "web-basic", "web-thorough"]
+    meta = {"description": "Watch for HTTP endpoints that support NTLM authentication"}
+    options = {"try_all": False}
+    options_desc = {"try_all": "Try every NTLM endpoint"}
+
+    in_scope_only = True
+
+    async def setup(self):
+        self.processed = set()
+        self.found = set()
+        self.try_all = self.config.get("try_all", False)
         return True
 
-    def handle_event(self, event):
-        # generate individual IP addresses from IP range
-        if event.type == "IP_RANGE" and self.range_to_ip:
-            net = ipaddress.ip_network(event.data)
-            ips = list(net)
-            random.shuffle(ips)
-            for ip in ips:
-                self.emit_event(ip, "IP_ADDRESS", source=event, internal=True)
-
-        # parent domains
-        if event.type == "DNS_NAME":
-            parent = self.helpers.parent_domain(event.data)
-            if parent != event.data:
-                self.emit_event(parent, "DNS_NAME", source=event, internal=True)
-
-        # generate open ports
-        emit_open_ports = self.open_port_consumers and not self.portscanner_enabled
-        # from URLs
-        if event.type == "URL" or (event.type == "URL_UNVERIFIED" and emit_open_ports):
-            if event.host and event.port not in self.ports:
+    async def handle_event(self, event):
+        found_hash = hash(f"{event.host}:{event.port}")
+        if found_hash not in self.found:
+            result, request_url = await self.handle_url(event)
+            if result and request_url:
+                self.found.add(found_hash)
                 self.emit_event(
-                    self.helpers.make_netloc(event.host, event.port),
-                    "OPEN_TCP_PORT",
+                    {
+                        "host": str(event.host),
+                        "url": request_url,
+                        "description": f"NTLM AUTH: {result}",
+                    },
+                    "FINDING",
                     source=event,
-                    internal=True,
-                    quick=(event.type == "URL"),
                 )
+                fqdn = result.get("FQDN", "")
+                if fqdn:
+                    self.emit_event(fqdn, "DNS_NAME", source=event)
+
+    async def filter_event(self, event):
+        if self.try_all:
+            return True
+        if event.type == "HTTP_RESPONSE":
+            if "www-authenticate" in event.data["header-dict"]:
+                header_value = event.data["header-dict"]["www-authenticate"].lower()
+                if "ntlm" in header_value or "negotiate" in header_value:
+                    return True
+        return False
 
-        # generate sub-directory URLS from URLS
+    async def handle_url(self, event):
         if event.type == "URL":
-            url_parents = self.helpers.url_parents(event.data)
-            for up in url_parents:
-                url_event = self.make_event(f"{up}/", "URL_UNVERIFIED", source=event)
-                # inherit web spider distance from parent (don't increment)
-                source_web_spider_distance = getattr(event, "web_spider_distance", 0)
-                url_event.web_spider_distance = source_web_spider_distance
-                self.emit_event(url_event)
-
-        # from hosts
-        if emit_open_ports:
-            # don't act on unresolved DNS_NAMEs
-
-            usable_dns = False
-            if event.type == "DNS_NAME":
-                if "a-record" in event.tags or "aaaa-record" in event.tags:
-                    usable_dns = True
-
-            if event.type == "IP_ADDRESS" or usable_dns:
-                for port in self.ports:
-                    self.emit_event(
-                        self.helpers.make_netloc(event.data, port),
-                        "OPEN_TCP_PORT",
-                        source=event,
-                        internal=True,
-                        quick=True,
-                    )
-
-    def filter_event(self, event):
-        # don't accept IP_RANGE --> IP_ADDRESS events from self
-        if str(event.module) == "speculate":
-            if not (event.type == "IP_ADDRESS" and str(getattr(event.source, "type")) == "IP_RANGE"):
-                return False
-        # don't accept errored DNS_NAMEs
-        if any(t in event.tags for t in ("unresolved", "a-error", "aaaa-error")):
-            return False
-        return True
+            urls = {
+                event.data,
+            }
+        else:
+            urls = {
+                event.data["url"],
+            }
+        if self.try_all:
+            for endpoint in ntlm_discovery_endpoints:
+                urls.add(f"{event.parsed.scheme}://{event.parsed.netloc}/{endpoint}")
+
+        tasks = []
+        for url in urls:
+            url_hash = hash(url)
+            if url_hash in self.processed:
+                continue
+            self.processed.add(url_hash)
+            task = self.helpers.create_task(self.check_ntlm(url))
+            tasks.append(task)
+
+        for task in self.helpers.as_completed(tasks):
+            try:
+                result, url = await task
+                if result:
+                    await self.helpers.cancel_tasks(tasks)
+                    return result, url
+            except (RequestError, ReadTimeout) as e:
+                if str(e):
+                    self.warning(str(e))
+                # cancel all the tasks if there's an error
+                await self.helpers.cancel_tasks(tasks)
+                break
+
+        return None, None
+
+    async def check_ntlm(self, test_url):
+        # use lower timeout value
+        http_timeout = self.config.get("httpx_timeout", 5)
+        r = await self.helpers.request(
+            test_url, headers=NTLM_test_header, raise_error=True, allow_redirects=False, timeout=http_timeout
+        )
+        ntlm_resp = r.headers.get("WWW-Authenticate", "")
+        if ntlm_resp:
+            ntlm_resp_b64 = max(ntlm_resp.split(","), key=lambda x: len(x)).split()[-1]
+            try:
+                ntlm_resp_decoded = self.helpers.ntlm.ntlmdecode(ntlm_resp_b64)
+                if ntlm_resp_decoded:
+                    return ntlm_resp_decoded, test_url
+            except NTLMError as e:
+                self.verbose(str(e))
+                return None, test_url
+        return None, test_url
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1793rc0/bbot/modules/ipneighbor.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     flags = ["passive", "subdomain-enum", "aggressive"]
     meta = {"description": "Look beside IPs in their surrounding subnet"}
     options = {"num_bits": 4}
     options_desc = {"num_bits": "Netmask size (in CIDR notation) to check. Default is 4 bits (16 hosts)"}
     scope_distance_modifier = 1
     _scope_shepherding = False
 
-    def setup(self):
+    async def setup(self):
         self.processed = set()
         self.num_bits = max(1, int(self.config.get("num_bits", 4)))
         return True
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if str(event.module) in ("speculate", "ipneighbor"):
             return False
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         main_ip = event.host
         netmask = main_ip.max_prefixlen - min(main_ip.max_prefixlen, self.num_bits)
         network = ipaddress.ip_network(f"{main_ip}/{netmask}", strict=False)
         subnet_hash = hash(network)
         if not subnet_hash in self.processed:
             self.processed.add(subnet_hash)
             for ip in network:
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1793rc0/bbot/modules/ipstack.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,32 +15,35 @@
     options_desc = {"api_key": "IPStack GeoIP API Key"}
     scope_distance_modifier = 1
     _priority = 2
     suppress_dupes = False
 
     base_url = "http://api.ipstack.com/"
 
-    def ping(self):
-        r = self.request_with_fail_count(f"{self.base_url}/check?access_key={self.api_key}")
+    async def filter_event(self, event):
+        return True
+
+    async def ping(self):
+        url = f"{self.base_url}/check?access_key={self.api_key}"
+        r = await self.request_with_fail_count(url)
         resp_content = getattr(r, "text", "")
         assert getattr(r, "status_code", 0) == 200, resp_content
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         try:
             url = f"{self.base_url}/{event.data}?access_key={self.api_key}"
-            result = self.request_with_fail_count(url)
+            result = await self.request_with_fail_count(url)
             if result:
                 j = result.json()
                 if not j:
                     self.verbose(f"No JSON response from {url}")
             else:
                 self.verbose(f"No response from {url}")
         except Exception:
-            self.verbose(f"Error retrieving results for {event.data}")
-            self.trace()
+            self.verbose(f"Error retrieving results for {event.data}", trace=True)
             return
         geo_data = {
             "ip": j.get("ip"),
             "country": j.get("country_name"),
             "city": j.get("city"),
             "zip_code": j.get("zip"),
             "region": j.get("region_name"),
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1793rc0/bbot/modules/certspotter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from .crobat import crobat
+from bbot.modules.crobat import crobat
 
 
-class leakix(crobat):
+class certspotter(crobat):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query leakix.net for subdomains"}
+    meta = {"description": "Query Certspotter's API for subdomains"}
 
-    base_url = "https://leakix.net"
+    base_url = "https://api.certspotter.com/v1"
 
     def request_url(self, query):
-        url = f"{self.base_url}/api/subdomains/{self.helpers.quote(query)}"
-        return self.request_with_fail_count(url, headers={"Accept": "application/json"})
+        url = f"{self.base_url}/issuances?domain={self.helpers.quote(query)}&include_subdomains=true&expand=dns_names"
+        return self.request_with_fail_count(url, timeout=self.http_timeout + 30)
 
-    def parse_results(self, r, query=None):
+    def parse_results(self, r, query):
         json = r.json()
         if json:
-            for entry in json:
-                subdomain = entry.get("subdomain", "")
-                if subdomain:
-                    yield subdomain
+            for r in json:
+                for dns_name in r.get("dns_names", []):
+                    yield dns_name.lstrip(".*").rstrip(".")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1793rc0/bbot/modules/masscan.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,26 +46,26 @@
         {
             "name": "Install masscan",
             "copy": {"src": "#{BBOT_TEMP}/masscan/bin/masscan", "dest": "#{BBOT_TOOLS}/", "mode": "u+x,g+x,o+x"},
         },
     ]
     _qsize = 100
 
-    def setup(self):
+    async def setup(self):
         self.ports = self.config.get("ports", "80,443")
         self.rate = self.config.get("rate", 600)
         self.wait = self.config.get("wait", 10)
         self.ping_first = self.config.get("ping_first", False)
         self.alive_hosts = dict()
         # make a quick dry run to validate ports etc.
         self._target_findkey = "9.8.7.6"
         if not self.helpers.in_tests:
             try:
                 dry_run_command = self._build_masscan_command(self._target_findkey, dry_run=True)
-                dry_run_result = self.helpers.run(dry_run_command)
+                dry_run_result = await self.helpers.run(dry_run_command)
                 self.masscan_config = dry_run_result.stdout
                 self.masscan_config = "\n".join(l for l in self.masscan_config.splitlines() if "nocapture" not in l)
             except subprocess.CalledProcessError as e:
                 self.warning(f"Error in masscan: {e.stderr}")
                 return False
 
         self.run_time = self.helpers.make_date()
@@ -87,15 +87,15 @@
                 )
         else:
             self.helpers.depsinstaller.ensure_root(message="Masscan requires root privileges")
         self.ping_cache_fd = None
         self.syn_cache_fd = None
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         if self.use_cache:
             self.emit_from_cache()
         else:
             exclude, invalid_exclude = self._build_targets(self.scan.blacklist)
             targets, invalid_targets = self._build_targets(self.scan.whitelist)
             if invalid_exclude > 0:
                 self.warning(
@@ -110,30 +110,30 @@
                 self.warning("No targets specified")
                 return
 
             # ping scan
             if self.ping_first:
                 self.verbose("Starting masscan (ping scan)")
 
-                self.masscan(targets, result_callback=self.append_alive_host, exclude=exclude, ping=True)
+                await self.masscan(targets, result_callback=self.append_alive_host, exclude=exclude, ping=True)
                 targets = ",".join(str(h) for h in self.alive_hosts)
                 if not targets:
                     self.warning("No hosts responded to pings")
                     return
 
             # TCP SYN scan
             if self.ports:
                 self.verbose("Starting masscan (TCP SYN scan)")
-                self.masscan(targets, result_callback=self.emit_open_tcp_port, exclude=exclude)
+                await self.masscan(targets, result_callback=self.emit_open_tcp_port, exclude=exclude)
             else:
                 self.verbose("No ports specified, skipping TCP SYN scan")
             # save memory
             self.alive_hosts.clear()
 
-    def masscan(self, targets, result_callback, exclude=None, ping=False):
+    async def masscan(self, targets, result_callback, exclude=None, ping=False):
         # config file
         masscan_config = self.masscan_config.replace(self._target_findkey, targets)
         self.debug("Masscan config:")
         for line in masscan_config.splitlines():
             self.debug(line)
         config_file = self.helpers.tempfile(masscan_config)
         # output file
@@ -141,15 +141,15 @@
         # json_output_file = self.helpers.tempfile_tail(process_output)
         # command
         command = self._build_masscan_command(config=config_file, exclude=exclude, ping=ping)
         # execute
         stats_file = self.helpers.tempfile_tail(callback=self.verbose)
         try:
             with open(stats_file, "w") as stats_fh:
-                for line in self.helpers.run_live(command, sudo=True, stderr=stats_fh):
+                async for line in self.helpers.run_live(command, sudo=True, stderr=stats_fh):
                     self.process_output(line, result_callback=result_callback)
         finally:
             stats_file.unlink()
 
     def _build_masscan_command(self, targets=None, config=None, exclude=None, dry_run=False, ping=False):
         command = ("masscan", "--rate", self.rate, "--wait", self.wait, "--open-only", "-oJ", "-")
         if targets is not None:
@@ -250,15 +250,15 @@
             t = self.helpers.make_ip_type(t.data)
             if isinstance(t, str):
                 invalid_targets += 1
             else:
                 targets.append(t)
         return ",".join(str(t) for t in targets), invalid_targets
 
-    def cleanup(self):
+    async def cleanup(self):
         if self.ping_first:
             with suppress(Exception):
                 self.ping_cache_fd.close()
         with suppress(Exception):
             self.syn_cache_fd.close()
 
     def _write_ping_result(self, host):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1793rc0/bbot/modules/massdns.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class massdns(crobat):
     flags = ["subdomain-enum", "passive", "slow", "aggressive"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     meta = {"description": "Brute-force subdomains with massdns (highly effective)"}
     options = {
         "wordlist": "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Discovery/DNS/subdomains-top1million-5000.txt",
-        "max_resolvers": 500,
+        "max_resolvers": 1000,
         "max_mutations": 500,
     }
     options_desc = {
         "wordlist": "Subdomain wordlist URL",
         "max_resolvers": "Number of concurrent massdns resolvers",
         "max_mutations": "Max number of smart mutations per subdomain",
     }
@@ -53,57 +53,57 @@
             "when": "ansible_facts['system'] != 'Linux'",
         },
         {
             "name": "Install massdns",
             "copy": {"src": "#{BBOT_TEMP}/massdns/bin/massdns", "dest": "#{BBOT_TOOLS}/", "mode": "u+x,g+x,o+x"},
         },
     ]
-    reject_wildcards = "cloud_only"
+    reject_wildcards = "strict"
     _qsize = 100
 
     digit_regex = re.compile(r"\d+")
 
-    def setup(self):
+    async def setup(self):
         self.found = dict()
         self.mutations_tried = set()
         self.source_events = dict()
-        self.subdomain_file = self.helpers.wordlist(self.config.get("wordlist"))
-        self.max_resolvers = self.config.get("max_resolvers", 500)
+        self.subdomain_file = await self.helpers.wordlist(self.config.get("wordlist"))
+        self.max_resolvers = self.config.get("max_resolvers", 1000)
         self.max_mutations = self.config.get("max_mutations", 500)
         nameservers_url = (
             "https://raw.githubusercontent.com/blacklanternsecurity/public-dns-servers/master/nameservers.txt"
         )
-        self.resolver_file = self.helpers.wordlist(
+        self.resolver_file = await self.helpers.wordlist(
             nameservers_url,
             cache_hrs=24 * 7,
         )
         self.devops_mutations = list(self.helpers.word_cloud.devops_mutations)
-        return super().setup()
+        return await super().setup()
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         query = self.make_query(event)
-        eligible, reason = self.eligible_for_enumeration(event)
+        eligible, reason = await self.eligible_for_enumeration(event)
         if eligible:
             self.add_found(event)
         # reject if already processed
         if self.already_processed(query):
             return False, f'Query "{query}" was already processed'
         if eligible:
             self.processed.add(hash(query))
             return True, reason
         return False, reason
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
         h = hash(query)
         if not h in self.source_events:
             self.source_events[h] = event
 
-        self.info(f"Brute-forcing subdomains for {query}")
-        for hostname in self.massdns(query, self.helpers.read_file(self.subdomain_file)):
+        self.info(f"Brute-forcing subdomains for {query} (source: {event.data})")
+        for hostname in await self.massdns(query, self.helpers.read_file(self.subdomain_file)):
             self.emit_result(hostname, event, query)
 
     def abort_if(self, event):
         if not event.scope_distance == 0:
             return True, "event is not in scope"
         if "wildcard" in event.tags:
             return True, "event is a wildcard"
@@ -114,41 +114,46 @@
             self.emit_event(result, "DNS_NAME", source_event, **kwargs)
 
     def already_processed(self, hostname):
         if hash(hostname) in self.processed:
             return True
         return False
 
-    def massdns(self, domain, subdomains):
+    async def massdns(self, domain, subdomains):
         abort_msg = f"Aborting massdns on {domain} due to false positives"
-        if self._canary_check(domain):
+        if await self._canary_check(domain):
             self.info(abort_msg)
             return []
-        results = list(self._massdns(domain, subdomains))
+        results = [l async for l in self._massdns(domain, subdomains)]
         if len(results) > 50:
-            if self._canary_check(domain):
+            if await self._canary_check(domain):
                 self.info(abort_msg)
                 return []
         self.verbose(f"Resolving batch of {len(results):,} results")
-        resolved = dict(self.helpers.resolve_batch(results, type=("A", "AAAA", "CNAME"), cache_result=True))
+        resolved = dict(
+            [l async for l in self.helpers.resolve_batch(results, type=("A", "AAAA", "CNAME"), cache_result=True)]
+        )
         resolved = {k: v for k, v in resolved.items() if v}
         for hostname in resolved:
             self.add_found(hostname)
         return list(resolved)
 
-    def _canary_check(self, domain, num_checks=50):
+    async def _canary_check(self, domain, num_checks=50):
         random_subdomains = list(self.gen_random_subdomains(num_checks))
         self.verbose(f"Testing {len(random_subdomains):,} canaries against {domain}")
-        canary_results = list(self._massdns(domain, random_subdomains))
-        for result in canary_results:
-            if self.helpers.resolve(result):
+        canary_results = [l async for l in self._massdns(domain, random_subdomains)]
+        async for result in self.helpers.resolve_batch(canary_results):
+            if result:
                 return True
+        # for result in canary_results:
+        #     if await self.helpers.resolve(result):
+        #         return True
         return False
 
-    def _massdns(self, domain, subdomains):
+    async def _massdns(self, domain, subdomains):
         """
         {
           "name": "www.blacklanternsecurity.com.",
           "type": "A",
           "class": "IN",
           "status": "NOERROR",
           "data": {
@@ -172,15 +177,15 @@
           "resolver": "168.215.165.186:53"
         }
         """
         if self.scan.stopping:
             return
 
         domain_wildcard_rdtypes = set()
-        for domain, rdtypes in self.helpers.is_wildcard_domain(domain).items():
+        for domain, rdtypes in (await self.helpers.is_wildcard_domain(domain)).items():
             for rdtype, results in rdtypes.items():
                 if results:
                     domain_wildcard_rdtypes.add(rdtype)
 
         command = (
             "massdns",
             "-r",
@@ -193,15 +198,15 @@
             "AAAA",
             "-o",
             "J",
             "-q",
         )
         subdomains = self.gen_subdomains(subdomains, domain)
         hosts_yielded = set()
-        for line in self.helpers.run_live(command, stderr=subprocess.DEVNULL, input=subdomains):
+        async for line in self.helpers.run_live(command, stderr=subprocess.DEVNULL, input=subdomains):
             try:
                 j = json.loads(line)
             except json.decoder.JSONDecodeError:
                 self.debug(f"Failed to decode line: {line}")
                 continue
             answers = j.get("data", {}).get("answers", [])
             if type(answers) == list and len(answers) > 0:
@@ -218,24 +223,24 @@
                             # skip wildcard checking on multi-level subdomains for performance reasons
                             stem = hostname.split(domain)[0].strip(".")
                             if "." in stem:
                                 self.debug(
                                     f"Skipping {hostname}:{rdtype} because it may be a wildcard (reason: performance)"
                                 )
                                 continue
-                            wildcard_rdtypes = self.helpers.is_wildcard(hostname, ips=(data,))
+                            wildcard_rdtypes = await self.helpers.is_wildcard(hostname, ips=(data,))
                             if rdtype in wildcard_rdtypes:
                                 self.debug(f"Skipping {hostname}:{rdtype} because it's a wildcard")
                                 continue
                         hostname_hash = hash(hostname)
                         if hostname_hash not in hosts_yielded:
                             hosts_yielded.add(hostname_hash)
                             yield hostname
 
-    def finish(self):
+    async def finish(self):
         found = sorted(self.found.items(), key=lambda x: len(x[-1]), reverse=True)
         # if we have a lot of rounds to make, don't try mutations on less-populated domains
         trimmed_found = []
         if found:
             avg_subdomains = sum([len(subdomains) for domain, subdomains in found[:50]]) / len(found[:50])
             for i, (domain, subdomains) in enumerate(found):
                 # accept domains that are in the top 50 or have more than 5 percent of the average number of subdomains
@@ -306,15 +311,15 @@
                     for subdomain in self.helpers.word_cloud.dns_mutator.mutations(
                         subdomains, max_mutations=self.max_mutations
                     ):
                         add_mutation(domain_hash, subdomain)
 
                     if mutations:
                         self.info(f"Trying {len(mutations):,} mutations against {domain} ({i+1}/{len(found)})")
-                        results = list(self.massdns(query, mutations))
+                        results = list(await self.massdns(query, mutations))
                         for hostname in results:
                             source_event = self.get_source_event(hostname)
                             if source_event is None:
                                 self.warning(f"Could not correlate source event from: {hostname}")
                                 continue
                             self.emit_result(hostname, source_event, query)
                         if results:
@@ -330,15 +335,15 @@
             subdomain, domain = host.split(".", 1)
             if not self.helpers.is_ptr(subdomain):
                 try:
                     self.found[domain].add(subdomain)
                 except KeyError:
                     self.found[domain] = set((subdomain,))
 
-    def gen_subdomains(self, prefixes, domain):
+    async def gen_subdomains(self, prefixes, domain):
         for p in prefixes:
             d = f"{p}.{domain}"
             yield d
 
     def gen_random_subdomains(self, n=50):
         delimeters = (".", "-")
         lengths = list(range(10, 20))
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1793rc0/bbot/modules/naabu.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     }
     options_desc = {
         "ports": "ports to scan",
         "top_ports": "top ports to scan",
         "skip_host_discovery": "skip host discovery (-Pn)",
         "version": "naabu version",
     }
-    max_event_handlers = 2
+    max_event_handlers = 1
     batch_size = 256
     _priority = 2
 
     deps_ansible = [
         {
             "name": "install libpcap (Debian)",
             "package": {"name": "libpcap0.8", "state": "present"},
@@ -52,23 +52,23 @@
                 "include": "naabu",
                 "dest": "#{BBOT_TOOLS}",
                 "remote_src": True,
             },
         },
     ]
 
-    def setup(self):
+    async def setup(self):
         self.helpers.depsinstaller.ensure_root(message="Naabu requires root privileges")
         self.skip_host_discovery = self.config.get("skip_host_discovery", True)
         return True
 
-    def handle_batch(self, *events):
+    async def handle_batch(self, *events):
         _input = [str(e.data) for e in events]
         command = self.construct_command()
-        for line in self.helpers.run_live(command, input=_input, stderr=subprocess.DEVNULL, sudo=False):
+        async for line in self.helpers.run_live(command, input=_input, stderr=subprocess.DEVNULL, sudo=False):
             try:
                 j = json.loads(line)
             except Exception as e:
                 self.debug(f'Error parsing line "{line}" as JSON: {e}')
                 break
             host = j.get("host", j.get("ip"))
             port = j.get("port")
@@ -111,10 +111,10 @@
             command += ["-Pn"]
         if ports:
             command += ["-p", ports]
         else:
             command += ["-top-ports", top_ports]
         return command
 
-    def cleanup(self):
+    async def cleanup(self):
         resume_file = self.helpers.current_dir / "resume.cfg"
         resume_file.unlink(missing_ok=True)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/otx.py` & `bbot-1.0.5.1793rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1793rc0/bbot/modules/output/asset_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import ipaddress
+from contextlib import suppress
 
 from .csv import CSV
 from bbot.core.helpers.misc import make_ip_type, is_ip, is_port
 
 severity_map = {
     "INFO": 0,
     0: "N/A",
@@ -29,44 +30,45 @@
         "use_previous": "Emit previous asset inventory as new events (use in conjunction with -n <old_scan_name>)",
         "summary_netmask": "Subnet mask to use when summarizing IP addresses at end of scan",
     }
 
     header_row = ["Host", "Provider", "IP(s)", "Status", "Open Ports", "Risk Rating", "Findings", "Description"]
     filename = "asset-inventory.csv"
 
-    def setup(self):
+    async def setup(self):
         self.assets = {}
         self.open_port_producers = "httpx" in self.scan.modules or any(
             ["portscan" in m.flags for m in self.scan.modules.values()]
         )
         self.use_previous = self.config.get("use_previous", False)
         self.summary_netmask = self.config.get("summary_netmask", 16)
         self.emitted_contents = False
-        ret = super().setup()
+        self._ran_hooks = False
+        ret = await super().setup()
         return ret
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if event._internal:
             return False, "event is internal"
         if event.type not in self.watched_events:
             return False, "event type is not in watched_events"
         if not self.scan.in_scope(event):
             return False, "event is not in scope"
         if "unresolved" in event.tags:
             return False, "event is unresolved"
         return True, ""
 
-    def handle_event(self, event):
-        if self.filter_event(event)[0]:
+    async def handle_event(self, event):
+        if (await self.filter_event(event))[0]:
             hostkey = _make_hostkey(event.host, event.resolved_hosts)
             if hostkey not in self.assets:
                 self.assets[hostkey] = Asset(event.host)
             self.assets[hostkey].absorb_event(event)
 
-    def report(self):
+    async def report(self):
         stats = dict()
         totals = dict()
 
         def increment_stat(stat, value):
             try:
                 totals[stat] += 1
             except KeyError:
@@ -74,15 +76,22 @@
             if not stat in stats:
                 stats[stat] = {}
             try:
                 stats[stat][value] += 1
             except KeyError:
                 stats[stat][value] = 1
 
-        for asset in sorted(self.assets.values(), key=lambda a: str(a.host)):
+        def sort_key(asset):
+            host = str(asset.host)
+            is_digit = False
+            with suppress(IndexError):
+                is_digit = host[0].isdigit()
+            return (is_digit, host)
+
+        for asset in sorted(self.assets.values(), key=sort_key):
             findings_and_vulns = asset.findings.union(asset.vulnerabilities)
             ports = getattr(asset, "ports", set())
             ports = [str(p) for p in sorted([int(p) for p in asset.ports])]
             ips = sorted([str(i) for i in getattr(asset, "ip_addresses", [])])
             host = getattr(asset, "host", "")
             if host:
                 domain = self.helpers.tldextract(host).registered_domain
@@ -113,18 +122,17 @@
                 stats_sorted = sorted(stats[header].items(), key=lambda x: x[-1], reverse=True)
                 total = totals[header]
                 for k, v in stats_sorted:
                     table.append([str(k), f"{v:,}/{total} ({v/total*100:.1f}%)"])
                 self.log_table(table, table_header, table_name=f"asset-inventory-{header}")
 
         if self._file is not None:
-            with self._report_lock:
-                self.info(f"Saved asset-inventory output to {self.output_file}")
+            self.info(f"Saved asset-inventory output to {self.output_file}")
 
-    def emit_contents(self):
+    async def finish(self):
         if self.use_previous and not self.emitted_contents:
             self.emitted_contents = True
             if self.output_file.is_file():
                 self.info(f"Emitting previous results from {self.output_file}")
                 with open(self.output_file, newline="") as f:
                     c = csv.DictReader(f)
                     for row in c:
@@ -154,17 +162,16 @@
                                     netloc = self.helpers.make_netloc(ip, port)
                                     open_port_event = self.make_event(netloc, "OPEN_TCP_PORT", source=ip_event)
                                     self.emit_event(open_port_event)
             else:
                 self.warning(
                     f"use_previous=True was set but no previous asset inventory was found at {self.output_file}"
                 )
-
-    def finish(self):
-        self.emit_contents()
+        else:
+            self._run_hooks()
 
     def _run_hooks(self):
         """
         modules can use self.asset_inventory_hook() to add custom functionality to asset_inventory
         the asset inventory module is passed in as the first argument to the method.
         """
         if not self._ran_hooks:
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1793rc0/bbot/modules/output/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     meta = {"description": "Output to CSV"}
     options = {"output_file": ""}
     options_desc = {"output_file": "Output to CSV file"}
 
     header_row = ["Event type", "Event data", "IP Address", "Source Module", "Scope Distance", "Event Tags"]
     filename = "output.csv"
 
-    def setup(self):
+    async def setup(self):
         self.custom_headers = []
         self._headers_set = set()
         self._writer = None
         self._prep_output_dir(self.filename)
         return True
 
     @property
@@ -39,38 +39,37 @@
     def fieldnames(self):
         return self.header_row + list(self.custom_headers)
 
     def writerow(self, row):
         self.writer.writerow(row)
         self.file.flush()
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         # ["Event type", "Event data", "IP Address", "Source Module", "Scope Distance", "Event Tags"]
         self.writerow(
             {
                 "Event type": getattr(event, "type", ""),
                 "Event data": getattr(event, "data", ""),
                 "IP Address": ",".join(
                     str(x) for x in getattr(event, "resolved_hosts", set()) if self.helpers.is_ip(x)
                 ),
                 "Source Module": str(getattr(event, "module_sequence", "")),
                 "Scope Distance": str(getattr(event, "scope_distance", "")),
                 "Event Tags": ",".join(sorted(list(getattr(event, "tags", [])))),
             }
         )
 
-    def cleanup(self):
+    async def cleanup(self):
         if getattr(self, "_file", None) is not None:
             with suppress(Exception):
                 self.file.close()
 
-    def report(self):
+    async def report(self):
         if self._file is not None:
-            with self._report_lock:
-                self.info(f"Saved CSV output to {self.output_file}")
+            self.info(f"Saved CSV output to {self.output_file}")
 
     def add_custom_headers(self, headers):
         if isinstance(headers, str):
             headers = [headers]
         for header in headers:
             if header not in self._headers_set:
                 self._headers_set.add(header)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1793rc0/bbot/modules/output/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import requests
-from requests.auth import HTTPBasicAuth
-from requests.exceptions import RequestException
+from bbot.core.errors import RequestError
 
 from bbot.modules.output.base import BaseOutputModule
 
 
 class HTTP(BaseOutputModule):
     watched_events = ["*"]
     meta = {"description": "Send every event to a custom URL via a web request"}
@@ -21,36 +19,43 @@
         "method": "HTTP method",
         "bearer": "Authorization Bearer token",
         "username": "Username (basic auth)",
         "password": "Password (basic auth)",
         "timeout": "HTTP timeout",
     }
 
-    def setup(self):
-        self.session = requests.Session()
-        if not self.config.get("url", ""):
+    async def setup(self):
+        self.url = self.config.get("url", "")
+        self.method = self.config.get("method", "POST")
+        self.timeout = self.config.get("timeout", 10)
+        self.headers = {}
+        bearer = self.config.get("bearer", "")
+        if bearer:
+            self.headers["Authorization"] = f"Bearer {bearer}"
+        username = self.config.get("username", "")
+        password = self.config.get("password", "")
+        self.auth = None
+        if username:
+            self.auth = (username, password)
+        if not self.url:
             self.warning("Must set URL")
             return False
-        if not self.config.get("method", ""):
+        if not self.method:
             self.warning("Must set HTTP method")
             return False
         return True
 
-    def handle_event(self, event):
-        r = requests.Request(
-            url=self.config.get("url"),
-            method=self.config.get("method", "POST"),
-        )
-        r.headers["User-Agent"] = self.scan.useragent
-        r.json = dict(event)
-        username = self.config.get("username", "")
-        password = self.config.get("password", "")
-        if username:
-            r.auth = HTTPBasicAuth(username, password)
-        bearer = self.config.get("bearer", "")
-        if bearer:
-            r.headers["Authorization"] = f"Bearer {bearer}"
-        try:
-            timeout = self.config.get("timeout", 10)
-            self.session.send(r.prepare(), timeout=timeout)
-        except RequestException as e:
-            self.warning(f"Error sending {event}: {e}")
+    async def handle_event(self, event):
+        while 1:
+            try:
+                await self.helpers.request(
+                    url=self.url,
+                    method=self.method,
+                    auth=self.auth,
+                    headers=self.headers,
+                    json=dict(event),
+                    raise_error=True,
+                )
+                break
+            except RequestError as e:
+                self.warning(f"Error sending {event}: {e}, retrying...")
+                await self.helpers.sleep(1)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1793rc0/bbot/modules/output/human.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 class Human(BaseOutputModule):
     watched_events = ["*"]
     meta = {"description": "Output to text"}
     options = {"output_file": "", "console": True}
     options_desc = {"output_file": "Output to file", "console": "Output to console"}
     vuln_severity_map = {"LOW": "HUGEWARNING", "MEDIUM": "HUGEWARNING", "HIGH": "CRITICAL", "CRITICAL": "CRITICAL"}
 
-    def setup(self):
+    async def setup(self):
         self._prep_output_dir("output.txt")
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         event_type = f"[{event.type}]"
         event_tags = ""
         if getattr(event, "tags", []):
             event_tags = f'\t({", ".join(sorted(getattr(event, "tags", [])))})'
         event_str = f"{event_type:<20}\t{event.data_human}\t{event.module_sequence}{event_tags}"
         # log vulnerabilities in vivid colors
         if event.type == "VULNERABILITY":
@@ -32,16 +32,15 @@
 
         if self.file is not None:
             self.file.write(event_str + "\n")
             self.file.flush()
         if self.config.get("console", True):
             self.stdout(event_str)
 
-    def cleanup(self):
+    async def cleanup(self):
         if getattr(self, "_file", None) is not None:
             with suppress(Exception):
                 self.file.close()
 
-    def report(self):
+    async def report(self):
         if self._file is not None:
-            with self._report_lock:
-                self.info(f"Saved TXT output to {self.output_file}")
+            self.info(f"Saved TXT output to {self.output_file}")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1793rc0/bbot/modules/output/web_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     options = {
         "output_file": "",
         "css_theme_file": "https://cdnjs.cloudflare.com/ajax/libs/github-markdown-css/5.1.0/github-markdown.min.css",
     }
     options_desc = {"output_file": "Output to file", "css_theme_file": "CSS theme URL for HTML output"}
     deps_pip = ["markdown~=3.4.3"]
 
-    def setup(self):
+    async def setup(self):
         html_css_file = self.config.get("css_theme_file", "")
 
         self.html_header = f"""
         <!DOCTYPE html>
         <html>
         <head>
         <link rel="stylesheet" href="{html_css_file}">
@@ -28,15 +28,15 @@
         self.html_footer = "</body></html>"
         self.web_assets = {}
         self.markdown = ""
 
         self._prep_output_dir("web_report.html")
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         if event.type == "URL":
             parsed = event.parsed
             host = f"{parsed.scheme}://{parsed.netloc}/"
             if host not in self.web_assets.keys():
                 self.web_assets[host] = {"URL": []}
             source_chain = []
 
@@ -70,15 +70,15 @@
                 if host not in self.web_assets.keys():
                     self.web_assets[host] = {"URL": []}
                 if event.type not in self.web_assets[host].keys():
                     self.web_assets[host][event.type] = [html.escape(event.pretty_string)]
                 else:
                     self.web_assets[host][event.type].append(html.escape(event.pretty_string))
 
-    def report(self):
+    async def report(self):
         for host in self.web_assets.keys():
             self.markdown += f"# {host}\n\n"
 
             for event_type in self.web_assets[host].keys():
                 self.markdown += f"### {event_type}\n"
                 dedupe = []
                 for e in self.web_assets[host][event_type]:
@@ -89,9 +89,8 @@
                 self.markdown += "\n"
 
         if self.file is not None:
             self.file.write(self.html_header)
             self.file.write(markdown.markdown(self.markdown))
             self.file.write(self.html_footer)
             self.file.flush()
-            with self._report_lock:
-                self.info(f"Web Report saved to {self.output_file}")
+            self.info(f"Web Report saved to {self.output_file}")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1793rc0/bbot/modules/output/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,51 @@
-import json
-import threading
-import websocket
-from time import sleep
-
-from bbot.modules.output.base import BaseOutputModule
-
-
-class Websocket(BaseOutputModule):
-    watched_events = ["*"]
-    meta = {"description": "Output to websockets"}
-    options = {"url": "", "token": ""}
-    options_desc = {"url": "Web URL", "token": "Authorization Bearer token"}
-
-    def setup(self):
-        self.url = self.config.get("url", "")
-        if not self.url:
-            return False, "Must set URL"
-        kwargs = {}
-        self.token = self.config.get("token", "")
-        if self.token:
-            kwargs.update({"header": {"Authorization": f"Bearer {self.token}"}})
-        self.ws = websocket.WebSocketApp(self.url, **kwargs)
-        self.started = False
-        return True
-
-    def start_websocket(self):
-        if not self.started:
-            self.thread = threading.Thread(target=self._start_websocket, daemon=True)
-            self.thread.start()
-            self.started = True
-
-    def _start_websocket(self):
-        not_keyboardinterrupt = False
-        while not self.scan.stopping:
-            not_keyboardinterrupt = self.ws.run_forever()
-            if not not_keyboardinterrupt:
-                break
-            sleep(1)
-
-    def handle_event(self, event):
-        self.start_websocket()
-        event_json = event.json()
-        self.send(event_json)
-
-    def send(self, message):
-        while self.ws is not None:
-            try:
-                self.ws.send(json.dumps(message))
-                break
-            except Exception as e:
-                self.warning(f"Error sending message: {e}, retrying")
-                sleep(1)
-                continue
-
-    def cleanup(self):
-        self.ws.close()
-        self.ws = None
+import logging
+from pathlib import Path
+from bbot.modules.base import BaseModule
+
+
+class BaseOutputModule(BaseModule):
+    accept_dupes = True
+    _type = "output"
+    scope_distance_modifier = None
+    _stats_exclude = True
+
+    def _event_precheck(self, event):
+        # omitted events such as HTTP_RESPONSE etc.
+        if event._omit:
+            return False, "_omit is True"
+        # forced events like intermediary links in a DNS resolution chain
+        if event._force_output:
+            return True, "_force_output is True"
+        # internal events like those from speculate, ipneighbor
+        # or events that are over our report distance
+        if event._internal:
+            return False, "_internal is True"
+        return super()._event_precheck(event)
+
+    def _prep_output_dir(self, filename):
+        self.output_file = self.config.get("output_file", "")
+        if self.output_file:
+            self.output_file = Path(self.output_file)
+        else:
+            self.output_file = self.scan.home / str(filename)
+        self.helpers.mkdir(self.output_file.parent)
+        self._file = None
+
+    @property
+    def file(self):
+        if self._file is None:
+            self._file = open(self.output_file, mode="a")
+        return self._file
+
+    @property
+    def config(self):
+        config = self.scan.config.get("output_modules", {}).get(self.name, {})
+        if config is None:
+            config = {}
+        return config
+
+    @property
+    def log(self):
+        if self._log is None:
+            self._log = logging.getLogger(f"bbot.modules.output.{self.name}")
+        return self._log
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1793rc0/bbot/modules/paramminer_cookies.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from bbot.core.errors import ScanCancelledError
 from .paramminer_headers import paramminer_headers
 
 
 class paramminer_cookies(paramminer_headers):
     """
     Inspired by https://github.com/PortSwigger/param-miner
     """
@@ -17,19 +16,17 @@
     options_desc = {"wordlist": "Define the wordlist to be used to derive cookies"}
     scanned_hosts = []
     cookie_blacklist = []
     max_event_handlers = 12
     in_scope_only = True
     compare_mode = "cookie"
 
-    def check_batch(self, compare_helper, url, cookie_list):
-        if self.scan.stopping:
-            raise ScanCancelledError()
+    async def check_batch(self, compare_helper, url, cookie_list):
         cookies = {p: self.rand_string(14) for p in cookie_list}
-        return compare_helper.compare(url, cookies=cookies)
+        return await compare_helper.compare(url, cookies=cookies)
 
     def gen_count_args(self, url):
         cookie_count = 40
         while 1:
             if cookie_count < 0:
                 break
             fake_cookies = {self.rand_string(14): self.rand_string(14) for _ in range(0, cookie_count)}
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1793rc0/bbot/modules/paramminer_getparams.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from bbot.core.errors import ScanCancelledError
 from .paramminer_headers import paramminer_headers
 
 
 class paramminer_getparams(paramminer_headers):
     """
     Inspired by https://github.com/PortSwigger/param-miner
     """
@@ -12,23 +11,20 @@
     flags = ["active", "aggressive", "slow", "web-paramminer"]
     meta = {"description": "Use smart brute-force to check for common HTTP GET parameters"}
 
     options = {"wordlist": "https://raw.githubusercontent.com/PortSwigger/param-miner/master/resources/params"}
     options_desc = {"wordlist": "Define the wordlist to be used to derive GET params"}
     scanned_hosts = []
     getparam_blacklist = []
-    max_threads = 12
     in_scope_only = True
     compare_mode = "getparam"
 
-    def check_batch(self, compare_helper, url, getparam_list):
-        if self.scan.stopping:
-            raise ScanCancelledError()
+    async def check_batch(self, compare_helper, url, getparam_list):
         test_getparams = {p: self.rand_string(14) for p in getparam_list}
-        return compare_helper.compare(self.helpers.add_get_params(url, test_getparams).geturl())
+        return await compare_helper.compare(self.helpers.add_get_params(url, test_getparams).geturl())
 
     def gen_count_args(self, url):
         getparam_count = 40
         while 1:
             if getparam_count < 0:
                 break
             fake_getparams = {self.rand_string(14): self.rand_string(14) for _ in range(0, getparam_count)}
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1793rc0/bbot/modules/paramminer_headers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from bbot.modules.base import BaseModule
-from bbot.core.errors import HttpCompareError, ScanCancelledError
+from bbot.core.errors import HttpCompareError
 
 
 class paramminer_headers(BaseModule):
     """
     Inspired by https://github.com/PortSwigger/param-miner
     """
 
@@ -25,57 +25,55 @@
         "if-none-match",
         "if-unmodified-since",
     ]
     max_event_handlers = 12
     in_scope_only = True
     compare_mode = "header"
 
-    def setup(self):
+    async def setup(self):
         wordlist_url = self.config.get("wordlist", "")
-        self.wordlist = self.helpers.wordlist(wordlist_url)
+        self.wordlist = await self.helpers.wordlist(wordlist_url)
         return True
 
     def rand_string(self, *args, **kwargs):
         return self.helpers.rand_string(*args, **kwargs)
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         url = event.data
         try:
             compare_helper = self.helpers.http_compare(url)
         except HttpCompareError as e:
             self.debug(e)
             return
-        batch_size = self.count_test(url)
+        batch_size = await self.count_test(url)
         if batch_size == None or batch_size <= 0:
             self.debug(f"Failed to get baseline max {self.compare_mode} count, aborting")
             return
         self.debug(f"Resolved batch_size at {str(batch_size)}")
 
-        if compare_helper.canary_check(url, mode=self.compare_mode) == False:
+        if await compare_helper.canary_check(url, mode=self.compare_mode) == False:
             self.verbose(f'Aborting "{url}" due to failed canary check')
             return
 
         fl = [h.strip().lower() for h in self.helpers.read_file(self.wordlist)]
 
         wordlist_cleaned = list(filter(self.clean_list, fl))
 
         results = set()
         abort_threshold = 25
         try:
             for group in self.helpers.grouper(wordlist_cleaned, batch_size):
-                for result, reasons, reflection in self.binary_search(compare_helper, url, group):
+                async for result, reasons, reflection in self.binary_search(compare_helper, url, group):
                     results.add((result, ",".join(reasons), reflection))
                     if len(results) >= abort_threshold:
                         self.warning(
                             f"Abort threshold ({abort_threshold}) reached, too many {self.compare_mode}s found"
                         )
                         results.clear()
                         assert False
-        except ScanCancelledError:
-            return
         except AssertionError:
             pass
 
         for result, reasons, reflection in results:
             tags = []
             if reflection:
                 tags = ["http_reflection"]
@@ -83,22 +81,22 @@
             self.emit_event(
                 {"host": str(event.host), "url": url, "description": description},
                 "FINDING",
                 event,
                 tags=tags,
             )
 
-    def count_test(self, url):
-        baseline = self.helpers.request(url)
+    async def count_test(self, url):
+        baseline = await self.helpers.request(url)
         if baseline is None:
             return
         if str(baseline.status_code)[0] in ("4", "5"):
             return
         for count, args, kwargs in self.gen_count_args(url):
-            r = self.helpers.request(*args, **kwargs)
+            r = await self.helpers.request(*args, **kwargs)
             if r is not None and not ((str(r.status_code)[0] in ("4", "5"))):
                 return count
 
     def gen_count_args(self, url):
         header_count = 95
         while 1:
             if header_count < 0:
@@ -110,30 +108,29 @@
             header_count -= 5
 
     def clean_list(self, header):
         if (len(header) > 0) and ("%" not in header) and (header not in self.header_blacklist):
             return True
         return False
 
-    def binary_search(self, compare_helper, url, group, reasons=None, reflection=False):
+    async def binary_search(self, compare_helper, url, group, reasons=None, reflection=False):
         if reasons is None:
             reasons = []
         self.debug(f"Entering recursive binary_search with {len(group):,} sized group")
         if len(group) == 1:
             if reasons:
                 yield group[0], reasons, reflection
         elif len(group) > 1:
             for group_slice in self.helpers.split_list(group):
-                match, reasons, reflection, subject_response = self.check_batch(compare_helper, url, group_slice)
+                match, reasons, reflection, subject_response = await self.check_batch(compare_helper, url, group_slice)
                 if match == False:
-                    yield from self.binary_search(compare_helper, url, group_slice, reasons, reflection)
+                    async for r in self.binary_search(compare_helper, url, group_slice, reasons, reflection):
+                        yield r
         else:
             self.warning(f"Submitted group of size 0 to binary_search()")
 
-    def check_batch(self, compare_helper, url, header_list):
-        if self.scan.stopping:
-            raise ScanCancelledError()
+    async def check_batch(self, compare_helper, url, header_list):
         rand = self.rand_string()
         test_headers = {}
         for header in header_list:
             test_headers[header] = rand
-        return compare_helper.compare(url, headers=test_headers, check_reflection=(len(header_list) == 1))
+        return await compare_helper.compare(url, headers=test_headers, check_reflection=(len(header_list) == 1))
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1793rc0/bbot/modules/passivetotal.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Query the PassiveTotal API for subdomains", "auth_required": True}
     options = {"username": "", "api_key": ""}
     options_desc = {"username": "RiskIQ Username", "api_key": "RiskIQ API Key"}
 
     base_url = "https://api.passivetotal.org/v2"
 
-    def setup(self):
+    async def setup(self):
         self.username = self.config.get("username", "")
         self.api_key = self.config.get("api_key", "")
         self.auth = (self.username, self.api_key)
-        return super().setup()
+        return await super().setup()
 
-    def ping(self):
+    async def ping(self):
         url = f"{self.base_url}/account/quota"
-        j = self.request_with_fail_count(url, auth=self.auth).json()
+        j = (await self.request_with_fail_count(url, auth=self.auth)).json()
         limit = j["user"]["limits"]["search_api"]
         used = j["user"]["counts"]["search_api"]
         assert used < limit, "No quota remaining"
 
     def abort_if(self, event):
         # RiskIQ is famous for their junk data
         return super().abort_if(event) or "unresolved" in event.tags
 
-    def request_url(self, query):
+    async def request_url(self, query):
         url = f"{self.base_url}/enrichment/subdomains?query={self.helpers.quote(query)}"
-        return self.request_with_fail_count(url, auth=self.auth)
+        return await self.request_with_fail_count(url, auth=self.auth)
 
     def parse_results(self, r, query):
         for subdomain in r.json().get("subdomains", []):
             yield f"{subdomain}.{query}"
 
     @property
     def auth_secret(self):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1793rc0/bbot/modules/pgp.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,26 @@
         "search_urls": [
             "https://keyserver.ubuntu.com/pks/lookup?fingerprint=on&op=vindex&search=<query>",
             "http://the.earth.li:11371/pks/lookup?fingerprint=on&op=vindex&search=<query>",
         ]
     }
     options_desc = {"search_urls": "PGP key servers to search"}
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        results = self.query(query)
+        results = await self.query(query)
         if results:
             for hostname in results:
                 if not hostname == event:
                     self.emit_event(hostname, "EMAIL_ADDRESS", event, abort_if=self.abort_if)
 
-    def query(self, query):
+    async def query(self, query):
+        results = set()
         for url in self.config.get("search_urls", []):
             url = url.replace("<query>", self.helpers.quote(query))
-            response = self.helpers.request(url)
+            response = await self.helpers.request(url)
             if response is not None:
                 for email in self.helpers.extract_emails(response.text):
                     email = email.lower()
-                    if email.lower().endswith(query):
-                        yield email
+                    if email.endswith(query):
+                        results.add(email)
+        return results
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1793rc0/bbot/modules/rapiddns.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     meta = {"description": "Query rapiddns.io for subdomains"}
 
     base_url = "https://rapiddns.io"
 
-    def request_url(self, query):
+    async def request_url(self, query):
         url = f"{self.base_url}/subdomain/{self.helpers.quote(query)}?full=1#result"
-        return self.request_with_fail_count(url)
+        response = await self.request_with_fail_count(url)
+        return response
 
     def parse_results(self, r, query):
         results = set()
         text = getattr(r, "text", "")
         for match in self.helpers.regexes.dns_name_regex.findall(text):
             match = match.lower()
             if match.endswith(query):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1793rc0/bbot/modules/report/affiliates.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     watched_events = ["*"]
     produced_events = []
     flags = ["passive", "safe", "affiliates"]
     meta = {"description": "Summarize affiliate domains at the end of a scan"}
     scope_distance_modifier = None
     accept_dupes = True
 
-    def setup(self):
+    async def setup(self):
         self.affiliates = {}
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         self.add_affiliate(event)
 
-    def report(self):
+    async def report(self):
         affiliates = sorted(self.affiliates.items(), key=lambda x: x[-1]["weight"], reverse=True)
         header = ["Affiliate", "Score", "Count"]
         table = []
         for domain, stats in affiliates:
             count = stats["count"]
             weight = stats["weight"]
             table.append([domain, f"{weight:.2f}", f"{count:,}"])
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1793rc0/bbot/modules/report/asn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-from bbot.core.errors import ScanCancelledError
 from bbot.modules.report.base import BaseReportModule
 
 
 class asn(BaseReportModule):
     watched_events = ["IP_ADDRESS"]
     produced_events = ["ASN"]
     flags = ["passive", "subdomain-enum", "safe"]
     meta = {"description": "Query ripe and bgpview.io for ASNs"}
     scope_distance_modifier = 1
     # we accept dupes to avoid missing data
     # because sometimes IP addresses are re-emitted with lower scope distances
     accept_dupes = True
 
-    def setup(self):
+    async def setup(self):
         self.asn_counts = {}
         self.asn_cache = {}
         self.sources = ["bgpview", "ripe"]
         self.unknown_asn = {
             "asn": "UNKNOWN",
             "subnet": "0.0.0.0/32",
             "name": "unknown",
             "description": "unknown",
             "country": "",
         }
         return True
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if getattr(event.host, "is_private", False):
             return False
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         host = event.host
         if self.cache_get(host) == False:
-            asns = list(self.get_asn(host))
+            asns = await self.get_asn(host)
             if not asns:
                 self.cache_put(self.unknown_asn)
             else:
                 for asn in asns:
                     emails = asn.pop("emails", [])
                     self.cache_put(asn)
                     asn_event = self.make_event(asn, "ASN", source=event)
                     self.emit_event(asn_event)
                     for email in emails:
                         self.emit_event(email, "EMAIL_ADDRESS", source=asn_event)
 
-    def report(self):
+    async def report(self):
         asn_data = sorted(self.asn_cache.items(), key=lambda x: self.asn_counts[x[0]], reverse=True)
         if not asn_data:
             return
         header = ["ASN", "Subnet", "Host Count", "Name", "Description", "Country"]
         table = []
         for subnet, asn in asn_data:
             count = self.asn_counts[subnet]
@@ -78,64 +77,64 @@
                 self.asn_counts[p] += 1
                 if ret == False:
                     ret = p
             except KeyError:
                 continue
         return ret
 
-    def get_asn(self, ip, retries=1):
+    async def get_asn(self, ip, retries=1):
         """
         Takes in an IP
         returns a list of ASNs, e.g.:
             [{'asn': '54113', 'subnet': '2606:50c0:8000::/48', 'name': 'FASTLY', 'description': 'Fastly', 'country': 'US', 'emails': []}, {'asn': '54113', 'subnet': '2606:50c0:8000::/46', 'name': 'FASTLY', 'description': 'Fastly', 'country': 'US', 'emails': []}]
         """
         for attempt in range(retries + 1):
             for i, source in enumerate(list(self.sources)):
-                if self.scan.stopping:
-                    raise ScanCancelledError()
                 get_asn_fn = getattr(self, f"get_asn_{source}")
-                res = get_asn_fn(ip)
+                res = await get_asn_fn(ip)
                 if res == False:
                     # demote the current source to lowest priority since it just failed
                     self.sources.append(self.sources.pop(i))
                     self.verbose(f"Failed to contact {source}, retrying")
                     continue
                 return res
-        self.warning(f"Error retrieving ASN via for {ip}")
+        self.warning(f"Error retrieving ASN for {ip}")
         return []
 
-    def get_asn_ripe(self, ip):
+    async def get_asn_ripe(self, ip):
         url = f"https://stat.ripe.net/data/network-info/data.json?resource={ip}"
-        response = self.get_url(url, "ASN")
+        response = await self.get_url(url, "ASN")
         asns = []
         if response == False:
             return False
         data = response.get("data", {})
         if not data:
             data = {}
         prefix = data.get("prefix", "")
         asn_numbers = data.get("asns", [])
         if not prefix or not asn_numbers:
             return []
         if not asn_numbers:
             asn_numbers = []
         for number in asn_numbers:
-            asn = self.get_asn_metadata_ripe(number)
+            asn = await self.get_asn_metadata_ripe(number)
+            if asn == False:
+                return False
             asn["subnet"] = prefix
             asns.append(asn)
         return asns
 
-    def get_asn_metadata_ripe(self, asn_number):
+    async def get_asn_metadata_ripe(self, asn_number):
         metadata_keys = {
             "name": ["ASName", "OrgId"],
             "description": ["OrgName", "OrgTechName", "RTechName"],
             "country": ["Country"],
         }
         url = f"https://stat.ripe.net/data/whois/data.json?resource={asn_number}"
-        response = self.get_url(url, "ASN Metadata", cache=True)
+        response = await self.get_url(url, "ASN Metadata", cache=True)
         if response == False:
             return False
         data = response.get("data", {})
         if not data:
             data = {}
         records = data.get("records", [])
         if not records:
@@ -154,17 +153,17 @@
                     for keyname, keyvals in metadata_keys.items():
                         if key in keyvals and not asn.get(keyname, ""):
                             asn[keyname] = value
         asn["emails"] = list(emails)
         asn["asn"] = str(asn_number)
         return asn
 
-    def get_asn_bgpview(self, ip):
+    async def get_asn_bgpview(self, ip):
         url = f"https://api.bgpview.io/ip/{ip}"
-        data = self.get_url(url, "ASN")
+        data = await self.get_url(url, "ASN")
         asns = []
         asns_tried = set()
         if data == False:
             return False
         data = data.get("data", {})
         prefixes = data.get("prefixes", [])
         for prefix in prefixes:
@@ -174,48 +173,48 @@
             if not (asn or subnet):
                 continue
             name = details.get("name") or prefix.get("name") or ""
             description = details.get("description") or prefix.get("description") or ""
             country = details.get("country_code") or prefix.get("country_code") or ""
             emails = []
             if not asn in asns_tried:
-                emails = self.get_emails_bgpview(asn)
+                emails = await self.get_emails_bgpview(asn)
                 if emails == False:
                     return False
                 asns_tried.add(asn)
             asns.append(
                 dict(asn=asn, subnet=subnet, name=name, description=description, country=country, emails=emails)
             )
         if not asns:
             self.debug(f'No results for "{ip}"')
         return asns
 
-    def get_emails_bgpview(self, asn):
+    async def get_emails_bgpview(self, asn):
         contacts = []
         url = f"https://api.bgpview.io/asn/{asn}"
-        data = self.get_url(url, "ASN metadata", cache=True)
+        data = await self.get_url(url, "ASN metadata", cache=True)
         if data == False:
             return False
         data = data.get("data", {})
         if not data:
             self.debug(f'No results for "{asn}"')
             return
         email_contacts = data.get("email_contacts", [])
         abuse_contacts = data.get("abuse_contacts", [])
         contacts = [l.strip().lower() for l in email_contacts + abuse_contacts]
         return list(set(contacts))
 
-    def get_url(self, url, data_type, cache=False):
+    async def get_url(self, url, data_type, cache=False):
         kwargs = {}
         if cache:
             kwargs["cache_for"] = 60 * 60 * 24
-        r = self.helpers.request(url, **kwargs)
+        r = await self.helpers.request(url, **kwargs)
         data = {}
         try:
             j = r.json()
             if not isinstance(j, dict):
                 return data
             return j
         except Exception as e:
-            self.verbose(f"Error retrieving {data_type} at {url}: {e}")
+            self.verbose(f"Error retrieving {data_type} at {url}: {e}", trace=True)
             self.debug(f"Got data: {getattr(r, 'content', '')}")
             return False
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1793rc0/bbot/modules/riddler.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     meta = {"description": "Query riddler.io for subdomains"}
 
     base_url = "https://riddler.io"
 
-    def request_url(self, query):
+    async def request_url(self, query):
         url = f"{self.base_url}/search/exportcsv?q=pld:{self.helpers.quote(query)}"
-        return self.request_with_fail_count(url)
+        response = await self.request_with_fail_count(url)
+        return response
 
     def parse_results(self, r, query):
         results = set()
         text = getattr(r, "text", "")
         for match in self.helpers.regexes.dns_name_regex.findall(text):
             match = match.lower()
             if match.endswith(query):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/robots.py` & `bbot-1.0.5.1793rc0/bbot/modules/robots.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,31 @@
         "include_sitemap": "Include 'sitemap' entries",
         "include_allow": "Include 'Allow' Entries",
         "include_disallow": "Include 'Disallow' Entries",
     }
 
     in_scope_only = True
 
-    def setup(self):
+    async def setup(self):
         self.scanned_hosts = set()
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         parsed_host = event.parsed
         host = f"{parsed_host.scheme}://{parsed_host.netloc}/"
         host_hash = hash(host)
         if host_hash in self.scanned_hosts:
             self.debug(f"Host {host} was already scanned, exiting")
             return
         else:
             self.scanned_hosts.add(host_hash)
 
         result = None
         url = f"{host}robots.txt"
-        result = self.helpers.request(url)
+        result = await self.helpers.request(url)
         if result:
             body = result.text
 
             if body:
                 lines = body.split("\n")
                 for l in lines:
                     if len(l) > 0:
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1793rc0/bbot/modules/secretsdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     }
     options_desc = {
         "min_confidence": "Only use signatures with this confidence score or higher",
         "signatures": "File path or URL to YAML signatures",
     }
     deps_pip = ["pyyaml~=6.0"]
 
-    def setup(self):
+    async def setup(self):
         self.rules = []
         self.min_confidence = self.config.get("min_confidence", 99)
-        self.sig_file = self.helpers.wordlist(self.config.get("signatures", ""))
+        self.sig_file = await self.helpers.wordlist(self.config.get("signatures", ""))
         with open(self.sig_file) as f:
             rules_yaml = yaml.safe_load(f).get("patterns", [])
         for r in rules_yaml:
             r = r.get("pattern", {})
             if not r:
                 continue
             name = r.get("name", "").lower()
@@ -37,28 +37,35 @@
                     compiled_regex = re.compile(regex)
                     r["regex"] = compiled_regex
                     self.rules.append(r)
                 except Exception:
                     self.debug(f"Error compiling regex: r'{regex}'")
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         resp_body = event.data.get("body", "")
         resp_headers = event.data.get("raw_header", "")
+        all_matches = await self.scan.run_in_executor(self.search_data, resp_body, resp_headers)
+        for matches, name in all_matches:
+            matches = [m.string[m.start() : m.end()] for m in matches]
+            description = f"Possible secret ({name}): {matches}"
+            event_data = {"host": str(event.host), "description": description}
+            parsed_url = getattr(event, "parsed", None)
+            if parsed_url:
+                event_data["url"] = parsed_url.geturl()
+            self.emit_event(
+                event_data,
+                "FINDING",
+                source=event,
+            )
+
+    def search_data(self, resp_body, resp_headers):
+        all_matches = []
         for r in self.rules:
             regex = r["regex"]
             name = r["name"]
             for text in (resp_body, resp_headers):
                 if text:
                     matches = list(regex.finditer(text))
                     if matches:
-                        matches = [m.string[m.start() : m.end()] for m in matches]
-                        description = f"Possible secret ({name}): {matches}"
-                        event_data = {"host": str(event.host), "description": description}
-                        parsed_url = getattr(event, "parsed", None)
-                        if parsed_url:
-                            event_data["url"] = parsed_url.geturl()
-                        self.emit_event(
-                            event_data,
-                            "FINDING",
-                            source=event,
-                        )
+                        all_matches.append((matches, name))
+        return all_matches
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1793rc0/bbot/modules/shodan_dns.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-from .shodan_dns import shodan_dns
+from .crobat import crobat
 
 
-class securitytrails(shodan_dns):
+class shodan_dns(crobat):
+    """
+    A typical module for authenticated, API-based subdomain enumeration
+    Inherited by several other modules including securitytrails, c99.nl, etc.
+    """
+
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the SecurityTrails API for subdomains", "auth_required": True}
+    meta = {"description": "Query Shodan for subdomains", "auth_required": True}
     options = {"api_key": ""}
-    options_desc = {"api_key": "SecurityTrails API key"}
+    options_desc = {"api_key": "Shodan API key"}
 
-    base_url = "https://api.securitytrails.com/v1"
+    base_url = "https://api.shodan.io"
 
-    def setup(self):
-        self.limit = 100
-        return super().setup()
+    async def setup(self):
+        await super().setup()
+        return await self.require_api_key()
 
-    def ping(self):
-        r = self.request_with_fail_count(f"{self.base_url}/ping?apikey={self.api_key}")
+    async def ping(self):
+        url = f"{self.base_url}/api-info?key={self.api_key}"
+        r = await self.request_with_fail_count(url)
         resp_content = getattr(r, "text", "")
         assert getattr(r, "status_code", 0) == 200, resp_content
 
-    def request_url(self, query):
-        url = f"{self.base_url}/domain/{query}/subdomains?apikey={self.api_key}"
-        return self.request_with_fail_count(url)
+    async def request_url(self, query):
+        url = f"{self.base_url}/dns/domain/{self.helpers.quote(query)}?key={self.api_key}"
+        response = await self.request_with_fail_count(url)
+        return response
 
     def parse_results(self, r, query):
-        j = r.json()
-        if isinstance(j, dict):
-            for host in j.get("subdomains", []):
-                yield f"{host}.{query}"
+        json = r.json()
+        if json:
+            for hostname in json.get("subdomains", []):
+                yield f"{hostname}.{query}"
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1793rc0/bbot/modules/securitytrails.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-from .crobat import crobat
+from .shodan_dns import shodan_dns
 
 
-class shodan_dns(crobat):
-    """
-    A typical module for authenticated, API-based subdomain enumeration
-    Inherited by several other modules including securitytrails, c99.nl, etc.
-    """
-
+class securitytrails(shodan_dns):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query Shodan for subdomains", "auth_required": True}
+    meta = {"description": "Query the SecurityTrails API for subdomains", "auth_required": True}
     options = {"api_key": ""}
-    options_desc = {"api_key": "Shodan API key"}
+    options_desc = {"api_key": "SecurityTrails API key"}
 
-    base_url = "https://api.shodan.io"
+    base_url = "https://api.securitytrails.com/v1"
 
-    def setup(self):
-        super().setup()
-        return self.require_api_key()
+    async def setup(self):
+        self.limit = 100
+        return await super().setup()
 
-    def ping(self):
-        r = self.request_with_fail_count(f"{self.base_url}/api-info?key={self.api_key}")
+    async def ping(self):
+        url = f"{self.base_url}/ping?apikey={self.api_key}"
+        r = await self.request_with_fail_count(url)
         resp_content = getattr(r, "text", "")
         assert getattr(r, "status_code", 0) == 200, resp_content
 
-    def request_url(self, query):
-        url = f"{self.base_url}/dns/domain/{self.helpers.quote(query)}?key={self.api_key}"
-        return self.request_with_fail_count(url)
+    async def request_url(self, query):
+        url = f"{self.base_url}/domain/{query}/subdomains?apikey={self.api_key}"
+        response = await self.request_with_fail_count(url)
+        return response
 
     def parse_results(self, r, query):
-        json = r.json()
-        if json:
-            for hostname in json.get("subdomains"):
-                yield f"{hostname}.{query}"
+        j = r.json()
+        if isinstance(j, dict):
+            for host in j.get("subdomains", []):
+                yield f"{host}.{query}"
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1793rc0/bbot/modules/skymem.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     watched_events = ["DNS_NAME"]
     produced_events = ["EMAIL_ADDRESS"]
     flags = ["passive", "email-enum", "safe"]
     meta = {"description": "Query skymem.info for email addresses"}
 
     base_url = "https://www.skymem.info"
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         _, query = self.helpers.split_domain(event.data)
         # get first page
         url = f"{self.base_url}/srch?q={self.helpers.quote(query)}"
-        r = self.request_with_fail_count(url)
+        r = await self.request_with_fail_count(url)
         if not r:
             return
-        for email in self.extract_emails(r.text):
+        for email in self.helpers.extract_emails(r.text):
             self.emit_event(email, "EMAIL_ADDRESS", source=event)
 
         # iterate through other pages
         domain_ids = re.findall(r'<a href="/domain/([a-z0-9]+)\?p=', r.text, re.I)
         if not domain_ids:
             return
         domain_id = domain_ids[0]
         for page in range(2, 22):
-            r2 = self.request_with_fail_count(f"{self.base_url}/domain/{domain_id}?p={page}")
+            r2 = await self.request_with_fail_count(f"{self.base_url}/domain/{domain_id}?p={page}")
             if not r2:
                 continue
-            for email in self.extract_emails(r2.text):
+            for email in self.helpers.extract_emails(r2.text):
                 self.emit_event(email, "EMAIL_ADDRESS", source=event)
             pages = re.findall(r"/domain/" + domain_id + r"\?p=(\d+)", r2.text)
             if not pages:
                 break
             last_page = max([int(p) for p in pages])
             if page >= last_page:
                 break
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1793rc0/bbot/modules/smuggler.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     deps_ansible = [
         {
             "name": "Get smuggler repo",
             "git": {"repo": "https://github.com/defparam/smuggler.git", "dest": "#{BBOT_TOOLS}/smuggler"},
         }
     ]
 
-    def setup(self):
+    async def setup(self):
         self.scanned_hosts = set()
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         host = f"{event.parsed.scheme}://{event.parsed.netloc}/"
         host_hash = hash(host)
         if host_hash in self.scanned_hosts:
             self.debug(f"Host {host} was already scanned, exiting")
             return
         else:
             self.scanned_hosts.add(host_hash)
@@ -40,15 +40,18 @@
             sys.executable,
             f"{self.scan.helpers.tools_dir}/smuggler/smuggler.py",
             "--no-color",
             "-q",
             "-u",
             event.data,
         ]
-        for f in self.helpers.run_live(command):
-            if "Issue Found" in f:
-                technique = f.split(":")[0].rstrip()
-                text = f.split(":")[1].split("-")[0].strip()
-                description = f"[HTTP SMUGGLER] [{text}] Technique: {technique}"
-                self.emit_event(
-                    {"host": str(event.host), "url": event.data, "description": description}, "FINDING", source=event
-                )
+        async for line in self.helpers.run_live(command):
+            for f in line.split("\r"):
+                if "Issue Found" in f:
+                    technique = f.split(":")[0].rstrip()
+                    text = f.split(":")[1].split("-")[0].strip()
+                    description = f"[HTTP SMUGGLER] [{text}] Technique: {technique}"
+                    self.emit_event(
+                        {"host": str(event.host), "url": event.data, "description": description},
+                        "FINDING",
+                        source=event,
+                    )
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/social.py` & `bbot-1.0.5.1793rc0/bbot/modules/social.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         "bitbucket": r"(?:https?:\/\/)?(?:www\.)?bitbucket\.org\/[a-zA-Z0-9_-]+\/?",
         "gitlab": r"(?:https?:\/\/)?(?:www\.)?gitlab\.com\/[a-zA-Z0-9_-]+\/?",
         "discord": r"(?:https?:\/\/)?(?:www\.)?discord\.gg\/[a-zA-Z0-9_-]+\/?",
     }
 
     scope_distance_modifier = 1
 
-    def setup(self):
+    async def setup(self):
         self.compiled_regexes = {k: re.compile(v) for k, v in self.social_media_regex.items()}
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         for platform, regex in self.compiled_regexes.items():
             for match in regex.findall(event.data):
                 social_media_links = {"platform": platform, "url": match}
                 self.emit_event(social_media_links, "SOCIAL", source=event)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1793rc0/bbot/modules/sslcert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,82 @@
-import select
-import socket
-import threading
-from OpenSSL import SSL
-from ssl import PROTOCOL_TLSv1
+import ssl
+import asyncio
+from OpenSSL import crypto
 from contextlib import suppress
 
 from bbot.modules.base import BaseModule
 from bbot.core.errors import ValidationError
-from bbot.core.helpers.threadpool import NamedLock
+from bbot.core.helpers.async_helpers import NamedLock
 
 
 class sslcert(BaseModule):
     watched_events = ["OPEN_TCP_PORT"]
     produced_events = ["DNS_NAME", "EMAIL_ADDRESS"]
     flags = ["affiliates", "subdomain-enum", "email-enum", "active", "safe", "web-basic", "web-thorough"]
     meta = {
         "description": "Visit open ports and retrieve SSL certificates",
     }
     options = {"timeout": 5.0, "skip_non_ssl": True}
     options_desc = {"timeout": "Socket connect timeout in seconds", "skip_non_ssl": "Don't try common non-SSL ports"}
     deps_apt = ["openssl"]
     deps_pip = ["pyOpenSSL~=23.1.1"]
-    max_threads = 50
     max_event_handlers = 25
     scope_distance_modifier = 1
     _priority = 2
 
-    def setup(self):
+    async def setup(self):
         self.timeout = self.config.get("timeout", 5.0)
         self.skip_non_ssl = self.config.get("skip_non_ssl", True)
         self.non_ssl_ports = (22, 53, 80)
 
         # sometimes we run into a server with A LOT of SANs
         # these are usually stupid and useless, so we abort based on a different threshold
         # depending on whether the source event is in scope
         self.in_scope_abort_threshold = 50
         self.out_of_scope_abort_threshold = 10
 
         self.hosts_visited = set()
-        self.hosts_visited_lock = threading.Lock()
         self.ip_lock = NamedLock()
         return True
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if self.skip_non_ssl and event.port in self.non_ssl_ports:
             return False, f"Port {event.port} doesn't typically use SSL"
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         _host = event.host
         if event.port:
             port = event.port
         else:
             port = 443
 
         # turn hostnames into IP address(es)
         if self.helpers.is_ip(_host):
             hosts = [_host]
         else:
-            hosts = list(self.helpers.resolve(_host))
-
-        futures = {}
-        for host in hosts:
-            future = self.submit_task(self.visit_host, host, port)
-            futures[future] = host
+            hosts = list(await self.helpers.resolve(_host))
 
         if event.scope_distance == 0:
             abort_threshold = self.in_scope_abort_threshold
             log_fn = self.info
         else:
             abort_threshold = self.out_of_scope_abort_threshold
             log_fn = self.verbose
-        for future in self.helpers.as_completed(futures):
-            host = futures[future]
-            result = future.result()
-            if not isinstance(result, tuple) or not len(result) == 2:
+
+        tasks = []
+        for host in hosts:
+            task = self.helpers.create_task(self.visit_host(host, port))
+            tasks.append(task)
+
+        for task in self.helpers.as_completed(tasks):
+            result = await task
+            if not isinstance(result, tuple) or not len(result) == 3:
                 continue
-            dns_names, emails = result
+            dns_names, emails, (host, port) = result
             if len(dns_names) > abort_threshold:
                 netloc = self.helpers.make_netloc(host, port)
                 log_fn(
                     f"Skipping Subject Alternate Names (SANs) on {netloc} because number of hostnames ({len(dns_names):,}) exceeds threshold ({abort_threshold})"
                 )
                 dns_names = dns_names[:1]
             for event_type, results in (("DNS_NAME", dns_names), ("EMAIL_ADDRESS", emails)):
@@ -96,81 +92,82 @@
                             self.debug(f"Invalid data at {host}:{port}: {e}")
 
     def on_success_callback(self, event):
         source_scope_distance = event.get_source().scope_distance
         if source_scope_distance == 0 and event.scope_distance > 0:
             event.add_tag("affiliate")
 
-    def visit_host(self, host, port):
+    async def visit_host(self, host, port):
         host = self.helpers.make_ip_type(host)
         netloc = self.helpers.make_netloc(host, port)
         host_hash = hash((host, port))
         dns_names = []
         emails = set()
-        with self.ip_lock.get_lock(host_hash):
-            with self.hosts_visited_lock:
-                if host_hash in self.hosts_visited:
-                    self.debug(f"Already processed {host} on port {port}, skipping")
-                    return [], []
-                else:
-                    self.hosts_visited.add(host_hash)
-
-            socket_type = socket.AF_INET
-            if self.helpers.is_ip(host):
-                if host.version == 6:
-                    socket_type = socket.AF_INET6
+        async with self.ip_lock.lock(host_hash):
+            if host_hash in self.hosts_visited:
+                self.debug(f"Already processed {host} on port {port}, skipping")
+                return [], [], (host, port)
+            else:
+                self.hosts_visited.add(host_hash)
+
             host = str(host)
+
+            # Create an SSL context
             try:
-                sock = socket.socket(socket_type, socket.SOCK_STREAM)
+                ssl_context = ssl.create_default_context()
+                ssl_context.check_hostname = False
+                ssl_context.verify_mode = ssl.CERT_NONE
+                ssl_context.options &= ~ssl.OP_NO_SSLv2 & ~ssl.OP_NO_SSLv3
+                ssl_context.set_ciphers("ALL:@SECLEVEL=0")
+                ssl_context.options |= 0x4  # Add the OP_LEGACY_SERVER_CONNECT option
             except Exception as e:
-                self.warning(f"Error creating socket for {netloc}: {e}. Do you have IPv6 disabled?")
-                return [], []
-            sock.settimeout(self.timeout)
-            try:
-                context = SSL.Context(PROTOCOL_TLSv1)
-            except AttributeError as e:
-                # AttributeError: module 'lib' has no attribute 'SSL_CTX_set_ecdh_auto'
                 self.warning(f"Error creating SSL context: {e}")
-                return [], []
-            self.debug(f"Connecting to {host} on port {port}")
+                return [], [], (host, port)
+
+            # Connect to the host
             try:
-                sock.connect((host, port))
+                transport, _ = await asyncio.wait_for(
+                    self.scan._loop.create_connection(lambda: asyncio.Protocol(), host, port, ssl=ssl_context),
+                    timeout=self.timeout,
+                )
+            except asyncio.TimeoutError:
+                self.debug(f"Timed out after {self.timeout} seconds while connecting to {netloc}")
+                return [], [], (host, port)
             except Exception as e:
-                self.debug(f"Error connecting to {host} on port {port}: {e}")
-                return [], []
-            connection = SSL.Connection(context, sock)
-            connection.set_tlsext_host_name(self.helpers.smart_encode(host))
-            connection.set_connect_state()
+                log_fn = self.warning
+                if isinstance(e, OSError):
+                    log_fn = self.debug
+                log_fn(f"Error connecting to {netloc}: {e}")
+                return [], [], (host, port)
+            finally:
+                with suppress(Exception):
+                    transport.close()
+
+            # Get the SSL object
             try:
-                while 1:
-                    try:
-                        connection.do_handshake()
-                    except SSL.WantReadError:
-                        rd, _, _ = select.select([sock], [], [], sock.gettimeout())
-                        if not rd:
-                            raise SSL.Error("select timed out")
-                        continue
-                    break
+                ssl_object = transport.get_extra_info("ssl_object")
             except Exception as e:
-                self.debug(f"Error with SSL handshake on {host} port {port}: {e}")
-                return [], []
-            cert = connection.get_peer_certificate()
-            sock.close()
+                self.verbose(f"Error getting ssl_object: {e}", trace=True)
+                return [], [], (host, port)
+
+            # Get the certificate
+            der = ssl_object.getpeercert(binary_form=True)
+            cert = crypto.load_certificate(crypto.FILETYPE_ASN1, der)
             issuer = cert.get_issuer()
             if issuer.emailAddress and self.helpers.regexes.email_regex.match(issuer.emailAddress):
                 emails.add(issuer.emailAddress)
             subject = cert.get_subject()
             if subject.emailAddress and self.helpers.regexes.email_regex.match(subject.emailAddress):
                 emails.add(subject.emailAddress)
             common_name = str(subject.commonName).lstrip("*.").lower()
             dns_names = set(self.get_cert_sans(cert))
             with suppress(KeyError):
                 dns_names.remove(common_name)
             dns_names = [common_name] + list(dns_names)
-        return dns_names, list(emails)
+        return dns_names, list(emails), (host, port)
 
     @staticmethod
     def get_cert_sans(cert):
         sans = []
         raw_sans = None
         ext_count = cert.get_extension_count()
         for i in range(0, ext_count):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1793rc0/bbot/modules/subdomain_hijack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 import json
-import requests
+import httpx
 
 from bbot.modules.base import BaseModule
 from bbot.core.helpers.misc import tldextract
 
 
 class subdomain_hijack(BaseModule):
     flags = ["subdomain-hijack", "subdomain-enum", "cloud-enum", "safe", "active", "web-basic", "web-thorough"]
@@ -14,17 +14,17 @@
     options = {
         "fingerprints": "https://raw.githubusercontent.com/EdOverflow/can-i-take-over-xyz/master/fingerprints.json"
     }
     options_desc = {"fingerprints": "URL or path to fingerprints.json"}
     scope_distance_modifier = 3
     max_event_handlers = 5
 
-    def setup(self):
+    async def setup(self):
         fingerprints_url = self.config.get("fingerprints")
-        fingerprints_file = self.helpers.wordlist(fingerprints_url)
+        fingerprints_file = await self.helpers.wordlist(fingerprints_url)
         with open(fingerprints_file) as f:
             fingerprints = json.load(f)
         self.fingerprints = []
         for f in fingerprints:
             try:
                 f = Fingerprint(f)
             except Exception as e:
@@ -36,16 +36,16 @@
             self.debug(f"Processed fingerprint: {f}")
             self.fingerprints.append(f)
         if not self.fingerprints:
             return None, "No valid fingerprints"
         self.debug(f"Successfully processed {len(self.fingerprints):,} fingerprints")
         return True
 
-    def handle_event(self, event):
-        hijackable, reason = self.check_subdomain(event)
+    async def handle_event(self, event):
+        hijackable, reason = await self.check_subdomain(event)
         if hijackable:
             source_hosts = []
             e = event
             while 1:
                 host = getattr(e, "host", "")
                 if host:
                     if e not in source_hosts:
@@ -62,58 +62,58 @@
                 for e in source_hosts[1:]:
                     source_hosts_str += f" -[{e.module.name}]-> {e.host}"
                 description += f" ({source_hosts_str})"
             self.emit_event({"host": event.host, "url": url, "description": description}, "FINDING", source=event)
         else:
             self.debug(reason)
 
-    def check_subdomain(self, event):
+    async def check_subdomain(self, event):
         for f in self.fingerprints:
             for domain in f.domains:
                 self_matches = self.helpers.host_in_host(event.data, domain)
                 child_matches = any(self.helpers.host_in_host(domain, h) for h in event.resolved_hosts)
                 if event.type == "DNS_NAME_UNRESOLVED":
                     if self_matches and f.nxdomain:
                         return True, "NXDOMAIN"
                 else:
                     if self_matches or child_matches:
                         for scheme in ("https", "http"):
                             if self.scan.stopping:
                                 return False, "Scan cancelled"
                             # first, try base request
                             url = f"{scheme}://{event.data}"
-                            match, reason = self._verify_fingerprint(f, url, cache_for=60 * 60 * 24)
+                            match, reason = await self._verify_fingerprint(f, url, cache_for=60 * 60 * 24)
                             if match:
                                 return match, reason
                             # next, try subdomain -[CNAME]-> other_domain
                             url = f"{scheme}://{domain}"
                             headers = {"Host": event.data}
-                            match, reason = self._verify_fingerprint(f, url, headers=headers)
+                            match, reason = await self._verify_fingerprint(f, url, headers=headers)
                             if match:
                                 return match, reason
         return False, f'Subdomain "{event.data}" not hijackable'
 
-    def _verify_fingerprint(self, fingerprint, *args, **kwargs):
+    async def _verify_fingerprint(self, fingerprint, *args, **kwargs):
         kwargs["raise_error"] = True
         kwargs["timeout"] = 10
         kwargs["retries"] = 0
         if fingerprint.http_status is not None:
             kwargs["allow_redirects"] = False
         try:
-            r = self.helpers.request(*args, **kwargs)
+            r = await self.helpers.request(*args, **kwargs)
             if fingerprint.http_status is not None and r.status_code == fingerprint.http_status:
                 return True, f"HTTP status == {fingerprint.http_status}"
             text = getattr(r, "text", "")
             if (
                 not fingerprint.nxdomain
                 and not fingerprint.http_status
                 and fingerprint.fingerprint_regex.findall(text)
             ):
                 return True, "Fingerprint match"
-        except requests.exceptions.RequestException as e:
+        except httpx.RequestError as e:
             if fingerprint.nxdomain and "Name or service not known" in str(e):
                 return True, f"NXDOMAIN"
         return False, "No match"
 
 
 class Fingerprint:
     def __init__(self, fingerprint):
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1793rc0/bbot/modules/telerik.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from bbot.modules.base import BaseModule
-from urllib.parse import urlparse
+import asyncio
 from sys import executable
+from urllib.parse import urlparse
+
+from bbot.modules.base import BaseModule
 
 
 class telerik(BaseModule):
     watched_events = ["URL"]
     produced_events = ["VULNERABILITY", "FINDING"]
     flags = ["active", "aggressive", "slow", "web-thorough"]
     meta = {"description": "Scan for critical Telerik vulnerabilities"}
@@ -152,30 +154,30 @@
                 "remote_src": True,
             },
         },
     ]
 
     max_event_handlers = 5
 
-    def setup(self):
+    async def setup(self):
         self.scanned_hosts = set()
         self.timeout = self.scan.config.get("httpx_timeout", 5)
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         host = f"{event.parsed.scheme}://{event.parsed.netloc}/"
         host_hash = hash(host)
         if host_hash in self.scanned_hosts:
             self.debug(f"Host {host} was already scanned, exiting")
             return
         else:
             self.scanned_hosts.add(host_hash)
 
         webresource = "Telerik.Web.UI.WebResource.axd?type=rau"
-        result = self.test_detector(event.data, webresource)
+        result, _ = await self.test_detector(event.data, webresource)
         if result:
             if "RadAsyncUpload handler is registered succesfully" in result.text:
                 self.debug(f"Detected Telerik instance (Telerik.Web.UI.WebResource.axd?type=rau)")
                 description = f"Telerik RAU AXD Handler detected"
                 self.emit_event(
                     {"host": str(event.host), "url": f"{event.data}{webresource}", "description": description},
                     "FINDING",
@@ -194,15 +196,15 @@
                                 str(root_tool_path / "RAU_crypto-master/RAU_crypto.py"),
                                 "-P",
                                 "C:\\\\Windows\\\\Temp",
                                 version,
                                 str(root_tool_path / "testfile.txt"),
                                 result.url,
                             ]
-                            output = self.helpers.run(command)
+                            output = await self.helpers.run(command)
                             description = f"[CVE-2017-11317] [{str(version)}] {webresource}"
                             if "fileInfo" in output.stdout:
                                 self.debug(f"Confirmed Vulnerable Telerik (version: {str(version)}")
                                 self.emit_event(
                                     {
                                         "severity": "CRITICAL",
                                         "description": description,
@@ -210,57 +212,57 @@
                                         "url": f"{event.data}{webresource}",
                                     },
                                     "VULNERABILITY",
                                     event,
                                 )
                                 break
 
-        futures = {}
+        tasks = []
         for dh in self.DialogHandlerUrls:
-            future = self.submit_task(self.test_detector, event.data, f"{dh}?dp=1")
-            futures[future] = dh
+            tasks.append(self.helpers.create_task(self.test_detector(event.data, f"{dh}?dp=1")))
 
         fail_count = 0
-        for future in self.helpers.as_completed(futures):
-            dh = futures[future]
-            result = future.result()
+        for task in self.helpers.as_completed(tasks):
+            try:
+                result, dh = await task
+            except asyncio.CancelledError:
+                continue
 
             # cancel if we run into timeouts etc.
             if result is None:
                 fail_count += 1
 
                 # tolerate some random errors
                 if fail_count < 2:
                     continue
                 self.debug(f"Cancelling run against {event.data} due to failed request")
-                for future in futures:
-                    future.cancel()
+                await self.helpers.cancel_tasks(tasks)
                 break
-            if result:
+            else:
                 if "Cannot deserialize dialog parameters" in result.text:
-                    for future in futures:
-                        future.cancel()
-
+                    await self.helpers.cancel_tasks(tasks)
                     self.debug(f"Detected Telerik UI instance ({dh})")
                     description = f"Telerik DialogHandler detected"
                     self.emit_event(
                         {"host": str(event.host), "url": f"{event.data}{dh}", "description": description},
                         "FINDING",
                         event,
                     )
-                # Once we have a match we need to stop, because the basic handler (Telerik.Web.UI.DialogHandler.aspx) usually works with a path wildcard
-                break
+                    # Once we have a match we need to stop, because the basic handler (Telerik.Web.UI.DialogHandler.aspx) usually works with a path wildcard
+                    break
+
+        await self.helpers.cancel_tasks(tasks)
 
         spellcheckhandler = "Telerik.Web.UI.SpellCheckHandler.axd"
-        result = self.test_detector(event.data, spellcheckhandler)
+        result, _ = await self.test_detector(event.data, spellcheckhandler)
         try:
             # The standard behavior for the spellcheck handler without parameters is a 500
             if result.status_code == 500:
                 # Sometimes webapps will just return 500 for everything, so rule out the false positive
-                validate_result = self.test_detector(event.data, self.helpers.rand_string())
+                validate_result, _ = await self.test_detector(event.data, self.helpers.rand_string())
                 self.debug(validate_result)
                 if validate_result.status_code != 500:
                     self.debug(f"Detected Telerik UI instance (Telerik.Web.UI.SpellCheckHandler.axd)")
                     description = f"Telerik SpellCheckHandler detected"
                     self.emit_event(
                         {
                             "host": str(event.host),
@@ -269,21 +271,21 @@
                         },
                         "FINDING",
                         event,
                     )
         except Exception:
             pass
 
-    def test_detector(self, baseurl, detector):
+    async def test_detector(self, baseurl, detector):
         result = None
         if "/" != baseurl[-1]:
             url = f"{baseurl}/{detector}"
         else:
             url = f"{baseurl}{detector}"
-        result = self.helpers.request(url, timeout=self.timeout)
-        return result
+        result = await self.helpers.request(url, timeout=self.timeout)
+        return result, detector
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         if "endpoint" in event.tags:
             return False
         else:
             return True
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1793rc0/bbot/modules/threatminer.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,13 +7,15 @@
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {
         "description": "Query threatminer's API for subdomains",
     }
 
     base_url = "https://api.threatminer.org/v2"
 
-    def request_url(self, query):
-        return self.request_with_fail_count(f"{self.base_url}/domain.php?q={self.helpers.quote(query)}&rt=5")
+    async def request_url(self, query):
+        url = f"{self.base_url}/domain.php?q={self.helpers.quote(query)}&rt=5"
+        r = await self.request_with_fail_count(url, timeout=self.http_timeout + 30)
+        return r
 
     def parse_results(self, r, query):
         j = r.json()
-        yield from j.get("results", [])
+        return list(j.get("results", []))
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1793rc0/bbot/modules/url_manipulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     in_scope_only = True
 
     options = {"allow_redirects": True}
     options_desc = {
         "allow_redirects": "Allowing redirects will sometimes create false positives. Disallowing will sometimes create false negatives. Allowed by default."
     }
 
-    def setup(self):
+    async def setup(self):
         # ([string]method,[string]path,[bool]strip trailing slash)
         self.signatures = []
 
         self.rand_string = self.helpers.rand_string()
 
         # Test for abuse of extension based routing
         extensions = [
@@ -34,30 +34,30 @@
         ]
         for ext in extensions:
             self.signatures.append(("GET", "{scheme}://{netloc}/{path}?%s=%s" % (self.rand_string, ext), False))
 
         self.allow_redirects = self.config.get("allow_redirects", True)
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         try:
             compare_helper = self.helpers.http_compare(
                 event.data, allow_redirects=self.allow_redirects, include_cache_buster=False
             )
         except HttpCompareError as e:
             self.debug(e)
             return
 
         if compare_helper.canary_check(event.data, mode="getparam") == False:
             self.verbose(f'Aborting "{event.data}" due to failed canary check')
             return
 
         for sig in self.signatures:
             sig = self.format_signature(sig, event)
-            match, reasons, reflection, subject_response = compare_helper.compare(
+            match, reasons, reflection, subject_response = await compare_helper.compare(
                 sig[1], method=sig[0], allow_redirects=self.allow_redirects
             )
 
             if subject_response:
                 subject_content = "".join([str(x) for x in subject_response.headers])
                 if subject_response.text != None:
                     subject_content += subject_response.text
@@ -74,15 +74,15 @@
                                     source=event,
                                 )
                         else:
                             self.debug(f"Status code changed to {str(subject_response.status_code)}, ignoring")
                 else:
                     self.debug("Ignoring positive result due to presence of parameter name in result")
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         accepted_status_codes = ["200", "301", "302"]
 
         for c in accepted_status_codes:
             if f"status-{c}" in event.tags:
                 return True
         return False
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1793rc0/bbot/modules/urlscan.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,21 @@
         "description": "Query urlscan.io for subdomains",
     }
     options = {"urls": False}
     options_desc = {"urls": "Emit URLs in addition to DNS_NAMEs"}
 
     base_url = "https://urlscan.io/api/v1"
 
-    def setup(self):
+    async def setup(self):
         self.urls = self.config.get("urls", False)
-        return super().setup()
+        return await super().setup()
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        for domain, url in self.query(query):
+        for domain, url in await self.query(query):
             source_event = event
             if domain and domain != query:
                 domain_event = self.make_event(domain, "DNS_NAME", source=event)
                 if domain_event:
                     if str(domain_event.host).endswith(query) and not str(domain_event.host) == str(event.host):
                         self.emit_event(domain_event, abort_if=self.abort_if)
                         source_event = domain_event
@@ -34,30 +34,33 @@
                         if self.urls:
                             self.emit_event(url_event, abort_if=self.abort_if)
                         else:
                             self.emit_event(str(url_event.host), "DNS_NAME", source=event, abort_if=self.abort_if)
                     else:
                         self.debug(f"{url_event.host} does not match {query}")
 
-    def query(self, query):
-        results = self.helpers.request(f"{self.base_url}/search/?q={self.helpers.quote(query)}")
+    async def query(self, query):
+        results = set()
+        url = f"{self.base_url}/search/?q={self.helpers.quote(query)}"
+        r = await self.helpers.request(url)
         try:
-            json = results.json()
+            json = r.json()
             if json and type(json) == dict:
                 for result in json.get("results", []):
                     if result and type(result) == dict:
                         task = result.get("task", {})
                         if task and type(task) == dict:
                             domain = task.get("domain", "")
                             url = task.get("url", "")
                             if domain or url:
-                                yield domain, url
+                                results.add((domain, url))
                         page = result.get("page", {})
                         if page and type(page) == dict:
                             domain = page.get("domain", "")
                             url = page.get("url", "")
                             if domain or url:
-                                yield domain, url
+                                results.add((domain, url))
             else:
                 self.debug(f'No results for "{query}"')
         except Exception:
             self.verbose(f"Error retrieving urlscan results")
+        return results
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1793rc0/bbot/modules/viewdns.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from bs4 import BeautifulSoup
 
 from bbot.modules.base import BaseModule
 
 
 class viewdns(BaseModule):
     """
     Used as a base for modules that only act on root domains and not individual hostnames
@@ -11,57 +10,61 @@
 
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "passive", "safe"]
     meta = {
         "description": "Query viewdns.info's reverse whois for related domains",
     }
-    deps_pip = ["bs4", "lxml~=4.9.2"]
     base_url = "https://viewdns.info"
     in_scope_only = True
     _qsize = 1
 
-    def setup(self):
+    async def setup(self):
         self.processed = set()
         self.date_regex = re.compile(r"\d{4}-\d{2}-\d{2}")
         return True
 
-    def filter_event(self, event):
+    async def filter_event(self, event):
         _, domain = self.helpers.split_domain(event.data)
         if hash(domain) in self.processed:
             return False
         self.processed.add(hash(domain))
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         _, query = self.helpers.split_domain(event.data)
-        for domain, _ in self.query(query):
+        for domain, _ in await self.query(query):
             self.emit_event(domain, "DNS_NAME", source=event, tags=["affiliate"])
             # todo: registrar?
 
-    def query(self, query):
+    async def query(self, query):
+        results = set()
         url = f"{self.base_url}/reversewhois/?q={query}"
-        r = self.helpers.request(url)
+        r = await self.helpers.request(url)
         status_code = getattr(r, "status_code", 0)
         if status_code not in (200,):
             self.verbose(f"Error retrieving reverse whois results (status code: {status_code})")
 
         content = getattr(r, "content", b"")
-        html = BeautifulSoup(content, features="lxml")
-        yielded = set()
+        from bs4 import BeautifulSoup
+
+        html = BeautifulSoup(content, "html.parser")
+        found = set()
         for table_row in html.findAll("tr"):
             table_cells = table_row.findAll("td")
             # make double-sure we're in the right table by checking the date field
             try:
                 if self.date_regex.match(table_cells[1].text.strip()):
                     # domain == first cell
                     domain = table_cells[0].text.strip().lower()
                     # registrar == last cell
                     registrar = table_cells[-1].text.strip()
                     if domain and not domain == query:
-                        to_yield = (domain, registrar)
-                        to_yield_hash = hash(to_yield)
-                        if to_yield_hash not in yielded:
-                            yield to_yield
+                        result = (domain, registrar)
+                        result_hash = hash(result)
+                        if result_hash not in found:
+                            found.add(result_hash)
+                            results.add(result)
             except IndexError:
                 self.debug(f"Invalid row {str(table_row)[:40]}...")
                 continue
+        return results
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1793rc0/bbot/modules/wafw00f.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,34 +15,35 @@
     deps_pip = ["wafw00f~=2.2.0"]
 
     options = {"generic_detect": True}
     options_desc = {"generic_detect": "When no specific WAF detections are made, try to peform a generic detect"}
 
     in_scope_only = True
 
-    def setup(self):
+    async def setup(self):
         self.scanned_hosts = set()
         return True
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         parsed_host = event.parsed
         host = f"{parsed_host.scheme}://{parsed_host.netloc}/"
         host_hash = hash(host)
         if host_hash in self.scanned_hosts:
             self.debug(f"Host {host} was already scanned, exiting")
             return
         else:
             self.scanned_hosts.add(host_hash)
 
-        WW = wafw00f_main.WAFW00F(host)
-        waf_detections = WW.identwaf()
+        WW = await self.scan.run_in_executor(wafw00f_main.WAFW00F, host)
+        waf_detections = await self.scan.run_in_executor(WW.identwaf)
         if waf_detections:
-            for waf in WW.identwaf():
+            for waf in waf_detections:
                 self.emit_event({"host": host, "WAF": waf}, "WAF", source=event)
         else:
             if self.config.get("generic_detect") == True:
-                if WW.genericdetect():
+                generic = await self.scan.run_in_executor(WW.genericdetect)
+                if generic:
                     self.emit_event(
                         {"host": host, "WAF": "generic detection", "info": WW.knowledge["generic"]["reason"]},
                         "WAF",
                         source=event,
                     )
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1793rc0/bbot/modules/wappalyzer.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,20 +18,20 @@
         "description": "Extract technologies from web responses",
     }
     deps_pip = ["python-Wappalyzer~=0.3.1"]
     # accept all events regardless of scope distance
     scope_distance_modifier = None
     max_event_handlers = 5
 
-    def setup(self):
-        self.wappalyzer = Wappalyzer.latest()
+    async def setup(self):
+        self.wappalyzer = await self.scan.run_in_executor(Wappalyzer.latest)
         return True
 
-    def handle_event(self, event):
-        for res in self.wappalyze(event.data):
+    async def handle_event(self, event):
+        for res in await self.scan.run_in_executor(self.wappalyze, event.data):
             self.emit_event(
                 {"technology": res.lower(), "url": event.data["url"], "host": str(event.host)}, "TECHNOLOGY", event
             )
 
     def wappalyze(self, data):
         w = WebPage(url=data["url"], html=data.get("body", ""), headers=data.get("header-dict", {}))
         return self.wappalyzer.analyze(w)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1793rc0/bbot/modules/wayback.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,28 @@
         "urls": "emit URLs in addition to DNS_NAMEs",
         "garbage_threshold": "Dedupe similar urls if they are in a group of this size or higher (lower values == less garbage data)",
     }
     in_scope_only = True
 
     base_url = "http://web.archive.org"
 
-    def setup(self):
+    async def setup(self):
         self.urls = self.config.get("urls", False)
         self.garbage_threshold = self.config.get("garbage_threshold", 10)
-        return super().setup()
+        return await super().setup()
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        for result, event_type in self.query(query):
+        for result, event_type in await self.query(query):
             self.emit_event(result, event_type, event, abort_if=self.abort_if)
 
-    def query(self, query):
+    async def query(self, query):
+        results = set()
         waybackurl = f"{self.base_url}/cdx/search/cdx?url={self.helpers.quote(query)}&matchType=domain&output=json&fl=original&collapse=original"
-        r = self.helpers.request(waybackurl, timeout=self.http_timeout + 10)
+        r = await self.helpers.request(waybackurl, timeout=self.http_timeout + 10)
         if not r:
             self.warning(f'Error connecting to archive.org for query "{query}"')
             return
         try:
             j = r.json()
             assert type(j) == list
         except Exception:
@@ -51,10 +52,11 @@
         dns_names = set()
         for parsed_url in self.helpers.collapse_urls(urls, threshold=self.garbage_threshold):
             if not self.urls:
                 dns_name = parsed_url.hostname
                 h = hash(dns_name)
                 if h not in dns_names:
                     dns_names.add(h)
-                    yield dns_name, "DNS_NAME"
+                    results.add((dns_name, "DNS_NAME"))
             else:
-                yield parsed_url.geturl(), "URL_UNVERIFIED"
+                results.add((parsed_url.geturl(), "URL_UNVERIFIED"))
+        return results
```

### Comparing `bbot-1.0.5.1665rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1793rc0/bbot/modules/zoomeye.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,42 +11,51 @@
         "api_key": "ZoomEye API key",
         "max_pages": "How many pages of results to fetch",
         "include_related": "Include domains which may be related to the target",
     }
 
     base_url = "https://api.zoomeye.org"
 
-    def setup(self):
+    async def setup(self):
         self.max_pages = self.config.get("max_pages", 20)
         self.headers = {"API-KEY": self.config.get("api_key", "")}
         self.include_related = self.config.get("include_related", False)
-        return super().setup()
+        return await super().setup()
 
-    def ping(self):
-        r = self.helpers.request(f"{self.base_url}/resources-info", headers=self.headers)
+    async def ping(self):
+        url = f"{self.base_url}/resources-info"
+        r = await self.helpers.request(url, headers=self.headers)
         assert int(r.json()["quota_info"]["remain_total_quota"]) > 0, "No quota remaining"
 
-    def handle_event(self, event):
+    async def handle_event(self, event):
         query = self.make_query(event)
-        results = self.query(query)
+        results = await self.query(query)
         if results:
             for hostname in results:
                 if hostname == event:
                     continue
                 tags = []
                 if not hostname.endswith(f".{query}"):
                     tags = ["affiliate"]
                 self.emit_event(hostname, "DNS_NAME", event, tags=tags)
 
-    def query(self, query):
+    async def query(self, query):
+        results = set()
         query_type = 0 if self.include_related else 1
         url = f"{self.base_url}/domain/search?q={self.helpers.quote(query)}&type={query_type}&page=" + "{page}"
-        for i, j in enumerate(self.helpers.api_page_iter(url, headers=self.headers)):
-            results = list(self.parse_results(j))
-            if results:
-                yield from results
-            if not results or i >= (self.max_pages - 1) or self.scan.stopping:
-                break
+        i = 0
+        agen = self.helpers.api_page_iter(url, headers=self.headers)
+        try:
+            async for j in agen:
+                r = list(self.parse_results(j))
+                if r:
+                    results.update(set(r))
+                if not r or i >= (self.max_pages - 1):
+                    break
+                i += 1
+        finally:
+            agen.aclose()
+        return results
 
     def parse_results(self, r):
         for entry in r.get("list", []):
             yield entry["name"]
```

### Comparing `bbot-1.0.5.1665rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1793rc0/bbot/scanner/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,80 @@
-import queue
+import asyncio
 import logging
-import threading
 import traceback
-from time import sleep
 from contextlib import suppress
-from datetime import datetime, timedelta
 
-from ..core.helpers.queueing import EventQueue
-from ..core.errors import ScanCancelledError, ValidationError
+from ..core.errors import ValidationError
+from ..core.helpers.async_helpers import TaskCounter
 
 log = logging.getLogger("bbot.scanner.manager")
 
 
 class ScanManager:
     """
     Manages modules and events during a scan
     """
 
     def __init__(self, scan):
         self.scan = scan
-        self.incoming_event_queue = EventQueue()
+
+        self.incoming_event_queue = asyncio.PriorityQueue()
 
         # tracks duplicate events on a global basis
         self.events_distributed = set()
-
         # tracks duplicate events on a per-module basis
         self.events_accepted = set()
-        self.events_accepted_lock = threading.Lock()
-
-        self._lock = threading.Lock()
-        self.event_emitted = threading.Condition(self._lock)
-
-        self.events_resolved = dict()
         self.dns_resolution = self.scan.config.get("dns_resolution", False)
+        self._task_counter = TaskCounter()
+        self._new_activity = True
+        self._modules_by_priority = None
+        self._incoming_queues = None
+        self._module_priority_weights = None
 
-        self.status_frequency = self.scan.config.get("status_frequency", 15)
-
-        self.last_log_time = datetime.now()
-
-    def init_events(self):
+    async def init_events(self):
         """
         seed scanner with target events
         """
-        self.distribute_event(self.scan.root_event)
-        sorted_events = sorted(self.scan.target.events, key=lambda e: len(e.data))
-        for event in sorted_events:
-            self.scan.verbose(f"Target: {event}")
-            self.emit_event(event, _block=False, _force_submit=True)
-        # force submit batches
-        for mod in self.scan.modules.values():
-            mod._handle_batch(force=True)
+        async with self.scan.acatch(context=self.init_events):
+            with self._task_counter:
+                await self.distribute_event(self.scan.root_event)
+                sorted_events = sorted(self.scan.target.events, key=lambda e: len(e.data))
+                for event in sorted_events:
+                    self.scan.verbose(f"Target: {event}")
+                    self.queue_event(event)
+                await asyncio.sleep(0.1)
+                self.scan._finished_init = True
 
-    def emit_event(self, event, *args, **kwargs):
+    async def emit_event(self, event, *args, **kwargs):
         """
         TODO: Register + kill duplicate events immediately?
         bbot.scanner: scan._event_thread_pool: running for 0 seconds: ScanManager._emit_event(DNS_NAME("sipfed.online.lync.com"))
         bbot.scanner: scan._event_thread_pool: running for 0 seconds: ScanManager._emit_event(DNS_NAME("sipfed.online.lync.com"))
         bbot.scanner: scan._event_thread_pool: running for 0 seconds: ScanManager._emit_event(DNS_NAME("sipfed.online.lync.com"))
         """
-        # skip event if it fails precheck
-        if not self._event_precheck(event):
-            event._resolved.set()
-            return False
+        with self._task_counter:
+            # skip event if it fails precheck
+            if not self._event_precheck(event):
+                event._resolved.set()
+                return
 
-        # "quick" queues the event immediately
-        quick = kwargs.pop("quick", False)
-        if quick:
             log.debug(f'Module "{event.module}" raised {event}')
-            event._resolved.set()
-            for kwarg in ["abort_if", "on_success_callback", "_block"]:
-                kwargs.pop(kwarg, None)
-            try:
-                self.distribute_event(event, *args, **kwargs)
-                return True
-            except ScanCancelledError:
-                return False
-            except Exception as e:
-                log.error(f"Unexpected error in manager.emit_event(): {e}")
-                log.trace(traceback.format_exc())
-        else:
-            # don't raise an exception if the thread pool has been shutdown
-            try:
-                self.scan._event_thread_pool.submit_task(self.catch, self._emit_event, event, *args, **kwargs)
+
+            # "quick" queues the event immediately
+            quick = kwargs.pop("quick", False)
+            if quick:
                 log.debug(f'Module "{event.module}" raised {event}')
-                return True
-            except ScanCancelledError:
-                return False
-            except queue.Full:
-                raise
-            except Exception as e:
-                log.error(f"Unexpected error in manager.emit_event(): {e}")
-                log.trace(traceback.format_exc())
-            finally:
                 event._resolved.set()
-        return False
+                for kwarg in ["abort_if", "on_success_callback"]:
+                    kwargs.pop(kwarg, None)
+                async with self.scan.acatch(context=self.distribute_event):
+                    await self.distribute_event(event, *args, **kwargs)
+            else:
+                async with self.scan.acatch(context=self._emit_event, finally_callback=event._resolved.set):
+                    await self._emit_event(event, *args, **kwargs)
 
     def _event_precheck(self, event, exclude=("DNS_NAME",)):
         """
         Check an event previous to its DNS resolution etc. to see if we can save on performance by skipping it
         """
         if event._dummy:
             log.warning(f"Cannot emit dummy event: {event}")
@@ -106,15 +83,15 @@
             log.debug(f"Skipping event with self as source: {event}")
             return False
         if not event._force_output and self.is_duplicate_event(event):
             log.debug(f"Skipping {event} because it is a duplicate")
             return False
         return True
 
-    def _emit_event(self, event, *args, **kwargs):
+    async def _emit_event(self, event, *args, **kwargs):
         log.debug(f"Emitting {event}")
         distribute_event = True
         event_distributed = False
         try:
             on_success_callback = kwargs.pop("on_success_callback", None)
             abort_if = kwargs.pop("abort_if", None)
 
@@ -130,15 +107,15 @@
             else:
                 # DNS resolution
                 (
                     dns_tags,
                     event_whitelisted_dns,
                     event_blacklisted_dns,
                     dns_children,
-                ) = self.scan.helpers.dns.resolve_event(event, minimal=not self.dns_resolution)
+                ) = await self.scan.helpers.dns.resolve_event(event, minimal=not self.dns_resolution)
                 resolved_hosts = set()
                 for rdtype, ips in dns_children.items():
                     if rdtype in ("A", "AAAA", "CNAME"):
                         for ip in ips:
                             resolved_hosts.add(ip)
 
             # kill runaway DNS chains
@@ -177,69 +154,81 @@
             if event.type == "DNS_NAME" and "unresolved" in event.tags and not "target" in event.tags:
                 event.type = "DNS_NAME_UNRESOLVED"
 
             # Cloud tagging
             for provider in self.scan.helpers.cloud.providers.values():
                 provider.tag_event(event)
 
+            event_is_duplicate = self.is_duplicate_event(event)
+
             # Scope shepherding
+            # here, we buff or nerf an event based on its attributes and certain scan settings
             event_is_duplicate = self.is_duplicate_event(event)
             event_in_report_distance = event.scope_distance <= self.scan.scope_report_distance
             set_scope_distance = event.scope_distance
             if event_whitelisted:
                 set_scope_distance = 0
             if event.host:
-                if (event_whitelisted or event_in_report_distance) and (event._force_output or not event_is_duplicate):
+                # here, we evaluate some weird logic
+                # the reason this exists is to ensure we don't have orphans in the graph
+                # because forcefully internalizing certain events can orphan their children
+                event_will_be_output = event_whitelisted or event_in_report_distance
+                event_is_duplicate = event_is_duplicate and not event._force_output
+                if event_will_be_output and not event_is_duplicate:
                     if set_scope_distance == 0:
                         log.debug(f"Making {event} in-scope")
-                    source_trail = event.make_in_scope(set_scope_distance)
+                    source_trail = event.set_scope_distance(set_scope_distance)
+                    # force re-emit internal source events
                     for s in source_trail:
-                        self.emit_event(s, _block=False, _force_submit=True)
+                        await self.emit_event(s, _block=False, _force_submit=True)
                 else:
                     if event.scope_distance > self.scan.scope_report_distance:
                         log.debug(
                             f"Making {event} internal because its scope_distance ({event.scope_distance}) > scope_report_distance ({self.scan.scope_report_distance})"
                         )
                         event.make_internal()
 
             # check for wildcards
             if event.scope_distance <= self.scan.scope_search_distance:
                 if not "unresolved" in event.tags:
                     if not self.scan.helpers.is_ip_type(event.host):
-                        self.scan.helpers.dns.handle_wildcard_event(event, dns_children)
+                        await self.scan.helpers.dns.handle_wildcard_event(event, dns_children)
 
             # now that the event is properly tagged, we can finally make decisions about it
+            abort_result = False
             if callable(abort_if):
-                abort_result = abort_if(event)
+                async with self.scan.acatch(context=abort_if):
+                    abort_result = await self.scan.helpers.execute_sync_or_async(abort_if, event)
                 msg = f"{event.module}: not raising event {event} due to custom criteria in abort_if()"
                 with suppress(ValueError, TypeError):
                     abort_result, reason = abort_result
                     msg += f": {reason}"
                 if abort_result:
                     log.debug(msg)
                     return
 
             if not self.accept_event(event):
                 return
 
             # run success callback before distributing event (so it can add tags, etc.)
             if distribute_event:
                 if callable(on_success_callback):
-                    self.catch(on_success_callback, event)
+                    async with self.scan.acatch(context=on_success_callback):
+                        await self.scan.helpers.execute_sync_or_async(on_success_callback, event)
 
             if not event.host or (event.always_emit and not event_is_duplicate):
                 log.debug(
-                    f"Force-emitting {event} because it does not have identifying scope information or because always_emit was True"
+                    f"Force-emitting {event} (host:{event.host}, always_emit={event.always_emit}, is_duplicate={event_is_duplicate})"
                 )
                 source_trail = event.unmake_internal(force_output=True)
                 for s in source_trail:
-                    self.emit_event(s, _block=False, _force_submit=True)
+                    self.queue_event(s)
 
             if distribute_event:
-                self.distribute_event(event)
+                await self.distribute_event(event)
                 event_distributed = True
 
             # speculate DNS_NAMES and IP_ADDRESSes from other event types
             source_event = event
             if (
                 event.host
                 and event.type not in ("DNS_NAME", "DNS_NAME_UNRESOLVED", "IP_ADDRESS", "IP_RANGE")
@@ -249,25 +238,25 @@
                 source_module._priority = 4
                 source_event = self.scan.make_event(event.host, "DNS_NAME", module=source_module, source=event)
                 # only emit the event if it's not already in the parent chain
                 if source_event is not None and source_event not in source_event.get_sources():
                     source_event.scope_distance = event.scope_distance
                     if "target" in event.tags:
                         source_event.add_tag("target")
-                    self.emit_event(source_event, _block=False, _force_submit=True)
+                    self.queue_event(source_event)
 
             ### Emit DNS children ###
             if self.dns_resolution:
                 emit_children = -1 < event.scope_distance < self.scan.dns_search_distance
                 if emit_children:
+                    # only emit DNS children once for each unique host
                     host_hash = hash(str(event.host))
-                    with self.events_accepted_lock:
-                        if host_hash in self.events_accepted:
-                            emit_children = False
-                        self.events_accepted.add(host_hash)
+                    if host_hash in self.events_accepted:
+                        emit_children = False
+                    self.events_accepted.add(host_hash)
 
                 if emit_children:
                     dns_child_events = []
                     if dns_children:
                         for rdtype, records in dns_children.items():
                             module = self.scan.helpers.dns._get_dummy_module(rdtype)
                             module._priority = 4
@@ -278,26 +267,24 @@
                                     )
                                     dns_child_events.append(child_event)
                                 except ValidationError as e:
                                     log.warning(
                                         f'Event validation failed for DNS child of {source_event}: "{record}" ({rdtype}): {e}'
                                     )
                     for child_event in dns_child_events:
-                        self.emit_event(child_event, _block=False, _force_submit=True)
+                        self.queue_event(child_event)
 
         except ValidationError as e:
             log.warning(f"Event validation failed with args={args}, kwargs={kwargs}: {e}")
             log.trace(traceback.format_exc())
 
         finally:
             event._resolved.set()
             if event_distributed:
                 self.scan.stats.event_distributed(event)
-            with self.event_emitted:
-                self.event_emitted.notify()
             log.debug(f"{event.module}.emit_event() finished for {event}")
 
     def hash_event(self, event):
         """
         Hash an event for duplicate detection
 
         This is necessary because duplicate events from certain sources (e.g. DNS)
@@ -312,204 +299,159 @@
 
     def is_duplicate_event(self, event, add=False):
         """
         Calculate whether an event is a duplicate on a per-module basis
         """
         event_hash = self.hash_event(event)
         suppress_dupes = getattr(event.module, "suppress_dupes", True)
-        with self.events_accepted_lock:
-            duplicate_event = suppress_dupes and event_hash in self.events_accepted
-            if add:
-                self.events_accepted.add(event_hash)
+        duplicate_event = suppress_dupes and event_hash in self.events_accepted
+        if add:
+            self.events_accepted.add(event_hash)
         return duplicate_event
 
     def accept_event(self, event):
         is_duplicate = self.is_duplicate_event(event, add=True)
         if is_duplicate and not event._force_output:
             log.debug(f"{event.module}: not raising duplicate event {event}")
             return False
         return True
 
-    def catch(self, callback, *args, **kwargs):
-        """
-        Wrapper to ensure error messages get surfaced to the user
-        """
-        ret = None
-        on_finish_callback = kwargs.pop("_on_finish_callback", None)
-        force = kwargs.pop("_force", False)
-        fn = callback
-        for arg in args:
-            if callable(arg):
-                fn = arg
-            else:
-                break
-        try:
-            if not self.scan.stopping or force:
-                ret = callback(*args, **kwargs)
-        except ScanCancelledError as e:
-            log.debug(f"ScanCancelledError in {fn.__qualname__}(): {e}")
-        except BrokenPipeError as e:
-            log.debug(f"BrokenPipeError in {fn.__qualname__}(): {e}")
-        except Exception as e:
-            log.error(f"Error in {fn.__qualname__}(): {e}")
-            log.trace(traceback.format_exc())
-        except KeyboardInterrupt:
-            log.debug(f"Interrupted")
-            self.scan.stop()
-        if callable(on_finish_callback):
-            try:
-                on_finish_callback()
-            except Exception as e:
-                log.error(
-                    f"Error in on_finish_callback {on_finish_callback.__qualname__}() after {fn.__qualname__}(): {e}"
-                )
-                log.trace(traceback.format_exc())
-        return ret
+    async def _register_running(self, callback, *args, **kwargs):
+        with self._task_counter:
+            return await callback(*args, **kwargs)
 
-    def distribute_event(self, *args, **kwargs):
+    async def distribute_event(self, *args, **kwargs):
         """
         Queue event with modules
         """
-        event = self.scan.make_event(*args, **kwargs)
-
-        event_hash = hash(event)
-        dup = event_hash in self.events_distributed
-        if dup:
-            self.scan.verbose(f"{event.module}: Duplicate event: {event}")
-        else:
-            self.events_distributed.add(event_hash)
-        # absorb event into the word cloud if it's in scope
-        if not dup and -1 < event.scope_distance < 1:
-            self.scan.word_cloud.absorb_event(event)
-        for mod in self.scan.modules.values():
-            if not dup or mod.accept_dupes:
-                mod.queue_event(event)
+        async with self.scan.acatch(context=self.distribute_event):
+            event = self.scan.make_event(*args, **kwargs)
 
-    def loop_until_finished(self):
-        modules = list(self.scan.modules.values())
-        activity = True
+            event_hash = hash(event)
+            dup = event_hash in self.events_distributed
+            if dup:
+                self.scan.verbose(f"{event.module}: Duplicate event: {event}")
+            else:
+                self.events_distributed.add(event_hash)
+            # absorb event into the word cloud if it's in scope
+            if not dup and -1 < event.scope_distance < 1:
+                self.scan.word_cloud.absorb_event(event)
+            for mod in self.scan.modules.values():
+                if not dup or mod.accept_dupes:
+                    await mod.queue_event(event)
 
+    async def _worker_loop(self):
         try:
-            self.scan.dispatcher.on_start(self.scan)
-
-            while 1:
-                # abort if we're aborting
-                if self.scan.aborting:
-                    # Empty event queues
-                    for module in self.scan.modules.values():
-                        with suppress(queue.Empty):
-                            while 1:
-                                module.incoming_event_queue.get_nowait()
-                    with suppress(queue.Empty):
-                        while 1:
-                            self.incoming_event_queue.get_nowait()
-                    break
-
-                if "python" in self.scan.modules:
-                    events, finish, report = self.scan.modules["python"].events_waiting
-                    yield from events
-
+            while not self.scan.stopped:
                 try:
-                    self.log_status(self.status_frequency)
-                    event, kwargs = self.incoming_event_queue.get_nowait()
-                    while not self.scan.aborting:
-                        try:
-                            acceptable = self.emit_event(event, _block=False, **kwargs)
-                            if acceptable:
-                                activity = True
-                            break
-                        except queue.Full:
-                            self.log_status(self.status_frequency)
-                            with self.event_emitted:
-                                self.event_emitted.wait(timeout=0.1)
-                except queue.Empty:
-                    # if we're on the last module
-                    modules_status = self.modules_status()
-                    finished = modules_status.get("finished", False)
-                    # And if the scan is finished
-                    if finished:
-                        # And if new events were generated since last time we were here
-                        if activity:
-                            activity = False
-                            self.scan.status = "FINISHING"
-                            # Trigger .finished() on every module and start over
-                            log.info("Finishing scan")
-                            finished_event = self.scan.make_event("FINISHED", "FINISHED", dummy=True)
-                            for module in modules:
-                                module.queue_event(finished_event)
-                        else:
-                            # Otherwise stop the scan if no new events were generated since last time
-                            break
-                    with self.incoming_event_queue.not_empty:
-                        self.incoming_event_queue.not_empty.wait(timeout=0.1)
-
-        except KeyboardInterrupt:
-            self.scan.stop()
+                    event, kwargs = self.get_event_from_modules()
+                except asyncio.queues.QueueEmpty:
+                    await asyncio.sleep(0.1)
+                    continue
+                await self.emit_event(event, **kwargs)
 
         except Exception:
             log.critical(traceback.format_exc())
 
-        finally:
-            # Run .report() on every module
-            for mod in self.scan.modules.values():
-                self.catch(mod._register_running, mod.report, _force=True)
+    @property
+    def modules_by_priority(self):
+        if not self._modules_by_priority:
+            self._modules_by_priority = sorted(list(self.scan.modules.values()), key=lambda m: m.priority)
+        return self._modules_by_priority
+
+    @property
+    def incoming_queues(self):
+        if not self._incoming_queues:
+            queues_by_priority = [m.outgoing_event_queue for m in self.modules_by_priority]
+            self._incoming_queues = [self.incoming_event_queue] + queues_by_priority
+        return self._incoming_queues
+
+    @property
+    def module_priority_weights(self):
+        if not self._module_priority_weights:
+            # we subtract from six because lower priorities == higher weights
+            priorities = [5] + [6 - m.priority for m in self.modules_by_priority]
+            self._module_priority_weights = priorities
+        return self._module_priority_weights
 
-    def log_status(self, frequency=15):
-        # print status every 15 seconds (or status_frequency setting)
-        timedelta_secs = timedelta(seconds=frequency)
-        now = datetime.now()
-        time_since_last_log = now - self.last_log_time
-        if time_since_last_log > timedelta_secs:
-            self.modules_status(_log=True, passes=1)
-            self.last_log_time = now
-
-    def modules_status(self, _log=False, passes=None):
-        # If scan looks to be finished, check an additional five times to ensure that it really is
-        # There is a tiny chance of a race condition, which this helps to avoid
-        if passes is None:
-            passes = 5
-        else:
-            passes = max(1, int(passes))
+    def get_event_from_modules(self):
+        for q in self.scan.helpers.weighted_shuffle(self.incoming_queues, self.module_priority_weights):
+            try:
+                return q.get_nowait()
+            except (asyncio.queues.QueueEmpty, AttributeError):
+                continue
+        raise asyncio.queues.QueueEmpty()
+
+    @property
+    def queued_event_types(self):
+        event_types = {}
+        for q in self.incoming_queues:
+            for event, _ in q._queue:
+                event_type = getattr(event, "type", None)
+                if event_type is not None:
+                    try:
+                        event_types[event_type] += 1
+                    except KeyError:
+                        event_types[event_type] = 1
+        return event_types
+
+    def queue_event(self, event, **kwargs):
+        if event:
+            # nerf event's priority if it's likely not to be in scope
+            if event.scope_distance > 0:
+                event_in_scope = self.scan.whitelisted(event) and not self.scan.blacklisted(event)
+                if not event_in_scope:
+                    event.module_priority += event.scope_distance
+            # Wait for parent event to resolve (in case its scope distance changes)
+            # await resolved = event.source._resolved.wait()
+            # update event's scope distance based on its parent
+            event.scope_distance = event.source.scope_distance + 1
+            self.incoming_event_queue.put_nowait((event, kwargs))
+
+    @property
+    def running(self):
+        active_tasks = self._task_counter.value
+        incoming_events = self.incoming_event_queue.qsize()
+        return active_tasks > 0 or incoming_events > 0
+
+    @property
+    def modules_finished(self):
+        finished_modules = [m.finished for m in self.scan.modules.values()]
+        return all(finished_modules)
+
+    @property
+    def active(self):
+        return self.running or not self.modules_finished
 
+    def modules_status(self, _log=False):
         finished = True
-        while passes > 0:
-            status = {"modules": {}, "scan": self.scan.status_detailed}
+        status = {"modules": {}}
 
-            for num_tasks in status["scan"]["queued_tasks"].values():
-                if num_tasks > 0:
-                    finished = False
-
-            for m in self.scan.modules.values():
-                mod_status = m.status
-                if mod_status["active"]:
-                    finished = False
-                status["modules"][m.name] = mod_status
+        for m in self.scan.modules.values():
+            mod_status = m.status
+            if mod_status["running"]:
+                finished = False
+            status["modules"][m.name] = mod_status
 
-            for mod in self.scan.modules.values():
-                if mod.errored and mod.incoming_event_queue not in [None, False]:
-                    with suppress(Exception):
-                        mod.set_error_state()
-
-            passes -= 1
-            if finished and passes > 0:
-                sleep(0.1)
-            else:
-                break
+        for mod in self.scan.modules.values():
+            if mod.errored and mod.incoming_event_queue not in [None, False]:
+                with suppress(Exception):
+                    mod.set_error_state()
 
         status["finished"] = finished
 
         modules_errored = [m for m, s in status["modules"].items() if s["errored"]]
 
         if _log:
             modules_status = []
             for m, s in status["modules"].items():
                 running = s["running"]
                 incoming = s["events"]["incoming"]
                 outgoing = s["events"]["outgoing"]
-                tasks = s["tasks"]["total"]
+                tasks = s["tasks"]
                 total = sum([incoming, outgoing, tasks])
                 if running or total > 0:
                     modules_status.append((m, running, incoming, outgoing, tasks, total))
             modules_status.sort(key=lambda x: x[-1], reverse=True)
 
             if modules_status:
                 modules_status_str = ", ".join([f"{m}({i:,}:{t:,}:{o:,})" for m, r, i, o, t, _ in modules_status])
@@ -524,49 +466,51 @@
             if event_type_summary:
                 self.scan.info(
                     f'{self.scan.name}: Events produced so far: {", ".join([f"{k}: {v}" for k,v in event_type_summary])}'
                 )
             else:
                 self.scan.info(f"{self.scan.name}: No events produced yet")
 
-            total_tasks = status["scan"]["queued_tasks"]["total"]
-            event_tasks = status["scan"]["queued_tasks"]["event"]
-            internal_tasks = status["scan"]["queued_tasks"]["internal"]
-            self.scan.verbose(
-                f"{self.scan.name}: Thread pool tasks: {total_tasks:,} (Event: {event_tasks:,}, Internal: {internal_tasks:,})"
-            )
-
             if modules_errored:
                 self.scan.verbose(
                     f'{self.scan.name}: Modules errored: {len(modules_errored):,} ({", ".join([m for m in modules_errored])})'
                 )
 
-            queued_events_by_type = [(k, v) for k, v in self.incoming_event_queue.event_types.items() if v > 0]
+            queued_events_by_type = [(k, v) for k, v in self.queued_event_types.items() if v > 0]
             if queued_events_by_type:
                 queued_events_by_type.sort(key=lambda x: x[-1], reverse=True)
                 queued_events_by_type_str = ", ".join(f"{m}: {t:,}" for m, t in queued_events_by_type)
+                num_queued_events = sum(v for k, v in queued_events_by_type)
                 self.scan.info(
-                    f"{self.scan.name}: {self.incoming_event_queue.qsize():,} events in queue ({queued_events_by_type_str})"
+                    f"{self.scan.name}: {num_queued_events:,} events in queue ({queued_events_by_type_str})"
                 )
             else:
                 self.scan.info(f"{self.scan.name}: No events in queue")
 
-            # if debugging is enabled
-            self.scan.debug(f"THREAD POOL STATUS:")
             if self.scan.log_level <= logging.DEBUG:
-                # log thread pool statuses
-                threadpool_names = [
-                    "_internal_thread_pool",
-                    "_event_thread_pool",
-                    "_thread_pool",
-                ]
-                for threadpool_name in threadpool_names:
-                    threadpool = getattr(self.scan, threadpool_name)
-                    for thread_status in threadpool.threads_status:
-                        self.scan.debug(f"    - {threadpool_name}: {thread_status}")
+                # status debugging
+                scan_active_status = []
+                scan_active_status.append(f"scan._finished_init: {self.scan._finished_init}")
+                scan_active_status.append(f"manager.active: {self.active}")
+                scan_active_status.append(f"    manager.running: {self.running}")
+                scan_active_status.append(f"        manager._task_counter.value: {self._task_counter.value}")
+                scan_active_status.append(
+                    f"        manager.incoming_event_queue.qsize(): {self.incoming_event_queue.qsize()}"
+                )
+                scan_active_status.append(f"    manager.modules_finished: {self.modules_finished}")
+                for m in self.scan.modules.values():
+                    scan_active_status.append(f"        {m}.finished: {m.finished}")
+                    scan_active_status.append(f"            running: {m.running}")
+                    scan_active_status.append(f"            num_incoming_events: {m.num_incoming_events}")
+                    scan_active_status.append(
+                        f"            outgoing_event_queue.qsize(): {m.outgoing_event_queue.qsize()}"
+                    )
+                for line in scan_active_status:
+                    self.scan.debug(line)
+
                 # log module memory usage
                 module_memory_usage = []
                 for module in self.scan.modules.values():
                     memory_usage = module.memory_usage
                     module_memory_usage.append((module.name, memory_usage))
                 module_memory_usage.sort(key=lambda x: x[-1], reverse=True)
                 self.scan.debug(f"MODULE MEMORY USAGE:")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1793rc0/bbot/scanner/scanner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+import asyncio
 import logging
-import threading
 import traceback
+import contextlib
 from sys import exc_info
 from pathlib import Path
-import concurrent.futures
+import multiprocessing as mp
 from datetime import datetime
+from functools import partial
 from omegaconf import OmegaConf
-from contextlib import suppress
-from collections import OrderedDict, deque
+from collections import OrderedDict
+from concurrent.futures import ProcessPoolExecutor
 
 from bbot import config as bbot_config
 
 from .stats import ScanStats
 from .target import ScanTarget
 from .manager import ScanManager
 from .dispatcher import Dispatcher
 from bbot.modules import module_loader
 from bbot.core.event import make_event
 from bbot.core.helpers.misc import sha1, rand_string
 from bbot.core.helpers.helper import ConfigAwareHelper
-from bbot.core.logger import init_logging, get_log_level
 from bbot.core.helpers.names_generator import random_name
+from bbot.core.helpers.async_helpers import async_to_sync_gen
 from bbot.core.configurator.environ import prepare_environment
-from bbot.core.helpers.threadpool import ThreadPoolWrapper, BBOTThreadPoolExecutor
-from bbot.core.errors import BBOTError, ScanError, ScanCancelledError, ValidationError
+from bbot.core.errors import BBOTError, ScanError, ValidationError
+from bbot.core.logger import init_logging, get_log_level, set_log_level
 
 log = logging.getLogger("bbot.scanner")
 
 init_logging()
 
 
 class Scanner:
@@ -69,44 +71,29 @@
 
         if config is None:
             config = OmegaConf.create({})
         else:
             config = OmegaConf.create(config)
         self.config = OmegaConf.merge(bbot_config, config)
         prepare_environment(self.config)
+        if self.config.get("debug", False):
+            set_log_level(logging.DEBUG)
 
         self.strict_scope = strict_scope
         self.force_start = force_start
 
         if scan_id is not None:
             self.id = str(scan_id)
         else:
             self.id = f"SCAN:{sha1(rand_string(20)).hexdigest()}"
         self._status = "NOT_STARTED"
         self._status_code = 0
 
-        # Set up thread pools
-        max_workers = max(1, self.config.get("max_threads", 25))
-        # Shared thread pool, for module use
-        self._thread_pool = BBOTThreadPoolExecutor(max_workers=max_workers)
-        # Event thread pool, for event emission
-        self._event_thread_pool = ThreadPoolWrapper(
-            BBOTThreadPoolExecutor(max_workers=max_workers * 2), qsize=max_workers
-        )
-        # Internal thread pool, for handle_event(), module setup, cleanup callbacks, etc.
-        self._internal_thread_pool = ThreadPoolWrapper(BBOTThreadPoolExecutor(max_workers=max_workers))
-        self.process_pool = ThreadPoolWrapper(concurrent.futures.ProcessPoolExecutor())
+        self.max_workers = max(1, self.config.get("max_threads", 25))
         self.helpers = ConfigAwareHelper(config=self.config, scan=self)
-        self.pools = {
-            "process_pool": self.process_pool,
-            "internal_thread_pool": self._internal_thread_pool,
-            "dns_thread_pool": self.helpers.dns._thread_pool,
-            "event_thread_pool": self._event_thread_pool,
-            "main_thread_pool": self._thread_pool,
-        }
         output_dir = self.config.get("output_dir", "")
 
         if name is None:
             tries = 0
 
             while 1:
                 if tries > 5:
@@ -166,114 +153,153 @@
         # custom HTTP headers warning
         self.custom_http_headers = self.config.get("http_headers", {})
         if self.custom_http_headers:
             self.warning(
                 "You have enabled custom HTTP headers. These will be attached to all in-scope requests and all requests made by httpx."
             )
 
+        # how often to print scan status
+        self.status_frequency = self.config.get("status_frequency", 15)
+
         self._prepped = False
-        self._thread_pools_shutdown = False
-        self._thread_pools_shutdown_threads = []
+        self._finished_init = False
         self._cleanedup = False
 
-    def prep(self):
+        self.__loop = None
+        self.manager_worker_loop_tasks = []
+        self.init_events_task = None
+        self.ticker_task = None
+        self.dispatcher_tasks = []
+
+        # multiprocessing thread pool
+        try:
+            mp.set_start_method("spawn")
+        except Exception:
+            self.warning(f"Failed to set multiprocessing spawn method. This may negatively affect performance.")
+        self.process_pool = ProcessPoolExecutor()
+
+        self._stopping = False
+
+    def _on_keyboard_interrupt(self, loop, event):
+        self.stop()
+
+    async def prep(self):
+        # event = asyncio.Event()
+        # self._loop.add_signal_handler(signal.SIGINT, self._on_keyboard_interrupt, loop, event)
+
         self.helpers.mkdir(self.home)
         if not self._prepped:
             start_msg = f"Scan with {len(self._scan_modules):,} modules seeded with {len(self.target):,} targets"
             details = []
             if self.whitelist != self.target:
                 details.append(f"{len(self.whitelist):,} in whitelist")
             if self.blacklist:
                 details.append(f"{len(self.blacklist):,} in blacklist")
             if details:
                 start_msg += f" ({', '.join(details)})"
             self.hugeinfo(start_msg)
 
-            self.load_modules()
+            await self.load_modules()
 
             self.info(f"Setting up modules...")
-            self.setup_modules()
+            await self.setup_modules()
 
             self.success(f"Setup succeeded for {len(self.modules):,} modules.")
             self._prepped = True
 
-    def start_without_generator(self):
-        deque(self.start(), maxlen=0)
-
     def start(self):
-        self.prep()
+        for event in async_to_sync_gen(self.async_start()):
+            yield event
 
-        failed = True
+    def start_without_generator(self):
+        for event in async_to_sync_gen(self.async_start()):
+            pass
 
-        if not self.target:
-            self.warning(f"No scan targets specified")
+    async def async_start_without_generator(self):
+        async for event in self.async_start():
+            pass
 
+    async def async_start(self):
+        failed = True
         scan_start_time = datetime.now()
         try:
+            await self.prep()
+
+            if not self.target:
+                self.warning(f"No scan targets specified")
+
+            # start status ticker
+            self.ticker_task = asyncio.create_task(self._status_ticker(self.status_frequency))
+
             self.status = "STARTING"
 
             if not self.modules:
                 self.error(f"No modules loaded")
                 self.status = "FAILED"
                 return
             else:
                 self.hugesuccess(f"Starting scan {self.name}")
 
-            if self.stopping:
-                return
+            await self.dispatcher.on_start(self)
 
-            # distribute seed events
-            self.manager.init_events()
+            # start manager worker loops
+            self.manager_worker_loop_tasks = [
+                asyncio.create_task(self.manager._worker_loop()) for _ in range(self.max_workers)
+            ]
 
-            if self.stopping:
-                return
+            # distribute seed events
+            self.init_events_task = asyncio.create_task(self.manager.init_events())
 
             self.status = "RUNNING"
             self.start_modules()
             self.verbose(f"{len(self.modules):,} modules started")
 
-            if self.stopping:
-                return
+            # main scan loop
+            while 1:
+                # abort if we're aborting
+                if self.aborting:
+                    self.drain_queues()
+                    break
 
-            yield from self.manager.loop_until_finished()
-            failed = False
+                if "python" in self.modules:
+                    events, finish, report = await self.modules["python"].events_waiting()
+                    for e in events:
+                        yield e
+
+                # if initialization finished and the scan is no longer active
+                if self._finished_init and not self.manager.active:
+                    new_activity = await self.finish()
+                    if not new_activity:
+                        break
 
-        except KeyboardInterrupt:
-            self.stop()
-            failed = False
+                await asyncio.sleep(0.1)
 
-        except ScanCancelledError:
-            self.debug("Scan cancelled")
+            failed = False
 
-        except ScanError as e:
-            self.error(f"{e}")
+        except BaseException as e:
+            exception_chain = self.helpers.get_exception_chain(e)
+            if any(isinstance(exc, (KeyboardInterrupt, asyncio.CancelledError)) for exc in exception_chain):
+                self.stop()
+                failed = False
+            else:
+                try:
+                    raise
+                except ScanError as e:
+                    self.error(f"{e}")
 
-        except BBOTError as e:
-            self.critical(f"Error during scan: {e}")
-            self.trace()
+                except BBOTError as e:
+                    self.critical(f"Error during scan: {e}")
 
-        except Exception:
-            self.critical(f"Unexpected error during scan:\n{traceback.format_exc()}")
+                except Exception:
+                    self.critical(f"Unexpected error during scan:\n{traceback.format_exc()}")
 
         finally:
-            self.cleanup()
-            self.shutdown_threadpools()
-            while 1:
-                for t in self._thread_pools_shutdown_threads:
-                    t.join(timeout=1)
-                    if t.is_alive():
-                        try:
-                            pool = t._args[0]
-                            for s in pool.threads_status:
-                                self.debug(s)
-                        except AttributeError:
-                            continue
-                if not any(t.is_alive() for t in self._thread_pools_shutdown_threads):
-                    self.debug("Finished shutting down thread pools")
-                    break
+            self.cancel_tasks()
+            await self.report()
+            await self.cleanup()
 
             log_fn = self.hugesuccess
             if self.status == "ABORTING":
                 self.status = "ABORTED"
                 log_fn = self.hugewarning
             elif failed:
                 self.status = "FAILED"
@@ -281,34 +307,29 @@
             else:
                 self.status = "FINISHED"
 
             scan_run_time = datetime.now() - scan_start_time
             scan_run_time = self.helpers.human_timedelta(scan_run_time)
             log_fn(f"Scan {self.name} completed in {scan_run_time} with status {self.status}")
 
-            self.dispatcher.on_finish(self)
+            await self.dispatcher.on_finish(self)
 
     def start_modules(self):
-        self.verbose(f"Starting module threads")
+        self.verbose(f"Starting module worker loops")
         for module_name, module in self.modules.items():
             module.start()
 
-    def setup_modules(self, remove_failed=True):
-        self.load_modules()
+    async def setup_modules(self, remove_failed=True):
+        await self.load_modules()
         self.verbose(f"Setting up modules")
         hard_failed = []
         soft_failed = []
-        setup_futures = dict()
 
-        for module_name, module in self.modules.items():
-            future = self._internal_thread_pool.submit_task(module._setup)
-            setup_futures[future] = module_name
-        for future in self.helpers.as_completed(setup_futures):
-            module_name = setup_futures[future]
-            status, msg = future.result()
+        for task in asyncio.as_completed([asyncio.create_task(m._setup()) for m in self.modules.values()]):
+            module_name, status, msg = await task
             if status == True:
                 self.debug(f"Setup succeeded for {module_name} ({msg})")
             elif status == False:
                 self.error(f"Setup hard-failed for {module_name}: {msg}")
                 self.modules[module_name].set_error_state()
                 hard_failed.append(module_name)
             else:
@@ -323,50 +344,92 @@
         total_failed = len(hard_failed + soft_failed)
         if hard_failed:
             msg = f"Setup hard-failed for {len(hard_failed):,} modules ({','.join(hard_failed)})"
             self.fail_setup(msg)
         elif total_failed > 0:
             self.warning(f"Setup failed for {total_failed:,} modules")
 
-    def stop(self, wait=False):
-        if self.status != "ABORTING":
+    def stop(self):
+        if not self._stopping:
+            self._stopping = True
             self.status = "ABORTING"
             self.hugewarning(f"Aborting scan")
+            self.trace()
+            self.cancel_tasks()
+            self.drain_queues()
             self.helpers.kill_children()
-            self.shutdown_threadpools()
+            self.drain_queues()
             self.helpers.kill_children()
 
-    def shutdown_threadpools(self):
-        if not self._thread_pools_shutdown:
-            self._thread_pools_shutdown = True
-
-            def shutdown_pool(pool, pool_name, **kwargs):
-                self.debug(f"Shutting down {pool_name} with kwargs={kwargs}")
-                pool.shutdown(**kwargs)
-                self.debug(f"Finished shutting down {pool_name} with kwargs={kwargs}")
-
-            self.debug(f"Shutting down thread pools")
-            for pool_name, pool in self.pools.items():
-                t = threading.Thread(
-                    target=shutdown_pool,
-                    args=(pool, pool_name),
-                    kwargs={"wait": True, "cancel_futures": True},
-                    daemon=True,
-                )
-                t.start()
-                self._thread_pools_shutdown_threads.append(t)
+    async def finish(self):
+        # if new events were generated since last time we were here
+        if self.manager._new_activity:
+            self.manager._new_activity = False
+            self.status = "FINISHING"
+            # Trigger .finished() on every module and start over
+            log.info("Finishing scan")
+            finished_event = self.make_event("FINISHED", "FINISHED", dummy=True)
+            for module in self.modules.values():
+                await module.queue_event(finished_event)
+            self.verbose("Completed finish()")
+            return True
+        # Return False if no new events were generated since last time
+        self.verbose("Completed final finish()")
+        return False
+
+    def drain_queues(self):
+        # Empty event queues
+        self.debug("Draining queues")
+        for module in self.modules.values():
+            with contextlib.suppress(asyncio.queues.QueueEmpty):
+                while 1:
+                    if module.incoming_event_queue:
+                        module.incoming_event_queue.get_nowait()
+            with contextlib.suppress(asyncio.queues.QueueEmpty):
+                while 1:
+                    if module.outgoing_event_queue:
+                        module.outgoing_event_queue.get_nowait()
+        with contextlib.suppress(asyncio.queues.QueueEmpty):
+            while 1:
+                self.manager.incoming_event_queue.get_nowait()
+        self.debug("Finished draining queues")
 
-    def cleanup(self):
+    def cancel_tasks(self):
+        tasks = []
+        # module workers
+        for m in self.modules.values():
+            tasks += getattr(m, "_tasks", [])
+        # init events
+        if self.init_events_task:
+            tasks.append(self.init_events_task)
+        # ticker
+        if self.ticker_task:
+            tasks.append(self.ticker_task)
+        # dispatcher
+        tasks += self.dispatcher_tasks
+        # manager worker loops
+        tasks += self.manager_worker_loop_tasks
+        self.helpers.cancel_tasks_sync(tasks)
+        # process pool
+        self.process_pool.shutdown(cancel_futures=True)
+
+    async def report(self):
+        for mod in self.modules.values():
+            async with self.acatch(context=mod.report):
+                with mod._task_counter:
+                    await mod.report()
+
+    async def cleanup(self):
         # clean up modules
         self.status = "CLEANING_UP"
         for mod in self.modules.values():
-            mod._cleanup()
+            await mod._cleanup()
         if not self._cleanedup:
             self._cleanedup = True
-            with suppress(Exception):
+            with contextlib.suppress(Exception):
                 self.home.rmdir()
             self.helpers.clean_old_scans()
 
     def in_scope(self, e):
         """
         Checks whitelist and blacklist, also taking scope_distance into account
         """
@@ -390,14 +453,18 @@
         return self.helpers.word_cloud
 
     @property
     def stopping(self):
         return not self.running
 
     @property
+    def stopped(self):
+        return self._status_code > 5
+
+    @property
     def running(self):
         return 0 < self._status_code < 4
 
     @property
     def aborting(self):
         return 5 <= self._status_code <= 6
 
@@ -411,36 +478,25 @@
         Block setting after status has been aborted
         """
         status = str(status).strip().upper()
         if status in self._status_codes:
             if self.status == "ABORTING" and not status == "ABORTED":
                 self.debug(f'Attempt to set invalid status "{status}" on aborted scan')
             else:
-                self._status = status
-                self._status_code = self._status_codes[status]
-                self.dispatcher.on_status(self._status, self.id)
+                if status != self._status:
+                    self._status = status
+                    self._status_code = self._status_codes[status]
+                    self.dispatcher_tasks.append(
+                        asyncio.create_task(self.dispatcher.catch(self.dispatcher.on_status, self._status, self.id))
+                    )
+                else:
+                    self.debug(f'Scan status is already "{status}"')
         else:
             self.debug(f'Attempt to set invalid status "{status}" on scan')
 
-    @property
-    def status_detailed(self):
-        event_threadpool_tasks = self._event_thread_pool.num_tasks
-        internal_tasks = self._internal_thread_pool.num_tasks
-        process_tasks = self.process_pool.num_tasks
-        total_tasks = event_threadpool_tasks + internal_tasks + process_tasks
-        status = {
-            "queued_tasks": {
-                "internal": internal_tasks,
-                "process": process_tasks,
-                "event": event_threadpool_tasks,
-                "total": total_tasks,
-            },
-        }
-        return status
-
     def make_event(self, *args, **kwargs):
         kwargs["scan"] = self
         event = make_event(*args, **kwargs)
         return event
 
     @property
     def log(self):
@@ -475,72 +531,91 @@
             j.update({"whitelist": [str(e.data) for e in self.whitelist]})
         if self.blacklist:
             j.update({"blacklist": [str(e.data) for e in self.blacklist]})
         if self.modules:
             j.update({"modules": [str(m) for m in self.modules]})
         return j
 
-    def debug(self, *args, **kwargs):
+    def debug(self, *args, trace=False, **kwargs):
         log.debug(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def verbose(self, *args, **kwargs):
+    def verbose(self, *args, trace=False, **kwargs):
         log.verbose(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def hugeverbose(self, *args, **kwargs):
+    def hugeverbose(self, *args, trace=False, **kwargs):
         log.hugeverbose(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def info(self, *args, **kwargs):
+    def info(self, *args, trace=False, **kwargs):
         log.info(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def hugeinfo(self, *args, **kwargs):
+    def hugeinfo(self, *args, trace=False, **kwargs):
         log.hugeinfo(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def success(self, *args, **kwargs):
+    def success(self, *args, trace=False, **kwargs):
         log.success(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def hugesuccess(self, *args, **kwargs):
+    def hugesuccess(self, *args, trace=False, **kwargs):
         log.hugesuccess(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
-    def warning(self, *args, **kwargs):
+    def warning(self, *args, trace=True, **kwargs):
         log.warning(*args, extra={"scan_id": self.id}, **kwargs)
-        self.trace()
+        if trace:
+            self.trace()
 
-    def hugewarning(self, *args, **kwargs):
+    def hugewarning(self, *args, trace=True, **kwargs):
         log.hugewarning(*args, extra={"scan_id": self.id}, **kwargs)
-        self.trace()
+        if trace:
+            self.trace()
 
-    def error(self, *args, **kwargs):
+    def error(self, *args, trace=True, **kwargs):
         log.error(*args, extra={"scan_id": self.id}, **kwargs)
-        self.trace()
+        if trace:
+            self.trace()
 
     def trace(self):
         e_type, e_val, e_traceback = exc_info()
         if e_type is not None:
             log.trace(traceback.format_exc())
 
-    def critical(self, *args, **kwargs):
+    def critical(self, *args, trace=True, **kwargs):
         log.critical(*args, extra={"scan_id": self.id}, **kwargs)
+        if trace:
+            self.trace()
 
     def _internal_modules(self):
         for modname in module_loader.preloaded(type="internal"):
             if self.config.get(modname, True):
                 yield modname
 
-    def load_modules(self):
+    async def load_modules(self):
         if not self._modules_loaded:
             all_modules = list(set(self._scan_modules + self._output_modules + self._internal_modules))
             if not all_modules:
                 self.warning(f"No modules to load")
                 return
 
             if not self._scan_modules:
                 self.warning(f"No scan modules to load")
 
             # install module dependencies
-            succeeded, failed = self.helpers.depsinstaller.install(
+            succeeded, failed = await self.helpers.depsinstaller.install(
                 *self._scan_modules, *self._output_modules, *self._internal_modules
             )
             if failed:
                 msg = f"Failed to install dependencies for {len(failed):,} modules: {','.join(failed)}"
                 self.fail_setup(msg)
             modules = sorted([m for m in self._scan_modules if m in succeeded])
             output_modules = sorted([m for m in self._output_modules if m in succeeded])
@@ -594,14 +669,20 @@
         else:
             raise ScanError(msg)
 
     @property
     def log_level(self):
         return get_log_level()
 
+    @property
+    def _loop(self):
+        if self.__loop is None:
+            self.__loop = asyncio.get_event_loop()
+        return self.__loop
+
     def _load_modules(self, modules):
         modules = [str(m) for m in modules]
         loaded_modules = {}
         failed = set()
         for module_name, module_class in module_loader.load_modules(modules).items():
             if module_class:
                 try:
@@ -610,7 +691,71 @@
                     continue
                 except Exception:
                     self.warning(f"Failed to load module {module_class}")
             else:
                 self.warning(f'Failed to load unknown module "{module_name}"')
             failed.add(module_name)
         return loaded_modules, failed
+
+    async def _status_ticker(self, interval=15):
+        async with self.acatch():
+            while 1:
+                await asyncio.sleep(interval)
+                self.manager.modules_status(_log=True)
+
+    @contextlib.contextmanager
+    def catch(self, context="scan", finally_callback=None):
+        """
+        Handle common errors by stopping scan, logging tracebacks, etc.
+
+        with catch():
+            do_stuff()
+        """
+        try:
+            yield
+        except BaseException as e:
+            self._handle_exception(e, context=context)
+
+    @contextlib.asynccontextmanager
+    async def acatch(self, context="scan", finally_callback=None):
+        """
+        Async version of catch()
+
+        async with catch():
+            await do_stuff()
+        """
+        try:
+            yield
+        except BaseException as e:
+            self._handle_exception(e, context=context)
+
+    def run_in_executor(self, callback, *args, **kwargs):
+        """
+        Run a synchronous task in the event loop's default thread pool executor
+        """
+        callback = partial(callback, **kwargs)
+        return self._loop.run_in_executor(None, callback, *args)
+
+    def run_in_executor_mp(self, callback, *args, **kwargs):
+        """
+        Same as run_in_executor() except with a process pool executor
+        """
+        callback = partial(callback, **kwargs)
+        return self._loop.run_in_executor(self.process_pool, callback, *args)
+
+    def _handle_exception(self, e, context="scan", finally_callback=None):
+        if callable(context):
+            context = f"{context.__qualname__}()"
+        filename, lineno, funcname = self.helpers.get_traceback_details(e)
+        exception_chain = self.helpers.get_exception_chain(e)
+        if any(isinstance(exc, KeyboardInterrupt) for exc in exception_chain):
+            log.debug(f"Interrupted")
+            self.stop()
+        elif isinstance(e, BrokenPipeError):
+            log.debug(f"BrokenPipeError in {filename}:{lineno}:{funcname}(): {e}")
+        elif isinstance(e, asyncio.CancelledError):
+            raise
+        elif isinstance(e, Exception):
+            log.error(f"Error in {context}: {filename}:{lineno}:{funcname}(): {e}")
+            log.trace(traceback.format_exc())
+        if callable(finally_callback):
+            self.helpers.execute_sync_or_async(finally_callback, e)
```

### Comparing `bbot-1.0.5.1665rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1793rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/scanner/target.py` & `bbot-1.0.5.1793rc0/bbot/scanner/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                     self._events[k] = set(t._events[k])
         else:
             if is_event(t):
                 event = t
             else:
                 event = self.scan.make_event(t, source=self.scan.root_event, module=self.dummy_module, tags=["target"])
             if self.make_in_scope:
-                event.make_in_scope()
+                event.set_scope_distance(0)
             try:
                 self._events[event.host].add(event)
             except KeyError:
                 self._events[event.host] = {
                     event,
                 }
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1793rc0/bbot/test/run_tests.sh`

 * *Files 15% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 echo "[+] Linting with flake8"
 echo "======================="
 flake8 --select F,E722 --ignore F403,F405,F541 --per-file-ignores="*/__init__.py:F401,F403" "$bbot_dir" || exit 1
 echo
 
 echo "[+] Testing with pytest"
-pytest --exitfirst --disable-warnings --log-cli-level=ERROR "$bbot_dir" --cov=bbot --cov-report term-missing
+pytest --exitfirst --disable-warnings --log-cli-level=ERROR "$bbot_dir" --cov=bbot/test/test_step_2/test_cli.py --cov-report term-missing
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test.conf` & `bbot-1.0.5.1793rc0/bbot/test/test.conf`

 * *Files 17% similar despite different names*

```diff
@@ -25,18 +25,27 @@
 http_proxy:
 http_headers: { "test": "header" }
 ssl_verify: false
 scope_search_distance: 0
 scope_report_distance: 0
 scope_dns_search_distance: 1
 plumbus: asdf
-dns_debug: false
+dns_debug: true
+user_agent: "BBOT Test User-Agent"
 http_debug: false
 keep_scans: 1
-agent_url: test
+agent_url: ws://127.0.0.1:8765
 agent_token: test
 dns_resolution: false
+dns_timeout: 1
 speculate: false
 excavate: false
 aggregate: false
 omit_event_types: []
 debug: true
+dns_wildcard_ignore:
+  - blacklanternsecurity.com
+  - fakedomain
+  - notreal
+  - google
+  - google.com
+  - example.com
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_cli.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ..bbot_fixtures import *
 
 
-def test_cli(monkeypatch, bbot_config):
+@pytest.mark.asyncio
+async def test_cli(monkeypatch, bbot_config):
     from bbot import cli
 
     monkeypatch.setattr(sys, "exit", lambda *args, **kwargs: True)
     monkeypatch.setattr(os, "_exit", lambda *args, **kwargs: True)
     monkeypatch.setattr(cli, "config", bbot_config)
 
     old_sys_argv = sys.argv
@@ -31,15 +32,15 @@
             "test_cli_scan",
             "-c",
             "dns_resolution=False",
             "-o",
             "/tmp",
         ],
     )
-    cli.main()
+    await cli._main()
 
     scan_home = scans_home / "test_cli_scan"
     assert (scan_home / "wordcloud.tsv").is_file()
     assert (scan_home / "output.txt").is_file()
     assert (scan_home / "output.csv").is_file()
     assert (scan_home / "output.json").is_file()
     with open(scan_home / "output.csv") as f:
@@ -57,27 +58,81 @@
                 ip_success = True
             if "[DNS_NAME]          \twww.example.com\tTARGET" in line:
                 dns_success = True
     assert ip_success and dns_success
 
     # show version
     monkeypatch.setattr("sys.argv", ["bbot", "--version"])
-    cli.main()
+    await cli._main()
+
+    # start agent
+    monkeypatch.setattr("sys.argv", ["bbot", "--agent-mode"])
+    task = asyncio.create_task(cli._main())
+    await asyncio.sleep(2)
+    task.cancel()
+    await task
+
+    # no args
+    monkeypatch.setattr("sys.argv", ["bbot"])
+    await cli._main()
+
+    # enable module by flag
+    monkeypatch.setattr("sys.argv", ["bbot", "-f", "report"])
+    await cli._main()
+
+    # unconsoleable output module
+    monkeypatch.setattr("sys.argv", ["bbot", "-om", "web_report"])
+    await cli._main()
+
+    # install all deps
+    monkeypatch.setattr("sys.argv", ["bbot", "--install-all-deps"])
+    success = await cli._main()
+    assert success, "--install-all-deps failed for at least one module"
+
+    # unresolved dependency
+    monkeypatch.setattr("sys.argv", ["bbot", "-m", "wappalyzer"])
+    await cli._main()
+
+    # resolved dependency, excluded module
+    monkeypatch.setattr("sys.argv", ["bbot", "-m", "ffuf_shortnames", "-em", "ffuf_shortnames"])
+    await cli._main()
+
+    # require flags
+    monkeypatch.setattr("sys.argv", ["bbot", "-f", "active", "-rf", "passive"])
+    await cli._main()
+
+    # excluded flags
+    monkeypatch.setattr("sys.argv", ["bbot", "-f", "active", "-ef", "active"])
+    await cli._main()
+
+    # slow modules
+    monkeypatch.setattr("sys.argv", ["bbot", "-m", "massdns"])
+    await cli._main()
+
+    # deadly modules
+    monkeypatch.setattr("sys.argv", ["bbot", "-m", "nuclei"])
+    result = await cli._main()
+    assert result == False
+
+    # --allow-deadly
+    monkeypatch.setattr("sys.argv", ["bbot", "-m", "nuclei", "--allow-deadly"])
+    result = await cli._main()
+    assert result != False
 
     # show current config
     monkeypatch.setattr("sys.argv", ["bbot", "-y", "--current-config"])
-    cli.main()
+    await cli._main()
 
     # list modules
     monkeypatch.setattr("sys.argv", ["bbot", "-l"])
-    cli.main()
+    await cli._main()
 
     # list module options
     monkeypatch.setattr("sys.argv", ["bbot", "--help-all"])
-    cli.main()
+    await cli._main()
 
     # unpatch sys.argv
     monkeypatch.setattr("sys.argv", old_sys_argv)
 
 
 def test_config_validation(monkeypatch, capsys, bbot_config):
     from bbot import cli
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_depsinstaller.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_events.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import random
 import ipaddress
 
 from ..bbot_fixtures import *
 
 
-def test_events(events, scan, helpers, bbot_config):
+@pytest.mark.asyncio
+async def test_events(events, scan, helpers, bbot_config):
     assert events.ipv4.type == "IP_ADDRESS"
     assert events.ipv6.type == "IP_ADDRESS"
     assert events.netv4.type == "IP_RANGE"
     assert events.netv6.type == "IP_RANGE"
     assert events.domain.type == "DNS_NAME"
     assert "domain" in events.domain.tags
     assert events.subdomain.type == "DNS_NAME"
@@ -135,15 +136,15 @@
     javascript_event = scan.make_event("http://evilcorp.com/asdf/a.js?b=c#d", "URL_UNVERIFIED", dummy=True)
     assert "extension-js" in javascript_event.tags
     assert "httpx-only" in javascript_event.tags
 
     # scope distance
     event1 = scan.make_event("1.2.3.4", dummy=True)
     assert event1._scope_distance == -1
-    event1.make_in_scope()
+    event1.set_scope_distance(0)
     assert event1._scope_distance == 0
     event2 = scan.make_event("2.3.4.5", source=event1)
     assert event2._scope_distance == 1
     event3 = scan.make_event("3.4.5.6", source=event2)
     assert event3._scope_distance == 2
     event4 = scan.make_event("3.4.5.6", source=event3)
     assert event4._scope_distance == 2
@@ -151,21 +152,21 @@
     assert event5._scope_distance == 3
 
     # internal event tracking
     root_event = scan.make_event("0.0.0.0", dummy=True)
     internal_event1 = scan.make_event("1.2.3.4", source=root_event, internal=True)
     assert internal_event1._internal == True
     assert internal_event1._made_internal == True
-    internal_event1.make_in_scope()
+    internal_event1.set_scope_distance(0)
     assert internal_event1._internal == False
     assert internal_event1._made_internal == False
     internal_event2 = scan.make_event("2.3.4.5", source=internal_event1, internal=True)
     internal_event3 = scan.make_event("3.4.5.6", source=internal_event2, internal=True)
     internal_event4 = scan.make_event("4.5.6.7", source=internal_event3)
-    source_trail = internal_event4.make_in_scope()
+    source_trail = internal_event4.set_scope_distance(0)
     assert internal_event4._internal == False
     assert internal_event3._internal == False
     assert internal_event2._internal == False
     assert len(source_trail) == 2
     assert internal_event2 in source_trail
     assert internal_event3 in source_trail
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_manager.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 from ..bbot_fixtures import *  # noqa: F401
 
 
-def test_manager(bbot_config, bbot_scanner):
+@pytest.mark.asyncio
+async def test_manager(bbot_config, bbot_scanner):
     dns_config = OmegaConf.merge(
         default_config, OmegaConf.create({"dns_resolution": True, "scope_report_distance": 1})
     )
 
     # test _emit_event
     results = []
     output = []
+    event_children = []
+
+    async def results_append(e):
+        results.append(e)
+
+    async def output_append(e):
+        output.append(e)
+
+    def event_children_append(e):
+        event_children.append(e)
+
     success_callback = lambda e: results.append("success")
     scan1 = bbot_scanner("127.0.0.1", modules=["ipneighbor"], output_modules=["human"], config=dns_config)
-    scan1.load_modules()
+    await scan1.load_modules()
     module = scan1.modules["ipneighbor"]
     module.scope_distance_modifier = 0
-    module.queue_event = lambda e: results.append(e)
+    module.queue_event = results_append
     output_module = scan1.modules["human"]
-    output_module.queue_event = lambda e: output.append(e)
+    output_module.queue_event = output_append
     scan1.status = "RUNNING"
     manager = scan1.manager
     # manager.distribute_event = lambda e: results.append(e)
     localhost = scan1.make_event("127.0.0.1", source=scan1.root_event, tags=["localhost"])
 
     class DummyModule1:
         _type = "output"
@@ -32,154 +44,167 @@
 
     class DummyModule3:
         _type = "DNS"
         suppress_dupes = True
 
     localhost.module = DummyModule1()
     # make sure abort_if works as intended
-    manager._emit_event(localhost, abort_if=lambda e: e.module._type == "output")
+    await manager._emit_event(localhost, abort_if=lambda e: e.module._type == "output")
     assert len(results) == 0
     manager.events_accepted.clear()
+    manager.events_distributed.clear()
+    await manager._emit_event(localhost, abort_if=lambda e: e.module._type != "output")
+    assert len(results) == 1
+    results.clear()
+    manager.events_accepted.clear()
+    manager.events_distributed.clear()
     # make sure success_callback works as intended
-    manager._emit_event(
+    await manager._emit_event(
         localhost, on_success_callback=success_callback, abort_if=lambda e: e.module._type == "plumbus"
     )
     assert localhost in results
     assert "success" in results
     results.clear()
     # make sure deduplication is working
     localhost2 = scan1.make_event("127.0.0.1", source=scan1.root_event, tags=["localhost2"])
     manager._emit_event(localhost2)
     assert len(results) == 0
     # make sure dns resolution is working
     googledns = scan1.make_event("8.8.8.8", source=scan1.root_event)
     googledns.module = DummyModule2()
     googledns.source = "asdf"
-    googledns.make_in_scope()
-    event_children = []
-    manager.emit_event = lambda e, *args, **kwargs: event_children.append(e)
-    manager._emit_event(googledns)
+    googledns.set_scope_distance(0)
+    manager.queue_event = event_children_append
+    await manager._emit_event(googledns)
     assert len(event_children) > 0
     assert googledns in results
     assert googledns in output
     results.clear()
     output.clear()
     event_children.clear()
     # make sure deduplication catches the same event
-    manager._emit_event(googledns)
+    await manager._emit_event(googledns)
     assert len(output) == 0
     assert len(results) == 0
     assert len(event_children) == 0
     output.clear()
     event_children.clear()
     # make sure _force_output overrides dup detection
     googledns._force_output = True
-    manager._emit_event(googledns)
+    await manager._emit_event(googledns)
     assert googledns in output
     assert len(event_children) == 0
     googledns._force_output = False
     results.clear()
     event_children.clear()
     # same dns event but different source
     source_event = manager.scan.make_event("1.2.3.4", "IP_ADDRESS", source=manager.scan.root_event)
     source_event._resolved.set()
     googledns.source = source_event
-    manager._emit_event(googledns)
+    await manager._emit_event(googledns)
     assert len(event_children) == 0
     assert googledns in output
 
+    # error catching
+    msg = "Ignore this error, it belongs here"
+    exceptions = (Exception(msg), KeyboardInterrupt(msg), BrokenPipeError(msg))
+    for e in exceptions:
+        with manager.scan.catch():
+            raise e
+
 
-def test_scope_distance(bbot_scanner, bbot_config):
+@pytest.mark.asyncio
+async def test_scope_distance(bbot_scanner, bbot_config):
     # event filtering based on scope_distance
     scan1 = bbot_scanner(
         "127.0.0.1", "evilcorp.com", modules=["ipneighbor"], output_modules=["json"], config=bbot_config
     )
     scan1.status = "RUNNING"
-    scan1.load_modules()
+    await scan1.load_modules()
     module = scan1.modules["ipneighbor"]
-    module_queue = module.incoming_event_queue.queue
+    module_queue = module.incoming_event_queue._queue
     output_module = scan1.modules["json"]
-    output_queue = output_module.incoming_event_queue.queue
+    output_queue = output_module.incoming_event_queue._queue
     manager = scan1.manager
     test_event1 = scan1.make_event("127.0.0.1", source=scan1.root_event)
 
     assert scan1.scope_search_distance == 0
     assert scan1.scope_report_distance == 0
     assert module.scope_distance_modifier == 1
 
     # test _emit_event() with scope_distance == 0
-    manager._emit_event(test_event1)
+    await manager._emit_event(test_event1)
     assert test_event1.scope_distance == 0
     assert test_event1._internal == False
     assert test_event1 in output_queue
     assert test_event1 in module_queue
 
     test_event2 = scan1.make_event("2.3.4.5", source=test_event1)
     test_event3 = scan1.make_event("3.4.5.6", source=test_event2)
     test_event4 = scan1.make_event("4.5.6.7", source=test_event2)
     test_event4._force_output = True
     dns_event = scan1.make_event("evilcorp.com", source=scan1.root_event)
 
     # non-watched event type
-    manager._emit_event(dns_event)
+    await manager._emit_event(dns_event)
     assert dns_event.scope_distance == 0
     assert dns_event in output_queue
     assert dns_event not in module_queue
 
     # test _emit_event() with scope_distance == 1
     assert test_event2.scope_distance == 1
-    manager._emit_event(test_event2)
+    await manager._emit_event(test_event2)
     assert test_event2.scope_distance == 1
     assert test_event2._internal == True
     assert test_event2 not in output_queue
     assert test_event2 in module_queue
-    valid, reason = module._event_postcheck(test_event2)
+    valid, reason = await module._event_postcheck(test_event2)
     assert valid
 
     # test _emit_event() with scope_distance == 2
     assert test_event3.scope_distance == 2
-    manager._emit_event(test_event3)
+    await manager._emit_event(test_event3)
     assert test_event3.scope_distance == 2
     assert test_event3._internal == True
     assert test_event3 not in output_queue
     assert test_event3 in module_queue
-    valid, reason = module._event_postcheck(test_event3)
+    valid, reason = await module._event_postcheck(test_event3)
     assert not valid
     assert reason.startswith("its scope_distance (2) exceeds the maximum allowed by the scan")
 
     # test _emit_event() with scope_distance == 2 and _force_output == True
     assert test_event4.scope_distance == 2
-    manager._emit_event(test_event4)
+    await manager._emit_event(test_event4)
     assert test_event4.scope_distance == 2
     assert test_event4._internal == True
     assert test_event4._force_output == True
     assert test_event4 in output_queue
     assert test_event4 in module_queue
-    valid, reason = module._event_postcheck(test_event4)
+    valid, reason = await module._event_postcheck(test_event4)
     assert not valid
     assert reason.startswith("its scope_distance (2) exceeds the maximum allowed by the scan")
 
     # test _always_emit == True
     geoevent = scan1.make_event("USA", "GEOLOCATION", source=test_event3)
     assert geoevent.scope_distance == 3
     assert geoevent.always_emit == True
     assert geoevent._force_output == False
-    manager._emit_event(geoevent)
+    await manager._emit_event(geoevent)
     assert geoevent._force_output == True
     assert geoevent in output_queue
     assert geoevent not in module_queue
 
     # test always_emit tag
     affiliate_event = scan1.make_event("5.6.7.8", source=test_event3, tags="affiliate")
     assert "affiliate" in affiliate_event.tags
     assert "affiliate" in affiliate_event._always_emit_tags
     assert affiliate_event.scope_distance == 3
     assert affiliate_event._always_emit == False
     assert affiliate_event.always_emit == True
     assert affiliate_event._force_output == False
-    manager._emit_event(affiliate_event)
+    await manager._emit_event(affiliate_event)
     assert affiliate_event._force_output == True
     assert affiliate_event in output_queue
     assert affiliate_event in module_queue
-    valid, reason = module._event_postcheck(affiliate_event)
+    valid, reason = await module._event_postcheck(affiliate_event)
     assert not valid
     assert reason.startswith("its scope_distance (3) exceeds the maximum allowed by the scan")
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_modules_basic.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,242 +1,157 @@
 import re
-import requests_mock
-from contextlib import suppress
 
 from ..bbot_fixtures import *
 
 
-def test_modules_basic(patch_commands, patch_ansible, scan, helpers, events, bbot_config, bbot_scanner):
+@pytest.mark.asyncio
+async def test_modules_basic(scan, helpers, events, bbot_config, bbot_scanner, httpx_mock):
     fallback_nameservers = scan.helpers.temp_dir / "nameservers.txt"
     with open(fallback_nameservers, "w") as f:
         f.write("8.8.8.8\n")
 
-    with requests_mock.Mocker() as m:
-        for http_method in ("GET", "CONNECT", "HEAD", "POST", "PUT", "TRACE", "DEBUG", "PATCH", "DELETE", "OPTIONS"):
-            m.request(http_method, re.compile(r".*"), text='{"test": "test"}')
-
-        # event filtering
-        from bbot.modules.base import BaseModule
-        from bbot.modules.output.base import BaseOutputModule
-        from bbot.modules.report.base import BaseReportModule
-        from bbot.modules.internal.base import BaseInternalModule
-
-        # output module specific event filtering tests
-        base_output_module = BaseOutputModule(scan)
-        base_output_module.watched_events = ["IP_ADDRESS"]
-        localhost = scan.make_event("127.0.0.1", source=scan.root_event)
-        assert base_output_module._event_precheck(localhost)[0] == True
-        localhost._internal = True
-        assert base_output_module._event_precheck(localhost)[0] == False
-        localhost._force_output = True
-        assert base_output_module._event_precheck(localhost)[0] == True
-        localhost._omit = True
-        assert base_output_module._event_precheck(localhost)[0] == False
-
-        # common event filtering tests
-        for module_class in (BaseModule, BaseOutputModule, BaseReportModule, BaseInternalModule):
-            base_module = module_class(scan)
-            localhost2 = scan.make_event("127.0.0.2", source=events.subdomain)
-            localhost2.make_in_scope()
-            # base cases
-            base_module._watched_events = None
-            base_module.watched_events = ["*"]
-            assert base_module._event_precheck(events.emoji)[0] == True
-            base_module._watched_events = None
-            base_module.watched_events = ["IP_ADDRESS"]
-            assert base_module._event_precheck(events.ipv4)[0] == True
-            assert base_module._event_precheck(events.domain)[0] == False
-            assert base_module._event_precheck(events.localhost)[0] == True
-            assert base_module._event_precheck(localhost2)[0] == True
-            # target only
-            base_module.target_only = True
-            assert base_module._event_precheck(localhost2)[0] == False
-            localhost2.add_tag("target")
-            assert base_module._event_precheck(localhost2)[0] == True
-            base_module.target_only = False
-            # special case for IPs and ranges
-            base_module.watched_events = ["IP_ADDRESS", "IP_RANGE"]
-            ip_range = scan.make_event("127.0.0.0/24", dummy=True)
-            localhost4 = scan.make_event("127.0.0.1", source=ip_range)
-            localhost4.make_in_scope()
-            localhost4.module = "plumbus"
-            assert base_module._event_precheck(localhost4)[0] == True
-            localhost4.module = "speculate"
-            assert base_module._event_precheck(localhost4)[0] == False
-
-            # in scope only
-            base_module.in_scope_only = True
-            localhost3 = scan.make_event("127.0.0.2", source=events.subdomain)
-            valid, reason = base_module._event_postcheck(localhost3)
-            if base_module._type == "output":
-                assert valid
-            else:
-                assert not valid
-                assert reason == "it did not meet in_scope_only filter criteria"
-            base_module.in_scope_only = False
-            base_module.scope_distance_modifier = 0
-            localhost4 = scan.make_event("127.0.0.1", source=events.subdomain)
-            valid, reason = base_module._event_postcheck(events.localhost)
-            assert valid
-
-        base_output_module = BaseOutputModule(scan)
-        base_output_module.watched_events = ["IP_ADDRESS"]
+    for http_method in ("GET", "CONNECT", "HEAD", "POST", "PUT", "TRACE", "DEBUG", "PATCH", "DELETE", "OPTIONS"):
+        httpx_mock.add_response(method=http_method, url=re.compile(r".*"), json={"test": "test"})
 
-        scan2 = bbot_scanner(
-            modules=list(set(available_modules + available_internal_modules)),
-            output_modules=list(available_output_modules),
-            config=bbot_config,
-        )
-        scan2.helpers.dns.fallback_nameservers_file = fallback_nameservers
-        patch_commands(scan2)
-        patch_ansible(scan2)
-        scan2.load_modules()
-        scan2.status = "RUNNING"
-
-        # attributes, descriptions, etc.
-        for module_name, module in scan2.modules.items():
-            # flags
-            assert module._type in ("internal", "output", "scan")
-
-        # module preloading
-        all_preloaded = module_loader.preloaded()
-        assert "massdns" in all_preloaded
-        assert "DNS_NAME" in all_preloaded["massdns"]["watched_events"]
-        assert "DNS_NAME" in all_preloaded["massdns"]["produced_events"]
-        assert "subdomain-enum" in all_preloaded["massdns"]["flags"]
-        assert "wordlist" in all_preloaded["massdns"]["config"]
-        assert type(all_preloaded["massdns"]["config"]["max_resolvers"]) == int
-        assert all_preloaded["sslcert"]["deps"]["pip"]
-        assert all_preloaded["sslcert"]["deps"]["apt"]
-        assert all_preloaded["massdns"]["deps"]["ansible"]
-
-        for module_name, preloaded in all_preloaded.items():
-            # either active or passive and never both
-            flags = preloaded.get("flags", [])
-            if preloaded["type"] == "scan":
-                assert ("active" in flags and not "passive" in flags) or (
-                    not "active" in flags and "passive" in flags
-                ), f'module "{module_name}" must have either "active" or "passive" flag'
-                assert preloaded.get("meta", {}).get("description", ""), f"{module_name} must have a description"
-
-            # attribute checks
-            watched_events = preloaded.get("watched_events")
-            produced_events = preloaded.get("produced_events")
-
-            assert type(watched_events) == list
-            assert type(produced_events) == list
-            if not preloaded.get("type", "") in ("internal",):
-                assert watched_events, f"{module_name}.watched_events must not be empty"
-            assert type(watched_events) == list, f"{module_name}.watched_events must be of type list"
-            assert type(produced_events) == list, f"{module_name}.produced_events must be of type list"
-            assert all(
-                [type(t) == str for t in watched_events]
-            ), f"{module_name}.watched_events entries must be of type string"
-            assert all(
-                [type(t) == str for t in produced_events]
-            ), f"{module_name}.produced_events entries must be of type string"
-
-            assert type(preloaded.get("deps_pip", [])) == list, f"{module_name}.deps_pip must be of type list"
-            assert (
-                type(preloaded.get("deps_pip_constraints", [])) == list
-            ), f"{module_name}.deps_pip_constraints must be of type list"
-            assert type(preloaded.get("deps_apt", [])) == list, f"{module_name}.deps_apt must be of type list"
-            assert type(preloaded.get("deps_shell", [])) == list, f"{module_name}.deps_shell must be of type list"
-            assert type(preloaded.get("config", None)) == dict, f"{module_name}.options must be of type list"
-            assert (
-                type(preloaded.get("options_desc", None)) == dict
-            ), f"{module_name}.options_desc must be of type list"
-            # options must have descriptions
-            assert set(preloaded.get("config", {})) == set(
-                preloaded.get("options_desc", {})
-            ), f"{module_name}.options do not match options_desc"
-            # descriptions most not be blank
-            assert all(
-                o for o in preloaded.get("options_desc", {}).values()
-            ), f"{module_name}.options_desc descriptions must not be blank"
-
-        # setups
-        futures = {}
-        for module_name, module in scan2.modules.items():
-            log.info(f"Testing {module_name}.setup()")
-            future = scan2._thread_pool.submit(module.setup)
-            futures[future] = module
-        for future in helpers.as_completed(futures):
-            module = futures[future]
-            result = future.result()
-            if type(result) == tuple:
-                assert len(result) == 2, f"if tuple, {module.name}.setup() return value must have length of 2"
-                status, msg = result
-                assert status in (
-                    True,
-                    False,
-                    None,
-                ), f"if tuple, the first element of {module.name}.setup()'s return value must be either True, False, or None"
-                assert (
-                    type(msg) == str
-                ), f"if tuple, the second element of {module.name}.setup()'s return value must be a message of type str"
-            else:
-                assert result in (
-                    True,
-                    False,
-                    None,
-                ), f"{module.name}.setup() must return a status of either True, False, or None"
-            if result == False:
-                module.set_error_state()
-
-        futures.clear()
-
-        # handle_event / handle_batch
-        futures = {}
-        for module_name, module in scan2.modules.items():
-            module.emit_event = lambda *args, **kwargs: None
-            module._filter = lambda *args, **kwargs: True, ""
-            events_to_submit = [e for e in events.all if e.type in module.watched_events]
-            if module.batch_size > 1:
-                log.info(f"Testing {module_name}.handle_batch()")
-                future = scan2._thread_pool.submit(module.handle_batch, *events_to_submit)
-                futures[future] = module
-            else:
-                for e in events_to_submit:
-                    log.info(f"Testing {module_name}.handle_event()")
-                    future = scan2._thread_pool.submit(module.handle_event, e)
-                    futures[future] = module
-        for future in helpers.as_completed(futures):
-            try:
-                assert future.result() == None
-            except Exception as e:
-                import traceback
-
-                module = futures[future]
-                assert module.errored == True, f'Error in module "{module}": {e}\n{traceback.format_exc()}'
-        futures.clear()
-
-        # finishes
-        futures = {}
-        for module_name, module in scan2.modules.items():
-            log.info(f"Testing {module_name}.finish()")
-            future = scan2._thread_pool.submit(module.finish)
-            futures[future] = module
-        for future in helpers.as_completed(futures):
-            assert future.result() == None
-        futures.clear()
-
-        # cleanups
-        futures = {}
-        for module_name, module in scan2.modules.items():
-            log.info(f"Testing {module_name}.cleanup()")
-            future = scan2._thread_pool.submit(module.cleanup)
-            futures[future] = module
-        for future in helpers.as_completed(futures):
-            assert future.result() == None
-        futures.clear()
-
-        # event filters
-        for module_name, module in scan2.modules.items():
-            log.info(f"Testing {module_name}.filter_event()")
-            result = module.filter_event(events.emoji)
-            with suppress(ValueError, TypeError):
-                result, reason = result
-            assert result in (
-                True,
-                False,
-            ), f"{module_name}.filter_event() must return either True or False"
+    # event filtering
+    from bbot.modules.base import BaseModule
+    from bbot.modules.output.base import BaseOutputModule
+    from bbot.modules.report.base import BaseReportModule
+    from bbot.modules.internal.base import BaseInternalModule
+
+    # output module specific event filtering tests
+    base_output_module = BaseOutputModule(scan)
+    base_output_module.watched_events = ["IP_ADDRESS"]
+    localhost = scan.make_event("127.0.0.1", source=scan.root_event)
+    assert base_output_module._event_precheck(localhost)[0] == True
+    localhost._internal = True
+    assert base_output_module._event_precheck(localhost)[0] == False
+    localhost._force_output = True
+    assert base_output_module._event_precheck(localhost)[0] == True
+    localhost._omit = True
+    assert base_output_module._event_precheck(localhost)[0] == False
+
+    # common event filtering tests
+    for module_class in (BaseModule, BaseOutputModule, BaseReportModule, BaseInternalModule):
+        base_module = module_class(scan)
+        localhost2 = scan.make_event("127.0.0.2", source=events.subdomain)
+        localhost2.set_scope_distance(0)
+        # base cases
+        base_module._watched_events = None
+        base_module.watched_events = ["*"]
+        assert base_module._event_precheck(events.emoji)[0] == True
+        base_module._watched_events = None
+        base_module.watched_events = ["IP_ADDRESS"]
+        assert base_module._event_precheck(events.ipv4)[0] == True
+        assert base_module._event_precheck(events.domain)[0] == False
+        assert base_module._event_precheck(events.localhost)[0] == True
+        assert base_module._event_precheck(localhost2)[0] == True
+        # target only
+        base_module.target_only = True
+        assert base_module._event_precheck(localhost2)[0] == False
+        localhost2.add_tag("target")
+        assert base_module._event_precheck(localhost2)[0] == True
+        base_module.target_only = False
+        # special case for IPs and ranges
+        base_module.watched_events = ["IP_ADDRESS", "IP_RANGE"]
+        ip_range = scan.make_event("127.0.0.0/24", dummy=True)
+        localhost4 = scan.make_event("127.0.0.1", source=ip_range)
+        localhost4.set_scope_distance(0)
+        localhost4.module = "plumbus"
+        assert base_module._event_precheck(localhost4)[0] == True
+        localhost4.module = "speculate"
+        assert base_module._event_precheck(localhost4)[0] == False
+
+        # in scope only
+        base_module.in_scope_only = True
+        localhost3 = scan.make_event("127.0.0.2", source=events.subdomain)
+        valid, reason = await base_module._event_postcheck(localhost3)
+        if base_module._type == "output":
+            assert valid
+        else:
+            assert not valid
+            assert reason == "it did not meet in_scope_only filter criteria"
+        base_module.in_scope_only = False
+        base_module.scope_distance_modifier = 0
+        localhost4 = scan.make_event("127.0.0.1", source=events.subdomain)
+        valid, reason = await base_module._event_postcheck(events.localhost)
+        assert valid
+
+    base_output_module = BaseOutputModule(scan)
+    base_output_module.watched_events = ["IP_ADDRESS"]
+
+    scan2 = bbot_scanner(
+        modules=list(set(available_modules + available_internal_modules)),
+        output_modules=list(available_output_modules),
+        config=bbot_config,
+    )
+    scan2.helpers.dns.fallback_nameservers_file = fallback_nameservers
+    await scan2.load_modules()
+    scan2.status = "RUNNING"
+
+    # attributes, descriptions, etc.
+    for module_name, module in sorted(scan2.modules.items()):
+        # flags
+        assert module._type in ("internal", "output", "scan")
+        # async stuff
+        not_async = []
+        for func_name in ("setup", "ping", "filter_event", "handle_event", "finish", "report", "cleanup"):
+            f = getattr(module, func_name)
+            if not scan2.helpers.is_async_function(f):
+                log.error(f"{f.__qualname__}() is not async")
+                not_async.append(f)
+    assert not any(not_async)
+
+    # module preloading
+    all_preloaded = module_loader.preloaded()
+    assert "massdns" in all_preloaded
+    assert "DNS_NAME" in all_preloaded["massdns"]["watched_events"]
+    assert "DNS_NAME" in all_preloaded["massdns"]["produced_events"]
+    assert "subdomain-enum" in all_preloaded["massdns"]["flags"]
+    assert "wordlist" in all_preloaded["massdns"]["config"]
+    assert type(all_preloaded["massdns"]["config"]["max_resolvers"]) == int
+    assert all_preloaded["sslcert"]["deps"]["pip"]
+    assert all_preloaded["sslcert"]["deps"]["apt"]
+    assert all_preloaded["massdns"]["deps"]["ansible"]
+
+    for module_name, preloaded in all_preloaded.items():
+        # either active or passive and never both
+        flags = preloaded.get("flags", [])
+        if preloaded["type"] == "scan":
+            assert ("active" in flags and not "passive" in flags) or (
+                not "active" in flags and "passive" in flags
+            ), f'module "{module_name}" must have either "active" or "passive" flag'
+            assert preloaded.get("meta", {}).get("description", ""), f"{module_name} must have a description"
+
+        # attribute checks
+        watched_events = preloaded.get("watched_events")
+        produced_events = preloaded.get("produced_events")
+
+        assert type(watched_events) == list
+        assert type(produced_events) == list
+        if not preloaded.get("type", "") in ("internal",):
+            assert watched_events, f"{module_name}.watched_events must not be empty"
+        assert type(watched_events) == list, f"{module_name}.watched_events must be of type list"
+        assert type(produced_events) == list, f"{module_name}.produced_events must be of type list"
+        assert all(
+            [type(t) == str for t in watched_events]
+        ), f"{module_name}.watched_events entries must be of type string"
+        assert all(
+            [type(t) == str for t in produced_events]
+        ), f"{module_name}.produced_events entries must be of type string"
+
+        assert type(preloaded.get("deps_pip", [])) == list, f"{module_name}.deps_pip must be of type list"
+        assert (
+            type(preloaded.get("deps_pip_constraints", [])) == list
+        ), f"{module_name}.deps_pip_constraints must be of type list"
+        assert type(preloaded.get("deps_apt", [])) == list, f"{module_name}.deps_apt must be of type list"
+        assert type(preloaded.get("deps_shell", [])) == list, f"{module_name}.deps_shell must be of type list"
+        assert type(preloaded.get("config", None)) == dict, f"{module_name}.options must be of type list"
+        assert type(preloaded.get("options_desc", None)) == dict, f"{module_name}.options_desc must be of type list"
+        # options must have descriptions
+        assert set(preloaded.get("config", {})) == set(
+            preloaded.get("options_desc", {})
+        ), f"{module_name}.options do not match options_desc"
+        # descriptions most not be blank
+        assert all(
+            o for o in preloaded.get("options_desc", {}).values()
+        ), f"{module_name}.options_desc descriptions must not be blank"
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_python_api.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,39 @@
 from ..bbot_fixtures import *
 
 
-def test_python_api(bbot_config):
+@pytest.mark.asyncio
+async def test_python_api(bbot_config):
     from bbot.scanner import Scanner
 
     # make sure events are properly yielded
     scan1 = Scanner("127.0.0.1", config=bbot_config)
-    events1 = list(scan1.start())
+    events1 = []
+    async for event in scan1.async_start():
+        events1.append(event)
+    assert any("127.0.0.1" == e for e in events1)
+    # make sure output files work
+    scan2 = Scanner("127.0.0.1", config=bbot_config, output_modules=["json"], name="python_api_test")
+    await scan2.async_start_without_generator()
+    out_file = scan2.helpers.scans_dir / "python_api_test" / "output.json"
+    assert list(scan2.helpers.read_file(out_file))
+    # make sure config loads properly
+    bbot_home = "/tmp/.bbot_python_api_test"
+    Scanner("127.0.0.1", config={"home": bbot_home})
+    assert os.environ["BBOT_TOOLS"] == str(Path(bbot_home) / "tools")
+
+
+def test_python_api_sync(bbot_config):
+    from bbot.scanner import Scanner
+
+    # make sure events are properly yielded
+    scan1 = Scanner("127.0.0.1", config=bbot_config)
+    events1 = []
+    for event in scan1.start():
+        events1.append(event)
     assert any("127.0.0.1" == e for e in events1)
     # make sure output files work
     scan2 = Scanner("127.0.0.1", config=bbot_config, output_modules=["json"], name="python_api_test")
     scan2.start_without_generator()
     out_file = scan2.helpers.scans_dir / "python_api_test" / "output.json"
     assert list(scan2.helpers.read_file(out_file))
     # make sure config loads properly
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_scan.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_scan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 from ..bbot_fixtures import *
 
 
-def test_scan(
-    patch_ansible,
-    patch_commands,
+@pytest.mark.asyncio
+async def test_scan(
     events,
     bbot_config,
     helpers,
     neograph,
-    websocketapp,
     monkeypatch,
     bbot_scanner,
 ):
     scan0 = bbot_scanner(
-        "8.8.8.8/31", "evilcorp.com", blacklist=["8.8.8.8/28", "www.evilcorp.com"], config=bbot_config
+        "8.8.8.8/31",
+        "evilcorp.com",
+        blacklist=["8.8.8.8/28", "www.evilcorp.com"],
+        modules=["ipneighbor"],
+        config=bbot_config,
     )
+    await scan0.load_modules()
     assert scan0.whitelisted("8.8.8.8")
     assert scan0.whitelisted("8.8.8.9")
     assert scan0.blacklisted("8.8.8.15")
     assert not scan0.blacklisted("8.8.8.16")
     assert scan0.blacklisted("8.8.8.8/30")
     assert not scan0.blacklisted("8.8.8.8/27")
     assert not scan0.in_scope("8.8.8.8")
     assert scan0.whitelisted("api.evilcorp.com")
     assert scan0.whitelisted("www.evilcorp.com")
     assert not scan0.blacklisted("api.evilcorp.com")
     assert scan0.blacklisted("asdf.www.evilcorp.com")
     assert scan0.in_scope("test.api.evilcorp.com")
     assert not scan0.in_scope("test.www.evilcorp.com")
     assert not scan0.in_scope("www.evilcorp.co.uk")
+    j = scan0.json
+    assert "8.8.8.8/31" in j["targets"]
+    assert "8.8.8.8/31" in j["whitelist"]
+    assert "8.8.8.0/28" in j["blacklist"]
+    assert "ipneighbor" in j["modules"]
 
     scan1 = bbot_scanner("8.8.8.8", whitelist=["8.8.4.4"], config=bbot_config)
     assert not scan1.blacklisted("8.8.8.8")
     assert not scan1.blacklisted("8.8.4.4")
     assert not scan1.whitelisted("8.8.8.8")
     assert scan1.whitelisted("8.8.4.4")
     assert scan1.in_scope("8.8.4.4")
@@ -42,49 +50,26 @@
     assert not scan2.blacklisted("8.8.8.8")
     assert not scan2.blacklisted("8.8.4.4")
     assert scan2.whitelisted("8.8.8.8")
     assert not scan2.whitelisted("8.8.4.4")
     assert scan2.in_scope("8.8.8.8")
     assert not scan2.in_scope("8.8.4.4")
 
-    scan3 = bbot_scanner(
-        "127.0.0.0/30",
-        "127.0.0.2:8443",
-        "https://localhost",
-        "[::1]:80",
-        "http://[::1]:8080",
-        modules=["ipneighbor"],
-        output_modules=list(available_output_modules),
-        config=bbot_config,
-        blacklist=["http://127.0.0.3:8000/asdf"],
-        whitelist=["127.0.0.0/29"],
-    )
-    patch_commands(scan3)
-    patch_ansible(scan3)
-    assert "targets" in scan3.json
-    assert "127.0.0.3" in scan3.target
-    assert "127.0.0.4" not in scan3.target
-    assert "127.0.0.4" in scan3.whitelist
-    assert scan3.whitelisted("127.0.0.4")
-    assert "127.0.0.3" in scan3.blacklist
-    assert scan3.blacklisted("127.0.0.3")
-    assert scan3.in_scope("127.0.0.1")
-    assert not scan3.in_scope("127.0.0.3")
-    scan3.prep()
-    monkeypatch.setattr(scan3.modules["websocket"], "ws", websocketapp())
-    events = list(scan3.start())
-
     # make sure DNS resolution works
     dns_config = OmegaConf.create({"dns_resolution": True})
     dns_config = OmegaConf.merge(bbot_config, dns_config)
     scan4 = bbot_scanner("8.8.8.8", config=dns_config)
-    events = list(scan4.start())
+    events = []
+    async for event in scan4.async_start():
+        events.append(event)
     event_data = [e.data for e in events]
     assert "dns.google" in event_data
 
     # make sure it doesn't work when you turn it off
     no_dns_config = OmegaConf.create({"dns_resolution": False})
     no_dns_config = OmegaConf.merge(bbot_config, no_dns_config)
     scan5 = bbot_scanner("8.8.8.8", config=no_dns_config)
-    events = list(scan5.start())
+    events = []
+    async for event in scan5.async_start():
+        events.append(event)
     event_data = [e.data for e in events]
     assert "dns.google" not in event_data
```

### Comparing `bbot-1.0.5.1665rc0/bbot/test/test_step_2/test_target.py` & `bbot-1.0.5.1793rc0/bbot/test/test_step_1/test_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..bbot_fixtures import *  # noqa: F401
 
 
-def test_target(patch_ansible, bbot_config, bbot_scanner):
+def test_target(bbot_config, bbot_scanner):
     scan1 = bbot_scanner("api.publicapis.org", "8.8.8.8/30", "2001:4860:4860::8888/126", config=bbot_config)
     scan2 = bbot_scanner("8.8.8.8/29", "publicapis.org", "2001:4860:4860::8888/125", config=bbot_config)
     scan3 = bbot_scanner("8.8.8.8/29", "publicapis.org", "2001:4860:4860::8888/125", config=bbot_config)
     scan4 = bbot_scanner("8.8.8.8/29", config=bbot_config)
     scan5 = bbot_scanner(config=bbot_config)
     assert not scan5.target
     assert len(scan1.target) == 9
```

### Comparing `bbot-1.0.5.1665rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1793rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1793rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1793rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1793rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1665rc0/pyproject.toml` & `bbot-1.0.5.1793rc0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1665rc"
+version = "v1.0.5.1793rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
 
@@ -13,36 +13,47 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 omegaconf = "^2.3.0"
 tldextract = "^3.4.0"
 psutil = "^5.9.4"
 wordninja = "^2.0.0"
-requests = "^2.28.2"
 dnspython = "^2.3.0"
 pydantic = "^1.10.6"
 ansible-runner = "^2.3.2"
 deepdiff = "^6.2.3"
 xmltojson = "^2.0.2"
 pycryptodome = "^3.17"
 idna = "^3.4"
 ansible = "^7.3.0"
-websocket-client = "^1.5.1"
 tabulate = "0.8.10"
 cloudcheck = "^2.0.0.34"
+websockets = "^11.0.2"
+httpx = {extras = ["http2"], version = "^0.24.0"}
+pyjwt = "^2.7.0"
+beautifulsoup4 = "^4.12.2"
+lxml = "^4.9.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 flake8 = "^6.0.0"
 black = "^23.1.0"
 pytest-cov = "^4.0.0"
-requests-mock = "^1.10.0"
 poetry-dynamic-versioning = "^0.21.4"
-pytest-httpserver = "^1.0.6"
 pytest-rerunfailures = "^11.1.2"
+pytest-asyncio = "^0.21.0"
+pytest-httpx = "^0.22.0"
+urllib3 = "^2.0.2"
+werkzeug = "^2.3.4"
+pytest-httpserver = "^1.0.8"
+
+[pytest]
+env = [
+    "BBOT_TESTING = True"
+]    
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 119
```

### Comparing `bbot-1.0.5.1665rc0/PKG-INFO` & `bbot-1.0.5.1793rc0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,94 +1,79 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1665rc0
+Version: 1.0.5.1793rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansible (>=7.3.0,<8.0.0)
 Requires-Dist: ansible-runner (>=2.3.2,<3.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cloudcheck (>=2.0.0.34,<3.0.0.0)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
+Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
 Requires-Dist: idna (>=3.4,<4.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: tabulate (==0.8.10)
 Requires-Dist: tldextract (>=3.4.0,<4.0.0)
-Requires-Dist: websocket-client (>=1.5.1,<2.0.0)
+Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Requires-Dist: wordninja (>=2.0.0,<3.0.0)
 Requires-Dist: xmltojson (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/blacklanternsecurity/bbot
 Description-Content-Type: text/markdown
 
-![bbot_banner](https://user-images.githubusercontent.com/20261699/158000235-6c1ace81-a267-4f8e-90a1-f4c16884ebac.png)
-
 # BEE·bot
 ### OSINT automation for hackers.
 
-~~~bash
-pip install bbot
-~~~
+[![Python Version](https://img.shields.io/badge/python-3.9+-FF8400)](https://www.python.org) [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License](https://img.shields.io/badge/license-GPLv3-FF8400.svg)](https://github.com/blacklanternsecurity/bbot/blob/dev/LICENSE) [![Tests](https://github.com/blacklanternsecurity/bbot/actions/workflows/tests.yml/badge.svg?branch=stable)](https://github.com/blacklanternsecurity/bbot/actions?query=workflow%3A"tests") [![Codecov](https://codecov.io/gh/blacklanternsecurity/bbot/branch/dev/graph/badge.svg?token=IR5AZBDM5K)](https://codecov.io/gh/blacklanternsecurity/bbot) [![Discord](https://img.shields.io/discord/859164869970362439)](https://discord.com/invite/PZqkgxu5SA)
 
-[![Python Version](https://img.shields.io/badge/python-3.9+-FF8400)](https://www.python.org) [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License](https://img.shields.io/badge/license-GPLv3-FF8400.svg)](https://github.com/blacklanternsecurity/bbot/blob/dev/LICENSE) [![Tests](https://github.com/blacklanternsecurity/bbot/actions/workflows/tests.yml/badge.svg?branch=stable)](https://github.com/blacklanternsecurity/bbot/actions?query=workflow%3A"tests") [![Codecov](https://codecov.io/gh/blacklanternsecurity/bbot/branch/dev/graph/badge.svg?token=IR5AZBDM5K)](https://codecov.io/gh/blacklanternsecurity/bbot)
+BBOT is a powerful and modular OSINT (Open Source Intelligence) framework designed to map the attack surface of an organization. With BBOT, you can execute the entire OSINT workflow with just a single command.
 
-![bbot-demo](https://user-images.githubusercontent.com/20261699/217346759-d5bf56c3-3936-43f7-ad14-4d73d2cd1417.gif)
+![bbot_banner](https://user-images.githubusercontent.com/20261699/158000235-6c1ace81-a267-4f8e-90a1-f4c16884ebac.png)
+
+BBOT is inspired by [Spiderfoot](https://github.com/smicallef/spiderfoot) but takes it to the next level with features like multi-target scans, lightning-fast asyncio performance, and NLP-powered subdomain mutations. It offers a wide range of functionality, including subdomain enumeration, port scanning, web screenshots, vulnerability scanning, and much more. BBOT has over 80 modules and counting.
 
-### **BBOT** is a **recursive**, **modular** OSINT framework inspired by Spiderfoot.
+Whether you're a pentester, security researcher, or bug bounty hunter, BBOT simplifies and automates the OSINT process so you can focus on the fun part: hacking!
 
-BBOT can execute the entire OSINT process in a single command: subdomain enumeration, port scans, web screenshots (with `gowitness`), vulnerability scanning (with `nuclei`), and much more. BBOT has over **80 modules** and counting.
+https://github.com/blacklanternsecurity/bbot/assets/20261699/ebf2a81e-7530-4a9e-922d-4e62eb949f35
 
-Read our [blog post](https://blog.blacklanternsecurity.com/p/subdomain-enumeration-tool-face-off) to find out why BBOT is the most thorough subdomain enumeration tool available.
+Visualization courtesy of [VivaGraphJS](https://github.com/blacklanternsecurity/bbot-vivagraphjs)
 
-![graphs-small](https://user-images.githubusercontent.com/20261699/199602154-14c71a93-57aa-4ac0-ad81-87ce64fbffc7.png)
+# Getting Started
 
 ## Installation ([pip](https://pypi.org/project/bbot/))
-Note: installing in a virtualenv (e.g. via `pipx`) is recommended
+Note: installing in a virtualenv (e.g. via `pipx`) is recommended. If you need help with installation, please refer to the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#installation).
 ~~~bash
+# Prerequisites:
+# - Linux (Windows and macOS are *not* supported)
+# - Python 3.9 or newer
+
 # stable version
 pip install bbot
 
 # bleeding edge (dev branch)
 pip install --pre bbot
 
 bbot --help
 ~~~
-Prerequisites:
-- Linux (Windows and macOS are *not* supported)
-- Python 3.9 or newer
-
-## Installation ([Docker](https://hub.docker.com/r/blacklanternsecurity/bbot))
-~~~bash
-# bleeding edge (dev)
-docker run -it blacklanternsecurity/bbot --help
-
-# stable
-docker run -it blacklanternsecurity/bbot:stable --help
-
-# note: alternatively there is a helper script that will map docker volumes to persist your BBOT scan data:
-./bbot-docker.sh --help
-~~~
 
-If you need help with installation, please refer to the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#installation).
-
-See also: [Release History](https://github.com/blacklanternsecurity/bbot/wiki/Release-History)
-
-## Scanning with BBOT
-
-### Examples
+## Example Commands
+Note: Scan output, logs, etc. are saved to `~/.bbot`.
 ~~~bash
 # subdomains
 bbot -t evilcorp.com -f subdomain-enum
 
 # subdomains (passive only)
 bbot -t evilcorp.com -f subdomain-enum -rf passive
 
@@ -105,15 +90,39 @@
 # subdomains + emails + cloud + port scan + non-intrusive web + web screenshots + nuclei
 bbot -t evilcorp.com -f subdomain-enum email-enum cloud-enum web-basic -m naabu gowitness nuclei --allow-deadly
 
 # list modules
 bbot -l
 ~~~
 
-### Targets
+## Using BBOT as a Python library
+**Synchronous**
+~~~python
+from bbot.scanner import Scanner
+
+# any number of targets can be specified
+scan = Scanner("example.com", "scanme.nmap.org", modules=["nmap", "sslcert"])
+for event in scan.start():
+    print(event.json())
+~~~
+
+**Asynchronous**
+~~~python
+from bbot.scanner import Scanner
+
+async def main():
+    scan = Scanner("example.com", "scanme.nmap.org", modules=["nmap", "sslcert"])
+    async for event in scan.async_start():
+        print(event.json())
+
+import asyncio
+asyncio.run(main())
+~~~
+
+## Targets
 
 Targets seed a scan with initial data. You can specify an unlimited number of targets, either directly on the command line or in files (or both!). Targets can be any of the following:
 
 - DNS_NAME (`evilcorp.com`)
 - IP_ADDRESS (`1.2.3.4`)
 - IP_RANGE (`1.2.3.0/24`)
 - URL (`https://www.evilcorp.com`)
@@ -122,122 +131,82 @@
 For example, the following scan is totally valid:
 
 ~~~bash
 # multiple targets
 bbot -t evilcorp.com evilcorp.co.uk http://www.evilcorp.cn 1.2.3.0/24 other_targets.txt
 ~~~
 
-#### Whitelists / Blacklists
-
-BBOT's whitelist determines what's considered to be in-scope. By default, the whitelist is simply your target. But if you want more granular scope control, you can override it with `--whitelist` (or add a `--blacklist`).
-
-~~~bash
-# seed a scan with two domains, but only consider assets to be in scope if they are inside 1.2.3.0/24
-bbot -t evilcorp.com evilcorp.co.uk --whitelist 1.2.3.0/24 --blacklist test.evilcorp.com 1.2.3.4 blacklist.txt
-~~~
-
 Visit the wiki for more [tips and tricks](https://github.com/blacklanternsecurity/bbot/wiki#tips-and-tricks).
 
-## Using BBOT as a Python library
-~~~python
-from bbot.scanner import Scanner
-
-# any number of targets can be specified
-scan = Scanner("evilcorp.com", "evilcorp.co.uk", modules=["httpx", "sslcert"])
-for event in scan.start():
-    print(event.json())
-~~~
-
-# Output
-By default, BBOT saves its output in TXT, JSON, and CSV formats. To enable more output modules, you can use `--output-module`.
+## [Docker](https://hub.docker.com/r/blacklanternsecurity/bbot)
+BBOT provides docker images, along with helper script `bbot-docker.sh` to persist your BBOT scan data.
 ~~~bash
-# tee to a file
-bbot -f subdomain-enum -t evilcorp.com | tee evilcorp.txt
+# helper script
+./bbot-docker.sh --help
 
-# output to JSON
-bbot --output-module json -f subdomain-enum -t evilcorp.com | jq
+# bleeding edge (dev)
+docker run -it blacklanternsecurity/bbot --help
 
-# output asset inventory in current directory
-bbot -o . --output-module asset_inventory -f subdomain-enum -t evilcorp.com
+# stable
+docker run -it blacklanternsecurity/bbot:stable --help
 ~~~
-For every scan, BBOT generates a unique and mildly-entertaining name like `demonic_jimmy`. Output for that scan, including the word cloud and any gowitness screenshots, etc., are saved to a folder by that name in `~/.bbot/scans`. The most recent 20 scans are kept, and older ones are removed. You can change the location of BBOT's output with `--output`, and you can also pick a custom scan name with `--name`.
 
-If you reuse a scan name, it will append to its original output files and leverage the previous word cloud.
-
-# Neo4j
-Neo4j is the funnest (and prettiest) way to view and interact with BBOT data.
-
-![neo4j](https://user-images.githubusercontent.com/20261699/182398274-729f3c48-c23c-4db0-8c2e-8b403c1bf790.png)
-
-- You can get Neo4j up and running with a single docker command:
-~~~bash
-docker run -p 7687:7687 -p 7474:7474 -v "$(pwd)/data/:/data/" -e NEO4J_AUTH=neo4j/bbotislife neo4j
-~~~
-- After that, run bbot with `--output-modules neo4j`
-~~~bash
-bbot -f subdomain-enum -t evilcorp.com --output-modules neo4j
-~~~
-- Browse data at http://localhost:7474
 
 # Usage
 ~~~
 $ bbot --help
-usage: bbot [-h] [--help-all] [-t TARGET [TARGET ...]] [-w WHITELIST [WHITELIST ...]] [-b BLACKLIST [BLACKLIST ...]] [--strict-scope] [-n SCAN_NAME] [-m MODULE [MODULE ...]] [-l] [-em MODULE [MODULE ...]]
-            [-f FLAG [FLAG ...]] [-rf FLAG [FLAG ...]] [-ef FLAG [FLAG ...]] [-om MODULE [MODULE ...]] [-o DIR] [-c [CONFIG ...]] [--allow-deadly] [-v] [-d] [-s] [--force] [-y] [--dry-run] [--current-config]
-            [--save-wordcloud FILE] [--load-wordcloud FILE] [--no-deps | --force-deps | --retry-deps | --ignore-failed-deps | --install-all-deps] [-a] [--version]
+usage: bbot [-h] [--help-all] [-t TARGET [TARGET ...]] [-w WHITELIST [WHITELIST ...]] [-b BLACKLIST [BLACKLIST ...]] [--strict-scope] [-m MODULE [MODULE ...]] [-l]
+            [-em MODULE [MODULE ...]] [-f FLAG [FLAG ...]] [-rf FLAG [FLAG ...]] [-ef FLAG [FLAG ...]] [-om MODULE [MODULE ...]] [--allow-deadly] [-n SCAN_NAME] [-o DIR] [-c [CONFIG ...]]
+            [-v] [-d] [-s] [--force] [-y] [--dry-run] [--current-config] [--no-deps | --force-deps | --retry-deps | --ignore-failed-deps | --install-all-deps] [-a] [--version]
 
 Bighuge BLS OSINT Tool
 
 options:
   -h, --help            show this help message and exit
   --help-all            Display full help including module config options
-  -n SCAN_NAME, --name SCAN_NAME
-                        Name of scan (default: random)
+
+Target:
+  -t TARGET [TARGET ...], --targets TARGET [TARGET ...]
+                        Targets to seed the scan
+  -w WHITELIST [WHITELIST ...], --whitelist WHITELIST [WHITELIST ...]
+                        What's considered in-scope (by default it's the same as --targets)
+  -b BLACKLIST [BLACKLIST ...], --blacklist BLACKLIST [BLACKLIST ...]
+                        Don't touch these things
+  --strict-scope        Don't consider subdomains of target/whitelist to be in-scope
+
+Modules:
   -m MODULE [MODULE ...], --modules MODULE [MODULE ...]
-                        Modules to enable. Choices: affiliates,anubisdb,asn,azure_tenant,badsecrets,bevigil,binaryedge,bucket_aws,bucket_azure,bucket_digitalocean,bucket_firebase,bucket_gcp,builtwith,bypass403,c99,censys,certspotter,crobat,crt,dnscommonsrv,dnsdumpster,dnszonetransfer,emailformat,ffuf,ffuf_shortnames,fingerprintx,fullhunt,generic_ssrf,github,gowitness,hackertarget,host_header,httpx,hunt,hunterio,iis_shortnames,ipneighbor,ipstack,leakix,masscan,massdns,naabu,ntlm,nuclei,otx,paramminer_cookies,paramminer_getparams,paramminer_headers,passivetotal,pgp,rapiddns,riddler,robots,secretsdb,securitytrails,shodan_dns,skymem,smuggler,social,sslcert,subdomain_hijack,sublist3r,telerik,threatminer,url_manipulation,urlscan,vhost,viewdns,virustotal,wafw00f,wappalyzer,wayback,zoomeye
+                        Modules to enable. Choices: affiliates,anubisdb,asn,azure_tenant,badsecrets,bevigil,binaryedge,bucket_aws,bucket_azure,bucket_digitalocean,bucket_firebase,bucket_gcp,builtwith,bypass403,c99,censys,certspotter,crobat,crt,dnscommonsrv,dnsdumpster,dnszonetransfer,emailformat,ffuf,ffuf_shortnames,fingerprintx,fullhunt,generic_ssrf,github,gowitness,hackertarget,host_header,httpx,hunt,hunterio,iis_shortnames,ipneighbor,ipstack,leakix,masscan,massdns,naabu,nmap,ntlm,nuclei,otx,paramminer_cookies,paramminer_getparams,paramminer_headers,passivetotal,pgp,rapiddns,riddler,robots,secretsdb,securitytrails,shodan_dns,skymem,smuggler,social,sslcert,subdomain_hijack,sublist3r,telerik,threatminer,url_manipulation,urlscan,vhost,viewdns,virustotal,wafw00f,wappalyzer,wayback,zoomeye
   -l, --list-modules    List available modules.
   -em MODULE [MODULE ...], --exclude-modules MODULE [MODULE ...]
                         Exclude these modules.
   -f FLAG [FLAG ...], --flags FLAG [FLAG ...]
                         Enable modules by flag. Choices: active,affiliates,aggressive,cloud-enum,deadly,email-enum,iis-shortnames,passive,portscan,report,safe,service-enum,slow,social-enum,subdomain-enum,subdomain-hijack,web-basic,web-paramminer,web-screenshots,web-thorough
   -rf FLAG [FLAG ...], --require-flags FLAG [FLAG ...]
-                        Disable modules that don't have these flags (e.g. -rf passive)
+                        Only enable modules with these flags (e.g. -rf passive)
   -ef FLAG [FLAG ...], --exclude-flags FLAG [FLAG ...]
                         Disable modules with these flags. (e.g. -ef aggressive)
   -om MODULE [MODULE ...], --output-modules MODULE [MODULE ...]
                         Output module(s). Choices: asset_inventory,csv,http,human,json,neo4j,python,web_report,websocket
+  --allow-deadly        Enable the use of highly aggressive modules
+
+Scan:
+  -n SCAN_NAME, --name SCAN_NAME
+                        Name of scan (default: random)
   -o DIR, --output-dir DIR
   -c [CONFIG ...], --config [CONFIG ...]
                         custom config file, or configuration options in key=value format: 'modules.shodan.api_key=1234'
-  --allow-deadly        Enable the use of highly aggressive modules
   -v, --verbose         Be more verbose
   -d, --debug           Enable debugging
   -s, --silent          Be quiet
   --force               Run scan even if module setups fail
   -y, --yes             Skip scan confirmation prompt
   --dry-run             Abort before executing scan
   --current-config      Show current config in YAML format
 
-Target:
-  -t TARGET [TARGET ...], --targets TARGET [TARGET ...]
-                        Targets to seed the scan
-  -w WHITELIST [WHITELIST ...], --whitelist WHITELIST [WHITELIST ...]
-                        What's considered in-scope (by default it's the same as --targets)
-  -b BLACKLIST [BLACKLIST ...], --blacklist BLACKLIST [BLACKLIST ...]
-                        Don't touch these things
-  --strict-scope        Don't consider subdomains of target/whitelist to be in-scope
-
-Word cloud:
-  Save/load wordlist of common words gathered during a scan
-
-  --save-wordcloud FILE
-                        Output wordcloud to custom file when the scan completes
-  --load-wordcloud FILE
-                        Load wordcloud from a custom file
-
 Module dependencies:
   Control how modules install their dependencies
 
   --no-deps             Don't install module dependencies
   --force-deps          Force install all module dependencies
   --retry-deps          Try again to install failed module dependencies
   --ignore-failed-deps  Run modules even if they have failed dependencies
@@ -248,20 +217,21 @@
 
   -a, --agent-mode      Start in agent mode
 
 Misc:
   --version             show BBOT version and exit
 ~~~
 
+
 # BBOT Config
-BBOT loads its config from these places in the following order:
+Additional config options (such as API keys, rate limits, user-agent, etc.) can be passed to BBOT via its YAML config. BBOT loads its config beginning from `~/.config/bbot`:
 
 - `~/.config/bbot/bbot.yml` <-- Use this one as your main config
 - `~/.config/bbot/secrets.yml` <-- Use this one for sensitive stuff like API keys
-- command line (`--config`)
+- command line (`--config`) <-- Use this to specify a custom `.yml` or override individual config options
 
 These config files will be automatically created for you when you first run BBOT.
 
 Command-line arguments take precedence over all others. You can give BBOT a custom config file with `--config myconf.yml`, or individual arguments like this: `--config http_proxy=http://127.0.0.1:8080 modules.shodan_dns.api_key=1234`. To display the full and current BBOT config, including any command-line arguments, use `bbot --current-config`.
 
 Note that placing the following in `bbot.yml`:
 ```yaml
@@ -272,14 +242,47 @@
 Is the same as:
 ```bash
 bbot --config modules.shodan.api_key=deadbeef
 ```
 
 For explanations of config options, see `defaults.yml` or the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#yaml-config)
 
+
+# Output
+By default, BBOT saves its output in TXT, JSON, and CSV formats. You can enable other output modules with `--output-module`.
+~~~bash
+# tee to a file
+bbot -f subdomain-enum -t evilcorp.com | tee evilcorp.txt
+
+# output to JSON
+bbot --output-module json -f subdomain-enum -t evilcorp.com | jq
+
+# output asset inventory in current directory
+bbot -o . --output-module asset_inventory -f subdomain-enum -t evilcorp.com
+~~~
+For every scan, BBOT generates a unique and mildly-entertaining name like `demonic_jimmy`. Output for that scan, including scan stats and any gowitness screenshots, etc., are saved to a folder by that name in `~/.bbot/scans`. The most recent 20 scans are kept, and older ones are removed. You can change the location of BBOT's output with `--output`, and you can also pick a custom scan name with `--name`.
+
+If you reuse a scan name, it will append to its original output files and leverage the previous.
+
+## Neo4j
+Neo4j is the funnest (and prettiest) way to view and interact with BBOT data.
+
+![neo4j](https://user-images.githubusercontent.com/20261699/182398274-729f3c48-c23c-4db0-8c2e-8b403c1bf790.png)
+
+- You can get Neo4j up and running with a single docker command:
+~~~bash
+docker run -p 7687:7687 -p 7474:7474 -v "$(pwd)/data/:/data/" -e NEO4J_AUTH=neo4j/bbotislife neo4j
+~~~
+- After that, run bbot with `--output-modules neo4j`
+~~~bash
+bbot -f subdomain-enum -t evilcorp.com --output-modules neo4j
+~~~
+- Browse data at http://localhost:7474
+
+
 # Modules
 
 ### Note: You can find more fun and interesting modules at the [Module Playground](https://github.com/blacklanternsecurity/bbot-module-playground). For instructions on how to install these other modules, see the [wiki](https://github.com/blacklanternsecurity/bbot/wiki#module-playground).
 
 To see modules' options (how to change wordlists, thread count, etc.), use `--help-all`.
 
 ~~~
@@ -336,14 +339,16 @@
 | iis_shortnames       | scan     |         | Check for IIS shortname vulnerability    | active,iis-shortnames,safe,web-          | URL_HINT                                 |
 |                      |          |         |                                          | basic,web-thorough                       |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | masscan              | scan     |         | Port scan IP subnets with masscan        | active,aggressive,portscan               | OPEN_TCP_PORT                            |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | naabu                | scan     |         | Execute port scans with naabu            | active,aggressive,portscan,web-thorough  | OPEN_TCP_PORT                            |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
+| nmap                 | scan     |         | Execute port scans with nmap             | active,aggressive,portscan,web-thorough  | OPEN_TCP_PORT                            |
++----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | ntlm                 | scan     |         | Watch for HTTP endpoints that support    | active,safe,web-basic,web-thorough       | DNS_NAME,FINDING                         |
 |                      |          |         | NTLM authentication                      |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | nuclei               | scan     |         | Fast and customisable vulnerability      | active,aggressive,deadly                 | FINDING,VULNERABILITY                    |
 |                      |          |         | scanner                                  |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | paramminer_cookies   | scan     |         | Smart brute-force to check for common    | active,aggressive,slow,web-paramminer    | FINDING                                  |
@@ -381,15 +386,15 @@
 | vhost                | scan     |         | Fuzz for virtual hosts                   | active,aggressive,deadly,slow            | DNS_NAME,VHOST                           |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | wafw00f              | scan     |         | Web Application Firewall Fingerprinting  | active,aggressive                        | WAF                                      |
 |                      |          |         | Tool                                     |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | wappalyzer           | scan     |         | Extract technologies from web responses  | active,safe,web-basic,web-thorough       | TECHNOLOGY                               |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
-| affiliates           | scan     |         | Summarize affiliate domains at the end   | passive,report,safe                      |                                          |
+| affiliates           | scan     |         | Summarize affiliate domains at the end   | affiliates,passive,report,safe           |                                          |
 |                      |          |         | of a scan                                |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | anubisdb             | scan     |         | Query jldc.me's database for subdomains  | passive,safe,subdomain-enum              | DNS_NAME                                 |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | asn                  | scan     |         | Query ripe and bgpview.io for ASNs       | passive,report,safe,subdomain-enum       | ASN                                      |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | azure_tenant         | scan     |         | Query Azure for tenant sister domains    | affiliates,passive,safe,subdomain-enum   | DNS_NAME                                 |
@@ -470,15 +475,15 @@
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | virustotal           | scan     | X       | Query VirusTotal's API for subdomains    | passive,safe,subdomain-enum              | DNS_NAME                                 |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | wayback              | scan     |         | Query archive.org's API for subdomains   | passive,safe,subdomain-enum              | DNS_NAME,URL_UNVERIFIED                  |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | zoomeye              | scan     | X       | Query ZoomEye's API for subdomains       | affiliates,passive,safe,subdomain-enum   | DNS_NAME                                 |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
-| asset_inventory      | output   |         | Output to an asset inventory style       |                                          |                                          |
+| asset_inventory      | output   |         | Output to an asset inventory style       |                                          | IP_ADDRESS,OPEN_TCP_PORT                 |
 |                      |          |         | flattened CSV file                       |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | csv                  | output   |         | Output to CSV                            |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | http                 | output   |         | Send every event to a custom URL via a   |                                          |                                          |
 |                      |          |         | web request                              |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
@@ -501,17 +506,30 @@
 |                      |          |         | scan data                                |                                          |                                          |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 | speculate            | internal |         | Derive certain event types from others   | passive                                  | DNS_NAME,FINDING,IP_ADDRESS,OPEN_TCP_POR |
 |                      |          |         | by common sense                          |                                          | T                                        |
 +----------------------+----------+---------+------------------------------------------+------------------------------------------+------------------------------------------+
 ~~~
 
-# Credit
 
-BBOT is written by @TheTechromancer. Web hacking in BBOT is made possible by @liquidsec, who wrote most of the web modules and helpers.
+# Acknowledgements
 
-Very special thanks to the following people who made BBOT possible:
+Thanks to all these amazing people for contributing to BBOT! :heart:
 
-- @kerrymilan for his Neo4j and Ansible expertise
+If you have an idea for a feature or run into bugs of any kind, please submit an issue or a PR. We welcome contributions!
+
+<p align="center">
+<a href="https://github.com/blacklanternsecurity/bbot/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=blacklanternsecurity/bbot&max=500">
+</a>
+</p>
+
+Special thanks to the following people who made BBOT possible:
+
+- @TheTechromancer for creating BBOT
+- @liquidsec for his extensive work on BBOT's web hacking features
 - Steve Micallef (@smicallef) for creating Spiderfoot
+- @kerrymilan for his Neo4j and Ansible expertise
 - Aleksei Kornev (@alekseiko) for allowing us ownership of the bbot Pypi repository <3
 
+See also: [Release History](https://github.com/blacklanternsecurity/bbot/wiki/Release-History)
+
```

