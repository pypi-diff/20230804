# Comparing `tmp/wordops-3.9.9.2.tar.gz` & `tmp/wordops-3.9.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wordops-3.9.9.2.tar", last modified: Fri Oct  4 22:47:33 2019, max compression
+gzip compressed data, was "dist/wordops-3.9.9.4.tar", last modified: Fri Oct 18 20:01:14 2019, max compression
```

## Comparing `wordops-3.9.9.2.tar` & `wordops-3.9.9.4.tar`

### file list

```diff
@@ -1,170 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/
--rw-r--r--   0 runner    (1001) docker     (115)    13211 2019-10-04 22:47:33.000000 wordops-3.9.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)    11053 2019-10-04 22:47:20.000000 wordops-3.9.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/config/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/config/bash_completion.d/
--rw-r--r--   0 runner    (1001) docker     (115)    16684 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/bash_completion.d/wo_auto.rc
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/config/plugins.d/
--rw-r--r--   0 runner    (1001) docker     (115)      240 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/clean.conf
--rw-r--r--   0 runner    (1001) docker     (115)      240 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/debug.conf
--rw-r--r--   0 runner    (1001) docker     (115)      250 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/import_slow_log.conf
--rw-r--r--   0 runner    (1001) docker     (115)      295 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/info.conf
--rw-r--r--   0 runner    (1001) docker     (115)      238 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/log.conf
--rw-r--r--   0 runner    (1001) docker     (115)      246 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/maintenance.conf
--rw-r--r--   0 runner    (1001) docker     (115)      241 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/secure.conf
--rw-r--r--   0 runner    (1001) docker     (115)      239 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/site.conf
--rw-r--r--   0 runner    (1001) docker     (115)      240 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/stack.conf
--rw-r--r--   0 runner    (1001) docker     (115)      241 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/plugins.d/update.conf
--rw-r--r--   0 runner    (1001) docker     (115)     1878 2019-10-04 22:47:20.000000 wordops-3.9.9.2/config/wo.conf
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (115)     8617 2019-10-04 22:47:20.000000 wordops-3.9.9.2/docs/wo.8
--rw-r--r--   0 runner    (1001) docker     (115)      232 2019-10-04 22:47:33.000000 wordops-3.9.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     2503 2019-10-04 22:47:20.000000 wordops-3.9.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (115)     2106 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/13_test_stack.py
--rw-r--r--   0 runner    (1001) docker     (115)      978 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/2_test_stack_services_start.py
--rw-r--r--   0 runner    (1001) docker     (115)      986 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/3_test_stack_services_status.py
--rw-r--r--   0 runner    (1001) docker     (115)      970 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/4_test_stack_services_stop.py
--rw-r--r--   0 runner    (1001) docker     (115)      994 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/5_test_stack_services_restart.py
--rw-r--r--   0 runner    (1001) docker     (115)     2136 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/8_test_site_create.py
--rw-r--r--   0 runner    (1001) docker     (115)      388 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/91_test_site_info.py
--rw-r--r--   0 runner    (1001) docker     (115)      580 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/93_test_site_list.py
--rw-r--r--   0 runner    (1001) docker     (115)      388 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/95_test_site_show.py
--rw-r--r--   0 runner    (1001) docker     (115)     2135 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/97_test_site_update.py
--rw-r--r--   0 runner    (1001) docker     (115)      392 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/9_test_site_enable.py
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      394 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/a_test_site_disable.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/tests/cli/ext/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/tests/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      219 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/plugins/test_example.py
--rw-r--r--   0 runner    (1001) docker     (115)      882 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (115)     2848 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (115)      712 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/test_info.py
--rw-r--r--   0 runner    (1001) docker     (115)      763 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/test_secure.py
--rw-r--r--   0 runner    (1001) docker     (115)     1203 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/test_site_delete.py
--rw-r--r--   0 runner    (1001) docker     (115)     2287 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/test_stack_purge.py
--rw-r--r--   0 runner    (1001) docker     (115)     2072 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/cli/test_stack_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/
--rw-r--r--   0 runner    (1001) docker     (115)       56 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/cli/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      303 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/cli/controllers/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      641 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/controllers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/cli/ext/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      810 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/ext/wo_outputhandler.py
--rw-r--r--   0 runner    (1001) docker     (115)     3735 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3291 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/clean.py
--rw-r--r--   0 runner    (1001) docker     (115)    41997 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/debug.py
--rw-r--r--   0 runner    (1001) docker     (115)      998 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/import_slow_log.py
--rw-r--r--   0 runner    (1001) docker     (115)    14650 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/info.py
--rw-r--r--   0 runner    (1001) docker     (115)    26420 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/log.py
--rw-r--r--   0 runner    (1001) docker     (115)     1444 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (115)     1990 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/models.py
--rw-r--r--   0 runner    (1001) docker     (115)    10772 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/secure.py
--rw-r--r--   0 runner    (1001) docker     (115)    95723 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/site.py
--rw-r--r--   0 runner    (1001) docker     (115)    71365 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/site_functions.py
--rw-r--r--   0 runner    (1001) docker     (115)     3829 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/sitedb.py
--rw-r--r--   0 runner    (1001) docker     (115)    46902 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/stack.py
--rw-r--r--   0 runner    (1001) docker     (115)     4979 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/stack_migrate.py
--rw-r--r--   0 runner    (1001) docker     (115)    66541 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/stack_pref.py
--rw-r--r--   0 runner    (1001) docker     (115)    16062 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/stack_services.py
--rw-r--r--   0 runner    (1001) docker     (115)    13839 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/stack_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (115)     4432 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/sync.py
--rw-r--r--   0 runner    (1001) docker     (115)     2900 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/plugins/update.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (115)     1594 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/22222.mustache
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      216 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/acl.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     8227 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/anemometer.mustache
--rw-r--r--   0 runner    (1001) docker     (115)       35 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/blockips.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      866 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/brotli.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      970 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/cf-update.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      785 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/cloudflare.mustache
--rw-r--r--   0 runner    (1001) docker     (115)       97 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/fail2ban-forbidden.mustache
--rw-r--r--   0 runner    (1001) docker     (115)       97 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/fail2ban-wp.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      471 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/fail2ban.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      814 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/fastcgi.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      280 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/freshclam.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      919 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/gzip.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      389 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/info_mysql.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      389 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/info_nginx.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     1673 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/info_php.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     2788 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/locations.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     2171 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/map-wp.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     5289 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/mime.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     5474 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/my.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     3112 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/nextcloud.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     2830 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/nginx-core.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      185 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/php-fpm.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      555 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/php-pool.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      272 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/php.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      466 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/proftpd-tls.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     1132 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/redis.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      595 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/siteinfo.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     2087 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/sshd.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      734 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/stub_status.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     7965 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/sysctl.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      586 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/tweaks.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     1595 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/ufw.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     1614 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/upstream.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     1931 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/virtualconf-php7.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     1930 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/virtualconf.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      180 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/webp.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      297 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wo-kernel-script.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      325 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wo-kernel-service.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     1671 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wo-plus.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      120 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wo-ufw.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      661 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wpce.mustache
--rw-r--r--   0 runner    (1001) docker     (115)     3103 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wpcommon.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      670 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wpfc.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      763 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wprocket.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      635 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wpsc.mustache
--rw-r--r--   0 runner    (1001) docker     (115)      366 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/cli/templates/wpsubdir.mustache
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/core/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     6759 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/acme.py
--rw-r--r--   0 runner    (1001) docker     (115)     2168 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/addswap.py
--rw-r--r--   0 runner    (1001) docker     (115)     4272 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/apt_repo.py
--rw-r--r--   0 runner    (1001) docker     (115)    10984 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/aptget.py
--rw-r--r--   0 runner    (1001) docker     (115)     1201 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/checkfqdn.py
--rw-r--r--   0 runner    (1001) docker     (115)     2053 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/cron.py
--rw-r--r--   0 runner    (1001) docker     (115)     1092 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/database.py
--rw-r--r--   0 runner    (1001) docker     (115)     1902 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/domainvalidate.py
--rw-r--r--   0 runner    (1001) docker     (115)     1992 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/download.py
--rw-r--r--   0 runner    (1001) docker     (115)      449 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/exc.py
--rw-r--r--   0 runner    (1001) docker     (115)      578 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/extract.py
--rw-r--r--   0 runner    (1001) docker     (115)    12778 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (115)     3311 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/git.py
--rw-r--r--   0 runner    (1001) docker     (115)     2654 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (115)     6105 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/logwatch.py
--rw-r--r--   0 runner    (1001) docker     (115)     5245 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/mysql.py
--rw-r--r--   0 runner    (1001) docker     (115)     1832 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/nginxhashbucket.py
--rw-r--r--   0 runner    (1001) docker     (115)      314 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/random.py
--rw-r--r--   0 runner    (1001) docker     (115)     1011 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/sendmail.py
--rw-r--r--   0 runner    (1001) docker     (115)     7940 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/services.py
--rw-r--r--   0 runner    (1001) docker     (115)     3194 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/shellexec.py
--rw-r--r--   0 runner    (1001) docker     (115)     7682 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/sslutils.py
--rw-r--r--   0 runner    (1001) docker     (115)     1670 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/template.py
--rw-r--r--   0 runner    (1001) docker     (115)     7101 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/core/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wo/utils/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      407 2019-10-04 22:47:20.000000 wordops-3.9.9.2/wo/utils/test.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)    13211 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     4267 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       67 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (115)      190 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)        9 2019-10-04 22:47:33.000000 wordops-3.9.9.2/wordops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/
+-rw-r--r--   0 runner    (1001) docker     (115)     1221 2019-10-18 20:01:00.000000 wordops-3.9.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)    13211 2019-10-18 20:01:14.000000 wordops-3.9.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)    11053 2019-10-18 20:01:00.000000 wordops-3.9.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/config/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/config/bash_completion.d/
+-rw-r--r--   0 runner    (1001) docker     (115)    16684 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/bash_completion.d/wo_auto.rc
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/config/plugins.d/
+-rw-r--r--   0 runner    (1001) docker     (115)      240 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/clean.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      240 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/debug.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      250 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/import_slow_log.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      295 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/info.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      238 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/log.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      246 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/maintenance.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      241 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/secure.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      239 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/site.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      240 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/stack.conf
+-rw-r--r--   0 runner    (1001) docker     (115)      241 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/plugins.d/update.conf
+-rw-r--r--   0 runner    (1001) docker     (115)     1878 2019-10-18 20:01:00.000000 wordops-3.9.9.4/config/wo.conf
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (115)     8617 2019-10-18 20:01:00.000000 wordops-3.9.9.4/docs/wo.8
+-rw-r--r--   0 runner    (1001) docker     (115)      267 2019-10-18 20:01:14.000000 wordops-3.9.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     2582 2019-10-18 20:01:00.000000 wordops-3.9.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (115)     2106 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/13_test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (115)      978 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/2_test_stack_services_start.py
+-rw-r--r--   0 runner    (1001) docker     (115)      986 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/3_test_stack_services_status.py
+-rw-r--r--   0 runner    (1001) docker     (115)      970 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/4_test_stack_services_stop.py
+-rw-r--r--   0 runner    (1001) docker     (115)      994 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/5_test_stack_services_restart.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2136 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/8_test_site_create.py
+-rw-r--r--   0 runner    (1001) docker     (115)      388 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/91_test_site_info.py
+-rw-r--r--   0 runner    (1001) docker     (115)      580 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/93_test_site_list.py
+-rw-r--r--   0 runner    (1001) docker     (115)      388 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/95_test_site_show.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2135 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/97_test_site_update.py
+-rw-r--r--   0 runner    (1001) docker     (115)      392 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/9_test_site_enable.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      394 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/a_test_site_disable.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/tests/cli/ext/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/tests/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      219 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/plugins/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (115)      882 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2848 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (115)      712 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (115)      763 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/test_secure.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1203 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/test_site_delete.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2287 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/test_stack_purge.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2072 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/cli/test_stack_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/
+-rw-r--r--   0 runner    (1001) docker     (115)       56 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/cli/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      271 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/cli/controllers/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      641 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/controllers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/cli/ext/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      810 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/ext/wo_outputhandler.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3735 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3253 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/clean.py
+-rw-r--r--   0 runner    (1001) docker     (115)    41959 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/debug.py
+-rw-r--r--   0 runner    (1001) docker     (115)      960 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/import_slow_log.py
+-rw-r--r--   0 runner    (1001) docker     (115)    14764 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/info.py
+-rw-r--r--   0 runner    (1001) docker     (115)    26382 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/log.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1406 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1990 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/models.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11024 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/secure.py
+-rw-r--r--   0 runner    (1001) docker     (115)    95685 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/site.py
+-rw-r--r--   0 runner    (1001) docker     (115)    70901 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/site_functions.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3829 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/sitedb.py
+-rw-r--r--   0 runner    (1001) docker     (115)    46962 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/stack.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4979 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/stack_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (115)    66499 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/stack_pref.py
+-rw-r--r--   0 runner    (1001) docker     (115)    16024 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/stack_services.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13282 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/stack_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4394 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/sync.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2862 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/plugins/update.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (115)     1594 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/22222.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      216 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/acl.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     8227 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/anemometer.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)       35 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/blockips.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      866 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/brotli.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      970 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/cf-update.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      785 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/cloudflare.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)       97 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/fail2ban-forbidden.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)       97 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/fail2ban-wp.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      471 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/fail2ban.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      814 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/fastcgi.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      280 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/freshclam.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      919 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/gzip.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      389 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/info_mysql.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      389 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/info_nginx.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     1673 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/info_php.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     2788 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/locations.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     2171 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/map-wp.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     5289 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/mime.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     5474 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/my.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     3112 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/nextcloud.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     2853 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/nginx-core.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      185 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/php-fpm.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      577 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/php-pool.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      272 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/php.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      466 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/proftpd-tls.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     1132 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/redis.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      595 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/siteinfo.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     2087 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/sshd.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      734 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/stub_status.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     7965 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/sysctl.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      695 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/tweaks.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     1595 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/ufw.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     1528 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/upstream.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     1931 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/virtualconf-php7.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     1930 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/virtualconf.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      180 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/webp.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      297 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wo-kernel-script.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      325 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wo-kernel-service.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     1671 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wo-plus.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      120 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wo-ufw.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      661 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wpce.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)     3103 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wpcommon.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      670 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wpfc.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      763 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wprocket.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      635 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wpsc.mustache
+-rw-r--r--   0 runner    (1001) docker     (115)      366 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/cli/templates/wpsubdir.mustache
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/core/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6786 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/acme.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2168 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/addswap.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4333 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/apt_repo.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10566 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/aptget.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1201 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/checkfqdn.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2053 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/cron.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1092 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1876 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/domainvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1992 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/download.py
+-rw-r--r--   0 runner    (1001) docker     (115)      449 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/exc.py
+-rw-r--r--   0 runner    (1001) docker     (115)      578 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/extract.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12778 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3311 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/git.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2654 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6105 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/logwatch.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5245 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1832 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/nginxhashbucket.py
+-rw-r--r--   0 runner    (1001) docker     (115)      514 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1011 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/sendmail.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7940 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/services.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3290 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/shellexec.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7682 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/sslutils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1668 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7027 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/core/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wo/utils/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      407 2019-10-18 20:01:00.000000 wordops-3.9.9.4/wo/utils/test.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)    13211 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     4275 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       67 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (115)      166 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        9 2019-10-18 20:01:14.000000 wordops-3.9.9.4/wordops.egg-info/top_level.txt
```

### Comparing `wordops-3.9.9.2/PKG-INFO` & `wordops-3.9.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordops
-Version: 3.9.9.2
+Version: 3.9.9.4
 Summary: WordPress & server administration toolset
 Home-page: https://github.com/WordOps/WordOps
 Author: WordOps
 Author-email: contact@wordops.io
 License: MIT
 Description: <p align="center"><img src="https://raw.githubusercontent.com/WordOps/WordOps/master/logo.png" width="400" alt="Wordops" /><a href="https://wordops.net">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wordops Version: 3.9.9.2 Summary: WordPress &
