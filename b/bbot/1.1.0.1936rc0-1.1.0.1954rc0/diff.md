# Comparing `tmp/bbot-1.1.0.1936rc0.tar.gz` & `tmp/bbot-1.1.0.1954rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.0.1936rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.0.1954rc0.tar", max compression
```

## Comparing `bbot-1.1.0.1936rc0.tar` & `bbot-1.1.0.1954rc0.tar`

### file list

```diff
@@ -1,286 +1,290 @@
--rw-r--r--   0        0        0    32473 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/LICENSE
--rw-r--r--   0        0        0     6679 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-14 14:54:50.423791 bbot-1.1.0.1936rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    14945 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9721 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5290 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1314 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31059 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1496 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1115 2023-07-14 14:54:32.511680 bbot-1.1.0.1936rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       61 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     1993 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5022 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9315 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    28361 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4373 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    35845 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    17481 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9603 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     2240 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3192 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    13681 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8020 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     4094 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3491 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2600 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    26361 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5461 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4851 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5125 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3260 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      908 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5718 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13949 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15858 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2539 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11600 2023-07-14 14:54:32.515680 bbot-1.1.0.1936rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1307 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      807 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7138 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5795 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5997 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9382 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16933 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5280 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1292 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    15167 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      811 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     4269 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     5248 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     1545 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/nsec.py
--rw-r--r--   0        0        0     4993 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11391 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1623 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1845 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3627 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1688 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     8861 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8302 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2007 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1398 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7882 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11061 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3843 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1397 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2291 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-14 14:54:32.519680 bbot-1.1.0.1936rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    24694 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27042 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     4763 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10464 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     3987 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1086 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    15109 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    26755 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7957 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     9758 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     2664 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0     8916 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     1886 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1949 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     2069 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      555 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0      972 2023-07-14 14:54:32.523680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      419 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
--rw-r--r--   0        0        0      659 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1262 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
--rw-r--r--   0        0        0     1116 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     1160 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2107 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10661 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2124 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      611 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     6024 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2370 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-14 14:54:32.527680 bbot-1.1.0.1936rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-14 14:54:32.535680 bbot-1.1.0.1936rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-14 14:54:32.535680 bbot-1.1.0.1936rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2023-07-14 14:54:32.535680 bbot-1.1.0.1936rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2023-07-14 14:54:32.535680 bbot-1.1.0.1936rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2023-07-14 14:54:32.535680 bbot-1.1.0.1936rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-14 14:54:32.535680 bbot-1.1.0.1936rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1537 2023-07-14 14:54:50.419791 bbot-1.1.0.1936rc0/pyproject.toml
--rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 bbot-1.1.0.1936rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/LICENSE
+-rw-r--r--   0        0        0     6679 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/README.md
+-rw-r--r--   0        0        0      211 2023-07-14 20:11:32.531037 bbot-1.1.0.1954rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14945 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9721 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5290 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1314 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31059 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1496 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1115 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       61 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     1993 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5022 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9315 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    28361 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4281 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    36996 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    17481 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     2282 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3192 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    13681 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8020 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     4094 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1202 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     3505 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2600 2023-07-14 20:11:10.882905 bbot-1.1.0.1954rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    26361 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5461 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4851 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5125 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3260 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      908 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5718 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13949 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15858 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2539 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11600 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1307 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      807 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7138 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5795 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5997 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9382 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16428 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5280 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1292 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    15129 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      811 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     4269 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     5248 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     1545 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/nsec.py
+-rw-r--r--   0        0        0     4993 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5163 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      728 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11378 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1845 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1688 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     8861 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-07-14 20:11:10.886905 bbot-1.1.0.1954rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8302 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2007 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1398 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7882 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11061 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3843 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1397 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2291 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    24694 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27985 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     4763 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10464 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     3987 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1103 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    15109 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    27583 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7957 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     9758 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     2664 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-07-14 20:11:10.890905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     8916 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     2757 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     1949 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     2069 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      555 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0      972 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      419 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
+-rw-r--r--   0        0        0      659 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1262 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
+-rw-r--r--   0        0        0     1116 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9253 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2107 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10661 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2124 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      611 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     6024 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2370 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-07-14 20:11:10.894905 bbot-1.1.0.1954rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-07-14 20:11:10.902905 bbot-1.1.0.1954rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-07-14 20:11:10.902905 bbot-1.1.0.1954rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2023-07-14 20:11:10.902905 bbot-1.1.0.1954rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2023-07-14 20:11:10.902905 bbot-1.1.0.1954rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2023-07-14 20:11:10.902905 bbot-1.1.0.1954rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-07-14 20:11:10.906905 bbot-1.1.0.1954rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1576 2023-07-14 20:11:32.531037 bbot-1.1.0.1954rc0/pyproject.toml
+-rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 bbot-1.1.0.1954rc0/PKG-INFO
```

### Comparing `bbot-1.1.0.1936rc0/LICENSE` & `bbot-1.1.0.1954rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/README.md` & `bbot-1.1.0.1954rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/agent/agent.py` & `bbot-1.1.0.1954rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/cli.py` & `bbot-1.1.0.1954rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.0.1954rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/configurator/args.py` & `bbot-1.1.0.1954rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/configurator/environ.py` & `bbot-1.1.0.1954rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/configurator/files.py` & `bbot-1.1.0.1954rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/errors.py` & `bbot-1.1.0.1954rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/event/base.py` & `bbot-1.1.0.1954rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/event/helpers.py` & `bbot-1.1.0.1954rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/flags.py` & `bbot-1.1.0.1954rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/cache.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/command.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/diff.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/dns.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/files.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/helper.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import logging
 from pathlib import Path
