# Comparing `tmp/bbot-1.1.0.1908rc0.tar.gz` & `tmp/bbot-1.1.0.1924rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.0.1908rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.0.1924rc0.tar", max compression
```

## Comparing `bbot-1.1.0.1908rc0.tar` & `bbot-1.1.0.1924rc0.tar`

### file list

```diff
@@ -1,286 +1,286 @@
--rw-r--r--   0        0        0    32473 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/LICENSE
--rw-r--r--   0        0        0     6762 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-12 21:43:23.548843 bbot-1.1.0.1908rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    14945 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9721 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5290 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1314 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31059 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1496 2023-07-12 21:42:54.062900 bbot-1.1.0.1908rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1115 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       61 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     1993 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5022 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9315 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    28361 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4373 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    34635 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    17481 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9603 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     2240 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3192 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    13681 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8020 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     4094 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3491 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2600 2023-07-12 21:42:54.066900 bbot-1.1.0.1908rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25482 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5461 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4851 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5125 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3260 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      908 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5718 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13670 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15858 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2539 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11304 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1307 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      807 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7437 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5795 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5997 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9552 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16933 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5124 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1292 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    15167 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      811 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     4269 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     5248 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     1545 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/nsec.py
--rw-r--r--   0        0        0     4993 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11391 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1623 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-12 21:42:54.070900 bbot-1.1.0.1908rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1845 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3627 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1688 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     8861 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8302 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2273 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1744 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7882 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11359 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3843 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1711 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2291 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    24694 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27042 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     4763 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10464 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     3987 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1086 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-12 21:42:54.074901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    15109 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    24751 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7957 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     8129 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     2664 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0     8916 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     1886 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1949 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     2069 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      555 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0      972 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-12 21:42:54.078901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      419 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
--rw-r--r--   0        0        0      659 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1262 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
--rw-r--r--   0        0        0     1116 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     1160 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2107 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10661 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2124 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      611 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     6024 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2370 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-12 21:42:54.082901 bbot-1.1.0.1908rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-12 21:42:54.086902 bbot-1.1.0.1908rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-12 21:42:54.086902 bbot-1.1.0.1908rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-12 21:42:54.094902 bbot-1.1.0.1908rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-12 21:42:54.094902 bbot-1.1.0.1908rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2023-07-12 21:42:54.094902 bbot-1.1.0.1908rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2023-07-12 21:42:54.094902 bbot-1.1.0.1908rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2023-07-12 21:42:54.094902 bbot-1.1.0.1908rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-12 21:42:54.094902 bbot-1.1.0.1908rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1537 2023-07-12 21:43:23.548843 bbot-1.1.0.1908rc0/pyproject.toml
--rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 bbot-1.1.0.1908rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-07-13 20:59:09.794570 bbot-1.1.0.1924rc0/LICENSE
+-rw-r--r--   0        0        0     6762 2023-07-13 20:59:09.794570 bbot-1.1.0.1924rc0/README.md
+-rw-r--r--   0        0        0      211 2023-07-13 20:59:41.247126 bbot-1.1.0.1924rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-13 20:59:09.794570 bbot-1.1.0.1924rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-13 20:59:09.794570 bbot-1.1.0.1924rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-07-13 20:59:09.794570 bbot-1.1.0.1924rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14945 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9721 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5290 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1314 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31059 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1496 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1115 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       61 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     1993 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5022 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9315 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    28361 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4373 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    35845 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    17481 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-07-13 20:59:09.798570 bbot-1.1.0.1924rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     2240 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3192 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    13681 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8020 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     4094 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3491 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2600 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    26361 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5461 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4851 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5125 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3260 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      908 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5718 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13949 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15858 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2539 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11600 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1307 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      807 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7138 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5795 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5997 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-07-13 20:59:09.802570 bbot-1.1.0.1924rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9382 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16933 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5280 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1292 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    15167 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      811 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     4269 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     5248 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     1545 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/nsec.py
+-rw-r--r--   0        0        0     4993 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11391 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1845 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1688 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     8861 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8302 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2007 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1398 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7882 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11061 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3843 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-07-13 20:59:09.806570 bbot-1.1.0.1924rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1397 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2291 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    24694 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27042 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     4763 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10464 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     3987 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1086 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    15109 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    26755 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7957 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     9758 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     2664 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     8916 2023-07-13 20:59:09.810570 bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     1886 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1949 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     2069 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      555 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0      972 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      419 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
+-rw-r--r--   0        0        0      659 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1262 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
+-rw-r--r--   0        0        0     1116 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     1160 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2107 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10661 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2124 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-07-13 20:59:09.814570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      611 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     6024 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2370 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-07-13 20:59:09.818570 bbot-1.1.0.1924rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-07-13 20:59:09.826570 bbot-1.1.0.1924rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-07-13 20:59:09.826570 bbot-1.1.0.1924rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2023-07-13 20:59:09.826570 bbot-1.1.0.1924rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2023-07-13 20:59:09.826570 bbot-1.1.0.1924rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2023-07-13 20:59:09.826570 bbot-1.1.0.1924rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-07-13 20:59:09.826570 bbot-1.1.0.1924rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1537 2023-07-13 20:59:41.243126 bbot-1.1.0.1924rc0/pyproject.toml
+-rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 bbot-1.1.0.1924rc0/PKG-INFO
```

### Comparing `bbot-1.1.0.1908rc0/LICENSE` & `bbot-1.1.0.1924rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/README.md` & `bbot-1.1.0.1924rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/agent/agent.py` & `bbot-1.1.0.1924rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/cli.py` & `bbot-1.1.0.1924rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.0.1924rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/configurator/args.py` & `bbot-1.1.0.1924rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/configurator/environ.py` & `bbot-1.1.0.1924rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/configurator/files.py` & `bbot-1.1.0.1924rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/errors.py` & `bbot-1.1.0.1924rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/event/base.py` & `bbot-1.1.0.1924rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/event/helpers.py` & `bbot-1.1.0.1924rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/flags.py` & `bbot-1.1.0.1924rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/cache.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/command.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/diff.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/dns.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/files.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/helper.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/logger.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/misc.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1196,7 +1196,43 @@
         chosen_index = random.choices(range(len(pool)), weights=weights, k=1)[0]
 
         # Add the chosen item to the shuffled list
         chosen_item, chosen_weight = pool.pop(chosen_index)
         shuffled_items.append(chosen_item)
 
     return shuffled_items