+Metadata-Version: 2.1 Name: wordops Version: 3.9.9.4 Summary: WordPress &
 server administration toolset Home-page: https://github.com/WordOps/WordOps
 Author: WordOps Author-email: contact@wordops.io License: MIT Description:
                                    [Wordops]
 ***** An essential toolset that eases WordPress site and server administration
                                      *****
                                    [WordOps]
                    [build] [MIT] [Commits] [GitHub release]
```

### Comparing `wordops-3.9.9.2/README.md` & `wordops-3.9.9.4/README.md`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/config/bash_completion.d/wo_auto.rc` & `wordops-3.9.9.4/config/bash_completion.d/wo_auto.rc`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/config/wo.conf` & `wordops-3.9.9.4/config/wo.conf`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/docs/wo.8` & `wordops-3.9.9.4/docs/wo.8`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/setup.py` & `wordops-3.9.9.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 
 import glob
 import os
 
 from setuptools import find_packages, setup
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+
+# read the contents of your README file
+this_directory = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    LONG = f.read()
 
 conf = []
 templates = []
 
 for name in glob.glob('config/plugins.d/*.conf'):
     conf.insert(1, name)
 
@@ -20,17 +23,17 @@
     if not os.path.exists('/var/log/wo/'):
         os.makedirs('/var/log/wo/')
 
     if not os.path.exists('/var/lib/wo/tmp/'):
         os.makedirs('/var/lib/wo/tmp/')
 
 setup(name='wordops',
-      version='3.9.9.2',
+      version='3.9.9.4',
       description='WordPress & server administration toolset',
-      long_description=long_description,
+      long_description=LONG,
       long_description_content_type='text/markdown',
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
           "Development Status :: 5 - Production/Stable",
           "Environment :: Console",
@@ -57,15 +60,14 @@
           'pynginxconfig >= 0.3.4',
           'PyMySQL >= 0.9.3',
           'psutil >= 5.6.3',
           'sh >= 1.12.14',
           'SQLAlchemy >= 1.3.8',
           'requests >= 2.22.0',
           'distro >= 1.4.0',
-          'apt-mirror-updater >= 6.1',
       ],
       extras_require={  # Optional
           'testing': ['nose', 'coverage'],
       },
       data_files=[('/etc/wo', ['config/wo.conf']),
                   ('/etc/wo/plugins.d', conf),
                   ('/usr/lib/wo/templates', templates),
```

### Comparing `wordops-3.9.9.2/tests/cli/13_test_stack.py` & `wordops-3.9.9.4/tests/cli/13_test_stack.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/2_test_stack_services_start.py` & `wordops-3.9.9.4/tests/cli/2_test_stack_services_start.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/3_test_stack_services_status.py` & `wordops-3.9.9.4/tests/cli/3_test_stack_services_status.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/4_test_stack_services_stop.py` & `wordops-3.9.9.4/tests/cli/4_test_stack_services_stop.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/5_test_stack_services_restart.py` & `wordops-3.9.9.4/tests/cli/5_test_stack_services_restart.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/8_test_site_create.py` & `wordops-3.9.9.4/tests/cli/8_test_site_create.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/93_test_site_list.py` & `wordops-3.9.9.4/tests/cli/93_test_site_list.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/97_test_site_update.py` & `wordops-3.9.9.4/tests/cli/97_test_site_update.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/test_clean.py` & `wordops-3.9.9.4/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/test_debug.py` & `wordops-3.9.9.4/tests/cli/test_debug.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/test_info.py` & `wordops-3.9.9.4/tests/cli/test_info.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/test_secure.py` & `wordops-3.9.9.4/tests/cli/test_secure.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/test_site_delete.py` & `wordops-3.9.9.4/tests/cli/test_site_delete.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/test_stack_purge.py` & `wordops-3.9.9.4/tests/cli/test_stack_purge.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/tests/cli/test_stack_remove.py` & `wordops-3.9.9.4/tests/cli/test_stack_remove.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/controllers/base.py` & `wordops-3.9.9.4/wo/cli/controllers/base.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/ext/wo_outputhandler.py` & `wordops-3.9.9.4/wo/cli/ext/wo_outputhandler.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/main.py` & `wordops-3.9.9.4/wo/cli/main.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/plugins/clean.py` & `wordops-3.9.9.4/wo/cli/plugins/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Clean Plugin for WordOps."""
 
 import os
 import urllib.request
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.core.aptget import WOAptGet
 from wo.core.logging import Log
 from wo.core.services import WOService
 from wo.core.shellexec import WOShellExec
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/debug.py` & `wordops-3.9.9.4/wo/cli/plugins/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Debug Plugin for WordOps"""
 
 import configparser
 import glob
 import os
 import signal
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 from pynginxconfig import NginxConfig
 
 from wo.cli.plugins.site_functions import logwatch
 from wo.core.aptget import WOAptGet
 from wo.core.fileutils import WOFileUtils
 from wo.core.logging import Log
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/import_slow_log.py` & `wordops-3.9.9.4/wo/cli/plugins/import_slow_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.core.logging import Log
 
 
 def wo_import_slow_log_hook(app):
     pass
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/info.py` & `wordops-3.9.9.4/wo/cli/plugins/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """WOInfo Plugin for WordOps"""
 
 import configparser
 import os
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 from pynginxconfig import NginxConfig
 
 from wo.core.aptget import WOAptGet
 from wo.core.logging import Log
 from wo.core.shellexec import WOShellExec
 
@@ -76,28 +75,28 @@
         expose_php = config['PHP']['expose_php']
         memory_limit = config['PHP']['memory_limit']
         post_max_size = config['PHP']['post_max_size']
         upload_max_filesize = config['PHP']['upload_max_filesize']
         max_execution_time = config['PHP']['max_execution_time']
 
         config.read('/etc/{0}/fpm/pool.d/www.conf'.format("php/7.2"))
-        www_listen = config['www']['listen']
-        www_ping_path = config['www']['ping.path']
-        www_pm_status_path = config['www']['pm.status_path']
-        www_pm = config['www']['pm']
-        www_pm_max_requests = config['www']['pm.max_requests']
-        www_pm_max_children = config['www']['pm.max_children']
-        www_pm_start_servers = config['www']['pm.start_servers']
-        www_pm_min_spare_servers = config['www']['pm.min_spare_servers']
-        www_pm_max_spare_servers = config['www']['pm.max_spare_servers']
-        www_request_terminate_time = (config['www']
+        www_listen = config['www-php72']['listen']
+        www_ping_path = config['www-php72']['ping.path']
+        www_pm_status_path = config['www-php72']['pm.status_path']
+        www_pm = config['www-php72']['pm']
+        www_pm_max_requests = config['www-php72']['pm.max_requests']
+        www_pm_max_children = config['www-php72']['pm.max_children']
+        www_pm_start_servers = config['www-php72']['pm.start_servers']
+        www_pm_min_spare_servers = config['www-php72']['pm.min_spare_servers']
+        www_pm_max_spare_servers = config['www-php72']['pm.max_spare_servers']
+        www_request_terminate_time = (config['www-php72']
                                             ['request_terminate_timeout'])
         try:
-            www_xdebug = (config['www']['php_admin_flag[xdebug.profiler_enable'
-                                        '_trigger]'])
+            www_xdebug = (config['www-php72']['php_admin_flag[xdebug.profiler_enable'
+                                              '_trigger]'])
         except Exception as e:
             Log.debug(self, "{0}".format(e))
             www_xdebug = 'off'
 
         config.read('/etc/{0}/fpm/pool.d/debug.conf'.format("php/7.2"))
         debug_listen = config['debug']['listen']
         debug_ping_path = config['debug']['ping.path']
@@ -153,28 +152,29 @@
         expose_php = config['PHP']['expose_php']
         memory_limit = config['PHP']['memory_limit']
         post_max_size = config['PHP']['post_max_size']
         upload_max_filesize = config['PHP']['upload_max_filesize']
         max_execution_time = config['PHP']['max_execution_time']
 
         config.read('/etc/php/7.3/fpm/pool.d/www.conf')
-        www_listen = config['www']['listen']
-        www_ping_path = config['www']['ping.path']
-        www_pm_status_path = config['www']['pm.status_path']
-        www_pm = config['www']['pm']
-        www_pm_max_requests = config['www']['pm.max_requests']
-        www_pm_max_children = config['www']['pm.max_children']
-        www_pm_start_servers = config['www']['pm.start_servers']
-        www_pm_min_spare_servers = config['www']['pm.min_spare_servers']
-        www_pm_max_spare_servers = config['www']['pm.max_spare_servers']
-        www_request_terminate_time = (config['www']
+        www_listen = config['www-php73']['listen']
+        www_ping_path = config['www-php73']['ping.path']
+        www_pm_status_path = config['www-php73']['pm.status_path']
+        www_pm = config['www-php73']['pm']
+        www_pm_max_requests = config['www-php73']['pm.max_requests']
+        www_pm_max_children = config['www-php73']['pm.max_children']
+        www_pm_start_servers = config['www-php73']['pm.start_servers']
+        www_pm_min_spare_servers = config['www-php73']['pm.min_spare_servers']
+        www_pm_max_spare_servers = config['www-php73']['pm.max_spare_servers']
+        www_request_terminate_time = (config['www-php73']
                                             ['request_terminate_timeout'])
         try:
-            www_xdebug = (config['www']['php_admin_flag[xdebug.profiler_enable'
-                                        '_trigger]'])
+            www_xdebug = (config['www-php73']
+                          ['php_admin_flag[xdebug.profiler_enable'
+                           '_trigger]'])
         except Exception as e:
             Log.debug(self, "{0}".format(e))
             www_xdebug = 'off'
 
         config.read('/etc/php/7.3/fpm/pool.d/debug.conf')
         debug_listen = config['debug']['listen']
         debug_ping_path = config['debug']['ping.path']
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/log.py` & `wordops-3.9.9.4/wo/cli/plugins/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Logfile Plugin for WordOps"""
 
 import glob
 import gzip
 import os
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.cli.plugins.site_functions import logwatch
 from wo.core.fileutils import WOFileUtils
 from wo.core.logging import Log
 from wo.core.mysql import WOMysql
 from wo.core.sendmail import WOSendMail
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/maintenance.py` & `wordops-3.9.9.4/wo/cli/plugins/maintenance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Maintenance Plugin for WordOps"""
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.core.aptget import WOAptGet
 from wo.core.logging import Log
 
 
 def wo_maintenance_hook(app):
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/models.py` & `wordops-3.9.9.4/wo/cli/plugins/models.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/plugins/secure.py` & `wordops-3.9.9.4/wo/cli/plugins/secure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import getpass
 import os
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.core.fileutils import WOFileUtils
 from wo.core.git import WOGit
 from wo.core.logging import Log
 from wo.core.random import RANDOM
 from wo.core.services import WOService
@@ -66,15 +65,15 @@
 
     @expose(hide=True)
     def secure_auth(self):
         """This function secures authentication"""
         WOGit.add(self, ["/etc/nginx"],
                   msg="Add Nginx to into Git")
         pargs = self.app.pargs
-        passwd = RANDOM.gen(self, length='24')
+        passwd = RANDOM.long(self)
         if not pargs.user_input:
             username = input("Provide HTTP authentication user "
                              "name [{0}] :".format(WOVar.wo_user))
             pargs.user_input = username
             if username == "":
                 pargs.user_input = WOVar.wo_user
         if not pargs.user_pass:
@@ -105,19 +104,20 @@
         pargs = self.app.pargs
         if pargs.user_input:
             while ((not pargs.user_input.isdigit()) and
                    (not pargs.user_input < 65536)):
                 Log.info(self, "Please enter a valid port number ")
                 pargs.user_input = input("WordOps "
                                          "admin port [22222]:")
-        if not pargs.user_input:
+        else:
             port = input("WordOps admin port [22222]:")
             if port == "":
                 port = 22222
-            while (not port.isdigit()) and (port != "") and (not port < 65536):
+            while ((not port.isdigit()) and (not port != "") and
+                   (not port < 65536)):
                 Log.info(self, "Please Enter valid port number :")
                 port = input("WordOps admin port [22222]:")
             pargs.user_input = port
         WOShellExec.cmd_exec(self, "sed -i \"s/listen.*/listen "
                              "{port} default_server ssl http2;/\" "
                              "/etc/nginx/sites-available/22222"
                              .format(port=pargs.user_input))
@@ -216,17 +216,22 @@
             port = input("Server SSH port [22]:")
             if port == "":
                 port = 22
             while (not port.isdigit()) and (port != "") and (not port < 65536):
                 Log.info(self, "Please Enter valid port number :")
                 port = input("Server SSH port [22]:")
             pargs.user_input = port
-        WOShellExec.cmd_exec(self, "sed -i \"s/Port.*/Port "
-                             "{port}/\" /etc/ssh/sshd_config"
-                             .format(port=pargs.user_input))
+        if WOFileUtils.grepcheck(self, '/etc/ssh/sshd_config', '#Port'):
+            WOShellExec.cmd_exec(self, "sed -i \"s/#Port.*/Port "
+                                 "{port}/\" /etc/ssh/sshd_config"
+                                 .format(port=pargs.user_input))
+        else:
+            WOShellExec.cmd_exec(self, "sed -i \"s/Port.*/Port "
+                                 "{port}/\" /etc/ssh/sshd_config"
+                                 .format(port=pargs.user_input))
         # allow new ssh port if ufw is enabled
         if os.path.isfile('/etc/ufw/ufw.conf'):
             # add rule for proftpd with UFW
             if WOFileUtils.grepcheck(
                     self, '/etc/ufw/ufw.conf', 'ENABLED=yes'):
                 try:
                     WOShellExec.cmd_exec(
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/site.py` & `wordops-3.9.9.4/wo/cli/plugins/site.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import glob
 import json
 import os
 import subprocess
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 from wo.cli.plugins.site_functions import *
 from wo.cli.plugins.sitedb import (addNewSite, deleteSiteInfo, getAllsites,
                                    getSiteInfo, updateSiteInfo)
 from wo.core.acme import WOAcme
 from wo.core.domainvalidate import WODomain
 from wo.core.fileutils import WOFileUtils
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/site_functions.py` & `wordops-3.9.9.4/wo/cli/plugins/site_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,18 +297,17 @@
         Log.debug(self, "/bin/bash -c \"{0} --allow-root "
                   .format(WOVar.wo_wpcli_path) +
                   "config create " +
                   "--dbname=\'{0}\' --dbprefix=\'{1}\' --dbuser=\'{2}\' "
                   "--dbhost=\'{3}\' "
                   .format(data['wo_db_name'], wo_wp_prefix,
                           data['wo_db_user'], data['wo_db_host']) +
-                  "--dbpass=\'{0}\' "
-                  "--extra-php<<PHP \n {1}\nPHP\""
-                  .format(data['wo_db_pass'],
-                          "\n\ndefine(\'WP_DEBUG\', false);"))
+                  "--dbpass= "
+                  "--extra-php<<PHP \n {0}\nPHP\""
+                  .format("\n\ndefine(\'WP_DEBUG\', false);"))
         try:
             if WOShellExec.cmd_exec(self, "/bin/bash -c \"{0} --allow-root"
                                     .format(WOVar.wo_wpcli_path) +
                                     " config create " +
                                     "--dbname=\'{0}\' --dbprefix=\'{1}\' "
                                     "--dbuser=\'{2}\' --dbhost=\'{3}\' "
                                     .format(data['wo_db_name'], wo_wp_prefix,
@@ -331,17 +330,17 @@
         Log.debug(self, "Generating wp-config for WordPress multisite")
         Log.debug(self, "/bin/bash -c \"{0} --allow-root "
                   .format(WOVar.wo_wpcli_path) +
                   "config create " +
                   "--dbname=\'{0}\' --dbprefix=\'{1}\' --dbhost=\'{2}\' "
                   .format(data['wo_db_name'],
                           wo_wp_prefix, data['wo_db_host']) +
-                  "--dbuser=\'{0}\' --dbpass=\'{1}\' "
-                  "--extra-php<<PHP \n {2} {3} {4} \nPHP\""
-                  .format(data['wo_db_user'], data['wo_db_pass'],
+                  "--dbuser=\'{0}\' --dbpass= "
+                  "--extra-php<<PHP \n {1} {2} {3} \nPHP\""
+                  .format(data['wo_db_user'],
                           "\ndefine(\'WPMU_ACCEL_REDIRECT\',"
                           " true);",
                           "\ndefine(\'CONCATENATE_SCRIPTS\',"
                           " false);",
                           "\n\ndefine(\'WP_DEBUG\', false);"))
         try:
             if WOShellExec.cmd_exec(self, "/bin/bash -c \"{0} --allow-root"
@@ -458,59 +457,61 @@
     Log.debug(self, "Setting up WordPress tables")
 
     if not data['multisite']:
         Log.debug(self, "Creating tables for WordPress Single site")
         Log.debug(self, "{0} --allow-root core install "
                   .format(WOVar.wo_wpcli_path) +
                   "--url=\'{0}\' --title=\'{0}\' --admin_name=\'{1}\' "
-                  .format(data['www_domain'], wo_wp_user) +
-                  "--admin_password= --admin_email=\'{1}\'"
-                  .format(wo_wp_pass, wo_wp_email))
-        try:
-            if WOShellExec.cmd_exec(self, "{0} --allow-root core "
-                                    .format(WOVar.wo_wpcli_path) +
-                                    "install --url=\'{0}\' --title=\'{0}\' "
-                                    "--admin_name=\'{1}\' "
-                                    .format(data['www_domain'], wo_wp_user) +
-                                    "--admin_password=\'{0}\' "
-                                    "--admin_email=\'{1}\'"
-                                    .format(wo_wp_pass, wo_wp_email),
-                                    log=False):
+                  .format(data['site_name'], wo_wp_user) +
+                  "--admin_password= --admin_email=\'{0}\'"
+                  .format(wo_wp_email))
+        try:
+            if WOShellExec.cmd_exec(
+                self, "{0} --allow-root core "
+                .format(WOVar.wo_wpcli_path) +
+                "install --url=\'{0}\' --title=\'{0}\' "
+                "--admin_name=\'{1}\' "
+                .format(data['site_name'], wo_wp_user) +
+                "--admin_password=\'{0}\' "
+                "--admin_email=\'{1}\'"
+                .format(wo_wp_pass, wo_wp_email),
+                    log=False):
                 pass
             else:
                 raise SiteError(
                     "setup WordPress tables failed for single site")
         except CommandExecutionError:
             raise SiteError("setup WordPress tables failed for single site")
     else:
         Log.debug(self, "Creating tables for WordPress multisite")
         Log.debug(self, "{0} --allow-root "
                   .format(WOVar.wo_wpcli_path) +
                   "core multisite-install "
                   "--url=\'{0}\' --title=\'{0}\' --admin_name=\'{1}\' "
-                  .format(data['www_domain'], wo_wp_user) +
-                  "--admin_password= --admin_email=\'{1}\' "
+                  .format(data['site_name'], wo_wp_user) +
+                  "--admin_password= --admin_email=\'{0}\' "
                   "{subdomains}"
-                  .format(wo_wp_pass, wo_wp_email,
+                  .format(wo_wp_email,
                           subdomains='--subdomains'
                           if not data['wpsubdir'] else ''))
         try:
-            if WOShellExec.cmd_exec(self, "{0} --allow-root "
-                                    .format(WOVar.wo_wpcli_path) +
-                                    "core multisite-install "
-                                    "--url=\'{0}\' --title=\'{0}\' "
-                                    "--admin_name=\'{1}\' "
-                                    .format(data['www_domain'], wo_wp_user) +
-                                    "--admin_password=\'{0}\' "
-                                    "--admin_email=\'{1}\' "
-                                    "{subdomains}"
-                                    .format(wo_wp_pass, wo_wp_email,
-                                            subdomains='--subdomains'
-                                            if not data['wpsubdir'] else ''),
-                                    log=False):
+            if WOShellExec.cmd_exec(
+                self, "{0} --allow-root "
+                .format(WOVar.wo_wpcli_path) +
+                "core multisite-install "
+                "--url=\'{0}\' --title=\'{0}\' "
+                "--admin_name=\'{1}\' "
+                .format(data['site_name'], wo_wp_user) +
+                "--admin_password=\'{0}\' "
+                "--admin_email=\'{1}\' "
+                "{subdomains}"
+                .format(wo_wp_pass, wo_wp_email,
+                        subdomains='--subdomains'
+                        if not data['wpsubdir'] else ''),
+                    log=False):
                 pass
             else:
                 raise SiteError(
                     "setup WordPress tables failed for wp multi site")
         except CommandExecutionError:
             raise SiteError("setup WordPress tables failed for wp multi site")
 
@@ -1049,15 +1050,15 @@
                      "page=cache-enabler".format(data['site_name']))
 
 
 def logwatch(self, logfiles):
     import zlib
     import base64
     import time
-    from wo.core import logwatch
+    from wo.core.logwatch import LogWatcher
 
     def callback(filename, lines):
         for line in lines:
             if line.find(':::') == -1:
                 print(line)
             else:
                 data = line.split(':::')
@@ -1066,15 +1067,15 @@
                           zlib.decompress(base64.decodestring(data[2])))
                 except Exception as e:
                     Log.debug(self, str(e))
                     Log.info(time.time(),
                              'caught exception rendering a new log line in %s'
                              % filename)
 
-    logl = logwatch.LogWatcher(logfiles, callback)
+    logl = LogWatcher(logfiles, callback)
     logl.loop()
 
 
 def detSitePar(opts):
     """
         Takes dictionary of parsed arguments
         1.returns sitetype and cachetype
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/sitedb.py` & `wordops-3.9.9.4/wo/cli/plugins/sitedb.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/plugins/stack.py` & `wordops-3.9.9.4/wo/cli/plugins/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Stack Plugin for WordOps"""
 
 import os
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
-from wo.cli.plugins.site_functions import *
-from wo.cli.plugins.sitedb import *
 from wo.cli.plugins.stack_migrate import WOStackMigrateController
 from wo.cli.plugins.stack_pref import post_pref, pre_pref
 from wo.cli.plugins.stack_services import WOStackStatusController
 from wo.cli.plugins.stack_upgrade import WOStackUpgradeController
 from wo.core.aptget import WOAptGet
 from wo.core.download import WODownload
 from wo.core.fileutils import WOFileUtils
@@ -164,22 +161,22 @@
                             WOAptGet.is_installed(self, 'nginx')):
                         if not os.path.isfile('/usr/sbin/nginx'):
                             apt_packages = apt_packages + WOVar.wo_nginx
                     else:
                         if WOAptGet.is_installed(self, 'nginx-plus'):
                             Log.info(self, "NGINX PLUS Detected ...")
                             apt = ["nginx-plus"] + WOVar.wo_nginx
-                            self.post_pref(apt, empty_packages)
+                            post_pref(self, apt, empty_packages)
                         elif WOAptGet.is_installed(self, 'nginx'):
                             Log.info(self, "WordOps detected an already "
                                      "installed nginx package."
                                      "It may or may not have "
                                      "required modules.\n")
                             apt = ["nginx"] + WOVar.wo_nginx
-                            self.post_pref(apt, empty_packages)
+                            post_pref(self, apt, empty_packages)
                 else:
                     Log.debug(self, "Nginx already installed")
 
             # Redis
             if pargs.redis:
                 if not WOAptGet.is_installed(self, 'redis-server'):
                     apt_packages = apt_packages + WOVar.wo_redis
@@ -339,29 +336,30 @@
 
             # ADMINER
             if pargs.adminer:
                 if not os.path.isfile("{0}22222/htdocs/db/"
                                       "adminer/index.php"
                                       .format(wo_webroot)):
                     Log.debug(self, "Setting packages variable for Adminer ")
-                    packages = packages + [["https://github.com/vrana/adminer/"
-                                            "releases/download/v{0}"
-                                            "/adminer-{0}.php"
-                                            .format(WOVar.wo_adminer),
-                                            "{0}22222/"
-                                            "htdocs/db/adminer/index.php"
-                                            .format(WOVar.wo_webroot),
-                                            "Adminer"],
-                                           ["https://raw.githubusercontent.com"
-                                            "/vrana/adminer/master/designs/"
-                                            "pepa-linha/adminer.css",
-                                            "{0}22222/"
-                                            "htdocs/db/adminer/adminer.css"
-                                            .format(WOVar.wo_webroot),
-                                            "Adminer theme"]]
+                    packages = packages + [[
+                        "https://github.com/vrana/adminer/"
+                        "releases/download/v{0}"
+                        "/adminer-{0}.php"
+                        .format(WOVar.wo_adminer),
+                        "{0}22222/"
+                        "htdocs/db/adminer/index.php"
+                        .format(WOVar.wo_webroot),
+                        "Adminer"],
+                        ["https://raw.githubusercontent.com"
+                         "/vrana/adminer/master/designs/"
+                         "pepa-linha/adminer.css",
+                         "{0}22222/"
+                         "htdocs/db/adminer/adminer.css"
+                         .format(WOVar.wo_webroot),
+                         "Adminer theme"]]
                 else:
                     Log.debug(self, "Adminer already installed")
                     Log.info(self, "Adminer already installed")
 
             # mysqltuner
             if pargs.mysqltuner:
                 if not os.path.isfile("/usr/bin/mysqltuner"):
@@ -398,22 +396,22 @@
                     Log.info(self, "Netdata already installed")
 
             # WordOps Dashboard
             if pargs.dashboard:
                 if not os.path.isfile('/var/www/22222/htdocs/index.php'):
                     Log.debug(self,
                               "Setting packages variable for WO-Dashboard")
-                    packages = \
-                        packages + [["https://github.com/WordOps"
-                                     "/wordops-dashboard/"
-                                     "releases/download/v{0}/"
-                                     "wordops-dashboard.tar.gz"
-                                     .format(WOVar.wo_dashboard),
-                                     "/var/lib/wo/tmp/wo-dashboard.tar.gz",
-                                     "WordOps Dashboard"]]
+                    packages = packages + [[
+                        "https://github.com/WordOps"
+                        "/wordops-dashboard/"
+                        "releases/download/v{0}/"
+                        "wordops-dashboard.tar.gz"
+                        .format(WOVar.wo_dashboard),
+                        "/var/lib/wo/tmp/wo-dashboard.tar.gz",
+                        "WordOps Dashboard"]]
                 else:
                     Log.debug(self, "WordOps dashboard already installed")
                     Log.info(self, "WordOps dashboard already installed")
 
             # eXtplorer
             if pargs.extplorer:
                 if not os.path.isdir('/var/www/22222/htdocs/files'):
@@ -440,51 +438,52 @@
                 else:
                     Log.debug(self, "ngxblocker is already installed")
                     Log.info(self, "ngxblocker is already installed")
 
             # UTILS
             if pargs.utils:
                 Log.debug(self, "Setting packages variable for utils")
-                packages = packages + [["https://raw.githubusercontent.com"
-                                        "/rtCamp/eeadmin/master/cache/nginx/"
-                                        "clean.php",
-                                        "{0}22222/htdocs/cache/"
-                                        "nginx/clean.php"
-                                        .format(WOVar.wo_webroot),
-                                        "clean.php"],
-                                       ["https://raw.github.com/rlerdorf/"
-                                        "opcache-status/master/opcache.php",
-                                        "{0}22222/htdocs/cache/"
-                                        "opcache/opcache.php"
-                                        .format(WOVar.wo_webroot),
-                                        "opcache.php"],
-                                       ["https://raw.github.com/amnuts/"
-                                        "opcache-gui/master/index.php",
-                                        "{0}22222/htdocs/"
-                                        "cache/opcache/opgui.php"
-                                        .format(WOVar.wo_webroot),
-                                        "Opgui"],
-                                       ["https://raw.githubusercontent.com/"
-                                        "mlazarov/ocp/master/ocp.php",
-                                        "{0}22222/htdocs/cache/"
-                                        "opcache/ocp.php"
-                                        .format(WOVar.wo_webroot),
-                                        "OCP.php"],
-                                       ["https://github.com/jokkedk/webgrind/"
-                                        "archive/master.tar.gz",
-                                        '/var/lib/wo/tmp/webgrind.tar.gz',
-                                        'Webgrind'],
-                                       ["https://www.percona.com/"
-                                        "get/pt-query-digest",
-                                        "/usr/bin/pt-query-advisor",
-                                        "pt-query-advisor"],
-                                       ["https://github.com/box/Anemometer/"
-                                        "archive/master.tar.gz",
-                                        '/var/lib/wo/tmp/anemometer.tar.gz',
-                                        'Anemometer']]
+                packages = packages + [[
+                    "https://raw.githubusercontent.com"
+                    "/rtCamp/eeadmin/master/cache/nginx/"
+                    "clean.php",
+                    "{0}22222/htdocs/cache/"
+                    "nginx/clean.php"
+                    .format(WOVar.wo_webroot),
+                    "clean.php"],
+                    ["https://raw.github.com/rlerdorf/"
+                     "opcache-status/master/opcache.php",
+                     "{0}22222/htdocs/cache/"
+                     "opcache/opcache.php"
+                     .format(WOVar.wo_webroot),
+                     "opcache.php"],
+                    ["https://raw.github.com/amnuts/"
+                     "opcache-gui/master/index.php",
+                     "{0}22222/htdocs/"
+                     "cache/opcache/opgui.php"
+                     .format(WOVar.wo_webroot),
+                     "Opgui"],
+                    ["https://raw.githubusercontent.com/"
+                     "mlazarov/ocp/master/ocp.php",
+                     "{0}22222/htdocs/cache/"
+                     "opcache/ocp.php"
+                     .format(WOVar.wo_webroot),
+                     "OCP.php"],
+                    ["https://github.com/jokkedk/webgrind/"
+                     "archive/master.tar.gz",
+                     '/var/lib/wo/tmp/webgrind.tar.gz',
+                     'Webgrind'],
+                    ["https://www.percona.com/"
+                     "get/pt-query-digest",
+                     "/usr/bin/pt-query-advisor",
+                     "pt-query-advisor"],
+                    ["https://github.com/box/Anemometer/"
+                     "archive/master.tar.gz",
+                     '/var/lib/wo/tmp/anemometer.tar.gz',
+                     'Anemometer']]
 
         except Exception as e:
             Log.debug(self, "{0}".format(e))
 
         if (apt_packages) or (packages):
             if (apt_packages):
                 Log.debug(self, "Calling pre_pref")
@@ -532,15 +531,15 @@
             (not pargs.phpmyadmin) and (not pargs.composer) and
                 (not pargs.netdata) and (not pargs.dashboard) and
                 (not pargs.fail2ban) and (not pargs.security) and
                 (not pargs.mysqlclient) and (not pargs.mysqltuner) and
                 (not pargs.adminer) and (not pargs.utils) and
                 (not pargs.redis) and (not pargs.proftpd) and
                 (not pargs.extplorer) and (not pargs.clamav) and
-                (not pargs.ufw) and
+                (not pargs.ufw) and (not pargs.ngxblocker) and
                 (not pargs.phpredisadmin) and (not pargs.sendmail) and
                 (not pargs.php73)):
             pargs.web = True
             pargs.admin = True
 
         if pargs.all:
             pargs.web = True
@@ -566,14 +565,15 @@
             pargs.netdata = True
             pargs.mysqltuner = True
 
         if pargs.security:
             pargs.fail2ban = True
             pargs.clamav = True
             pargs.ufw = True
+            pargs.ngxblocker = True
 
         # NGINX
         if pargs.nginx:
             if WOAptGet.is_installed(self, 'nginx-custom'):
                 Log.debug(self, "Removing apt_packages variable of Nginx")
                 apt_packages = apt_packages + WOVar.wo_nginx
 
@@ -696,32 +696,44 @@
                                    .format(WOVar.wo_webroot),
                                    '{0}22222/htdocs/cache/nginx/'
                                    'clean.php'.format(WOVar.wo_webroot),
                                    '/usr/bin/pt-query-advisor',
                                    '{0}22222/htdocs/db/anemometer'
                                    .format(WOVar.wo_webroot)]
 
+        # netdata
         if pargs.netdata:
             Log.debug(self, "Removing Netdata")
             if os.path.isfile('/opt/netdata/usr/'
                               'libexec/netdata/netdata-uninstaller.sh'):
                 packages = packages + ['/var/lib/wo/tmp/kickstart.sh']
 
+        # wordops dashboard
         if pargs.dashboard:
             if (os.path.isfile('{0}22222/htdocs/index.php'
                                .format(WOVar.wo_webroot)) or
                     os.path.isfile('{0}22222/htdocs/index.html'
                                    .format(WOVar.wo_webroot))):
                 Log.debug(self, "Removing Wo-Dashboard")
                 packages = packages + ['{0}22222/htdocs/assets'
                                        .format(WOVar.wo_webroot),
                                        '{0}22222/htdocs/index.php'
                                        .format(WOVar.wo_webroot),
                                        '{0}22222/htdocs/index.html'
                                        .format(WOVar.wo_webroot)]
+        # ngxblocker
+        if pargs.ngxblocker:
+            if os.path.isfile('/usr/local/sbin/setup-ngxblocker'):
+                packages = packages + [
+                    '/usr/local/sbin/setup-ngxblocker',
+                    '/usr/local/sbin/install-ngxblocker',
+                    '/usr/local/sbin/update-ngxblocker',
+                    '/etc/nginx/conf.d/globalblacklist.conf',
+                    '/etc/nginx/conf.d/botblocker-nginx-settings.conf',
+                    '/etc/nginx/bots.d']
 
         if (packages) or (apt_packages):
             if (not pargs.force):
                 start_remove = input('Are you sure you to want to'
                                      ' remove from server.'
                                      '\nPackage configuration will remain'
                                      ' on server after this operation.\n'
@@ -736,22 +748,24 @@
                 WOMysql.backupAll(self)
                 WOService.stop_service(self, 'mysql')
 
             # Netdata uninstaller
             if (set(['/var/lib/wo/tmp/'
                      'kickstart.sh']).issubset(set(packages))):
                 if WOVar.wo_distro == 'Raspbian':
-                    WOShellExec.cmd_exec(self, "bash /usr/"
-                                         "libexec/netdata/"
-                                         "netdata-uninstaller.sh -y -f")
-                else:
-                    WOShellExec.cmd_exec(self, "bash /opt/netdata/usr/"
-                                         "libexec/netdata/"
-                                         "netdata-uninstaller.sh - y - f",
-                                         errormsg='', log=False)
+                    WOShellExec.cmd_exec(
+                        self, "bash /usr/"
+                        "libexec/netdata/"
+                        "netdata-uninstaller.sh -y -f")
+                else:
+                    WOShellExec.cmd_exec(
+                        self, "bash /opt/netdata/usr/"
+                        "libexec/netdata/"
+                        "netdata-uninstaller.sh - y - f",
+                        errormsg='', log=False)
 
             if (packages):
                 Log.wait(self, "Removing packages           ")
                 WOFileUtils.remove(self, packages)
                 Log.valide(self, "Removing packages           ")
             if (apt_packages):
                 Log.debug(self, "Removing apt_packages")
@@ -775,15 +789,15 @@
             (not pargs.phpmyadmin) and (not pargs.composer) and
                 (not pargs.netdata) and (not pargs.dashboard) and
                 (not pargs.fail2ban) and (not pargs.security) and
                 (not pargs.mysqlclient) and (not pargs.mysqltuner) and
                 (not pargs.adminer) and (not pargs.utils) and
                 (not pargs.redis) and (not pargs.proftpd) and
                 (not pargs.extplorer) and (not pargs.clamav) and
-                (not pargs.ufw) and
+                (not pargs.ufw) and (not pargs.ngxblocker) and
                 (not pargs.phpredisadmin) and (not pargs.sendmail) and
                 (not pargs.php73)):
             pargs.web = True
             pargs.admin = True
             pargs.security = True
 
         if pargs.all:
@@ -809,14 +823,15 @@
             pargs.netdata = True
             pargs.mysqltuner = True
 
         if pargs.security:
             pargs.fail2ban = True
             pargs.clamav = True
             pargs.ufw = True
+            pargs.ngxblocker = True
 
         # NGINX
         if pargs.nginx:
             if WOAptGet.is_installed(self, 'nginx-custom'):
                 Log.debug(self, "Add Nginx to apt_packages list")
                 apt_packages = apt_packages + WOVar.wo_nginx
             else:
@@ -954,21 +969,33 @@
 
         if pargs.netdata:
             Log.debug(self, "Removing Netdata")
             if os.path.isfile('/opt/netdata/usr/'
                               'libexec/netdata/netdata-uninstaller.sh'):
                 packages = packages + ['/var/lib/wo/tmp/kickstart.sh']
 
+        # wordops dashboard
         if pargs.dashboard:
             Log.debug(self, "Removing Wo-Dashboard")
             packages = packages + ['{0}22222/htdocs/assets/'
                                    .format(WOVar.wo_webroot),
                                    '{0}22222/htdocs/index.php'
                                    .format(WOVar.wo_webroot)]
 
+        # ngxblocker
+        if pargs.ngxblocker:
+            if os.path.isfile('/usr/local/sbin/setup-ngxblocker'):
+                packages = packages + [
+                    '/usr/local/sbin/setup-ngxblocker',
+                    '/usr/local/sbin/install-ngxblocker',
+                    '/usr/local/sbin/update-ngxblocker',
+                    '/etc/nginx/conf.d/globalblacklist.conf',
+                    '/etc/nginx/conf.d/botblocker-nginx-settings.conf',
+                    '/etc/nginx/bots.d']
+
         if (packages) or (apt_packages):
             if (not pargs.force):
                 start_purge = input('Are you sure you to want to'
                                     ' purge stacks from this server ?'
                                     '\nPackage configuration and data '
                                     'will not remain'
                                     ' on this server after this operation.\n'
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/stack_migrate.py` & `wordops-3.9.9.4/wo/cli/plugins/stack_migrate.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/plugins/stack_pref.py` & `wordops-3.9.9.4/wo/cli/plugins/stack_pref.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
                           "sfo1.mirrors.digitalocean.com"
                           "\nPin-Priority: 1000\n")
             with open('/etc/apt/preferences.d/'
                       'MariaDB.pref', 'w') as mysql_pref_file:
                 mysql_pref_file.write(mysql_pref)
             WORepo.add(self, repo_url=WOVar.wo_mysql_repo)
             WORepo.add_key(self, '0xcbcb082a1bb943db',
-                           keyserver='keys.gnupg.net')
+                           keyserver='keyserver.ubuntu.com')
             WORepo.add_key(self, '0xF1656F24C74CD1D8',
-                           keyserver='keys.gnupg.net')
+                           keyserver='keyserver.ubuntu.com')
     if "mariadb-server" in apt_packages:
         # generate random 24 characters root password
         chars = ''.join(random.sample(string.ascii_letters, 24))
 
         # configure MySQL non-interactive install
         if ((WOVar.wo_distro == 'raspbian') and
                 (WOVar.wo_platform_codename == 'stretch')):