-from threading import Lock
 
 from . import misc
 from .dns import DNSHelper
 from .web import WebHelper
 from .diff import HttpCompare
 from .wordcloud import WordCloud
 from .cloud import CloudProviders
@@ -38,16 +37,14 @@
         self.wordlist_dir = Path(__file__).parent.parent.parent / "wordlists"
         self.current_dir = Path.cwd()
         self.keep_old_scans = self.config.get("keep_scans", 20)
         self.mkdir(self.cache_dir)
         self.mkdir(self.temp_dir)
         self.mkdir(self.tools_dir)
         self.mkdir(self.lib_dir)
-        self._futures = set()
-        self._future_lock = Lock()
 
         self.dns = DNSHelper(self)
         self.web = WebHelper(self)
         self.depsinstaller = DepsInstaller(self)
         self.word_cloud = WordCloud(self)
         self.dummy_modules = {}
```

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/logger.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/misc.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 import xml.etree.ElementTree as ET
 from collections.abc import Mapping
 from hashlib import sha1 as hashlib_sha1
 from urllib.parse import urlparse, quote, unquote, urlunparse  # noqa F401
 from asyncio import as_completed, create_task, sleep, wait_for  # noqa
 
 from .url import *  # noqa F401
-from . import regexes
 from .. import errors
 from .punycode import *  # noqa F401
 from .logger import log_to_stderr
+from . import regexes as bbot_regexes
 from .names_generator import random_name, names, adjectives  # noqa F401
 
 log = logging.getLogger("bbot.core.helpers.misc")
 
 
 def is_domain(d):
     """
@@ -67,20 +67,20 @@
 
 
 def is_ptr(d):
     """
     "wsc-11-22-33-44.evilcorp.com" --> True
     "www2.evilcorp.com" --> False
     """
-    return bool(regexes.ptr_regex.search(str(d)))
+    return bool(bbot_regexes.ptr_regex.search(str(d)))
 
 
 def is_url(u):
     u = str(u)
-    for r in regexes.event_type_regexes["URL"]:
+    for r in bbot_regexes.event_type_regexes["URL"]:
         if r.match(u):
             return True
     return False
 
 
 uri_regex = re.compile(r"^([a-z0-9]{2,20})://", re.I)
 
@@ -186,15 +186,21 @@
 
 
 def split_domain(hostname):
     """
     "www.internal.evilcorp.co.uk" --> ("www.internal", "evilcorp.co.uk")
     """
     parsed = tldextract(hostname)
-    return (parsed.subdomain, parsed.registered_domain)
+    subdomain = parsed.subdomain
+    domain = parsed.registered_domain
+    if not domain:
+        split = hostname.split(".")
+        subdomain = ".".join(split[:-2])
+        domain = ".".join(split[-2:])
+    return (subdomain, domain)
 
 
 def domain_stem(domain):
     """
     An abbreviated representation of hostname that removes the TLD
         www.evilcorp.com --> www.evilcorp
     """
@@ -216,17 +222,17 @@
     return p and p.isdigit() and 0 <= int(p) <= 65535
 
 
 def is_dns_name(d):
     if is_ip(d):
         return False
     d = smart_decode(d)
-    if regexes.hostname_regex.match(d):
+    if bbot_regexes.hostname_regex.match(d):
         return True
-    if regexes.dns_name_regex.match(d):
+    if bbot_regexes.dns_name_regex.match(d):
         return True
     return False
 
 
 def is_ip(d, version=None):
     """
     "192.168.1.1" --> True
@@ -416,49 +422,49 @@
         tags.add(current_element.tag)
         for child in current_element:
             stack.append(child)
     return tags
 
 
 def extract_params_html(html_data):
-    input_tag = regexes.input_tag_regex.findall(html_data)
+    input_tag = bbot_regexes.input_tag_regex.findall(html_data)
 
     for i in input_tag:
         log.debug(f"FOUND PARAM ({i}) IN INPUT TAGS")
         yield i
 
     # check for jquery get parameters
-    jquery_get = regexes.jquery_get_regex.findall(html_data)
+    jquery_get = bbot_regexes.jquery_get_regex.findall(html_data)
 
     for i in jquery_get:
         log.debug(f"FOUND PARAM ({i}) IN JQUERY GET PARAMS")
         yield i
 
     # check for jquery post parameters
-    jquery_post = regexes.jquery_post_regex.findall(html_data)
+    jquery_post = bbot_regexes.jquery_post_regex.findall(html_data)
     if jquery_post:
         for i in jquery_post:
             for x in i.split(","):
                 s = x.split(":")[0].rstrip()
                 log.debug(f"FOUND PARAM ({s}) IN A JQUERY POST PARAMS")
                 yield s
 
-    a_tag = regexes.a_tag_regex.findall(html_data)
+    a_tag = bbot_regexes.a_tag_regex.findall(html_data)
     for s in a_tag:
         log.debug(f"FOUND PARAM ({s}) IN A TAG GET PARAMS")
         yield s
 
 
 def extract_words(data, acronyms=True, wordninja=True, model=None, max_length=100, word_regexes=None):
     """
     Intelligently extract words from given data
     Returns set() of extracted words
     """
     if word_regexes is None:
-        word_regexes = regexes.word_regexes
+        word_regexes = bbot_regexes.word_regexes
     words = set()
     data = smart_decode(data)
     for r in word_regexes:
         for word in set(r.findall(data)):
             # blacklanternsecurity
             if len(word) <= max_length:
                 words.add(word)
@@ -673,14 +679,47 @@
     elif isinstance(d, str):
         for find, replace in kwargs.items():
             find = "#{" + str(find) + "}"
             d = d.replace(find, replace)
     return d
 
 
+def search_dict_values(d, *regexes):
+    """
+    Recursively search a dictionary's values based on regexes
+
+    dict_to_search = {
+        "key1": {
+            "key2": [
+                {
+                    "key3": "A URL: https://www.evilcorp.com"
+                }
+            ]
+        }
+    })
+
+    search_dict_values(dict_to_search, url_regexes) --> "https://www.evilcorp.com"
+    """
+    results = set()
+    if isinstance(d, str):
+        for r in regexes:
+            for match in r.finditer(d):
+                result = match.group()
+                h = hash(result)
+                if h not in results:
+                    results.add(h)
+                    yield result
+    elif isinstance(d, dict):
+        for _, v in d.items():
+            yield from search_dict_values(v, *regexes)
+    elif isinstance(d, list):
+        for v in d:
+            yield from search_dict_values(v, *regexes)
+
+
 def filter_dict(d, *key_names, fuzzy=False, invert=False, exclude_keys=None, prev_key=None):
     """
     Recursively filter a dictionary based on key names
     filter_dict({"key1": "test", "key2": "asdf"}, "key2")
         --> {"key2": "asdf"}
     """
     if exclude_keys is None:
@@ -855,15 +894,15 @@
             msg = f"Failed to delete directory: {path}, {e}"
             if raise_error:
                 raise errors.DirectoryDeletionError()
             log.warning(msg)
 
 
 def extract_emails(s):
-    for email in regexes.email_regex.findall(smart_decode(s)):
+    for email in bbot_regexes.email_regex.findall(smart_decode(s)):
         yield email.lower()
 
 
 def can_sudo_without_password():
     """
     Return True if the current user can sudo without a password
     """
```

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/modules.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/punycode.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/regexes.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,19 +23,24 @@
 ipv6_regex = re.compile(_ipv6_regex, re.I)
 _dns_name_regex = r"(?:(?:[\w-]+)\.)+(?:[^\W_0-9]{2,20})"
 _hostname_regex = r"^[\w-]+$"
 _email_regex = r"(?:[^\W_][\w\-\.\+]{,100})@(?:\w[\w\-\._]{,100})\.(?:[^\W_0-9]{2,8})"
 email_regex = re.compile(_email_regex, re.I)
 _ptr_regex = r"(?:[0-9]{1,3}[-_\.]){3}[0-9]{1,3}"
 ptr_regex = re.compile(_ptr_regex)