+
+
+def parse_port_string(port_string):
+    elements = port_string.split(",")
+    ports = []
+
+    for element in elements:
+        if element.isdigit():
+            port = int(element)
+            if 1 <= port <= 65535:
+                ports.append(port)
+            else:
+                raise ValueError(f"Invalid port: {element}")
+        elif "-" in element:
+            range_parts = element.split("-")
+            if len(range_parts) != 2 or not all(part.isdigit() for part in range_parts):
+                raise ValueError(f"Invalid port or port range: {element}")
+            start, end = map(int, range_parts)
+            if not (1 <= start < end <= 65535):
+                raise ValueError(f"Invalid port range: {element}")
+            ports.extend(range(start, end + 1))
+        else:
+            raise ValueError(f"Invalid port or port range: {element}")
+
+    return ports
+
+
+def parse_list_string(list_string):
+    elements = list_string.split(",")
+    result = []
+
+    for element in elements:
+        if any((c in '<>:"/\\|?*') or (ord(c) < 32 and c != " ") for c in element):
+            raise ValueError(f"Invalid character in string: {element}")
+        result.append(element)
+    return result
```

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/modules.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/punycode.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/url.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/validators.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/web.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.0.1924rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/core/logger/logger.py` & `bbot-1.1.0.1924rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/db/neo4j.py` & `bbot-1.1.0.1924rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/defaults.yml` & `bbot-1.1.0.1924rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/anubisdb.py` & `bbot-1.1.0.1924rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.0.1924rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/badsecrets.py` & `bbot-1.1.0.1924rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/base.py` & `bbot-1.1.0.1924rc0/bbot/modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     deps_shell = []
     # list of ansible tasks for when other dependency installation methods aren't enough
     deps_ansible = []
     # Whether to accept incoming duplicate events
     accept_dupes = False
     # Whether to block outgoing duplicate events
     suppress_dupes = True
+    # Limit the module to only scanning once per host. By default, defined by event.host, but can be customized by overriding
+    per_host_only = False
 
     # Scope distance modifier - accept/deny events based on scope distance
     # None == accept all events
     # 2 == accept events up to and including the scan's configured search distance plus two
     # 1 == accept events up to and including the scan's configured search distance plus one
     # 0 == (DEFAULT) accept events up to and including the scan's configured search distance
     # -1 == accept events up to and including the scan's configured search distance minus one
@@ -98,14 +100,17 @@
         self._request_failures = 0
 
         self._tasks = []
         self._event_received = asyncio.Condition()
         self._event_queued = asyncio.Condition()
         self._event_dequeued = asyncio.Condition()
 
+        # used for optional "per host" tracking
+        self._per_host_tracker = set()
+
     async def setup(self):
         """
         Perform setup functions at the beginning of the scan.
         Optionally override this method.
 
         Must return True or False based on whether the setup was successful
         """
@@ -423,14 +428,20 @@
             msg = str(self._custom_filter_criteria_msg)
             with suppress(ValueError, TypeError):
                 filter_result, reason = filter_result
                 msg += f": {reason}"
             if not filter_result:
                 return False, msg
 
+        if self.per_host_only:
+            if self.get_per_host_hash(event) in self._per_host_tracker:
+                return False, "per_host_only enabled and already seen host"
+            else:
+                self._per_host_tracker.add(self.get_per_host_hash(event))
+
         if self._type == "output" and not event._stats_recorded:
             event._stats_recorded = True
             self.scan.stats.event_produced(event)
 
         self.debug(f"{event} passed post-check")
         return True, ""
 
@@ -497,14 +508,23 @@
                 with suppress(asyncio.queues.QueueEmpty):
                     while 1:
                         self.incoming_event_queue.get_nowait()
                 # set queue to None to prevent its use
                 # if there are leftover objects in the queue, the scan will hang.
                 self._incoming_event_queue = False
 
+    # override in the module to define different values to comprise the hash
+    def get_per_host_hash(self, event):
+        parsed = getattr(event, "parsed", None)
+        if parsed is None:
+            to_hash = self.helpers.make_netloc(event.host, event.port)
+        else:
+            to_hash = f"{parsed.scheme}://{parsed.netloc}/"
+        return hash(to_hash)
+
     @property
     def name(self):
         return str(self._name)
 
     @property
     def helpers(self):
         return self.scan.helpers
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/bevigil.py` & `bbot-1.1.0.1924rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/binaryedge.py` & `bbot-1.1.0.1924rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/bucket_aws.py` & `bbot-1.1.0.1924rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.0.1924rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.0.1924rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.0.1924rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/bucket_gcp.py` & `bbot-1.1.0.1924rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/builtwith.py` & `bbot-1.1.0.1924rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/bypass403.py` & `bbot-1.1.0.1924rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/c99.py` & `bbot-1.1.0.1924rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/censys.py` & `bbot-1.1.0.1924rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/certspotter.py` & `bbot-1.1.0.1924rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/columbus.py` & `bbot-1.1.0.1924rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/crobat.py` & `bbot-1.1.0.1924rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/crt.py` & `bbot-1.1.0.1924rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.0.1924rc0/bbot/modules/deadly/ffuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from bbot.modules.base import BaseModule
+from bbot.core.helpers.misc import parse_list_string
 
 import random
 import string
 import json
 import base64
 
 
@@ -50,15 +51,20 @@
         self.canary = "".join(random.choice(string.ascii_lowercase) for i in range(10))
         wordlist_url = self.config.get("wordlist", "")
         self.debug(f"Using wordlist [{wordlist_url}]")
         self.wordlist = await self.helpers.wordlist(wordlist_url)
         self.wordlist_lines = list(self.helpers.read_file(self.wordlist))
         self.tempfile, tempfile_len = self.generate_templist()
         self.verbose(f"Generated dynamic wordlist with length [{str(tempfile_len)}]")
-        self.extensions = self.config.get("extensions", "")
+        try:
+            self.extensions = parse_list_string(self.config.get("extensions", ""))
+            self.critical(f"Using custom extensions: [{','.join(self.extensions)}]")
+        except ValueError as e:
+            self.warning(f"Error parsing extensions: {e}")
+            return False
         return True
 
     async def handle_event(self, event):
         if self.helpers.url_depth(event.data) > self.config.get("max_depth"):
             self.debug(f"Exceeded max depth, aborting event")
             return
 
@@ -68,15 +74,15 @@
             return
         else:
             # if we think its a directory, normalize it.
             fixed_url = event.data.rstrip("/") + "/"
 
         exts = ["", "/"]
         if self.extensions:
-            for ext in self.extensions.split(","):
+            for ext in self.extensions:
                 exts.append(f".{ext}")
 
         filters = await self.baseline_ffuf(fixed_url, exts=exts)
         async for r in self.execute_ffuf(self.tempfile, fixed_url, exts=exts, filters=filters):
             self.emit_event(r["url"], "URL_UNVERIFIED", source=event, tags=[f"status-{r['status']}"])
 
     async def filter_event(self, event):
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.0.1924rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.0.1924rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.0.1924rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.0.1924rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.1.0.1924rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/emailformat.py` & `bbot-1.1.0.1924rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.0.1924rc0/bbot/modules/ffuf_shortnames.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import random
 import string
 
 from bbot.modules.deadly.ffuf import ffuf
+from bbot.core.helpers.misc import parse_list_string
 
 
 def find_common_prefixes(strings, minimum_set_length=4):
     prefix_candidates = [s[:i] for s in strings if len(s) == 6 for i in range(3, 6)]
     frequency_dict = {item: prefix_candidates.count(item) for item in prefix_candidates}
     frequency_dict = {k: v for k, v in frequency_dict.items() if v >= minimum_set_length}
     prefix_list = list(set(frequency_dict.keys()))
@@ -82,15 +83,22 @@
         self.wordlist_lines = list(self.helpers.read_file(self.wordlist))
 
         wordlist_extensions = self.config.get("wordlist_extensions", "")
         if not wordlist_extensions:
             wordlist_extensions = f"{self.helpers.wordlist_dir}/raft-small-extensions-lowercase_CLEANED.txt"
         self.debug(f"Using [{wordlist_extensions}] for shortname candidate extension list")
         self.wordlist_extensions = await self.helpers.wordlist(wordlist_extensions)
-        self.extensions = self.config.get("extensions")
+
+        try:
+            self.extensions = parse_list_string(self.config.get("extensions", ""))
+            self.critical(f"Using custom extensions: [{','.join(self.extensions)}]")
+        except ValueError as e:
+            self.warning(f"Error parsing extensions: {e}")
+            return False
+
         self.ignore_redirects = self.config.get("ignore_redirects")
 
         self.per_host_collection = {}
         self.shortname_to_event = {}
         return True
 
     def build_extension_list(self, event):
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.0.1924rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/fullhunt.py` & `bbot-1.1.0.1924rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.0.1924rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/git.py` & `bbot-1.1.0.1924rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/github.py` & `bbot-1.1.0.1924rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/gowitness.py` & `bbot-1.1.0.1924rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/hackertarget.py` & `bbot-1.1.0.1924rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/host_header.py` & `bbot-1.1.0.1924rc0/bbot/modules/host_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 class host_header(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "web-thorough"]
     meta = {"description": "Try common HTTP Host header spoofing techniques"}
 
     in_scope_only = True
+    per_host_only = True
 
     deps_apt = ["curl"]
 
     async def setup(self):
-        self.scanned_hosts = set()
-
         self.subdomain_tags = {}
         if self.scan.config.get("interactsh_disable", False) == False:
             try:
                 self.interactsh_instance = self.helpers.interactsh()
                 self.domain = await self.interactsh_instance.register(callback=self.interactsh_callback)
             except InteractshError as e:
                 self.warning(f"Interactsh failure: {e}")
@@ -70,22 +69,14 @@
                 self.debug(
                     f"successfully deregistered interactsh session with correlation_id {self.interactsh_instance.correlation_id}"
                 )
             except InteractshError as e:
                 self.warning(f"Interactsh failure: {e}")
 
     async def handle_event(self, event):
-        host = f"{event.parsed.scheme}://{event.parsed.netloc}/"
-        host_hash = hash(host)
-        if host_hash in self.scanned_hosts:
-            self.debug(f"Host {host} was already scanned, exiting")
-            return
-        else:
-            self.scanned_hosts.add(host_hash)
-
         # get any set-cookie responses from the response and add them to the request
 
         added_cookies = {}
 
         for header, header_value in event.data["header-dict"].items():
             if header_value.lower() == "set-cookie":
                 header_split = header_value.split("=")
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/httpx.py` & `bbot-1.1.0.1924rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/hunt.py` & `bbot-1.1.0.1924rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/hunterio.py` & `bbot-1.1.0.1924rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.0.1924rc0/bbot/modules/iis_shortnames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from threading import Lock
 
 from bbot.modules.base import BaseModule
 
 valid_chars = "ETAONRISHDLFCMUGYPWBVKJXQZ0123456789_-$~()&!#%'@^`{}]]"
 
 
 def encode_all(string):
