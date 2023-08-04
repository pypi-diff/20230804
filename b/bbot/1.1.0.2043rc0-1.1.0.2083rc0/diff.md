# Comparing `tmp/bbot-1.1.0.2043rc0.tar.gz` & `tmp/bbot-1.1.0.2083rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.0.2043rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.0.2083rc0.tar", max compression
```

## Comparing `bbot-1.1.0.2043rc0.tar` & `bbot-1.1.0.2083rc0.tar`

### file list

```diff
@@ -1,295 +1,297 @@
--rw-r--r--   0        0        0    32473 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/LICENSE
--rw-r--r--   0        0        0     6787 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-31 03:26:09.541574 bbot-1.1.0.2043rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    15236 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9721 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5290 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1314 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31059 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1182 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1115 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       61 2023-07-31 03:25:50.641292 bbot-1.1.0.2043rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     2985 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5271 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9315 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    28343 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4281 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    37365 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    17480 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9724 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0     1491 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     2661 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3123 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    14898 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8020 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     4097 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     1344 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/azure_realm.py
--rw-r--r--   0        0        0     3505 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2768 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    27022 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5441 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4851 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5922 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3260 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      689 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5718 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13946 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15894 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0      884 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/digitorus.py
--rw-r--r--   0        0        0     2539 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11597 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-31 03:25:50.645292 bbot-1.1.0.2043rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1313 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      856 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7138 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5795 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5997 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9362 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16428 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5279 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1519 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    16018 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      811 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     5248 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     1545 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/nsec.py
--rw-r--r--   0        0        0     5006 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0     5620 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/oauth.py
--rw-r--r--   0        0        0      728 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11404 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1710 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1907 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     1513 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/subdomains.py
--rw-r--r--   0        0        0     3627 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1688 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     9436 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8373 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2007 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1398 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     8151 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0     1249 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/subdomaincenter.py
--rw-r--r--   0        0        0      507 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11098 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     4010 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1397 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2307 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    25632 2023-07-31 03:25:50.649292 bbot-1.1.0.2043rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27991 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     4763 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10464 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     3987 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1103 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    15109 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    28277 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7957 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     9758 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     7135 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_regexes.py
--rw-r--r--   0        0        0     2664 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0    10843 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     2757 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1207 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
--rw-r--r--   0        0        0     1949 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     3551 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      564 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0     1613 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
--rw-r--r--   0        0        0      972 2023-07-31 03:25:50.653292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      659 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1262 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
--rw-r--r--   0        0        0     1116 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     9356 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
--rw-r--r--   0        0        0     1160 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2142 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10680 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2190 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      610 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
--rw-r--r--   0        0        0     1116 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
--rw-r--r--   0        0        0      611 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     6024 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2374 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-31 03:25:50.657292 bbot-1.1.0.2043rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-31 03:25:50.665293 bbot-1.1.0.2043rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-31 03:25:50.665293 bbot-1.1.0.2043rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2023-07-31 03:25:50.665293 bbot-1.1.0.2043rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2023-07-31 03:25:50.665293 bbot-1.1.0.2043rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2023-07-31 03:25:50.665293 bbot-1.1.0.2043rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-31 03:25:50.665293 bbot-1.1.0.2043rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1595 2023-07-31 03:26:09.541574 bbot-1.1.0.2043rc0/pyproject.toml
--rw-r--r--   0        0        0     8223 1970-01-01 00:00:00.000000 bbot-1.1.0.2043rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/LICENSE
+-rw-r--r--   0        0        0     6832 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/README.md
+-rw-r--r--   0        0        0      211 2023-08-04 15:47:19.584583 bbot-1.1.0.2083rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    15210 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9721 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5290 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1314 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      617 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31059 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1182 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1115 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       61 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3439 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5580 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9315 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    32362 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4281 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    37365 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    17480 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9724 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0     1491 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     2661 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3123 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    15200 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8116 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     4097 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-08-04 15:47:02.064353 bbot-1.1.0.2083rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1344 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     3527 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2768 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    27216 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5441 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4851 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5922 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3190 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      689 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5732 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13946 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15894 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0      884 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/digitorus.py
+-rw-r--r--   0        0        0     2539 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11597 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1313 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      856 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7138 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5686 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5997 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9501 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16428 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5252 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1519 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    17219 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      811 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     5248 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     1545 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/nsec.py
+-rw-r--r--   0        0        0     5007 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5620 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      728 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11404 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1710 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1907 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     1513 2023-08-04 15:47:02.068354 bbot-1.1.0.2083rc0/bbot/modules/output/subdomains.py
+-rw-r--r--   0        0        0     3627 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1688 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     9436 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8373 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2007 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1973 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/sitedossier.py
+-rw-r--r--   0        0        0     1466 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1398 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     8151 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0     1249 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/subdomaincenter.py
+-rw-r--r--   0        0        0      507 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11098 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     4010 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1397 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2307 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    25459 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27955 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     4763 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10464 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     3987 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1103 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     5853 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6647 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    15109 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    28277 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7957 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     9758 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     7135 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_regexes.py
+-rw-r--r--   0        0        0     2664 2023-08-04 15:47:02.072353 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0    10843 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4982 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     2757 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     1949 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     3551 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      564 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0     1613 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
+-rw-r--r--   0        0        0      972 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      659 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1262 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
+-rw-r--r--   0        0        0     1116 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9356 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2142 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10680 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2190 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     6220 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
+-rw-r--r--   0        0        0     2321 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      610 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
+-rw-r--r--   0        0        0     1116 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
+-rw-r--r--   0        0        0      611 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     6024 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-08-04 15:47:02.076354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2374 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-08-04 15:47:02.080354 bbot-1.1.0.2083rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-08-04 15:47:02.084354 bbot-1.1.0.2083rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-08-04 15:47:02.084354 bbot-1.1.0.2083rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2023-08-04 15:47:02.084354 bbot-1.1.0.2083rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2023-08-04 15:47:02.084354 bbot-1.1.0.2083rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2023-08-04 15:47:02.084354 bbot-1.1.0.2083rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-08-04 15:47:02.088354 bbot-1.1.0.2083rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1597 2023-08-04 15:47:19.584583 bbot-1.1.0.2083rc0/pyproject.toml
+-rw-r--r--   0        0        0     8268 1970-01-01 00:00:00.000000 bbot-1.1.0.2083rc0/PKG-INFO
```

### Comparing `bbot-1.1.0.2043rc0/LICENSE` & `bbot-1.1.0.2083rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/README.md` & `bbot-1.1.0.2083rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,19 @@
 ```
 <!-- END BBOT EXAMPLE COMMANDS -->
 
 ## Targets
 
 BBOT accepts an unlimited number of targets. You can specify targets either directly on the command line or in files (or both!). Targets can be any of the following:
 
-- DNS_NAME (`evilcorp.com`)
-- IP_ADDRESS (`1.2.3.4`)
-- IP_RANGE (`1.2.3.0/24`)
-- URL (`https://www.evilcorp.com`)
+- `DNS_NAME` (`evilcorp.com`)
+- `IP_ADDRESS` (`1.2.3.4`)
+- `IP_RANGE` (`1.2.3.0/24`)
+- `OPEN_TCP_PORT` (`192.168.0.1:80`)
+- `URL` (`https://www.evilcorp.com`)
 
 For more information, see [Targets](https://www.blacklanternsecurity.com/bbot/scanning/#targets-t). To learn how BBOT handles scope, see [Scope](https://www.blacklanternsecurity.com/bbot/scanning/#scope).
 
 ## BBOT as a Python library
 
 **Synchronous**
```

### Comparing `bbot-1.1.0.2043rc0/bbot/agent/agent.py` & `bbot-1.1.0.2083rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/cli.py` & `bbot-1.1.0.2083rc0/bbot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 
                 # Make a list of the modules which can be output to the console
                 consoleable_output_modules = [
                     k for k, v in module_loader.preloaded(type="output").items() if "console" in v["config"]
                 ]
 
                 # if none of the output modules provided on the command line are consoleable, don't turn off the defaults. Instead, just add the one specified to the defaults.
-                if not any(o in consoleable_output_modules for o in options.output_modules):
-                    options.output_modules += default_output_modules
+                if not any(o in consoleable_output_modules for o in output_modules):
+                    output_modules += default_output_modules
 
                 scanner = Scanner(
                     *options.targets,
                     modules=list(modules),
                     output_modules=list(output_modules),
                     config=config,
                     name=options.name,
@@ -288,15 +288,15 @@
                                 log.hugewarning(
                                     "This is a (safe) active scan. Non-intrusive connections will be made to target"
                                 )
                     else:
                         log.hugeinfo("This is a passive scan. No connections will be made to target")
                     if slow_modules:
                         log.warning(
-                            f"You have enabled the following slow modules: {','.join(slow_modules)}. Scan may take longer than usual"
+                            f"You have enabled the following slow modules: {','.join(slow_modules)}. Scan may take a while"
                         )
 
                 scanner.helpers.word_cloud.load()
 
                 await scanner.prep()
 
                 if not options.dry_run:
```

### Comparing `bbot-1.1.0.2043rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.0.2083rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/configurator/args.py` & `bbot-1.1.0.2083rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/configurator/environ.py` & `bbot-1.1.0.2083rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/configurator/files.py` & `bbot-1.1.0.2083rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/errors.py` & `bbot-1.1.0.2083rc0/bbot/core/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from httpx import RequestError, ReadTimeout  # noqa
+from httpx import HTTPError, RequestError  # noqa
 
 
 class BBOTError(Exception):
     pass
 
 
 class ScanError(BBOTError):
@@ -41,9 +41,13 @@
     pass
 
 
 class DNSError(BBOTError):
     pass
 
 
+class DNSWildcardBreak(DNSError):
+    pass
+
+
 class CurlError(BBOTError):
     pass
```

### Comparing `bbot-1.1.0.2043rc0/bbot/core/event/base.py` & `bbot-1.1.0.2083rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/event/helpers.py` & `bbot-1.1.0.2083rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/flags.py` & `bbot-1.1.0.2083rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/async_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,39 +39,47 @@
         async with lock:
             yield
 
 
 class TaskCounter:
     def __init__(self):
         self.tasks = {}
+        self.lock = asyncio.Lock()  # create a new lock
 
     @property
     def value(self):
         return len(self.tasks)
 
-    def count(self, task_name):
+    def count(self, task_name, _log=True):
         if callable(task_name):
             task_name = f"{task_name.__qualname__}()"
-        return self.Task(self, task_name)
+        return self.Task(self, task_name, _log)
 
     class Task:
-        def __init__(self, manager, task_name):
+        def __init__(self, manager, task_name, _log=True):
             self.manager = manager
             self.task_name = task_name
             self.task_id = None
             self.start_time = None
+            self.log = _log
 
         async def __aenter__(self):
             self.task_id = uuid.uuid4()  # generate a unique ID for the task
-            self.start_time = datetime.now()
-            self.manager.tasks[self.task_id] = self
+            if self.log:
+                log.trace(f"Starting task {self.task_name} ({self.task_id})")
+            async with self.manager.lock:  # acquire the lock
+                self.start_time = datetime.now()
+                self.manager.tasks[self.task_id] = self
             return self.task_id  # this will be passed as 'task_id' to __aexit__
 
         async def __aexit__(self, exc_type, exc_val, exc_tb):
-            self.manager.tasks.pop(self.task_id, None)  # remove only current task
+            async with self.manager.lock:  # acquire the lock
+                self.manager.tasks.pop(self.task_id, None)  # remove only current task
+            if self.log:
+                log.trace(f"Finished task {self.task_name} ({self.task_id})")
 
         def __str__(self):
             running_for = human_timedelta(datetime.now() - self.start_time)
             return f"{self.task_name} running for {running_for}"
 
 
 def async_to_sync_gen(async_gen):
```

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/cache.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/command.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,21 @@
     proc, _input, command = await self._spawn_proc(*command, **kwargs)
     if proc is not None:
         input_task = None
         if _input is not None:
             input_task = asyncio.create_task(_write_stdin(proc, _input))
 
         while 1:
-            line = await proc.stdout.readline()
+            try:
+                line = await proc.stdout.readline()
+            except ValueError as e:
+                command_str = " ".join([str(c) for c in command])
+                log.warning(f"Error executing command {command_str}: {e}")
+                log.trace(traceback.format_exc())
+                continue
             if not line:
                 break
             if text:
                 line = smart_decode(line).rstrip("\r\n")
             else:
                 line = line.rstrip(b"\r\n")
             yield line
@@ -114,16 +120,17 @@
             async for chunk in _input:
                 proc.stdin.write(smart_encode(chunk) + b"\n")
         await proc.stdin.drain()
         proc.stdin.close()
 
 
 def _prepare_command_kwargs(self, command, kwargs):
-    # limit = 10MB (this is needed for cases like httpx that are sending large JSON blobs over stdout)
-    kwargs["limit"] = 1024 * 1024 * 10
+    # limit = 100MB (this is needed for cases like httpx that are sending large JSON blobs over stdout)
+    if not "limit" in kwargs:
+        kwargs["limit"] = 1024 * 1024 * 100
     if not "stdout" in kwargs:
         kwargs["stdout"] = asyncio.subprocess.PIPE
     if not "stderr" in kwargs:
         kwargs["stderr"] = asyncio.subprocess.PIPE
     sudo = kwargs.pop("sudo", False)
 
     if len(command) == 1 and isinstance(command[0], (list, tuple)):
```

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/diff.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/dns.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/dns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import asyncio
 import logging
 import ipaddress
 import traceback
 import contextlib
 import dns.exception
 import dns.asyncresolver
+from contextlib import suppress
 
 from .regexes import dns_name_regex
 from bbot.core.helpers.ratelimiter import RateLimiter
 from bbot.core.helpers.async_helpers import NamedLock
-from bbot.core.errors import ValidationError, DNSError
+from bbot.core.errors import ValidationError, DNSError, DNSWildcardBreak
 from .misc import is_ip, is_domain, is_dns_name, domain_parents, parent_domain, rand_string, cloudcheck, as_completed
 
 log = logging.getLogger("bbot.core.helpers.dns")
 
 
 class DNSHelper:
     """
@@ -85,31 +87,37 @@
         }
         "evilcorp.com" --> {
             "1.2.3.4",
             "dead::beef"
         }
         """
         results = set()
-        r = await self.resolve_raw(query, **kwargs)
-        if r:
-            raw_results, errors = r
-            for rdtype, answers in raw_results:
-                for answer in answers:
-                    for _, t in self.extract_targets(answer):
-                        results.add(t)
+        try:
+            r = await self.resolve_raw(query, **kwargs)
+            if r:
+                raw_results, errors = r
+                for rdtype, answers in raw_results:
+                    for answer in answers:
+                        for _, t in self.extract_targets(answer):
+                            results.add(t)
+        except BaseException:
+            log.trace(f"Caught exception in resolve({query}, {kwargs}):")
+            log.trace(traceback.format_exc())
+            raise
+
         return results
 
     async def resolve_raw(self, query, **kwargs):
         # DNS over TCP is more reliable
         # But setting this breaks DNS resolution on Ubuntu because systemd-resolve doesn't support TCP
         # kwargs["tcp"] = True
         results = []
         errors = []
-        query = str(query).strip()
         try:
+            query = str(query).strip()
             if is_ip(query):
                 kwargs.pop("type", None)
                 kwargs.pop("rdtype", None)
                 results, errors = await self._resolve_ip(query, **kwargs)
                 return [("PTR", results)], [("PTR", e) for e in errors]
             else:
                 types = ["A", "AAAA"]
@@ -125,17 +133,18 @@
                         types = [str(_).strip().upper() for _ in t]
                 for t in types:
                     r, e = await self._resolve_hostname(query, rdtype=t, **kwargs)
                     if r:
                         results.append((t, r))
                     for error in e:
                         errors.append((t, error))
-        except RuntimeError as e:
-            log.debug(f"Error in resolve_raw({query}, kwargs={kwargs}): {e}")
+        except BaseException:
+            log.trace(f"Caught exception in resolve_raw({query}, {kwargs}):")
             log.trace(traceback.format_exc())
+            raise
 
         return (results, errors)
 
     async def _resolve_hostname(self, query, **kwargs):
         self.debug(f"Resolving {query} with kwargs={kwargs}")
         results = []
         errors = []
@@ -156,26 +165,52 @@
         while tries_left > 0:
             try:
                 try:
                     results = self._dns_cache[dns_cache_hash]
                 except KeyError:
                     error_count = self._errors.get(parent_hash, 0)
                     if error_count >= self.abort_threshold:
-                        log.verbose(
-                            f'Aborting query "{query}" because failed {rdtype} queries for "{parent}" ({error_count:,}) exceeded abort threshold ({self.abort_threshold:,})'
-                        )
-                        return results, errors
+                        try:
+                            dns_server_working = list(
+                                await asyncio.wait_for(
+                                    self.resolver.resolve("www.google.com", rdtype="A"), self.timeout + 10
+                                )
+                            )
+                        except Exception:
+                            dns_server_working = []
+                        if not dns_server_working:
+                            log.warning(f"DNS queries are failing, you may be blasting a little too hard")
+                            self._errors.clear()
+                        else:
+                            log.info(
+                                f'Aborting query "{query}" because failed {rdtype} queries for "{parent}" ({error_count:,}) exceeded abort threshold ({self.abort_threshold:,})'
+                            )
+                            if parent_hash not in self._dns_warnings:
+                                log.warning(
+                                    f'Aborting future {rdtype} queries to "{parent}" because error count ({error_count:,}) exceeded abort threshold ({self.abort_threshold:,})'
+                                )
+                            self._dns_warnings.add(parent_hash)
+                            return results, errors
                     async with self.dns_rate_limiter:
-                        results = await self._catch(self.resolver.resolve, query, **kwargs)
+                        # wait_for exists here because of this:
+                        #  https://github.com/rthalley/dnspython/issues/976
+                        results = await asyncio.wait_for(
+                            self._catch(self.resolver.resolve, query, **kwargs), self.timeout + 10
+                        )
                     if cache_result:
                         self._dns_cache[dns_cache_hash] = results
                     if parent_hash in self._errors:
                         self._errors[parent_hash] = 0
                 break
-            except (dns.resolver.NoNameservers, dns.exception.Timeout, dns.resolver.LifetimeTimeout) as e:
+            except (
+                dns.resolver.NoNameservers,
+                dns.exception.Timeout,
+                dns.resolver.LifetimeTimeout,
+                TimeoutError,
+            ) as e:
                 try:
                     self._errors[parent_hash] += 1
                 except KeyError:
                     self._errors[parent_hash] = 1
                 errors.append(e)
                 # don't retry if we get a SERVFAIL
                 if isinstance(e, dns.resolver.NoNameservers):
@@ -203,179 +238,197 @@
         dns_cache_hash = hash(f"{query}:PTR")
         while tries_left > 0:
             try:
                 try:
                     results = self._dns_cache[dns_cache_hash]
                 except KeyError:
                     async with self.dns_rate_limiter:
-                        results = await self._catch(self.resolver.resolve_address, query, **kwargs)
+                        results = await asyncio.wait_for(
+                            self._catch(self.resolver.resolve_address, query, **kwargs), self.timeout + 10
+                        )
                     if cache_result:
                         self._dns_cache[dns_cache_hash] = results
                 break
-            except (dns.exception.Timeout, dns.resolver.LifetimeTimeout, dns.resolver.NoNameservers) as e:
+            except (
+                dns.exception.Timeout,
+                dns.resolver.LifetimeTimeout,
+                dns.resolver.NoNameservers,
+                TimeoutError,
+            ) as e:
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
 
     async def handle_wildcard_event(self, event, children):
-        event_host = str(event.host)
-        # wildcard checks
-        if not is_ip(event.host):
-            # check if this domain is using wildcard dns
-            event_target = "target" in event.tags
-            for hostname, wildcard_domain_rdtypes in (
-                await self.is_wildcard_domain(event_host, log_info=event_target)
-            ).items():
-                if wildcard_domain_rdtypes:
-                    event.add_tag("wildcard-domain")
-                    for rdtype, ips in wildcard_domain_rdtypes.items():
-                        event.add_tag(f"{rdtype.lower()}-wildcard-domain")
-            # check if the dns name itself is a wildcard entry
-            wildcard_rdtypes = await self.is_wildcard(event_host)
-            for rdtype, (is_wildcard, wildcard_host) in wildcard_rdtypes.items():
-                wildcard_tag = "error"
-                if is_wildcard == True:
-                    event.add_tag("wildcard")
-                    wildcard_tag = "wildcard"
-                event.add_tag(f"{rdtype.lower()}-{wildcard_tag}")
-
-        # wildcard event modification (www.evilcorp.com --> _wildcard.evilcorp.com)
-        if not is_ip(event.host) and wildcard_rdtypes and children:
-            # these are the rdtypes that successfully resolve
-            resolved_rdtypes = set([c.upper() for c in children])
-            # these are the rdtypes that have wildcards
-            wildcard_rdtypes_set = set(wildcard_rdtypes)
-            # consider the event a full wildcard if all its records are wildcards
-            event_is_wildcard = False
-            if resolved_rdtypes:
-                event_is_wildcard = all(r in wildcard_rdtypes_set for r in resolved_rdtypes)
-            # if event_is_wildcard and event.type in ("DNS_NAME",) and not "_wildcard" in event.data.split("."):
-            if event_is_wildcard:
-                if event.type in ("DNS_NAME",) and not "_wildcard" in event.data.split("."):
-                    wildcard_parent = self.parent_helper.parent_domain(event_host)
-                    for rdtype, (_is_wildcard, _parent_domain) in wildcard_rdtypes.items():
-                        if _is_wildcard:
-                            wildcard_parent = _parent_domain
-                            break
-                    wildcard_data = f"_wildcard.{wildcard_parent}"
-                    if wildcard_data != event.data:
-                        log.debug(f'Wildcard detected, changing event.data "{event.data}" --> "{wildcard_data}"')
-                        event.data = wildcard_data
+        log.debug(f"Entering handle_wildcard_event({event}, children={children})")
+        try:
+            event_host = str(event.host)
+            # wildcard checks
+            if not is_ip(event.host):
+                # check if the dns name itself is a wildcard entry
+                wildcard_rdtypes = await self.is_wildcard(event_host)
+                for rdtype, (is_wildcard, wildcard_host) in wildcard_rdtypes.items():
+                    wildcard_tag = "error"
+                    if is_wildcard == True:
+                        event.add_tag("wildcard")
+                        wildcard_tag = "wildcard"
+                    event.add_tag(f"{rdtype.lower()}-{wildcard_tag}")
+
+            # wildcard event modification (www.evilcorp.com --> _wildcard.evilcorp.com)
+            if not is_ip(event.host) and children:
+                if wildcard_rdtypes:
+                    # these are the rdtypes that successfully resolve
+                    resolved_rdtypes = set([c.upper() for c in children])
+                    # these are the rdtypes that have wildcards
+                    wildcard_rdtypes_set = set(wildcard_rdtypes)
+                    # consider the event a full wildcard if all its records are wildcards
+                    event_is_wildcard = False
+                    if resolved_rdtypes:
+                        event_is_wildcard = all(r in wildcard_rdtypes_set for r in resolved_rdtypes)
+
+                    if event_is_wildcard:
+                        if event.type in ("DNS_NAME",) and not "_wildcard" in event.data.split("."):
+                            wildcard_parent = self.parent_helper.parent_domain(event_host)
+                            for rdtype, (_is_wildcard, _parent_domain) in wildcard_rdtypes.items():
+                                if _is_wildcard:
+                                    wildcard_parent = _parent_domain
+                                    break
+                            wildcard_data = f"_wildcard.{wildcard_parent}"
+                            if wildcard_data != event.data:
+                                log.debug(
+                                    f'Wildcard detected, changing event.data "{event.data}" --> "{wildcard_data}"'
+                                )
+                                event.data = wildcard_data
+                else:
+                    # check if this domain is using wildcard dns
+                    event_target = "target" in event.tags
+                    wildcard_domain_results = await self.is_wildcard_domain(event_host, log_info=event_target)
+                    for hostname, wildcard_domain_rdtypes in wildcard_domain_results.items():
+                        if wildcard_domain_rdtypes:
+                            event.add_tag("wildcard-domain")
+                            for rdtype, ips in wildcard_domain_rdtypes.items():
+                                event.add_tag(f"{rdtype.lower()}-wildcard-domain")
+        finally:
+            log.debug(f"Finished handle_wildcard_event({event}, children={children})")
 
     async def resolve_event(self, event, minimal=False):
         """
         Tag event with appropriate dns record types
         Optionally create child events from dns resolutions
         """
         log.debug(f"Resolving {event}")
         event_host = str(event.host)
         event_tags = set()
         dns_children = dict()
         event_whitelisted = False
         event_blacklisted = False
 
-        if not event.host or event.type in ("IP_RANGE",):
-            return event_tags, event_whitelisted, event_blacklisted, dns_children
+        try:
+            if not event.host or event.type in ("IP_RANGE",):
+                return event_tags, event_whitelisted, event_blacklisted, dns_children
 
-        # lock to ensure resolution of the same host doesn't start while we're working here
-        async with self._event_cache_locks.lock(event_host):
-            # try to get data from cache
-            _event_tags, _event_whitelisted, _event_blacklisted, _dns_children = self.event_cache_get(event_host)
-            event_tags.update(_event_tags)
-            # if we found it, return it
-            if _event_whitelisted is not None:
-                return event_tags, _event_whitelisted, _event_blacklisted, _dns_children
-
-            # then resolve
-            types = ()
-            if self.parent_helper.is_ip(event.host):
-                if not minimal:
-                    types = ("PTR",)
-            else:
-                if event.type == "DNS_NAME" and not minimal:
-                    types = self.all_rdtypes
+            # lock to ensure resolution of the same host doesn't start while we're working here
+            async with self._event_cache_locks.lock(event_host):
+                # try to get data from cache
+                _event_tags, _event_whitelisted, _event_blacklisted, _dns_children = self.event_cache_get(event_host)
+                event_tags.update(_event_tags)
+                # if we found it, return it
+                if _event_whitelisted is not None:
+                    return event_tags, _event_whitelisted, _event_blacklisted, _dns_children
+
+                # then resolve
+                types = ()
+                if self.parent_helper.is_ip(event.host):
+                    if not minimal:
+                        types = ("PTR",)
                 else:
-                    types = ("A", "AAAA")
+                    if event.type == "DNS_NAME" and not minimal:
+                        types = self.all_rdtypes
+                    else:
+                        types = ("A", "AAAA")
 
-            if types:
-                tasks = [self.resolve_raw(event_host, type=t, cache_result=True) for t in types]
-                async for task in as_completed(tasks):
-                    resolved_raw, errors = await task
-                    for rdtype, e in errors:
-                        if rdtype not in resolved_raw:
-                            event_tags.add(f"{rdtype.lower()}-error")
-                    for rdtype, records in resolved_raw:
-                        rdtype = str(rdtype).upper()
-                        if records:
-                            event_tags.add("resolved")
-                            event_tags.add(f"{rdtype.lower()}-record")
-
-                        # whitelisting and blacklisting of IPs
-                        for r in records:
-                            for _, t in self.extract_targets(r):
-                                if t:
-                                    ip = self.parent_helper.make_ip_type(t)
-
-                                    if rdtype in ("A", "AAAA", "CNAME"):
-                                        with contextlib.suppress(ValidationError):
-                                            if self.parent_helper.is_ip(ip):
-                                                if self.parent_helper.scan.whitelisted(ip):
-                                                    event_whitelisted = True
-                                        with contextlib.suppress(ValidationError):
-                                            if self.parent_helper.scan.blacklisted(ip):
-                                                event_blacklisted = True
-
-                                    if self.filter_bad_ptrs and rdtype in ("PTR") and self.parent_helper.is_ptr(t):
-                                        self.debug(f"Filtering out bad PTR: {t}")
-                                        continue
-
-                                    try:
-                                        dns_children[rdtype].add(ip)
-                                    except KeyError:
-                                        dns_children[rdtype] = {ip}
-
-                # tag with cloud providers
-                if not self.parent_helper.in_tests:
-                    to_check = set()
-                    if event.type == "IP_ADDRESS":
-                        to_check.add(event.data)
+                if types:
+                    tasks = [self.resolve_raw(event_host, type=t, cache_result=True) for t in types]
+                    async for task in as_completed(tasks):
+                        resolved_raw, errors = await task
+                        for rdtype, e in errors:
+                            if rdtype not in resolved_raw:
+                                event_tags.add(f"{rdtype.lower()}-error")
+                        for rdtype, records in resolved_raw:
+                            rdtype = str(rdtype).upper()
+                            if records:
+                                event_tags.add("resolved")
+                                event_tags.add(f"{rdtype.lower()}-record")
+
+                            # whitelisting and blacklisting of IPs
+                            for r in records:
+                                for _, t in self.extract_targets(r):
+                                    if t:
+                                        ip = self.parent_helper.make_ip_type(t)
+
+                                        if rdtype in ("A", "AAAA", "CNAME"):
+                                            with contextlib.suppress(ValidationError):
+                                                if self.parent_helper.is_ip(ip):
+                                                    if self.parent_helper.scan.whitelisted(ip):
+                                                        event_whitelisted = True
+                                            with contextlib.suppress(ValidationError):
+                                                if self.parent_helper.scan.blacklisted(ip):
+                                                    event_blacklisted = True
+
+                                        if self.filter_bad_ptrs and rdtype in ("PTR") and self.parent_helper.is_ptr(t):
+                                            self.debug(f"Filtering out bad PTR: {t}")
+                                            continue
+
+                                        try:
+                                            dns_children[rdtype].add(ip)
+                                        except KeyError:
+                                            dns_children[rdtype] = {ip}
+
+                    # tag with cloud providers
+                    if not self.parent_helper.in_tests:
+                        to_check = set()
+                        if event.type == "IP_ADDRESS":
+                            to_check.add(event.data)
+                        for rdtype, ips in dns_children.items():
+                            if rdtype in ("A", "AAAA"):
+                                for ip in ips:
+                                    to_check.add(ip)
+                        for ip in to_check:
+                            provider, provider_type, subnet = cloudcheck(ip)
+                            if provider:
+                                event_tags.add(f"{provider_type}-{provider}")
+
+                    # if needed, mark as unresolved
+                    if not is_ip(event_host) and "resolved" not in event_tags:
+                        event_tags.add("unresolved")
+                    # check for private IPs
                     for rdtype, ips in dns_children.items():
-                        if rdtype in ("A", "AAAA"):
-                            for ip in ips:
-                                to_check.add(ip)
-                    for ip in to_check:
-                        provider, provider_type, subnet = cloudcheck(ip)
-                        if provider:
-                            event_tags.add(f"{provider_type}-{provider}")
-
-                # if needed, mark as unresolved
-                if not is_ip(event_host) and "resolved" not in event_tags:
-                    event_tags.add("unresolved")
-                # check for private IPs
-                for rdtype, ips in dns_children.items():
-                    for ip in ips:
-                        try:
-                            ip = ipaddress.ip_address(ip)
-                            if ip.is_private:
-                                event_tags.add("private-ip")
-                        except ValueError:
-                            continue
+                        for ip in ips:
+                            try:
+                                ip = ipaddress.ip_address(ip)
+                                if ip.is_private:
+                                    event_tags.add("private-ip")
+                            except ValueError:
+                                continue
+
+                    self._event_cache[event_host] = (event_tags, event_whitelisted, event_blacklisted, dns_children)
 
-                self._event_cache[event_host] = (event_tags, event_whitelisted, event_blacklisted, dns_children)
+            return event_tags, event_whitelisted, event_blacklisted, dns_children
 
-        return event_tags, event_whitelisted, event_blacklisted, dns_children
+        finally:
+            log.debug(f"Finished resolving {event}")
 
     def event_cache_get(self, host):
         try:
             return self._event_cache[host]
         except KeyError:
             return set(), None, None, set()
 
@@ -435,16 +488,16 @@
         return str(record).rstrip(".").lower()
 
     async def _catch(self, callback, *args, **kwargs):
         try:
             return await callback(*args, **kwargs)
         except dns.resolver.NoNameservers:
             raise
-        except (dns.exception.Timeout, dns.resolver.LifetimeTimeout):
-            log.debug(f"DNS query with args={args}, kwargs={kwargs} timed out after {self.timeout} seconds")
+        except (dns.exception.Timeout, dns.resolver.LifetimeTimeout, TimeoutError):
+            log.verbose(f"DNS query with args={args}, kwargs={kwargs} timed out after {self.timeout} seconds")
             raise
         except dns.exception.DNSException as e:
             self.debug(f"{e} (args={args}, kwargs={kwargs})")
         except Exception as e:
             log.warning(f"Error in {callback.__qualname__}() with args={args}, kwargs={kwargs}: {e}")
             log.trace(traceback.format_exc())
         return []
@@ -462,126 +515,146 @@
 
             is_wildcard("www.github.io") --> {"A": (True, "github.io"), "AAAA": (True, "github.io")}
 
         Note that is_wildcard can be True, False, or None (indicating that wildcard detection was inconclusive)
         """
         result = {}
 
+        if [ips, rdtype].count(None) == 1:
+            raise ValueError("Both ips and rdtype must be specified")
+
         if not is_dns_name(query):
             return {}
 
         # skip check if the query's parent domain is excluded in the config
         for d in self.wildcard_ignore:
             if self.parent_helper.host_in_host(query, d):
                 log.debug(f"Skipping wildcard detection on {query} because it is excluded in the config")
                 return {}
 
-        if rdtype is None:
-            rdtype = "ANY"
-
         query = self._clean_dns_record(query)
         # skip check if it's an IP
         if is_ip(query) or not "." in query:
             return {}
         # skip check if the query is a domain
         if is_domain(query):
             return {}
 
         parent = parent_domain(query)
         parents = list(domain_parents(query))
 
-        wildcard_tasks = {t: [] for t in self.all_rdtypes}
+        rdtypes_to_check = [rdtype] if rdtype is not None else self.all_rdtypes
+
         base_query_ips = dict()
         # if the caller hasn't already done the work of resolving the IPs
         if ips is None:
             # then resolve the query for all rdtypes
-            for _rdtype in self.all_rdtypes:
-                # resolve the base query
-                wildcard_tasks[_rdtype].append(self.resolve_raw(query, type=_rdtype, cache_result=True))
-
-            for _rdtype, tasks in wildcard_tasks.items():
-                async for task in as_completed(tasks):
-                    raw_results, errors = await task
-                    if errors and not raw_results:
-                        self.debug(f"Failed to resolve {query} ({_rdtype}) during wildcard detection")
-                        result[_rdtype] = (None, parent)
-                        continue
-                    for __rdtype, answers in raw_results:
-                        base_query_ips[__rdtype] = set()
-                        for answer in answers:
-                            for _, t in self.extract_targets(answer):
-                                base_query_ips[__rdtype].add(t)
+            base_query_tasks = {
+                t: asyncio.create_task(self.resolve_raw(query, type=t, cache_result=True)) for t in rdtypes_to_check
+            }
+            for _rdtype, task in base_query_tasks.items():
+                raw_results, errors = await task
+                if errors and not raw_results:
+                    self.debug(f"Failed to resolve {query} ({_rdtype}) during wildcard detection")
+                    result[_rdtype] = (None, parent)
+                    continue
+                for __rdtype, answers in raw_results:
+                    base_query_results = set()
+                    for answer in answers:
+                        for _, t in self.extract_targets(answer):
+                            base_query_results.add(t)
+                    if base_query_results:
+                        base_query_ips[__rdtype] = base_query_results
         else:
             # otherwise, we can skip all that
-            base_query_ips[rdtype] = set([self._clean_dns_record(ip) for ip in ips])
+            cleaned_ips = set([self._clean_dns_record(ip) for ip in ips])
+            if not cleaned_ips:
+                raise ValueError("Valid IPs must be specified")
+            base_query_ips[rdtype] = cleaned_ips
         if not base_query_ips:
             return result
 
         # once we've resolved the base query and have IP addresses to work with
         # we can compare the IPs to the ones we have on file for wildcards
-        # for every rdtype
-        for _rdtype in self.all_rdtypes:
-            # get the IPs from above
-            query_ips = base_query_ips.get("ANY", base_query_ips.get(_rdtype, set()))
-            if not query_ips:
-                continue
-            # for every parent domain, starting with the longest
+
+        # for every parent domain, starting with the shortest
+        try:
             for host in parents[::-1]:
-                host_hash = hash(host)
-                # make sure we've checked that domain for wildcards
-                await self.is_wildcard_domain(host)
-                if host_hash in self._wildcard_cache:
-                    # then get its IPs from our wildcard cache
-                    wildcard_rdtypes = self._wildcard_cache[host_hash]
-                    # then check to see if our IPs match the wildcard ones
-                    if _rdtype in wildcard_rdtypes:
-                        wildcard_ips = wildcard_rdtypes[_rdtype]
-                        # if our IPs match the wildcard ones, then ladies and gentlemen we have a wildcard
-                        is_wildcard = any(r in wildcard_ips for r in query_ips)
-                        if is_wildcard:
-                            result[_rdtype] = (True, host)
-                            break
+                # for every rdtype
+                for _rdtype in list(base_query_ips):
+                    # get the IPs from above
+                    query_ips = base_query_ips.get(_rdtype, set())
+                    # make sure we've checked that domain for wildcards
+                    await self.is_wildcard_domain(host)
+                    host_hash = hash(host)
+
+                    if host_hash in self._wildcard_cache:
+                        # then get its IPs from our wildcard cache
+                        wildcard_rdtypes = self._wildcard_cache[host_hash]
+
+                        # then check to see if our IPs match the wildcard ones
+                        if _rdtype in wildcard_rdtypes:
+                            wildcard_ips = wildcard_rdtypes[_rdtype]
+                            # if our IPs match the wildcard ones, then ladies and gentlemen we have a wildcard
+                            is_wildcard = any(r in wildcard_ips for r in query_ips)
+
+                            if is_wildcard and not result.get(_rdtype, (None, None))[0] is True:
+                                result[_rdtype] = (True, host)
+
+                    # if we've reached a point where the dns name is a complete wildcard, class can be dismissed early
+                    base_query_rdtypes = set(base_query_ips)
+                    wildcard_rdtypes_set = set([k for k, v in result.items() if v[0] is True])
+                    if base_query_rdtypes and wildcard_rdtypes_set and base_query_rdtypes == wildcard_rdtypes_set:
+                        log.debug(
+                            f"Breaking from wildcard detection for {query} at {host} because base query rdtypes ({base_query_rdtypes}) == wildcard rdtypes ({wildcard_rdtypes_set})"
+                        )
+                        raise DNSWildcardBreak()
+        except DNSWildcardBreak:
+            pass
 
         return result
 
     async def is_wildcard_domain(self, domain, log_info=False):
         """
         Check whether a domain is using wildcard DNS
 
         Returns a dictionary containing any DNS record types that are wildcards, and their associated IPs
             is_wildcard_domain("github.io") --> {"A": {"1.2.3.4",}, "AAAA": {"dead::beef",}}
         """
+
         wildcard_domain_results = {}
         domain = self._clean_dns_record(domain)
 
         if not is_dns_name(domain):
             return {}
 
         # skip check if the query's parent domain is excluded in the config
         for d in self.wildcard_ignore:
             if self.parent_helper.host_in_host(domain, d):
                 log.debug(f"Skipping wildcard detection on {domain} because it is excluded in the config")
                 return {}
 
+        rdtypes_to_check = set(self.all_rdtypes)
+
         # make a list of its parents
         parents = list(domain_parents(domain, include_self=True))
         # and check each of them, beginning with the highest parent (i.e. the root domain)
         for i, host in enumerate(parents[::-1]):
             # have we checked this host before?
             host_hash = hash(host)
             async with self._wildcard_lock.lock(host_hash):
                 # if we've seen this host before
                 if host_hash in self._wildcard_cache:
                     wildcard_domain_results[host] = self._wildcard_cache[host_hash]
                     continue
 
                 # determine if this is a wildcard domain
-                wildcard_tasks = {t: [] for t in self.all_rdtypes}
+                wildcard_tasks = {t: [] for t in rdtypes_to_check}
                 # resolve a bunch of random subdomains of the same parent
-                for rdtype in self.all_rdtypes:
+                for rdtype in rdtypes_to_check:
                     # continue if a wildcard was already found for this rdtype
                     # if rdtype in self._wildcard_cache[host_hash]:
                     #     continue
                     for _ in range(self.wildcard_tests):
                         rand_query = f"{rand_string(digits=False, length=10)}.{host}"
                         wildcard_tasks[rdtype].append(self.resolve(rand_query, type=rdtype, cache_result=False))
 
@@ -592,14 +665,18 @@
                     async for task in as_completed(tasks):
                         results = await task
                         if results:
                             is_wildcard = True
                             if not rdtype in wildcard_results:
                                 wildcard_results[rdtype] = set()
                             wildcard_results[rdtype].update(results)
+                            # we know this rdtype is a wildcard
+                            # so we don't need to check it anymore
+                            with suppress(KeyError):
+                                rdtypes_to_check.remove(rdtype)
 
                 self._wildcard_cache.update({host_hash: wildcard_results})
                 wildcard_domain_results.update({host: wildcard_results})
                 if is_wildcard:
                     wildcard_rdtypes_str = ",".join(sorted([t.upper() for t, r in wildcard_results.items() if r]))
                     log_fn = log.verbose
                     if log_info:
```

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/files.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/helper.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/logger.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/misc.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/modules.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/punycode.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/url.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/validators.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/web.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import re
 import ssl
 import anyio
 import httpx
 import logging
+import warnings
 import traceback
 from pathlib import Path
 from bs4 import BeautifulSoup
 
 from httpx._models import Cookies
 
 from bbot.core.errors import WordlistError, CurlError
 from bbot.core.helpers.ratelimiter import RateLimiter
 
+from bs4 import MarkupResemblesLocatorWarning
+from bs4.builder import XMLParsedAsHTMLWarning
+
+warnings.filterwarnings("ignore", category=XMLParsedAsHTMLWarning)
+warnings.filterwarnings("ignore", category=MarkupResemblesLocatorWarning)
+
 log = logging.getLogger("bbot.core.helpers.web")
 
 
 class DummyCookies(Cookies):
     def extract_cookies(self, *args, **kwargs):
         pass
 
@@ -116,25 +123,28 @@
             kwargs["method"] = "GET"
 
         client_kwargs = {}
         for k in list(kwargs):
             if k in self.client_only_options:
                 v = kwargs.pop(k)
                 client_kwargs[k] = v
+
         if client_kwargs:
             client = self.AsyncClient(**client_kwargs)
 
         try:
             if self.http_debug:
                 logstr = f"Web request: {str(args)}, {str(kwargs)}"
                 log.debug(logstr)
             async with self.web_rate_limiter:
                 response = await client.request(*args, **kwargs)
             if self.http_debug:
-                log.debug(f"Web response: {response} (Length: {len(response.content)}) headers: {response.headers}")
+                log.debug(
+                    f"Web response from {url}: {response} (Length: {len(response.content)}) headers: {response.headers}"
+                )
             return response
         except httpx.TimeoutException:
             log.verbose(f"HTTP timeout to URL: {url}")
             if raise_error:
                 raise
         except httpx.ConnectError:
             log.verbose(f"HTTP connect failed to URL: {url}")
```

### Comparing `bbot-1.1.0.2043rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.0.2083rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/core/logger/logger.py` & `bbot-1.1.0.2083rc0/bbot/core/logger/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,21 +118,23 @@
 
 
 def log_worker_setup(logging_queue):
     """
     This needs to be run whenever a new multiprocessing.Process() is spawned
     """
     log_level = get_log_level()
-    log = logging.getLogger("bbot")
+    bbot_log = logging.getLogger("bbot")
+    asyncio_log = logging.getLogger("asyncio")
     # Don't do this more than once
-    if len(log.handlers) == 0:
-        log.setLevel(log_level)
+    if len(bbot_log.handlers) == 0:
         queue_handler = QueueHandler(logging_queue)
-        log.addHandler(queue_handler)
-    return log
+        for log in (bbot_log, asyncio_log):
+            log.setLevel(log_level)
+            log.addHandler(queue_handler)
+    return bbot_log
 
 
 def log_listener_setup(logging_queue):
     log_dir = Path(config["home"]) / "logs"
     if not mkdir(log_dir, raise_error=False):
         error_and_exit(f"Failure creating or error writing to BBOT logs directory ({log_dir})")
 
@@ -218,17 +220,16 @@
 
 def set_log_level(level, logger=None):
     global _log_level_override
     if logger is not None:
         logger.hugeinfo(f"Setting log level to {logging.getLevelName(level)}")
     config["silent"] = False
     _log_level_override = level
-    log = logging.getLogger("bbot")
-    log.setLevel(level)
-    logging.getLogger("asyncio").setLevel(level)
+    for logname in ("bbot", "asyncio"):
+        logging.getLogger(logname).setLevel(level)
 
 
 def toggle_log_level(logger=None):
     log_level = get_log_level()
     if log_level in verbosity_levels_toggle:
         for i, level in enumerate(verbosity_levels_toggle):
             if log_level == level:
```

### Comparing `bbot-1.1.0.2043rc0/bbot/db/neo4j.py` & `bbot-1.1.0.2083rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/defaults.yml` & `bbot-1.1.0.2083rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/anubisdb.py` & `bbot-1.1.0.2083rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/azure_realm.py` & `bbot-1.1.0.2083rc0/bbot/modules/azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.0.2083rc0/bbot/modules/azure_tenant.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.d_xml_regex = re.compile(r"<Domain>([^<>/]*)</Domain>", re.I)
         return True
 
     async def handle_event(self, event):
         _, query = self.helpers.split_domain(event.data)
         domains, _ = await self.query(query)
         if domains:
-            self.success(f'Found {len(domains):,} domains under tenant for "{query}"')
+            self.success(f'Found {len(domains):,} domains under tenant for "{query}": {", ".join(sorted(domains))}')
         for domain in domains:
             if domain != query:
                 self.emit_event(domain, "DNS_NAME", source=event, tags=["affiliate"])
         # todo: tenants?
 
     async def query(self, domain):
         url = f"{self.base_url}/autodiscover/autodiscover.svc"
@@ -52,18 +52,18 @@
             "SOAPAction": '"http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformation"',
             "User-Agent": "AutodiscoverClient",
             "Accept-Encoding": "identity",
         }
 
         self.debug(f"Retrieving tenant domains at {url}")
 
-        r = await self.request_with_fail_count(url, method="POST", headers=headers, data=data)
+        r = await self.helpers.request(url, method="POST", headers=headers, data=data)
         status_code = getattr(r, "status_code", 0)
         if status_code not in (200, 421):
-            self.warning(f'Error retrieving azure_tenant domains for "{domain}" (status code: {status_code})')
+            self.verbose(f'Error retrieving azure_tenant domains for "{domain}" (status code: {status_code})')
             return set(), set()
         found_domains = list(set(self.d_xml_regex.findall(r.text)))
         domains = set()
         tenantnames = set()
 
         for d in found_domains:
             # tenant names
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/badsecrets.py` & `bbot-1.1.0.2083rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/base.py` & `bbot-1.1.0.2083rc0/bbot/modules/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 import traceback
 from sys import exc_info
 from contextlib import suppress
 
-from ..core.helpers.misc import get_size
+from ..core.helpers.misc import get_size  # noqa
 from ..core.helpers.async_helpers import TaskCounter
 from ..core.errors import ValidationError, WordlistError
 
 
 class BaseModule:
     # Event types to watch
     watched_events = []
@@ -98,15 +98,14 @@
 
         # track number of failures (for .request_with_fail_count())
         self._request_failures = 0
 
         self._tasks = []
         self._event_received = asyncio.Condition()
         self._event_queued = asyncio.Condition()
-        self._event_dequeued = asyncio.Condition()
 
         # used for optional "per host" tracking
         self._per_host_tracker = set()
 
     async def setup(self):
         """
         Perform setup functions at the beginning of the scan.
@@ -207,28 +206,28 @@
         """
         if self._watched_events is None:
             self._watched_events = set(self.watched_events)
         return self._watched_events
 
     async def _handle_batch(self):
         finish = False
-        async with self._task_counter.count("handle_batch()"):
+        async with self._task_counter.count(f"{self.name}.handle_batch()"):
             submitted = False
             if self.batch_size <= 1:
                 return
             if self.num_incoming_events > 0:
                 events, finish = await self.events_waiting()
-                if not self.errored:
+                if events and not self.errored:
                     self.debug(f"Handling batch of {len(events):,} events")
-                    if events:
-                        submitted = True
-                        async with self.scan.acatch("handle_batch()"):
-                            await self.handle_batch(*events)
+                    submitted = True
+                    async with self.scan.acatch(f"{self.name}.handle_batch()"):
+                        await self.handle_batch(*events)
+                    self.debug(f"Finished handling batch of {len(events):,} events")
         if finish:
-            context = "finish()"
+            context = f"{self.name}.finish()"
             async with self.scan.acatch(context), self._task_counter.count(context):
                 await self.finish()
         return submitted
 
     def make_event(self, *args, **kwargs):
         raise_error = kwargs.pop("raise_error", False)
         try:
@@ -249,14 +248,22 @@
             v = event_kwargs.pop(o, None)
             if v is not None:
                 emit_kwargs[o] = v
         event = self.make_event(*args, **event_kwargs)
         if event:
             self.queue_outgoing_event(event, **emit_kwargs)
 
+    async def emit_event_wait(self, *args, **kwargs):
+        """
+        Same as emit_event except we wait on the outgoing queue
+        """
+        while self.outgoing_event_queue.qsize() > self._qsize:
+            await self.helpers.sleep(0.2)
+        return self.emit_event(*args, **kwargs)
+
     async def events_waiting(self):
         """
         yields all events in queue, up to maximum batch size
         """
         events = []
         finish = False
         while self.incoming_event_queue:
@@ -341,22 +348,24 @@
                         self.debug(f"Got {event} from {getattr(event, 'module', 'unknown_module')}")
                         async with self._task_counter.count(f"event_postcheck({event})"):
                             acceptable, reason = await self._event_postcheck(event)
                         if not acceptable:
                             self.debug(f"Not accepting {event} because {reason}")
                         if acceptable:
                             if event.type == "FINISHED":
-                                context = "finish()"
+                                context = f"{self.name}.finish()"
                                 async with self.scan.acatch(context), self._task_counter.count(context):
                                     await self.finish()
                             else:
-                                context = f"handle_event({event})"
+                                context = f"{self.name}.handle_event({event})"
                                 self.scan.stats.event_consumed(event, self)
+                                self.debug(f"Handling {event}")
                                 async with self.scan.acatch(context), self._task_counter.count(context):
                                     await self.handle_event(event)
+                                self.debug(f"Finished handling {event}")
             except asyncio.CancelledError:
                 self.log.trace("Worker cancelled")
                 self.trace()
                 raise
         self.log.trace(f"Worker stopped")
 
     @property
@@ -455,24 +464,24 @@
                 )
         return True, ""
 
     async def _cleanup(self):
         if not self._cleanedup:
             self._cleanedup = True
             for callback in [self.cleanup] + self.cleanup_callbacks:
-                context = f"cleanup()"
+                context = f"{self.name}.cleanup()"
                 if callable(callback):
                     async with self.scan.acatch(context), self._task_counter.count(context):
                         await self.helpers.execute_sync_or_async(callback)
 
     async def queue_event(self, event):
         """
         Queue (incoming) event with module
         """
-        async with self._task_counter.count("queue_event()"):
+        async with self._task_counter.count("queue_event()", _log=False):
             if self.incoming_event_queue is False:
                 self.debug(f"Not in an acceptable state to queue incoming event")
                 return
             acceptable, reason = self._event_precheck(event)
             if not acceptable:
                 if reason and reason != "its type is not in watched_events":
                     self.debug(f"Not accepting {event} because {reason}")
@@ -493,24 +502,14 @@
         Queue (outgoing) event with module
         """
         try:
             self.outgoing_event_queue.put_nowait((event, kwargs))
         except AttributeError:
             self.debug(f"Not in an acceptable state to queue outgoing event")
 
-    async def dequeue_outgoing_event(self):
-        await self.outgoing_event_queue.get()
-        with self._event_dequeued:
-            self._event_dequeued.notify()
-
-    def dequeue_outgoing_event_nowait(self):
-        return self.outgoing_event_queue.get_nowait()
-        with self._event_dequeued:
-            self._event_dequeued.notify()
-
     def set_error_state(self, message=None):
         if not self.errored:
             log_msg = f"Setting error state for module {self.name}"
             if message is not None:
                 log_msg += f": {message}"
             self.warning(log_msg)
             self.errored = True
@@ -618,15 +617,15 @@
         return self._log
 
     @property
     def memory_usage(self):
         """
         Return how much memory the module is currently using in bytes
         """
-        seen = {self.scan, self.helpers, self.log}
+        seen = {self.scan, self.helpers, self.log}  # noqa
         return get_size(self, max_depth=3, seen=seen)
 
     def __str__(self):
         return self.name
 
     def log_table(self, *args, **kwargs):
         table_name = kwargs.pop("table_name", None)
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/bevigil.py` & `bbot-1.1.0.2083rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/binaryedge.py` & `bbot-1.1.0.2083rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/bucket_aws.py` & `bbot-1.1.0.2083rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.0.2083rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.0.2083rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.0.2083rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/bucket_gcp.py` & `bbot-1.1.0.2083rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/builtwith.py` & `bbot-1.1.0.2083rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/bypass403.py` & `bbot-1.1.0.2083rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/c99.py` & `bbot-1.1.0.2083rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/censys.py` & `bbot-1.1.0.2083rc0/bbot/modules/censys.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 class censys(shodan_dns):
     """
     thanks to https://github.com/owasp-amass/amass/blob/master/resources/scripts/cert/censys.ads
     """
 
     watched_events = ["DNS_NAME"]
-    produced_events = ["DNS_NAME", "EMAIL_ADDRESS", "IP_ADDRESS", "OPEN_PORT", "PROTOCOL"]
-    flags = ["subdomain-enum", "email-enum", "passive", "safe"]
+    produced_events = ["DNS_NAME"]
+    flags = ["subdomain-enum", "passive", "safe"]
     meta = {"description": "Query the Censys API", "auth_required": True}
     options = {"api_id": "", "api_secret": "", "max_pages": 5}
     options_desc = {
         "api_id": "Censys.io API ID",
         "api_secret": "Censys.io API Secret",
         "max_pages": "Maximum number of pages to fetch (100 results per page)",
     }
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/certspotter.py` & `bbot-1.1.0.2083rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/columbus.py` & `bbot-1.1.0.2083rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/crobat.py` & `bbot-1.1.0.2083rc0/bbot/modules/crobat.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         if parse_fn is None:
             parse_fn = self.parse_results
         if request_fn is None:
             request_fn = self.request_url
         try:
             response = await request_fn(query)
             if response is None:
-                self.info(f'Query "{query}" failed')
+                self.info(f'Query "{query}" failed (no response)')
                 return []
             try:
                 results = list(parse_fn(response, query))
             except Exception as e:
                 if response:
                     self.info(
                         f'Error parsing results for query "{query}" (status code {response.status_code})', trace=True
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/crt.py` & `bbot-1.1.0.2083rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.0.2083rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.0.2083rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.0.2083rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/digitorus.py` & `bbot-1.1.0.2083rc0/bbot/modules/digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.0.2083rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.0.2083rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.1.0.2083rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/emailformat.py` & `bbot-1.1.0.2083rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.0.2083rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.0.2083rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/fullhunt.py` & `bbot-1.1.0.2083rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.0.2083rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/git.py` & `bbot-1.1.0.2083rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/github.py` & `bbot-1.1.0.2083rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/gowitness.py` & `bbot-1.1.0.2083rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/hackertarget.py` & `bbot-1.1.0.2083rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/host_header.py` & `bbot-1.1.0.2083rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/httpx.py` & `bbot-1.1.0.2083rc0/bbot/modules/httpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,15 @@
             return False, "event has spider danger"
 
         # scope filtering
         in_scope_only = self.config.get("in_scope_only", True)
         safe_to_visit = "httpx-safe" in event.tags
         if not safe_to_visit and (in_scope_only and not self.scan.in_scope(event)):
             return False, "event is not in scope"
-        # reject base URLs to avoid visiting a resource twice
-        # note: speculate makes open ports from
+
         return True
 
     async def handle_batch(self, *events):
         stdin = {}
         for e in events:
             url_hash = None
             if e.type.startswith("URL"):
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/hunt.py` & `bbot-1.1.0.2083rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/hunterio.py` & `bbot-1.1.0.2083rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.0.2083rc0/bbot/modules/iis_shortnames.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,19 @@
         while 1:
             payload = encode_all(f"{base_hint}~{str(count)}*")
             url = f"{target}{payload}{suffix}"
 
             duplicate_check_results = await self.helpers.request(
                 method=method, url=url, allow_redirects=False, retries=2, timeout=10
             )
+
+            if not duplicate_check_results:
+                self.debug("duplicate check produced NoneType sample")
+                break
+
             if duplicate_check_results.status_code != affirmative_status_code:
                 break
             else:
                 duplicates.append(f"{base_hint}~{str(count)}")
                 count += 1
 
             if count > 5:
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/internal/base.py` & `bbot-1.1.0.2083rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.0.2083rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.0.2083rc0/bbot/modules/internal/speculate.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     meta = {"description": "Derive certain event types from others by common sense"}
 
     options = {"max_hosts": 65536, "ports": "80,443"}
     options_desc = {
         "max_hosts": "Max number of IP_RANGE hosts to convert into IP_ADDRESS events",
         "ports": "The set of ports to speculate on",
     }
-    max_event_handlers = 5
     scope_distance_modifier = 1
     _scope_shepherding = False
     _priority = 4
 
     async def setup(self):
         self.open_port_consumers = any(["OPEN_TCP_PORT" in m.watched_events for m in self.scan.modules.values()])
         self.portscanner_enabled = any(["portscan" in m.flags for m in self.scan.modules.values()])
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.0.2083rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/ipstack.py` & `bbot-1.1.0.2083rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/leakix.py` & `bbot-1.1.0.2083rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/masscan.py` & `bbot-1.1.0.2083rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/massdns.py` & `bbot-1.1.0.2083rc0/bbot/modules/massdns.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,57 +117,98 @@
         if hash(hostname) in self.processed:
             return True
         return False
 
     async def massdns(self, domain, subdomains):
         subdomains = list(subdomains)
 
+        domain_wildcard_rdtypes = set()
+        for domain, rdtypes in (await self.helpers.is_wildcard_domain(domain)).items():
+            for rdtype, results in rdtypes.items():
+                if results:
+                    domain_wildcard_rdtypes.add(rdtype)
+
+        if "A" in domain_wildcard_rdtypes:
+            self.info(
+                f"Aborting massdns on {domain} because it's a wildcard domain ({','.join(domain_wildcard_rdtypes)})"
+            )
+            self.found.pop(domain, None)
+            return []
+        else:
+            self.log.trace(f"{domain}: A is not in domain_wildcard_rdtypes:{domain_wildcard_rdtypes}")
+
         # before we start, do a canary check for wildcards
         abort_msg = f"Aborting massdns on {domain} due to false positive"
         canary_result = await self._canary_check(domain)
         if canary_result:
             self.info(abort_msg + f": {canary_result}")
             return []
+        else:
+            self.log.trace(f"Canary result for {domain}: {canary_result}")
 
-        results = [l async for l in self._massdns(domain, subdomains)]
+        results = []
+        async for hostname, ip, rdtype in self._massdns(domain, subdomains):
+            # allow brute-forcing of wildcard domains
+            # this is dead code but it's kinda cool so it can live here
+            if rdtype in domain_wildcard_rdtypes:
+                # skip wildcard checking on multi-level subdomains for performance reasons
+                stem = hostname.split(domain)[0].strip(".")
+                if "." in stem:
+                    self.debug(f"Skipping {hostname}:A because it may be a wildcard (reason: performance)")
+                    continue
+                wildcard_rdtypes = await self.helpers.is_wildcard(hostname, ips=(ip,), rdtype=rdtype)
+                if rdtype in wildcard_rdtypes:
+                    self.debug(f"Skipping {hostname}:{rdtype} because it's a wildcard")
+                    continue
+            results.append(hostname)
 
         # do another canary check for good measure
         if len(results) > 50:
             canary_result = await self._canary_check(domain)
             if canary_result:
                 self.info(abort_msg + f": {canary_result}")
                 return []
+            else:
+                self.log.trace(f"Canary result for {domain}: {canary_result}")
 
         # abort if there are a suspiciously high number of results
         # (the results are over 2000, and this is more than 20 percent of the input size)
-        if len(results) > 2000 and len(results) / len(subdomains) > 0.2:
-            self.info(
-                f"Aborting because the number of results ({len(results):,}) is suspiciously high for the length of the wordlist ({len(subdomains):,})"
-            )
-            return []
+        if len(results) > 2000:
+            if len(results) / len(subdomains) > 0.2:
+                self.info(
+                    f"Aborting because the number of results ({len(results):,}) is suspiciously high for the length of the wordlist ({len(subdomains):,})"
+                )
+                return []
+            else:
+                self.info(
+                    f"{len(results):,} results returned from massdns against {domain} (wordlist size = {len(subdomains):,})"
+                )
 
         # everything checks out
         self.verbose(f"Resolving batch of {len(results):,} results")
         resolved = dict([l async for l in self.helpers.resolve_batch(results, type=("A", "CNAME"), cache_result=True)])
         resolved = {k: v for k, v in resolved.items() if v}
         for hostname in resolved:
             self.add_found(hostname)
         return list(resolved)
 
-    async def _canary_check(self, domain, num_checks=100):
+    async def _canary_check(self, domain, num_checks=50):
         random_subdomains = list(self.gen_random_subdomains(num_checks))
         self.verbose(f"Testing {len(random_subdomains):,} canaries against {domain}")
-        canary_results = [l async for l in self._massdns(domain, random_subdomains)]
+        canary_results = [h async for h, d, r in self._massdns(domain, random_subdomains)]
+        self.log.trace(f"canary results for {domain}: {canary_results}")
         resolved_canaries = self.helpers.resolve_batch(canary_results)
+        self.log.trace(f"resolved canary results for {domain}: {canary_results}")
         async for query, result in resolved_canaries:
             if result:
                 await resolved_canaries.aclose()
                 result = f"{query}:{result}"
                 self.log.trace(f"Found false positive: {result}")
                 return result
+        self.log.trace(f"Passed canary check for {domain}")
         return False
 
     async def _massdns(self, domain, subdomains):
         """
         {
           "name": "www.blacklanternsecurity.com.",
           "type": "A",
@@ -193,20 +234,14 @@
           },
           "resolver": "168.215.165.186:53"
         }
         """
         if self.scan.stopping:
             return
 
-        domain_wildcard_rdtypes = set()
-        for domain, rdtypes in (await self.helpers.is_wildcard_domain(domain)).items():
-            for rdtype, results in rdtypes.items():
-                if results:
-                    domain_wildcard_rdtypes.add(rdtype)
-
         command = (
             "massdns",
             "-r",
             self.resolver_file,
             "-s",
             self.max_resolvers,
             "-t",
@@ -229,31 +264,18 @@
                 hostname = answer.get("name", "").strip(".").lower()
                 if hostname.endswith(f".{domain}"):
                     data = answer.get("data", "")
                     rdtype = answer.get("type", "").upper()
                     # avoid garbage answers like this:
                     # 8AAAA queries have been locally blocked by dnscrypt-proxy/Set block_ipv6 to false to disable this feature
                     if data and rdtype and not " " in data:
-                        # skip wildcards
-                        if rdtype in domain_wildcard_rdtypes:
-                            # skip wildcard checking on multi-level subdomains for performance reasons
-                            stem = hostname.split(domain)[0].strip(".")
-                            if "." in stem:
-                                self.debug(
-                                    f"Skipping {hostname}:{rdtype} because it may be a wildcard (reason: performance)"
-                                )
-                                continue
-                            wildcard_rdtypes = await self.helpers.is_wildcard(hostname, ips=(data,))
-                            if rdtype in wildcard_rdtypes:
-                                self.debug(f"Skipping {hostname}:{rdtype} because it's a wildcard")
-                                continue
                         hostname_hash = hash(hostname)
                         if hostname_hash not in hosts_yielded:
                             hosts_yielded.add(hostname_hash)
-                            yield hostname
+                            yield hostname, data, rdtype
 
     async def finish(self):
         found = sorted(self.found.items(), key=lambda x: len(x[-1]), reverse=True)
         # if we have a lot of rounds to make, don't try mutations on less-populated domains
         trimmed_found = []
         if found:
             avg_subdomains = sum([len(subdomains) for domain, subdomains in found[:50]]) / len(found[:50])
@@ -331,48 +353,52 @@
                     if mutations:
                         self.info(f"Trying {len(mutations):,} mutations against {domain} ({i+1}/{len(found)})")
                         results = list(await self.massdns(query, mutations))
                         for hostname in results:
                             source_event = self.get_source_event(hostname)
                             if source_event is None:
                                 self.warning(f"Could not correlate source event from: {hostname}")
-                                continue
+                                source_event = self.scan.root_event
                             self.emit_result(hostname, source_event, query)
                         if results:
                             continue
                     break
         except AssertionError as e:
             self.warning(e)
 
     def add_found(self, host):
         if not isinstance(host, str):
             host = host.data
         if self.helpers.is_subdomain(host):
             subdomain, domain = host.split(".", 1)
-            if not self.helpers.is_ptr(subdomain):
+            is_ptr = self.helpers.is_ptr(subdomain)
+            in_scope = self.scan.in_scope(domain)
+            if in_scope and not is_ptr:
                 try:
                     self.found[domain].add(subdomain)
                 except KeyError:
                     self.found[domain] = set((subdomain,))
 
     async def gen_subdomains(self, prefixes, domain):
         for p in prefixes:
             d = f"{p}.{domain}"
             yield d
 
     def gen_random_subdomains(self, n=50):
         delimeters = (".", "-")
-        lengths = list(range(10, 20))
-        for i in range(0, n):
+        lengths = list(range(3, 8))
+        for i in range(0, max(0, n - 5)):
             d = delimeters[i % len(delimeters)]
             l = lengths[i % len(lengths)]
             segments = list(random.choice(self.devops_mutations) for _ in range(l))
             segments.append(self.helpers.rand_string(length=8, digits=False))
             subdomain = d.join(segments)
             yield subdomain
+        for _ in range(5):
+            yield self.helpers.rand_string(length=8, digits=False)
 
     def get_source_event(self, hostname):
         for p in self.helpers.domain_parents(hostname):
             try:
                 return self.source_events[hash(p)]
             except KeyError:
                 continue
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/myssl.py` & `bbot-1.1.0.2083rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/nmap.py` & `bbot-1.1.0.2083rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/nsec.py` & `bbot-1.1.0.2083rc0/bbot/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/ntlm.py` & `bbot-1.1.0.2083rc0/bbot/modules/ntlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from bbot.modules.base import BaseModule
-from bbot.core.errors import NTLMError, RequestError, ReadTimeout
+from bbot.core.errors import NTLMError, HTTPError
 
 ntlm_discovery_endpoints = [
     "",
     "autodiscover/autodiscover.xml",
     "ecp/",
     "ews/",
     "ews/exchange.asmx",
@@ -121,29 +121,31 @@
         for url in urls:
             url_hash = hash(url)
             if url_hash in self.processed:
                 continue
             self.processed.add(url_hash)
             tasks.append(self.helpers.create_task(self.check_ntlm(url)))
 
+        result, url = None, None
+
         gen = self.helpers.as_completed(tasks)
         async for task in gen:
             try:
                 result, url = await task
                 if result:
                     await self.helpers.cancel_tasks(tasks)
-                    return result, url
-            except (RequestError, ReadTimeout) as e:
+                    await gen.aclose()
+            except HTTPError as e:
                 if str(e):
                     self.warning(str(e))
                 # cancel all the tasks if there's an error
                 await self.helpers.cancel_tasks(tasks)
                 await gen.aclose()
 
-        return None, None
+        return result, url
 
     async def check_ntlm(self, test_url):
         # use lower timeout value
         http_timeout = self.config.get("httpx_timeout", 5)
         r = await self.helpers.request(
             test_url, headers=NTLM_test_header, raise_error=True, allow_redirects=False, timeout=http_timeout
         )
```

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/oauth.py` & `bbot-1.1.0.2083rc0/bbot/modules/oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/otx.py` & `bbot-1.1.0.2083rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/base.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/csv.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/http.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/human.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/json.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/subdomains.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/web_report.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/output/websocket.py` & `bbot-1.1.0.2083rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.0.2083rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.0.2083rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.0.2083rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/passivetotal.py` & `bbot-1.1.0.2083rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/pgp.py` & `bbot-1.1.0.2083rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/rapiddns.py` & `bbot-1.1.0.2083rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.0.2083rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/report/asn.py` & `bbot-1.1.0.2083rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/riddler.py` & `bbot-1.1.0.2083rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/robots.py` & `bbot-1.1.0.2083rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/secretsdb.py` & `bbot-1.1.0.2083rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/securitytrails.py` & `bbot-1.1.0.2083rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.0.2083rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/skymem.py` & `bbot-1.1.0.2083rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/smuggler.py` & `bbot-1.1.0.2083rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/social.py` & `bbot-1.1.0.2083rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/sslcert.py` & `bbot-1.1.0.2083rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.1.0.2083rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/subdomaincenter.py` & `bbot-1.1.0.2083rc0/bbot/modules/subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/telerik.py` & `bbot-1.1.0.2083rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/threatminer.py` & `bbot-1.1.0.2083rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.0.2083rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/urlscan.py` & `bbot-1.1.0.2083rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/viewdns.py` & `bbot-1.1.0.2083rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/virustotal.py` & `bbot-1.1.0.2083rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/wafw00f.py` & `bbot-1.1.0.2083rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.0.2083rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/wayback.py` & `bbot-1.1.0.2083rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/modules/zoomeye.py` & `bbot-1.1.0.2083rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.0.2083rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/scanner/manager.py` & `bbot-1.1.0.2083rc0/bbot/scanner/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,21 +456,19 @@
                 total = sum([incoming, outgoing, tasks])
                 if running or total > 0:
                     modules_status.append((m, running, incoming, outgoing, tasks, total))
             modules_status.sort(key=lambda x: x[-1], reverse=True)
 
             if modules_status:
                 modules_status_str = ", ".join([f"{m}({i:,}:{t:,}:{o:,})" for m, r, i, o, t, _ in modules_status])
-                running_modules_str = ", ".join([m[0] for m in modules_status if m[1]])
-                if not running_modules_str:
-                    running_modules_str = "None"
-                self.scan.info(f"{self.scan.name}: Modules running: {running_modules_str}")
-                self.scan.verbose(
-                    f"{self.scan.name}: Modules status (incoming:processing:outgoing) {modules_status_str}"
+                self.scan.info(
+                    f"{self.scan.name}: Modules running (incoming:processing:outgoing) {modules_status_str}"
                 )
+            else:
+                self.scan.info(f"{self.scan.name}: No modules running")
             event_type_summary = sorted(
                 self.scan.stats.events_emitted_by_type.items(), key=lambda x: x[-1], reverse=True
             )
             if event_type_summary:
                 self.scan.info(
                     f'{self.scan.name}: Events produced so far: {", ".join([f"{k}: {v}" for k,v in event_type_summary])}'
                 )
@@ -497,27 +495,27 @@
                 # status debugging
                 scan_active_status = []
                 scan_active_status.append(f"scan._finished_init: {self.scan._finished_init}")
                 scan_active_status.append(f"manager.active: {self.active}")
                 scan_active_status.append(f"    manager.running: {self.running}")
                 scan_active_status.append(f"        manager._task_counter.value: {self._task_counter.value}")
                 scan_active_status.append(f"        manager._task_counter.tasks:")
-                for task in self._task_counter.tasks.values():
+                for task in list(self._task_counter.tasks.values()):
                     scan_active_status.append(f"            - {task}:")
                 scan_active_status.append(
                     f"        manager.incoming_event_queue.qsize: {self.incoming_event_queue.qsize()}"
                 )
                 scan_active_status.append(f"    manager.modules_finished: {self.modules_finished}")
                 for m in sorted(self.scan.modules.values(), key=lambda m: m.name):
                     running = m.running
                     scan_active_status.append(f"        {m}.finished: {m.finished}")
                     scan_active_status.append(f"            running: {running}")
                     if running:
                         scan_active_status.append(f"            tasks:")
-                        for task in m._task_counter.tasks.values():
+                        for task in list(m._task_counter.tasks.values()):
                             scan_active_status.append(f"                - {task}:")
                     scan_active_status.append(f"            num_incoming_events: {m.num_incoming_events}")
                     scan_active_status.append(
                         f"            outgoing_event_queue.qsize: {m.outgoing_event_queue.qsize()}"
                     )
                 for line in scan_active_status:
                     self.scan.debug(line)
```

### Comparing `bbot-1.1.0.2043rc0/bbot/scanner/scanner.py` & `bbot-1.1.0.2083rc0/bbot/scanner/scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -777,8 +777,8 @@
             log.debug(f"BrokenPipeError in {filename}:{lineno}:{funcname}(): {e}")
         elif isinstance(e, asyncio.CancelledError):
             raise
         elif isinstance(e, Exception):
             log.error(f"Error in {context}: {filename}:{lineno}:{funcname}(): {e}")
             log.trace(traceback.format_exc())
         if callable(finally_callback):
-            self.helpers.execute_sync_or_async(finally_callback, e)
+            finally_callback(e)
```

### Comparing `bbot-1.1.0.2043rc0/bbot/scanner/stats.py` & `bbot-1.1.0.2083rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/scanner/target.py` & `bbot-1.1.0.2083rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/scripts/docs.py` & `bbot-1.1.0.2083rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.0.2083rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/conftest.py` & `bbot-1.1.0.2083rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/run_tests.sh` & `bbot-1.1.0.2083rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test.conf` & `bbot-1.1.0.2083rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_dns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ..bbot_fixtures import *
 
 
 @pytest.mark.asyncio
 async def test_dns(bbot_scanner, bbot_config):
-    scan = bbot_scanner("8.8.8.8")
+    scan = bbot_scanner("8.8.8.8", config=bbot_config)
     helpers = scan.helpers
 
     # lowest level functions
     a_responses = await helpers._resolve_hostname("dns.google")
     aaaa_responses = await helpers._resolve_hostname("dns.google", rdtype="AAAA")
     ip_responses = await helpers._resolve_ip("8.8.8.8")
     assert a_responses[0].response.answer[0][0].address in ("8.8.8.8", "8.8.4.4")
@@ -58,34 +58,59 @@
     assert hash(f"dns.google:AAAA") not in helpers.dns._dns_cache
     await helpers.resolve("8.8.8.8", cache_result=True)
     assert hash(f"8.8.8.8:PTR") in helpers.dns._dns_cache
     await helpers.resolve("dns.google", cache_result=True)
     assert hash(f"dns.google:A") in helpers.dns._dns_cache
     assert hash(f"dns.google:AAAA") in helpers.dns._dns_cache
 
+    # Ensure events with hosts have resolved_hosts attribute populated
+    resolved_hosts_event1 = scan.make_event("dns.google", "DNS_NAME", dummy=True)
+    resolved_hosts_event2 = scan.make_event("http://dns.google/", "URL_UNVERIFIED", dummy=True)
+    event_tags1, event_whitelisted1, event_blacklisted1, children1 = await scan.helpers.resolve_event(
+        resolved_hosts_event1
+    )
+    event_tags2, event_whitelisted2, event_blacklisted2, children2 = await scan.helpers.resolve_event(
+        resolved_hosts_event2
+    )
+    assert "8.8.8.8" in [str(x) for x in children1["A"]]
+    assert "8.8.8.8" in [str(x) for x in children2["A"]]
+    assert set(children1.keys()) == set(children2.keys())
+
+
+@pytest.mark.asyncio
+async def test_wildcards(bbot_scanner, bbot_config):
+    scan = bbot_scanner("8.8.8.8", config=bbot_config)
+    helpers = scan.helpers
+
     # wildcards
     wildcard_domains = await helpers.is_wildcard_domain("asdf.github.io")
+    assert hash("github.io") in helpers.dns._wildcard_cache
+    assert hash("asdf.github.io") in helpers.dns._wildcard_cache
     assert "github.io" in wildcard_domains
     assert "A" in wildcard_domains["github.io"]
     assert "SRV" not in wildcard_domains["github.io"]
     assert wildcard_domains["github.io"]["A"] and all(helpers.is_ip(r) for r in wildcard_domains["github.io"]["A"])
+    helpers.dns._wildcard_cache.clear()
 
     wildcard_rdtypes = await helpers.is_wildcard("blacklanternsecurity.github.io")
     assert "A" in wildcard_rdtypes
     assert "SRV" not in wildcard_rdtypes
     assert wildcard_rdtypes["A"] == (True, "github.io")
     assert hash("github.io") in helpers.dns._wildcard_cache
     assert len(helpers.dns._wildcard_cache[hash("github.io")]) > 0
     helpers.dns._wildcard_cache.clear()
 
     wildcard_rdtypes = await helpers.is_wildcard("asdf.asdf.asdf.github.io")
     assert "A" in wildcard_rdtypes
     assert "SRV" not in wildcard_rdtypes
     assert wildcard_rdtypes["A"] == (True, "github.io")
     assert hash("github.io") in helpers.dns._wildcard_cache
+    assert not hash("asdf.github.io") in helpers.dns._wildcard_cache
+    assert not hash("asdf.asdf.github.io") in helpers.dns._wildcard_cache
+    assert not hash("asdf.asdf.asdf.github.io") in helpers.dns._wildcard_cache
     assert len(helpers.dns._wildcard_cache[hash("github.io")]) > 0
     wildcard_event1 = scan.make_event("wat.asdf.fdsa.github.io", "DNS_NAME", dummy=True)
     wildcard_event2 = scan.make_event("wats.asd.fdsa.github.io", "DNS_NAME", dummy=True)
     wildcard_event3 = scan.make_event("github.io", "DNS_NAME", dummy=True)
 
     # event resolution
     event_tags1, event_whitelisted1, event_blacklisted1, children1 = await scan.helpers.resolve_event(wildcard_event1)
@@ -102,20 +127,7 @@
     assert "srv-wildcard" not in wildcard_event2.tags
     assert wildcard_event1.data == "_wildcard.github.io"
     assert wildcard_event2.data == "_wildcard.github.io"
     assert wildcard_event1.tags == wildcard_event2.tags
     assert "wildcard-domain" in wildcard_event3.tags
     assert "a-wildcard-domain" in wildcard_event3.tags
     assert "srv-wildcard-domain" not in wildcard_event3.tags
-
-    # Ensure events with hosts have resolved_hosts attribute populated
-    resolved_hosts_event1 = scan.make_event("dns.google", "DNS_NAME", dummy=True)
-    resolved_hosts_event2 = scan.make_event("http://dns.google/", "URL_UNVERIFIED", dummy=True)
-    event_tags1, event_whitelisted1, event_blacklisted1, children1 = await scan.helpers.resolve_event(
-        resolved_hosts_event1
-    )
-    event_tags2, event_whitelisted2, event_blacklisted2, children2 = await scan.helpers.resolve_event(
-        resolved_hosts_event2
-    )
-    assert "8.8.8.8" in [str(x) for x in children1["A"]]
-    assert "8.8.8.8" in [str(x) for x in children2["A"]]
-    assert set(children1.keys()) == set(children2.keys())
```

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_regexes.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,23 +98,25 @@
 
         def mock_record(self, *args, **kwargs):
             return MockRecord(*args, **kwargs)
 
     @pytest_asyncio.fixture
     async def module_test(self, httpx_mock, bbot_httpserver, bbot_httpserver_ssl, monkeypatch, request):
         module_test = self.ModuleTest(self, httpx_mock, bbot_httpserver, bbot_httpserver_ssl, monkeypatch, request)
+        module_test.log.info(f"Starting {self.name} module test")
         await self.setup_before_prep(module_test)
         await module_test.scan.prep()
         await self.setup_after_prep(module_test)
         module_test.events = [e async for e in module_test.scan.async_start()]
         yield module_test
 
     @pytest.mark.asyncio
     async def test_module_run(self, module_test):
         self.check(module_test, module_test.events)
+        module_test.log.info(f"Finished {self.name} module test")
 
     def check(self, module_test, events):
         assert False, f"Must override {self.name}.check()"
 
     @property
     def name(self):
         if self.module_name is not None:
```

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.0.2083rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/testsslcert.pem` & `bbot-1.1.0.2083rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/test/testsslkey.pem` & `bbot-1.1.0.2083rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.0.2083rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.0.2083rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.0.2083rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.0.2083rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.0.2083rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.0.2083rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.2043rc0/pyproject.toml` & `bbot-1.1.0.2083rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.0.2043rc"
+version = "v1.1.0.2083rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
 
@@ -28,15 +28,15 @@
 tabulate = "0.8.10"
 cloudcheck = "^2.0.0.34"
 websockets = "^11.0.2"
 pyjwt = "^2.7.0"
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.2"
 httpx = {extras = ["http2"], version = "^0.24.1"}
-anyio = "4.0.0rc1"
+anyio = "==4.0.0rc1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 flake8 = "^6.0.0"
 black = "^23.1.0"
 pytest-cov = "^4.0.0"
 poetry-dynamic-versioning = "^0.21.4"
```

### Comparing `bbot-1.1.0.2043rc0/PKG-INFO` & `bbot-1.1.0.2083rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.0.2043rc0
+Version: 1.1.0.2083rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -118,18 +118,19 @@
 ```
 <!-- END BBOT EXAMPLE COMMANDS -->
 
 ## Targets
 
 BBOT accepts an unlimited number of targets. You can specify targets either directly on the command line or in files (or both!). Targets can be any of the following:
 
-- DNS_NAME (`evilcorp.com`)
-- IP_ADDRESS (`1.2.3.4`)
-- IP_RANGE (`1.2.3.0/24`)
-- URL (`https://www.evilcorp.com`)
+- `DNS_NAME` (`evilcorp.com`)
+- `IP_ADDRESS` (`1.2.3.4`)
+- `IP_RANGE` (`1.2.3.0/24`)
+- `OPEN_TCP_PORT` (`192.168.0.1:80`)
+- `URL` (`https://www.evilcorp.com`)
 
 For more information, see [Targets](https://www.blacklanternsecurity.com/bbot/scanning/#targets-t). To learn how BBOT handles scope, see [Scope](https://www.blacklanternsecurity.com/bbot/scanning/#scope).
 
 ## BBOT as a Python library
 
 **Synchronous**
```