+_url_regexes = (
+    r"https?://((?:\w|\w[\w\-]*\w)[\.]?)+(?:\w[\w\-]*\w|\w)(?::[0-9]{1,5})?.*$",
+    r"https?://\[" + _ipv6_regex + r"\](?::[0-9]{1,5})?.*$",
+)
+url_regexes = list(re.compile(r, re.I) for r in _url_regexes)
 
 event_type_regexes = OrderedDict(
-    [
+    (
         (k, tuple(re.compile(r, re.I) for r in regexes))
-        for k, regexes in [
+        for k, regexes in (
             (
                 "DNS_NAME",
                 (r"^" + _dns_name_regex + r"$",),
             ),
             (
                 "EMAIL_ADDRESS",
                 (r"^" + _email_regex + r"$",),
@@ -45,21 +50,18 @@
                 (
                     r"^((?:\w|\w[\w\-]*\w)[\.]?)+(?:\w[\w\-]*\w|\w):[0-9]{1,5}$",
                     r"^\[" + _ipv6_regex + r"\]:[0-9]{1,5}$",
                 ),
             ),
             (
                 "URL",
-                (
-                    r"https?://((?:\w|\w[\w\-]*\w)[\.]?)+(?:\w[\w\-]*\w|\w)(?::[0-9]{1,5})?.*$",
-                    r"https?://\[" + _ipv6_regex + r"\](?::[0-9]{1,5})?.*$",
-                ),
+                _url_regexes,
             ),
-        ]
-    ]
+        )
+    )
 )
 
 event_id_regex = re.compile(r"[0-9a-f]{40}:[A-Z0-9_]+")
 dns_name_regex = re.compile(_dns_name_regex, re.I)
 scan_name_regex = re.compile(r"[a-z]{3,20}_[a-z]{3,20}")
 hostname_regex = re.compile(_hostname_regex, re.I)