@@ -43,15 +42,14 @@
                     "Error Code</th><td>0x00000000" in test.text
                 ):
                     detections.append((method, 0, technique))
                     technique = "HTTP Body Error Message"
         return detections
 
     async def setup(self):
-        self.scanned_tracker_lock = Lock()
         self.scanned_tracker = set()
         return True
 
     @staticmethod
     def normalize_url(url):
         return str(url.rstrip("/") + "/").lower()
 
@@ -141,16 +139,15 @@
         if len(prefix) > 0 and found_results == False:
             url_hint_list.append(f"{prefix}")
             self.verbose(f"Found new (possibly partial) URL_HINT: {prefix} from node {target}")
         return url_hint_list
 
     async def handle_event(self, event):
         normalized_url = self.normalize_url(event.data)
-        with self.scanned_tracker_lock:
-            self.scanned_tracker.add(normalized_url)
+        self.scanned_tracker.add(normalized_url)
 
         detections = await self.detect(normalized_url)
 
         technique_strings = []
         if detections:
             for detection in detections:
                 method, affirmative_status_code, technique = detection
@@ -209,12 +206,11 @@
                             hint_type = "shortname-file"
                         else:
                             hint_type = "shortname-directory"
                         self.emit_event(f"{normalized_url}/{url_hint}", "URL_HINT", event, tags=[hint_type])
 
     async def filter_event(self, event):
         if "dir" in event.tags:
-            with self.scanned_tracker_lock:
-                if self.normalize_url(event.data) not in self.scanned_tracker:
-                    return True
-                return False
+            if self.normalize_url(event.data) not in self.scanned_tracker:
+                return True
+            return False
         return False
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/internal/base.py` & `bbot-1.1.0.1924rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.0.1924rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.0.1924rc0/bbot/modules/internal/speculate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 import ipaddress
 
+from bbot.core.helpers.misc import parse_port_string
 from bbot.modules.internal.base import BaseInternalModule
 
 
 class speculate(BaseInternalModule):
     """
     Bridge the gap between ranges and ips, or ips and open ports
     in situations where e.g. a port scanner isn't enabled
@@ -20,15 +21,15 @@
         "HTTP_RESPONSE",
         "STORAGE_BUCKET",
     ]
     produced_events = ["DNS_NAME", "OPEN_TCP_PORT", "IP_ADDRESS", "FINDING"]
     flags = ["passive"]
     meta = {"description": "Derive certain event types from others by common sense"}
 
-    options = {"max_hosts": 65536, "ports": [80, 443]}
+    options = {"max_hosts": 65536, "ports": "80,443"}
     options_desc = {
         "max_hosts": "Max number of IP_RANGE hosts to convert into IP_ADDRESS events",
         "ports": "The set of ports to speculate on",
     }
     max_event_handlers = 5
     scope_distance_modifier = 1
     _scope_shepherding = False
@@ -36,17 +37,22 @@
 
     async def setup(self):
         self.open_port_consumers = any(["OPEN_TCP_PORT" in m.watched_events for m in self.scan.modules.values()])
         self.portscanner_enabled = any(["portscan" in m.flags for m in self.scan.modules.values()])
         self.range_to_ip = True
         self.dns_resolution = self.scan.config.get("dns_resolution", True)
 
-        self.ports = self.config.get("ports", [80, 443])
-        if isinstance(self.ports, int):
-            self.ports = [self.ports]
+        port_string = self.config.get("ports", "80,443")
+
+        try:
+            self.ports = parse_port_string(port_string)
+        except ValueError as e:
+            self.warning(f"Error parsing ports: {e}")
+            return False
+
         if not self.portscanner_enabled:
             self.info(f"No portscanner enabled. Assuming open ports: {', '.join(str(x) for x in self.ports)}")
 
         target_len = len(self.scan.target)
         if target_len > self.config.get("max_hosts", 65536):
             if not self.portscanner_enabled:
                 self.hugewarning(
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.0.1924rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/ipstack.py` & `bbot-1.1.0.1924rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/leakix.py` & `bbot-1.1.0.1924rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/masscan.py` & `bbot-1.1.0.1924rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/massdns.py` & `bbot-1.1.0.1924rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/myssl.py` & `bbot-1.1.0.1924rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/naabu.py` & `bbot-1.1.0.1924rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/nmap.py` & `bbot-1.1.0.1924rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/nsec.py` & `bbot-1.1.0.1924rc0/bbot/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/ntlm.py` & `bbot-1.1.0.1924rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/otx.py` & `bbot-1.1.0.1924rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/base.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/csv.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/http.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/human.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/json.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/web_report.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/output/websocket.py` & `bbot-1.1.0.1924rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.0.1924rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.0.1924rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.0.1924rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/passivetotal.py` & `bbot-1.1.0.1924rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/pgp.py` & `bbot-1.1.0.1924rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/rapiddns.py` & `bbot-1.1.0.1924rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.0.1924rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/report/asn.py` & `bbot-1.1.0.1924rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/riddler.py` & `bbot-1.1.0.1924rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/robots.py` & `bbot-1.1.0.1924rc0/bbot/modules/zoomeye.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-from bbot.modules.base import BaseModule
+from bbot.modules.shodan_dns import shodan_dns
 
 
-class robots(BaseModule):
-    watched_events = ["URL"]
-    produced_events = ["URL_UNVERIFIED"]
-    flags = ["active", "safe", "web-basic", "web-thorough"]
-    meta = {"description": "Look for and parse robots.txt"}
-
-    options = {"include_sitemap": False, "include_allow": True, "include_disallow": True}
+class zoomeye(shodan_dns):
+    watched_events = ["DNS_NAME"]
+    produced_events = ["DNS_NAME"]
+    flags = ["affiliates", "subdomain-enum", "passive", "safe"]
+    meta = {"description": "Query ZoomEye's API for subdomains", "auth_required": True}
+    options = {"api_key": "", "max_pages": 20, "include_related": False}
     options_desc = {
-        "include_sitemap": "Include 'sitemap' entries",
-        "include_allow": "Include 'Allow' Entries",
-        "include_disallow": "Include 'Disallow' Entries",
+        "api_key": "ZoomEye API key",
+        "max_pages": "How many pages of results to fetch",
+        "include_related": "Include domains which may be related to the target",
     }
 
-    in_scope_only = True
+    base_url = "https://api.zoomeye.org"
 
     async def setup(self):
-        self.scanned_hosts = set()
-        return True
+        self.max_pages = self.config.get("max_pages", 20)
+        self.headers = {"API-KEY": self.config.get("api_key", "")}
+        self.include_related = self.config.get("include_related", False)
+        return await super().setup()
+
+    async def ping(self):
+        url = f"{self.base_url}/resources-info"
+        r = await self.helpers.request(url, headers=self.headers)
+        assert int(r.json()["quota_info"]["remain_total_quota"]) > 0, "No quota remaining"
 
     async def handle_event(self, event):
-        parsed_host = event.parsed
-        host = f"{parsed_host.scheme}://{parsed_host.netloc}/"
-        host_hash = hash(host)
-        if host_hash in self.scanned_hosts:
-            self.debug(f"Host {host} was already scanned, exiting")
-            return
-        else:
-            self.scanned_hosts.add(host_hash)
-
-        result = None
-        url = f"{host}robots.txt"
-        result = await self.helpers.request(url)
-        if result:
-            body = result.text
-
-            if body:
-                lines = body.split("\n")
-                for l in lines:
-                    if len(l) > 0:
-                        split_l = l.split(": ")
-                        if (split_l[0].lower() == "allow" and self.config.get("include_allow") == True) or (
-                            split_l[0].lower() == "disallow" and self.config.get("include_disallow") == True
-                        ):
-                            unverified_url = f"{host}{split_l[1].lstrip('/')}".replace(
-                                "*", self.helpers.rand_string(4)
-                            )
-
-                        elif split_l[0].lower() == "sitemap" and self.config.get("include_sitemap") == True:
-                            unverified_url = split_l[1]
-                        else:
-                            continue
-
-                        tags = []
-                        if self.is_spider_danger(event, unverified_url):
-                            tags.append("spider-danger")
-                        self.emit_event(unverified_url, "URL_UNVERIFIED", source=event, tags=tags)
+        query = self.make_query(event)
+        results = await self.query(query)
+        if results:
+            for hostname in results:
+                if hostname == event:
+                    continue
+                tags = []
+                if not hostname.endswith(f".{query}"):
+                    tags = ["affiliate"]
+                self.emit_event(hostname, "DNS_NAME", event, tags=tags)
+
+    async def query(self, query):
+        results = set()
+        query_type = 0 if self.include_related else 1
+        url = f"{self.base_url}/domain/search?q={self.helpers.quote(query)}&type={query_type}&page=" + "{page}"
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
+
+    def parse_results(self, r):
+        for entry in r.get("list", []):
+            yield entry["name"]
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/secretsdb.py` & `bbot-1.1.0.1924rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/securitytrails.py` & `bbot-1.1.0.1924rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.0.1924rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/skymem.py` & `bbot-1.1.0.1924rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/smuggler.py` & `bbot-1.1.0.1924rc0/bbot/modules/smuggler.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,35 +11,24 @@
 class smuggler(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "slow", "web-thorough"]
     meta = {"description": "Check for HTTP smuggling"}
 
     in_scope_only = True
+    per_host_only = True
 
     deps_ansible = [
         {
             "name": "Get smuggler repo",
             "git": {"repo": "https://github.com/defparam/smuggler.git", "dest": "#{BBOT_TOOLS}/smuggler"},
         }
     ]
 
-    async def setup(self):
-        self.scanned_hosts = set()
-        return True
-
     async def handle_event(self, event):
-        host = f"{event.parsed.scheme}://{event.parsed.netloc}/"
-        host_hash = hash(host)
-        if host_hash in self.scanned_hosts:
-            self.debug(f"Host {host} was already scanned, exiting")
-            return
-        else:
-            self.scanned_hosts.add(host_hash)
-
         command = [
             sys.executable,
             f"{self.scan.helpers.tools_dir}/smuggler/smuggler.py",
             "--no-color",
             "-q",
             "-u",
             event.data,
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/social.py` & `bbot-1.1.0.1924rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/sslcert.py` & `bbot-1.1.0.1924rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.1.0.1924rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/telerik.py` & `bbot-1.1.0.1924rc0/bbot/modules/telerik.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 
     RAUConfirmed = []
 
     options = {"exploit_RAU_crypto": False}
     options_desc = {"exploit_RAU_crypto": "Attempt to confirm any RAU AXD detections are vulnerable"}
 
     in_scope_only = True
+    per_host_only = True
 
     deps_pip = ["pycryptodome~=3.17"]
 
     deps_ansible = [
         {"name": "Create telerik dir", "file": {"state": "directory", "path": "#{BBOT_TOOLS}/telerik/"}},
         {"file": {"state": "touch", "path": "#{BBOT_TOOLS}/telerik/testfile.txt"}},
         {
@@ -155,27 +156,18 @@
             },
         },
     ]
 
     max_event_handlers = 5
 
     async def setup(self):
-        self.scanned_hosts = set()
         self.timeout = self.scan.config.get("httpx_timeout", 5)
         return True
 
     async def handle_event(self, event):
-        host = f"{event.parsed.scheme}://{event.parsed.netloc}/"
-        host_hash = hash(host)
-        if host_hash in self.scanned_hosts:
-            self.debug(f"Host {host} was already scanned, exiting")
-            return
-        else:
-            self.scanned_hosts.add(host_hash)
-
         webresource = "Telerik.Web.UI.WebResource.axd?type=rau"
         result, _ = await self.test_detector(event.data, webresource)
         if result:
             if "RadAsyncUpload handler is registered succesfully" in result.text:
                 self.debug(f"Detected Telerik instance (Telerik.Web.UI.WebResource.axd?type=rau)")
                 description = f"Telerik RAU AXD Handler detected"
                 self.emit_event(
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/threatminer.py` & `bbot-1.1.0.1924rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.0.1924rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/urlscan.py` & `bbot-1.1.0.1924rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/viewdns.py` & `bbot-1.1.0.1924rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/virustotal.py` & `bbot-1.1.0.1924rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/wafw00f.py` & `bbot-1.1.0.1924rc0/bbot/modules/wafw00f.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,29 +14,18 @@
 
     deps_pip = ["wafw00f~=2.2.0"]
 
     options = {"generic_detect": True}
     options_desc = {"generic_detect": "When no specific WAF detections are made, try to peform a generic detect"}
 
     in_scope_only = True
-
-    async def setup(self):
-        self.scanned_hosts = set()
-        return True
+    per_host_only = True
 
     async def handle_event(self, event):
-        parsed_host = event.parsed
-        host = f"{parsed_host.scheme}://{parsed_host.netloc}/"
-        host_hash = hash(host)
-        if host_hash in self.scanned_hosts:
-            self.debug(f"Host {host} was already scanned, exiting")
-            return
-        else:
-            self.scanned_hosts.add(host_hash)
-
+        host = f"{event.parsed.scheme}://{event.parsed.netloc}/"
         WW = await self.scan.run_in_executor(wafw00f_main.WAFW00F, host)
         waf_detections = await self.scan.run_in_executor(WW.identwaf)
         if waf_detections:
             for waf in waf_detections:
                 self.emit_event({"host": host, "WAF": waf}, "WAF", source=event)
         else:
             if self.config.get("generic_detect") == True:
```

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.0.1924rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/modules/wayback.py` & `bbot-1.1.0.1924rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.0.1924rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/scanner/manager.py` & `bbot-1.1.0.1924rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/scanner/scanner.py` & `bbot-1.1.0.1924rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/scanner/stats.py` & `bbot-1.1.0.1924rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/scanner/target.py` & `bbot-1.1.0.1924rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/scripts/docs.py` & `bbot-1.1.0.1924rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.0.1924rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/conftest.py` & `bbot-1.1.0.1924rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/run_tests.sh` & `bbot-1.1.0.1924rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test.conf` & `bbot-1.1.0.1924rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -576,7 +576,71 @@
     l = []
     while 1:
         try:
             l.append(next(sync_gen))
         except StopIteration:
             break
     assert l == [0, 1, 2, 3, 4]
+
+
+# test parse_port_string helper
+
+
+def test_portparse_singleports(helpers):
+    assert helpers.parse_port_string("80,443,22") == [80, 443, 22]
+
+
+def test_portparse_range_valid(helpers):
+    assert helpers.parse_port_string("80,443,22,1000-1002") == [80, 443, 22, 1000, 1001, 1002]
+
+
+def test_portparse_invalidport(helpers):
+    with pytest.raises(ValueError) as e:
+        helpers.parse_port_string("80,443,22,70000")
+    assert str(e.value) == "Invalid port: 70000"
+
+
+def test_portparse_range_invalid(helpers):
+    with pytest.raises(ValueError) as e:
+        helpers.parse_port_string("80,443,22,1000-70000")
+    assert str(e.value) == "Invalid port range: 1000-70000"
+
+
+def test_portparse_range_morethantwoparts(helpers):
+    with pytest.raises(ValueError) as e:
+        helpers.parse_port_string("80,443,22,1000-1001-1002")
+    assert str(e.value) == "Invalid port or port range: 1000-1001-1002"
+
+
+def test_portparse_range_startgreaterthanend(helpers):
+    with pytest.raises(ValueError) as e:
+        helpers.parse_port_string("80,443,22,1002-1000")
+    assert str(e.value) == "Invalid port range: 1002-1000"
+
+
+def test_portparse_nonnumericinput(helpers):
+    with pytest.raises(ValueError) as e:
+        helpers.parse_port_string("80,443,22,foo")
+    assert str(e.value) == "Invalid port or port range: foo"
+
+
+# test parse_list_string helper
+
+
+def test_liststring_valid_strings(helpers):
+    assert helpers.parse_list_string("hello,world,bbot") == ["hello", "world", "bbot"]
+
+
+def test_liststring_invalid_string(helpers):
+    with pytest.raises(ValueError) as e:
+        helpers.parse_list_string("hello,world,\x01")
+    assert str(e.value) == "Invalid character in string: \x01"
+
+
+def test_liststring_singleitem(helpers):
+    assert helpers.parse_list_string("hello") == ["hello"]
+
+
+def test_liststring_invalidfnchars(helpers):
+    with pytest.raises(ValueError) as e:
+        helpers.parse_list_string("hello,world,bbot|test")
+    assert str(e.value) == "Invalid character in string: bbot|test"
```

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import re
 
 from ..bbot_fixtures import *
 
+from bbot.modules.base import BaseModule
+from bbot.modules.output.base import BaseOutputModule
+from bbot.modules.report.base import BaseReportModule
+from bbot.modules.internal.base import BaseInternalModule
+
 
 @pytest.mark.asyncio
 async def test_modules_basic(scan, helpers, events, bbot_config, bbot_scanner, httpx_mock):
     fallback_nameservers = scan.helpers.temp_dir / "nameservers.txt"
     with open(fallback_nameservers, "w") as f:
         f.write("8.8.8.8\n")
 
     for http_method in ("GET", "CONNECT", "HEAD", "POST", "PUT", "TRACE", "DEBUG", "PATCH", "DELETE", "OPTIONS"):
         httpx_mock.add_response(method=http_method, url=re.compile(r".*"), json={"test": "test"})
 
-    # event filtering
-    from bbot.modules.base import BaseModule
-    from bbot.modules.output.base import BaseOutputModule
-    from bbot.modules.report.base import BaseReportModule
-    from bbot.modules.internal.base import BaseInternalModule
-
     # output module specific event filtering tests
     base_output_module = BaseOutputModule(scan)
     base_output_module.watched_events = ["IP_ADDRESS"]
     localhost = scan.make_event("127.0.0.1", source=scan.root_event)
     assert base_output_module._event_precheck(localhost)[0] == True
     localhost._internal = True
     assert base_output_module._event_precheck(localhost)[0] == False
@@ -163,7 +162,46 @@
 
     from bbot.core.flags import flag_descriptions
 
     for flag in all_flags:
         assert flag in flag_descriptions, f'Flag "{flag}" not listed in bbot/core/flags.py'
         description = flag_descriptions.get(flag, "")
         assert description, f'Flag "{flag}" has no description in bbot/core/flags.py'
+
+
+@pytest.mark.asyncio
+async def test_modules_basic_perhostonly(scan, helpers, events, bbot_config, bbot_scanner, httpx_mock, monkeypatch):
+    per_host_scan = bbot_scanner(
+        "evilcorp.com",
+        modules=list(set(available_modules + available_internal_modules)),
+        config=bbot_config,
+    )
+
+    await per_host_scan.load_modules()
+    await per_host_scan.setup_modules()
+    per_host_scan.status = "RUNNING"
+
+    # ensure that multiple events to the same "host" (schema + host) are blocked and check the per host tracker
+    for module_name, module in sorted(per_host_scan.modules.items()):
+        #    module.filter_event = base_module.filter_event
+        monkeypatch.setattr(module, "filter_event", BaseModule(per_host_scan).filter_event)
+
+        if "URL" in module.watched_events:
+            url_1 = per_host_scan.make_event(
+                "http://evilcorp.com/1", event_type="URL", source=per_host_scan.root_event, tags=["status-200"]
+            )
+            url_1.set_scope_distance(0)
+            url_2 = per_host_scan.make_event(
+                "http://evilcorp.com/2", event_type="URL", source=per_host_scan.root_event, tags=["status-200"]
+            )
+            url_2.set_scope_distance(0)
+            valid_1, reason_1 = await module._event_postcheck(url_1)
+            valid_2, reason_2 = await module._event_postcheck(url_2)
+
+            if module.per_host_only == True:
+                assert valid_1 == True
+                assert valid_2 == False
+                assert hash("http://evilcorp.com/") in module._per_host_tracker
+
+            else:
+                assert valid_1 == True
+                assert valid_2 == True
```

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.0.1924rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/testsslcert.pem` & `bbot-1.1.0.1924rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/test/testsslkey.pem` & `bbot-1.1.0.1924rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.0.1924rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.0.1924rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.0.1924rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.0.1924rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.0.1924rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.0.1924rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1908rc0/pyproject.toml` & `bbot-1.1.0.1924rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.0.1908rc"
+version = "v1.1.0.1924rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.1.0.1908rc0/PKG-INFO` & `bbot-1.1.0.1924rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.0.1908rc0
+Version: 1.1.0.1924rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