@@ -847,15 +847,14 @@
                               msg="Adding Fail2ban into Git")
 
         # Proftpd configuration
         if "proftpd-basic" in apt_packages:
             WOGit.add(self, ["/etc/proftpd"],
                       msg="Adding ProFTPd into Git")
             if os.path.isfile("/etc/proftpd/proftpd.conf"):
-                Log.info(self, "Configuring ProFTPd")
                 Log.debug(self, "Setting up Proftpd configuration")
                 WOFileUtils.searchreplace(
                     self, "/etc/proftpd/proftpd.conf",
                     "# DefaultRoot", "DefaultRoot")
                 WOFileUtils.searchreplace(
                     self, "/etc/proftpd/proftpd.conf",
                     "# RequireValidShell", "RequireValidShell")
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/stack_services.py` & `wordops-3.9.9.4/wo/cli/plugins/stack_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.core.aptget import WOAptGet
 from wo.core.logging import Log
 from wo.core.services import WOService
 from wo.core.variables import WOVar
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/stack_upgrade.py` & `wordops-3.9.9.4/wo/cli/plugins/stack_upgrade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import os
 import shutil
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.cli.plugins.stack_pref import post_pref, pre_pref
 from wo.core.aptget import WOAptGet
 from wo.core.download import WODownload
 from wo.core.extract import WOExtract
 from wo.core.fileutils import WOFileUtils
 from wo.core.logging import Log