```

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/url.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/validators.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/web.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.0.1954rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/core/logger/logger.py` & `bbot-1.1.0.1954rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/db/neo4j.py` & `bbot-1.1.0.1954rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/defaults.yml` & `bbot-1.1.0.1954rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/anubisdb.py` & `bbot-1.1.0.1954rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.0.1954rc0/bbot/modules/azure_tenant.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .viewdns import viewdns
 
 
 class azure_tenant(viewdns):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    flags = ["affiliates", "subdomain-enum", "passive", "safe"]
+    flags = ["affiliates", "subdomain-enum", "cloud-enum", "passive", "safe"]
     meta = {"description": "Query Azure for tenant sister domains"}
 
     base_url = "https://autodiscover-s.outlook.com"
     in_scope_only = True
 
     async def setup(self):
         self.processed = set()
```

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/badsecrets.py` & `bbot-1.1.0.1954rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/base.py` & `bbot-1.1.0.1954rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/bevigil.py` & `bbot-1.1.0.1954rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/binaryedge.py` & `bbot-1.1.0.1954rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/bucket_aws.py` & `bbot-1.1.0.1954rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.0.1954rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.0.1954rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.0.1954rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/bucket_gcp.py` & `bbot-1.1.0.1954rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/builtwith.py` & `bbot-1.1.0.1954rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/bypass403.py` & `bbot-1.1.0.1954rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/c99.py` & `bbot-1.1.0.1954rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/censys.py` & `bbot-1.1.0.1954rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/certspotter.py` & `bbot-1.1.0.1954rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/columbus.py` & `bbot-1.1.0.1954rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/crobat.py` & `bbot-1.1.0.1954rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/crt.py` & `bbot-1.1.0.1954rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.0.1954rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.0.1954rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.0.1954rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.0.1954rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.0.1954rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.1.0.1954rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/emailformat.py` & `bbot-1.1.0.1954rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.0.1954rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.0.1954rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/fullhunt.py` & `bbot-1.1.0.1954rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.0.1954rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/git.py` & `bbot-1.1.0.1954rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/github.py` & `bbot-1.1.0.1954rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/gowitness.py` & `bbot-1.1.0.1954rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/hackertarget.py` & `bbot-1.1.0.1954rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/host_header.py` & `bbot-1.1.0.1954rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/httpx.py` & `bbot-1.1.0.1954rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/hunt.py` & `bbot-1.1.0.1954rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/hunterio.py` & `bbot-1.1.0.1954rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.0.1954rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/internal/base.py` & `bbot-1.1.0.1954rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.0.1954rc0/bbot/modules/internal/excavate.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,23 +36,16 @@
         pass
 
 
 class HostnameExtractor(BaseExtractor):
     regexes = {}
 
     def __init__(self, excavate):
-        dns_targets = set(t.host for t in excavate.scan.target if t.host and isinstance(t.host, str))
-        dns_whitelist = set(t.host for t in excavate.scan.whitelist if t.host and isinstance(t.host, str))
-        dns_targets.update(dns_whitelist)
-        dns_targets = sorted(dns_targets, key=len)
-        dns_targets_set = set()
-        for i, t in enumerate(dns_targets):
-            if not any(x in dns_targets_set for x in excavate.helpers.domain_parents(t, include_self=True)):
-                dns_targets_set.add(t)
-                self.regexes[f"dns_name_{i+1}"] = r"((?:(?:[\w-]+)\.)+" + re.escape(t) + ")"
+        for i, r in enumerate(excavate.scan.dns_regexes):
+            self.regexes[f"dns_name_{i+1}"] = r.pattern
         super().__init__(excavate)
 
     def report(self, result, name, event, **kwargs):
         self.excavate.emit_event(result, "DNS_NAME", source=event)
 
 
 class URLExtractor(BaseExtractor):
```

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.0.1954rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.0.1954rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/ipstack.py` & `bbot-1.1.0.1954rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/leakix.py` & `bbot-1.1.0.1954rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/masscan.py` & `bbot-1.1.0.1954rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/massdns.py` & `bbot-1.1.0.1954rc0/bbot/modules/massdns.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,16 +190,14 @@
             "massdns",
             "-r",
             self.resolver_file,
             "-s",
             self.max_resolvers,
             "-t",
             "A",
-            "-t",
-            "AAAA",
             "-o",
             "J",
             "-q",
         )
         subdomains = self.gen_subdomains(subdomains, domain)
         hosts_yielded = set()
         async for line in self.helpers.run_live(command, stderr=subprocess.DEVNULL, input=subdomains):
```

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/myssl.py` & `bbot-1.1.0.1954rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/naabu.py` & `bbot-1.1.0.1954rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/nmap.py` & `bbot-1.1.0.1954rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/nsec.py` & `bbot-1.1.0.1954rc0/bbot/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/ntlm.py` & `bbot-1.1.0.1954rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/otx.py` & `bbot-1.1.0.1954rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/asset_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         for asset in sorted(self.assets.values(), key=sort_key):
             findings_and_vulns = asset.findings.union(asset.vulnerabilities)
             ports = getattr(asset, "ports", set())
             ports = [str(p) for p in sorted([int(p) for p in asset.ports])]
             ips = sorted([str(i) for i in getattr(asset, "ip_addresses", [])])
             host = getattr(asset, "host", "")
             if host:
-                domain = self.helpers.tldextract(host).registered_domain
+                _, domain = self.helpers.split_domain(host)
                 if domain:
                     increment_stat("Domains", domain)
             for ip in ips:
                 net = ipaddress.ip_network(f"{ip}/{self.summary_netmask}", strict=False)
                 increment_stat("IP Addresses", str(net))
             for port in ports:
                 increment_stat("Open Ports", port)