-from wo.core.services import WOService
 from wo.core.shellexec import WOShellExec
 from wo.core.variables import WOVar
 
 
 class WOStackUpgradeController(CementBaseController):
     class Meta:
         label = 'upgrade'
@@ -90,42 +88,36 @@
             pargs.mysql = True
             pargs.wpcli = True
 
         if pargs.nginx:
             if WOAptGet.is_installed(self, 'nginx-custom'):
                 apt_packages = apt_packages + WOVar.wo_nginx
             else:
-                if os.path.isfile(self, '/usr/sbin/nginx'):
+                if os.path.isfile('/usr/sbin/nginx'):
                     Log.info(self, "Updating Nginx templates")
                     post_pref(self, WOVar.wo_nginx, [])
                 else:
                     Log.info(self, "Nginx Stable is not already installed")
 
         if pargs.php:
             if WOAptGet.is_installed(self, 'php7.2-fpm'):
-                if not WOAptGet.is_installed(self, 'php7.3-fpm'):
-                    apt_packages = apt_packages + WOVar.wo_php + \
-                        WOVar.wo_php_extra
-                else:
-                    apt_packages = apt_packages + WOVar.wo_php
+                apt_packages = apt_packages + WOVar.wo_php + \
+                    WOVar.wo_php_extra
             else:
                 Log.info(self, "PHP 7.2 is not installed")
 
         if pargs.php73:
             if WOAptGet.is_installed(self, 'php7.3-fpm'):