```

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/base.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/csv.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/http.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/human.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/json.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/web_report.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/output/websocket.py` & `bbot-1.1.0.1954rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.0.1954rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.0.1954rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.0.1954rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/passivetotal.py` & `bbot-1.1.0.1954rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/pgp.py` & `bbot-1.1.0.1954rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/rapiddns.py` & `bbot-1.1.0.1954rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.0.1954rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/report/asn.py` & `bbot-1.1.0.1954rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/riddler.py` & `bbot-1.1.0.1954rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/robots.py` & `bbot-1.1.0.1954rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/secretsdb.py` & `bbot-1.1.0.1954rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/securitytrails.py` & `bbot-1.1.0.1954rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.0.1954rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/skymem.py` & `bbot-1.1.0.1954rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/smuggler.py` & `bbot-1.1.0.1954rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/social.py` & `bbot-1.1.0.1954rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/sslcert.py` & `bbot-1.1.0.1954rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.1.0.1954rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/telerik.py` & `bbot-1.1.0.1954rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/threatminer.py` & `bbot-1.1.0.1954rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.0.1954rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/urlscan.py` & `bbot-1.1.0.1954rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/viewdns.py` & `bbot-1.1.0.1954rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/virustotal.py` & `bbot-1.1.0.1954rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/wafw00f.py` & `bbot-1.1.0.1954rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.0.1954rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/wayback.py` & `bbot-1.1.0.1954rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/modules/zoomeye.py` & `bbot-1.1.0.1954rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.0.1954rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/scanner/manager.py` & `bbot-1.1.0.1954rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/scanner/scanner.py` & `bbot-1.1.0.1954rc0/bbot/scanner/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import asyncio
 import logging
 import traceback
 import contextlib
 from sys import exc_info
 from pathlib import Path
 import multiprocessing as mp
@@ -175,14 +176,16 @@
             mp.set_start_method("spawn")
         except Exception:
             self.warning(f"Failed to set multiprocessing spawn method. This may negatively affect performance.")
         self.process_pool = ProcessPoolExecutor()
 
         self._stopping = False
 
+        self._dns_regexes = None
+
     def _on_keyboard_interrupt(self, loop, event):
         self.stop()
 
     async def prep(self):
         # event = asyncio.Event()
         # self._loop.add_signal_handler(signal.SIGINT, self._on_keyboard_interrupt, loop, event)
 
@@ -738,14 +741,34 @@
     def run_in_executor_mp(self, callback, *args, **kwargs):
         """
         Same as run_in_executor() except with a process pool executor
         """
         callback = partial(callback, **kwargs)
         return self._loop.run_in_executor(self.process_pool, callback, *args)
 
+    @property
+    def dns_regexes(self):
+        """
+        Return a list of regexes for extracting target hostnames
+        """
+        if self._dns_regexes is None:
+            dns_targets = set(t.host for t in self.target if t.host and isinstance(t.host, str))
+            dns_whitelist = set(t.host for t in self.whitelist if t.host and isinstance(t.host, str))
+            dns_targets.update(dns_whitelist)
+            dns_targets = sorted(dns_targets, key=len)
+            dns_targets_set = set()
+            dns_regexes = []
+            for t in dns_targets:
+                if not any(x in dns_targets_set for x in self.helpers.domain_parents(t, include_self=True)):
+                    dns_targets_set.add(t)
+                    dns_regexes.append(re.compile(r"((?:(?:[\w-]+)\.)+" + re.escape(t) + ")", re.I))
+            self._dns_regexes = dns_regexes
+
+        return self._dns_regexes
+
     def _handle_exception(self, e, context="scan", finally_callback=None):
         if callable(context):
             context = f"{context.__qualname__}()"
         filename, lineno, funcname = self.helpers.get_traceback_details(e)
         exception_chain = self.helpers.get_exception_chain(e)
         if any(isinstance(exc, KeyboardInterrupt) for exc in exception_chain):
             log.debug(f"Interrupted")
```

### Comparing `bbot-1.1.0.1936rc0/bbot/scanner/stats.py` & `bbot-1.1.0.1954rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/scanner/target.py` & `bbot-1.1.0.1954rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/scripts/docs.py` & `bbot-1.1.0.1954rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.0.1954rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/conftest.py` & `bbot-1.1.0.1954rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/run_tests.sh` & `bbot-1.1.0.1954rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test.conf` & `bbot-1.1.0.1954rc0/bbot/test/test.conf`

 * *Files 10% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 debug: true
 dns_wildcard_ignore:
   - blacklanternsecurity.com
   - fakedomain
   - notreal
   - google
   - google.com