-                if not WOAptGet.is_installed(self, 'php7.2-fpm'):
-                    apt_packages = apt_packages + WOVar.wo_php73 + \
-                        WOVar.wo_php_extra
-                else:
-                    apt_packages = apt_packages + WOVar.wo_php73
+                apt_packages = apt_packages + WOVar.wo_php73 + \
+                    WOVar.wo_php_extra
             else:
                 Log.info(self, "PHP 7.3 is not installed")
 
         if pargs.mysql:
-            if WOAptGet.is_installed(self, 'mariadb-server'):
+            if WOShellExec.cmd_exec(self, 'mysqladmin ping'):
                 apt_packages = apt_packages + ['mariadb-server']
             else:
                 Log.info(self, "MariaDB is not installed")
 
         if pargs.redis:
             if WOAptGet.is_installed(self, 'redis-server'):
                 apt_packages = apt_packages + ['redis-server']
@@ -168,37 +160,36 @@
                       "/phpMyAdmin/{0}/"
                       "phpMyAdmin-{0}-"
                       "all-languages"
                       ".tar.gz".format(WOVar.wo_phpmyadmin),
                       "/var/lib/wo/tmp/pma.tar.gz",
                       "PHPMyAdmin"]]
             else:
-                Log.error(self, "phpMyAdmin isn't installed")
+                Log.info(self, "phpMyAdmin isn't installed")
 
         if pargs.composer:
             if os.path.isfile('/usr/local/bin/composer'):
                 packages = packages + [["https://getcomposer.org/installer",
                                         "/var/lib/wo/tmp/composer-install",
                                         "Composer"]]
             else:
-                Log.error(self, "Composer isn't installed")
+                Log.info(self, "Composer isn't installed")
 
         if ((not (apt_packages)) and (not(packages))):
             self.app.args.print_help()
         else:
             if (apt_packages):
-                if not (set(["php7.2-fpm"]).issubset(set(apt_packages)) and
-                        set(["php7.3-fpm"]).issubset(set(apt_packages)) and
-                        set(["nginx-custom",
-                             "nginx-wo"]).issubset(set(apt_packages)) and
-                        set(['mariadb-server']).issubset(set(apt_packages))):
+                if (("php7.2-fpm" not in apt_packages) and
+                        ("php7.3-fpm" not in apt_packages) and
+                        ("nginx-custom" not in apt_packages) and
+                        ("mariadb-server" not in apt_packages)):
                     pass
                 else:
                     Log.info(
-                        self, "Your site may be down for few seconds if "
+                        self, "Your sites may be down for few seconds if "
                         "you are upgrading Nginx, PHP-FPM, MariaDB or Redis")
                 # Check prompt
                 if ((not pargs.no_prompt) and (not pargs.force)):
                     start_upgrade = input("Do you want to continue:[y/N]")
                     if start_upgrade != "Y" and start_upgrade != "y":
                         Log.error(self, "Not starting package update")
                 Log.wait(self, "Updating APT packages")
@@ -215,15 +206,14 @@
                                     auto=False, purge=True)
                 if ["php7.3-fpm"] in apt_packages:
                     WOAptGet.remove(self, ['php7.3-fpm'],
                                     auto=False, purge=True)
                 # check if nginx upgrade is blocked
                 if os.path.isfile(
                         '/etc/apt/preferences.d/nginx-block'):
-                    apt_packages.remove(WOVar.wo_nginx)
                     post_pref(self, WOVar.wo_nginx, [], True)
                 # upgrade packages
                 WOAptGet.install(self, apt_packages)
                 Log.valide(self, "Upgrading APT Packages")
                 Log.wait(self, "Configuring APT Packages")
                 post_pref(self, apt_packages, [], True)
                 Log.valide(self, "Configuring APT Packages")
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/sync.py` & `wordops-3.9.9.4/wo/cli/plugins/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import glob
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.cli.plugins.sitedb import getAllsites, updateSiteInfo
 from wo.core.fileutils import WOFileUtils
 from wo.core.logging import Log
 from wo.core.mysql import StatementExcecutionError, WOMysql
```

### Comparing `wordops-3.9.9.2/wo/cli/plugins/update.py` & `wordops-3.9.9.4/wo/cli/plugins/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import time
 
-from cement.core import handler, hook
 from cement.core.controller import CementBaseController, expose
 
 from wo.core.download import WODownload
 from wo.core.logging import Log
 
 
 def wo_update_hook(app):
```

### Comparing `wordops-3.9.9.2/wo/cli/templates/22222.mustache` & `wordops-3.9.9.4/wo/cli/templates/22222.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/anemometer.mustache` & `wordops-3.9.9.4/wo/cli/templates/anemometer.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/brotli.mustache` & `wordops-3.9.9.4/wo/cli/templates/brotli.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/cf-update.mustache` & `wordops-3.9.9.4/wo/cli/templates/cf-update.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/cloudflare.mustache` & `wordops-3.9.9.4/wo/cli/templates/cloudflare.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/fastcgi.mustache` & `wordops-3.9.9.4/wo/cli/templates/fastcgi.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/gzip.mustache` & `wordops-3.9.9.4/wo/cli/templates/gzip.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/info_php.mustache` & `wordops-3.9.9.4/wo/cli/templates/info_php.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/locations.mustache` & `wordops-3.9.9.4/wo/cli/templates/locations.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/map-wp.mustache` & `wordops-3.9.9.4/wo/cli/templates/map-wp.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/mime.mustache` & `wordops-3.9.9.4/wo/cli/templates/mime.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/my.mustache` & `wordops-3.9.9.4/wo/cli/templates/my.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/nextcloud.mustache` & `wordops-3.9.9.4/wo/cli/templates/nextcloud.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/nginx-core.mustache` & `wordops-3.9.9.4/wo/cli/templates/nginx-core.mustache`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 	# SSL Settings
 	##
 
 	ssl_session_timeout 1d;
 	ssl_session_cache shared:SSL:50m;
 	ssl_session_tickets off;
 	ssl_prefer_server_ciphers on;
+    ssl_early_data on;
 	{{#tls13}}ssl_ciphers 'TLS13+AESGCM+AES256:TLS13+AESGCM+AES128:TLS13+CHACHA20:EECDH+AESGCM:EECDH+CHACHA20';
 	ssl_protocols TLSv1.2 TLSv1.3;{{/tls13}}
 	ssl_ecdh_curve X25519:P-521:P-384:P-256;
 	# Previous TLS v1.2 configuration
 	{{^tls13}}ssl_protocols TLSv1.2;
 	ssl_ciphers EECDH+CHACHA20:EECDH+AESGCM:EECDH+AES;{{/tls13}}
```

### Comparing `wordops-3.9.9.2/wo/cli/templates/php-pool.mustache` & `wordops-3.9.9.4/wo/cli/templates/php-pool.mustache`

 * *Files 18% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 chdir = /
 prefix = /var/run/php
 listen.mode = 0660
 listen.backlog = 32768
 catch_workers_output = yes
 
 
-{{#openbasedir}}php_admin_value[open_basedir] = "/var/www/:/usr/share/php/:/tmp/:/var/run/nginx-cache/"{{/openbasedir}}
+{{#openbasedir}}php_admin_value[open_basedir] = "/var/www/:/usr/share/php/:/tmp/:/var/run/nginx-cache/:/dev/urandom:/dev/shm"{{/openbasedir}}
```

### Comparing `wordops-3.9.9.2/wo/cli/templates/redis.mustache` & `wordops-3.9.9.4/wo/cli/templates/redis.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/siteinfo.mustache` & `wordops-3.9.9.4/wo/cli/templates/siteinfo.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/sshd.mustache` & `wordops-3.9.9.4/wo/cli/templates/sshd.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/stub_status.mustache` & `wordops-3.9.9.4/wo/cli/templates/stub_status.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/sysctl.mustache` & `wordops-3.9.9.4/wo/cli/templates/sysctl.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/ufw.mustache` & `wordops-3.9.9.4/wo/cli/templates/ufw.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/virtualconf-php7.mustache` & `wordops-3.9.9.4/wo/cli/templates/virtualconf-php7.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/virtualconf.mustache` & `wordops-3.9.9.4/wo/cli/templates/virtualconf.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/wo-plus.mustache` & `wordops-3.9.9.4/wo/cli/templates/wo-plus.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/wpce.mustache` & `wordops-3.9.9.4/wo/cli/templates/wpce.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/wpcommon.mustache` & `wordops-3.9.9.4/wo/cli/templates/wpcommon.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/wpfc.mustache` & `wordops-3.9.9.4/wo/cli/templates/wpfc.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/wprocket.mustache` & `wordops-3.9.9.4/wo/cli/templates/wprocket.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/cli/templates/wpsc.mustache` & `wordops-3.9.9.4/wo/cli/templates/wpsc.mustache`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/acme.py` & `wordops-3.9.9.4/wo/core/acme.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,25 @@
         Log.wait(self, "Issuing SSL cert with acme.sh")
         if not WOShellExec.cmd_exec(
                 self, "{0} ".format(WOAcme.wo_acme_exec) +
                 "--issue -d '{0}' {1} -k {2} -f"
                 .format(all_domains, acme_mode, keylenght)):
             Log.failed(self, "Issuing SSL cert with acme.sh")
             if acmedata['dns'] is True:
-                Log.warn(
+                Log.error(
                     self, "Please make sure your properly "
                     "set your DNS API credentials for acme.sh")
+                return False
             else:
                 Log.error(
                     self, "Your domain is properly configured "
                     "but acme.sh was unable to issue certificate.\n"
                     "You can find more informations in "
-                    "/var/log/wo/wordops.log", False)
-            return False
+                    "/var/log/wo/wordops.log")
+                return False
         else:
             Log.valide(self, "Issuing SSL cert with acme.sh")
             return True
 
     def deploycert(self, wo_domain_name):
         if not os.path.isfile('/etc/letsencrypt/renewal/{0}_ecc/fullchain.cer'
                               .format(wo_domain_name)):
```

### Comparing `wordops-3.9.9.2/wo/core/addswap.py` & `wordops-3.9.9.4/wo/core/addswap.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/apt_repo.py` & `wordops-3.9.9.4/wo/core/apt_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,19 @@
             except IOError as e:
                 Log.debug(self, "{0}".format(e))
                 Log.error(self, "File I/O error.")
             except Exception as e:
                 Log.debug(self, "{0}".format(e))
                 Log.error(self, "Unable to add repo")
         if ppa is not None:
-            WOShellExec.cmd_exec(
-                self, "LC_ALL=C.UTF-8 add-apt-repository -yu '{ppa_name}'"
-                .format(ppa_name=ppa))
+            if WOShellExec.cmd_exec(
+                    self, "LC_ALL=C.UTF-8 add-apt-repository -yu '{ppa_name}'"
+                    .format(ppa_name=ppa)):
+                return True
+        return False
 
     def remove(self, ppa=None, repo_url=None):
         """
         This function used to remove ppa's
         If ppa is provided adds repo file to
             /etc/apt/sources.list.d/
         command.
```

### Comparing `wordops-3.9.9.2/wo/core/aptget.py` & `wordops-3.9.9.4/wo/core/aptget.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,39 +14,48 @@
 
     def update(self):
         """
         Similar to `apt-get update`
         """
         try:
             with open('/var/log/wo/wordops.log', 'a') as f:
-                proc = subprocess.Popen('apt-mirror-updater -u',
-                                        shell=True,
-                                        stdin=None, stdout=f,
-                                        stderr=subprocess.PIPE,
-                                        executable="/bin/bash")
+                proc = subprocess.Popen(
+                    'DEBIAN_FRONTEND=noninteractive apt-get update -qq '
+                    '--allow-releaseinfo-change',
+                    shell=True, stdin=None, stdout=f,
+                    stderr=subprocess.PIPE, executable="/bin/bash")
                 proc.wait()
                 output, error_output = proc.communicate()
 
+                if "--allow-releaseinfo-change" in str(error_output):
+                    proc = subprocess.Popen(
+                        'DEBIAN_FRONTEND=noninteractive apt-get update -qq',
+                        shell=True,
+                        stdin=None, stdout=f, stderr=f,
+                        executable="/bin/bash")
+                    proc.wait()
+                    output, error_output = proc.communicate()
                 # Check what is error in error_output
                 if "NO_PUBKEY" in str(error_output):
                     # Split the output
                     Log.info(self, "Fixing missing GPG keys, please wait...")
                     error_list = str(error_output).split("\\n")
 
                     # Use a loop to add misising keys
                     for single_error in error_list:
                         if "NO_PUBKEY" in single_error:
                             key = single_error.rsplit(None, 1)[-1]
                             WORepo.add_key(
                                 self, key, keyserver="hkp://pgp.mit.edu")
 
-                    proc = subprocess.Popen('apt-get update',
-                                            shell=True,
-                                            stdin=None, stdout=f, stderr=f,
-                                            executable="/bin/bash")
+                    proc = subprocess.Popen(
+                        'DEBIAN_FRONTEND=noninteractive apt-get update -qq',
+                        shell=True,
+                        stdin=None, stdout=f, stderr=f,
+                        executable="/bin/bash")
                     proc.wait()
 
                 if proc.returncode == 0:
                     return True
                 else:
                     Log.info(self, Log.FAIL +
                              "Whoops, something went wrong...")
@@ -79,26 +88,24 @@
 
     def dist_upgrade(self):
         """
         Similar to `apt-get upgrade`
         """
         try:
             with open('/var/log/wo/wordops.log', 'a') as f:
-                proc = subprocess.Popen("DEBIAN_FRONTEND=noninteractive "
-                                        "apt-get dist-upgrade "
-                                        "--option=Dpkg::options::="
-                                        "--force-confdef "
-                                        "--option=Dpkg::options::="
-                                        "--force-unsafe-io "
-                                        "--option=Dpkg::options::="
-                                        "--force-confold "
-                                        "--assume-yes --quiet ",
-                                        shell=True, stdin=None,
-                                        stdout=f, stderr=f,
-                                        executable="/bin/bash")
+                proc = subprocess.Popen(
+                    "DEBIAN_FRONTEND=noninteractive "
+                    "apt-get "
+                    "--option=Dpkg::options::=--force-confdef "
+                    "--option=Dpkg::options::=--force-unsafe-io "
+                    "--option=Dpkg::options::=--force-confold "
+                    "--assume-yes --quiet dist-upgrade",
+                    shell=True, stdin=None,
+                    stdout=f, stderr=f,
+                    executable="/bin/bash")
                 proc.wait()
 
             if proc.returncode == 0:
                 return True
             else:
                 Log.info(self, Log.FAIL + "Oops Something went "
                          "wrong!!")
@@ -110,25 +117,23 @@
             Log.error(self, "Error while installing packages, "
                       "apt-get exited with error")
 
     def install(self, packages):
         all_packages = ' '.join(packages)
         try:
             with open('/var/log/wo/wordops.log', 'a') as f:
-                proc = subprocess.Popen("DEBIAN_FRONTEND=noninteractive "
-                                        "apt-get install "
-                                        "--option=Dpkg::options::="
-                                        "--force-confdef "
-                                        "--option=Dpkg::options::="
-                                        "--force-confold "
-                                        "--assume-yes "
-                                        "--allow-unauthenticated {0}"
-                                        .format(all_packages), shell=True,
-                                        stdin=None, stdout=f, stderr=f,
-                                        executable="/bin/bash")
+                proc = subprocess.Popen(
+                    "DEBIAN_FRONTEND=noninteractive "
+                    "apt-get install "
+                    "--option=Dpkg::options::=--force-confdef "
+                    "--option=Dpkg::options::=--force-confold "
+                    "--assume-yes --allow-unauthenticated {0}"
+                    .format(all_packages), shell=True,
+                    stdin=None, stdout=f, stderr=f,
+                    executable="/bin/bash")
                 proc.wait()
 
             if proc.returncode == 0:
                 return True
             else:
                 Log.info(self, Log.FAIL + "Oops Something went "
                          "wrong!!")
@@ -145,27 +150,27 @@
                       "and please try again...")
 
     def remove(self, packages, auto=False, purge=False):
         all_packages = ' '.join(packages)
         try:
             with open('/var/log/wo/wordops.log', 'a') as f:
                 if purge:
-                    proc = subprocess.Popen('DEBIAN_FRONTEND=noninteractive '
-                                            'apt-get autoremove --purge '
-                                            '-qq {0}'
-                                            .format(all_packages), shell=True,
-                                            stdin=None, stdout=f, stderr=f,
-                                            executable="/bin/bash")
+                    proc = subprocess.Popen(
+                        'DEBIAN_FRONTEND=noninteractive '
+                        'apt-get autoremove --purge -qq {0}'
+                        .format(all_packages), shell=True,
+                        stdin=None, stdout=f, stderr=f,
+                        executable="/bin/bash")
                 else:
-                    proc = subprocess.Popen('DEBIAN_FRONTEND=noninteractive '
-                                            'apt-get autoremove '
-                                            '-qq {0}'
-                                            .format(all_packages), shell=True,
-                                            stdin=None, stdout=f, stderr=f,
-                                            executable="/bin/bash")
+                    proc = subprocess.Popen(
+                        'DEBIAN_FRONTEND=noninteractive '
+                        'apt-get autoremove -qq {0}'
+                        .format(all_packages), shell=True,
+                        stdin=None, stdout=f, stderr=f,
+                        executable="/bin/bash")
                 proc.wait()
             if proc.returncode == 0:
                 return True
             else:
                 Log.info(self, Log.FAIL + "Oops Something went "
                          "wrong!!")
                 Log.error(self, "Check the WordOps log for more details "
@@ -224,24 +229,26 @@
         packages = ' '.join(package_name)
         try:
             with open('/var/log/wo/wordops.log', 'a') as f:
                 if repo_url is not None:
                     WORepo.add(self, repo_url=repo_url)
                 if repo_key is not None:
                     WORepo.add_key(self, repo_key)
-                proc = subprocess.Popen("apt-get update && "
-                                        "DEBIAN_FRONTEND=noninteractive "
-                                        "apt-get install -o "
-                                        "Dpkg::Options::=\"--force-confdef\""
-                                        " -o "
-                                        "Dpkg::Options::=\"--force-confold\""
-                                        " -y  --download-only {0}"
-                                        .format(packages), shell=True,
-                                        stdin=None, stdout=f, stderr=f,
-                                        executable="/bin/bash")
+                proc = subprocess.Popen(
+                    "DEBIAN_FRONTEND=noninteractive apt-get update "
+                    "-qq && "
+                    "DEBIAN_FRONTEND=noninteractive "
+                    "apt-get install -o "
+                    "Dpkg::Options::=\"--force-confdef\""
+                    " -o "
+                    "Dpkg::Options::=\"--force-confold\""
+                    " -y --download-only {0}"
+                    .format(packages), shell=True,
+                    stdin=None, stdout=f, stderr=f,
+                    executable="/bin/bash")
                 proc.wait()
 
             if proc.returncode == 0:
                 return True
             else:
                 Log.error(
                     self, "Error in fetching dpkg package.\n"
```

### Comparing `wordops-3.9.9.2/wo/core/checkfqdn.py` & `wordops-3.9.9.4/wo/core/checkfqdn.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/cron.py` & `wordops-3.9.9.4/wo/core/cron.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/database.py` & `wordops-3.9.9.4/wo/core/database.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/domainvalidate.py` & `wordops-3.9.9.4/wo/core/domainvalidate.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,36 +17,37 @@
             domain_name = domain_name[2]
         else:
             domain_name = domain_name[0]
         www_domain_name = domain_name.split('.')
         final_domain = ''
         if www_domain_name[0] == 'www':
             final_domain = '.'.join(www_domain_name[1:])
-        else:
-            final_domain = domain_name
+            return final_domain
+        return domain_name
+
 
-        return final_domain
 
     def getlevel(self, domain):
         """
             Returns the domain type : domain, subdomain and the root domain
         """
         domain_name = domain.lower().strip().split('.')
         if domain_name[0] == 'www':
             domain_name = domain_name[1:]
         domain_type = ''
         if os.path.isfile("/var/lib/wo/public_suffix_list.dat"):
             # Read mode opens a file for reading only.
             suffix_file = open(
-                "/var/lib/wo/public_suffix_list.dat", encoding='utf-8', )
+                "/var/lib/wo/public_suffix_list.dat", encoding='utf-8')
             # Read all the lines into a list.
             for domain_suffix in suffix_file:
                 if (str(domain_suffix).strip()) == ('.'.join(domain_name[1:])):
                     domain_type = 'domain'
-                    root_domain = ('.'.join(domain_name[0:]))
                     break
                 else:
                     domain_type = 'subdomain'
-                    root_domain = ('.'.join(domain_name[1:]))
             suffix_file.close()
-            return (domain_type, root_domain)
-        return ('other', domain)
+        if domain_type == 'domain':
+            root_domain = ('.'.join(domain_name[0:]))
+        else:
+            root_domain = ('.'.join(domain_name[1:]))
+        return (domain_type, root_domain)
```

### Comparing `wordops-3.9.9.2/wo/core/download.py` & `wordops-3.9.9.4/wo/core/download.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/extract.py` & `wordops-3.9.9.4/wo/core/extract.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/fileutils.py` & `wordops-3.9.9.4/wo/core/fileutils.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/git.py` & `wordops-3.9.9.4/wo/core/git.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/logging.py` & `wordops-3.9.9.4/wo/core/logging.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/logwatch.py` & `wordops-3.9.9.4/wo/core/logwatch.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/mysql.py` & `wordops-3.9.9.4/wo/core/mysql.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/nginxhashbucket.py` & `wordops-3.9.9.4/wo/core/nginxhashbucket.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/sendmail.py` & `wordops-3.9.9.4/wo/core/sendmail.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/services.py` & `wordops-3.9.9.4/wo/core/services.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/shellexec.py` & `wordops-3.9.9.4/wo/core/shellexec.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
         try:
             log and Log.debug(self, "Running command: {0}".format(command))
 
             with subprocess.Popen([command], stdout=subprocess.PIPE,
                                   stderr=subprocess.PIPE, shell=True) as proc:
                 (cmd_stdout_bytes, cmd_stderr_bytes) = proc.communicate()
                 (cmd_stdout, cmd_stderr) = (cmd_stdout_bytes.decode('utf-8',
-                                            "replace"),
+                                                                    "replace"),
                                             cmd_stderr_bytes.decode('utf-8',
-                                            "replace"))
+                                                                    "replace"))
 
             if proc.returncode == 0:
                 Log.debug(self, "Command Output: {0}, \nCommand Error: {1}"
                                 .format(cmd_stdout, cmd_stderr))
                 return True
             else:
                 Log.debug(self, "Command Output: {0}, \nCommand Error: {1}"
@@ -56,17 +56,17 @@
         """Run shell command from Python"""
         try:
             log and Log.debug(self, "Running command: {0}".format(command))
             with subprocess.Popen([command], stdout=subprocess.PIPE,
                                   stderr=subprocess.PIPE, shell=True) as proc:
                 (cmd_stdout_bytes, cmd_stderr_bytes) = proc.communicate()
                 (cmd_stdout, cmd_stderr) = (cmd_stdout_bytes.decode('utf-8',
-                                            "replace"),
+                                                                    "replace"),
                                             cmd_stderr_bytes.decode('utf-8',
-                                            "replace"))
+                                                                    "replace"))
 
             if proc.returncode == 0:
                 Log.debug(self, "Command Output: {0}, \nCommand Error: {1}"
                                 .format(cmd_stdout, cmd_stderr))
                 return cmd_stdout
             else:
                 Log.debug(self, "Command Output: {0}, \nCommand Error: {1}"
```

### Comparing `wordops-3.9.9.2/wo/core/sslutils.py` & `wordops-3.9.9.4/wo/core/sslutils.py`

 * *Files identical despite different names*

### Comparing `wordops-3.9.9.2/wo/core/template.py` & `wordops-3.9.9.4/wo/core/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 """
 Render Templates
 """
 
 
-class WOTemplate():
+class WOTemplate:
     """WordOps template utilities"""
 
     def deploy(self, fileconf, template, data, overwrite=True):
         """Deploy template with render()"""
         data = dict(data)
         if (not os.path.isfile('{0}.custom'
                                .format(fileconf))):
```

### Comparing `wordops-3.9.9.2/wo/core/variables.py` & `wordops-3.9.9.4/wo/core/variables.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sh import git
 
 
 class WOVar():
     """Intialization of core variables"""
 
     # WordOps version
-    wo_version = "3.9.9.2"
+    wo_version = "3.9.9.4"
     # WordOps packages versions
     wo_wp_cli = "2.3.0"
     wo_adminer = "4.7.3"
     wo_phpmyadmin = "4.9.1"
     wo_extplorer = "2.1.13"
     wo_dashboard = "1.2"
 
@@ -136,52 +136,51 @@
                 "php7.3-readline", "php7.3-common", "php7.3-recode",
                 "php7.3-cli", "php7.3-mbstring", "php7.3-intl",
                 "php7.3-bcmath", "php7.3-mysql", "php7.3-opcache",
                 "php7.3-zip", "php7.3-xml", "php7.3-soap"]
     wo_php_extra = ["php-memcached", "php-imagick",
                     "graphviz", "php-xdebug", "php-msgpack", "php-redis"]
 
-    if not wo_distro == 'raspbian':
-        if (not wo_platform_codename == 'jessie'):
-            wo_mysql = ["mariadb-server", "percona-toolkit",
-                        "python3-mysqldb", "mariadb-backup"]
-        else:
-            wo_mysql = ["mariadb-server", "percona-toolkit",
-                        "python3-mysql.connector"]
+    wo_mysql = ["mariadb-server", "percona-toolkit"]
+    if wo_distro == 'raspbian':
+        wo_mysql = wo_mysql + ["python3-mysqldb"]
     else:
-        wo_mysql = ["mariadb-server", "percona-toolkit",
-                    "python3-mysqldb"]
+        if wo_platform_codename == 'jessie':
+            wo_mysql = wo_mysql + ["python3-mysql.connector"]
+        else:
+            wo_mysql = wo_mysql + ["python3-mysqldb", "mariadb-backup"]
 
+    wo_mysql_client = ["mariadb-client"]
     if wo_platform_codename == 'jessie':
-        wo_mysql_client = ["mariadb-client", "python3-mysqldb"]
+        wo_mysql_client = wo_mysql_client + ["python3-mysqldb"]
     else:
-        wo_mysql_client = ["mariadb-client", "python3-mysql.connector"]
+        wo_mysql_client = wo_mysql_client + ["python3-mysql.connector"]
 
     wo_fail2ban = ["fail2ban"]
     wo_clamav = ["clamav", "clamav-freshclam"]
 
     # Redis repo details
     if wo_distro == 'ubuntu':
         wo_php_repo = "ppa:ondrej/php"
         wo_redis_repo = ("ppa:chris-lea/redis-server")
         wo_goaccess_repo = ("ppa:alex-p/goaccess")
         wo_mysql_repo = ("deb [arch=amd64,ppc64el] "
-                         "http://sfo1.mirrors.digitalocean.com/mariadb/repo/"
+                         "http://mariadb.mirrors.ovh.net/MariaDB/repo/"
                          "10.3/ubuntu {codename} main"
                          .format(codename=wo_platform_codename))
 
     else:
         wo_php_repo = (
             "deb https://packages.sury.org/php/ {codename} main"
             .format(codename=wo_platform_codename))
         wo_php_key = 'AC0E47584A7A714D'
         wo_redis_repo = ("deb https://packages.sury.org/php/ {codename} all"
                          .format(codename=wo_platform_codename))
         wo_mysql_repo = ("deb [arch=amd64,ppc64el] "
-                         "http://sfo1.mirrors.digitalocean.com/mariadb/repo/"
+                         "http://mariadb.mirrors.ovh.net/MariaDB/repo/"
                          "10.3/debian {codename} main"
                          .format(codename=wo_platform_codename))
 
     wo_redis = ['redis-server']
 
     # Repo path
     wo_repo_file = "wo-repo.list"
```

### Comparing `wordops-3.9.9.2/wordops.egg-info/PKG-INFO` & `wordops-3.9.9.4/wordops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordops
-Version: 3.9.9.2
+Version: 3.9.9.4
 Summary: WordPress & server administration toolset
 Home-page: https://github.com/WordOps/WordOps
 Author: WordOps
 Author-email: contact@wordops.io
 License: MIT
 Description: <p align="center"><img src="https://raw.githubusercontent.com/WordOps/WordOps/master/logo.png" width="400" alt="Wordops" /><a href="https://wordops.net">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wordops Version: 3.9.9.2 Summary: WordPress &
+Metadata-Version: 2.1 Name: wordops Version: 3.9.9.4 Summary: WordPress &
 server administration toolset Home-page: https://github.com/WordOps/WordOps
 Author: WordOps Author-email: contact@wordops.io License: MIT Description:
                                    [Wordops]
 ***** An essential toolset that eases WordPress site and server administration
                                      *****
                                    [WordOps]
                    [build] [MIT] [Commits] [GitHub release]
```

### Comparing `wordops-3.9.9.2/wordops.egg-info/SOURCES.txt` & `wordops-3.9.9.4/wordops.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 config/wo.conf
 config/bash_completion.d/wo_auto.rc
 config/plugins.d/clean.conf
 config/plugins.d/debug.conf
```