-  - example.com
+  - example.com
+  - evilcorp.com
```

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import ipaddress
 
 from ..bbot_fixtures import *
 
 
 @pytest.mark.asyncio
-async def test_helpers(helpers, scan, bbot_scanner, bbot_config, bbot_httpserver):
+async def test_helpers_misc(helpers, scan, bbot_scanner, bbot_config, bbot_httpserver):
     ### URL ###
     bad_urls = (
         "http://e.co/index.html",
         "http://e.co/u/1111/info",
         "http://e.co/u/2222/info",
         "http://e.co/u/3333/info",
         "http://e.co/u/4444/info",
@@ -102,14 +102,20 @@
     assert tuple(helpers.extract_emails("asdf@asdf.com\nT@t.Com&a=a@a.com__ b@b.com")) == (
         "asdf@asdf.com",
         "t@t.com",
         "a@a.com",
         "b@b.com",
     )
 
+    assert helpers.split_domain("www.evilcorp.co.uk") == ("www", "evilcorp.co.uk")
+    assert helpers.split_domain("asdf.www.test.notreal") == ("asdf.www", "test.notreal")
+    assert helpers.split_domain("www.test.notreal") == ("www", "test.notreal")
+    assert helpers.split_domain("test.notreal") == ("", "test.notreal")
+    assert helpers.split_domain("notreal") == ("", "notreal")
+
     assert helpers.split_host_port("https://evilcorp.co.uk") == ("evilcorp.co.uk", 443)
     assert helpers.split_host_port("http://evilcorp.co.uk:666") == ("evilcorp.co.uk", 666)
     assert helpers.split_host_port("evilcorp.co.uk:666") == ("evilcorp.co.uk", 666)
     assert helpers.split_host_port("evilcorp.co.uk") == ("evilcorp.co.uk", None)
     assert helpers.split_host_port("d://wat:wat") == ("wat", None)
     assert helpers.split_host_port("https://[dead::beef]:8338") == (ipaddress.ip_address("dead::beef"), 8338)
     extracted_words = helpers.extract_words("blacklanternsecurity")
@@ -150,14 +156,27 @@
 
     assert list(helpers.search_dict_by_key("asdf", {"asdf": "fdsa", 4: [{"asdf": 5}]})) == ["fdsa", 5]
     assert list(helpers.search_dict_by_key("asdf", {"wat": {"asdf": "fdsa"}})) == ["fdsa"]
     assert list(helpers.search_dict_by_key("asdf", [{"wat": {"nope": 1}}, {"wat": [{"asdf": "fdsa"}]}])) == ["fdsa"]
     assert not list(helpers.search_dict_by_key("asdf", [{"wat": {"nope": 1}}, {"wat": [{"fdsa": "asdf"}]}]))
     assert not list(helpers.search_dict_by_key("asdf", "asdf"))
 
+    from bbot.core.helpers.regexes import url_regexes
+
+    dict_to_search = {
+        "key1": {
+            "key2": [{"key3": "A url of some kind: https://www.evilcorp.com/asdf"}],
+            "key4": "A url of some kind: https://www.evilcorp.com/fdsa",
+        }
+    }
+    assert set(helpers.search_dict_values(dict_to_search, *url_regexes)) == {
+        "https://www.evilcorp.com/asdf",
+        "https://www.evilcorp.com/fdsa",
+    }
+
     filtered_dict = helpers.filter_dict(
         {"modules": {"c99": {"api_key": "1234", "filterme": "asdf"}, "ipneighbor": {"test": "test"}}}, "api_key"
     )
     assert "api_key" in filtered_dict["modules"]["c99"]
     assert "filterme" not in filtered_dict["modules"]["c99"]
     assert "ipneighbor" not in filtered_dict["modules"]
```

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 from .base import ModuleTestBase
 
 
 class TestAsset_Inventory(ModuleTestBase):
-    targets = ["8.8.8.8"]
+    targets = ["127.0.0.1", "bbottest.notreal"]
     scan_name = "asset_inventory_test"
-    config_overrides = {"dns_resolution": True}
+    config_overrides = {"dns_resolution": True, "internal_modules": {"speculate": {"ports": "9999"}}}
     modules_overrides = ["asset_inventory", "speculate", "sslcert"]
 
+    async def setup_before_prep(self, module_test):
+        old_resolve_fn = module_test.scan.helpers.dns.resolve_event
+
+        async def resolve_event(event, minimal=False):
+            if event.data == "www.bbottest.notreal":
+                return ["a-record"], True, False, {"A": {"127.0.0.1"}}
+            elif event.data == "127.0.0.1":
+                return ["ptr-record"], False, False, {"PTR": {"asdf.bbottest.notreal"}}
+            return await old_resolve_fn(event, minimal)
+
+        module_test.monkeypatch.setattr(module_test.scan.helpers.dns, "resolve_event", resolve_event)
+
     def check(self, module_test, events):
-        assert any(e.type == "OPEN_TCP_PORT" for e in events), "No open port found"
-        assert any(e.type == "DNS_NAME" for e in events), "No DNS name found"
+        assert any(e.data == "127.0.0.1:9999" for e in events), "No open port found"
+        assert any(e.data == "www.bbottest.notreal" for e in events), "No DNS name found"
         filename = next(module_test.scan.home.glob("asset-inventory.csv"))
         with open(filename) as f:
-            assert "8.8.8.8,,8.8.8.8" in f.read()
+            content = f.read()
+            assert "www.bbottest.notreal,,127.0.0.1" in content
         filename = next(module_test.scan.home.glob("asset-inventory-ip-addresses-table*.txt"))
         with open(filename) as f:
-            assert "8.8.0.0/16" in f.read()
+            assert "127.0.0.0/16" in f.read()
         filename = next(module_test.scan.home.glob("asset-inventory-domains-table*.txt"))
         with open(filename) as f:
-            assert "dns.google" in f.read()
+            content = f.read()
+            assert "bbottest.notreal" in content
 
 
 class TestAsset_InventoryEmitPrevious(TestAsset_Inventory):
     config_overrides = {"dns_resolution": True, "output_modules": {"asset_inventory": {"use_previous": True}}}
     modules_overrides = ["asset_inventory"]
 
     def check(self, module_test, events):
-        assert any(e.type == "OPEN_TCP_PORT" for e in events), "No open port found"
-        assert any(e.type == "DNS_NAME" for e in events), "No DNS name found"
+        assert any(e.data == "www.bbottest.notreal:9999" for e in events), "No open port found"
+        assert any(e.data == "www.bbottest.notreal" for e in events), "No DNS name found"
         filename = next(module_test.scan.home.glob("asset-inventory.csv"))
         with open(filename) as f:
-            assert "8.8.8.8,,8.8.8.8" in f.read()
+            content = f.read()
+            assert "www.bbottest.notreal,,127.0.0.1" in content
         filename = next(module_test.scan.home.glob("asset-inventory-ip-addresses-table*.txt"))
         with open(filename) as f:
-            assert "8.8.0.0/16" in f.read()
+            assert "127.0.0.0/16" in f.read()
         filename = next(module_test.scan.home.glob("asset-inventory-domains-table*.txt"))
         with open(filename) as f:
-            assert "dns.google" in f.read()
+            content = f.read()
+            assert "bbottest.notreal" in content
```

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.0.1954rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/testsslcert.pem` & `bbot-1.1.0.1954rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/test/testsslkey.pem` & `bbot-1.1.0.1954rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.0.1954rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.0.1954rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.0.1954rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.0.1954rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.0.1954rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.0.1954rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1936rc0/pyproject.toml` & `bbot-1.1.0.1954rc0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.0.1936rc"
+version = "v1.1.0.1954rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
 
@@ -24,33 +24,34 @@
 xmltojson = "^2.0.2"
 pycryptodome = "^3.17"
 idna = "^3.4"
 ansible = "^7.3.0"
 tabulate = "0.8.10"
 cloudcheck = "^2.0.0.34"
 websockets = "^11.0.2"
-httpx = {extras = ["http2"], version = "^0.24.0"}
 pyjwt = "^2.7.0"
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.2"
+httpx = {extras = ["http2"], version = "^0.24.1"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 flake8 = "^6.0.0"
 black = "^23.1.0"
 pytest-cov = "^4.0.0"
 poetry-dynamic-versioning = "^0.21.4"
 pytest-rerunfailures = "^11.1.2"
 pytest-asyncio = "^0.21.0"
-pytest-httpx = "^0.22.0"
 urllib3 = "^2.0.2"
 werkzeug = "^2.3.4"
 pytest-httpserver = "^1.0.8"
+pytest-env = "^0.8.2"
+pytest-httpx = "^0.22.0"
 
-[pytest]
+[tool.pytest.ini_options]
 env = [
     "BBOT_TESTING = True"
 ]    
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `bbot-1.1.0.1936rc0/PKG-INFO` & `bbot-1.1.0.1954rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.0.1936rc0
+Version: 1.1.0.1954rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansible (>=7.3.0,<8.0.0)
 Requires-Dist: ansible-runner (>=2.3.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cloudcheck (>=2.0.0.34,<3.0.0.0)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
-Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
+Requires-Dist: httpx[http2] (>=0.24.1,<0.25.0)
 Requires-Dist: idna (>=3.4,<4.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
```

