# Comparing `tmp/hcs-cli-0.1.48.tar.gz` & `tmp/hcs-cli-0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.48.tar", last modified: Mon Jul 31 01:12:46 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.50.tar", last modified: Thu Aug  3 22:00:47 2023, max compression
```

## Comparing `hcs-cli-0.1.48.tar` & `hcs-cli-0.1.50.tar`

### file list

```diff
@@ -1,338 +1,340 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.294866 hcs-cli-0.1.48/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.48/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.047145 hcs-cli-0.1.48/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     3314 2023-07-31 00:05:25.000000 hcs-cli-0.1.48/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)      391 2023-07-26 01:21:48.000000 hcs-cli-0.1.48/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.48/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.48/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.48/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.48/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.48/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.48/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.48/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     3769 2023-07-31 01:12:46.294457 hcs-cli-0.1.48/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2895 2023-07-26 02:28:33.000000 hcs-cli-0.1.48/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.053218 hcs-cli-0.1.48/doc/
--rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.48/doc/az-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.48/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.48/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.48/doc/hcs-cli-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     6164 2023-07-18 01:31:14.000000 hcs-cli-0.1.48/doc/hcs-plan.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.057561 hcs-cli-0.1.48/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     3769 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     8169 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      295 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:45.999303 hcs-cli-0.1.48/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.058479 hcs-cli-0.1.48/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.48/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.48/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      296 2023-07-29 05:49:51.000000 hcs-cli-0.1.48/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-31 01:12:46.294995 hcs-cli-0.1.48/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-31 01:11:59.000000 hcs-cli-0.1.48/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.061777 hcs-cli-0.1.48/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/tests/conftest.py
--rwxr-xr-x   0 nanw       (501) staff       (20)       85 2023-07-26 00:47:17.000000 hcs-cli-0.1.48/tests/test.sh
--rw-r--r--   0 nanw       (501) staff       (20)     3363 2023-07-26 01:38:26.000000 hcs-cli-0.1.48/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.062493 hcs-cli-0.1.48/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.063109 hcs-cli-0.1.48/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.065537 hcs-cli-0.1.48/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.067183 hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.068751 hcs-cli-0.1.48/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)    12447 2023-07-29 15:57:43.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.070272 hcs-cli-0.1.48/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.48/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.072281 hcs-cli-0.1.48/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.077117 hcs-cli-0.1.48/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.078173 hcs-cli-0.1.48/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.082434 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/
--rw-r--r--   0 nanw       (501) staff       (20)      636 2023-07-24 16:33:32.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      984 2023-07-24 16:35:03.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      943 2023-07-24 16:35:13.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      855 2023-07-24 16:35:24.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.083393 hcs-cli-0.1.48/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1016 2023-07-19 21:52:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.088367 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2303 2023-07-24 18:15:37.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 21:53:29.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      861 2023-07-25 02:42:47.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.093833 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)     2606 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1039 2023-07-24 18:12:59.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)     1059 2023-07-19 21:54:27.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1101 2023-07-28 18:11:23.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.097622 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1119 2023-07-24 21:42:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:54:59.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1845 2023-07-24 21:40:06.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.101685 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/
--rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-19 21:55:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:55:32.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.105594 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-07-17 17:45:02.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-21 02:40:22.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      922 2023-07-19 22:38:04.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      857 2023-07-19 22:46:04.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.106569 hcs-cli-0.1.48/vhcs/cli/cmds/auth/
--rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.48/vhcs/cli/cmds/auth/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.108189 hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-24 16:53:46.000000 hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.108924 hcs-cli-0.1.48/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.111401 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-07-28 06:07:51.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     6571 2023-07-29 06:15:08.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.113767 hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4149 2023-07-31 00:47:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.118409 hcs-cli-0.1.48/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      957 2023-07-29 14:34:24.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      907 2023-07-25 15:46:38.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-25 00:33:49.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-24 23:58:01.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.122747 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-07-18 20:31:16.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1722 2023-07-24 18:08:29.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)     1284 2023-07-24 18:08:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1144 2023-07-19 21:58:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.126257 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1049 2023-07-19 21:58:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-19 21:58:43.000000 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.127990 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.133658 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      971 2023-07-19 21:58:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.140554 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1992 2023-07-19 22:34:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1063 2023-07-19 21:59:46.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1572 2023-07-19 21:59:58.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-07-19 22:32:52.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.48/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.011717 hcs-cli-0.1.48/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.142536 hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      981 2023-07-19 22:00:09.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.144313 hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:00:19.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.149324 hcs-cli-0.1.48/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1139 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1788 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.153260 hcs-cli-0.1.48/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2744 2023-07-30 23:31:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     2273 2023-07-30 23:31:29.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/destroy.py
--rw-r--r--   0 nanw       (501) staff       (20)     2113 2023-07-30 23:23:45.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/graph.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.154875 hcs-cli-0.1.48/vhcs/cli/cmds/portal/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.159183 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 22:02:34.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-24 21:35:27.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      862 2023-07-24 21:32:49.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.163090 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-19 22:02:34.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      940 2023-07-19 22:02:34.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-24 21:37:06.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.170931 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1108 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      912 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      934 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      837 2023-07-21 18:40:45.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1022 2023-07-21 18:42:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/set-edge.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.173005 hcs-cli-0.1.48/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.174016 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.177160 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.48/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.182558 hcs-cli-0.1.48/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-27 01:24:59.000000 hcs-cli-0.1.48/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.195508 hcs-cli-0.1.48/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.48/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.48/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.48/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.197594 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.48/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.48/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.48/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.48/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.48/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.48/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.48/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.48/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6919 2023-07-28 02:46:20.000000 hcs-cli-0.1.48/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2859 2023-07-27 01:21:30.000000 hcs-cli-0.1.48/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     7606 2023-07-29 14:44:11.000000 hcs-cli-0.1.48/vhcs/common/job_view.py
--rw-r--r--   0 nanw       (501) staff       (20)     6329 2023-07-13 00:38:57.000000 hcs-cli-0.1.48/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.203191 hcs-cli-0.1.48/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.48/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1808 2023-07-19 22:44:47.000000 hcs-cli-0.1.48/vhcs/common/sglib/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.48/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-18 18:53:18.000000 hcs-cli-0.1.48/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.48/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.48/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)      600 2023-07-19 22:16:46.000000 hcs-cli-0.1.48/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)    10097 2023-07-29 00:16:03.000000 hcs-cli-0.1.48/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.204928 hcs-cli-0.1.48/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.48/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.212051 hcs-cli-0.1.48/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      175 2023-07-27 17:24:35.000000 hcs-cli-0.1.48/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      125 2023-07-27 23:00:30.000000 hcs-cli-0.1.48/vhcs/plan/actions.py
--rw-r--r--   0 nanw       (501) staff       (20)     1299 2023-07-27 22:49:14.000000 hcs-cli-0.1.48/vhcs/plan/base_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)      113 2023-07-25 17:15:18.000000 hcs-cli-0.1.48/vhcs/plan/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    16672 2023-07-31 01:09:30.000000 hcs-cli-0.1.48/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)    10264 2023-07-30 23:25:14.000000 hcs-cli-0.1.48/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     6037 2023-07-30 19:15:09.000000 hcs-cli-0.1.48/vhcs/plan/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     5804 2023-07-31 00:03:11.000000 hcs-cli-0.1.48/vhcs/plan/kop.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.212823 hcs-cli-0.1.48/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.48/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.223219 hcs-cli-0.1.48/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)      166 2023-07-28 23:53:29.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7207 2023-07-29 05:50:22.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      650 2023-07-30 23:35:50.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1569 2023-07-29 15:07:09.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     2217 2023-07-29 15:07:18.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_user.py
--rw-r--r--   0 nanw       (501) staff       (20)     1418 2023-07-29 15:07:24.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/nat_gateway.py
--rw-r--r--   0 nanw       (501) staff       (20)     1564 2023-07-29 15:07:29.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)     1628 2023-07-29 15:07:34.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/public_ip.py
--rw-r--r--   0 nanw       (501) staff       (20)     1511 2023-07-31 00:16:15.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1962 2023-07-29 15:07:44.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/subnet.py
--rw-r--r--   0 nanw       (501) staff       (20)     1569 2023-07-29 15:07:48.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/virtual_network.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.226370 hcs-cli-0.1.48/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.48/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.48/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1695 2023-07-29 15:07:54.000000 hcs-cli-0.1.48/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.242772 hcs-cli-0.1.48/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1493 2023-07-29 15:07:59.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/ad.py
--rw-r--r--   0 nanw       (501) staff       (20)     3857 2023-07-29 15:08:03.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1317 2023-07-29 15:08:08.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1405 2023-07-29 15:08:12.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/identity_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     3515 2023-07-29 15:08:15.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/image.py
--rw-r--r--   0 nanw       (501) staff       (20)     1598 2023-07-29 15:08:19.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)     1527 2023-07-29 15:08:23.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     2044 2023-07-29 15:08:26.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     1646 2023-07-29 15:08:30.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     1405 2023-07-29 15:08:34.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/site.py
--rw-r--r--   0 nanw       (501) staff       (20)     2003 2023-07-29 15:08:37.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/uag.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.244284 hcs-cli-0.1.48/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     6989 2023-07-28 20:25:17.000000 hcs-cli-0.1.48/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.250053 hcs-cli-0.1.48/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       68 2023-07-24 16:34:10.000000 hcs-cli-0.1.48/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      853 2023-07-24 16:32:50.000000 hcs-cli-0.1.48/vhcs/service/admin/ad.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.48/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     3997 2023-07-28 20:25:54.000000 hcs-cli-0.1.48/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1082 2023-07-24 17:45:25.000000 hcs-cli-0.1.48/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1459 2023-07-18 19:54:38.000000 hcs-cli-0.1.48/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2106 2023-07-26 19:27:04.000000 hcs-cli-0.1.48/vhcs/service/admin/template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-26 04:28:07.000000 hcs-cli-0.1.48/vhcs/service/admin/uag.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.251636 hcs-cli-0.1.48/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.48/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      879 2023-07-24 17:10:24.000000 hcs-cli-0.1.48/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.254807 hcs-cli-0.1.48/vhcs/service/ims/
--rw-r--r--   0 nanw       (501) staff       (20)       71 2023-07-18 21:11:37.000000 hcs-cli-0.1.48/vhcs/service/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2383 2023-07-28 19:05:05.000000 hcs-cli-0.1.48/vhcs/service/ims/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      944 2023-07-19 21:57:09.000000 hcs-cli-0.1.48/vhcs/service/ims/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)     2083 2023-07-26 17:02:49.000000 hcs-cli-0.1.48/vhcs/service/ims/images.py
--rw-r--r--   0 nanw       (501) staff       (20)     3307 2023-07-26 04:28:49.000000 hcs-cli-0.1.48/vhcs/service/ims/version.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.256142 hcs-cli-0.1.48/vhcs/service/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.48/vhcs/service/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.48/vhcs/service/inventory/vm.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.258153 hcs-cli-0.1.48/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.48/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.48/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2755 2023-07-21 02:58:07.000000 hcs-cli-0.1.48/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.260550 hcs-cli-0.1.48/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.48/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.48/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.48/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.262317 hcs-cli-0.1.48/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.48/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.48/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.265548 hcs-cli-0.1.48/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.48/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-24 21:34:40.000000 hcs-cli-0.1.48/vhcs/service/portal/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-24 21:37:58.000000 hcs-cli-0.1.48/vhcs/service/portal/pool.py
--rw-r--r--   0 nanw       (501) staff       (20)     1493 2023-07-21 18:45:40.000000 hcs-cli-0.1.48/vhcs/service/portal/site.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.267440 hcs-cli-0.1.48/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.48/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.48/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.270277 hcs-cli-0.1.48/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.48/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.277938 hcs-cli-0.1.48/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.48/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1482 2023-07-13 00:23:42.000000 hcs-cli-0.1.48/vhcs/support/daas/cidr_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-07-28 06:08:00.000000 hcs-cli-0.1.48/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1320 2023-07-28 06:07:21.000000 hcs-cli-0.1.48/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     4369 2023-07-29 06:18:32.000000 hcs-cli-0.1.48/vhcs/support/daas/infra_green.py
--rw-r--r--   0 nanw       (501) staff       (20)     4072 2023-07-28 15:37:09.000000 hcs-cli-0.1.48/vhcs/support/daas/infra_reuse.py
--rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.48/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.030846 hcs-cli-0.1.48/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.289034 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)    14930 2023-07-30 19:46:33.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-green.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      365 2023-07-29 05:52:51.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-green.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)    13147 2023-07-30 18:26:48.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      518 2023-07-28 22:09:28.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-reuse.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     3820 2023-07-31 01:07:28.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      143 2023-07-30 16:28:42.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     4684 2023-07-31 00:13:55.000000 hcs-cli-0.1.48/vhcs/support/daas/tenant_calc.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.48/vhcs/support/plan_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.48/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.293732 hcs-cli-0.1.48/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1929 2023-07-18 18:58:54.000000 hcs-cli-0.1.48/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.365992 hcs-cli-0.1.50/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.055359 hcs-cli-0.1.50/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     3324 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      391 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      896 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     3832 2023-08-03 22:00:47.365520 hcs-cli-0.1.50/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2958 2023-08-03 21:59:00.000000 hcs-cli-0.1.50/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.062375 hcs-cli-0.1.50/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)    13312 2023-08-03 21:59:56.000000 hcs-cli-0.1.50/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.065773 hcs-cli-0.1.50/doc/images/
+-rw-r--r--   0 nanw       (501) staff       (20)    23659 2023-08-03 16:48:37.000000 hcs-cli-0.1.50/doc/images/hcs-plan-graph.svg
+-rw-r--r--   0 nanw       (501) staff       (20)   142119 2023-08-03 16:35:52.000000 hcs-cli-0.1.50/doc/images/hcs-plan.png
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.071976 hcs-cli-0.1.50/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     3832 2023-08-03 22:00:46.000000 hcs-cli-0.1.50/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     8063 2023-08-03 22:00:46.000000 hcs-cli-0.1.50/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-08-03 22:00:46.000000 hcs-cli-0.1.50/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-08-03 22:00:46.000000 hcs-cli-0.1.50/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      295 2023-08-03 22:00:46.000000 hcs-cli-0.1.50/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-08-03 22:00:46.000000 hcs-cli-0.1.50/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.008286 hcs-cli-0.1.50/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.073793 hcs-cli-0.1.50/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      296 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-08-03 22:00:47.366121 hcs-cli-0.1.50/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-08-03 22:00:41.000000 hcs-cli-0.1.50/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.130280 hcs-cli-0.1.50/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/tests/conftest.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)       85 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/tests/test.sh
+-rw-r--r--   0 nanw       (501) staff       (20)     3417 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.131410 hcs-cli-0.1.50/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.132497 hcs-cli-0.1.50/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.137356 hcs-cli-0.1.50/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.141022 hcs-cli-0.1.50/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.152301 hcs-cli-0.1.50/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:43.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)    14616 2023-08-03 21:55:16.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.156773 hcs-cli-0.1.50/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.50/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.163283 hcs-cli-0.1.50/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.50/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.173773 hcs-cli-0.1.50/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.50/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.174854 hcs-cli-0.1.50/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.178982 hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/
+-rw-r--r--   0 nanw       (501) staff       (20)      636 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      972 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      934 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      845 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.179903 hcs-cli-0.1.50/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      990 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.183843 hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2105 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      917 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      853 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.187641 hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)     2592 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1032 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1052 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1061 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.191328 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1096 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      925 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1838 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.194162 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      994 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.197624 hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      849 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.198463 hcs-cli-0.1.50/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.200166 hcs-cli-0.1.50/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      908 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.201501 hcs-cli-0.1.50/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.204818 hcs-cli-0.1.50/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1037 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7130 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/daas/infra/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.207367 hcs-cli-0.1.50/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4604 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.211915 hcs-cli-0.1.50/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      951 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      900 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      921 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      995 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.215144 hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1715 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1132 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.217643 hcs-cli-0.1.50/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      937 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.218415 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.221713 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      964 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.227530 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1976 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1056 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1558 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6989 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/login.py
+-rw-r--r--   0 nanw       (501) staff       (20)      768 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/logout.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.021059 hcs-cli-0.1.50/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.229291 hcs-cli-0.1.50/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      974 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.230817 hcs-cli-0.1.50/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      883 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.236445 hcs-cli-0.1.50/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      883 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1774 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.240057 hcs-cli-0.1.50/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      666 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2445 2023-08-03 21:54:21.000000 hcs-cli-0.1.50/vhcs/cli/cmds/plan/apply.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2422 2023-08-03 21:54:08.000000 hcs-cli-0.1.50/vhcs/cli/cmds/plan/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2191 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/plan/graph.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.241117 hcs-cli-0.1.50/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.244371 hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      919 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      946 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      857 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.247054 hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      908 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      933 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.250733 hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1101 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      905 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      927 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      830 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1015 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/set-edge.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.252371 hcs-cli-0.1.50/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.50/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1744 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.253092 hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.255465 hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1120 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2849 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.257236 hcs-cli-0.1.50/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.50/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.270301 hcs-cli-0.1.50/vhcs/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.273116 hcs-cli-0.1.50/vhcs/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2407 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3971 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5102 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1208 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10790 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/data_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2856 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3063 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6342 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/logger.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6312 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1597 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6726 2023-08-02 22:37:12.000000 hcs-cli-0.1.50/vhcs/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.280672 hcs-cli-0.1.50/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      175 2023-08-03 21:56:23.000000 hcs-cli-0.1.50/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      125 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1298 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/base_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)      116 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    17656 2023-08-03 21:54:30.000000 hcs-cli-0.1.50/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10335 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7246 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5732 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.281469 hcs-cli-0.1.50/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.289828 hcs-cli-0.1.50/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)      167 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7225 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1574 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2225 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1392 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/nat_gateway.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1570 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1603 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/public_ip.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1517 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1965 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/subnet.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1574 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/azure/virtual_network.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.292795 hcs-cli-0.1.50/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1694 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1126 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.303192 hcs-cli-0.1.50/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1494 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3648 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1315 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1407 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/identity_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3513 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/image.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1529 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2046 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/pool_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1648 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1407 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/site.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1996 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/plan/provider/hcs/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.304110 hcs-cli-0.1.50/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.50/vhcs/service/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.313563 hcs-cli-0.1.50/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       69 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      868 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1219 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3799 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1312 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1478 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2014 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2333 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/admin/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.315503 hcs-cli-0.1.50/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       20 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      897 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.319926 hcs-cli-0.1.50/vhcs/service/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)       72 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2366 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/ims/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      960 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/ims/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2099 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/ims/images.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3356 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/ims/version.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.321659 hcs-cli-0.1.50/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       26 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1308 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.324290 hcs-cli-0.1.50/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2774 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.326827 hcs-cli-0.1.50/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1099 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1056 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.328581 hcs-cli-0.1.50/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1226 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.332713 hcs-cli-0.1.50/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      958 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)      944 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/portal/pool.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1510 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/portal/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.334621 hcs-cli-0.1.50/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       18 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1420 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.341944 hcs-cli-0.1.50/vhcs/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3756 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1781 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6806 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/client_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8043 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5191 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      897 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8061 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/sglib/login_support.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.344205 hcs-cli-0.1.50/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.352033 hcs-cli-0.1.50/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1469 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/cidr_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3845 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1305 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4323 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/infra_green.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4004 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/infra_reuse.py
+-rw-r--r--   0 nanw       (501) staff       (20)      436 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.039946 hcs-cli-0.1.50/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.360010 hcs-cli-0.1.50/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)    15004 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/templates/v1/infra-green.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      354 2023-08-02 19:08:25.000000 hcs-cli-0.1.50/vhcs/support/daas/templates/v1/infra-green.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)    13147 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      518 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/templates/v1/infra-reuse.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3972 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      143 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     4869 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/tenant_prep.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2096 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/daas/tenant_summary.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1470 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/plan_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2629 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-08-03 22:00:47.364780 hcs-cli-0.1.50/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.50/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7587 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/util/job_view.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1909 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1718 2023-08-01 22:36:44.000000 hcs-cli-0.1.50/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.48/.gitignore` & `hcs-cli-0.1.50/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/.vscode/launch.json` & `hcs-cli-0.1.50/.vscode/launch.json`

 * *Files 2% similar despite different names*

```diff
@@ -46,25 +46,25 @@
             "name": "plan destroy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "destroy", "-f", "nanw.plan.yml"]
+            "args" : ["plan", "destroy", "-f", "t1.plan.yml", "--sequential"]
         },
         {
             "name": "plan deploy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-f", "starter.plan.yml", "--sequential"]
+            "args" : ["plan", "deploy", "-f", "s17.plan.yml", "--sequential"]
         },
         {
             "name": "UT",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/python3",
             "console": "integratedTerminal",
@@ -86,11 +86,11 @@
             "name": "tmp",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-f", "t1.plan.yml", "--sequential"]
+            "args" : ["plan", "deploy", "-f", "t4.plan.yml", "--sequential"]
         },
     ]
 }
```

### Comparing `hcs-cli-0.1.48/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.50/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.50/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/GOVERNANCE.md` & `hcs-cli-0.1.50/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/LICENSE` & `hcs-cli-0.1.50/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/Makefile` & `hcs-cli-0.1.50/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 	rm -rf dist
 	rm -rf hcs_cli.egg-info
 	find . -name .DS_Store -delete
 	find . -name "*.pyc" -delete
 	
 lint:
 	python3 -m black .	
-
+sca:
+	mypy vhcs
 build:
 	export SCM_REV=$(shell git rev-parse --short HEAD); \
 	python3 setup.py sdist bdist_wheel
 
 update:
 	pipreqs . --force
```

### Comparing `hcs-cli-0.1.48/PKG-INFO` & `hcs-cli-0.1.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.48
+Version: 0.1.50
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -90,17 +90,16 @@
 hcs profile use
 ```
 
 
 ## Documentation
 
 * [HCS CLI Cheatsheet](doc/hcs-cli-cheatsheet.md)
-
+* [HCS Plan, a resource manager for deployment](doc/hcs-plan.md)
 * [Development Setup](doc/dev-setup.md)
-
 * Based on [Context Programming](https://github.com/nanw1103/context-programming)
 
   
 ## Contributing
 
 The horizon-cloud-service-cli project team welcomes contributions from the community. Before you start working with horizon-cloud-service-cli, please read and sign our Contributor License Agreement [CLA](https://cla.vmware.com/cla/1/preview). If you wish to contribute code and you have not signed our CLA, our bot will prompt you to do so when you open a Pull Request. For any questions about the CLA process, please refer to our [FAQ]([https://cla.vmware.com/faq](https://cla.vmware.com/faq)).
```

### Comparing `hcs-cli-0.1.48/README.md` & `hcs-cli-0.1.50/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,16 @@
 hcs profile use
 ```
 
 
 ## Documentation
 
 * [HCS CLI Cheatsheet](doc/hcs-cli-cheatsheet.md)
-
+* [HCS Plan, a resource manager for deployment](doc/hcs-plan.md)
 * [Development Setup](doc/dev-setup.md)
-
 * Based on [Context Programming](https://github.com/nanw1103/context-programming)
 
   
 ## Contributing
 
 The horizon-cloud-service-cli project team welcomes contributions from the community. Before you start working with horizon-cloud-service-cli, please read and sign our Contributor License Agreement [CLA](https://cla.vmware.com/cla/1/preview). If you wish to contribute code and you have not signed our CLA, our bot will prompt you to do so when you open a Pull Request. For any questions about the CLA process, please refer to our [FAQ]([https://cla.vmware.com/faq](https://cla.vmware.com/faq)).
```

### Comparing `hcs-cli-0.1.48/doc/az-cheatsheet.md` & `hcs-cli-0.1.50/doc/az-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/doc/dev-setup.md` & `hcs-cli-0.1.50/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.50/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.50/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.50/hcs_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.48
+Version: 0.1.50
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -90,17 +90,16 @@
 hcs profile use
 ```
 
 
 ## Documentation
 
 * [HCS CLI Cheatsheet](doc/hcs-cli-cheatsheet.md)
-
+* [HCS Plan, a resource manager for deployment](doc/hcs-plan.md)
 * [Development Setup](doc/dev-setup.md)
-
 * Based on [Context Programming](https://github.com/nanw1103/context-programming)
 
   
 ## Contributing
 
 The horizon-cloud-service-cli project team welcomes contributions from the community. Before you start working with horizon-cloud-service-cli, please read and sign our Contributor License Agreement [CLA](https://cla.vmware.com/cla/1/preview). If you wish to contribute code and you have not signed our CLA, our bot will prompt you to do so when you open a Pull Request. For any questions about the CLA process, please refer to our [FAQ]([https://cla.vmware.com/faq](https://cla.vmware.com/faq)).
```

### Comparing `hcs-cli-0.1.48/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.50/hcs_cli.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 .vscode/launch.json
 .vscode/settings.json
 doc/az-cheatsheet.md
 doc/dev-setup.md
 doc/get-csp-user-api-token.md
 doc/hcs-cli-cheatsheet.md
 doc/hcs-plan.md
+doc/images/hcs-plan-graph.svg
+doc/images/hcs-plan.png
 hcs_cli.egg-info/PKG-INFO
 hcs_cli.egg-info/SOURCES.txt
 hcs_cli.egg-info/dependency_links.txt
 hcs_cli.egg-info/entry_points.txt
 hcs_cli.egg-info/requires.txt
 hcs_cli.egg-info/top_level.txt
 payload/lcm/zero.json
@@ -42,14 +44,15 @@
 tests/vhcs/cli/cmds/plan/test_plan.py
 vhcs/__init__.py
 vhcs/__main__.py
 vhcs/cli/__init__.py
 vhcs/cli/main.py
 vhcs/cli/cmds/__init__.py
 vhcs/cli/cmds/login.py
+vhcs/cli/cmds/logout.py
 vhcs/cli/cmds/upgrade.py
 vhcs/cli/cmds/admin/__init__.py
 vhcs/cli/cmds/admin/ad/__init__.py
 vhcs/cli/cmds/admin/ad/delete.py
 vhcs/cli/cmds/admin/ad/get.py
 vhcs/cli/cmds/admin/ad/list.py
 vhcs/cli/cmds/admin/azure-infra/main.py
@@ -111,15 +114,15 @@
 vhcs/cli/cmds/pki/__init__.py
 vhcs/cli/cmds/pki/delete_org_cert.py
 vhcs/cli/cmds/pki/get_org_cert.py
 vhcs/cli/cmds/pki/get_root_ca.py
 vhcs/cli/cmds/pki/sign_resource_cert.py
 vhcs/cli/cmds/pki/test.py
 vhcs/cli/cmds/plan/__init__.py
-vhcs/cli/cmds/plan/deploy.py
+vhcs/cli/cmds/plan/apply.py
 vhcs/cli/cmds/plan/destroy.py
 vhcs/cli/cmds/plan/graph.py
 vhcs/cli/cmds/portal/__init__.py
 vhcs/cli/cmds/portal/entitlement/__init__.py
 vhcs/cli/cmds/portal/entitlement/delete.py
 vhcs/cli/cmds/portal/entitlement/get.py
 vhcs/cli/cmds/portal/entitlement/list.py
@@ -135,46 +138,36 @@
 vhcs/cli/cmds/portal/site/set-edge.py
 vhcs/cli/cmds/profile/__init__.py
 vhcs/cli/cmds/profile/init.py
 vhcs/cli/cmds/vmhub/__init__.py
 vhcs/cli/cmds/vmhub/otp/__init__.py
 vhcs/cli/cmds/vmhub/otp/redeem.py
 vhcs/cli/cmds/vmhub/otp/request.py
-vhcs/common/__init__.py
-vhcs/common/duration.py
-vhcs/common/job_view.py
-vhcs/common/logger.py
-vhcs/common/util.py
-vhcs/common/ctxp/README.md
-vhcs/common/ctxp/__init__.py
-vhcs/common/ctxp/_init.py
-vhcs/common/ctxp/cli_processor.py
-vhcs/common/ctxp/config.py
-vhcs/common/ctxp/context.py
-vhcs/common/ctxp/fstore.py
-vhcs/common/ctxp/init.py
-vhcs/common/ctxp/jsondot.py
-vhcs/common/ctxp/profile.py
-vhcs/common/ctxp/profile_store.py
-vhcs/common/ctxp/state.py
-vhcs/common/ctxp/util.py
-vhcs/common/ctxp/var_template.py
-vhcs/common/ctxp/built_in_cmds/__init__.py
-vhcs/common/ctxp/built_in_cmds/context.py
-vhcs/common/ctxp/built_in_cmds/profile.py
-vhcs/common/sglib/__init__.py
-vhcs/common/sglib/auth.py
-vhcs/common/sglib/cli_options.py
-vhcs/common/sglib/csp.py
-vhcs/common/sglib/ez_client.py
-vhcs/common/sglib/hcs_client.py
-vhcs/common/sglib/login_support.py
-vhcs/common/sglib/util.py
 vhcs/config/__init__.py
 vhcs/config/hcs-deployments.yaml
+vhcs/ctxp/README.md
+vhcs/ctxp/__init__.py
+vhcs/ctxp/_init.py
+vhcs/ctxp/cli_processor.py
+vhcs/ctxp/config.py
+vhcs/ctxp/context.py
+vhcs/ctxp/data_util.py
+vhcs/ctxp/duration.py
+vhcs/ctxp/fstore.py
+vhcs/ctxp/init.py
+vhcs/ctxp/jsondot.py
+vhcs/ctxp/logger.py
+vhcs/ctxp/profile.py
+vhcs/ctxp/profile_store.py
+vhcs/ctxp/state.py
+vhcs/ctxp/util.py
+vhcs/ctxp/var_template.py
+vhcs/ctxp/built_in_cmds/__init__.py
+vhcs/ctxp/built_in_cmds/context.py
+vhcs/ctxp/built_in_cmds/profile.py
 vhcs/plan/__init__.py
 vhcs/plan/actions.py
 vhcs/plan/base_provider.py
 vhcs/plan/context.py
 vhcs/plan/core.py
 vhcs/plan/dag.py
 vhcs/plan/helper.py
@@ -190,29 +183,28 @@
 vhcs/plan/provider/azure/public_ip.py
 vhcs/plan/provider/azure/resource_group.py
 vhcs/plan/provider/azure/subnet.py
 vhcs/plan/provider/azure/virtual_network.py
 vhcs/plan/provider/dev/__init__.py
 vhcs/plan/provider/dev/_prepare.py
 vhcs/plan/provider/dev/dummy.py
+vhcs/plan/provider/dev/fibonacci.py
 vhcs/plan/provider/hcs/__init__.py
 vhcs/plan/provider/hcs/_prepare.py
 vhcs/plan/provider/hcs/ad.py
 vhcs/plan/provider/hcs/edge.py
 vhcs/plan/provider/hcs/entitlement.py
 vhcs/plan/provider/hcs/identity_provider.py
 vhcs/plan/provider/hcs/image.py
-vhcs/plan/provider/hcs/launch_item.py
 vhcs/plan/provider/hcs/pool_group.py
 vhcs/plan/provider/hcs/pool_template.py
 vhcs/plan/provider/hcs/provider.py
 vhcs/plan/provider/hcs/site.py
 vhcs/plan/provider/hcs/uag.py
 vhcs/service/__init__.py
-vhcs/service/_util.py
 vhcs/service/admin/__init__.py
 vhcs/service/admin/ad.py
 vhcs/service/admin/azure_infra.py
 vhcs/service/admin/edge.py
 vhcs/service/admin/helper.py
 vhcs/service/admin/provider.py
 vhcs/service/admin/template.py
@@ -236,30 +228,40 @@
 vhcs/service/pki/certificate.py
 vhcs/service/portal/__init__.py
 vhcs/service/portal/entitlement.py
 vhcs/service/portal/pool.py
 vhcs/service/portal/site.py
 vhcs/service/vmhub/__init__.py
 vhcs/service/vmhub/otp.py
+vhcs/sglib/__init__.py
+vhcs/sglib/auth.py
+vhcs/sglib/cli_options.py
+vhcs/sglib/client_util.py
+vhcs/sglib/csp.py
+vhcs/sglib/ez_client.py
+vhcs/sglib/hcs_client.py
+vhcs/sglib/login_support.py
 vhcs/support/__init__.py
 vhcs/support/plan_util.py
 vhcs/support/profile.py
 vhcs/support/daas/__init__.py
 vhcs/support/daas/cidr_util.py
 vhcs/support/daas/helper.py
 vhcs/support/daas/infra.py
 vhcs/support/daas/infra_green.py
 vhcs/support/daas/infra_reuse.py
 vhcs/support/daas/template.py
-vhcs/support/daas/tenant_calc.py
+vhcs/support/daas/tenant_prep.py
+vhcs/support/daas/tenant_summary.py
 vhcs/support/daas/templates/v1/infra-green.blueprint.yml
 vhcs/support/daas/templates/v1/infra-green.vars.yml
 vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml
 vhcs/support/daas/templates/v1/infra-reuse.vars.yml
 vhcs/support/daas/templates/v1/tenant.blueprint.yml
 vhcs/support/daas/templates/v1/tenant.vars.yml
 vhcs/util/__init__.py
 vhcs/util/check_license.py
 vhcs/util/duration.py
+vhcs/util/job_view.py
 vhcs/util/pki_util.py
 vhcs/util/query_util.py
 vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.48/payload/lcm/zero.json` & `hcs-cli-0.1.50/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/pyproject.toml` & `hcs-cli-0.1.50/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/setup.py` & `hcs-cli-0.1.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.48"
+VERSION = "0.1.50"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.48/tests/conftest.py` & `hcs-cli-0.1.50/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/tests/test_utils.py` & `hcs-cli-0.1.50/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,18 +56,24 @@
     def NON_EMPTY_JSON(cls, data):
         if data is None or len(data) == 0:
             raise Exception("Expect non-empty json, but got empty.")
         d = json.loads(data)
         if len(d) == 0:
             raise Exception("Expect non-empty json, but got empty dict.")
 
-    def verify(self, cmd: str, expected_data: any, expected_return_code: int = 0, expect_stderr_empty: bool = True, stdin_payload: str = None):
+    def verify(
+        self,
+        cmd: str,
+        expected_data: any,
+        expected_return_code: int = 0,
+        expect_stderr_empty: bool = True,
+        stdin_payload: str = None,
+    ):
         stdout, stderr, returncode = _run(cmd, stdin_payload)
         try:
-
             # verify return code
             self.assertEqual(returncode, expected_return_code, "Invalid return code.")
 
             # verify stderr
             actual_stderr_empty = stderr is None or len(stderr) == 0
             self.assertEqual(
                 expect_stderr_empty,
@@ -88,10 +94,10 @@
                     data = json.loads(stdout)
                     self.assertEqual(expected_data, data)
             else:
                 raise Exception(
                     f"type of expected_data must be dict, string, or function. Current type: {t}. This is an error of the test case."
                 )
         except Exception:
-            print('<DUMP STDOUT>', stdout)
-            print('<DUMP STDERR>', stderr)
+            print("<DUMP STDOUT>", stdout)
+            print("<DUMP STDERR>", stderr)
             raise
```

### Comparing `hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.50/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.50/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.50/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.50/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/__main__.py` & `hcs-cli-0.1.50/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,21 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import portal
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
-def delete(id: str, org: str, **kwargs):
-    """Delete Active Directory record by ID"""
-
+def get(id: str, org: str):
+    """Get entitlement by ID"""
     org_id = cli.get_org_id(org)
-
-    ret = admin.ad.delete(id, org_id)
-    if not ret:
-        return '', 1
-    return ret
-    
+    ret = portal.entitlement.get(id, org_id)
+    if ret:
+        return ret
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/get.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 def get(id: str, org: str):
-    """Get Active Directory record by ID"""
-    ret = admin.ad.get(id, org_id = cli.get_org_id(org))
+    """Get UAG by ID"""
+    ret = admin.uag.get(id, org_id=cli.get_org_id(org))
     if ret:
         return ret
-    return '', 1
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import portal
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 def list(org: str, **kwargs):
-    """List Active Directory records"""
-    return admin.ad.list(org_id = cli.get_org_id(org), **kwargs)
-
+    """List entitlements"""
+    org_id = cli.get_org_id(org)
+    return portal.entitlement.list(org_id, **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,22 +12,18 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 import click
 from vhcs.service.admin import azure_infra
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @cli.limit
 @cli.sort
-@click.option(
-    "--provider", "-p", 
-    type=str,
-    required=True, 
-    help="Specify the provider instance id")
+@click.option("--provider", "-p", type=str, required=True, help="Specify the provider instance id")
 def get_compute_vm_skus(provider: str, **kwargs):
     """List compute VM SKUs"""
     return azure_infra.get_compute_vm_skus(provider, **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,67 +12,66 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import httpx
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 @cli.wait
-@click.option("--delete-all/--delete-edge-only", type=bool, default=True, help="Specify whether to delete associated resources, if any.")
+@click.option(
+    "--delete-all/--delete-edge-only",
+    type=bool,
+    default=True,
+    help="Specify whether to delete associated resources, if any.",
+)
 def delete(id: str, org: str, wait: str, delete_all: bool):
     """Delete edge by ID"""
 
     org_id = cli.get_org_id(org)
 
     ret = admin.edge.get(id, org_id)
     if not ret:
-        return '', 1
-    
+        return "", 1
+
     if delete_all:
-        uags = _get_uags_by_edge(id, org_id)
+        uags = admin.helper.get_uags_by_edge(id, org_id)
         for u in uags:
-            _start_deleting_uag(u['id'], org_id)
+            _start_deleting_uag(u["id"], org_id)
         for u in uags:
-            admin.uag.wait_for_deleted(u['id'], org_id, timeout = '10m')
+            admin.uag.wait_for_deleted(u["id"], org_id, timeout="10m")
 
     ret = admin.edge.delete(id, org_id)
     if not ret:
-        return '', 1
-    
+        return "", 1
+
     acceptable_status = [
-        'DELETE_PENDING',
-        'DELETED',
-        'FORCE_DELETE_PENDING',
-        'DELETING',
-        'FORCE_DELETING',
+        "DELETE_PENDING",
+        "DELETED",
+        "FORCE_DELETE_PENDING",
+        "DELETING",
+        "FORCE_DELETING",
     ]
-    accepted = ret['status'] in acceptable_status
+    accepted = ret["status"] in acceptable_status
     if not accepted:
         return ret, 1
-    
-    if wait == '0':
+
+    if wait == "0":
         return ret
-    
+
     admin.edge.wait_for_deleted(id, org_id, wait)
-    
+
+
 def _start_deleting_uag(uag_id: str, org_id: str):
     try:
         admin.uag.delete(uag_id, org_id)
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 409:
-            if e.response.text.find('UAG_DEPLOYMENT_DELETE_ALREADY_IN_PROGRESS') > 0:
+            if e.response.text.find("UAG_DEPLOYMENT_DELETE_ALREADY_IN_PROGRESS") > 0:
                 return
         raise
 
-def _get_uags_by_edge(edge_id: str, org_id: str):
-    uags = admin.uag.list(org_id)
-    ret = []
-    for u in uags:
-        if u['edgeDeploymentId'] == edge_id:
-            ret.append(u)
-    return ret
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 def get(id: str, org: str):
     """Get edge by ID"""
-    ret = admin.edge.get(id, org_id = cli.get_org_id(org))
+    ret = admin.edge.get(id, org_id=cli.get_org_id(org))
     if ret:
         return ret
-    return '', 1
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/edge/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @cli.search
 def list(org: str, **kwargs):
     """List edges"""
     org_id = cli.get_org_id(org)
     return admin.edge.list(org_id, **kwargs)
-
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/create.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-from vhcs.common.ctxp import panic
-import vhcs.common.sglib.cli_options as cli
+from vhcs.ctxp import panic
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @click.option(
     "--label",
     "-l",
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @click.option("--label", type=str, required=False, default="azure")
 @cli.org_id
 def delete(label: str, id: str, org: str):
     """Delete provider by ID"""
     ret = admin.provider.delete(label, id, org_id=cli.get_org_id(org), force=True)
     if ret:
-        return ''
-    return '', 1
+        return ""
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @click.option("--label", type=str, required=False, default="azure")
 @cli.org_id
 def get(label: str, id: str, org: str, **kwargs):
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/provider/list.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,28 +12,25 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @cli.limit
 @cli.sort
 @cli.search
 @click.option(
-    "--label", 
+    "--label",
     type=click.Choice(["azure", "vsphere"]),
-    required=False, 
-    default="azure", 
-    help="Specify the provider label")
+    required=False,
+    default="azure",
+    help="Specify the provider label",
+)
 def list(org: str, label: str, **kwargs):
     """List provider instances"""
-    return admin.provider.list(
-        org_id = cli.get_org_id(org),
-        label=label,
-        **kwargs
-    )
+    return admin.provider.list(org_id=cli.get_org_id(org), label=label, **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 @cli.wait
 def delete(id: str, org: str, wait: str):
     """Delete template by ID"""
 
     org_id = cli.get_org_id(org)
 
     ret = admin.template.get(id, org_id)
     if not ret:
-        return '', 1
-    
+        return "", 1
+
     ret = admin.template.delete(id, org_id)
-    
-    if wait == '0':
+
+    if wait == "0":
         return ret
-    
+
     admin.template.wait_for_deleted(id, org_id, wait)
-
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/inventory/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import inventory
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
+@click.argument("template", type=str, required=True)
 @cli.org_id
-def get(id: str, org: str):
-    """Get template by ID"""
-    ret = admin.template.get(id, org_id= cli.get_org_id(org))
+def list(template: str, org: str):
+    """List template VMs"""
+    ret = inventory.list(template, cli.get_org_id(org))
     if ret:
         return ret
-    return '', 1
+    return ret, 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @click.option("--limit", "-l", type=int, required=False, default=20, help="Optionally, specify cloud provider type.")
 @click.option("--brokerable-only", type=bool, required=False, default=False)
 @click.option("--expanded", type=bool, required=False, default=False)
@@ -32,16 +32,16 @@
 @click.option("--template-search", type=str, required=False, help="Search expression for selection of templates")
 @click.option(
     "--sort",
     type=str,
     required=False,
     help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
 )
-def list(org: str, 
-    limit: int, brokerable_only: bool, expanded: bool, reported_search: str, template_search: str, sort: str
+def list(
+    org: str, limit: int, brokerable_only: bool, expanded: bool, reported_search: str, template_search: str, sort: str
 ):
     """List templates"""
     org_id = cli.get_org_id(org)
     return admin.template.list(
         org_id=org_id,
         limit=limit,
         borkerable_only=brokerable_only,
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/vm/get.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
-
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument('template-id', type=str, required=True)
-@click.argument('vm-id', type=str, required=True)
+@click.argument("template-id", type=str, required=True)
+@click.argument("vm-id", type=str, required=True)
 @cli.org_id
 def get(template_id: str, vm_id: str, org: str, **kwargs):
     """Get template VM"""
     return admin.template.get_vm(template_id, vm_id, org_id=cli.get_org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import portal
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument('template-id', type=str, required=True)
+@click.argument("id", type=str, required=True)
 @cli.org_id
-def list(template_id: str, org: str, **kwargs):
-    """List template VMs"""
-    return admin.template.list_vms(template_id, org_id=cli.org_id(org), **kwargs)
+def delete(id: str, org: str):
+    """Delete a site."""
+    org_id = cli.get_org_id(org)
+    ret = portal.site.delete(id, org_id)
+    return ret
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/delete.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import httpx
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 @cli.wait
 def delete(id: str, org: str, wait: str):
     """Delete UAG by ID"""
 
-    org_id=cli.get_org_id(org)
+    org_id = cli.get_org_id(org)
     try:
         ret = admin.uag.delete(id, org_id)
         if not ret:
-            return '', 1
+            return "", 1
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 409:
             pass
         else:
             raise
-    if wait == '0':
+    if wait == "0":
         return ret
     admin.uag.wait_for_deleted(id, org_id, wait)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 def get(id: str, org: str):
-    """Get UAG by ID"""
-    ret = admin.uag.get(id, org_id=cli.get_org_id(org))
+    """Get template by ID"""
+    ret = admin.template.get(id, org_id=cli.get_org_id(org))
     if ret:
         return ret
-    return '', 1
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/get.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import admin
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
+@click.argument("id", type=str, required=True)
 @cli.org_id
-@cli.search
-def list(**kwargs):
-    """List UAG deployments"""
-    return admin.uag.list(org_id=cli.get_org_id(kwargs['org']), **kwargs)
-
+def get(id: str, org: str):
+    """Get Active Directory record by ID"""
+    ret = admin.ad.get(id, org_id=cli.get_org_id(org))
+    if ret:
+        return ret
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/auth/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/get_org_idp_map.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/org/detail/get.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import auth
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service.org_service import details
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
-def get_org_idp_map(org: str):
-    """Get org-idp-map by ID"""
+def get(org: str):
+    """Get org details"""
     org_id = cli.get_org_id(org)
-    ret = auth.admin.get_org_idp_map(org_id=org_id)
+    ret = details.get(org_id)
     if ret:
         return ret
     return ret, 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import vhcs.common.ctxp as ctxp
+import vhcs.ctxp as ctxp
 from vhcs.support.daas import infra
 
+
 @click.command()
 def get():
     """Get the shared infrastructure config."""
     return infra.get()
 
+
 @click.command()
 def file():
     """Get the infrastructure config file path."""
     return infra.file()
 
+
 @click.command()
 def edit():
     """Launch text editor to edit the config file directly"""
     file = infra.file()
     ctxp.util.launch_text_editor(file)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,159 +10,186 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import vhcs.common.ctxp as ctxp
-from vhcs.common.ctxp import choose
+import vhcs.ctxp as ctxp
+from vhcs.ctxp import choose
 from vhcs.plan.provider.azure import _az_facade as az
 from vhcs.support.daas import infra
 from vhcs.service import admin
 from vhcs.support.daas import infra, helper, cidr_util
 
-file_name = '.plan.yml'
+file_name = ".plan.yml"
+
 
 @click.command()
 def plan():
     """Interactive setup for shared infrastructure."""
 
-    name = click.prompt("Name of the infrastructure", default="starter")
-    modes = ['Create default infrastructure (automatic)', 'Reuse existing infrastructure (manual)']
+    name = _prompt("Name of the infrastructure", default="starter")
+    modes = ["Create default infrastructure (automatic)", "Reuse existing infrastructure (manual)"]
     mode = choose("Name of the infrastructure:", modes, selected=modes[0])
 
     if mode == modes[0]:
         _create_default_infra(name)
     else:
         _reuse_existing_infra(name)
-    
+
+
+def _prompt(text: str, default=None, is_secret: bool = False):
+    t = click.prompt(text=text, default=default, hide_input=is_secret, show_default=not is_secret)
+    return t.strip()
+
+
 def _create_default_infra(name):
     def collect_information(data):
-        vars = data['vars']
-        org_id = vars['orgId']
+        vars = data["vars"]
+        org_id = vars["orgId"]
         _select_region(vars)
         _select_provider(vars, org_id)
         _select_managed_identity(vars)
-        _input_vnet_cidr(vars['network'])
-        _config_desktop_defaults(vars['desktop'])
+        _input_vnet_cidr(vars["network"])
+        _config_desktop_defaults(vars["desktop"])
         infra.set(data)
 
-    return helper.prepare_plan_file(name, 'v1/infra-green.blueprint.yml', collect_information)
+    return helper.prepare_plan_file(name, "v1/infra-green.blueprint.yml", collect_information)
+
 
 def _reuse_existing_infra(name):
     def collect_information(data):
-        vars = data['vars']
-        org_id = vars['orgId']
+        vars = data["vars"]
+        org_id = vars["orgId"]
         _select_region(vars)
         _select_provider(vars, org_id)
         _select_managed_identity(vars)
-        _select_vnet(vars['network'])
-        _config_desktop_defaults(vars['desktop'])
+        _select_vnet(vars["network"])
+        _config_desktop_defaults(vars["desktop"])
         infra.set(data)
 
-    return helper.prepare_plan_file(name, 'v1/infra-reuse.blueprint.yml', collect_information)
+    return helper.prepare_plan_file(name, "v1/infra-reuse.blueprint.yml", collect_information)
+
 
 def _input_vnet_cidr(network):
-    cidr = click.prompt("vNet CIDR (/16):", default=network['cidr'] or "10.0.0.0/16")
-    network['cidr'] = cidr
+    cidr: str = None
+    while True:
+        cidr = _prompt("vNet CIDR (/16):", default=network["cidr"] or "10.0.0.0/16")
+        cidr = cidr.strip()
+        reserved_cidrs = ["169.254.0.0/16", "172.30.0.0/16", "172.31.0.0/16", "192.0.2.0/24"]
+        conflict, conflict_to = cidr_util.overlaps([cidr], reserved_cidrs)
+        if conflict:
+            click.echo("The specified CIDR conflicts to reserved CIDR " + conflict_to)
+        else:
+            break
+    network["cidr"] = cidr
+
 
 def _select_region(vars):
     locations = az.locations()
     selected = None
     for l in locations:
-        if l['name'] == 'eastus':
+        if l["name"] == "eastus":
             selected = l
             break
-    fn_get_text = lambda l: l['regionalDisplayName'] + f" ({l['name']})"
+    fn_get_text = lambda l: l["regionalDisplayName"] + f" ({l['name']})"
     region = choose("Select location:", locations, fn_get_text, selected)
-    vars['region'] = region['name']
+    vars["region"] = region["name"]
+
 
 def _select_managed_identity(vars):
     identities = list(az.managed_identity_client().user_assigned_identities.list_by_subscription())
     fn_get_text = lambda i: i.name
     selected = choose("Select managed identity:", identities, fn_get_text)
-    vars['edge']['managedIdentityId'] = selected.id
+    vars["edge"]["managedIdentityId"] = selected.id
+
 
 def _select_provider(vars: dict, org_id: str):
-    providers = admin.provider.list('azure', org_id)
-    region = vars['region']
-    filter_by_region = lambda p: p['providerDetails']['data']['region'] == region
+    providers = admin.provider.list("azure", org_id)
+    region = vars["region"]
+    filter_by_region = lambda p: p["providerDetails"]["data"]["region"] == region
     providers = list(filter(filter_by_region, providers))
     if providers:
+
         def _is_create_new(p):
             return isinstance(p, str)
 
         def fn_provider_text(p):
             if _is_create_new(p):
                 return p
             return f"{p['providerDetails']['data']['region']}, {p['name']}/{p['id']}"
 
         providers.append("<Create New Provider>")
         p = choose("Select region and provider", providers, fn_provider_text)
         if not p:
             return
         if not _is_create_new(p):
-            vars['provider']['id'] = p['id']
-            subscription_id = p['providerDetails']['data']['subscriptionId']
-            vars['provider']['subscriptionId'] = subscription_id
-            del vars['newProvider']
+            vars["provider"]["id"] = p["id"]
+            subscription_id = p["providerDetails"]["data"]["subscriptionId"]
+            vars["provider"]["subscriptionId"] = subscription_id
+            del vars["newProvider"]
             az.set_subscription(subscription_id)
             return p
     else:
         click.echo(f"No provider configured for region {region}. Need to create a new provider.")
-    _input_azure_sp(vars['newProvider'])
-    
+    del vars["provider"]["id"]
+    _input_azure_sp(vars["newProvider"])
+    vars["provider"]["subscriptionId"] = vars["newProvider"]["subscriptionId"]
+
 
 def _input_azure_sp(data):
-    data['subscriptionId'] = click.prompt("Azure subscription ID", default=data['subscriptionId'])
-    data['region'] = click.prompt("Azure Region", default=data['region'])
-    data['directoryId'] = click.prompt("Azure Directory ID", default=data['directoryId'])
-    data['applicationId'] = click.prompt("Azure service principle application ID", default=data['applicationId'])
-    data['applicationKey'] = click.prompt("Azure service principle application key", default=data['applicationKey'])
-
-    ret = az.login(data['applicationId'], data['applicationKey'], data['directoryId'])
-    print(ret)
-    ret = az.set_subscription(data['subscriptionId'])
-    print(ret)
-    
+    data["subscriptionId"] = _prompt("Azure subscription ID", default=data["subscriptionId"])
+    data["directoryId"] = _prompt("Azure Directory ID", default=data["directoryId"])
+    data["applicationId"] = _prompt("Azure service principle application ID", default=data["applicationId"])
+    data["applicationKey"] = _prompt(
+        "Azure service principle application key", default=data["applicationKey"], is_secret=True
+    )
+
+    az.login(data["applicationId"], data["applicationKey"], data["directoryId"])
+    az.set_subscription(data["subscriptionId"])
+
+
 def _select_vnet(data):
     vnets = az.network.vnet.list()
     fn_get_text = lambda vnet: f"{vnet['name']} ({','.join(vnet['addressSpace']['addressPrefixes'])})"
     vnet = choose("Select vNet:", vnets, fn_get_text)
-    data['vNetId'] = vnet['id']
-    
+    data["vNetId"] = vnet["id"]
+
     while True:
-        tenant_cidrs = ctxp.util.input_array("Tenant CIDRs", default=data['tenantCIDRs'])
+        tenant_cidrs = ctxp.util.input_array("Tenant CIDRs", default=data["tenantCIDRs"])
         if not tenant_cidrs:
             return
-        err = _validate_cidr(tenant_cidrs, vnet['addressSpace']['addressPrefixes'])
+        err = _validate_cidr(tenant_cidrs, vnet["addressSpace"]["addressPrefixes"])
         if err:
             click.echo(err)
         else:
             break
-    data['tenantCIDRs'] = tenant_cidrs
+    data["tenantCIDRs"] = tenant_cidrs
+
 
 def _validate_cidr(input, limit):
     is_subnet, problem = cidr_util.subnets_of(input, limit)
     if not is_subnet:
         return f"The specified CIDR {problem} is not subnet of vNet address spaces: {limit}"
     reserved_cidrs = [
-        "172.17.0.0/26",    #docker bridge
-		"192.170.0.0/21",   #podCidr
-		"192.169.0.0/27",   #serviceCidr
+        "172.17.0.0/26",  # docker bridge
+        "192.170.0.0/21",  # podCidr
+        "192.169.0.0/27",  # serviceCidr
     ]
     overlap, problem = cidr_util.overlaps(input, reserved_cidrs)
     if overlap:
         return f"The specified address {problem} conflict to reserved address spaces: {reserved_cidrs}"
 
+
 def _config_desktop_defaults(data):
     groups = az.aad.group.list()
-    fn_get_text = lambda g: g['displayName']
+    fn_get_text = lambda g: g["displayName"]
     prev = None
     for g in groups:
-        if g['displayName'] == data['userGroup']:
+        if g["displayName"] == data["userGroup"]:
             prev = g
-    click.echo("To allow user login, they must have either 'Virtual Machine User Login' role or 'Virtual Machine Administrator Login' role.")
+    click.echo(
+        "To allow user login, they must have either 'Virtual Machine User Login' role or 'Virtual Machine Administrator Login' role."
+    )
     selected = choose("Select a user group with one of the above roles:", groups, fn_get_text, selected=prev)
-    data['userGroup'] = selected['displayName']
-    
+    data["userGroup"] = selected["displayName"]
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,72 +10,89 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
+import re
 from vhcs.service import admin, ims, portal
-from vhcs.common.ctxp import choose, util as cli_util
-from vhcs.common.sglib.cli_options import get_org_id
+from vhcs.ctxp import choose, util as cli_util
+from vhcs.sglib.cli_options import get_org_id
 from vhcs.support.daas import infra, helper
 
 _context = {}
 
+
 @click.command()
-@click.argument("name", type=str, required=True)
-def plan(name: str):
+def plan():
+    deployment_id = _input_tenant_deployment_id()
     """Interactive command to request a DaaS tenant"""
-    return helper.prepare_plan_file(name, 'v1/tenant.blueprint.yml', _collect_info)
+    return helper.prepare_plan_file(deployment_id, "v1/tenant.blueprint.yml", _collect_info)
+
+
+def _input_tenant_deployment_id():
+    pattern = re.compile("^[a-zA-Z0-9][a-zA-Z0-9_\-]*$")
+    while True:
+        deployment_id: str = click.prompt("Tenant unique deployment ID", "tenant1")
+        deployment_id = deployment_id.strip()
+        # if deployment_id.isidentifier():
+        if pattern.match(deployment_id):
+            break
+        click.echo("Invalid deployment ID. Use only alphabetics, numbers, -, or _.")
+    return deployment_id
+
 
 def _collect_info(data):
-    #_fill_info_from_infra()
-    vars = data['vars']
+    # _fill_info_from_infra()
+    vars = data["vars"]
     _select_edge(vars)
     _config_desktop(vars)
     _input_user_emails(vars)
 
+
 def _select_edge(vars):
-    org_id = vars['orgId']
+    org_id = vars["orgId"]
     edges = admin.edge.list(org_id)
     titan_lite_infra = []
-    edge_id = vars['edgeId']
+    edge_id = vars["edgeId"]
     prev_selected = None
     for s in edges:
-        name = s['name']
-        if name.startswith('titanlite-'):
+        name = s["name"]
+        if name.startswith("titanlite-"):
             titan_lite_infra.append(s)
-            if edge_id == s['id']:
+            if edge_id == s["id"]:
                 prev_selected = s
 
     fn_get_text = lambda s: f"{s['name']} ({s['hdc']['vmHub']['name']})"
     selected_edge = choose("Select edge", titan_lite_infra, fn_get_text, prev_selected)
-    vars['edgeId'] = selected_edge['id']
-    _context['provider_instance_id'] = selected_edge['providerInstanceId']
+    vars["edgeId"] = selected_edge["id"]
+    _context["provider_instance_id"] = selected_edge["providerInstanceId"]
 
 
 def _config_desktop(vars: dict):
-    org_id = vars['orgId']
+    org_id = vars["orgId"]
+
     def _select_image_and_vm_sku():
-        images = ims.helper.get_images_by_provider_instance_with_asset_details(_context['provider_instance_id'], org_id)
+        images = ims.helper.get_images_by_provider_instance_with_asset_details(_context["provider_instance_id"], org_id)
         fn_get_text = lambda d: f"{d['name']}: {d['description']}"
         prev_selected_image = None
-        if vars['desktop']['streamId']:
+        if vars["desktop"]["streamId"]:
             for i in images:
-                if i['id'] == vars['desktop']['streamId']:
+                if i["id"] == vars["desktop"]["streamId"]:
                     prev_selected_image = i
                     break
         selected_image = choose("Select image:", images, fn_get_text, selected=prev_selected_image)
-        vars['desktop']['streamId'] = selected_image['id']
+        vars["desktop"]["streamId"] = selected_image["id"]
 
         fn_get_text = lambda m: f"{m['name']}"
-        selected_marker = choose("Select marker:", selected_image['markers'], fn_get_text)
-        vars['desktop']['markerId'] = selected_marker['id']
+        selected_marker = choose("Select marker:", selected_image["markers"], fn_get_text)
+        vars["desktop"]["markerId"] = selected_marker["id"]
 
-        image_asset_details = selected_image['_assetDetails']['data']
+        image_asset_details = selected_image["_assetDetails"]["data"]
 
         # search = f"capabilities.HyperVGenerations $in {image_asset_details['generationType']}"
         # vm_skus = admin.azure_infra.get_compute_vm_skus(data['provider']['id'], limit=200, search=search)
         # prev_selected_vm_sku = None
         # if data['desktop']['vmSkuName']:
         #     selected_vm_sku_name = data['desktop']['vmSkuName']
         # else:
@@ -86,18 +103,19 @@
         #             prev_selected_vm_sku = sku
         #             break
 
         # fn_get_text = lambda d: f"{d['data']['name']} (CPU: {d['data']['capabilities']['vCPUs']}, RAM: {d['data']['capabilities']['MemoryGB']})"
 
         # selected = choose("Select VM size:", vm_skus, fn_get_text, selected=prev_selected_vm_sku)
         # data['desktop']['vmSkuName'] = selected['data']['name']
-        vars['desktop']['vmSkuName'] = image_asset_details['vmSize']
+        vars["desktop"]["vmSkuName"] = image_asset_details["vmSize"]
 
     def _select_desktop_type():
-        types = ['FLOATING', 'MULTI_SESSION']
-        vars['desktop']['templateType'] = choose("Desktop type:", types)
+        types = ["FLOATING", "MULTI_SESSION"]
+        vars["desktop"]["templateType"] = choose("Desktop type:", types)
 
     _select_image_and_vm_sku()
     _select_desktop_type()
 
+
 def _input_user_emails(data):
-    data['userEmails'] = cli_util.input_array("User emails", default=data['userEmails'])
+    data["userEmails"] = cli_util.input_array("User emails", default=data["userEmails"])
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import ims
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("ids", type=str, required=True, nargs=-1)
 @cli.org_id
 @cli.wait
 def delete(ids: list[str], org: str, wait: str, **kwargs):
     """Delete an image by ID"""
 
     org_id = cli.get_org_id(org)
-    ims.helper.delete_images(ids, org_id, wait)
+    ims.helper.delete_images(ids, org_id, wait)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import ims
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str)
 @cli.org_id
 @cli.search
 def get(id: str, org: str, **kwargs):
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import ims
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--limit", "-l", type=int, required=False, default=20)
 @cli.org_id
 @cli.search
 def list(org: str, **kwargs):
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/list_copies.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import ims
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--limit", "-l", type=int, default=20)
 @click.option("--include-catalog-details/--no-catalog-details", type=bool, default=True)
 @cli.org_id
 def list_copies(org: str, **kwargs):
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import httpx
 from vhcs.service import ims
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--image", "-i", type=str, required=False, help="Image ID")
 @click.argument("id", type=str, required=True)
 @cli.org_id
 @cli.wait
@@ -47,10 +47,10 @@
         if not ret:
             return
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 422:
             pass
         else:
             raise
-    if wait == '0':
+    if wait == "0":
         return ret
     v.wait_for_deleted(version_id)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import ims
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--image", "-i", type=str, required=False, help="Image ID")
 @click.argument("id", type=str, required=True)
 @cli.org_id
 def get(image: str, id: str, org: str, **kwargs):
@@ -28,12 +28,12 @@
     if image:
         ret = ims.version(image, org_id).get(id)
         if ret:
             return ret
     else:
         images = ims.images.list(org_id)
         for i in images:
-            image_id = i['id']
+            image_id = i["id"]
             ret = ims.version(image_id, org_id).get(id)
             if ret:
                 return ret
-    return '', 1
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/ims/version/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import ims
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--image", "-i", type=str, required=False, help="Image ID")
 @cli.org_id
 def list(image: str, org: str, **kwargs):
     """List image versions"""
 
     org_id = cli.get_org_id(org)
     if image:
         return ims.version(image, org_id).list(**kwargs)
-    
+
     images = ims.images.list(org_id)
     ret = []
     for i in images:
-        image_id = i['id']
+        image_id = i["id"]
         ret.extend(ims.version(image_id, org_id).list())
     return ret
-
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/inventory/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/inventory/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/inventory/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import inventory
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--template", "-t", type=str, required=True, help="Template id")
 @click.option("--vm", "-v", type=str, required=True, help="VM id")
 @cli.org_id
 def get(template: str, vm: str, org: str):
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/inventory/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import inventory
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import portal
+import vhcs.sglib.cli_options as cli
+
 
 @click.command()
-@click.argument("template", type=str, required=True)
+@click.argument("id", type=str, required=True)
 @cli.org_id
-def list(template: str, org: str):
-    """List template VMs"""
-    ret = inventory.list(template, cli.get_org_id(org))
-    if ret:
-        return ret
-    return ret, 1
+def delete(id: str, org: str):
+    """Delete pool by ID"""
+    org_id = cli.get_org_id(org)
+    ret = portal.pool.delete(id, org_id)
+    return ret
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.lcm import provider
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
 def list(org: str, type: str):
     """List providers"""
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 limitations under the License.
 """
 
 import sys
 import json
 import random
 import click
-import vhcs.common.duration as duration
+import vhcs.ctxp.duration as duration
 import vhcs.service.lcm as lcm
-import vhcs.common.sglib.cli_options as cli
-from vhcs.common.ctxp.util import option_id_only
+import vhcs.sglib.cli_options as cli
+from vhcs.ctxp.util import option_id_only
 
 
 @click.command()
 @click.option(
     "--file",
     "-f",
     type=click.File("rt"),
@@ -51,15 +51,15 @@
     template["orgId"] = org_id
 
     provider = _create_zerocloud_provider(org_id)
     template["provider"]["providerAccessId"] = provider["id"]
 
     ret = lcm.template.create(template)
 
-    if wait != '0':
+    if wait != "0":
         template = lcm.template.wait(id, duration.to_seconds(wait))
     if id_only:
         return ret.get("id")
     return ret
 
 
 def _rand_id(n: int):
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.lcm import template
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 @click.option(
     "--force/--safe", default=True, help="In 'force' mode, the template deletion will continue and ignore any error."
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.lcm import template
-import vhcs.common.sglib.cli_options as cli
-from vhcs.common.ctxp.util import option_id_only
+import vhcs.sglib.cli_options as cli
+from vhcs.ctxp.util import option_id_only
 
 
 @click.command("list")
 @click.option(
     "--limit", "-l", type=int, required=False, default=20, help="Optionally, specify the number of records to return."
 )
 @cli.org_id
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import vhcs.common.sglib as sglib
-import vhcs.common.ctxp as ctxp
-from vhcs.common.sglib import login_support as login_support
+import vhcs.sglib as sglib
+import vhcs.ctxp as ctxp
+from vhcs.sglib import login_support as login_support
 from vhcs.support import profile as profile_support
 
 # Login use cases:
 
 # 1. Login scenario
 # 1.1. As a new user, I want to login.
 # 1.2. As a returning user, I want to re-login use the same auth method
@@ -34,25 +34,43 @@
 # 2.2. As a user, I want to login with client id/secret
 # 2.2. As a user, I want to login with bearer
 
 # 3. Information
 # 3.1. As a user, I want to get the login details (e.g. my permissions)
 # 3.2. As a user, I want to get the access token, so I can use it with REST API.
 
+
 @click.command()
-@click.option("--org", type=str, required=False, help="The CSP organization to login. If not specified, the user's default organization will be used.")
+@click.option(
+    "--org",
+    type=str,
+    required=False,
+    help="The CSP organization to login. If not specified, the user's default organization will be used.",
+)
 @click.option("--api-token", type=str, required=False, help="Login with a user CSP API token.")
 @click.option("--client-id", type=str, required=False, help="Login with OAuth client ID/secret.")
 @click.option("--client-secret", type=str, required=False, help="The OAuth client secret, used with --client-id.")
-@click.option("--browser/--auto", type=bool, default=False, help="Login with browser and remove other configured credentials.")
-@click.option("--details/--no-details", "-d", default=False, help="If specified, return the detailed information about the authentication information, otherwise return only the access token.")
-@click.option("--refresh/--no-refresh", "-r", default=False, help="Used only in non-interactive mode. If specified, forcefully refresh the cached access token.")
+@click.option(
+    "--browser/--auto", type=bool, default=False, help="Login with browser and remove other configured credentials."
+)
+@click.option(
+    "--details/--no-details",
+    "-d",
+    default=False,
+    help="If specified, return the detailed information about the authentication information, otherwise return only the access token.",
+)
+@click.option(
+    "--refresh/--no-refresh",
+    "-r",
+    default=False,
+    help="Used only in non-interactive mode. If specified, forcefully refresh the cached access token.",
+)
 def login(org: str, api_token: str, client_id: str, client_secret: str, browser: bool, details: bool, refresh: bool):
-    """Login Horizon Cloud Service. 
-    
+    """Login Horizon Cloud Service.
+
     This command works with the current profile and will update the current profile. If no token is specified, a browser will be launched to login interactively.
 
     \b
     Examples:
         1. Login with configured credentials, otherwise do an interactive login using browser:
             hcs login
         2. Get login details:
@@ -62,27 +80,28 @@
         4. Login with OAuth client id/secret:
             hcs login --client-id <oauth-client-id> --client-secret <oauth-client-secret>
     """
 
     current_profile = _ensure_current_profile()
     csp = current_profile.csp
 
-    err = _validate_auth_method(org=org, api_token=api_token, client_id=client_id, client_secret=client_secret, browser=browser)
+    err = _validate_auth_method(
+        org=org, api_token=api_token, client_id=client_id, client_secret=client_secret, browser=browser
+    )
     if err:
         return err
-    
+
     # if org is specified
     if org:
         # update the profile
         csp.orgId = org
-    else:   # no org id is specified.
+    else:  # no org id is specified.
         # try using the org_id from profile
         org = csp.orgId
 
-
     if api_token:
         _clear_credentials(csp)
         csp.apiToken = api_token
     elif client_id:
         _clear_credentials(csp)
         csp.clientId = client_id
         csp.clientSecret = client_secret
@@ -92,77 +111,83 @@
         # auto detect mode.
         pass
 
     interactive = not csp.apiToken and not csp.clientId
 
     # If this is interactive login, it's not ready on production yet. Raise error
     if interactive and not login_support.identify_client_id(csp.url):
-        return ctxp.error(f"The interactive login on the specified stack is not yet available. Try a different authentication method.")
+        return ctxp.error(
+            f"The interactive login on the specified stack is not yet available. Try a different authentication method."
+        )
 
     oauth_token = sglib.auth.login(force_refresh=refresh)
     if not oauth_token:
         if interactive:
             oauth_token = _do_browser_login()
             if oauth_token:
                 sglib.auth.use_oauth_token(oauth_token)
         if not oauth_token:
             return ctxp.error("Login failed")
     # else: the token still works
-    
+
     ctxp.profile.save()
 
     auth_details = sglib.auth.details(get_org_details=details)
     if csp.orgId and auth_details.org.id != csp.orgId:
         return ctxp.error("Org ID does not match config. This should be a regression bug in the CLI.")
 
+    return auth_details if details else oauth_token["access_token"]
 
-    return auth_details if details else oauth_token['access_token']
 
 def _do_browser_login():
     csp_config = ctxp.profile.current().csp
     org_id = csp_config.orgId
+
     def _echo(msg):
-        click.echo(click.style(msg, fg='yellow'), err=True)
+        click.echo(click.style(msg, fg="yellow"), err=True)
+
     _echo(f"Logging to HCS...")
     _echo(f"  CSP:          {csp_config.url}")
     _echo(f"  Organization: {org_id if org_id else '<default>'}")
     _echo(f"  Profile:      {ctxp.profile.name()}")
-    _echo(f"A web browser has been opened at {csp_config.url}. Continue the login in the web browser, and return to this terminal.")
+    _echo(
+        f"A web browser has been opened at {csp_config.url}. Continue the login in the web browser, and return to this terminal."
+    )
     return login_support.login_via_browser(csp_config.url, org_id)
 
 
 def _ensure_current_profile():
     profile = ctxp.profile
-    data = profile.current(exit_on_failure = False)
+    data = profile.current(exit_on_failure=False)
     if not data:
         profile_support.ensure_default_production_profile()
     return profile.current()
 
+
 def _clear_credentials(csp):
     csp.apiToken = None
     csp.clientId = None
     csp.clientSecret = None
 
-def _validate_auth_method(org: str, api_token: str, client_id: str, client_secret: str, browser: bool):
 
+def _validate_auth_method(org: str, api_token: str, client_id: str, client_secret: str, browser: bool):
     # validation: API-token and org ID must not be specified together
     if org and api_token:
         return "Invalid arguments. CSP API user token is org-scoped. --org is not needed with --api-token.", 1
 
     # validation: must not specify duplicated auth methods
     ret = {}
     if api_token:
-        ret['api_token'] = 1
+        ret["api_token"] = 1
     if client_id:
-        ret['client_id/secret'] = 1
+        ret["client_id/secret"] = 1
     if browser:
-        ret['browser'] = 1
-    
+        ret["browser"] = 1
+
     if len(ret) > 1:
         return ctxp.error(f"Specify only one authenticate method. Currently specified: {list(ret.keys())}")
 
     if client_id and not client_secret or not client_id and client_secret:
         return ctxp.error("--client-id and --client-secret must be used in pair.")
-    
+
     if client_id and not client_secret:
         return ctxp.error(f"Missing --client-secret, when --client-id is specified.")
-
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.org_service import datacenter
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command("list")
 @cli.org_id
 def list_datacenters(org: str):
     """List all datacenters"""
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service.org_service import details
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import admin
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
+@click.argument("id", type=str, required=True)
 @cli.org_id
-def get(org: str):
-    """Get org details"""
+def delete(id: str, org: str, **kwargs):
+    """Delete Active Directory record by ID"""
+
     org_id = cli.get_org_id(org)
-    ret = details.get(org_id)
-    if ret:
-        return ret
-    return ret, 1
+
+    ret = admin.ad.delete(id, org_id)
+    if not ret:
+        return "", 1
+    return ret
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.common.ctxp import panic
+from vhcs.ctxp import panic
 from vhcs.service.pki import certificate
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @click.option("--confirm/--no-confirm", default=False)
 def delete_org_cert(org: str, confirm: bool):
     """Delete the signing certificate of a specific org"""
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service.pki import certificate
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 def get_org_cert(org: str):
     """Get the signing certificate of a specific org"""
     org_id = cli.get_org_id(org)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.common.ctxp import profile
+from vhcs.ctxp import profile
 from vhcs.service.pki import certificate
 from vhcs.util import pki_util
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 def _write_file(file_path: str, text: str):
     with open(file_path, "w") as file:
         file.write(text)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/pki/test.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/plan/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 help = "Horizon Plan manages deployments by files."
-hidden = True
+hidden = True
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/plan/graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,54 +9,55 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import sys
 import click
 import vhcs.plan as plan
-import vhcs.support.plan_util as util
-from vhcs.common.ctxp.util import error_details
+import vhcs.support.plan_util as plan_util
+
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
-@click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy. This includes deploying dependent resources.")
-@click.option("--include-dependencies/--single-resource-only", type=bool, default=False, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
-@click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
-@click.option("--show-progress/--show-plain-log", type=bool, default=True, help="Control output format, interactive progress or plain logs.")
-def deploy(file, resource: str, include_dependencies: bool, parallel: bool, show_progress: bool):
-
-    data, extra = util.load_plan(file)
-    concurrency = 10 if parallel else 1
-
-    job_view = None
-    if show_progress and sys.stdout.isatty():
-        from vhcs.common.job_view import JobView
-        job_view = JobView.create_async()
-        plan.attach_job_view(job_view)
-        
-    try:        
-        return plan.deploy(data, 
-                           additional_context=extra, 
-                           target_resource_name=resource, 
-                           include_dependencies=include_dependencies, 
-                           concurrency=concurrency)
+@click.option(
+    "--view/--output-only",
+    "-v",
+    type=bool,
+    default=True,
+    help="If view mode is specified, open browser to view the graph.",
+)
+@click.option("--for-deploy/--for-destroy", type=bool, default=True, help="Specify whether for deploy or for destroy.")
+@click.option(
+    "--resource",
+    "-r",
+    type=str,
+    required=False,
+    help="Specify a single resource in the plan to deploy. This includes deploying dependent resources.",
+)
+@click.option(
+    "--include-dependencies/--single-resource-only",
+    type=bool,
+    default=False,
+    required=False,
+    help="Used with --resource. Specify whether to process related resources, or just the target resource.",
+)
+def graph(file, view: bool, for_deploy: bool, resource: str, include_dependencies: bool):
+    """Generate a graph view of the deployment, in Graphviz format."""
+
+    try:
+        data, extra = plan_util.load_plan(file)
+        g = plan.graph(data, extra, not for_deploy, resource, include_dependencies)
+        if view:
+            _view_graph(g.source)
+        return g.source
     except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
-        return error_details(e), 1
-    finally:
-        if job_view:
-            job_view.close()
-
-# def _identify_files(file: list[str], name: str):
-#     if not file and not name:
-#         panic("Either --file or --name must be specified")
-#     if file and name:
-#         panic("--file and --name must not be specified together")
-    
-#     if name:
-#         return [
-#             name + '.blueprint.yml',
-#             name + '.vars.yml',
-#         ]
-#     return file
+        return str(e), 1
+
+
+def _view_graph(src):
+    import urllib.parse
+    import webbrowser
+
+    url = "https://dreampuf.github.io/GraphvizOnline/#" + urllib.parse.quote(src)
+    webbrowser.open(url, new=0, autoraise=True)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/plan/apply.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,35 +12,65 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import sys
 import click
 import vhcs.plan as plan
-import vhcs.support.plan_util as util
+import vhcs.support.plan_util as plan_util
+from vhcs.ctxp.util import error_details
+
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
-@click.option("--force/--fail-fast", type=bool, default=True, required=False, help="Force mode: try deleting everything and continue on error. Fail-fast mode: Stop on the first error.")
-@click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy.")
-@click.option("--include-dependencies/--single-resource-only", type=bool, default=False, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
-@click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
-@click.option("--show-progress/--show-plain-log", type=bool, default=True, help="Control output format, interactive progress or plain logs.")
-def destroy(file, force: bool, resource: str, include_dependencies: bool, parallel: bool, show_progress: bool):
-
-    data, extra = util.load_plan(file)
+@click.option(
+    "--resource",
+    "-r",
+    type=str,
+    required=False,
+    help="Specify a single resource in the plan to deploy. This includes deploying dependent resources.",
+)
+@click.option(
+    "--include-dependencies/--single-resource-only",
+    type=bool,
+    default=False,
+    required=False,
+    help="Used with --resource. Specify whether to process related resources, or just the target resource.",
+)
+@click.option(
+    "--parallel/--sequential",
+    type=bool,
+    default=True,
+    required=False,
+    help="Specify deployment mode, parallel or sequential.",
+)
+@click.option(
+    "--show-progress/--show-plain-log",
+    type=bool,
+    default=True,
+    help="Control output format, interactive progress or plain logs.",
+)
+def apply(file, resource: str, include_dependencies: bool, parallel: bool, show_progress: bool):
+    """Apply a plan, create/update resources."""
+    data, extra = plan_util.load_plan(file)
     concurrency = 10 if parallel else 1
 
     job_view = None
     if show_progress and sys.stdout.isatty():
-        from vhcs.common.job_view import JobView
+        from vhcs.util.job_view import JobView
+
         job_view = JobView.create_async()
         plan.attach_job_view(job_view)
 
     try:
-        return plan.destroy(data, force, resource, include_dependencies, concurrency, extra)
+        return plan.apply(
+            data,
+            additional_context=extra,
+            target_resource_name=resource,
+            include_dependencies=include_dependencies,
+            concurrency=concurrency,
+        )
     except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
-        return str(e), 1
+        return error_details(e), 1
     finally:
         if job_view:
             job_view.close()
-
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/entitlement/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 def delete(id: str, org: str):
     """Get entitlement by ID"""
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/auth/admin/get_org_idp_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import auth
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
 @cli.org_id
-def get(id: str, org: str):
-    """Get entitlement by ID"""
+def get_org_idp_map(org: str):
+    """Get org-idp-map by ID"""
     org_id = cli.get_org_id(org)
-    ret = portal.entitlement.get(id, org_id)
+    ret = auth.admin.get_org_idp_map(org_id=org_id)
     if ret:
         return ret
-    return '', 1
+    return ret, 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/set-edge.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
+@click.argument("site-id")
+@click.option("--edge", type=str, required=True, help="Edge deployment ID.")
 @cli.org_id
-def list(org: str, **kwargs):
-    """List entitlements"""
-    org_id=cli.get_org_id(org)
-    return portal.entitlement.list(org_id, **kwargs)
+def set_edge(site_id: str, edge: str, org: str, **kwargs):
+    """Set the edge for a site."""
+    return portal.site.set_edge(site_id, org_id=cli.get_org_id(org), edge_deployment_id=edge, **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/pool/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
-def delete(id: str, org: str):
-    """Delete pool by ID"""
+def get(id: str, org: str):
+    """Get pool by ID"""
     org_id = cli.get_org_id(org)
-    ret = portal.pool.delete(id, org_id)
-    return ret
+    ret = portal.pool.get(id, org_id)
+    if ret:
+        return ret
+    return ret, 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @cli.org_id
 def get(id: str, org: str):
-    """Get pool by ID"""
+    """Get site."""
     org_id = cli.get_org_id(org)
-    ret = portal.pool.get(id, org_id)
+    ret = portal.site.get(id, org_id)
     if ret:
         return ret
-    return ret, 1
+    return "", 1
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
-@click.option("--search", "-s", type=str, required=False, help="Search condition")
 @cli.org_id
 def list(org: str, **kwargs):
-    """List pools"""
-    org_id=cli.get_org_id(org)
-    return portal.pool.list(org_id, **kwargs)
+    """List sites"""
+    return portal.site.list(org_id=cli.get_org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/create.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/portal/site/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @click.option("--name", "-n", type=str, required=True)
 @click.option("--description", "-d", type=str, required=False)
 @cli.org_id
 def create(name: str, description: str, org: str):
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/delete.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/ad/list.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import admin
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
 @cli.org_id
-def delete(id: str, org: str):
-    """Delete a site."""
-    org_id = cli.get_org_id(org)
-    ret = portal.site.delete(id, org_id)
-    return ret
+def list(org: str, **kwargs):
+    """List Active Directory records"""
+    return admin.ad.list(org_id=cli.get_org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/get.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/template/vm/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import admin
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
+@click.argument("template-id", type=str, required=True)
 @cli.org_id
-def get(id: str, org: str):
-    """Get site."""
-    org_id = cli.get_org_id(org)
-    ret = portal.site.get(id, org_id)
-    if ret:
-        return ret
-    return "", 1
+def list(template_id: str, org: str, **kwargs):
+    """List template VMs"""
+    return admin.template.list_vms(template_id, org_id=cli.org_id(org), **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/list.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/admin/uag/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
+from vhcs.service import admin
+import vhcs.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
-def list(org: str, **kwargs):
-    """List sites"""
-    return portal.site.list(org_id=cli.get_org_id(org), **kwargs)
+@cli.search
+def list(**kwargs):
+    """List UAG deployments"""
+    return admin.uag.list(org_id=cli.get_org_id(kwargs["org"]), **kwargs)
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/set-edge.py` & `hcs-cli-0.1.50/vhcs/ctxp/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,11 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
-from vhcs.service import portal
-import vhcs.common.sglib.cli_options as cli
-
-
-@click.command()
-@click.argument("site-id")
-@click.option("--edge", type=str, required=True, help="Edge deployment ID.")
-@cli.org_id
-def set_edge(site_id: str, edge: str, org: str, **kwargs):
-    """Set the edge for a site."""
-    return portal.site.set_edge(site_id, org_id=cli.get_org_id(org), edge_deployment_id=edge, **kwargs)
+from ._init import init
+from .util import panic, error, CtxpException, launch_text_editor, choose
+from . import profile, config, var_template, state
+from .profile_store import profile_store
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/profile/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,35 +10,33 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.common.ctxp import profile, panic
+from vhcs.ctxp import profile, panic
 import vhcs.support.profile as profile_support
 
+
 @click.command()
 @click.option("--name", "-n", type=str, required=False, help="Name of the profile, if a non-default one is needed.")
 @click.option("--dev/--no-dev", type=bool, default=False, help="Initialize default development profiles.")
 def init(name: str, dev: bool):
     """Init profile interactively"""
 
     profile_support.ensure_default_production_profile()
-    
+
     if name:
         profile.create(name, profile_support.get_default_profile_template())
         print("Create profile: " + profile.file(name))
         print("Use 'hcs profile edit' to check/update.")
         print("Use 'hcs login --help' to complete authentication.")
     elif dev:
         profile_support.ensure_dev_profiles()
         print()
-        print('Next step:')
+        print("Next step:")
         print("  'hcs profile --help' : to know profile operations.")
         print("  'hcs profile use'    : to swtich between profiles.")
         print("  'hcs login --help'   : to complete authentication for the current profile.")
     else:
-        panic('Specify the target profile name by --name')
-    
-
-    
+        panic("Specify the target profile name by --name")
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import vhcs.common.sglib.cli_options as cli
+import vhcs.sglib.cli_options as cli
 from vhcs.service.vmhub import otp
 
 
 @click.command()
 @cli.org_id
 @click.option(
     "--region",
```

### Comparing `hcs-cli-0.1.48/vhcs/cli/main.py` & `hcs-cli-0.1.50/vhcs/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 
 _script_dir = path.abspath(path.join(path.dirname(path.realpath(__file__)), "."))
 _module_dir = path.dirname(_script_dir)
 if __name__ == "__main__":
     _cli_dir = path.dirname(_module_dir)
     sys.path.append(_cli_dir)
 
-import vhcs.common.ctxp as ctxp
-from vhcs.common.ctxp.util import option_output, option_verbose, option_field, panic, CtxpException
+import vhcs.ctxp as ctxp
+from vhcs.ctxp.util import option_output, option_verbose, option_field, panic, CtxpException
 
 # -----------------------------------------------------------
-import vhcs.common.logger as logger
+import vhcs.ctxp.logger as logger
 
 logger.setup()
 logging.getLogger("charset_normalizer").setLevel(logging.WARN)
 logging.getLogger("csp").setLevel(logging.INFO)
 logging.getLogger("context").setLevel(logging.WARN)
 logging.getLogger("init").setLevel(logging.WARN)
 logging.getLogger("profile").setLevel(logging.WARN)
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.50/vhcs/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.50/vhcs/cli/cmds/logout.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,11 +9,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ._init import init
-from .util import panic, error, CtxpException, launch_text_editor, choose
-from . import profile, config, var_template, state
-from .profile_store import profile_store
+import click
+from vhcs.ctxp import profile
+
+
+@click.command()
+def logout():
+    """Delete the stored login state, for the current profile."""
+    profile.auth.delete()
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.50/vhcs/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.50/vhcs/ctxp/built_in_cmds/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import os
 import subprocess
-import vhcs.common.ctxp as ctxp
-import vhcs.common.ctxp.util as util
+import vhcs.ctxp as ctxp
+import vhcs.ctxp.util as util
+
 
 @click.group(cls=ctxp.cli_processor.LazyGroup)
 def context():
     """Commands for context. Each profile has its own context. The commands work for the current profile."""
 
 
 @context.command()
@@ -66,21 +67,24 @@
 
 
 @context.command()
 def clear():
     """Delete all context objects."""
     ctxp.context.clear()
 
+
 @context.command()
-@click.argument("name", type=str, required = True)
+@click.argument("name", type=str, required=True)
 def file(name: str):
     """Get the file path of the specific context object."""
     return _get_file(name)
 
+
 def _get_file(name: str) -> str:
     return ctxp.context._store()._get_path(name)
 
+
 @context.command()
-@click.argument("name", type=str, required = True)
-def edit(name : str):
+@click.argument("name", type=str, required=True)
+def edit(name: str):
     """Launch platform-specific editor to edit a context file."""
-    util.launch_text_editor(_get_file(name))
+    util.launch_text_editor(_get_file(name))
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.50/vhcs/ctxp/built_in_cmds/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,63 +13,65 @@
 limitations under the License.
 """
 
 import click
 import sys
 import json
 import questionary
-from vhcs.common.ctxp import util, panic, profile, cli_processor
+from vhcs.ctxp import util, panic, profile, cli_processor
 
 
-@click.group(name='profile', cls=cli_processor.LazyGroup)
+@click.group(name="profile", cls=cli_processor.LazyGroup)
 def profile_cmd_group():
     """Commands for profile."""
 
 
 @profile_cmd_group.command()
 def list():
     """List all profile names."""
     return profile.names()
 
 
 @profile_cmd_group.command()
 @click.argument("name", required=False)
 def use(name: str):
     """Switch to a specific profile. If no name specified, launch interactive list to choose profile."""
-    
+
     if name:
         if profile.use(name) == None:
             panic("No such profile: " + name)
     else:
         current = profile.name()
         choices = profile.names()
         if not choices:
-            panic('No profile available.')
+            panic("No profile available.")
 
         ret = questionary.select("Select profile", choices, default=current, show_selected=True).ask()
         if ret:
             if profile.use(ret) == None:
                 panic("No such profile: " + name)
         else:
             # aborted
             return "", 1
-    
+
+
 @profile_cmd_group.command()
 @click.option("--from-name", "-f", required=True)
 @click.option("--to-name", "-t", required=True)
 def copy(from_name: str, to_name: str):
     """Copy profile."""
-    
+
     data = profile.get(from_name)
     if not data:
         panic("No such profile: " + from_name)
     if profile.exists(to_name):
         panic("Profile already exists: " + to_name)
     profile.create(to_name, data, True)
 
+
 @profile_cmd_group.command()
 @click.argument("name", required=False)
 def get(name: str):
     """Get content of a specific profile."""
     if name:
         data = profile.get(name)
         if data == None:
@@ -118,21 +120,23 @@
     try:
         data = json.loads(text)
     except Exception as e:
         panic(f"Invalid json {e}")
 
     profile.create(name, data)
 
+
 @profile_cmd_group.command()
 def name():
     """Get current profile name."""
     return profile.name()
 
+
 @profile_cmd_group.command()
-@click.argument("name", type=str, required = False)
-def edit(name : str):
+@click.argument("name", type=str, required=False)
+def edit(name: str):
     """Launch platform-specific editor to edit the profile file."""
 
     if not name:
         name = profile.name()
     file_name = profile.file(name)
     util.launch_text_editor(file_name)
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.50/vhcs/ctxp/cli_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,24 @@
     subgroup = LazyGroup(name=name, help=help, mod_path=mod_path)
     current.add_command(subgroup)
     return subgroup
 
 
 def _read_group_meta(mod_path: Path) -> dict:
     meta_file = mod_path.absolute().joinpath("__init__.py")
-    
-    ret = {
-        'help': None,
-        'hidden': False
-    }
+
+    ret = {"help": None, "hidden": False}
     if meta_file.exists():
         # TODO
         with open(meta_file, "r") as f:
             lines = f.readlines()
 
     return ret
 
 
-
-
 _excluded_names = ["__pycache__", "__init__.py", ".DS_Store"]
 
 
 def _add_subcommands(commands_dir: str, group: Group):
     for mod_path in Path(commands_dir).glob("*"):
         if mod_path.name in _excluded_names:
             continue
@@ -144,15 +139,15 @@
             validate_error_return(data, return_code)
             if isinstance(data, Exception):
                 print_error(data)
             else:
                 print_output(data, kwargs.get("output"), kwargs.get("field"), file=sys.stderr)
             ctx = click.get_current_context()
             ctx.exit(return_code)
-        #else fall-through
+        # else fall-through
     elif isinstance(result, Exception):
         print_error(result)
         ctx = click.get_current_context()
         ctx.exit(1)
     else:
         print_output(result, kwargs.get("output"), kwargs.get("field"))
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.50/vhcs/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.50/vhcs/ctxp/context.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 from .jsondot import dotdict
 from . import profile
 from .profile_store import profile_store, fstore, _store_from_profile_name
 
 
 def _store() -> fstore:
-    return profile_store('context')
+    return profile_store("context")
+
 
 def list() -> list[str]:
     return _store().keys()
 
 
 def get(name: str, reload: bool = False, default=None) -> dotdict:
     return _store().get(key=name, reload=reload, default=default)
@@ -32,12 +33,14 @@
 def set(name: str, data: dict):
     return _store().save(name, data)
 
 
 def delete(name: str):
     return _store().delete(name)
 
+
 def file(name: str):
     return _store()._get_path(name)
 
+
 def clear():
     return _store().clear()
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.50/vhcs/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.50/vhcs/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.50/vhcs/ctxp/jsondot.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,18 @@
     __delattr__ = dict.__delitem__
 
 
 # TODO: how to remove the lib-specific dependency from this utility class?
 # Register the represent_dict function with SafeDumper
 def _represent_dict(dumper, data):
     return dumper.represent_dict(data.items())
+
+
 import yaml
+
 yaml.SafeDumper.add_representer(dotdict, _represent_dict)
 
 
 def dotify(target: Any) -> Any:
     """Deeply convert an object from dict to dotdict"""
 
     # If already dotified, skip
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.50/vhcs/ctxp/profile.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 import pathlib
 import shutil
 import os
 from typing import Any
 from .util import panic, CtxpException
 from .jsondot import dotdict, dotify
 from . import state
-from ..util import load_data_file, save_data_file
+from .data_util import load_data_file, save_data_file
 
 _repo_path: str = None
 _active_profile_name: str = None
 _data: dotdict = None
+_auth_cache: dict = None
+
 
 def _set_active_profile_name(name):
     global _active_profile_name
     _active_profile_name = name
-    state.set('active_profile', name)
+    state.set("active_profile", name)
+
 
 def init(repo_path: str, active_profile_name: str = None) -> None:
     if active_profile_name:
         _set_active_profile_name(active_profile_name)
 
     global _repo_path
     _repo_path = repo_path
@@ -45,28 +48,29 @@
     if not profile_name:
         profile_name = name()
     return os.path.join(_repo_path, profile_name)
 
 
 def create(name: str, data: dict, auto_use: bool = True):
     if exists(name):
-        raise CtxpException('Profile already exists: ' + name)
+        raise CtxpException("Profile already exists: " + name)
     file_path = file(name)
     pathlib.Path(os.path.dirname(file_path)).mkdir(parents=True, exist_ok=True)
     save_data_file(data, file(name))
     if auto_use:
         use(name)
     return get(name)
 
+
 def copy(from_name: str, to_name: str, overwrite: bool = True):
     if exists(to_name) and not overwrite:
-        raise CtxpException('Profile already exists: ' + to_name)
+        raise CtxpException("Profile already exists: " + to_name)
     data = get(from_name)
     if not data:
-        raise CtxpException('Profile does not exist: ' + from_name)
+        raise CtxpException("Profile does not exist: " + from_name)
     create(to_name, deepcopy(data), auto_use=False)
 
 
 def current(reload: bool = False, exit_on_failure=True, exclude_secret: bool = False) -> dict:
     """Get content of the current active profile"""
     profile_name = name()
     data = get(profile_name, reload)
@@ -74,33 +78,35 @@
     if data is None and exit_on_failure:
         panic(
             "Profile not set. Use 'hcs profile use [profile-name]' to choose one, or use 'hcs profile init' to create default profiles."
         )
 
     if exclude_secret:
         data = dotdict(dict(data))
-        csp_config = dict(data['csp'])
-        csp_config['apiToken'] = None
-        csp_config['clientSecret'] = None
-        data['csp'] = csp_config
+        csp_config = dict(data["csp"])
+        csp_config["apiToken"] = None
+        csp_config["clientSecret"] = None
+        data["csp"] = csp_config
     return data
 
+
 def save():
     """Save the current profile"""
     global _data
     if _data != None:
         save_data_file(_data, file(name()))
 
+
 def name() -> str:
     """Get the current active profile name"""
     global _active_profile_name
     if not _active_profile_name:
-        _active_profile_name = state.get('active_profile', default='default')
+        _active_profile_name = state.get("active_profile", default="default")
         if not exists(_active_profile_name):
-            _set_active_profile_name('default')
+            _set_active_profile_name("default")
     return _active_profile_name
 
 
 def use(name: str) -> str:
     """Use to the specified profile"""
 
     profile_exists = name in names()
@@ -121,19 +127,20 @@
 def delete(profile_name: str = None) -> None:
     """Delete a profile"""
 
     if profile_name is None:
         profile_name = name()
     global _active_profile_name, _data
     if _active_profile_name == profile_name:
-        _active_profile_name = 'default'
+        _active_profile_name = "default"
         _data = None
-    
+
     shutil.rmtree(os.path.join(_repo_path, profile_name), ignore_errors=True)
 
+
 def get(profile_name: str, reload: bool = False, default=None) -> dotdict:
     """Get profile data by name"""
     if profile_name == name():
         global _data
         if _data != None and not reload:
             return _data
         data = load_data_file(file(profile_name), default=default)
@@ -145,20 +152,50 @@
         if data != None:
             data = dotify(data)
     return data
 
 
 def file(profile_name: str) -> str:
     """Get the file path of a profile"""
-    return os.path.join(_repo_path, profile_name, 'profile.yml')
+    return os.path.join(_repo_path, profile_name, "profile.yml")
 
 
 def exists(profile_name: str) -> bool:
     return profile_name in names()
 
+
+class auth:
+    @staticmethod
+    def _file_name() -> str:
+        return os.path.join(_repo_path, name(), ".auth")
+
+    @staticmethod
+    def get() -> dict:
+        global _auth_cache
+        if _auth_cache == None:
+            _auth_cache = dotify(load_data_file(auth._file_name(), {}, "yaml"))
+        return deepcopy(_auth_cache)
+
+    @staticmethod
+    def set(data: dict) -> None:
+        global _auth_cache
+        import json
+
+        if json.dumps(data) == json.dumps(_auth_cache):
+            return
+        _auth_cache = dotify(deepcopy(data))
+        file_name = auth._file_name()
+        save_data_file(data, file_name, "yaml")
+        os.chmod(file_name, 0o600)
+
+    @staticmethod
+    def delete() -> None:
+        os.unlink(auth._file_name())
+
+
 # --------------------------------------------------
 
 
 def _nested_obj_to_plain_dict(obj: Any, path: str, result: dotdict) -> None:
     t = type(obj)
     if t is str or t is int or t is float or t is bool:
         result[path] = obj
@@ -171,15 +208,14 @@
             v = obj[i]
             _nested_obj_to_plain_dict(v, path + "[" + i + "]", result)
     else:
         raise Exception(f"TODO: type={t}")
 
 
 def plain() -> dotdict:
-    
     _plain = dotdict()
     data = current()
     for k in data:
         _nested_obj_to_plain_dict(data[k], k, _plain)
 
     return _plain
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.50/vhcs/ctxp/profile_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .fstore import fstore
 from .util import CtxpException
 
 _store_map: dict[str, fstore] = {}
 _active_profile_name: str = None
 
 
-def profile_store(store_name : str) -> fstore:
+def profile_store(store_name: str) -> fstore:
     global _store_map, _active_profile_name
 
     profile_name = profile.name()
     if not profile_name:
         raise CtxpException("Profile not specified")
 
     if profile_name != _active_profile_name:
@@ -42,8 +42,8 @@
         _store_map[store_name] = ret
     return ret
 
 
 def _store_from_profile_name(profile_name: str, store_name: str) -> fstore:
     profile_path = profile.path(profile_name)
     store_path = os.path.join(profile_path, store_name)
-    return fstore(store_path)
+    return fstore(store_path)
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.50/vhcs/ctxp/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 """
 
 import pathlib
 from typing import Any
 import os
 from . import jsondot
 
+
 class _StateFile:
     def __init__(self, file_path: str):
         self._path = file_path
         self._cache = None
         pathlib.Path(os.path.dirname(file_path)).mkdir(parents=True, exist_ok=True)
-        
+
     def _data(self, reload: bool = False):
         if self._cache is None or reload:
             self._cache = jsondot.load(self._path, {})
         return self._cache
 
     def get(self, key: str, default: Any, reload: bool = False):
         return self._data(reload).get(key, default)
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.50/vhcs/ctxp/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,53 +25,54 @@
 from typing import Any, Callable
 import questionary
 
 
 class CtxpException(Exception):
     pass
 
+
 def error(reason: any, return_code: int = 1) -> tuple[CtxpException, int]:
-    
     # Shortcut if the reason is an Exception already
     if isinstance(reason, Exception):
         return reason, return_code
-    
+
     # Convert reason to string and wrap as CtxpException
     if isinstance(reason, str):
         pass
     elif isinstance(reason, dict):
         reason = json.dumps(reason, indent=4)
     else:
         reason = str(reason)
     return CtxpException(reason), return_code
 
+
 def validate_error_return(reason, return_code):
     if return_code == 0:
         raise CtxpException("Invalid return code. return_code must not be 0 (success) in error situation.")
     if not isinstance(return_code, int):
         raise CtxpException("Invalid return code. return_code must be integer, but got " + type(return_code))
-    
 
-def print_output(data: Any, output: str = "json", fields: str = None, file = sys.stdout):
+
+def print_output(data: Any, output: str = "json", fields: str = None, file=sys.stdout):
     if type(data) is str:
         text = data
     elif isinstance(data, Exception):
         text = f"{type(data).__name__}: {data}"
     else:
-
         try:
             data = _convert_generator(data)
             _filter_fields(data, fields)
 
             if output == "json":
                 text = json.dumps(data, default=vars, indent=4)
             elif output == "json-compact":
                 text = json.dumps(data, default=vars)
             elif output == "yaml":
-                import vhcs.common.ctxp as ctxp
+                import vhcs.ctxp as ctxp
+
                 text = yaml.dump(ctxp.jsondot.plain(data))
             elif output == "text":
                 if isinstance(data, list):
                     text = ""
                     for i in data:
                         line = i if type(i) is str else json.dumps(i)
                         text += line + "\n"
@@ -82,35 +83,33 @@
             else:
                 raise Exception(f"Unexpected output format: {output}")
         except Exception as e:
             print("Fail converting object:", e, file=sys.stderr)
             text = data
     print(text, end="", file=file)
 
+
 def print_error(error):
-    known_exceptions = [
-        httpx.HTTPStatusError,
-        httpx.ConnectError,
-        CtxpException,
-        TimeoutError,
-        subprocess.CalledProcessError,
-        KeyboardInterrupt
+    critical_errors = [
+        KeyError,
     ]
-    for ex in known_exceptions:
+    for ex in critical_errors:
         if isinstance(error, ex):
-            msg = error_details(error)
-            print(msg, file=sys.stderr)
-            return
-    traceback.print_exception(type(error), error, error.__traceback__, file=sys.stderr)
+            traceback.print_exception(type(error), error, error.__traceback__, file=sys.stderr)
+            break
+    msg = error_details(error)
+    print(msg, file=sys.stderr)
+
 
 def _convert_generator(data: Any):
     if isinstance(data, types.GeneratorType):
         return list(data)
     return data
 
+
 def _filter_fields(obj: Any, fields: str):
     if not fields:
         return obj
     parts = fields.split(",")
 
     def _filter_obj(o):
         if not isinstance(o, dict):
@@ -131,76 +130,80 @@
     elif isinstance(reason, Exception):
         text = type(reason).__name__ + ": " + str(reason)
     else:
         text = reason
     print(text, file=sys.stderr)
     sys.exit(code)
 
-def launch_text_editor(file_name : str, default_editor : str = None):
+
+def launch_text_editor(file_name: str, default_editor: str = None):
     if not default_editor:
-        default_editor = 'vi'
-    cmd = os.environ.get('EDITOR', default_editor) + ' ' + file_name
+        default_editor = "vi"
+    cmd = os.environ.get("EDITOR", default_editor) + " " + file_name
     subprocess.call(cmd, shell=True)
 
 
-def choose(prompt: str, items: list, fn_get_text: Callable = None, selected = None):
+def choose(prompt: str, items: list, fn_get_text: Callable = None, selected=None):
     if len(items) == 0:
         panic(prompt + " ERROR: no item available.")
 
     if fn_get_text == None:
         fn_get_text = lambda t: str(t)
-        
+
     if len(items) == 1:
         ret = items[0]
         print(prompt + " only one item available. Select by default: " + fn_get_text(ret))
         return ret
-    
+
     choices = []
     size = len(items)
     for i in range(size):
         label = fn_get_text(items[i])
-        #if label in choices:
+        # if label in choices:
         #    raise Exception("Problem with the provided fn_get_text: generates non-unique label. Item=" + label)
         choices.append(label)
 
-    #hack workaround bug of the questionary lib
+    # hack workaround bug of the questionary lib
     selected_key = fn_get_text(selected) if selected else None
     k = questionary.select(prompt, choices, default=selected_key, show_selected=True).ask()
     if k == None:
         panic()
     for i in range(size):
         if k == choices[i]:
             return items[i]
     raise Exception("This is a bug and should not happen")
 
+
 def input_array(prompt: str, default: list[str] = None):
     default_value = ",".join(default) if default else None
-    
+
     input_value = click.prompt(prompt, default_value)
     if not input_value:
         return []
     parts = input_value.split(",")
     ret = []
     for p in parts:
         ret.append(p.strip())
     return ret
 
+
 def error_details(e: Exception | Any):
     if isinstance(e, Exception):
-        details = e.__class__.__name__ + ': ' + str(e)
+        details = e.__class__.__name__ + ": " + str(e)
         cause = e.__cause__
         if cause and cause != e:
             details += " | Caused by: " + error_details(cause)
 
         if isinstance(e, httpx.HTTPStatusError):
             details += "\n" + e.response.text
         return details
     else:
         return str(e)
 
+
 option_verbose = click.option(
     "-v",
     "--verbose",
     count=True,
     default=0,
     help="Print debug logs",
 )
```

### Comparing `hcs-cli-0.1.48/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.50/vhcs/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/common/duration.py` & `hcs-cli-0.1.50/vhcs/ctxp/duration.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 # PT555H
 # PT13320H
 
 
 def to_seconds(duration_string: str):
     if not duration_string:
         return 0
-    
+
     duration_string = duration_string.upper()
-    if not duration_string.startswith('P'):
-        duration_string = 'PT' + duration_string
+    if not duration_string.startswith("P"):
+        duration_string = "PT" + duration_string
 
     p = re.compile(PATTERN)
     matcher = p.fullmatch(duration_string)
     if matcher is None:
         raise Exception("Unsupported duration format: %s" % duration_string)
 
     if matcher.start(3) >= 0 and matcher.end(3) == matcher.start(3) + 1 and duration_string[matcher.start(3)] == "T":
@@ -80,8 +80,8 @@
     assert to_seconds("PT2H3M") == 2 * 3600 + 3 * 60
     assert to_seconds("PT2H3S") == 2 * 3600 + 3
     assert to_seconds("PT2H3M4S") == 2 * 3600 + 3 * 60 + 4
     assert to_seconds("P1D") == 1 * 24 * 60 * 60
     assert to_seconds("P1DT1M") == 1 * 24 * 60 * 60 + 1 * 60
     assert to_seconds("P1DT1S") == 1 * 24 * 60 * 60 + 1
     assert to_seconds("P1DT1H1S") == 1 * 24 * 60 * 60 + 1 * 3600 + 1
-    print("SUCCESS")
+    print("SUCCESS")
```

### Comparing `hcs-cli-0.1.48/vhcs/common/job_view.py` & `hcs-cli-0.1.50/vhcs/util/job_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,41 +18,42 @@
 from time import sleep, monotonic
 import sys
 import os
 from rich.live import Live
 from rich.progress import Progress, Task, ProgressBar, SpinnerColumn, TextColumn, TimeRemainingColumn, ProgressColumn
 from rich.table import Column
 from rich.text import Text
-import vhcs.common.duration as duration
+import vhcs.ctxp.duration as duration
 
 
 def _shorten_package_name(package_name, max_length):
     if len(package_name) <= max_length:
         return package_name
 
-    parts = package_name.split('.')
+    parts = package_name.split(".")
     shortened_parts = []
 
     for i, part in enumerate(parts):
         shortened_parts.append(part[0])
 
         if i == len(parts) - 1:
             # Last package name
-            remaining_length = max_length - len('.'.join(shortened_parts))
+            remaining_length = max_length - len(".".join(shortened_parts))
             if len(part) > remaining_length:
-                shortened_parts[-1] = '...' + part[-remaining_length + 3:]
+                shortened_parts[-1] = "..." + part[-remaining_length + 3 :]
             else:
                 shortened_parts[-1] = part
         else:
-            new_package_name = '.'.join(shortened_parts)
+            new_package_name = ".".join(shortened_parts)
 
             if len(new_package_name) + len(parts) - i - 1 > max_length:
                 break
 
-    return '.'.join(shortened_parts)
+    return ".".join(shortened_parts)
+
 
 class _MyPlainBarColumn(ProgressColumn):
     def __init__(self) -> None:
         super().__init__(table_column=Column(min_width=10))
 
     def render(self, task: Task) -> ProgressBar:
         """Gets a progress bar widget for a task."""
@@ -66,16 +67,15 @@
             complete_style="bar.complete",
             finished_style="bar.finished",
             pulse_style="bar.pulse",
         )
 
 
 class _MyTimeRemainingColumn(ProgressColumn):
-    """Renders estimated time remaining.
-    """
+    """Renders estimated time remaining."""
 
     # Only refresh twice a second to prevent jitter
     max_refresh = 0.5
 
     def __init__(
         self,
         compact: bool = False,
@@ -107,99 +107,103 @@
 
         if self.compact and not hours:
             formatted = f"{minutes:02d}:{seconds:02d}"
         else:
             formatted = f"{hours:d}:{minutes:02d}:{seconds:02d}"
 
         return Text(formatted, style=style)
-    
+
+
 def _timeout_to_seconds(timeout: str, default: int = 60) -> int:
     t = duration.to_seconds(timeout)
     if t == 0 and default:
         t = default
     return t
 
+
 class JobView:
     def __init__(self, auto_close: bool = True):
         self._map = {}
         self._todo = set()
         self._auto_close = auto_close
         self._closed = False
 
         w, h = os.get_terminal_size()
-        msg_width = w - 40 - 1 - 1 - 1 - 10 - 1 -  5 - 1 - 1
+        msg_width = w - 40 - 1 - 1 - 1 - 10 - 1 - 5 - 1 - 1
         self._job_ctl = Progress(
             TextColumn("{task.description}", table_column=Column(max_width=40, min_width=10)),
             SpinnerColumn(table_column=Column(min_width=1)),
-            #BarColumn(pulse_style='white'),
+            # BarColumn(pulse_style='white'),
             _MyPlainBarColumn(),
-            #TextColumn("[white][progress.percentage][white]{task.percentage:>3.0f}%"),
-            #TaskProgressColumn(show_speed=True),
-            TimeRemainingColumn(compact=True, elapsed_when_finished=True, table_column=Column(style='white', min_width=5)),
+            # TextColumn("[white][progress.percentage][white]{task.percentage:>3.0f}%"),
+            # TaskProgressColumn(show_speed=True),
+            TimeRemainingColumn(
+                compact=True, elapsed_when_finished=True, table_column=Column(style="white", min_width=5)
+            ),
             TextColumn("{task.fields[details]}", table_column=Column(max_width=msg_width, no_wrap=True)),
-            get_time=monotonic
+            get_time=monotonic,
         )
 
     def add(self, id: str, name: str):
         name = _shorten_package_name(name, 30)
-        self._map[id] = self._job_ctl.add_task(name, start=False, details='')
+        self._map[id] = self._job_ctl.add_task(name, start=False, details="")
         self._todo.add(id)
 
     def remove(self, id: str):
         task_id = self._map[id]
         self._job_ctl.remove_task(task_id)
         del self._map[id]
         self._todo.discard(id)
 
     def refresh(self):
         for task_id in self._map.values():
             task = self._job_ctl._tasks[task_id]
-            
+
             if task.started and not task.finished and not task.stop_time:
                 completed = monotonic() - task.start_time
                 if completed >= task.total:
                     completed = task.total - 1
                 self._job_ctl.update(task_id, completed=completed)
 
     def update(self, id: str, details: str):
         task_id = self._map[id]
         if not details:
-            details = ''
+            details = ""
         self._job_ctl.update(task_id, details=details)
 
     def start(self, id: str, timeout: str) -> None:
         task_id = self._map[id]
         if timeout:
             total = _timeout_to_seconds(timeout)
             self._job_ctl.update(task_id, total=total)
         self._job_ctl.start_task(task_id)
 
     def _ensure_started(self, id: str) -> None:
         self.start(id, None)
-        
+
     def success(self, id: str) -> None:
         self._ensure_started(id)
         task_id = self._map[id]
         self._job_ctl.update(task_id, completed=sys.float_info.max)
         self._todo.discard(id)
 
     def skip(self, id: str, reason: str) -> None:
         self._ensure_started(id)
         task_id = self._map[id]
-        details = 'skipped'
+        details = "skipped"
         if reason:
-            details += f': {reason}'
+            details += f": {reason}"
         self._job_ctl.update(task_id, completed=sys.float_info.max, details=details)
         self._todo.discard(id)
 
     def error(self, id: str, details: str):
         self._ensure_started(id)
         task_id = self._map[id]
         if not details:
-            details = ''
+            details = ""
         self._job_ctl.update(task_id, details=details)
         self._job_ctl.stop_task(task_id)
         self._todo.discard(id)
 
     def close(self) -> None:
         self._todo.clear()
         self._closed = True
@@ -209,17 +213,16 @@
             while True:
                 self.refresh()
                 if self._closed:
                     break
                 if self._auto_close and not self._todo:
                     break
                 sleep(0.2)
-                
 
     @staticmethod
     def create_async(auto_close: bool = False) -> "JobView":
         import threading
+
         inst = JobView(auto_close)
         t = threading.Thread(target=inst.show, daemon=True)
         t.start()
         return inst
-
```

### Comparing `hcs-cli-0.1.48/vhcs/common/logger.py` & `hcs-cli-0.1.50/vhcs/ctxp/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 LOG_FORMAT_SIMPLE = "%(levelname)-4s %(asctime)s %(name)-16s %(message)s"
 LOG_FORMAT_LONG = (
     "%(color_on)s%(asctime)s [%(process)-5d:%(threadName)-12s] %(levelname)-7s [%(name)-16s] %(message)s%(color_off)s"
 )
 DATE_FORMAT_SIMPLE = "%H:%M:%S"
 
+
 def mask_password(msg: str) -> str:
     msg = re.sub(r"(\"password\"\s*:\s*\"?)(.*?)(\"?[\s*,? | \s*\}])", r"\1******\3", msg)
     return msg
 
 
 class LogFormatter(logging.Formatter):
     COLOR_CODES = {
@@ -51,102 +52,103 @@
             record.color_on = self.COLOR_CODES[record.levelno]
             record.color_off = self.RESET_CODE
         else:
             record.color_on = ""
             record.color_off = ""
 
         record.name = _shorten_package_name(record.name, 16)
-    
+
         msg = super(LogFormatter, self).format(record, *args, **kwargs)
         return mask_password(msg) if self.mask else msg
 
-class LogFormatterFixedNameWidth(logging.Formatter):
 
+class LogFormatterFixedNameWidth(logging.Formatter):
     def __init__(self, *args, **kwargs):
         super(LogFormatter, self).__init__(*args, **kwargs)
 
     def format(self, record, *args, **kwargs):
         record.name = _shorten_package_name(record.name, 16)
         return super(LogFormatterFixedNameWidth, self).format(record, *args, **kwargs)
-    
+
+
 def _shorten_package_name(package_name, max_length):
     if len(package_name) <= max_length:
         return package_name
 
-    parts = package_name.split('.')
+    parts = package_name.split(".")
     shortened_parts = []
 
     for i, part in enumerate(parts):
         shortened_parts.append(part[0])
 
         if i == len(parts) - 1:
             # Last package name
-            remaining_length = max_length - len('.'.join(shortened_parts))
+            remaining_length = max_length - len(".".join(shortened_parts))
             if len(part) > remaining_length:
-                shortened_parts[-1] = '...' + part[-remaining_length + 3:]
+                shortened_parts[-1] = "..." + part[-remaining_length + 3 :]
             else:
                 shortened_parts[-1] = part
         else:
-            new_package_name = '.'.join(shortened_parts)
+            new_package_name = ".".join(shortened_parts)
 
             if len(new_package_name) + len(parts) - i - 1 > max_length:
                 break
 
-    return '.'.join(shortened_parts)
+    return ".".join(shortened_parts)
+
 
 def setup(
     console_log_output="stdout",
     console_log_level="INFO",
     console_log_color=True,
     console_log_mask=True,
     logfile_file=None,
     logfile_log_level="INFO",
     logfile_log_color=False,
     logfile_log_mask=True,
     log_line_template=LOG_FORMAT_SIMPLE,
-    date_fmt=DATE_FORMAT_SIMPLE
+    date_fmt=DATE_FORMAT_SIMPLE,
 ):
     # Alternative: 'global logger; logger = logging.getLogger("<name>")'
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
 
     if console_log_output is not None:
         setup_console_output(
             logger,
             console_log_output,
             console_log_level,
             console_log_color,
             console_log_mask,
             log_line_template,
-            date_fmt
+            date_fmt,
         )
 
     if logfile_file:
         setup_file_output(
             logger,
             logfile_file,
             logfile_log_level,
             logfile_log_color,
             logfile_log_mask,
             log_line_template,
         )
 
 
 def setup_console_output(
-    logger,
-    console_log_output,
-    console_log_level,
-    console_log_color,
-    console_log_mask,
-    log_line_template,
-    date_fmt
+    logger, console_log_output, console_log_level, console_log_color, console_log_mask, log_line_template, date_fmt
 ):
     if not date_fmt:
         date_fmt = coloredlogs.DEFAULT_DATE_FORMAT
-    coloredlogs.install(level=console_log_level, fmt=log_line_template, datefmt=date_fmt, formatter=LogFormatter(fmt=log_line_template, color=console_log_color, mask=console_log_mask))
+    coloredlogs.install(
+        level=console_log_level,
+        fmt=log_line_template,
+        datefmt=date_fmt,
+        formatter=LogFormatter(fmt=log_line_template, color=console_log_color, mask=console_log_mask),
+    )
 
     # console_log_output = console_log_output.lower()
     # if console_log_output == "stdout":
     #     console_log_output = sys.stdout
     # elif console_log_output == "stderr":
     #     console_log_output = sys.stderr
     # else:
```

### Comparing `hcs-cli-0.1.48/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.50/vhcs/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.50/vhcs/sglib/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,133 +14,103 @@
 """
 
 import time
 import jwt
 import json
 import hashlib
 import logging
-from vhcs.common.ctxp import profile, context, panic, jsondot
+from vhcs.ctxp import profile, panic, jsondot
 from .csp import CspClient
 from .login_support import create_oauth_client, refresh_oauth_token
 
 log = logging.getLogger(__name__)
 
 
-# def _validate_profile_readiness():
-#     csp_config = profile.current().csp
-#     if not csp_config:
-#         panic(f"Profile property missing: profile.csp. Current profile: {profile.name()}")
-#     if csp_config.apiToken:
-#         return
-#     if csp_config.clientId and csp_config.clientSecret:
-#         return
-    
-#     # This could be interactive login.
-#     # Check existance of the previous login.
-#     if _get_auth_data():
-#         return
-    
-#     panic(
-#         f"Profile not ready. Perform an interactive login using 'hcs login', or use 'hcs profile edit' to update profile.csp.apiToken or profile.csp.clientId/clientSecret. Current profile: {profile.name()}"
-#     )
-
-
 def _get_profile_auth_hash():
     csp = profile.current().csp
     text = json.dumps(csp, default=vars)
-    return profile.name() + '#' + hashlib.md5(text.encode("ascii")).hexdigest()
+    return profile.name() + "#" + hashlib.md5(text.encode("ascii")).hexdigest()
 
 
 def _is_auth_valid(auth_data):
     if not auth_data:
         return
     if not auth_data.token:
         return
     if auth_data.hash != _get_profile_auth_hash():
         return
     if time.time() + 0 * 5 * 60 > auth_data.token.expires_at:
         return
     return True
 
 
-def _get_auth_data():
-    return context.get(".auth", default=dict())
-
-
 def login(force_refresh: bool = False):
     """Ensure login state, using credentials from the current profile. Return oauth token."""
 
     # _validate_profile_readiness()
 
-    auth_data = _get_auth_data()
+    auth_data = profile.auth.get()
     if force_refresh or not _is_auth_valid(auth_data):
         oauth_token = _get_new_oauth_token(auth_data.token)
         if oauth_token:
             use_oauth_token(oauth_token)
     else:
         oauth_token = auth_data.token
     return oauth_token
 
+
 def _get_new_oauth_token(old_oauth_token):
     csp_config = profile.current().csp
-    
-    csp_client = CspClient(
-        url=csp_config.url
-    )
+
+    csp_client = CspClient(url=csp_config.url)
 
     if csp_config.apiToken:
         oauth_token = csp_client.login_with_api_token(csp_config.apiToken)
     elif csp_config.clientId:
-        oauth_token = csp_client.login_with_client_id_and_secret(csp_config.clientId, csp_config.clientSecret, csp_config.orgId)
+        oauth_token = csp_client.login_with_client_id_and_secret(
+            csp_config.clientId, csp_config.clientSecret, csp_config.orgId
+        )
     else:
-        # This should be a config from interactive login. 
+        # This should be a config from interactive login.
         # Use existing oauth_token to refresh.
         if old_oauth_token:
             oauth_token = refresh_oauth_token(old_oauth_token, csp_config.url)
         else:
             oauth_token = None
     return oauth_token
 
+
 def oauth_client():
     login(False)
-    oauth_token = _get_auth_data().token
+    oauth_token = profile.auth.get().token
     csp_url = profile.current().csp.url
+
     def fn_on_new_oauth_token(token, refresh_token=None, access_token=None):
         use_oauth_token(token)
+
     return create_oauth_client(oauth_token, csp_url, fn_on_new_oauth_token)
-    
+
 
 def details(get_org_details: bool = False) -> jsondot.dotdict:
     """Get the auth details, for the current profile"""
     oauth_token = login()
     if not oauth_token:
         return
-    
-    decoded = jwt.decode(oauth_token['access_token'], options={"verify_signature": False})
+
+    decoded = jwt.decode(oauth_token["access_token"], options={"verify_signature": False})
     org_id = decoded["context_name"]
-    ret = {
-        'token': oauth_token,
-        'jwt': decoded,
-        'org': {
-            'id': org_id
-        }
-    }
+    ret = {"token": oauth_token, "jwt": decoded, "org": {"id": org_id}}
 
     if get_org_details:
-        csp_client = CspClient(url = profile.current().csp.url, oauth_token = oauth_token)
+        csp_client = CspClient(url=profile.current().csp.url, oauth_token=oauth_token)
         try:
             org_details = csp_client.get_org_details(org_id)
         except Exception as e:
-            org_details = {
-                'error': f"Fail retrieving org details: {e}"
-            }
-        ret['org'].update(org_details)
+            org_details = {"error": f"Fail retrieving org details: {e}"}
+        ret["org"].update(org_details)
     return jsondot.dotify(ret)
-    
+
 
 def use_oauth_token(oauth_token):
-    if 'expires_at' not in oauth_token:
-        oauth_token['expires_at'] = int(time.time()) + oauth_token["expires_in"]
-    context.set(".auth", {
-        'token': oauth_token,
-        'hash': _get_profile_auth_hash()
-    })
+    if "expires_at" not in oauth_token:
+        oauth_token["expires_at"] = int(time.time()) + oauth_token["expires_in"]
+    profile.auth.set({"token": oauth_token, "hash": _get_profile_auth_hash()})
```

### Comparing `hcs-cli-0.1.48/vhcs/common/sglib/cli_options.py` & `hcs-cli-0.1.50/vhcs/sglib/cli_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,53 +10,52 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.common.ctxp import CtxpException
+from vhcs.ctxp import CtxpException
 
 org_id = click.option(
     "--org",
     type=str,
     default=None,
     required=False,
     help="Specify org ID. If not specified, org ID from the current auth token will be used.",
 )
 wait = click.option(
-    "--wait", "-w",
-    type=str, 
-    required=False, 
-    default='10m', 
-    help="Wait time. E.g. '30s', or '5m'. Default: 10m. Specify '0' to disable waiting and return immediately."
+    "--wait",
+    "-w",
+    type=str,
+    required=False,
+    default="10m",
+    help="Wait time. E.g. '30s', or '5m'. Default: 10m. Specify '0' to disable waiting and return immediately.",
 )
 search = click.option(
-    "--search", "-s",
+    "--search",
+    "-s",
     type=str,
     required=False,
-    help="Specify REST search. E.g. 'name $eq something'. Note: use single quote in bash/sh."
+    help="Specify REST search. E.g. 'name $eq something'. Note: use single quote in bash/sh.",
 )
 sort = click.option(
-    "--sort", 
+    "--sort",
     type=str,
     required=False,
     help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
 )
 limit = click.option(
-    "--limit", 
-    type=int, 
-    required=False, 
-    default=20, 
-    help="Optionally, specify the number of records to fetch."
+    "--limit", type=int, required=False, default=20, help="Optionally, specify the number of records to fetch."
 )
 
+
 def get_org_id(org: str) -> str:
     if org:
         return org
 
-    from vhcs.common.sglib import auth
+    from vhcs.sglib import auth
 
     auth_info = auth.details(False)
     if not auth_info:
         raise CtxpException("Not authorized. See 'hcs login --help'.")
     return auth_info.org.id
```

### Comparing `hcs-cli-0.1.48/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.50/vhcs/sglib/csp.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 log = logging.getLogger(__name__)
 
 log_http_details = False
 
 
 def _raise_on_4xx_5xx(response: httpx.Response):
-
     if not response.is_success:
         response.read()
         if len(response.text) > 0:
             text = _try_formatting_json(response.text)
             log.debug(text)
 
     response.raise_for_status()
@@ -60,70 +59,69 @@
     log.debug(f"<-- {request.headers}")
     response.read()
     if len(response.text) > 0:
         text = _try_formatting_json(response.text)
         log.debug(text)
     log.debug("\n")
 
+
 class CspClient:
-    def __init__(self, url: str, oauth_token: dict = None, org_id : str = None) -> None:
+    def __init__(self, url: str, oauth_token: dict = None, org_id: str = None) -> None:
         self._base_url = url
         self._oauth_token = oauth_token
         self._org_id = org_id
 
         self._client = httpx.Client(
             base_url=url,
             timeout=20,
             event_hooks={
                 "request": [_log_request],
                 "response": [_log_response, _raise_on_4xx_5xx],
             },
         )
 
     def login_with_api_token(self, api_token: str) -> dict:
-        #https://console-stg.cloud.vmware.com/csp/gateway/authn/api/swagger-ui.html#/Authentication/getAccessTokenByApiRefreshTokenUsingPOST
+        # https://console-stg.cloud.vmware.com/csp/gateway/authn/api/swagger-ui.html#/Authentication/getAccessTokenByApiRefreshTokenUsingPOST
 
         # curl -X 'POST' \
         # 'https://console.cloud.vmware.com/csp/gateway/am/api/auth/api-tokens/authorize' \
         # -H 'accept: application/json' \
         # -H 'Content-Type: application/x-www-form-urlencoded' \
         # -d 'refresh_token=<the-refresh-token>'
 
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Accept": "application/json",
         }
         # <no org id for this API>
         resp = self._client.post(
-            "/csp/gateway/am/api/auth/api-tokens/authorize",
-            headers=headers,
-            data=f"api_token={api_token}"
+            "/csp/gateway/am/api/auth/api-tokens/authorize", headers=headers, data=f"api_token={api_token}"
         )
         self._oauth_token = resp.json()
         return self._oauth_token
-    
+
     def login_with_client_id_and_secret(self, client_id: str, client_secret: str, org_id: str) -> dict:
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Accept": "application/json",
         }
         params = {
             "grant_type": "client_credentials",
         }
         if org_id:
-            params['orgId'] = org_id
+            params["orgId"] = org_id
         resp = self._client.post(
             "/csp/gateway/am/api/auth/authorize",
             auth=(client_id, client_secret),
             headers=headers,
             params=params,
         )
         self._oauth_token = resp.json()
         return self._oauth_token
-    
+
     # def get_oauth_token(self, force=False):
     #     if self._oauth_token and not force:
     #         return self._oauth_token
 
     #     if self._api_token:
     #         resp = self._login_by_api_token()
     #     elif self._refresh_token:
@@ -169,15 +167,15 @@
     #         params['orgId'] = self._org_id
     #     return self._client.post(
     #         "/csp/gateway/am/api/auth/authorize",
     #         auth=(self._client_id, self._client_key),
     #         headers=headers,
     #         params=params,
     #     )
-    
+
     # def _login_by_refresh_token_from_api_token(self):
     #     #https://console-stg.cloud.vmware.com/csp/gateway/authn/api/swagger-ui.html#/Authentication/getAccessTokenByApiRefreshTokenUsingPOST
 
     #     # curl -X 'POST' \
     #     # 'https://console.cloud.vmware.com/csp/gateway/am/api/auth/api-tokens/authorize' \
     #     # -H 'accept: application/json' \
     #     # -H 'Content-Type: application/x-www-form-urlencoded' \
```

### Comparing `hcs-cli-0.1.48/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.50/vhcs/sglib/ez_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from authlib.integrations.httpx_client import OAuth2Client
 from http.client import HTTPResponse
 import httpx
 from typing import Callable
 import logging
 import json
-from vhcs.common.ctxp import jsondot
+from vhcs.ctxp import jsondot
 
 log = logging.getLogger(__name__)
 
 
 def _raise_on_4xx_5xx(response: httpx.Response):
     if not response.is_success:
         response.read()
@@ -79,50 +79,52 @@
         except:
             log.info("--- Fail parsing json. Dump content ---")
             log.info(resp.content)
             raise
     else:
         return
 
+
 def _is_404(e: httpx.HTTPStatusError) -> bool:
     return e.response.status_code == 404
 
+
 def on404ReturnNone(func):
     try:
         resp = func()
         return _parse_resp(resp)
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 404:
             return None
         raise
 
 
 class EzClient:
     def __init__(self, base_url: str, oauth_client: OAuth2Client = None, lazy_oauth_client: Callable = None) -> None:
-        #self._client = httpx.Client(base_url=base_url, timeout=30, event_hooks=event_hooks)
+        # self._client = httpx.Client(base_url=base_url, timeout=30, event_hooks=event_hooks)
         self._base_url = base_url
         self._client_impl = oauth_client
         self._lazy_oauth_client = lazy_oauth_client
 
     def _client(self):
         if not self._client_impl:
             client = self._lazy_oauth_client()
             client.base_url = self._base_url
             client.timeout = 30
-            request_hooks = client.event_hooks['request']
-            response_hooks = client.event_hooks['response']
+            request_hooks = client.event_hooks["request"]
+            response_hooks = client.event_hooks["response"]
             if _log_request not in request_hooks:
                 request_hooks.append(_log_request)
             if _log_response not in response_hooks:
                 response_hooks.append(_log_response)
             if _raise_on_4xx_5xx not in response_hooks:
                 response_hooks.append(_raise_on_4xx_5xx)
             self._client_impl = client
         return self._client_impl
-    
+
     def post(self, url: str, json: dict = None, text: str = None, headers: dict = None):
         if text:
             resp = self._client().post(url, content=text, headers=headers)
         else:
             resp = self._client().post(url, json=json)
         return _parse_resp(resp)
 
@@ -145,15 +147,15 @@
 
     def delete(self, url: str, raise_on_404: bool = False):
         try:
             resp = self._client().delete(url)
             return _parse_resp(resp)
         except httpx.HTTPStatusError as e:
             if _is_404(e):
-                if raise_on_404: 
+                if raise_on_404:
                     raise
                 else:
                     pass
             else:
                 raise
 
     def put(self, url: str, json: dict):
```

### Comparing `hcs-cli-0.1.48/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.50/vhcs/sglib/hcs_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.common.ctxp import profile
+from vhcs.ctxp import profile
 from .ez_client import EzClient
 from . import auth as auth
 
 
 def hcs_client(url: str) -> EzClient:
     if not url:
         url = profile.current().hcs.url
     if url.endswith("/"):
         url = url[:-1]
 
-    return EzClient(url, lazy_oauth_client = auth.oauth_client)
+    return EzClient(url, lazy_oauth_client=auth.oauth_client)
```

### Comparing `hcs-cli-0.1.48/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.50/vhcs/sglib/login_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,31 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # nanw @ 2023
-#PKCE with authlib: https://docs.authlib.org/en/latest/specs/rfc7636.html
+# PKCE with authlib: https://docs.authlib.org/en/latest/specs/rfc7636.html
 
 import threading
 import webbrowser
 import secrets
 import logging
 from authlib.integrations.httpx_client import OAuth2Client
 from authlib.oauth2.rfc7636 import create_s256_code_challenge
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from urllib.parse import urlparse, parse_qs
 
 log = logging.getLogger(__name__)
 
-_server_address = ('localhost', 10762)
-_callback_url = '/hcs-cli/oauth/callback'
+_server_address = ("localhost", 10762)
+_callback_url = "/hcs-cli/oauth/callback"
 
-_public_client_ids = {
-    'production': '',   # Not ready yet.
-    'staging': 'BbwHlgWt0vFwPUZMJTb5IKltynXjDmb46IO'
-}
+_public_client_ids = {"production": "", "staging": "BbwHlgWt0vFwPUZMJTb5IKltynXjDmb46IO"}  # Not ready yet.
 
 _auth_code_event = threading.Event()
 _state = None
 
 _auth_html = """
 <!DOCTYPE html>
 <html>
@@ -70,160 +67,163 @@
     hcs login --api-token &lt;my-CSP-user-API-token&gt; <br/><br/>
     # Switch to a different profile:<br/>
     hcs profile use <br/><br/>
     </code>
 </body>
 </html>
 """
+
+
 class OAuthCallbackHandler(BaseHTTPRequestHandler):
     def do_GET(self):
-
-        def _respond(code: int, reason: str, content_type: str = 'text/plain'):
+        def _respond(code: int, reason: str, content_type: str = "text/plain"):
             self.send_response(code)
-            self.send_header('Content-type', content_type)
+            self.send_header("Content-type", content_type)
             self.end_headers()
             self.wfile.write(reason.encode())
             self.wfile.flush()
-        
+
         try:
             # Parse the query parameters from the callback URL
             parsed_url = urlparse(self.path)
             log.debug(parsed_url)
-            if parsed_url.path == _callback_url or parsed_url.path == '/hcsadmin/index.html':
+            if parsed_url.path == _callback_url or parsed_url.path == "/hcsadmin/index.html":
                 query_components = parse_qs(parsed_url.query)
-                codes = query_components.get('code', None)
-                states = query_components.get('state', None)
+                codes = query_components.get("code", None)
+                states = query_components.get("state", None)
 
                 # Check if the 'code' parameter is present in the callback URL
                 if not codes:
-                    _respond(400, 'Missing authorization code')
+                    _respond(400, "Missing authorization code")
                     return
                 if not states:
-                    _respond(400, 'Missing state in server response')
+                    _respond(400, "Missing state in server response")
                     return
                 state = states[0]
                 if _state != state:
-                    _respond(401, 'Response state mismatch')
+                    _respond(401, "Response state mismatch")
                     return
-                
+
                 code = codes[0]
                 # Process the authorization code
                 log.debug("auth code", code)
                 _auth_code_event.value = code
-                
+
                 # Send a response back to the client
-                _respond(200, _auth_html, 'text/html')
+                _respond(200, _auth_html, "text/html")
             else:
                 _respond(404, "Not found")
         finally:
             # Terminate the server
             _auth_code_event.set()
-            threading.Thread(target=lambda : self.server.shutdown()).start()
+            threading.Thread(target=lambda: self.server.shutdown()).start()
 
     def log_message(self, *args):
         log.debug(*args)
 
 
 def run_server_async():
     def run_server():
-        log.debug('oauth callback httpd - start')
+        log.debug("oauth callback httpd - start")
         httpd = HTTPServer(_server_address, OAuthCallbackHandler)
         httpd.serve_forever()
-        log.debug('oauth callback httpd - exit')
+        log.debug("oauth callback httpd - exit")
+
     threading.Thread(target=run_server, daemon=True).start()
 
+
 def do_oauth2_pkce(csp_url: str, client_id: str, org_id: str):
-    
     # OAuth2 server details
-    #authorization_endpoint = csp_url + '/csp/gateway/am/api/auth/api-tokens/authorize'
-    discovery_endpoint = csp_url + '/csp/gateway/discovery'
-    token_endpoint = csp_url + '/csp/gateway/am/api/auth/token'
+    # authorization_endpoint = csp_url + '/csp/gateway/am/api/auth/api-tokens/authorize'
+    discovery_endpoint = csp_url + "/csp/gateway/discovery"
+    token_endpoint = csp_url + "/csp/gateway/am/api/auth/token"
 
-    redirect_uri = f'http://{_server_address[0]}:{_server_address[1]}{_callback_url}'
+    redirect_uri = f"http://{_server_address[0]}:{_server_address[1]}{_callback_url}"
 
     # Create an OAuth2Session instance
     session = OAuth2Client(client_id, redirect_uri=redirect_uri)
 
     # Generate a code verifier and code challenge
 
     code_verifier = secrets.token_urlsafe(64)
     code_challenge = create_s256_code_challenge(code_verifier)
-    #code_challenge = CodeChallenge().from_code_verifier(code_verifier)
+    # code_challenge = CodeChallenge().from_code_verifier(code_verifier)
 
     # Create authorization URL
     # https://console-stg.cloud.vmware.com/csp/gateway/authn/api/swagger-ui.html#/Discovery/getDiscoveryUsingGET
     global _state
     authorization_url, _state = session.create_authorization_url(
-        discovery_endpoint,
-        orgId=org_id,
-        code_challenge=code_challenge,
-        code_challenge_method='S256'
+        discovery_endpoint, orgId=org_id, code_challenge=code_challenge, code_challenge_method="S256"
     )
-    
+
     log.debug(authorization_url)
 
     # Redirect the user to the authorization URL
     webbrowser.open(authorization_url, new=0, autoraise=True)
 
     try:
         _auth_code_event.wait()
     except:
-        log.info('Aborted')
+        log.info("Aborted")
         return
     # Once the user is redirected back to your app with an authorization code, exchange it for an access token
     authorization_code = _auth_code_event.value
-    log.debug('authorization_code: %s', authorization_code)
+    log.debug("authorization_code: %s", authorization_code)
     if not authorization_code:
-        log.debug('Login failed')
+        log.debug("Login failed")
         return
 
     token = session.fetch_token(
         token_endpoint,
-        auth=(client_id, ''),  # auth method required by CSP API for PKCE flow
-        authorization_response=redirect_uri + '?code=' + authorization_code,
-        code_verifier=code_verifier
+        auth=(client_id, ""),  # auth method required by CSP API for PKCE flow
+        authorization_response=redirect_uri + "?code=" + authorization_code,
+        code_verifier=code_verifier,
     )
 
-    log.debug('token: %s', token)
+    log.debug("token: %s", token)
     return token
-    
+
+
 def identify_client_id(csp_url: str) -> str:
-    if csp_url.find('console.cloud') >= 0:
-        return _public_client_ids['production']
-    if csp_url.find('console-stg.cloud') >= 0:
-        return _public_client_ids['staging']
+    if csp_url.find("console.cloud") >= 0:
+        return _public_client_ids["production"]
+    if csp_url.find("console-stg.cloud") >= 0:
+        return _public_client_ids["staging"]
     raise Exception("Unknonw CSP url: " + csp_url)
 
 
 def login_via_browser(csp_url: str, org_id: str):
     client_id = identify_client_id(csp_url)
     run_server_async()
     return do_oauth2_pkce(csp_url, client_id, org_id)
 
 
 def create_oauth_client(oauth_token: dict, csp_url: str, fn_on_new_oauth_token):
-    
-    client = OAuth2Client(client_id = identify_client_id(csp_url), 
-                           client_secret = '',  # Required by CSP auth
-                           token = oauth_token, 
-                           token_endpoint = csp_url + '/csp/gateway/am/api/auth/token', 
-                           token_endpoint_auth_method = 'client_secret_basic',
-                           update_token = fn_on_new_oauth_token)
+    client = OAuth2Client(
+        client_id=identify_client_id(csp_url),
+        client_secret="",  # Required by CSP auth
+        token=oauth_token,
+        token_endpoint=csp_url + "/csp/gateway/am/api/auth/token",
+        token_endpoint_auth_method="client_secret_basic",
+        update_token=fn_on_new_oauth_token,
+    )
     return client
-    
+
+
 def refresh_oauth_token(old_oauth_token: dict, csp_url: str):
     client = create_oauth_client(old_oauth_token, csp_url, None)
-    token_endpoint = csp_url + '/csp/gateway/am/api/auth/token'
+    token_endpoint = csp_url + "/csp/gateway/am/api/auth/token"
     new_token = client.refresh_token(token_endpoint)
     return new_token
 
+
 # def _test():
 #     import jwt
 #     import json
 #     csp_url = 'https://console-stg.cloud.vmware.com'
 #     org_id = '06e09ab5-dc8d-413c-bd57-2c1e929a412c' #stg horizonv2-syntest
 #     token = interactive_login_via_browser(csp_url, org_id)
 #     decoded = jwt.decode(token['access_token'], options={"verify_signature": False})
 #     print(json.dumps(decoded, indent=4))
 
 # if __name__ == '__main__':
-#     _test()
+#     _test()
```

### Comparing `hcs-cli-0.1.48/vhcs/common/util.py` & `hcs-cli-0.1.50/vhcs/ctxp/data_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 from os import path
 from typing import Tuple, Any
 import json
 import yaml
 import re
-from vhcs.common.ctxp.util import CtxpException
+from .util import CtxpException
+
 
 def load_data(file_name: str, class_type: str):
     data = load_data_file(file_name)
     if data == None:
         return
     return strict_dict_to_class(data, class_type)
 
-def load_data_file(file_name: str, default = None, format='auto') -> dict | str | None:
+
+def load_data_file(file_name: str, default=None, format="auto") -> dict | str | None:
     if not path.exists(file_name) or not path.isfile(file_name):
         return default
 
-    with open(file_name, encoding='utf-8') as file:
+    with open(file_name, encoding="utf-8") as file:
         text = file.read()
 
     _, ext = path.splitext(file_name)
-    if ext == ".json" or format == 'json':
-        if format != 'auto' and format != 'json':
-            raise Exception(f'File extension does not match specified format. File={file_name}, format={format}')
+    if ext == ".json" or format == "json":
+        if format != "auto" and format != "json":
+            raise CtxpException(f"File extension does not match specified format. File={file_name}, format={format}")
         data = json.loads(text)
-        return default if data == None else data    # handle empty file
-    if ext == ".yaml" or ext == ".yml" or format == 'yml' or format == 'yaml':
-        if format != 'auto' and format != 'yaml' and format != 'yml':
-            raise Exception(f'File extension does not match specified format. File={file_name}, format={format}')
+        return default if data == None else data  # handle empty file
+    if ext == ".yaml" or ext == ".yml" or format == "yml" or format == "yaml":
+        if format != "auto" and format != "yaml" and format != "yml":
+            raise CtxpException(f"File extension does not match specified format. File={file_name}, format={format}")
         data = yaml.safe_load(text)
-        return default if data == None else data    # handle empty file
+        return default if data == None else data  # handle empty file
     return text
 
-def save_data_file(data: dict | list, file_name: str, format: str = 'yaml'):
+
+def save_data_file(data: dict | list, file_name: str, format: str = "yaml"):
     with open(file_name, "w") as file:
-        if format == 'yaml':
+        if format == "yaml":
             # TODO
-            #yaml.safe_dump(data, file, sort_keys=False)
+            # yaml.safe_dump(data, file, sort_keys=False)
             yaml.safe_dump(json.loads(json.dumps(data, default=vars)), file, sort_keys=False)
-        elif format == 'json':
+        elif format == "json":
             json.dump(data, file, indent=4, default=vars)
         else:
-            raise Exception("Invalid format: " + format)
-        
-def strict_dict_to_class(data: dict, class_type):
+            raise CtxpException("Invalid format: " + format)
+
 
+def strict_dict_to_class(data: dict, class_type):
     actual_keys = set(data.keys())
     declared_keys = set(class_type.__annotations__.keys())
     unexpected_fields = actual_keys - declared_keys
     if unexpected_fields:
         raise ValueError(f"Unexpected fields: {unexpected_fields} while deserializing class {class_type.__name__}")
-    
+
     mandatory_keys = set()
     for k in declared_keys:
         if not hasattr(class_type, k):
             mandatory_keys.add(k)
     missing_fields = mandatory_keys - actual_keys
     if missing_fields:
         raise ValueError(f"Missing fields: {class_type.__name__}.{missing_fields}")
@@ -65,30 +68,33 @@
         if isinstance(value, field_type):
             setattr(inst, field_name, value)
             continue
         if isinstance(value, dict):
             value = strict_dict_to_class(value, field_type)
             setattr(inst, field_name, value)
             continue
-        raise ValueError(f"Field '{class_type.__name__}.{field_name}' has an incorrect type. Declared: {field_type}, actual: {type(value)}")
+        raise ValueError(
+            f"Field '{class_type.__name__}.{field_name}' has an incorrect type. Declared: {field_type}, actual: {type(value)}"
+        )
     return inst
 
-def deep_update_object_value(obj, fn_change, _current_path: str = ""):
 
+def deep_update_object_value(obj, fn_change, _current_path: str = ""):
     if isinstance(obj, list):
         for i in range(len(obj)):
             obj[i] = deep_update_object_value(obj[i], fn_change, _current_path + f"[{i}]")
     elif isinstance(obj, dict):
         for k, v in obj.items():
-            item_path = _current_path + '.' + k if _current_path else k
+            item_path = _current_path + "." + k if _current_path else k
             obj[k] = deep_update_object_value(v, fn_change, item_path)
     else:
         obj = fn_change(_current_path, obj)
     return obj
 
+
 def deep_apply_defaults(to_obj: dict, from_obj: dict) -> bool:
     """If a property in to_obj is empty, use the value from from_obj if the same property is not empty"""
     if not from_obj:
         return
     changed = False
     for k, v in to_obj.items():
         v1 = from_obj.get(k)
@@ -99,145 +105,158 @@
             changed = True
             continue
         if isinstance(v, dict):
             if deep_apply_defaults(v, v1):
                 changed = True
     return changed
 
+
 def deep_get_attr(obj: dict, path: str):
-    parts = path.split('.')
+    parts = path.split(".")
     for k in parts:
         try:
             obj = _get_obj_attr(obj, k)
         except KeyError:
-            raise Exception("Property path not found: " + path)
+            raise CtxpException("Property path not found: " + path)
     return obj
 
+
 def deep_set_attr(obj: dict, path: str, value):
-    parts = path.split('.')
+    parts = path.split(".")
     k = None
     try:
         for i in range(len(parts)):
             k = parts[i]
             obj = _get_obj_attr(obj, k)
 
             if i == len(parts) - 2:
                 # found the one before the leaf.
                 _set_obj_attr(obj, parts[i + 1], value)
                 break
         return obj
     except (KeyError, TypeError, IndexError) as e:
-        raise Exception(f"Property path error: {path}. Cause={e}, current={k}, i={i}")
+        raise CtxpException(f"Property path error: {path}. Cause={e}, current={k}, i={i}")
 
-def _get_obj_attr(o, k):
 
+def _get_obj_attr(o, k):
     name, array_index = _parse_array_property_name(k)
 
     if isinstance(o, dict):
         ret = o[name]
     else:
         ret = getattr(o, name)
 
     if array_index != None:
         ret = ret[array_index]
 
     return ret
 
+
 def _set_obj_attr(o, k, v):
     name, array_index = _parse_array_property_name(k)
     if isinstance(o, dict):
         if array_index is None:
             o[name] = v
         else:
             o[name][array_index] = v
     else:
         if array_index is None:
             setattr(o, name, v)
         else:
             array_elem = getattr(o, name)
             array_elem[array_index] = v
 
-_array_index_matcher = re.compile('(.+)\[(\d+)\]')
+
+_array_index_matcher = re.compile("(.+)\[(\d+)\]")
+
+
 def _parse_array_property_name(k: str) -> Tuple[str, int]:
     m = _array_index_matcher.match(k)
     if m:
         return m.group(1), int(m.group(2))
     return k, None
 
+
 def deep_iterate(obj, fn_on_value):
     if isinstance(obj, list) or isinstance(obj, set):
         for v in obj:
             deep_iterate(v, fn_on_value)
     elif isinstance(obj, dict):
         for k, v in obj.items():
             deep_iterate(v, fn_on_value)
     else:
         fn_on_value(obj)
 
+
 def deep_find_variables(obj):
     collector = set()
+
     def fn_on_value(v):
         if not v or not isinstance(v, str):
             return
         matches = re.findall(_pattern_var_only, v)
         if matches:
             m2 = _pattern_var_list.match(v)
             if m2:
                 collector.add(m2.group(2))
             else:
                 for i in matches:
                     collector.add(i)
+
     deep_iterate(obj, fn_on_value)
     return collector
 
-def process_variables(obj: dict, fn_get_var = None):
+
+def process_variables(obj: dict, fn_get_var=None):
     if fn_get_var == None:
+
         def _fn_get_var(name):
             try:
                 return deep_get_attr(obj, name), True
             except:
                 return None, False
+
         fn_get_var = _fn_get_var
 
     total_changed = {}
     while True:
         ret = _process_variables_impl(obj, fn_get_var)
-        total_changed.update(ret['changed'])
-        if not ret['changed']:
+        total_changed.update(ret["changed"])
+        if not ret["changed"]:
             return {
-                'data': ret['data'],
-                'changed': total_changed,
-                'pending': ret['pending'],
+                "data": ret["data"],
+                "changed": total_changed,
+                "pending": ret["pending"],
             }
 
-_pattern_var = re.compile('.*\$\{(.+?)\}.*')
-_pattern_var_only = re.compile('\$\{(.+?)\}')
-_pattern_var_list = re.compile('\$\{\s*\[\s*for\s+(.+?)\s+in\s+(.+?)\s*\:\s*(.+)\s*]\s*\}')
-def _process_variables_impl(obj: dict, fn_get_var = None):
+
+_pattern_var = re.compile(".*\$\{(.+?)\}.*")
+_pattern_var_only = re.compile("\$\{(.+?)\}")
+_pattern_var_list = re.compile("\$\{\s*\[\s*for\s+(.+?)\s+in\s+(.+?)\s*\:\s*(.+)\s*]\s*\}")
+
+
+def _process_variables_impl(obj: dict, fn_get_var=None):
     changed = {}
     pending = {}
 
     def fn_change(path, v):
         resolved, pending_var = resolve_expression(v, fn_get_var, path)
         if pending_var:
             pending[path] = pending_var
         elif resolved != v:
             changed[path] = v
         return resolved
 
     data = deep_update_object_value(obj, fn_change)
-    return {
-        'changed': changed,
-        'pending': pending,
-        'data': data
-    }
+    return {"changed": changed, "pending": pending, "data": data}
+
 
 def resolve_expression(expr, fn_get_value, referencing_attr_path) -> Tuple[Any, str]:
     """Try resolving expression. Returned updated value and None, or value and pending var name"""
-    
+
     if not isinstance(expr, str):
         return expr, None
     # get variable names from expr
     m1 = _pattern_var.match(expr)
     if not m1:
         return expr, None
     m2 = _pattern_var_list.match(expr)
@@ -247,42 +266,58 @@
         src_var_name = m2.group(2)
         mapped_value = m2.group(3)
 
         target_value, found = fn_get_value(src_var_name)
         if not found:
             return expr, src_var_name
         if not isinstance(target_value, list):
-            raise CtxpException(f"Invalid variable value for expression. Expect list, actual {type(target_value).__name__}. attr_path={referencing_attr_path}, src_var_name={src_var_name}")
-        if not mapped_value.startswith(tmp_var_name + '.'):
-            raise CtxpException(f"Unsupported expression. attr_path={referencing_attr_path}, src_var_name={src_var_name}")
-        new_attr_path = mapped_value[len(tmp_var_name) + 1:]
+            raise CtxpException(
+                f"Invalid variable value for expression. Expect list, actual {type(target_value).__name__}. attr_path={referencing_attr_path}, src_var_name={src_var_name}"
+            )
+        if not mapped_value.startswith(tmp_var_name + "."):
+            raise CtxpException(
+                f"Unsupported expression. attr_path={referencing_attr_path}, src_var_name={src_var_name}"
+            )
+        new_attr_path = mapped_value[len(tmp_var_name) + 1 :]
         ret = []
         for i in target_value:
-            item = deep_get_attr(i, new_attr_path)
+            if i == None:
+                # raise CtxpException(f"Invalid value encountered during processing array expansion expression. The value in the referenced array is None. This is normally a problem of the data, not the caller. attr_path={referencing_attr_path}, src_var_name={src_var_name}")
+                # There are valid cases that some of such items are null. Raising exception
+                # makes the handling hard. Pass-on null in such scenario, so enable the downstream
+                # components to decide what to do with the null case.
+                item = None
+            else:
+                item = deep_get_attr(i, new_attr_path)
             ret.append(item)
-        return ret, None  #replace the entire value using the new value.
+        return ret, None  # replace the entire value using the new value.
     else:
         var_name = m1.group(1)
         # string replacement
         actual_value, found = fn_get_value(var_name)
         if not found:
             return expr, var_name
         if isinstance(actual_value, str):
-            return expr.replace('${' + var_name + '}', actual_value), None
+            return expr.replace("${" + var_name + "}", actual_value), None
         # replacement is an object. Make sure this var is the entire value.
         if len(expr) != len(var_name) + 3:
-            raise CtxpException(f"Invalid variable: can not replace variable in string with non-string. attr_path={referencing_attr_path}, var_name={var_name}, replacement={actual_value}, expr={expr}")
+            raise CtxpException(
+                f"Invalid variable: can not replace variable in string with non-string. attr_path={referencing_attr_path}, var_name={var_name}, replacement={actual_value}, expr={expr}"
+            )
         return actual_value, None
-        
+
+
 def to_json(o) -> str:
     class SetEncoder(json.JSONEncoder):
         def default(self, obj):
             if isinstance(obj, set):
                 return list(obj)
             return json.JSONEncoder.default(self, obj)
+
     return json.dumps(o, cls=SetEncoder, indent=4)
 
+
 def get_common_items(iter1, iter2):
     set1 = set(iter1)
     set2 = set(iter2)
     common_items = set1.intersection(set2)
-    return common_items
+    return common_items
```

### Comparing `hcs-cli-0.1.48/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.50/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/plan/base_provider.py` & `hcs-cli-0.1.50/vhcs/plan/base_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
 Copyright 2023-2023 VMware Inc.
 SPDX-License-Identifier: Apache-2.0
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
@@ -14,16 +13,16 @@
 limitations under the License.
 """
 
 from abc import ABC, abstractmethod
 from typing import Callable
 from .actions import actions
 
-class BaseProvider(ABC):
 
+class BaseProvider(ABC):
     def __init__(self, data: dict, state: dict, fn_save_state: Callable):
         self.data = data
         self.state = state
         self._save_state = fn_save_state
 
     def save(self, data: dict):
         self._save_state(data)
@@ -40,11 +39,11 @@
         pass
 
     @abstractmethod
     def delete(self) -> dict:
         pass
 
     def eta_create(self):
-        return '1m'
+        return "1m"
 
     def eta_delete(self):
-        return '1m'
+        return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/core.py` & `hcs-cli-0.1.50/vhcs/plan/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,413 +15,494 @@
 
 import threading
 import typing
 import inspect
 import re
 from subprocess import CalledProcessError
 from copy import deepcopy
-import vhcs.common.util as util
+import vhcs.ctxp.data_util as data_util
 from . import dag
 from . import context
 from .helper import PlanException, process_template
 from .actions import actions
 from .kop import KOP
 from importlib import import_module
 
 import logging
+
 log = logging.getLogger(__name__)
 log.setLevel(logging.INFO)
 
+
 def _prepare_data(data: dict, additional_context: dict, target_resource_name: str):
     if additional_context:
-        common_items = util.get_common_items(additional_context.keys(), data.keys())
+        common_items = data_util.get_common_items(additional_context.keys(), data.keys())
         if common_items:
             raise PlanException("blueprint and context have conflict keys: " + str(common_items))
         data.update(additional_context)
     blueprint, pending = process_template(data)
-    if target_resource_name and target_resource_name not in blueprint['resources'] and target_resource_name not in blueprint.get('runtimes', {}):
+
+    if (
+        target_resource_name
+        and target_resource_name not in blueprint["resources"]
+        and target_resource_name not in blueprint["runtimes"]
+    ):
         raise PlanException("Target resource or runtime not found: " + target_resource_name)
-    
+
     for k, v in pending.items():
-        if v.startswith('defaults.') or v.startswith('vars.'):
+        if v.startswith("defaults.") or v.startswith("vars."):
             if not k.find(".conditions."):
-                raise PlanException(f"Invalid blueprint. Unresolved static references. Variable not found: {v}. Required by {k}")
-    deployment_id = blueprint['deploymentId']
-    state_file = deployment_id + '.state.yml'
-    prev = util.load_data_file(state_file, default={})
-    state = {'pending': pending}
+                raise PlanException(
+                    f"Invalid blueprint. Unresolved static references. Variable not found: {v}. Required by {k}"
+                )
+    deployment_id = blueprint["deploymentId"]
+    state_file = deployment_id + ".state.yml"
+    prev = data_util.load_data_file(state_file, default={})
+    state = {"pending": pending}
     state.update(blueprint)
-    if 'providers' not in state:
-        state['providers'] = {}
-    if 'runtimes' not in state:
-        state['runtimes'] = {}
-    state['output'] = prev.get('output', {})
-    state['destroy_output'] = prev.get('destroy_output', {})
-    state['log'] = prev.get('log', {})
-    exec_log = state['log']
-    if 'create' not in exec_log:
-        exec_log['create'] = []
-    if 'delete' not in exec_log:
-        exec_log['delete'] = []
+    if "providers" not in state:
+        state["providers"] = {}
+    if "runtimes" not in state:
+        state["runtimes"] = {}
+    state["output"] = prev.get("output", {})
+    state["destroy_output"] = prev.get("destroy_output", {})
+    state["log"] = prev.get("log", {})
+    exec_log = state["log"]
+    if "create" not in exec_log:
+        exec_log["create"] = []
+    if "delete" not in exec_log:
+        exec_log["delete"] = []
+
+    context.set("deploymentId", state["deploymentId"])
 
-    context.set('deploymentId', state['deploymentId'])
-    
     # try solving more variables
     # for k, v in state['output'].items():
     #     if not v:
     #         continue
     #     if not _has_successful_deployment(state, k):
     #         continue
     #     _resolve_pending_keys(state, k)
-    
+
     return blueprint, state, state_file
 
+
 # def _has_successful_deployment(state, name):
 #     for v in state['log']['create']:
 #         if v['name'] != name:
 #             continue
 #         if v['action'] == 'success':
 #             return True
-        
-def deploy(data: dict, additional_context: dict = None, target_resource_name: str = None, include_dependencies: bool = True, concurrency: int = 4):
-    
+
+
+def apply(
+    data: dict,
+    additional_context: dict = None,
+    target_resource_name: str = None,
+    include_dependencies: bool = True,
+    concurrency: int = 4,
+):
     blueprint, state, state_file = _prepare_data(data, additional_context, target_resource_name)
-    state['log']['create'] = []    # clear deploy log
+    state["log"]["create"] = []  # clear deploy log
 
     def deploy_resource_or_runtime(name, res_data):
         _deploy_res(name, res_data, state)
-        util.save_data_file(state, state_file)
+        data_util.save_data_file(state, state_file)
 
     def process_resource_node(name: str):
-        if name in blueprint['resources']:
-            res_data = blueprint['resources'][name]
+        if name in blueprint["resources"]:
+            res_data = blueprint["resources"][name]
             return deploy_resource_or_runtime(name, res_data)
-        elif name in blueprint.get('runtimes', {}):
-            res_data = blueprint['runtimes'][name]
+        elif name in blueprint["runtimes"]:
+            res_data = blueprint["runtimes"][name]
             return deploy_resource_or_runtime(name, res_data)
-        elif name in blueprint.get('providers', {}):
+        elif name in blueprint["providers"]:
             # ignore.
-            # Provide init is always ensured before running the resource 
+            # Provide init is always ensured before running the resource
             # and does not follow deploy/destroy sequenct.
             pass
         else:
             # defaults, vars, etc.
             pass
+
     try:
-        dag.process_blueprint(blueprint, process_resource_node, False, concurrency, target_resource_name, include_dependencies)
+        dag.process_blueprint(
+            blueprint=blueprint,
+            fn_process_node=process_resource_node,
+            continue_on_error=False,
+            reverse=False,
+            concurrency=concurrency,
+            target_node_name=target_resource_name,
+            include_dependencies=include_dependencies,
+        )
     except CalledProcessError as e:
         raise PlanException(str(e))
     finally:
-        util.save_data_file(state, state_file)
+        data_util.save_data_file(state, state_file)
 
 
-def _parse_statement_for(name, state) -> typing.Tuple[str, list]:
+def _parse_statement_for(res_name, state) -> typing.Tuple[str, list]:
     # for: email in vars.userEmails
-    res = state['resources'][name]
-    for_statement = res.get('for')
+    res = state["resources"][res_name]
+    for_statement = res.get("for")
     if not for_statement:
         return None, None
-    pattern = r'(.+?)\s+in\s+(.+)'
+    pattern = r"(.+?)\s+in\s+(.+)"
     matcher = re.search(pattern, for_statement)
 
     def _raise_error(reason):
-        raise PlanException(f"Invalid for statement: {reason}. Resource={name}, statement={for_statement}")
-    
+        raise PlanException(f"Invalid for statement: {reason}. Resource={res_name}, statement={for_statement}")
+
     if not matcher:
-        _raise_error('Invalid syntax')
+        _raise_error("Invalid syntax")
     var_name = matcher.group(1)
     values_name = matcher.group(2)
-    values = _get_value_by_path(state, values_name, f"resources.{name}.for")
+    values = _get_value_by_path(state, values_name, f"resources.{res_name}.for")
     if not isinstance(values, list):
-        reason = 'The referencing value is not a list. Actual type=' + type(values).__name__
+        reason = "The referencing value is not a list. Actual type=" + type(values).__name__
         _raise_error(reason)
 
     return var_name, values
 
+
 def _get_value_by_path(state, var_name, required_by_attr_path):
-    i = var_name.find('.')
+    i = var_name.find(".")
     if i < 0:
         resource_name = var_name
     else:
         resource_name = var_name[:i]
 
     def _raise(e):
         msg = f"Plugin error: '{var_name}' does not exist in the output of resource '{resource_name}', which is required by '{required_by_attr_path}'"
         raise PlanException(msg) from e
-    
-    if resource_name in state['resources']:
+
+    if resource_name in state["resources"]:
         try:
-            return util.deep_get_attr(state, "output." + var_name)
+            return data_util.deep_get_attr(state, "output." + var_name)
         except Exception as e:
             _raise(e)
     if resource_name in state:
         try:
-            return util.deep_get_attr(state, var_name)
+            return data_util.deep_get_attr(state, var_name)
         except Exception as e:
             _raise(e)
 
+
 def _get_value_by_path2(state, var_name):
-    i = var_name.find('.')
+    i = var_name.find(".")
     if i < 0:
         resource_name = var_name
     else:
         resource_name = var_name[:i]
 
-    if resource_name in state['resources'] or resource_name in state['runtimes'] or resource_name in state['providers']:
+    if resource_name in state["resources"] or resource_name in state["runtimes"] or resource_name in state["providers"]:
         try:
-            return util.deep_get_attr(state, "output." + var_name), True
+            return data_util.deep_get_attr(state, "output." + var_name), True
         except Exception as e:
             log.debug(e)
             return None, False
-        
+
     if resource_name in state:
         try:
-            return util.deep_get_attr(state, var_name), True
+            return data_util.deep_get_attr(state, var_name), True
         except Exception as e:
             log.debug(e)
             return None, False
     return None, False
 
+
 def _deploy_res(name, res, state):
     def fn_deploy1(handler, res_data: dict, res_state: dict, fn_set_state: typing.Callable, kop: KOP):
         if _is_runtime(res):
-            kop.start(KOP.MODE.create, handler.eta('create', res_data, state))
+            kop.start(KOP.MODE.create, handler.eta("create", res_data, state))
             new_state = handler.process(res_data, deepcopy(state))
             if new_state:
                 fn_set_state(new_state)
             return
-        
+
         if not res_state:
             action = actions.create
         else:
             action = handler.decide(res_data, res_state)
-            
+
         if action == actions.skip:
-            kop.skip('Already deployed')
+            kop.skip("Already deployed")
             return
-        
+
         if action == actions.recreate:
-            with KOP(state, res['kind'], name) as kop2:
-                kop2.id(res_state.get('id'))
+            with KOP(state, res["kind"], name) as kop2:
+                kop2.id(res_state.get("id"))
                 kop2.start(KOP.MODE.delete, handler.eta(actions.delete, res_data, res_state))
                 handler.destroy(res_data, res_state, False)
             action = actions.create
 
         new_state = None
         if action == actions.create or action == None:
             kop.start(KOP.MODE.create, handler.eta(actions.create, res_data, res_state))
             if _has_save_state(handler.deploy):
                 new_state = handler.deploy(res_data, res_state, fn_set_state)
             else:
                 new_state = handler.deploy(res_data, res_state)
             kop.id(_discover_id(new_state))
         elif action == actions.update:
-            kop.id(res_state.get('id'))
+            kop.id(res_state.get("id"))
             kop.start(KOP.MODE.update, handler.eta(actions.update, res_data, res_state))
             if _has_save_state(handler.update):
                 new_state = handler.update(res_data, res_state, fn_set_state)
             else:
                 new_state = handler.update(res_data, res_state)
         else:
-            raise PlanException(f"Unknown action. This is a problem of the concrete plugin.decide function. Plugin={name}, action={action}")
-        
+            raise PlanException(
+                f"Unknown action. This is a problem of the concrete plugin.decide function. Plugin={name}, action={action}"
+            )
+
         if new_state:
             fn_set_state(new_state)
+
     _handle_resource(name, res, state, True, fn_deploy1)
 
+
 def _is_runtime(res):
-    return 'impl' in res
+    return "impl" in res
+
 
 def _has_save_state(fn):
     signature = inspect.signature(fn)
     args = list(signature.parameters.keys())
     if len(args) < 3:
         return False
     name = args[2]
-    if name == 'save_state':
+    if name == "save_state":
         return True
     p = signature.parameters[args[2]]
     return p.annotation == typing.Callable
 
+
 def _assert_all_vars_resolved(data, name):
     def fn_on_value(path, value):
-        if isinstance(value, str) and value.find('${') >= 0:
+        if isinstance(value, str) and value.find("${") >= 0:
             raise PlanException(f"Unresolved variable '{path}' for plugin '{name}'. Value={value}")
         return value
-    util.deep_update_object_value(data, fn_on_value)
+
+    data_util.deep_update_object_value(data, fn_on_value)
+
 
 _providers = {}
 _provider_lock = threading.Lock()
+
+
 def _ensure_provider(provider_id: str, state: dict):
     # Ensure provider initialized
     with _provider_lock:
         if not provider_id in _providers:
             provider = import_module("vhcs.plan.provider." + provider_id)
             # Get provider data
-            meta = state['providers'].get(provider_id)
+            meta = state["providers"].get(provider_id)
+
             def _get_value(path):
                 return _get_value_by_path2(state, path)
-            util.process_variables(meta, _get_value)
 
-            data = meta.get('data') if meta else None
+            data_util.process_variables(meta, _get_value)
+
+            data = meta.get("data") if meta else None
             if data:
                 _assert_all_vars_resolved(data, provider_id)
             else:
                 data = {}
             log.debug("[init] Provider: %s", provider_id)
-            state['output'][provider_id] = provider.prepare(data)
+            state["output"][provider_id] = provider.prepare(data)
             log.debug("[ok  ] Provider: %s", provider_id)
             _providers[provider_id] = 1
 
+
 def _get_resource_handler(kind: str, state: dict):
-    provider_id, res_handler_type = kind.split('/')
-    res_handler_type = res_handler_type.replace('-', '_')
+    provider_id, res_handler_type = kind.split("/")
+    res_handler_type = res_handler_type.replace("-", "_")
     _ensure_provider(provider_id, state)
     module_name = f"vhcs.plan.provider.{provider_id}.{res_handler_type}"
     return import_module(module_name)
 
+
 def _get_runtime_handler(impl_name: str):
     return import_module(impl_name)
 
+
 def get_common_items(iter1, iter2):
     return set(iter1).intersection(set(iter2))
 
+
 def _handle_resource(name, res, state, for_deploy: bool, fn_process: typing.Callable):
-    if 'kind' in res:
-        kind = res['kind']
-    elif 'impl' in res:
-        kind = 'runtime'
+    if "kind" in res:
+        kind = res["kind"]
+    elif "impl" in res:
+        kind = "runtime"
     else:
         raise PlanException("Invalid definition. Neither kind nor impl attribute found. Resource name: " + name)
 
     kop_mode = KOP.MODE.create if for_deploy else KOP.MODE.delete
     with KOP(state, kind, name, kop_mode) as kop:
 
         def _get_value(path):
             return _get_value_by_path2(state, path)
-        
-        conditions = res.get('conditions')
+
+        conditions = res.get("conditions")
         if conditions:
             conditions = deepcopy(conditions)
-            ret = util.process_variables(conditions, _get_value)
+            ret = data_util.process_variables(conditions, _get_value)
             unsatisfied_condition_name = _get_unsatisfied_condition_name(conditions)
             if unsatisfied_condition_name:
-                kop.skip('Condition not met: ' + unsatisfied_condition_name)
+                kop.skip("Condition not met: " + unsatisfied_condition_name)
                 return
-            
+
         # resolve vars
-        data = res.get('data', {})
+        data = res.get("data", {})
         if data:
             data = deepcopy(data)
-            ret = util.process_variables(data, _get_value)
+            ret = data_util.process_variables(data, _get_value)
             if for_deploy:
-                if ret['pending']:
+                if ret["pending"]:
                     msg = f"Fail resolving variables for resource '{name}'. Unresolvable variables: {ret['pending']}"
                     raise PlanException(msg)
-        state['resources'][name] = dict(res)
-        state['resources'][name]['data'] = data
+        state["resources"][name] = dict(res)
+        state["resources"][name]["data"] = data
 
-        if kind == 'runtime':
-            handler = _get_runtime_handler(res['impl'])
+        if kind == "runtime":
+            handler = _get_runtime_handler(res["impl"])
         else:
             handler = _get_resource_handler(kind, state)
 
         def _handle_resource_1(resource_data, resource_state, fn_set_state, kop) -> bool:
-            if _is_runtime(res):   # runtime has no refresh
+            if _is_runtime(res):  # runtime has no refresh
                 pass
             else:
                 new_state = handler.refresh(resource_data, resource_state)
                 fn_set_state(new_state)
                 resource_state = new_state
 
             fn_process(handler, resource_data, resource_state, fn_set_state, kop)
 
         for_var_name, values = _parse_statement_for(name, state)
         if for_var_name:
             if for_var_name in data:
-                raise PlanException(f"Invalid blueprint: variable name defined in for-statement already exists in data declaration. Resource: {name}. Conflicting names: {common}")
-            kop.id('(group)')
+                raise PlanException(
+                    f"Invalid blueprint: variable name defined in for-statement already exists in data declaration. Resource: {name}. Conflicting names: {for_var_name}"
+                )
+            kop.id("(group)")
             kop.start()
             size = len(values)
             # ensure output array placeholder
-            output = state['output'].setdefault(name, [])
+            output = state["output"].get(name)
+            if not output:
+                output = []
+                state["output"][name] = output
             while len(output) < size:
                 output.append(None)
             for i in range(size):
                 v = values[i]
-                with KOP(state, kind, name + f'#{i}', kop_mode) as kop_per_item:
+                with KOP(state, kind, name + f"#{i}", kop_mode) as kop_per_item:
                     kop_per_item.id(str(i))
                     resource_state = output[i]
+
                     def _fn_set_state(o):
                         output[i] = deepcopy(o)
+
                     resource_data = deepcopy(data)
                     resource_data[for_var_name] = v
-                    _handle_resource_1(resource_data, resource_state, _fn_set_state, kop_per_item)
+                    if v == None:
+                        kop_per_item.skip("No input data")
+                    else:
+                        _handle_resource_1(resource_data, resource_state, _fn_set_state, kop_per_item)
         else:
-            resource_state = state['output'].get(name)
+            resource_state = state["output"].get(name)
+
             def _fn_set_state(o):
-                state['output'][name] = deepcopy(o)
+                state["output"][name] = deepcopy(o)
+
             resource_data = deepcopy(data)
             _handle_resource_1(resource_data, resource_state, _fn_set_state, kop)
 
+
 def _get_unsatisfied_condition_name(conditions):
     if not conditions:
         return
     for condition_name, expr in conditions.items():
         if not expr:
             return condition_name
-        if expr.find('${') >= 0: # still have unresolved variables
-            return condition_name
+        if isinstance(expr, str):
+            if expr.find("${") >= 0:  # still have unresolved variables
+                return condition_name
+        # expr could be an object. It's already "True". So skip.
 
 
 def _discover_id(obj):
     if isinstance(obj, dict):
-        return obj.get('id')
+        return obj.get("id")
+
 
 def _destroy_res(name, res_node, state, force):
     def fn_destroy1(handler, res_data: dict, res_state: dict, fn_set_state: typing.Callable, kop: KOP):
         if not res_state:
-            kop.skip('Not found')
+            kop.skip("Not found")
             return
         kop.id(_discover_id(res_state))
         kop.start(KOP.MODE.delete, handler.eta(actions.delete, res_data, res_state))
         ret = handler.destroy(res_data, res_state, force)
-        state['destroy_output'][name] = deepcopy(ret)
-        fn_set_state(None)
+        state["destroy_output"][name] = deepcopy(ret)
+
+        if _is_runtime(res_node):
+            # No set empty data for runtime. Runtime is special and normally the data needs to be referenced in the next run.
+            pass
+        else:
+            fn_set_state(None)
 
     _handle_resource(name, res_node, state, False, fn_destroy1)
 
-def destroy(data, force: bool, target_resource_name: str = None, include_related_resources: bool = True, concurrency: int = 4, additional_context: dict = None):
-    
+
+def destroy(
+    data,
+    force: bool,
+    target_resource_name: str = None,
+    include_dependencies: bool = True,
+    concurrency: int = 4,
+    additional_context: dict = None,
+):
     blueprint, state, state_file = _prepare_data(data, additional_context, target_resource_name)
-    state['log']['delete'] = []    # clear destroy log
+    state["log"]["delete"] = []  # clear destroy log
 
     def destroy_resource(node_name):
         # ignore functional nodes (defaults, providers)
-        node = blueprint['resources'].get(node_name)
+        node = blueprint["resources"].get(node_name)
+        if not node:
+            node = blueprint["runtimes"].get(node_name)
+
         if not node:
             return dag.walker.next
-        # skip runtime
-        if node['kind'].startswith('runtime/'):
-            return dag.walker.next
-        
-        res_node = state['resources'].get(node_name)
-        if not res_node:
-            res_node = blueprint['resources'][node_name]
 
-        _destroy_res(node_name, res_node, state, force)
-        util.save_data_file(state, state_file)
+        _destroy_res(node_name, node, state, force)
+        data_util.save_data_file(state, state_file)
         return dag.walker.next
-            
 
     try:
-        dag.process_blueprint(blueprint, destroy_resource, True, concurrency)
+        dag.process_blueprint(
+            blueprint=blueprint,
+            fn_process_node=destroy_resource,
+            continue_on_error=force,
+            reverse=True,
+            concurrency=concurrency,
+            target_node_name=target_resource_name,
+            include_dependencies=include_dependencies,
+        )
     except CalledProcessError as e:
         raise PlanException(str(e))
     finally:
-        util.save_data_file(state, state_file)
+        data_util.save_data_file(state, state_file)
+
 
-def graph(data: dict, additional_context: dict = None, reverse: bool = False, target_resource: str = None, include_dependencies: bool = True):
+def graph(
+    data: dict,
+    additional_context: dict = None,
+    reverse: bool = False,
+    target_resource: str = None,
+    include_dependencies: bool = True,
+):
     blueprint, state, state_file = _prepare_data(data, additional_context, None)
     g = dag.graph(blueprint, state, reverse, target_resource, include_dependencies)
     return g
-
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/dag.py` & `hcs-cli-0.1.50/vhcs/plan/dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,134 +18,147 @@
 import threading
 from graphlib import TopologicalSorter
 from graphviz import Digraph
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Callable
 import atexit
 
+
 class walker:
-    next = 'next'
-    stop = 'stop'
+    next = "next"
+    stop = "stop"
+
 
 class _NodeType:
-    vars = 'vars'
-    const = 'const'
-    provider = 'provider'
-    resource = 'resource'
-    runtime = 'runtime'
+    vars = "vars"
+    const = "const"
+    provider = "provider"
+    resource = "resource"
+    runtime = "runtime"
+
 
 class DAG:
     graph: dict[str, set[str]]
     data: dict[str, Any]
 
     def __init__(self):
         self.graph = {}
         self.data = {}
         self.extra_source = []
 
-    def add(self, id: str, type: str, data: Any, dependencies = None):
+    def add(self, id: str, type: str, data: Any, dependencies=None):
         if id in self.data:
-            raise Exception('Node already added to graph: ' + id)
-        self.data[id] = {
-            'type': type,
-            'data': data
-        }
+            raise Exception("Node already added to graph: " + id)
+        self.data[id] = {"type": type, "data": data}
         self.graph[id] = set(dependencies) if dependencies else set()
 
     def validate(self, extra):
         all_keys = self.data.keys()
         for k, v in self.graph.items():
             for d in v:
                 if d in all_keys:
                     continue
                 if d in extra:
                     continue
                 raise Exception(f"Blueprint error: target dpendency not found: from={k}, target={d}")
-    
-def process_blueprint(blueprint, fn_process_node: Callable, reverse: bool, concurrency: int = 3, target_node_name: str = None, include_dependencies: bool = True):
+
+
+def process_blueprint(
+    blueprint,
+    fn_process_node: Callable,
+    continue_on_error: bool = False,
+    reverse: bool = False,
+    concurrency: int = 3,
+    target_node_name: str = None,
+    include_dependencies: bool = True,
+):
     dag = _build_graph(blueprint, reverse, target_node_name, include_dependencies)
-    return _walkthrough(dag, fn_process_node, concurrency)
+    return _walkthrough(dag, fn_process_node, continue_on_error, concurrency)
+
 
 def _filter_dag_by_target_node(dag: DAG, target_node_name, include_dependencies):
     if include_dependencies:
         # Remove all nodes that are not dependencies (both direct and indirect) of the target
         all_nodes = set(dag.graph.keys())
         dependencies = set()
         dependencies.add(target_node_name)
         open_nodes = set(dag.graph[target_node_name])
         while open_nodes:
             n = open_nodes.pop()
             if n in dependencies:
                 continue
             dependencies.add(n)
             open_nodes |= dag.graph[n]
-        
+
         to_delete = set(dag.graph.keys()) - dependencies
         for n in to_delete:
             del dag.graph[n]
             del dag.data[n]
     else:
         # keep only the target node
-        dag.data = {
-            target_node_name: dag.data[target_node_name]
-        }
-        dag.graph = {
-            target_node_name: set()
-        }
+        dag.data = {target_node_name: dag.data[target_node_name]}
+        dag.graph = {target_node_name: set()}
     pass
 
+
 def _build_graph(blueprint, reverse: bool, target_node_name: str, include_dependencies: bool):
     dag = DAG()
     extra = blueprint.keys()
 
-    from vhcs.common import util
+    from vhcs.ctxp import data_util
+
     def add_node(name, type, obj):
         dependencies = set()
 
         # identify dependencies due to variables
-        variables = util.deep_find_variables(obj)
+        variables = data_util.deep_find_variables(obj)
         for v in variables:
-            i = v.find('.')
+            i = v.find(".")
             resource_name = v if i < 0 else v[:i]
-            if resource_name == 'vars':
-                continue    # ignore dependencies to vars, which is a common thing.
+            if resource_name == "vars":
+                continue  # ignore dependencies to vars, which is a common thing.
             dependencies.add(resource_name)
 
         # identify dependencies due to explicit "after" statement
-        after = obj.get('after')
+        after = obj.get("after")
         if after:
+
             def _add(t):
                 if t in dependencies:
-                    raise Exception("Invalid blueprint: statement after contains a dependency that is already implicitly created. This is not necessary. Key: " + t)
+                    raise Exception(
+                        "Invalid blueprint: statement after contains a dependency that is already implicitly created. This is not necessary. Key: "
+                        + t
+                    )
                 dependencies.add(t)
+
             if isinstance(after, str):
                 _add(after)
             else:
                 for v in after:
                     _add(v)
-        
+
         # identify dependencies due to provider
         if type == _NodeType.resource:
             provider_type = _get_provider_id(obj)
             dependencies.add(provider_type)
         dag.add(name, type, obj, dependencies)
-    
+
     required_providers = set()
-    for k,v in blueprint['resources'].items():
+    for k, v in blueprint["resources"].items():
         required_providers.add(_get_provider_id(v))
         add_node(k, _NodeType.resource, v)
-    for k, v in blueprint.get('runtimes', {}).items():
+    for k, v in blueprint["runtimes"].items():
         add_node(k, _NodeType.runtime, v)
-    defaults = blueprint.get('defaults')
+    defaults = blueprint["defaults"]
     if defaults:
-        add_node('defaults', _NodeType.const, defaults)
-    vars = blueprint.get('vars')
+        add_node("defaults", _NodeType.const, defaults)
+    vars = blueprint["vars"]
     if vars:
-        add_node('vars', _NodeType.vars, vars)
-    providers = blueprint.get('providers')
+        add_node("vars", _NodeType.vars, vars)
+    providers = blueprint["providers"]
     if providers:
         for provider_id, data in providers.items():
             add_node(provider_id, _NodeType.provider, data)
     # Provider config is optional. Add place-holder nodes for all missing providers.
     for provider_id in required_providers:
         if provider_id not in dag.data:
             add_node(provider_id, _NodeType.provider, {})
@@ -155,171 +168,166 @@
     if reverse:
         _reverse_dag(dag)
     if target_node_name:
         _filter_dag_by_target_node(dag, target_node_name, include_dependencies)
 
     return dag
 
+
 def _get_provider_id(node_data):
-    kind = node_data['kind']
-    provider_type = kind[:kind.find('/')]
-    if provider_type == 'runtime':
+    kind = node_data["kind"]
+    provider_type = kind[: kind.find("/")]
+    if provider_type == "runtime":
         raise Exception("This is a regression bug. Must not be runtime here")
     return provider_type
 
 
-def _walkthrough(dag: DAG, fn_process_node: Callable, concurrency: int):
+def _walkthrough(dag: DAG, fn_process_node: Callable, continue_on_error: bool, concurrency: int):
     topological_sorter = TopologicalSorter(dag.graph)
     topological_sorter.prepare()
     lock = threading.Lock()
 
-    flags = {
-        'err': None,
-        'stop': False
-    }
+    flags = {"err": None, "stop": False}
 
     def process_node(node_id):
         try:
             ret = fn_process_node(node_id)
             with lock:
                 if ret == walker.stop:
-                    flags['stop'] = True
+                    flags["stop"] = True
                 topological_sorter.done(node_id)
         except Exception as e:
             with lock:
-                flags['err'] = e
+                flags["err"] = e
+                if continue_on_error:
+                    topological_sorter.done(node_id)
 
     with ThreadPoolExecutor(max_workers=concurrency) as executor:
 
         def close():
-            flags['stop'] = True
+            flags["stop"] = True
             executor.shutdown(wait=False, cancel_futures=True)
 
         atexit.register(close)
-        
+
         while topological_sorter.is_active():
             with lock:
-                if flags['err'] or flags['stop']:
+                if flags["stop"]:
+                    break
+                if not continue_on_error and flags["err"]:
                     break
                 read_nodes = topological_sorter.get_ready()
             if not len(read_nodes):
                 time.sleep(0.1)
                 continue
             for node in read_nodes:
                 executor.submit(process_node, node)
         executor.shutdown(wait=True)
-        if flags['err']:
-            raise flags['err']
-        
+        if flags["err"]:
+            raise flags["err"]
+
         atexit.unregister(close)
-        
+
+
 def _has_indirect_dependency(tree: dict, from_node: str, to_node: str):
     deps = list(tree[from_node])
     deps.remove(to_node)
     while deps:
         n = deps.pop()
         new_deps = tree[n]
         if to_node in new_deps:
             return True
         deps += new_deps
     return False
 
+
 def graph(blueprint: dict, state: dict, reverse: bool, target_resource: str, include_dependencies: bool) -> Digraph:
     dag = _build_graph(blueprint, reverse, target_resource, include_dependencies)
     topological_sorter = TopologicalSorter(dag.graph)
     sorted_nodes = list(topological_sorter.static_order())
     graph = Digraph(name=f"Deployment {blueprint['deploymentId']}", comment="Simplified")
-    
+
     class styles:
-        deployed = {
-            'style': 'filled',
-            'fillcolor': 'lightgrey'
-        }
+        deployed = {"style": "filled", "fillcolor": "lightgrey"}
 
     # https://graphviz.org/doc/info/shapes.html#:~:text=There%20are%20three%20main%20types,and%20an%20HTML%2Dlike%20label.
     node_type_style_map = {
-        _NodeType.const: {
-            'shape': 'tab'
-        },
-        _NodeType.provider: {
-            'shape': 'component'
-        },
+        _NodeType.const: {"shape": "tab"},
+        _NodeType.provider: {"shape": "component"},
         _NodeType.resource: {
             # empty
         },
-        _NodeType.vars: {
-            'shape': 'note'
-        },
-        _NodeType.runtime: {
-            'shape': 'hexagon'
-        }
+        _NodeType.vars: {"shape": "note"},
+        _NodeType.runtime: {"shape": "hexagon"},
     }
+
     def _is_deployed(node_name):
-        data = state['output'].get(node_name)
+        data = state["output"].get(node_name)
         if isinstance(data, list):
             return any(d for d in data)
         return data
 
     def _get_node_style(node_name):
         n = dag.data[node_name]
-        attr = {} | node_type_style_map[n['type']]
+        attr = {} | node_type_style_map[n["type"]]
         if _is_deployed(node_name):
             attr |= styles.deployed
         return attr
-    
+
     for node in sorted_nodes:
         attrs = _get_node_style(node)
         graph.node(node, **attrs)
 
     # Add the edges based on the dependencies
     for node, dependencies in dag.graph.items():
         for dependency in dependencies:
             if _has_indirect_dependency(dag.graph, from_node=node, to_node=dependency):
-                continue    #simplify the diagram by removing ommitable 
+                continue  # simplify the diagram by removing ommitable
             graph.edge(dependency, node)
 
     return graph
 
+
 def _reverse_dag(dag: DAG):
     old_dep = deepcopy(dag.graph)
     dag.graph = {}
     for k, h in old_dep.items():
         dag.graph[k] = set()
 
     def add_dep(from_node: str, to_node: str):
         holder = dag.graph[from_node]
         holder.add(to_node)
-    
+
     for k, h in old_dep.items():
         for t in h:
             if t in old_dep:
                 add_dep(t, k)
             else:
                 # This is an external dependency and not part of our node
                 pass
 
 
-
 def _test(reverse):
-    print('reverse=', reverse)
+    print("reverse=", reverse)
     dag = DAG()
     dag.add("a", "a")
     dag.add("b1", "b1", {"a"})
     dag.add("b2", "b2", {"a"})
     dag.add("c", "c", {"b1"})
     dag.add("d", "d", {"b2", "c"})
 
     if reverse:
         _reverse_dag(dag)
 
     def fn_proc(id):
         print("-> ", id)
-        print('sleeping', id)
+        print("sleeping", id)
         time.sleep(2)
         print("<- ", id)
 
-    _walkthrough(dag, fn_proc, 3)
-    print('exit')
+    _walkthrough(dag, fn_proc, False, 3)
+    print("exit")
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     _test(False)
-    _test(True)
+    _test(True)
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/helper.py` & `hcs-cli-0.1.50/vhcs/plan/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,25 @@
 limitations under the License.
 """
 
 import json
 import yaml
 from typing import Tuple
 import os
-from vhcs.common.util import load_data_file, strict_dict_to_class, process_variables
+from vhcs.ctxp.data_util import load_data_file, strict_dict_to_class, process_variables
+
 
 class PlanException(Exception):
     pass
 
+
 class PluginException(Exception):
     pass
 
+
 class Blueprint:
     vars: dict
     defaults: dict
     providers: dict
     resources: dict
 
     def __init__(self):
@@ -36,127 +39,181 @@
         self.defaults = {}
         self.providers = {}
         self.resources = {}
 
     def __repr__(self):
         return f"Blueprint"
 
+
 def load_files(files: list[str]) -> dict:
     ret = {}
     for file in files:
         data = load_data_file(file)
         if data == None or isinstance(data, str):
             raise FileNotFoundError("Fail loading file: " + file)
         ret = _merge_dict_fail_on_dup(ret, _smart_load_file(file))
     return ret
 
 
 def process_template(template) -> Tuple[dict, dict]:
+
+    # Ensure default sections are not None
+    if "vars" not in template:
+        template["vars"] = {}
+    if "defaults" not in template:
+        template["defaults"] = {}
+    if "resources" not in template:
+        template["resources"] = {}
+    if "runtimes" not in template:
+        template["runtimes"] = {}
+    if "providers" not in template:
+        template["providers"] = {}
+
     _validate_blueprint(template)
     bp, pending = _materialize_blueprint(template)
     return bp, pending
 
+
 def _validate_blueprint(blueprint: dict):
     _validate_resource_schema(blueprint)
     _validate_resource_id_not_conflict_to_reserved_names(blueprint)
     _validate_no_conflict_resource_id_provider_types_runtime_id(blueprint)
     _validate_statement_after(blueprint)
 
+
 def _validate_resource_schema(blueprint: dict):
-    resources = blueprint.get('resources')
+    resources = blueprint["resources"]
     if not resources:
         return
-    required_keys = set(['kind'])
-    optional_keys = set(['eta', 'data', 'conditions', 'for', 'after'])
+    required_keys = set(["kind"])
+    optional_keys = set(["eta", "data", "conditions", "for", "after"])
     for k, v in resources.items():
+
         def _raise(reason):
             raise PlanException(f"Invalid blueprint: {reason}. Resource: {k}")
+
         actual_keys = set(v.keys())
         missed_keys = required_keys - actual_keys
         if missed_keys:
-            _raise(f'Missing required keys: {missed_keys}')
+            _raise(f"Missing required keys: {missed_keys}")
         extra_keys = actual_keys - required_keys - optional_keys
         if extra_keys:
-            _raise(f'Unknown extra keys: {extra_keys}')
+            _raise(f"Unknown extra keys: {extra_keys}")
+
 
 def _get_duplicates(lst):
     return [item for item in set(lst) if lst.count(item) > 1]
 
-def _validate_statement_after(blueprint: dict):
 
+def _validate_statement_after(blueprint: dict):
     def _raise(owner, reason):
         raise PlanException(f"Invalid statement: after. Owner={owner}, reason={reason}.")
-    
+
+    items = {}
+    items |= blueprint['resources']
+    items |= blueprint['runtimes']
+
     def _validate_after(target_name, owner_resource_name):
         if not isinstance(target_name, str):
             _raise(owner_resource_name, f"Invalid value type: {type(target_name).__name__}")
-    
-        if target_name not in blueprint['resources']:
+
+        if target_name not in items:
             _raise(owner_resource_name, "Target not found: " + target_name)
 
-    for k, v in blueprint['resources'].items():
-        after = v.get('after')
+    for k, v in items.items():
+        after = v.get("after")
         if after:
             if isinstance(after, list):
                 for a in after:
                     _validate_after(a, k)
 
                 dup = _get_duplicates(after)
                 if dup:
-                    _raise(k, 'Duplicated keys: ' + dup)
+                    _raise(k, "Duplicated keys: " + dup)
             elif isinstance(after, str):
                 _validate_after(after, k)
             else:
                 _raise(k, "Invalid type, expect str or list, got: " + type(after).__name__)
 
 
 def _validate_no_conflict_resource_id_provider_types_runtime_id(blueprint: dict):
     provider_names = set()
-    runtime_names = set(blueprint.get('runtimes', {}).keys())
-    for v in blueprint['resources'].values():
-        name, _ = v['kind'].split('/')
+    runtime_names = set(blueprint["runtimes"].keys())
+    for v in blueprint["resources"].values():
+        name, _ = v["kind"].split("/")
         provider_names.add(name)
-    for name in blueprint['resources']:
-        if name in provider_names:
-            raise PlanException("Invalid blueprint. Invalid resource name due to conflict to provider type. Name: " + name)
-        if name in runtime_names:
-            raise PlanException("Invalid blueprint. Invalid resource name due to conflict to runtime name. Name: " + name)
-
-    if provider_names & runtime_names:
-        raise PlanException("Invalid blueprint. Provider id and runtime id conflict. Runtime must not have conflict id as provider.")
-    
+
+    declared_provider_names = set(blueprint["providers"].keys())
+    excessive = declared_provider_names - provider_names
+    if excessive:
+        raise PlanException(
+            f"Invalid blueprint. Unused provider definition: {excessive}."
+        )
+    resource_names = set(blueprint["resources"].keys())
+    conflict = provider_names & resource_names
+    if conflict:
+        raise PlanException(
+            f"Invalid blueprint. Provider ID and resource ID conflict: {conflict}."
+        )
+    conflict = runtime_names & resource_names
+    if conflict:
+        raise PlanException(
+            f"Invalid blueprint. Runtime ID and resource ID conflict: {conflict}."
+        )
+    conflict = provider_names & runtime_names
+    if conflict:
+        raise PlanException(
+            f"Invalid blueprint. Provider ID and runtime ID conflict: {conflict}."
+        )
+
+
 def _validate_resource_id_not_conflict_to_reserved_names(blueprint: dict):
-    reserved_names_for_state = ['result', 'pending', 'log', 'destroy_output']
-    reserved_names_for_blueprint = ['defaults', 'vars', 'providers', 'resources']
-    reserved_names_for_function = ['profile', 'context']
+    reserved_names_for_state = ["result", "pending", "log", "destroy_output"]
+    reserved_names_for_blueprint = ["defaults", "vars", "providers", "resources", "runtimes"]
+    reserved_names_for_function = ["profile", "context"]
     existing_names_top_level = blueprint.keys()
-    reserved_names = set([*existing_names_top_level, *reserved_names_for_blueprint, *reserved_names_for_state, *reserved_names_for_function])
-    for name in blueprint['resources']:
+    reserved_names = set(
+        [
+            *existing_names_top_level,
+            *reserved_names_for_blueprint,
+            *reserved_names_for_state,
+            *reserved_names_for_function,
+        ]
+    )
+    for name in blueprint["resources"]:
         if name in reserved_names:
             raise PlanException("Invalid blueprint. Resource name conflicts to a reserved name: " + name)
+    for name in blueprint["runtimes"]:
+        if name in reserved_names:
+            raise PlanException("Invalid blueprint. Runtime name conflicts to a reserved name: " + name)
+    for name in blueprint["providers"]:
+        if name in reserved_names:
+            raise PlanException("Invalid blueprint. Provider name conflicts to a reserved name: " + name)
+
 
 def _smart_load_file(file: str):
     if not os.path.exists(file):
         raise Exception("File not found: " + file)
     if not os.path.isfile(file):
         raise Exception("Not a file: " + file)
-    if file.endswith('.json'):
+    if file.endswith(".json"):
         with open(file, "r") as f:
             return json.load(f)
-    elif file.endswith('.yaml') or file.endswith('.yml'):
+    elif file.endswith(".yaml") or file.endswith(".yml"):
         with open(file, "r") as f:
             return yaml.safe_load(f)
     else:
         raise Exception("Unknown file extention: " + file)
-    
+
+
 def _merge_dict_fail_on_dup(o1: dict, o2: dict) -> dict:
     ret = dict(o1)
     for k, v in o2.items():
         if k in o1:
             raise Exception("Fail processing file. Duplicated key found: " + k)
         ret[k] = v
     return ret
 
 
 def _materialize_blueprint(template: dict) -> Tuple[dict, dict]:
     ret = process_variables(template)
-    return template, ret['pending']
+    return template, ret["pending"]
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/kop.py` & `hcs-cli-0.1.50/vhcs/plan/kop.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,72 +14,85 @@
 """
 
 import time
 import traceback
 import traceback
 import logging
 from typing import Any
-from vhcs.common.ctxp.util import CtxpException
+from vhcs.ctxp.util import CtxpException
 from httpx import HTTPStatusError
 from subprocess import CalledProcessError
-from vhcs.common.ctxp.util import error_details
+from vhcs.ctxp.util import error_details
 from .helper import PlanException, PluginException
 
 log = logging.getLogger(__name__)
 
-class KopException(Exception): pass
+
+class KopException(Exception):
+    pass
+
 
 class KopMode:
-    create = 'create'
-    delete = 'delete'
-    update = 'update'
+    create = "create"
+    delete = "delete"
+    update = "update"
+
 
 class KopAction:
-    start = 'start'
-    success = 'success'
-    error = 'error'
-    skip = 'skip'
+    start = "start"
+    success = "success"
+    error = "error"
+    skip = "skip"
+
 
 class _DummyJobView:
     def add(id, name):
         pass
+
     def update(id, text: str):
         pass
+
     def start(id, eta: str):
         pass
+
     def success(id):
         pass
+
     def skip(id, reason):
         pass
+
     def error(id, err):
         pass
+
+
 _job_view = _DummyJobView
 
+
 def attach_job_view(view):
     global _job_view
     _job_view = view
 
+
 class KOP:
     MODE = KopMode
 
     def __init__(self, state: dict, kind: str, name: str, mode: str = KopMode.create) -> "KOP":
         self._state = state
         self._kind = kind
         self._name = name
         self._id = None
         self._mode = mode
         self._started = False
         self._closed = False
-        job_id = kind + '/' + name
+        job_id = kind + "/" + name
         _job_view.add(job_id, job_id)
 
-    
     def _job_id(self):
-        return self._kind + '/' + self._name
-    
+        return self._kind + "/" + self._name
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         if exc_value:
             self.error(exc_value)
         else:
@@ -87,15 +100,15 @@
             if not self._closed:
                 self._success()
 
     # Getter and setter for dollars...
     @property
     def dollars(self):
         return self.total_cents // 100
-    
+
     @dollars.setter
     def dollars(self, new_dollars):
         self.total_cents = 100 * new_dollars + self.cents
 
     def id(self, res_id: str):
         self._id = res_id
         _job_view.update(self._job_id(), res_id)
@@ -109,17 +122,19 @@
             self._mode = mode
         self._started = True
         self._add_log(KopAction.start)
         _job_view.start(self._job_id(), eta)
 
     def _success(self):
         if not self._started:
-            raise KopException("Kop not started. This is a framework logging issue. Call kop.start() before starting the resource operation.")
+            raise KopException(
+                "Kop not started. This is a framework logging issue. Call kop.start() before starting the resource operation."
+            )
         if self._closed:
-            raise KopException("Kop already closed. This is a framework logging issue.");
+            raise KopException("Kop already closed. This is a framework logging issue.")
         self._add_log(KopAction.success)
         self._closed = True
         _job_view.success(self._job_id())
 
     def error(self, err):
         if isinstance(err, Exception):
             if _need_stack_trace(err):
@@ -135,55 +150,49 @@
         self._add_log(KopAction.skip, reason)
         self._closed = True
         _job_view.skip(self._job_id(), reason)
 
     def _add_log(self, action: str, details: str = None):
         labels = {
             KopMode.create: {
-                KopAction.start:    '[creating]',
-                KopAction.success:  '[created ]',
-                KopAction.skip:     '[skipped ]',
-                KopAction.error:    '[error   ]'
+                KopAction.start: "[creating]",
+                KopAction.success: "[created ]",
+                KopAction.skip: "[skipped ]",
+                KopAction.error: "[error   ]",
             },
             KopMode.delete: {
-                KopAction.start:    '[deleting]',
-                KopAction.success:  '[deleted ]',
-                KopAction.skip:     '[skipped ]',
-                KopAction.error:    '[error   ]'
+                KopAction.start: "[deleting]",
+                KopAction.success: "[deleted ]",
+                KopAction.skip: "[skipped ]",
+                KopAction.error: "[error   ]",
             },
             KopMode.update: {
-                KopAction.start:    '[updating]',
-                KopAction.success:  '[updated ]',
-                KopAction.skip:     '[skipped ]',
-                KopAction.error:    '[error   ]'
-            }
+                KopAction.start: "[updating]",
+                KopAction.success: "[updated ]",
+                KopAction.skip: "[skipped ]",
+                KopAction.error: "[error   ]",
+            },
         }
         label_map = labels.get(self._mode)
         if not label_map:
             raise KopException(f"Invalid mode: {self._mode}")
         label = label_map[action]
-        msg = f'{label} {self._kind}:{self._name}'
+        msg = f"{label} {self._kind}:{self._name}"
         if self._id:
-            msg += ' ' + self._id
+            msg += " " + self._id
 
         if _job_view == _DummyJobView:
             log.info(msg)
-        entry = {
-            'name': self._name,
-            'time': int(time.time()),
-            'action': action,
-            'id': self._id
-        }
+        entry = {"name": self._name, "time": int(time.time()), "action": action, "id": self._id}
         if details:
-            entry['details'] = details
-        self._state['log'][self._mode].append(entry)
-        if action == 'error':
+            entry["details"] = details
+        self._state["log"][self._mode].append(entry)
+        if action == "error":
             if self._id:
                 log.warning('Plugin "%s:%s" failed: %s. Id=%s', self._kind, self._name, details, self._id)
             else:
                 log.warning('Plugin "%s:%s" failed: %s.', self._kind, self._name, details)
 
 
 def _need_stack_trace(e):
     if isinstance(e, KeyError):
         return True
-
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/_az_facade.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/_az_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import json
 import logging
 
 log = logging.getLogger(__name__)
 
 _subscription = None
 
-def _az(command: str, silent: bool =False) -> dict:
+
+def _az(command: str, silent: bool = False) -> dict:
     log.debug(command)
-    args = command.split(' ')
+    args = command.split(" ")
     p = subprocess.run(args, capture_output=True, text=True, timeout=None, check=False)
     if p.returncode:
         if silent:
             pass
         else:
             log.error("RETURN: " + str(p.returncode))
             log.error("STDOUT: " + p.stdout)
@@ -37,56 +38,62 @@
         if p.stdout:
             try:
                 return json.loads(p.stdout)
             except Exception as e:
                 log.error("Fail parsing response %s", e)
                 log.warning("Payload: %s", p.stdout)
 
+
 def login(username: str, password: str, tenant_id: str):
     return _az(f"az login --service-principal -u {username} -p {password} --tenant {tenant_id}")
 
+
 def _formalize_tags(tags: dict) -> str:
     list_tags = []
     if tags:
         for k, v in tags.items():
-            list_tags.append(f'{k}={v}')
-    return ' '.join(list_tags)
+            list_tags.append(f"{k}={v}")
+    return " ".join(list_tags)
+
 
 def set_subscription(id: str):
     global _subscription
     _subscription = id
     return _az(f"az account set --subscription {id}")
 
+
 def locations():
     return _az("az account list-locations")
 
+
 class resource_group:
     @staticmethod
     def create(name: str, location: str, tags: dict = None):
         tags_str = _formalize_tags(tags)
         return _az(f"az group create --location {location} --name {name} --tags {tags_str}")
 
     @staticmethod
     def delete(name: str):
         exists = _az(f"az group exists --name {name}")
         if exists:
             _az(f"az group delete --name {name} --yes")
             return True
         return False
 
-class _aad_group_member:
 
+class _aad_group_member:
     @staticmethod
     def list(id_or_display_name: str):
         return _az(f"az ad group member list --group {id_or_display_name}")
 
     @staticmethod
     def add(id_or_display_name: str, member_id: str):
         return _az(f"az ad group member add --group {id_or_display_name} --member-id {member_id}")
-    
+
+
 class _aad_group:
     member = _aad_group_member
 
     @staticmethod
     def create(display_name: str, mail_nickname: str, description: str = None):
         cmd = f"az ad group create --display-name {display_name} --mail-nickname {mail_nickname}"
         if description:
@@ -100,117 +107,130 @@
     @staticmethod
     def delete(id_or_display_name: str):
         return _az(f"az ad group delete --group {id_or_display_name}")
 
     @staticmethod
     def list():
         return _az(f"az ad group list")
-    
+
 
 class _aad_user:
     @staticmethod
     def create(display_name: str, password: str, principal_name: str):
-        return _az(f"az ad user create --display-name {display_name} --password {password} --user-principal-name {principal_name}")
-    
+        return _az(
+            f"az ad user create --display-name {display_name} --password {password} --user-principal-name {principal_name}"
+        )
+
     @staticmethod
     def get(id_or_principal_name: str):
         return _az(f"az ad user show --id {id_or_principal_name}", silent=True)
 
     @staticmethod
     def delete(id: str):
         return _az(f"az ad user delete --id {id}")
 
 
 class aad:
     group = _aad_group
     user = _aad_user
-    
+
 
 class _vnet:
     @staticmethod
     def get(id: str):
         return _az(f"az network vnet show --ids {id}")
-    
+
     @staticmethod
     def create(rg_name: str, name: str, address_prefix: str):
         return _az(f"az network vnet create -g {rg_name} -n {name} --address-prefix {address_prefix}")
-    
+
     @staticmethod
     def delete(rg_name: str, name: str, address_prefix: str):
         return _az(f"az network vnet create -g {rg_name} -n {name} --address-prefix {address_prefix}")
-    
 
     @staticmethod
     def list():
         return _az("az network vnet list")
-    
+
+
 class _nsg:
     @staticmethod
     def create(rg_name: str, name: str, location: str, tags: list[str] = None):
         tags_str = _formalize_tags(tags)
         return _az(f"az network nsg create -g {rg_name} -n {name} --location {location} --tags {tags_str}")
-    
+
     @staticmethod
     def delete_by_id(id: str):
         return _az(f"az network nsg delete --ids {id}")
-    
+
     @staticmethod
     def delete(rg_name: str, name: str):
         return _az(f"az network nsg delete -g {rg_name} -n {name}")
-    
-class _subnet:
 
+
+class _subnet:
     @staticmethod
     def create(rg_name: str, vnet_name: str, name: str, cidr: str, nsg_name: str):
-        return _az(f"az network vnet subnet create -g {rg_name} --vnet-name {vnet_name} -n {name} --address-prefixes {cidr} --network-security-group {nsg_name}")
-    
+        return _az(
+            f"az network vnet subnet create -g {rg_name} --vnet-name {vnet_name} -n {name} --address-prefixes {cidr} --network-security-group {nsg_name}"
+        )
+
     @staticmethod
     def delete_by_id(id: str):
         return _az(f"az network vnet subnet delete --ids {id}")
-    
+
     @staticmethod
     def delete(rg_name: str, vnet_name: str, name: str):
         return _az(f"az network vnet subnet delete -g {rg_name} --vnet-name {vnet_name} -n {name}")
-    
+
     @staticmethod
     def list(rg_name: str, vnet_name: str):
         return _az(f"az network vnet subnet list -g {rg_name} --vnet-name {vnet_name}")
 
+
 class _public_ip:
     @staticmethod
     def create(rg_name: str, name: str, location: str):
-        return _az(f"az network public-ip create -g {rg_name} -n {name} --location {location} --allocation-method Static")
-    
+        return _az(
+            f"az network public-ip create -g {rg_name} -n {name} --location {location} --allocation-method Static"
+        )
+
     @staticmethod
     def get(rg_name: str, name: str):
         return _az(f"az network public-ip show -g {rg_name} -n {name}")
-    
+
     @staticmethod
     def delete(rg_name: str, name: str):
         return _az(f"az network public-ip delete -g {rg_name} -n {name}")
 
+
 class network:
     vnet = _vnet
     nsg = _nsg
     subnet = _subnet
     public_ip = _public_ip
 
+
 def adjust_tags(parameters) -> str:
     return parameters
 
+
 from vhcs.plan import context
 from azure.identity import AzureCliCredential
 from azure.mgmt.network import NetworkManagementClient
 from azure.mgmt.resource import ResourceManagementClient
 from azure.mgmt.msi import ManagedServiceIdentityClient
 
+
 def network_management_client() -> NetworkManagementClient:
     credentials = AzureCliCredential()
     return NetworkManagementClient(credentials, _subscription)
 
+
 def resource_management_client() -> ResourceManagementClient:
     credentials = AzureCliCredential()
     return ResourceManagementClient(credentials, _subscription)
 
+
 def managed_identity_client() -> ManagedServiceIdentityClient:
     credentials = AzureCliCredential()
-    return ManagedServiceIdentityClient(credentials, _subscription)
+    return ManagedServiceIdentityClient(credentials, _subscription)
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/_prepare.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/_prepare.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from . import _az_facade as az
 
 log = logging.getLogger(__name__)
 
+
 def prepare(data: dict):
-    subscription_id = data['subscriptionId']
+    subscription_id = data["subscriptionId"]
     az.set_subscription(subscription_id)
 
-    applicationId = data.get('applicationId')
+    applicationId = data.get("applicationId")
     if applicationId:
         log.info("Initializing with configured SP.")
-        applicationKey = data.get('applicationKey')
-        #az.login(applicationId, applicationKey, )
+        applicationKey = data.get("applicationKey")
+        # az.login(applicationId, applicationKey, )
 
-    
     # _az_facade.login(provider['applicationId'], provider['applicationKey'], directory_id)
     # _az_facade.set_subscription(subscription_id)
     else:
-        log.info("No configured SP found. Using Azure CLI stored login.")
+        log.info("No configured SP found. Using Azure CLI stored login.")
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_group.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/aad_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,34 +13,38 @@
 limitations under the License.
 """
 
 from vhcs.plan import actions
 from azure.core.exceptions import ResourceNotFoundError
 from . import _az_facade as az
 
+
 def deploy(data: dict, state: dict) -> dict:
-    display_name = data['displayName']
-    mail_nickname = data['mailNickname']
-    description = data.get('description')
-    parent_group = data.get('parentGroup')
+    display_name = data["displayName"]
+    mail_nickname = data["mailNickname"]
+    description = data.get("description")
+    parent_group = data.get("parentGroup")
     ret = az.aad.group.create(display_name, mail_nickname, description)
     if parent_group:
-        az.aad.group.member.add(parent_group, ret['id'])
+        az.aad.group.member.add(parent_group, ret["id"])
     return ret
 
 
 def refresh(data: dict, state: dict) -> dict:
-    display_name = data['displayName']
+    display_name = data["displayName"]
     return az.aad.group.get(display_name)
 
+
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
     if state:
-        id = state['id']
+        id = state["id"]
         return az.aad.group.delete(id)
-    display_name = data['displayName']
+    display_name = data["displayName"]
     return az.aad.group.delete(display_name)
 
+
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_user.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/resource_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,58 +11,40 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
 from azure.core.exceptions import ResourceNotFoundError
-import random
-from . import _az_facade as az
+from ._az_facade import resource_management_client as client, adjust_tags
+
 
 def deploy(data: dict, state: dict) -> dict:
-    group = data['group']
-    email = data['email']
-    domain_name = data['domainName']
-
-    pname = _convert_email_to_principle(email, domain_name)
-    display_name = pname
-    password = _generate_password()
-    principal_name = pname
-    ret = az.aad.user.create(display_name, password, principal_name)
-    az.aad.group.member.add(group, ret['id'])
-    ret['password'] = password
-    return ret
-
-def _convert_email_to_principle(email: str, domain_name: str) -> str:
-    name = email.replace('@', '_')
-    return name + '@' + domain_name
-
-def _generate_password() -> str:
-    ret = random.choices("ABCDEFGHJKMNPQRSTUVWXY")
-    ret += random.choices("abcdefghjkmnpqrstuvwxy23456789", k=10)
-    ret += random.choices("!@$%&*")
-    return "".join(ret)
+    name = data["name"]
+    parameters = adjust_tags(data["parameters"])
+    return client().resource_groups.create_or_update(name, parameters)
+
 
 def refresh(data: dict, state: dict) -> dict:
-    if state:
-        id = state['id']
-        ret = az.aad.user.get(id)
-        if ret:
-            ret['password'] = state.get('password')
-            return ret
-    email = data['email']
-    domain_name = data['domainName']
-    pname = _convert_email_to_principle(email, domain_name)
-    return az.aad.user.get(pname)
+    name = data["name"]
+    try:
+        return client().resource_groups.get(name)
+    except ResourceNotFoundError:
+        pass
+
 
 def decide(data: dict, state: dict):
-    if not state.get('password'):
-        return actions.recreate
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    id = state['id']
-    ret = az.aad.user.delete(id)
-    return ret
+    name = data["name"]
+    try:
+        return client().resource_groups.begin_delete(name).wait()
+    except ResourceNotFoundError:
+        pass
+
 
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    if action == actions.delete:
+        return "5m"
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/nat_gateway.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/nsg.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,36 +9,40 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.plan import actions, context
+from vhcs.plan import actions
 from azure.core.exceptions import ResourceNotFoundError
 from ._az_facade import network_management_client as client, adjust_tags
 
 
 def deploy(data: dict, state: dict) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
-    parameters = adjust_tags(data['parameters'])
-
-    return client().nat_gateways.begin_create_or_update(
-        rg_name,
-        name,
-        parameters
-    ).result()
+    rg_name = data["resourceGroup"]
+    name = data["name"]
+    parameters = adjust_tags(data["parameters"])
+    return client().network_security_groups.begin_create_or_update(rg_name, name, parameters).result()
+
 
 def refresh(data: dict, state: dict) -> dict:
-    return state
+    rg_name = data["resourceGroup"]
+    name = data["name"]
+    try:
+        return client().network_security_groups.get(rg_name, name)
+    except ResourceNotFoundError:
+        pass
+
 
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
-    client().nat_gateways.begin_delete(rg_name, name).wait()
+    rg_name = data["resourceGroup"]
+    name = data["name"]
+    client().network_security_groups.begin_delete(rg_name, name).wait()
+
 
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/public_ip.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,31 +13,37 @@
 limitations under the License.
 """
 
 from vhcs.plan import actions
 from azure.core.exceptions import ResourceNotFoundError
 from ._az_facade import network_management_client as client, adjust_tags
 
+
 def deploy(data: dict, state: dict) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
-    parameters = adjust_tags(data['parameters'])
-    return client().network_security_groups.begin_create_or_update(rg_name, name, parameters).result()
+    name = data["name"]
+    resource_group = data["resourceGroup"]
+    parameters = adjust_tags(data["parameters"])
+
+    return client().public_ip_addresses.begin_create_or_update(resource_group, name, parameters).result()
+
 
 def refresh(data: dict, state: dict) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
+    name = data["name"]
+    resource_group = data["resourceGroup"]
     try:
-        return client().network_security_groups.get(rg_name, name)
+        return client().public_ip_addresses.get(resource_group, name)
     except ResourceNotFoundError:
         pass
 
+
 def decide(data: dict, state: dict):
-    return actions.skip
+    return actions.create
+
 
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
-    client().network_security_groups.begin_delete(rg_name, name).wait()
+    name = data["name"]
+    resource_group = data["resourceGroup"]
+    client().public_ip_addresses.begin_delete(resource_group, name).wait()
+
 
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/public_ip.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/virtual_network.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,40 +9,41 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.plan import actions
+from vhcs.plan import actions, context
 from azure.core.exceptions import ResourceNotFoundError
 from ._az_facade import network_management_client as client, adjust_tags
 
+
 def deploy(data: dict, state: dict) -> dict:
-    name = data['name']
-    resource_group = data['resourceGroup']
-    parameters = adjust_tags(data['parameters'])
-
-    return client().public_ip_addresses.begin_create_or_update(
-        resource_group,
-        name,
-        parameters
-    ).result()
+    rg_name = data["resourceGroup"]
+    name = data["name"]
+    parameters = adjust_tags(data["parameters"])
+    vnet = client().virtual_networks.begin_create_or_update(rg_name, name, parameters).result()
+    return vnet
+
 
 def refresh(data: dict, state: dict) -> dict:
-    name = data['name']
-    resource_group = data['resourceGroup']
+    rg_name = data["resourceGroup"]
+    name = data["name"]
     try:
-        return client().public_ip_addresses.get(resource_group, name)
+        return client().virtual_networks.get(rg_name, name)
     except ResourceNotFoundError:
         pass
 
+
 def decide(data: dict, state: dict):
-    return actions.create
+    return actions.skip
+
 
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    name = data['name']
-    resource_group = data['resourceGroup']
-    client().public_ip_addresses.begin_delete(resource_group, name).wait()
+    rg_name = data["resourceGroup"]
+    name = data["name"]
+    client().virtual_networks.begin_delete(rg_name, name).wait()
+
 
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/identity_provider.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,36 +10,40 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
-from azure.core.exceptions import ResourceNotFoundError
-from ._az_facade import resource_management_client as client, adjust_tags
+from vhcs.service import portal
+
 
 def deploy(data: dict, state: dict) -> dict:
-    name = data['name']
-    parameters = adjust_tags(data['parameters'])
-    return client().resource_groups.create_or_update(name, parameters)
+    return portal.site.create(data)
+
 
 def refresh(data: dict, state: dict) -> dict:
-    name = data['name']
-    try:
-        return client().resource_groups.get(name)
-    except ResourceNotFoundError:
-        pass
+    org_id = data["orgId"]
+    if state:
+        id = state.get("id")
+        if id:
+            ret = portal.site.get(id, org_id)
+            if ret:
+                return ret
+
+    # Fall back with smart find by name
+    return portal.site.find_by_name(data["name"], org_id)
+
 
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    name = data['name']
-    try:
-        return client().resource_groups.begin_delete(name).wait()
-    except ResourceNotFoundError:
-        pass
+    return portal.site.delete(state["id"], data["orgId"])
+
 
 def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return "1m"
     if action == actions.delete:
-        return '5m'
-    return '1m'
+        return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/subnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,41 +14,48 @@
 """
 
 from retry import retry
 from vhcs.plan import actions
 from azure.core.exceptions import ResourceNotFoundError, ResourceExistsError
 from ._az_facade import network_management_client as client, adjust_tags
 import logging
+
 log = logging.getLogger(__name__)
 
+
 def deploy(data: dict, state: dict) -> dict:
-    rg_name = data['resourceGroup']
-    vnet_name = data['vNetName']
-    name = data['name']
-    parameters = adjust_tags(data['parameters'])
+    rg_name = data["resourceGroup"]
+    vnet_name = data["vNetName"]
+    name = data["name"]
+    parameters = adjust_tags(data["parameters"])
 
     return _create(rg_name, vnet_name, name, parameters)
 
-@retry(exceptions=ResourceExistsError, tries = 10, delay = 10, backoff=2, jitter=(0, 10), logger=log)
+
+@retry(exceptions=ResourceExistsError, tries=10, delay=10, backoff=2, jitter=(0, 10), logger=log)
 def _create(rg_name, vnet_name, name, parameters):
     return client().subnets.begin_create_or_update(rg_name, vnet_name, name, parameters).result()
 
+
 def refresh(data: dict, state: dict) -> dict:
-    rg_name = data['resourceGroup']
-    vnet_name = data['vNetName']
-    name = data['name']
+    rg_name = data["resourceGroup"]
+    vnet_name = data["vNetName"]
+    name = data["name"]
     try:
         return client().subnets.get(rg_name, vnet_name, name)
     except ResourceNotFoundError:
         pass
 
+
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    rg_name = data['resourceGroup']
-    vnet_name = data['vNetName']
-    name = data['name']
+    rg_name = data["resourceGroup"]
+    vnet_name = data["vNetName"]
+    name = data["name"]
     return client().subnets.begin_delete(rg_name, vnet_name, name).wait()
 
+
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/azure/virtual_network.py` & `hcs-cli-0.1.50/vhcs/plan/provider/azure/nat_gateway.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 limitations under the License.
 """
 
 from vhcs.plan import actions, context
 from azure.core.exceptions import ResourceNotFoundError
 from ._az_facade import network_management_client as client, adjust_tags
 
+
 def deploy(data: dict, state: dict) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
-    parameters = adjust_tags(data['parameters'])
-    vnet = client().virtual_networks.begin_create_or_update(rg_name, name, parameters).result()
-    return vnet
+    rg_name = data["resourceGroup"]
+    name = data["name"]
+    parameters = adjust_tags(data["parameters"])
+
+    return client().nat_gateways.begin_create_or_update(rg_name, name, parameters).result()
+
 
 def refresh(data: dict, state: dict) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
-    try:
-        return client().virtual_networks.get(rg_name, name)
-    except ResourceNotFoundError:
-        pass
+    return state
+
 
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    rg_name = data['resourceGroup']
-    name = data['name']
-    client().virtual_networks.begin_delete(rg_name, name).wait()
+    rg_name = data["resourceGroup"]
+    name = data["name"]
+    client().nat_gateways.begin_delete(rg_name, name).wait()
+
 
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.50/vhcs/plan/provider/dev/dummy.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
 from copy import deepcopy
 from typing import Callable
-import vhcs.common.duration as duration
+import vhcs.ctxp.duration as duration
 from vhcs.plan import actions
 from vhcs.plan import PluginException
 
 
 def deploy(data: dict, state: dict, save_state: Callable) -> dict:
     text = data.get("text")
     error = data.get("error")
     delay = data.get("delay")
-    a = data.get("a", 0) 
+    a = data.get("a", 0)
     b = data.get("b", 0)
     error_before_save = data.get("error_before_save")
     delay_seconds = duration.to_seconds(delay)
     if delay_seconds:
         time.sleep(delay_seconds)
     ret = deepcopy(data)
     ret["outputText"] = text
-    ret['n'] = a + b
+    ret["n"] = a + b
 
     if not error_before_save:
         save_state(ret)
 
     if error:
         raise PluginException(error)
 
@@ -51,12 +51,13 @@
 def decide(data: dict, state: dict):
     return actions.skip
 
 
 def destroy(data: dict, state: dict, force: bool) -> dict:
     return {}
 
+
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '10s'
+        return "10s"
     if action == actions.delete:
-        return '10s'
+        return "10s"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/ad.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,37 +12,46 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
 from vhcs.service import admin
 
+
 def deploy(data: dict, state: dict) -> dict:
-    label = data['providerLabel']
-    return admin.ad.create(label, data)
+    label = data["providerLabel"]
+    return admin.provider.create(label, data)
+
 
 def refresh(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
+    org_id = data["orgId"]
+    label = data["providerLabel"]
+    id = None
     if state:
-        id = state.get('id')
-        if id:
-            return admin.ad.get(id, org_id)
-    
+        id = state["id"]
+        p = admin.provider.get(label, id, org_id)
+        if p:
+            return p
+
     # Fall back with smart find by name
-    search = "name $eq " + data['name']
-    ads = admin.ad.list(org_id=org_id, search=search)
-    if ads:
-        return ads[0]
+    search = "name $eq " + data["name"]
+    providers = admin.provider.list(label, org_id=org_id, search=search)
+    if providers:
+        return providers[0]
+
 
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    org_id = data['orgId']
-    id = state['id']
-    return admin.ad.delete(id, org_id)
+    org_id = data["orgId"]
+    label = data["providerLabel"]
+    id = state["id"]
+    return admin.provider.delete(label, id, org_id)
+
 
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '1m'
+        return "1m"
     if action == actions.delete:
-        return '1m'
+        return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/edge.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/edge.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,79 +22,75 @@
     if not state:
         deployment = admin.edge.create(data)
         save_state(deployment)
     else:
         deployment = state
     id = deployment["id"]
     is_ready = lambda s: s in [
-        'CREATE_PENDING',
-        'CREATING',
-        'READY',
-        'POST_PROVISIONING_CONFIG_IN_PROGRESS',
-        'UPDATE_PENDING', 
-        'UPDATING', 
-        'UPGRADE_PENDING', 
-        'UPGRADING',
+        "CREATE_PENDING",
+        "CREATING",
+        "READY",
+        "POST_PROVISIONING_CONFIG_IN_PROGRESS",
+        "UPDATE_PENDING",
+        "UPDATING",
+        "UPGRADE_PENDING",
+        "UPGRADING",
     ]
-    is_error = lambda s: s.endswith('_FAILED') or s in [
-        # 'CREATE_FAILED', 
-        'DELETED', 
-        # 'DELETE_FAILED', 
-        'DELETE_PENDING', 
-        'DELETING',
-        'FORCE_DELETE_PENDING', 
-        'FORCE_DELETING', 
-        'FORCE_REPAIR_ACCEPTED', 
-        'FORCE_REPAIR_PENDING',
-        # CONNECT_PENDING, 
-        # CREATE_ACCEPTED, 
-        # CREATE_FAILED, 
-        # CREATE_PENDING, 
-        # CREATING, 
-        'DELETED', 
-        #'DELETE_FAILED', 
-        'DELETE_PENDING', 
-        'DELETING', 
-        'FORCE_DELETE_PENDING', 
-        'FORCE_DELETING', 
-        'FORCE_REPAIR_ACCEPTED', 
-        'FORCE_REPAIR_PENDING', 
-        #'MIGRATE_FAILED', 
-        'MIGRATE_PENDING', 
-        'MIGRATING', 
-        # POST_PROVISIONING_CONFIG_IN_PROGRESS, 
-        # READY, 
-        'REPAIRING', 
-        'REPAIR_ACCEPTED', 
-        #'REPAIR_FAILED', 
-        'REPAIR_PENDING', 
-        #'UPDATE_FAILED', 
-        #'UPDATE_PENDING', 
-        #'UPDATING', 
-        #'UPGRADE_FAILED', 
-        #'UPGRADE_PENDING', 
+    is_error = lambda s: s.endswith("_FAILED") or s in [
+        # 'CREATE_FAILED',
+        "DELETED",
+        # 'DELETE_FAILED',
+        "DELETE_PENDING",
+        "DELETING",
+        "FORCE_DELETE_PENDING",
+        "FORCE_DELETING",
+        "FORCE_REPAIR_ACCEPTED",
+        "FORCE_REPAIR_PENDING",
+        # CONNECT_PENDING,
+        # CREATE_ACCEPTED,
+        # CREATE_FAILED,
+        # CREATE_PENDING,
+        # CREATING,
+        "DELETED",
+        #'DELETE_FAILED',
+        "DELETE_PENDING",
+        "DELETING",
+        "FORCE_DELETE_PENDING",
+        "FORCE_DELETING",
+        "FORCE_REPAIR_ACCEPTED",
+        "FORCE_REPAIR_PENDING",
+        #'MIGRATE_FAILED',
+        "MIGRATE_PENDING",
+        "MIGRATING",
+        # POST_PROVISIONING_CONFIG_IN_PROGRESS,
+        # READY,
+        "REPAIRING",
+        "REPAIR_ACCEPTED",
+        #'REPAIR_FAILED',
+        "REPAIR_PENDING",
+        #'UPDATE_FAILED',
+        #'UPDATE_PENDING',
+        #'UPDATING',
+        #'UPGRADE_FAILED',
+        #'UPGRADE_PENDING',
         #'UPGRADING',
     ]
-    is_transition = lambda s: s.endswith('ING') or s in [
-        'CREATE_ACCEPTED',
+    is_transition = lambda s: s.endswith("ING") or s in [
+        "CREATE_ACCEPTED",
     ]
     try:
-        deployment = admin.edge.wait_for(id, 
-                                         org_id, 
-                                         is_ready=is_ready,
-                                         is_error=is_error,
-                                         is_transition=is_transition)
+        deployment = admin.edge.wait_for(id, org_id, is_ready=is_ready, is_error=is_error, is_transition=is_transition)
     except Exception as e:
         deployment = admin.edge.get(id, org_id)
         save_state(deployment)
         raise PluginException("Error waiting for edge deployment. Status=" + deployment["status"]) from e
-    
+
     site_id = data["siteId"]
     portal.site.set_edge(site_id, org_id, id)
-    
+
     return deployment
 
 
 def refresh(data: dict, state: dict) -> dict:
     org_id = data["orgId"]
     if state:
         id = state.get("id")
@@ -112,14 +108,15 @@
         return actions.skip
     # https://gitlab.eng.vmware.com/horizonv2-sg/admin/-/blob/master/src/main/java/com/vmware/horizon/admin/model/edgedeployment/EdgeDeploymentV2Status.java
 
 
 def destroy(data: dict, state: dict, force: bool) -> dict:
     id = state["id"]
     org_id = data["orgId"]
-    admin.edge.safe_delete(id, org_id, '20m')
+    admin.edge.safe_delete(id, org_id, "20m")
+
 
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '15m'
+        return "15m"
     if action == actions.delete:
-        return '10m'
+        return "10m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/entitlement.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,30 +11,35 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from vhcs.plan import actions
 from vhcs.service import portal
 
+
 def deploy(data: dict, state: dict) -> dict:
     return portal.entitlement.create(data)
 
+
 def refresh(data: dict, state: dict) -> dict:
     if state:
-        id = state.get('id')
+        id = state.get("id")
         if id:
-            return portal.entitlement.get(id, data['orgId'])
-    
+            return portal.entitlement.get(id, data["orgId"])
+
     # Fall back with smart find by users
     # TODO
 
+
 def decide(data: dict, state: dict):
     return actions.skip
-    
+
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    return portal.entitlement.delete(state['id'], data['orgId'])
+    return portal.entitlement.delete(state["id"], data["orgId"])
+
 
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '1m'
+        return "1m"
     if action == actions.delete:
-        return '1m'
+        return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/identity_provider.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/site.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,33 +12,38 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
 from vhcs.service import portal
 
+
 def deploy(data: dict, state: dict) -> dict:
     return portal.site.create(data)
 
+
 def refresh(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
+    org_id = data["orgId"]
     if state:
-        id = state.get('id')
+        id = state.get("id")
         if id:
             ret = portal.site.get(id, org_id)
             if ret:
                 return ret
-    
+
     # Fall back with smart find by name
-    return portal.site.find_by_name(data['name'], org_id)
+    return portal.site.find_by_name(data["name"], org_id)
+
 
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    return portal.site.delete(state['id'], data['orgId'])
+    return portal.site.delete(state["id"], data["orgId"])
+
 
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '1m'
+        return "1m"
     if action == actions.delete:
-        return '1m'
+        return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/image.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,84 +12,87 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.service import ims
 from vhcs.plan import actions
 
+
 def deploy(data: dict, state: dict, save_state) -> dict:
-    image_catalog_request = data['import']
-    version_publish_create_TO = data['publish']
-    org_id = image_catalog_request['orgId']
+    image_catalog_request = data["import"]
+    version_publish_create_TO = data["publish"]
+    org_id = image_catalog_request["orgId"]
     img = refresh(data, state)
 
     if not img:
-        image_catalog_representation = ims.images.create('import', image_catalog_request)
-        stream_id = image_catalog_representation['streamId']
-        # The IMS API does not follow REST convention and has inconsistent return model 
-        # between the creation API and read APIs. 
+        image_catalog_representation = ims.images.create("import", image_catalog_request)
+        stream_id = image_catalog_representation["streamId"]
+        # The IMS API does not follow REST convention and has inconsistent return model
+        # between the creation API and read APIs.
         # https://jira.eng.vmware.com/browse/HV-78267
         img = ims.images.get(stream_id, org_id)
     save_state(img)
-    image_id = img['id']
+    image_id = img["id"]
 
-    img = ims.images.wait_for(image_id, org_id, ['IMPORT_COMPLETE', 'AVAILABLE'])
+    img = ims.images.wait_for(image_id, org_id, ["IMPORT_COMPLETE", "AVAILABLE"])
     save_state(img)
-    status = img['status']
-    if status == 'IMPORT_COMPLETE':
+    status = img["status"]
+    if status == "IMPORT_COMPLETE":
         version_api = ims.version(image_id, org_id)
         versions = version_api.list()
         if not versions:
-            raise Exception("No version found for image "+ image_id)
-        version_id = versions[0]['id']
+            raise Exception("No version found for image " + image_id)
+        version_id = versions[0]["id"]
         version_api.publish(version_id, version_publish_create_TO)
-        ims.images.wait_for(image_id, org_id, ['AVAILABLE'])
-    elif status == 'AVAILABLE':
+        ims.images.wait_for(image_id, org_id, ["AVAILABLE"])
+    elif status == "AVAILABLE":
         pass
     else:
-        raise Exception('Broken logic. This is a regression.')
+        raise Exception("Broken logic. This is a regression.")
     return ims.images.get(image_id, org_id)
 
 
 def refresh(data: dict, state: dict) -> dict:
-    org_id = data['import']['orgId']
+    org_id = data["import"]["orgId"]
     img = None
     if state:
-        image_id = state['id']
+        image_id = state["id"]
         img = ims.images.get(image_id, org_id)
     if not img:
-        existing_images = ims.images.list(org_id, search='name $eq ' + data['import']['streamName'])
+        existing_images = ims.images.list(org_id, search="name $eq " + data["import"]["streamName"])
         if existing_images:
             img = existing_images[0]
     return img
 
 
 def decide(data: dict, state: dict):
-    status = state['status']
+    status = state["status"]
     status_to_action = {
-        'AVAILABLE': actions.skip,
-        'IMPORT_COMPLETE': actions.create,
-        'DELETING': actions.recreate,
-        'DISABLED': actions.recreate,
-        'FAILED': actions.recreate,
-        'IMPORT_COMPLETE': actions.create,
-        'IN_PROGRESS': actions.create,
-        'PARTIALLY_AVAILABLE': actions.skip,
-        'PENDING': actions.create,
+        "AVAILABLE": actions.skip,
+        "IMPORT_COMPLETE": actions.create,
+        "DELETING": actions.recreate,
+        "DISABLED": actions.recreate,
+        "FAILED": actions.recreate,
+        "IMPORT_COMPLETE": actions.create,
+        "IN_PROGRESS": actions.create,
+        "PARTIALLY_AVAILABLE": actions.skip,
+        "PENDING": actions.create,
     }
     action = status_to_action.get(status)
     if not action:
         raise Exception(f"Unknown image status: {status}")
     return action
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    org_id = data['import']['orgId']
-    image_id = state['id']
-    ims.helper.delete_images([image_id], org_id, '15m')
+    org_id = data["import"]["orgId"]
+    image_id = state["id"]
+    ims.helper.delete_images([image_id], org_id, "15m")
+
 
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '60m'
-    # when the image is in-process creating/publishing, the deletion needs 
+        return "60m"
+    # when the image is in-process creating/publishing, the deletion needs
     # to start after the image is ready (at least with IMS today), which could take a considerable time.
-    if action == actions.delete:    
-        return '60m'
+    if action == actions.delete:
+        return "60m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/pool_group.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,43 +9,46 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ulid import ULID
 from vhcs.plan import actions
+import vhcs.service.portal as portal
+
 
 def deploy(data: dict, state: dict) -> dict:
-    users = data['users']
-    entitlementId = data['entitlementId']
-    domainName = data['domainName']
-    stackUrl = data['stackUrl']
-
-    launch_items = []
-
-    for u in users:
-        horizonId = str(ULID())
-        login_hint = u['userPrincipalName']
-        launch_items.append({
-            'user': u,
-            'launchUrl': f"{stackUrl}/appblast/webclient/?horizonId={horizonId}&entitlementId={entitlementId}&domainName={domainName}&action=start-session&login_hint={login_hint}#/desktop"
-        })
-        
-    return launch_items
-    
+    return portal.pool.create(data)
+
 
 def refresh(data: dict, state: dict) -> dict:
+    org_id = data["orgId"]
+    if state:
+        id = state.get("id")
+        if id:
+            return portal.pool.get(id, org_id)
+
+    # Fall back with smart find by name
+    pools = portal.pool.list(org_id, search=f"name $eq {data['name']}")
+    if pools and len(pools) == 1:
+        return pools[0]
     return state
 
+
 def decide(data: dict, state: dict):
     return actions.skip
 
+
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    return {}
+    if state:
+        id = state.get("id")
+        if id:
+            return portal.pool.delete(id, data["orgId"])
+    return state
+
 
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '1m'
+        return "1m"
     if action == actions.delete:
-        return '1m'
+        return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.50/vhcs/plan/provider/dev/fibonacci.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,41 +9,33 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.plan import actions
-import vhcs.service.portal as portal
 
-def deploy(data: dict, state: dict) -> dict:
-    return portal.pool.create(data)
 
-def refresh(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
-    if state:
-        id = state.get('id')
-        if id:
-            return portal.pool.get(id, org_id)
-    
-    # Fall back with smart find by name
-    pools = portal.pool.list(org_id, search=f"name $eq {data['name']}")
-    if pools and len(pools) == 1:
-        return pools[0]
-    return state
-
-def decide(data: dict, state: dict):
-    return actions.skip
+def process(data: dict, state: dict) -> dict:
+    n = data["n"]
+    return {
+        'fibonacci': _fibonacci(n)
+    }
+
+def _fibonacci(n: int):
+    if n <= 0:
+        raise ValueError("n must be a positive integer.")
+    if n == 1:
+        return 0
+    if n == 2:
+        return 1
+
+    prev, curr = 0, 1
+    for _ in range(3, n + 1):
+        prev, curr = curr, prev + curr
+    return curr
 
 def destroy(data: dict, state: dict, force: bool) -> dict:
-    if state:
-        id = state.get('id')
-        if id:
-            return portal.pool.delete(id, data['orgId'])
-    return state
+    return
 
 def eta(action: str, data: dict, state: dict):
-    if action == actions.create:
-        return '1m'
-    if action == actions.delete:
-        return '1m'
+    return "10s"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/pool_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def deploy(data: dict, state: dict, save_state: Callable) -> dict:
     ret = admin.template.create(data)
     save_state(ret)
     id = ret["id"]
     org_id = data["orgId"]
     try:
-        template = admin.template.wait_for_ready(id, org_id, timeout='20m')
+        template = admin.template.wait_for_ready(id, org_id, timeout="20m")
     except Exception as e:
         template = admin.template.get(id, org_id)
         save_state(template)
         raise PluginException("Template deployment failed.") from e
     return template
 
 
@@ -56,12 +56,13 @@
 
 def destroy(data: dict, state: dict, force: bool) -> dict:
     id = state["id"]
     org_id = data["orgId"]
     admin.template.delete(id, org_id)
     admin.template.wait_for_deleted(id, org_id, 600)
 
+
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '15m'
+        return "15m"
     if action == actions.delete:
-        return '10m'
+        return "10m"
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/site.py` & `hcs-cli-0.1.50/vhcs/support/plan_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,36 +9,37 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.plan import actions
-from vhcs.service import portal
-
-def deploy(data: dict, state: dict) -> dict:
-    return portal.site.create(data)
-
-def refresh(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
-    if state:
-        id = state.get('id')
-        if id:
-            ret = portal.site.get(id, org_id)
-            if ret:
-                return ret
-    
-    # Fall back with smart find by name
-    return portal.site.find_by_name(data['name'], org_id)
-
-def decide(data: dict, state: dict):
-    return actions.skip
-
-def destroy(data: dict, state: dict, force: bool) -> dict:
-    return portal.site.delete(state['id'], data['orgId'])
-
-def eta(action: str, data: dict, state: dict):
-    if action == actions.create:
-        return '1m'
-    if action == actions.delete:
-        return '1m'
+import yaml
+import os
+from vhcs.ctxp import profile
+from vhcs.plan import PlanException
+
+
+def load_plan(file):
+    if not file:
+        file = _try_locating_plan_file()
+
+    with file:
+        payload = file.read()
+    data = yaml.safe_load(payload)
+    extra = {"profile": profile.current(exclude_secret=True)}
+    return data, extra
+
+
+def _try_locating_plan_file():
+    files = os.listdir()
+    candidates = []
+    for name in files:
+        if name.endswith(".plan.yml"):
+            if candidates:
+                raise PlanException(
+                    "Multiple plan files exist. Use the --file parameter to specify a target plan file."
+                )
+            candidates.append(name)
+    if not candidates:
+        raise PlanException("No plan yaml file found. Use the --file parameter to specify a target plan file.")
+    return open(candidates[0], "rt")
```

### Comparing `hcs-cli-0.1.48/vhcs/plan/provider/hcs/uag.py` & `hcs-cli-0.1.50/vhcs/plan/provider/hcs/uag.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 def deploy(data: dict, state: dict, save_state) -> dict:
     org_id = data["orgId"]
     if not state:
         deployment = admin.uag.create(data)
         save_state(deployment)
     else:
         deployment = state
-    id = deployment['id']
+    id = deployment["id"]
     try:
-        deployment = admin.uag.wait_for_ready(id, org_id, '10m')
+        deployment = admin.uag.wait_for_ready(id, org_id, "10m")
     except Exception as e:
         deployment = admin.uag.get(id, org_id)
         save_state(deployment)
         raise PluginException("Fail waiting for UAG deployment.") from e
     return deployment
 
 
@@ -53,15 +53,15 @@
         return actions.skip
 
 
 def destroy(data: dict, state: dict, force: bool) -> dict:
     id = state["id"]
     org_id = data["orgId"]
     admin.uag.delete(id, org_id)
-    admin.uag.wait_for_deleted(id, org_id, '10m')
-    
+    admin.uag.wait_for_deleted(id, org_id, "10m")
+
+
 def eta(action: str, data: dict, state: dict):
     if action == actions.create:
-        return '10m'
+        return "10m"
     if action == actions.delete:
-        return '10m'
-    
+        return "10m"
```

### Comparing `hcs-cli-0.1.48/vhcs/service/_util.py` & `hcs-cli-0.1.50/vhcs/sglib/client_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+
 from typing import Callable
 import time
-from vhcs.common.ctxp import profile, panic
-from vhcs.common.sglib import hcs_client
+from vhcs.ctxp import profile, panic
+from vhcs.sglib import hcs_client
 from vhcs.util.query_util import with_query, PageRequest
-from vhcs.common import duration
+from vhcs.ctxp import duration
+
 
 def hdc_service_client(service_name: str):
     url = profile.current().hcs.url
     if not url.endswith("/"):
         url += "/"
     url += service_name
     return hcs_client(url)
@@ -47,20 +49,21 @@
     if not url:
         panic("Missing profile property: hcs.regions")
     if not url.endswith("/"):
         url += "/"
     url += service_name
     return hcs_client(url)
 
+
 class default_crud:
     def __init__(self, client, base_context: str, resource_type_name: str):
         self._client = client
         self._base_context = base_context
         self._resource_type_name = resource_type_name
-    
+
     def get(self, id: str, org_id: str, **kwargs):
         url = with_query(f"{self._base_context}/{id}?org_id={org_id}", **kwargs)
         return self._client.get(url)
 
     def list(self, org_id: str, **kwargs):
         def _get_page(query_string):
             url = self._base_context + f"?org_id={org_id}&" + query_string
@@ -73,82 +76,85 @@
         return self._client.post(url, json=payload)
 
     def delete(self, id: str, org_id: str, **kwargs):
         url = with_query(f"{self._base_context}/{id}?org_id={org_id}", **kwargs)
         return self._client.delete(url)
 
     def wait_for_deleted(self, id: str, org_id: str, timeout: str | int):
-        name = self._resource_type_name + '/' + id
+        name = self._resource_type_name + "/" + id
         fn_get = lambda: self.get(id, org_id)
         return wait_for_res_deleted(name, fn_get, timeout)
 
+
 def _parse_timeout(timeout: str | int):
     if isinstance(timeout, int):
         return timeout
     if isinstance(timeout, str):
         return duration.to_seconds(timeout)
-        
+
     raise Exception(f"Invalid timout. Type={type(timeout).__name__}, value={timeout}")
 
+
 def wait_for_res_deleted(resource_name: str, fn_get: Callable, timeout: str | int, polling_interval_seconds: int = 20):
     timeout_seconds = _parse_timeout(timeout)
     start = time.time()
     while True:
         t = fn_get()
         if t == None:
             return
-        
+
         now = time.time()
         remaining_seconds = timeout_seconds - (now - start)
         if remaining_seconds < 1:
             msg = f"Error waiting for resource {resource_name} deleted: timeout."
             raise TimeoutError(msg)
         sleep_seconds = remaining_seconds
         if sleep_seconds > polling_interval_seconds:
             sleep_seconds = polling_interval_seconds
         time.sleep(sleep_seconds)
 
 
-
-def wait_for_res_status(resource_name: str, 
-                        fn_get: Callable, 
-                        get_status: str | Callable, 
-                        status_map: dict = None, 
-                        is_ready: Callable = None, 
-                        is_error: Callable = None, 
-                        is_transition: Callable = None, 
-                        timeout: str | int = '10m', 
-                        polling_interval: str | int = '20s',
-                        not_found_as_success: bool = False):
+def wait_for_res_status(
+    resource_name: str,
+    fn_get: Callable,
+    get_status: str | Callable,
+    status_map: dict = None,
+    is_ready: Callable = None,
+    is_error: Callable = None,
+    is_transition: Callable = None,
+    timeout: str | int = "10m",
+    polling_interval: str | int = "20s",
+    not_found_as_success: bool = False,
+):
     timeout_seconds = _parse_timeout(timeout)
     polling_interval_seconds = _parse_timeout(polling_interval)
     if polling_interval_seconds < 3:
         polling_interval_seconds = 3
     start = time.time()
     prefix = f"Error waiting for resource {resource_name}: "
 
     if isinstance(get_status, str):
         field_name = get_status
         get_status = lambda t: t[field_name]
     if status_map:
-        if isinstance(status_map['ready'], str):
-            status_map['ready'] = [status_map['ready']]
-        if isinstance(status_map['transition'], str):
-            status_map['transition'] = [status_map['transition']]
-        if isinstance(status_map['error'], str):
-            status_map['error'] = [status_map['error']]
+        if isinstance(status_map["ready"], str):
+            status_map["ready"] = [status_map["ready"]]
+        if isinstance(status_map["transition"], str):
+            status_map["transition"] = [status_map["transition"]]
+        if isinstance(status_map["error"], str):
+            status_map["error"] = [status_map["error"]]
         if is_ready:
             raise Exception("Can not specify is_ready when status_map is provided.")
         if is_error:
             raise Exception("Can not specify is_error when status_map is provided.")
         if is_transition:
             raise Exception("Can not specify is_transition when status_map is provided.")
-        is_ready = lambda s: s in status_map['ready']
-        is_error = lambda s: s in status_map['error']
-        is_transition = lambda s: s in status_map['transition']
+        is_ready = lambda s: s in status_map["ready"]
+        is_error = lambda s: s in status_map["error"]
+        is_transition = lambda s: s in status_map["transition"]
     else:
         if not is_ready:
             raise Exception("Either status_map or is_ready must be specified.")
         if not is_error:
             raise Exception("Either status_map or is_error must be specified.")
         if not is_transition:
             raise Exception("Either status_map or is_transition must be specified.")
@@ -164,15 +170,17 @@
             msg = prefix + f"Status error. Actual={status}"
             if status_map:
                 msg += f", expected={status_map['ready']}"
             raise RuntimeError(msg)
         if is_ready(status):
             return t
         if not is_transition(status):
-            raise RuntimeError(prefix + f"Unexpected status: {status}. If this is a transition, add it to status_map['transition'].")
+            raise RuntimeError(
+                prefix + f"Unexpected status: {status}. If this is a transition, add it to status_map['transition']."
+            )
 
         now = time.time()
         remaining_seconds = timeout_seconds - (now - start)
         if remaining_seconds < 1:
             raise TimeoutError(prefix + "Timeout.")
         sleep_seconds = remaining_seconds
         if sleep_seconds > polling_interval_seconds:
```

### Comparing `hcs-cli-0.1.48/vhcs/service/admin/ad.py` & `hcs-cli-0.1.50/vhcs/service/admin/ad.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client, default_crud, wait_for_res_status
+from vhcs.sglib.client_util import hdc_service_client, default_crud, wait_for_res_status
 
 _client = hdc_service_client("admin")
-_crud = default_crud(_client, "/v2/active-directories", 'ad')
+_crud = default_crud(_client, "/v2/active-directories", "ad")
 get = _crud.get
 list = _crud.list
 create = _crud.create
 delete = _crud.delete
```

### Comparing `hcs-cli-0.1.48/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.50/vhcs/service/admin/azure_infra.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("admin")
 
+
 def get_compute_vm_skus(provider_instance_id: str, **kwargs):
     def _get_page(query_string):
         url = f"/v2/providers/azure/instances/{provider_instance_id}/compute-vm-skus?" + query_string
         ret = _client.get(url)
-        
+
         return ret
 
     return PageRequest(_get_page, **kwargs).get()
 
 
 def get_networks(providerInstanceId: str, **kwargs):
     url = f"/v2/providers/azure/instances/{providerInstanceId}/preferences/networks"
```

### Comparing `hcs-cli-0.1.48/vhcs/service/admin/edge.py` & `hcs-cli-0.1.50/vhcs/service/admin/edge.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,122 +12,140 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import httpx
 import logging
 from typing import Callable
-from .._util import hdc_service_client, default_crud, wait_for_res_status
+from vhcs.sglib.client_util import hdc_service_client, default_crud, wait_for_res_status
 from . import edge
 
 log = logging.getLogger(__name__)
 
 _client = hdc_service_client("admin")
-_crud = default_crud(_client, "/v2/edge-deployments", 'edge')
+_crud = default_crud(_client, "/v2/edge-deployments", "edge")
 
 get = _crud.get
 list = _crud.list
 delete = _crud.delete
 create = _crud.create
 wait_for_deleted = _crud.wait_for_deleted
 
-def wait_for(id: str, org_id: str, 
-             status_map: dict = None, 
-             is_ready: Callable = None, 
-             is_error: Callable = None, 
-             is_transition: Callable = None, 
-             timeout: str | int = '20m'):
-    name = 'edge/' + id
+
+def wait_for(
+    id: str,
+    org_id: str,
+    status_map: dict = None,
+    is_ready: Callable = None,
+    is_error: Callable = None,
+    is_transition: Callable = None,
+    timeout: str | int = "20m",
+):
+    name = "edge/" + id
+
     def fn_get():
         return get(id, org_id)
-    return wait_for_res_status(resource_name=name, 
-                               fn_get=fn_get, 
-                               get_status='status', 
-                               status_map=status_map, 
-                               is_ready=is_ready,
-                               is_error=is_error,
-                               is_transition=is_transition,
-                               timeout=timeout, 
-                               polling_interval=60)
+
+    return wait_for_res_status(
+        resource_name=name,
+        fn_get=fn_get,
+        get_status="status",
+        status_map=status_map,
+        is_ready=is_ready,
+        is_error=is_error,
+        is_transition=is_transition,
+        timeout=timeout,
+        polling_interval=60,
+    )
     # Edge status
-    # [ 
-    # CONNECT_PENDING, 
-    # CREATE_ACCEPTED, 
-    # CREATE_FAILED, 
-    # CREATE_PENDING, 
-    # CREATING, 
-    # DELETED, 
-    # DELETE_FAILED, 
-    # DELETE_PENDING, 
-    # DELETING, 
-    # FORCE_DELETE_PENDING, 
-    # FORCE_DELETING, 
-    # FORCE_REPAIR_ACCEPTED, 
-    # FORCE_REPAIR_PENDING, 
-    # MIGRATE_FAILED, 
-    # MIGRATE_PENDING, 
-    # MIGRATING, 
-    # POST_PROVISIONING_CONFIG_IN_PROGRESS, 
-    # READY, 
-    # REPAIRING, 
-    # REPAIR_ACCEPTED, 
-    # REPAIR_FAILED, 
-    # REPAIR_PENDING, 
-    # UPDATE_FAILED, 
-    # UPDATE_PENDING, 
-    # UPDATING, 
-    # UPGRADE_FAILED, 
-    # UPGRADE_PENDING, 
-    # UPGRADING 
+    # [
+    # CONNECT_PENDING,
+    # CREATE_ACCEPTED,
+    # CREATE_FAILED,
+    # CREATE_PENDING,
+    # CREATING,
+    # DELETED,
+    # DELETE_FAILED,
+    # DELETE_PENDING,
+    # DELETING,
+    # FORCE_DELETE_PENDING,
+    # FORCE_DELETING,
+    # FORCE_REPAIR_ACCEPTED,
+    # FORCE_REPAIR_PENDING,
+    # MIGRATE_FAILED,
+    # MIGRATE_PENDING,
+    # MIGRATING,
+    # POST_PROVISIONING_CONFIG_IN_PROGRESS,
+    # READY,
+    # REPAIRING,
+    # REPAIR_ACCEPTED,
+    # REPAIR_FAILED,
+    # REPAIR_PENDING,
+    # UPDATE_FAILED,
+    # UPDATE_PENDING,
+    # UPDATING,
+    # UPGRADE_FAILED,
+    # UPGRADE_PENDING,
+    # UPGRADING
     # ]
-def safe_delete(id: str, org_id: str, timeout: str | int = '20m'):
 
+
+def safe_delete(id: str, org_id: str, timeout: str | int = "20m"):
     try:
         edge.delete(id, org_id=org_id)
     except httpx.HTTPStatusError as e:
         if e.response.status_code != 409:
             raise
         _wait_for_terminal_state(id, org_id, timeout)
         edge.delete(id, org_id=org_id)
 
     edge.wait_for_deleted(id, org_id, "10m")
 
+
 def _wait_for_terminal_state(id, org_id, timeout):
-    name = 'edge/' + id
-    terminal_status = ['CREATE_FAILED', 'DELETED', 'DELETE_FAILED', 'MIGRATE_FAILED', 'READY', 'REPAIR_FAILED', 'UPDATE_FAILED', 'UPGRADE_FAILED']
+    name = "edge/" + id
+    terminal_status = [
+        "CREATE_FAILED",
+        "DELETED",
+        "DELETE_FAILED",
+        "MIGRATE_FAILED",
+        "READY",
+        "REPAIR_FAILED",
+        "UPDATE_FAILED",
+        "UPGRADE_FAILED",
+    ]
     transition_status = [
-        'CONNECT_PENDING', 
-        'CREATE_ACCEPTED', 
-        'CREATE_PENDING', 
-        'CREATING',  
-        'DELETE_PENDING', 
-        'DELETING', 
-        'FORCE_DELETE_PENDING', 
-        'FORCE_DELETING', 
-        'FORCE_REPAIR_ACCEPTED', 
-        'FORCE_REPAIR_PENDING', 
-        'MIGRATE_PENDING', 
-        'MIGRATING', 
-        'POST_PROVISIONING_CONFIG_IN_PROGRESS', 
-        'REPAIRING', 
-        'REPAIR_ACCEPTED', 
-        'REPAIR_PENDING',
-        'UPDATE_PENDING', 
-        'UPDATING', 
-        'UPGRADE_PENDING', 
-        'UPGRADING'
+        "CONNECT_PENDING",
+        "CREATE_ACCEPTED",
+        "CREATE_PENDING",
+        "CREATING",
+        "DELETE_PENDING",
+        "DELETING",
+        "FORCE_DELETE_PENDING",
+        "FORCE_DELETING",
+        "FORCE_REPAIR_ACCEPTED",
+        "FORCE_REPAIR_PENDING",
+        "MIGRATE_PENDING",
+        "MIGRATING",
+        "POST_PROVISIONING_CONFIG_IN_PROGRESS",
+        "REPAIRING",
+        "REPAIR_ACCEPTED",
+        "REPAIR_PENDING",
+        "UPDATE_PENDING",
+        "UPDATING",
+        "UPGRADE_PENDING",
+        "UPGRADING",
     ]
+
     def fn_get():
         return get(id, org_id)
-    status_map = {
-        'ready': terminal_status,
-        'error': [],
-        'transition': transition_status
-    }
-    
+
+    status_map = {"ready": terminal_status, "error": [], "transition": transition_status}
+
     wait_for_res_status(
-        resource_name=name, 
-        fn_get=fn_get, 
-        get_status='status', 
-        status_map=status_map, 
+        resource_name=name,
+        fn_get=fn_get,
+        get_status="status",
+        status_map=status_map,
         timeout=timeout,
-        not_found_as_success=True)
+        not_found_as_success=True,
+    )
```

### Comparing `hcs-cli-0.1.48/vhcs/service/admin/helper.py` & `hcs-cli-0.1.50/vhcs/service/admin/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,30 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
+from . import uag
 
 _client = hdc_service_client("admin")
 
 
 def list_resources_by_provider(resource_type: str, provider_instance_id: str, limit: int = 10):
     def _get_page(query_string):
         url = f"/v2/{resource_type}?" + query_string
         return _client.get(url)
 
     search = f"providerInstanceId $eq {provider_instance_id}"
     return PageRequest(_get_page, search=search, limit=limit).get()
+
+
+def get_uags_by_edge(edge_id: str, org_id: str):
+    uags = uag.list(org_id)
+    ret = []
+    for u in uags:
+        if u["edgeDeploymentId"] == edge_id:
+            ret.append(u)
+    return ret
```

### Comparing `hcs-cli-0.1.48/vhcs/service/admin/provider.py` & `hcs-cli-0.1.50/vhcs/service/admin/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,35 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("admin")
 
+
 def list(label: str, org_id: str, **kwargs):
     def _get_page(query_string):
         url = f"/v2/providers/{label}/instances?{query_string}?org_id={org_id}"
         return _client.get(url)
 
     return PageRequest(_get_page, **kwargs).get()
 
+
 def get(label: str, id: str, org_id: str, **kwargs):
     url = f"/v2/providers/{label}/instances/{id}?org_id={org_id}"
     url = with_query(url, **kwargs)
     return _client.get(url)
 
+
 def create(label: str, payload):
     return _client.post(f"/v2/providers/{label}/instances", json=payload)
 
 
 def delete(label: str, id: str, org_id: str, **kwargs):
     url = f"/v2/providers/{label}/instances/{id}?org_id={org_id}"
     url = with_query(url, **kwargs)
-    return _client.delete(url)
+    return _client.delete(url)
```

### Comparing `hcs-cli-0.1.48/vhcs/service/admin/template.py` & `hcs-cli-0.1.50/vhcs/service/admin/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,49 +9,54 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client, default_crud, wait_for_res_status
+from vhcs.sglib.client_util import hdc_service_client, default_crud, wait_for_res_status
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("admin")
-_crud = default_crud(_client, "/v2/templates", 'template')
+_crud = default_crud(_client, "/v2/templates", "template")
 get = _crud.get
 list = _crud.list
 
+
 def create(payload):
     return _crud.create(payload, ignore_warnings=True)
 
+
 def delete(id: str, org_id: str, force: bool = True):
     return _crud.delete(id, org_id, force=force)
 
-def wait_for_ready(id: str, org_id: str, timeout: str | int = '10m'):
-    name = 'template/' + id
+
+def wait_for_ready(id: str, org_id: str, timeout: str | int = "10m"):
+    name = "template/" + id
     fn_get = lambda: get(id, org_id)
-    fn_get_status = lambda t: t['reportedStatus'].get('statusValue')
+    fn_get_status = lambda t: t["reportedStatus"].get("statusValue")
     status_map = {
-        'ready': 'READY',
-        'error': 'ERROR',
-        'transition': ['EXPANDING', 'SHRINKING', 'INIT']
+        "ready": "READY",
+        "error": "ERROR",
+        "transition": ["EXPANDING", "SHRINKING", "INIT"]
         # Unexpected:
         # DELETING
     }
-    return wait_for_res_status(resource_name=name, 
-                               fn_get=fn_get, 
-                               get_status=fn_get_status, 
-                               status_map=status_map, 
-                               timeout=timeout)
+    return wait_for_res_status(
+        resource_name=name, fn_get=fn_get, get_status=fn_get_status, status_map=status_map, timeout=timeout
+    )
+
 
 wait_for_deleted = _crud.wait_for_deleted
 
+
 def list_vms(template_id: str, **kwargs):
     def _get_page(query_string):
         url = f"/v2/templates/{template_id}/vms?" + query_string
         return _client.get(url)
+
     return PageRequest(_get_page, **kwargs).get()
 
+
 def get_vm(template_id: str, vm_id: str, **kwargs):
     url = with_query(f"/v2/templates/{template_id}/vms/{vm_id}", **kwargs)
     return _client.get(url)
```

### Comparing `hcs-cli-0.1.48/vhcs/service/admin/uag.py` & `hcs-cli-0.1.50/vhcs/service/admin/uag.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,60 +9,60 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client, default_crud, wait_for_res_status
+from vhcs.sglib.client_util import hdc_service_client, default_crud, wait_for_res_status
 
 _client = hdc_service_client("admin")
-_crud = default_crud(_client, "/v2/uag-deployments", 'uag')
+_crud = default_crud(_client, "/v2/uag-deployments", "uag")
 get = _crud.get
 list = _crud.list
 create = _crud.create
 delete = _crud.delete
 wait_for_deleted = _crud.wait_for_deleted
+
+
 def wait_for_ready(id, org_id, timeout):
-    name = 'uag/' + id
+    name = "uag/" + id
     fn_get = lambda: get(id, org_id)
     status_map = {
-        'ready': 'READY',
-        'error': 'FAILED',
-        'transition': [
-            'DEPLOYING', 
-            'PENDING', 
+        "ready": "READY",
+        "error": "FAILED",
+        "transition": [
+            "DEPLOYING",
+            "PENDING",
         ]
         # Other
-        # 'ADDING_EXTERNAL_ACCESS', 
-        # 'ADDING_EXTERNAL_ACCESS_FAILED', 
-        # 'ADDING_EXTERNAL_ACCESS_ROLLBACK', 
-        # 'ADDING_EXTERNAL_ACCESS_ROLLBACK_FAILED', 
-        # 'ADDING_INTERNAL_ACCESS', 
-        # 'ADDING_INTERNAL_ACCESS_FAILED', 
-        # 'ADDING_INTERNAL_ACCESS_ROLLBACK', 
-        # 'ADDING_INTERNAL_ACCESS_ROLLBACK_FAILED', 
-        # 'DELETED', 
-        # 'DELETE_PENDING', 
-        # 'DELETING', 
-        # 'DELETION_FAILED', 
-        # 'PARTIALLY_READY', 
-        # 'REMOVING_EXTERNAL_ACCESS', 
-        # 'REMOVING_EXTERNAL_ACCESS_FAILED', 
-        # 'REMOVING_EXTERNAL_ACCESS_ROLLBACK', 
-        # 'REMOVING_EXTERNAL_ACCESS_ROLLBACK_FAILED', 
-        # 'REMOVING_INTERNAL_ACCESS', 
-        # 'REMOVING_INTERNAL_ACCESS_FAILED', 
-        # 'REMOVING_INTERNAL_ACCESS_ROLLBACK', 
-        # 'REMOVING_INTERNAL_ACCESS_ROLLBACK_FAILED', 
-        # 'UPDATE_FAILED', 
-        # 'UPDATE_PENDING', 
-        # 'UPDATING', 
-        # 'UPGRADE_FAILED', 
-        # 'UPGRADE_PENDING', 
+        # 'ADDING_EXTERNAL_ACCESS',
+        # 'ADDING_EXTERNAL_ACCESS_FAILED',
+        # 'ADDING_EXTERNAL_ACCESS_ROLLBACK',
+        # 'ADDING_EXTERNAL_ACCESS_ROLLBACK_FAILED',
+        # 'ADDING_INTERNAL_ACCESS',
+        # 'ADDING_INTERNAL_ACCESS_FAILED',
+        # 'ADDING_INTERNAL_ACCESS_ROLLBACK',
+        # 'ADDING_INTERNAL_ACCESS_ROLLBACK_FAILED',
+        # 'DELETED',
+        # 'DELETE_PENDING',
+        # 'DELETING',
+        # 'DELETION_FAILED',
+        # 'PARTIALLY_READY',
+        # 'REMOVING_EXTERNAL_ACCESS',
+        # 'REMOVING_EXTERNAL_ACCESS_FAILED',
+        # 'REMOVING_EXTERNAL_ACCESS_ROLLBACK',
+        # 'REMOVING_EXTERNAL_ACCESS_ROLLBACK_FAILED',
+        # 'REMOVING_INTERNAL_ACCESS',
+        # 'REMOVING_INTERNAL_ACCESS_FAILED',
+        # 'REMOVING_INTERNAL_ACCESS_ROLLBACK',
+        # 'REMOVING_INTERNAL_ACCESS_ROLLBACK_FAILED',
+        # 'UPDATE_FAILED',
+        # 'UPDATE_PENDING',
+        # 'UPDATING',
+        # 'UPGRADE_FAILED',
+        # 'UPGRADE_PENDING',
         # 'UPGRADING'
     }
-    return wait_for_res_status(resource_name=name, 
-                               fn_get=fn_get, 
-                               get_status='status', 
-                               status_map=status_map, 
-                               timeout=timeout)
+    return wait_for_res_status(
+        resource_name=name, fn_get=fn_get, get_status="status", status_map=status_map, timeout=timeout
+    )
```

### Comparing `hcs-cli-0.1.48/vhcs/service/auth/admin.py` & `hcs-cli-0.1.50/vhcs/service/auth/admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("auth")
 
+
 def get_org_idp_map(**kwargs):
     url = with_query(f"/v1/admin/org-idp-map", **kwargs)
     return _client.get(url)
 
-#def create_org_idp_map():
+
+# def create_org_idp_map():
```

### Comparing `hcs-cli-0.1.48/vhcs/service/ims/helper.py` & `hcs-cli-0.1.50/vhcs/service/ims/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,54 +14,57 @@
 """
 
 import time
 import httpx
 from . import images, image_copies
 from .version import version
 
+
 def get_images_by_provider_instance_with_asset_details(providerInstanceId: str, org_id: str):
     all_images = images.list(org_id)
-    copies = image_copies.list(org_id, include_catalog_details=True,
-                      search=f"providerInstanceId $eq {providerInstanceId}")
+    copies = image_copies.list(
+        org_id, include_catalog_details=True, search=f"providerInstanceId $eq {providerInstanceId}"
+    )
     ret = []
     for copy in copies:
         imageId = copy["catalogDetails"]["imageId"]
         for image in all_images:
-            if image['id'] == imageId:
+            if image["id"] == imageId:
                 # add additional info
-                image['_assetDetails'] = copy['assetDetails']
+                image["_assetDetails"] = copy["assetDetails"]
                 ret.append(image)
                 break
     return ret
 
+
 def delete_images(image_ids: list[str], org_id: str, timeout: int | str):
     def del_impl(image_id: str):
         version_api = version(image_id, org_id)
         versions = version_api.list()
         everything_ok = True
         for v in versions:
-            s = v['status']
-            if s == 'DELETING':
+            s = v["status"]
+            if s == "DELETING":
                 continue
             # AVAILABLE, DELETING, DISABLED, FAILED, IMPORT_COMPLETE, IMPORT_IN_PROGRESS, PARTIALLY_AVAILABLE, PENDING, PUBLISH_IN_PROGRESS, REPLICATION_IN_PROGRESS
             try:
-                version_api.delete(v['id'])
+                version_api.delete(v["id"])
             except httpx.HTTPStatusError:
                 everything_ok = False
         return everything_ok
 
     to_delete = list(image_ids)
 
     while True:
         temp = list(to_delete)
         for image_id in temp:
             if del_impl(image_id):
                 to_delete.remove(image_id)
         if not to_delete:
             break
         time.sleep(60)
-        
-    if timeout == '0':
+
+    if timeout == "0":
         return
-    
+
     for image_id in image_ids:
-        images.wait_for_deleted(image_id, org_id, timeout)  # todo: timeout
+        images.wait_for_deleted(image_id, org_id, timeout)  # todo: timeout
```

### Comparing `hcs-cli-0.1.48/vhcs/service/ims/image_copies.py` & `hcs-cli-0.1.50/vhcs/service/ims/image_copies.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import PageRequest
 
 _client = hdc_service_client("ims-catalog")
 
 
 def list(org_id: str, **kwargs):
     def _get_page(query_string):
         url = f"/v1/image-copies?org_id={org_id}&{query_string}"
         return _client.get(url)
+
     return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.48/vhcs/service/ims/images.py` & `hcs-cli-0.1.50/vhcs/service/ims/images.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,39 +10,49 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import builtins
-from .._util import hdc_service_client, default_crud, wait_for_res_status
+from vhcs.sglib.client_util import hdc_service_client, default_crud, wait_for_res_status
 from vhcs.util.query_util import PageRequest
 
 _imagemgmt_client = hdc_service_client("imagemgmt")
 _ims_catalog_client = hdc_service_client("ims-catalog")
-_crud = default_crud(_ims_catalog_client, "/v1/images", 'image')
+_crud = default_crud(_ims_catalog_client, "/v1/images", "image")
 
 list = _crud.list
 get = _crud.get
 delete = _crud.delete
 wait_for_deleted = _crud.wait_for_deleted
 
+
 def create(action: str, image_catalog_request: dict):
-    #https://cloud-sg.horizon.vmware.com/images/swagger-ui/index.html#/Images/createImageCatalogUsingPOST
+    # https://cloud-sg.horizon.vmware.com/images/swagger-ui/index.html#/Images/createImageCatalogUsingPOST
 
-    #POST https://cloud-sg.horizon.vmware.com/imagemgmt/v1/images?action=import
+    # POST https://cloud-sg.horizon.vmware.com/imagemgmt/v1/images?action=import
     return _imagemgmt_client.post("/v1/images?action=" + action, image_catalog_request)
 
+
 def wait_for(image_id: str, org_id: str, expected_status):
-    res_name = 'image/' + image_id
+    res_name = "image/" + image_id
     fn_get = lambda: get(image_id, org_id)
-    unexpected_status = set(['IMPORT_COMPLETE', 'AVAILABLE', 'FAILED', 'DELETING', 'DISABLED', 'REPLICATION_IN_PROGRESS', 'PARTIALLY_AVAILABLE'])
+    unexpected_status = set(
+        [
+            "IMPORT_COMPLETE",
+            "AVAILABLE",
+            "FAILED",
+            "DELETING",
+            "DISABLED",
+            "REPLICATION_IN_PROGRESS",
+            "PARTIALLY_AVAILABLE",
+        ]
+    )
     status_map = {
-        'ready': expected_status,
-        'transition': ['IN_PROGRESS', 'PUBLISH_IN_PROGRESS', 'PENDING'],
-        'error': builtins.list(unexpected_status - set(expected_status))
+        "ready": expected_status,
+        "transition": ["IN_PROGRESS", "PUBLISH_IN_PROGRESS", "PENDING"],
+        "error": builtins.list(unexpected_status - set(expected_status)),
     }
-    return wait_for_res_status(resource_name=res_name, 
-                               fn_get=fn_get, 
-                               get_status='status', 
-                               status_map=status_map, 
-                               timeout="60m")
+    return wait_for_res_status(
+        resource_name=res_name, fn_get=fn_get, get_status="status", status_map=status_map, timeout="60m"
+    )
```

### Comparing `hcs-cli-0.1.48/vhcs/service/ims/version.py` & `hcs-cli-0.1.50/vhcs/service/ims/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client, wait_for_res_deleted, wait_for_res_status
+from vhcs.sglib.client_util import hdc_service_client, wait_for_res_deleted, wait_for_res_status
 from vhcs.util.query_util import PageRequest, with_query
 
 _imagemgmt_client = hdc_service_client("imagemgmt")
 _ims_catalog_client = hdc_service_client("ims-catalog")
 
+
 class version:
     def __init__(self, image_id: str, org_id: str):
         self._image_id = image_id
         self._org_id = org_id
 
     def get(self, id: str, **kwargs):
         url = with_query(f"/v1/images/{self._image_id}/versions/{id}?org_id={self._org_id}", **kwargs)
@@ -39,35 +40,45 @@
     #     url = f"/v1/images/{image_id}/versions?org_id={org_id}"
     #     url = with_query(url, **kwargs)
     #     return _client.post(url, json=payload)
 
     def delete(self, id: str, **kwargs):
         url = with_query(f"/v1/images/{self._image_id}/versions/{id}?org_id={self._org_id}", **kwargs)
         return _imagemgmt_client.delete(url)
-    
-    def wait_for_deleted(self, id: str, timeout: int | str='10m'):
-        name = 'image_version/' + id
+
+    def wait_for_deleted(self, id: str, timeout: int | str = "10m"):
+        name = "image_version/" + id
+
         def fn_get():
             return self.get(id)
+
         return wait_for_res_deleted(name, fn_get, timeout)
 
     def publish(self, id: str, version_publish_create_TO: dict):
         # https://cloud-sg.horizon.vmware.com/images/swagger-ui/index.html#/Images/publishVersionV2UsingPOST
-        if version_publish_create_TO['orgId'] != self._org_id:
-            raise Exception(f"Invalid payload. version_publish_create_TO orgId {version_publish_create_TO['orgId']} does not match API context {self._org_id}")
+        if version_publish_create_TO["orgId"] != self._org_id:
+            raise Exception(
+                f"Invalid payload. version_publish_create_TO orgId {version_publish_create_TO['orgId']} does not match API context {self._org_id}"
+            )
         url = f"/v1/images/{self._image_id}/versions/{id}?action=publish"
         return _imagemgmt_client.post(url, version_publish_create_TO)
-    
-    def wait_for_publish_complete(self, id: str, timeout: str|int = '40m'):
-        res_name = 'version/' + id
+
+    def wait_for_publish_complete(self, id: str, timeout: str | int = "40m"):
+        res_name = "version/" + id
+
         def fn_get():
             return self.get(id)
+
         status_map = {
-            'ready': ['AVAILABLE'],
-            'transition': ['IMPORT_COMPLETE', 'IMPORT_IN_PROGRESS', 'PENDING', 'PUBLISH_IN_PROGRESS', 'REPLICATION_IN_PROGRESS'],
-            'error': ['FAILED', 'DELETING', 'DISABLED', 'PARTIALLY_AVAILABLE']
+            "ready": ["AVAILABLE"],
+            "transition": [
+                "IMPORT_COMPLETE",
+                "IMPORT_IN_PROGRESS",
+                "PENDING",
+                "PUBLISH_IN_PROGRESS",
+                "REPLICATION_IN_PROGRESS",
+            ],
+            "error": ["FAILED", "DELETING", "DISABLED", "PARTIALLY_AVAILABLE"],
         }
-        wait_for_res_status(resource_name=res_name, 
-                            fn_get=fn_get, 
-                            get_status='status', 
-                            status_map=status_map, 
-                            timeout=timeout)
+        wait_for_res_status(
+            resource_name=res_name, fn_get=fn_get, get_status="status", status_map=status_map, timeout=timeout
+        )
```

### Comparing `hcs-cli-0.1.48/vhcs/service/inventory/vm.py` & `hcs-cli-0.1.50/vhcs/service/inventory/vm.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("inventory")
 
+
 @staticmethod
 def get(template_id: str, vm_id: str, org_id: str = None, **kwargs):
     url = f"/v1/{template_id}/{vm_id}"
     if org_id:
         url += "?org_id=" + org_id
     url = with_query(url, **kwargs)
     return _client.get(url)
 
+
 @staticmethod
 def list(template_id: str, org_id: str, **kwargs):
     def _get_page(query_string):
         url = f"/v1/{template_id}?org_id={org_id}"
         if query_string:
             url += "&" + query_string
         print(url)
         return _client.get(url)
 
-    return PageRequest(_get_page, **kwargs).get()
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.48/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.50/vhcs/service/lcm/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,35 +11,38 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import json
 from typing import Any
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("lcm")
 
 
 def get(id: str, **kwargs: Any):
     url = with_query(f"/v1/providers/{id}", **kwargs)
     return _client.get(url)
 
+
 def list(**kwargs):
     def _get_page(query_string):
         url = "/v1/providers?" + query_string
         return _client.get(url)
 
     return PageRequest(_get_page, **kwargs).get()
 
+
 def delete(id: str):
     resp = _client.delete(f"/v1/providers/{id}")
     return _convert_resp(resp)
 
+
 def create(data: dict):
     url = "/v1/providers/" + data["type"].lower()
     return _client.post(url, json=data)
 
 
 def _convert_resp(resp):
     if resp:
```

### Comparing `hcs-cli-0.1.48/vhcs/service/lcm/template.py` & `hcs-cli-0.1.50/vhcs/service/lcm/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,45 +12,49 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
 import json
 from typing import Any
-from .._util import hdc_service_client, default_crud
+from vhcs.sglib.client_util import hdc_service_client, default_crud
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("lcm")
-_crud = default_crud(_client, "/v1/templates", 'template')
+_crud = default_crud(_client, "/v1/templates", "template")
 
 get = _crud.get
 
+
 def list(name: str = None, **kwargs):
     def _get_page(query_string):
         url = "/v1/templates?" + query_string
         return _client.get(url)
 
     ret = PageRequest(_get_page, **kwargs).get()
     if name:
         # filter_fn = lambda t : t.name.find(name) >= 0
         def filter_fn(t):
             return t.name.find(name) >= 0
 
         ret = list(filter(filter_fn, ret))
     return ret
 
+
 def delete(id: str, org_id: str, force: bool):
     resp = _client.delete(f"/v1/templates/{id}?org_id={org_id}&force={force}")
     return _convert_resp(resp)
 
+
 def create(template: dict):
     url = "/v1/templates"
     url += "/" + template["providerType"].lower()
     return _client.post(url=url, json=template)
 
+
 def wait(
     id: str,
     timeout_seconds: int,
     expected_status: list = ["READY"],
     exclude_status: list = ["ERROR"],
     interval_seconds: int = 10,
 ):
```

### Comparing `hcs-cli-0.1.48/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.50/vhcs/service/org_service/datacenter.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("org-service")
 
 
 def get(id: str, **kwargs):
     url = with_query(f"/v1/datacenters/{id}", **kwargs)
     return _client.get(url)
 
+
 def list(**kwargs):
     url = with_query(f"/v1/datacenters", **kwargs)
     return _client.get(url)
 
+
 def find_by_org(orgId, **kwargs):
     url = with_query(f"/v1/datacenters/orgs/{orgId}", **kwargs)
     return _client.get(url)
-
```

### Comparing `hcs-cli-0.1.48/vhcs/service/org_service/details.py` & `hcs-cli-0.1.50/vhcs/service/org_service/details.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("org-service")
 
 
 def get(id: str, **kwargs):
     url = with_query(f"/v1/org-details/{id}", **kwargs)
     return _client.get(url)
 
+
 def list(**kwargs):
     def _get_page(query_string):
         url = "/v1/org-details?" + query_string
         return _client.get(url)
 
     return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.48/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.50/vhcs/service/pki/certificate.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 
 _client = hdc_service_client("pki")
 
 
 def test():
     print("TODO: test. Migrate that from pki-util here")
```

### Comparing `hcs-cli-0.1.48/vhcs/service/portal/entitlement.py` & `hcs-cli-0.1.50/vhcs/service/portal/entitlement.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import logging
-from .._util import hdc_service_client, default_crud
+from vhcs.sglib.client_util import hdc_service_client, default_crud
 from vhcs.util.query_util import with_query, PageRequest
 
 log = logging.getLogger(__name__)
 _client = hdc_service_client("portal")
 _crud = default_crud(_client, "/v2/entitlements", "entitlement")
 
 create = _crud.create
 get = _crud.get
 list = _crud.list
-delete = _crud.delete
+delete = _crud.delete
```

### Comparing `hcs-cli-0.1.48/vhcs/service/portal/pool.py` & `hcs-cli-0.1.50/vhcs/service/portal/pool.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import logging
-from .._util import hdc_service_client, default_crud
+from vhcs.sglib.client_util import hdc_service_client, default_crud
 from vhcs.util.query_util import with_query, PageRequest
 
 log = logging.getLogger(__name__)
 _client = hdc_service_client("portal")
 _crud = default_crud(_client, "/v2/pools", "pool")
 
 create = _crud.create
```

### Comparing `hcs-cli-0.1.48/vhcs/service/portal/site.py` & `hcs-cli-0.1.50/vhcs/service/portal/site.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,39 +10,44 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import logging
-from .._util import hdc_service_client
+from vhcs.sglib.client_util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 log = logging.getLogger(__name__)
 _client = hdc_service_client("portal")
 
 
 def create(payload: dict):
     url = "/v2/sites"
     return _client.post(url, payload)
 
+
 def get(id: str, org_id: str):
     url = f"/v2/sites/{id}?org_id={org_id}"
     return _client.get(url)
 
+
 def list(**kwargs):
     url = with_query(f"/v2/sites", **kwargs)
     return _client.get(url)
 
+
 def delete(id: str, org_id: str):
     url = f"/v2/sites/{id}?org_id={org_id}"
     return _client.delete(url)
 
+
 def find_by_name(name: str, org_id: str):
     sites = list(org_id=org_id)
     for s in sites:
-        if s.get('name') == name:
+        if s.get("name") == name:
             return s
-    
+
+
 def set_edge(site_id: str, org_id: str, edge_deployment_id: str):
     url = f"/v1/sites/{site_id}/edge/{edge_deployment_id}"
-    return _client.put(url, {})
+    return _client.put(url, {})
```

### Comparing `hcs-cli-0.1.48/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.50/vhcs/service/vmhub/otp.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import base64
-from .._util import regional_service_client
+from vhcs.sglib.client_util import regional_service_client
 
 _region_name = None
 
 
 def use_region(region_name: str):
     global _region_name
     _region_name = region_name
@@ -39,8 +39,7 @@
 
 
 def redeem(resource_name: str, otp: str, csr: str):
     base64_encoded_csr = base64.b64encode(csr.encode("ascii")).decode("ascii")
 
     credentials_request = {"vmId": resource_name, "otp": otp, "clientCsr": base64_encoded_csr}
     return _client().post("/credentials", credentials_request)
-
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/cidr_util.py` & `hcs-cli-0.1.50/vhcs/support/daas/cidr_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 import ipaddress
 from typing import Tuple
 from ipaddress import ip_network
 
+
 def _formalize(cidrs: list[str]):
     def to_network(n):
         return ip_network(n)
+
     cidrs = map(to_network, cidrs)
     return list(ipaddress.collapse_addresses(cidrs))
 
+
 def _has_overlap(network, list_of_networks):
     for n in list_of_networks:
         if network.overlaps(n):
             return True
-        
+
+
 def _is_subnet(network, list_of_networks):
     for n in list_of_networks:
         if network.subnet_of(n):
             return True
-def find_available_cidr_24(total_cidrs: list[str], used_cidrs: list[str], configured_cidrs: list[str]):
-    
 
+
+def find_available_cidr_24(total_cidrs: list[str], used_cidrs: list[str], configured_cidrs: list[str]):
     total_cidrs = _formalize(total_cidrs)
     used_cidrs = _formalize(used_cidrs)
     configured_cidrs = _formalize(configured_cidrs)
 
     for t in configured_cidrs:
         for space in t.subnets(new_prefix=24):
             if not _is_subnet(space, total_cidrs):
                 continue
             if _has_overlap(space, used_cidrs):
                 continue
             return str(space)
-        
+
+
 def subnets_of(input: list[str], limit: list[str]) -> Tuple[bool, str]:
     input = _formalize(input)
     limit = _formalize(limit)
     for i in input:
         if not _is_subnet(i, limit):
             return False, str(i)
     return True, None
 
+
 def overlaps(a: list[str], b: list[str]) -> Tuple[bool, str]:
     a = _formalize(a)
     b = _formalize(b)
 
     for i in a:
         if _has_overlap(i, b):
             return True, i
-    return False, None
+    return False, None
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/helper.py` & `hcs-cli-0.1.50/vhcs/support/daas/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,91 +15,97 @@
 
 import logging
 import yaml
 from typing import Callable
 from vhcs.plan.provider.azure import _az_facade as az
 from vhcs.service import admin
 from . import template, infra
-from vhcs.common import util as data_util
-from vhcs.plan import PlanException
+from vhcs.ctxp import data_util as data_util
 
 log = logging.getLogger(__file__)
 
+
 def prep_az_cli(tenant_request):
-    provider = tenant_request['provider']
-    providerInstanceId = provider['providerInstanceId']
-    print('Provider:', providerInstanceId)
-    providerInstance = admin.provider.get('azure', providerInstanceId)
-    subscription_id = providerInstance['providerDetails']['data']['subscriptionId']
-    directory_id = providerInstance['providerDetails']['data']['directoryId']
-    application_id = providerInstance['providerDetails']['data']['applicationId']
-    region = providerInstance['providerDetails']['data']['region']
-    print('Subscription:', subscription_id)
-    print('Directory:', directory_id)
-    print('ApplicationId:', application_id)
-    print('Region:', region)
-    if application_id != provider['applicationId']:
+    provider = tenant_request["provider"]
+    providerInstanceId = provider["providerInstanceId"]
+    print("Provider:", providerInstanceId)
+    providerInstance = admin.provider.get("azure", providerInstanceId)
+    subscription_id = providerInstance["providerDetails"]["data"]["subscriptionId"]
+    directory_id = providerInstance["providerDetails"]["data"]["directoryId"]
+    application_id = providerInstance["providerDetails"]["data"]["applicationId"]
+    region = providerInstance["providerDetails"]["data"]["region"]
+    print("Subscription:", subscription_id)
+    print("Directory:", directory_id)
+    print("ApplicationId:", application_id)
+    print("Region:", region)
+    if application_id != provider["applicationId"]:
         log.warning("Configured application ID for CLI does not match application ID for provider.")
-    
-    az.login(provider['applicationId'], provider['applicationKey'], directory_id)
+
+    az.login(provider["applicationId"], provider["applicationKey"], directory_id)
     az.set_subscription(subscription_id)
 
+
 def prepare_plan_file(deployment_id: str, blueprint_id: str, fn_collect_info: Callable):
-    suffix = '.blueprint.yml'
+    suffix = ".blueprint.yml"
 
     if blueprint_id.endswith(suffix):
-        blueprint_id = blueprint_id[:-len(suffix)]
+        blueprint_id = blueprint_id[: -len(suffix)]
 
-    input_data = template.get(blueprint_id + '.vars.yml')
+    input_data = template.get(blueprint_id + ".vars.yml")
     file_name = _get_file_name(deployment_id)
 
     # Apply previous input, if any
     prev = data_util.load_data_file(file_name)
     if prev:
-        prev_vars = prev.get('vars')
+        prev_vars = prev.get("vars")
         if prev_vars:
-            data_util.deep_apply_defaults(input_data['vars'], prev_vars)
+            data_util.deep_apply_defaults(input_data["vars"], prev_vars)
 
     # Add defaults from shared infra config, if anything missing
     data_util.deep_apply_defaults(input_data, infra.get())
-    
+
     # Enforce key values
-    input_data['deploymentId'] = deployment_id
-    input_data['vars']['orgId'] = _get_org_id()
-    
+    input_data["deploymentId"] = deployment_id
+    input_data["vars"]["orgId"] = _get_org_id()
+
     def create_file(success):
         # Combine and save
-        blueprint_file = blueprint_id + '.blueprint.yml'
+        blueprint_file = blueprint_id + ".blueprint.yml"
         blueprint = template.get(blueprint_file)
-        text = "\n".join([
-            yaml.safe_dump(input_data, sort_keys=False),
-            "",
-            "# ----------------------------------",
-            "# Blueprint: " + blueprint_file,
-            "",
-            yaml.safe_dump(blueprint, sort_keys=False)
-        ])
+        text = "\n".join(
+            [
+                yaml.safe_dump(input_data, sort_keys=False),
+                "",
+                "# ----------------------------------",
+                "# Blueprint: " + blueprint_file,
+                "",
+                yaml.safe_dump(blueprint, sort_keys=False),
+            ]
+        )
         with open(file_name, "w") as file:
             file.write(text)
 
         if success:
             print("Plan saved as file: " + file_name)
             print(f"To view the plan:   'hcs plan graph -f {file_name}'")
             print(f"To deploy the plan: 'hcs plan deploy -f {file_name}'")
+
     success = False
     try:
         # Collect input from user
         fn_collect_info(input_data)
         success = True
     except Exception:
         raise
     finally:
         create_file(success)
 
 
 def _get_file_name(deployment_id: str) -> str:
-    return deployment_id + '.plan.yml'
+    return deployment_id + ".plan.yml"
+
 
 def _get_org_id():
-    from vhcs.common.sglib import auth
+    from vhcs.sglib import auth
+
     auth_info = auth.details(get_org_details=False)
     return auth_info.org.id
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/infra.py` & `hcs-cli-0.1.50/vhcs/support/daas/infra.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,47 +9,43 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.common.ctxp import context
+from vhcs.ctxp import context
 
 
 _config_name = "daas-infra"
 
+
 def get():
     return _get_config()
 
+
 def set(data: dict):
     return context.set(_config_name, data)
 
+
 def file():
     data = _get_config()
     context.set(_config_name, data)
     return context.file(_config_name)
 
+
 def _get_config():
     data = context.get(_config_name, default={})
     return _with_default(data, _config_template)
 
-def _with_default(target : dict, default : dict) -> dict:
+
+def _with_default(target: dict, default: dict) -> dict:
     ret = dict(default)
     ret.update(target)
     return ret
 
+
 _config_template = {
-	"provider": {
-		"id": ""
-	},
-	"network": {
-		"vNetId": "",
-		"tenantCIDRs": []
-	},
-	"desktop": {
-		"markerId": "",
-		"streamId": "",
-		"templateType": "",
-		"vmSkuName": ""
-	}
-}
+    "provider": {"id": ""},
+    "network": {"vNetId": "", "tenantCIDRs": []},
+    "desktop": {"markerId": "", "streamId": "", "templateType": "", "vmSkuName": ""},
+}
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/infra_green.py` & `hcs-cli-0.1.50/vhcs/support/daas/infra_green.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,116 +9,116 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import re
-import ipaddress
 import hashlib
 import logging
 from vhcs.service import admin
 from vhcs.plan.provider.azure import _az_facade as az
 from vhcs.plan import PlanException, context
 
 log = logging.getLogger(__name__)
 
+
 def process(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
-    provider = data['provider']
-    provider_id = provider['id']
+    org_id = data["orgId"]
+    provider = data["provider"]
+    provider_id = provider.get("id")
     if provider_id:
-        log.info('Reusing provider: %s', provider_id)
-        providerInstance = admin.provider.get('azure', provider_id, org_id)
+        log.info("Reusing provider: %s", provider_id)
+        providerInstance = admin.provider.get("azure", provider_id, org_id)
         if not providerInstance:
             raise PlanException("Provider not found: " + provider_id)
     else:
-        provider_id = state['output']['myProvider']['id']
+        provider_id = state["output"]["myProvider"]["id"]
 
     # identify subnets
     # subnet_map = _prepare_subnet_map(data['network']['vNetId'])
 
     # edge = {
     #     'managementNetwork': subnet_map[data['network']['managementNetworkName']]
     # }
     # uag = {
     #     'managementNetwork': subnet_map[data['network']['managementNetworkName']],
     #     'dmzNetwork': subnet_map[data['network']['dmzNetworkName']],
     #     'desktopNetwork': subnet_map[data['network']['desktopNetworkName']],
     # }
     image = {
-        'desktopPassword': [c for c in data['desktop']['adminPassword']],
-        'multiSessionImageName': _generate_image_name('m'),
-        'desktopImageName': _generate_image_name('d'),
+        "desktopPassword": [c for c in data["desktop"]["adminPassword"]],
+        "multiSessionImageName": _generate_image_name("m"),
+        "desktopImageName": _generate_image_name("d"),
     }
 
-    #https://confluence.eng.vmware.com/display/HCS/Titan+Lite+-+BOM#TitanLiteBOM-AddressSpaces
-    vnet_cidr = data['network']['cidr']
+    # https://confluence.eng.vmware.com/display/HCS/Titan+Lite+-+BOM#TitanLiteBOM-AddressSpaces
+    vnet_cidr = data["network"]["cidr"]
     if not vnet_cidr.endswith(".0/16"):
         raise Exception("The vNet CIDR must be /16")
-    prefix = vnet_cidr[:vnet_cidr.rindex('.')]
-    cidr_dmz = prefix + '.0/27'
-    cidr_mgmt = prefix + '.64/26'
-    cidr_shared_desktops = prefix + '.128/27'
+    prefix = vnet_cidr[: vnet_cidr.rindex(".")]
+    cidr_dmz = prefix + ".0/27"
+    cidr_mgmt = prefix + ".64/26"
+    cidr_shared_desktops = prefix + ".128/27"
     cidr = {
-        'dmz': cidr_dmz,
-        'mgmt': cidr_mgmt,
-        'sharedDesktops': cidr_shared_desktops,
-    }
-    return {
-        'providerInstanceId': provider_id,
-        'image': image,
-        'cidr': cidr
+        "dmz": cidr_dmz,
+        "mgmt": cidr_mgmt,
+        "sharedDesktops": cidr_shared_desktops,
     }
+    return {"providerInstanceId": provider_id, "image": image, "cidr": cidr}
+
 
 # def _prepare_subnet_map(vnet_id):
 #     #/subscriptions/a2ef2de8-f2b5-43da-bf68-2b182dd5f928/resourceGroups/horizonv2-sg-dev/providers/Microsoft.Network/virtualNetworks/westus2-vnet-1
 #     pattern = r'/subscriptions/.+?/resourceGroups/(.+?)/providers/Microsoft.Network/virtualNetworks/(.+)'
 #     matcher = re.search(pattern, vnet_id)
 #     if not matcher:
 #         raise PlanException("Fail parsing vNet ID: " + vnet_id)
 #     rg = matcher.group(1)
 #     vnet_name = matcher.group(2)
 #     subnets = az.network.subnet.list(rg, vnet_name)
-    
+
 #     ret = {}
 #     for subnet in subnets:
 #         subnet_name = subnet['name']
 #         cidr = subnet['addressPrefix']
 #         addrs = ipaddress.ip_network(cidr).num_addresses - 4
 #         ret[subnet_name] = _to_network(vnet_id, subnet_name, addrs, cidr)
 #     return ret
-        
+
 # def _to_network(vnet_id, subnet_name, available_ip_addresses, cidr):
 #     return {
 #         'kind': 'subnets',
 #         'id': f'{vnet_id}/subnets/{subnet_name}',
 #         'data': {
 #             'parent': vnet_id,
 #             'name': subnet_name,
 #             'availableIpAddresses': available_ip_addresses,
 #             'cidr': cidr
 #         }
 #     }
 
+
 def _generate_image_name(prefix: str) -> str:
-    ret = prefix + "-" + context.get('deploymentId')
+    ret = prefix + "-" + context.get("deploymentId")
     # 11 chars max
     return _to_limited_string(ret, 11)
 
+
 def _to_limited_string(text: str, limit: int) -> str:
     l = len(text)
     if l <= limit:
         return text
-    first_part = text[:limit - 4]
-    second_part = text[limit - 4:]
+    first_part = text[: limit - 4]
+    second_part = text[limit - 4 :]
 
     sha256_hash = hashlib.sha256(second_part.encode()).hexdigest()
     truncated_hash = sha256_hash[:3]
-    return first_part + '-' + truncated_hash
+    return first_part + "-" + truncated_hash
 
-def destroy(data: dict, pstaterev: dict):
+
+def destroy(data: dict, state: dict, force: bool):
     return
 
+
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/infra_reuse.py` & `hcs-cli-0.1.50/vhcs/support/daas/infra_reuse.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,100 +19,100 @@
 import logging
 from vhcs.service import admin
 from vhcs.plan.provider.azure import _az_facade as az
 from vhcs.plan import PlanException, context
 
 log = logging.getLogger(__name__)
 
+
 def process(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
-    provider = data['provider']
-    provider_id = provider['id']
+    org_id = data["orgId"]
+    provider = data["provider"]
+    provider_id = provider["id"]
     if provider_id:
-        log.info('Reusing provider: %s', provider_id)
-        providerInstance = admin.provider.get('azure', provider_id, org_id)
+        log.info("Reusing provider: %s", provider_id)
+        providerInstance = admin.provider.get("azure", provider_id, org_id)
         if providerInstance:
-            providerData = providerInstance['providerDetails']['data']
-            region = providerData['region']
+            providerData = providerInstance["providerDetails"]["data"]
+            region = providerData["region"]
         else:
             raise PlanException("Provider not found: " + provider_id)
     else:
-        region = data['newProvider']['region']
-        provider_id = state['output']['myProvider']['id']
+        region = data["newProvider"]["region"]
+        provider_id = state["output"]["myProvider"]["id"]
 
     # identify subnets
-    subnet_map = _prepare_subnet_map(data['network']['vNetId'])
+    subnet_map = _prepare_subnet_map(data["network"]["vNetId"])
 
-    edge = {
-        'managementNetwork': subnet_map[data['network']['managementNetworkName']]
-    }
+    edge = {"managementNetwork": subnet_map[data["network"]["managementNetworkName"]]}
     uag = {
-        'managementNetwork': subnet_map[data['network']['managementNetworkName']],
-        'dmzNetwork': subnet_map[data['network']['dmzNetworkName']],
-        'desktopNetwork': subnet_map[data['network']['desktopNetworkName']],
+        "managementNetwork": subnet_map[data["network"]["managementNetworkName"]],
+        "dmzNetwork": subnet_map[data["network"]["dmzNetworkName"]],
+        "desktopNetwork": subnet_map[data["network"]["desktopNetworkName"]],
     }
     image = {
-        'desktopSubnetId': uag['desktopNetwork']['id'],
-        'desktopPassword': [c for c in data['desktop']['adminPassword']],
-        'multiSessionImageName': _generate_image_name('m'),
-        'desktopImageName': _generate_image_name('d'),
+        "desktopSubnetId": uag["desktopNetwork"]["id"],
+        "desktopPassword": [c for c in data["desktop"]["adminPassword"]],
+        "multiSessionImageName": _generate_image_name("m"),
+        "desktopImageName": _generate_image_name("d"),
     }
-    
+
     return {
-        'location': region,
-        'providerInstanceId': provider_id,
-        'edge': edge,
-        'uag': uag,
-        'image': image,
+        "location": region,
+        "providerInstanceId": provider_id,
+        "edge": edge,
+        "uag": uag,
+        "image": image,
     }
 
+
 def _prepare_subnet_map(vnet_id):
-    #/subscriptions/a2ef2de8-f2b5-43da-bf68-2b182dd5f928/resourceGroups/horizonv2-sg-dev/providers/Microsoft.Network/virtualNetworks/westus2-vnet-1
-    pattern = r'/subscriptions/.+?/resourceGroups/(.+?)/providers/Microsoft.Network/virtualNetworks/(.+)'
+    # /subscriptions/a2ef2de8-f2b5-43da-bf68-2b182dd5f928/resourceGroups/horizonv2-sg-dev/providers/Microsoft.Network/virtualNetworks/westus2-vnet-1
+    pattern = r"/subscriptions/.+?/resourceGroups/(.+?)/providers/Microsoft.Network/virtualNetworks/(.+)"
     matcher = re.search(pattern, vnet_id)
     if not matcher:
         raise PlanException("Fail parsing vNet ID: " + vnet_id)
     rg = matcher.group(1)
     vnet_name = matcher.group(2)
     subnets = az.network.subnet.list(rg, vnet_name)
-    
+
     ret = {}
     for subnet in subnets:
-        subnet_name = subnet['name']
-        cidr = subnet['addressPrefix']
+        subnet_name = subnet["name"]
+        cidr = subnet["addressPrefix"]
         addrs = ipaddress.ip_network(cidr).num_addresses - 4
         ret[subnet_name] = _to_network(vnet_id, subnet_name, addrs, cidr)
     return ret
-        
+
+
 def _to_network(vnet_id, subnet_name, available_ip_addresses, cidr):
     return {
-        'kind': 'subnets',
-        'id': f'{vnet_id}/subnets/{subnet_name}',
-        'data': {
-            'parent': vnet_id,
-            'name': subnet_name,
-            'availableIpAddresses': available_ip_addresses,
-            'cidr': cidr
-        }
+        "kind": "subnets",
+        "id": f"{vnet_id}/subnets/{subnet_name}",
+        "data": {"parent": vnet_id, "name": subnet_name, "availableIpAddresses": available_ip_addresses, "cidr": cidr},
     }
 
+
 def _generate_image_name(prefix: str) -> str:
-    ret = prefix + "-" + context.get('deploymentId')
+    ret = prefix + "-" + context.get("deploymentId")
     # 11 chars max
     return _to_limited_string(ret, 11)
 
+
 def _to_limited_string(text: str, limit: int) -> str:
     l = len(text)
     if l <= limit:
         return text
-    first_part = text[:limit - 4]
-    second_part = text[limit - 4:]
+    first_part = text[: limit - 4]
+    second_part = text[limit - 4 :]
 
     sha256_hash = hashlib.sha256(second_part.encode()).hexdigest()
     truncated_hash = sha256_hash[:3]
-    return first_part + '-' + truncated_hash
+    return first_part + "-" + truncated_hash
 
-def destroy(data: dict, pstaterev: dict):
+
+def destroy(data: dict, state: dict, force: bool):
     return
 
+
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-green.blueprint.yml` & `hcs-cli-0.1.50/vhcs/support/daas/templates/v1/infra-green.blueprint.yml`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,18 @@
     kind: azure/subnet
     data:
       name: ${defaults.networkNames.dmz}
       resourceGroup: ${infraRG.name}
       vNetName: ${infraVNet.name}
       parameters:
         address_prefix: ${myRuntime.cidr.dmz}
-        network_security_group:
-          id: ${nsgDMZ.id}
+        # network_security_group:
+        #   id: ${nsgDMZ.id}
+    after:
+    - nsgDMZ
   nsgMgmt:
     kind: azure/nsg
     data:
       name: ${defaults.name}-nsg-${defaults.networkNames.mgmt}
       resourceGroup: ${infraRG.name}
       parameters:
         location: ${vars.region}
@@ -111,20 +113,21 @@
     kind: azure/subnet
     data:
       name: ${defaults.networkNames.mgmt}
       resourceGroup: ${infraRG.name}
       vNetName: ${infraVNet.name}
       parameters:
         address_prefix: ${myRuntime.cidr.mgmt}
-        network_security_group:
-          id: ${nsgMgmt.id}
+        # network_security_group:
+        #   id: ${nsgMgmt.id}
         nat_gateway:
           id: ${vnetNAT.id}
     after:
     - subnetDMZ
+    - nsgMgmt
   nsgSharedDesktops:
     kind: azure/nsg
     data:
       name: ${defaults.name}-nsg-${defaults.networkNames.sharedDesktops}
       resourceGroup: ${infraRG.name}
       parameters:
         location: ${vars.region}
@@ -133,18 +136,19 @@
     kind: azure/subnet
     data:
       name: ${defaults.networkNames.sharedDesktops}
       resourceGroup: ${infraRG.name}
       vNetName: ${infraVNet.name}
       parameters:
         address_prefix: ${myRuntime.cidr.sharedDesktops}
-        network_security_group:
-          id: ${nsgSharedDesktops.id}
+        # network_security_group:
+        #   id: ${nsgSharedDesktops.id}
     after:
     - subnetMgmt
+    - nsgSharedDesktops
   myEdge:
     kind: hcs/edge
     after:
     - vnetNAT
     data:
       orgId: ${vars.orgId}
       name: ${defaults.name}
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml` & `hcs-cli-0.1.50/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-reuse.vars.yml` & `hcs-cli-0.1.50/vhcs/support/daas/templates/v1/infra-reuse.vars.yml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.50/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files 13% similar despite different names*

```diff
@@ -6,104 +6,116 @@
     deployment: ${deploymentId}
     managed-by: titan-lite
 
 # The providers section specifies provider-specific data. Normally this required to initialize
 # a provider.
 providers:
   azure:
-    data: ${tenantCalc.provider}
+    data: ${tenantPrep.provider}
 
 runtimes:
-  tenantCalc:
-    impl: vhcs.support.daas.tenant_calc # Custom calculation of values
+  tenantPrep:
+    impl: vhcs.support.daas.tenant_prep # Custom calculation of values
     data: ${vars} # Take the entire unchanged vars as input
 
+  tenantSummary:
+    impl: vhcs.support.daas.tenant_summary # Custom calculation of values
+    data:
+      orgId: ${vars.orgId}
+      edgeId: ${vars.edgeId}
+      users: ${myAADUser}
+      entitlementId: ${myPoolGroup.name}
+      domainName: ${tenantPrep.orgIdpMap.idpTenantDomain}
+      stackUrl: ${profile.hcs.url}
+    after:
+    - myEntitlement
+
 resources:
   myRg:
     kind: azure/resource-group
     data:
       name: ${defaults.name}
       parameters:
         name: ${defaults.name}
-        location: ${tenantCalc.location}
+        location: ${tenantPrep.location}
         tags: ${defaults.tags}
 
-  myNsg:
-    kind: azure/nsg
-    data:
-      name: ${defaults.name}
-      resourceGroup: ${tenantCalc.vNet.resourceGroup}
-      parameters:
-        location: ${tenantCalc.location}
-        tags: ${defaults.tags}
+  # myNsg:
+  #   kind: azure/nsg
+  #   data:
+  #     name: ${defaults.name}
+  #     resourceGroup: ${tenantPrep.vNet.resourceGroup}
+  #     parameters:
+  #       location: ${tenantPrep.location}
+  #       tags: ${defaults.tags}
 
   mySubnet:
     kind: azure/subnet
     data:
       name: ${defaults.name}
-      resourceGroup: ${tenantCalc.vNet.resourceGroup}
-      vNetName: ${tenantCalc.vNet.name}
+      resourceGroup: ${tenantPrep.vNet.resourceGroup}
+      vNetName: ${tenantPrep.vNet.name}
       parameters:
-        address_prefix: ${tenantCalc.cidr}
-        network_security_group:
-          id: ${myNsg.id}
+        address_prefix: ${tenantPrep.cidr}
+        # network_security_group:
+        #   id: ${myNsg.id}
 
   myAADGroup:
     kind: azure/aad-group
     data:
       displayName: ${defaults.name}
       mailNickname: ${defaults.name}
       description:
       parentGroup: ${vars.desktop.userGroup}
   
   myAADUser:
     kind: azure/aad-user
     for: email in vars.userEmails
     data:
       group: ${myAADGroup.id}
-      domainName: ${tenantCalc.orgIdpMap.domains[0]}
+      domainName: ${tenantPrep.orgIdpMap.domains[0]}
 
   myTemplate:
     kind: hcs/pool-template
     data:
-      providerInstanceId: ${tenantCalc.provider.id}
-      uagDeploymentId: ${tenantCalc.template.uag_deployment_id}
-      edgeDeploymentId: ${tenantCalc.template.edge_deployment_id}
+      providerInstanceId: ${tenantPrep.provider.id}
+      uagDeploymentId: ${tenantPrep.template.uag_deployment_id}
+      edgeDeploymentId: ${tenantPrep.template.edge_deployment_id}
       orgId: ${vars.orgId}
       name: ${defaults.name}
-      vmNamePattern: d-
+      vmNamePattern: tl-${deploymentId}-
       templateType: ${vars.desktop.templateType}
       applicationProperties:
         azureActiveDirectoryJoined: 'true'
       networks:
       - kind: subnets
         id: ${mySubnet.id}
         data:
           parent: ${mySubnet.id}
           name: ${mySubnet.name}
           availableIpAddresses: 250
-          cidr: ${tenantCalc.cidr}
+          cidr: ${tenantPrep.cidr}
       imageReference:
         streamId: ${vars.desktop.streamId}
         markerId: ${vars.desktop.markerId}
       licenseProvided: true
       desktopAdminUsername: hcs-admin
-      desktopAdminPassword: ${tenantCalc.template.password}
+      desktopAdminPassword: ${tenantPrep.template.password}
       diskEncryption:
         enabled: false
       sparePolicy:
-        limit: ${tenantCalc.template.total_vms}
-        max: ${tenantCalc.template.total_vms}
-        min: ${tenantCalc.template.total_vms}
-      sessionsPerVm: ${tenantCalc.number_of_users}
+        limit: ${tenantPrep.template.total_vms}
+        max: ${tenantPrep.template.total_vms}
+        min: ${tenantPrep.template.total_vms}
+      sessionsPerVm: ${tenantPrep.template.sessions_per_vm}
       vmLicenseType: WINDOWS_CLIENT
       diskSizeInGB: 127
       infrastructure:
         vmSkus:
-        - ${tenantCalc.template.vm_sku}
+        - ${tenantPrep.template.vm_sku}
 
   myPoolGroup:
     kind: hcs/pool-group
     data:
       orgId: ${vars.orgId}
       name: ${defaults.name}
       type: DESKTOP
@@ -124,16 +136,7 @@
       orgId: ${vars.orgId}
       poolIds:
       - ${myPoolGroup.id}
       resourceDetails:
       - poolId: ${myPoolGroup.id}
       userIds: "${[for u in myAADUser: u.id]}"
 
-  myLaunchItem:
-    kind: hcs/launch-item
-    data:
-      users: ${myAADUser}
-      entitlementId: ${myPoolGroup.name}
-      domainName: ${tenantCalc.orgIdpMap.idpTenantDomain}
-      stackUrl: ${profile.hcs.url}
-    after:
-    - myEntitlement
```

### Comparing `hcs-cli-0.1.48/vhcs/support/daas/tenant_calc.py` & `hcs-cli-0.1.50/vhcs/support/daas/tenant_prep.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,106 +16,118 @@
 from vhcs.service import admin, auth
 from vhcs.plan.provider.azure import _az_facade as az
 from vhcs.plan import PluginException
 from .cidr_util import find_available_cidr_24
 
 log = logging.getLogger(__name__)
 
+
 def process(data: dict, state: dict) -> dict:
     import time
+
     time.sleep(10)
-    org_id = data['orgId']
-    edge = admin.edge.get(data['edgeId'], org_id)
-    provider_id = edge['providerInstanceId']
+    org_id = data["orgId"]
+    edge = admin.edge.get(data["edgeId"], org_id)
+    provider_id = edge["providerInstanceId"]
     # log.info('Provider: %s', provider_id)
-    provider = admin.provider.get('azure', provider_id, org_id)
+    provider = admin.provider.get("azure", provider_id, org_id)
     if not provider:
-        raise PluginException('Provider not found: ' + provider_id)
-    providerData = provider['providerDetails']['data']
-    subscription_id = providerData['subscriptionId']
+        raise PluginException("Provider not found: " + provider_id)
+    providerData = provider["providerDetails"]["data"]
+    subscription_id = providerData["subscriptionId"]
     # directory_id = providerData['directoryId']
     # application_id = providerData['applicationId']
-    region = providerData['region']
+    region = providerData["region"]
     # log.info('Subscription: %s', subscription_id)
     # log.info('Directory: %s', directory_id)
     # log.info('ApplicationId: %s', application_id)
     # log.info('Region: %s', region)
 
-    template_type = data['desktop']['templateType']
-    number_of_users = len(data['userEmails'])
+    template_type = data["desktop"]["templateType"]
+    number_of_users = len(data["userEmails"])
     is_multi_session = "MULTI_SESSION" == template_type
 
-    uag_deployments = admin.helper.list_resources_by_provider('uag-deployments', provider_id, limit=1)
+    uag_deployments = admin.helper.list_resources_by_provider("uag-deployments", provider_id, limit=1)
     if not uag_deployments:
         raise Exception("No UAG deployment found.")
-    uag_deployment_id = uag_deployments[0]['id']
+    uag_deployment_id = uag_deployments[0]["id"]
 
-    edge_deployments = admin.helper.list_resources_by_provider('edge-deployments', provider_id, limit=1)
+    edge_deployments = admin.helper.list_resources_by_provider("edge-deployments", provider_id, limit=1)
     if not edge_deployments:
         raise Exception("No UAG deployment found.")
-    edge_deployment_id = edge_deployments[0]['id']
+    edge_deployment_id = edge_deployments[0]["id"]
 
     search = f"name $eq {data['desktop']['vmSkuName']}"
     vm_skus = admin.azure_infra.get_compute_vm_skus(provider_instance_id=provider_id, search=search, limit=1)
     if not vm_skus:
         raise Exception("No VM SKUs found.")
 
+    if is_multi_session:
+        sessions_per_vm = 10
+        total_vms = int((number_of_users + sessions_per_vm - 1) / sessions_per_vm)
+    else:
+        sessions_per_vm = 1
+        total_vms = number_of_users
     template = {
-        'total_vms': 1 if is_multi_session else number_of_users,
-        'password': _generate_password(),
-        'uag_deployment_id': uag_deployment_id,
-        'edge_deployment_id': edge_deployment_id,
-        'vm_sku': vm_skus[0]
+        "total_vms": total_vms,
+        "sessions_per_vm": sessions_per_vm,
+        "password": _generate_password(),
+        "uag_deployment_id": uag_deployment_id,
+        "edge_deployment_id": edge_deployment_id,
+        "vm_sku": vm_skus[0],
     }
 
     org_idp_map = auth.admin.get_org_idp_map()
-    vnet = az.network.vnet.get(edge['infrastructure']['managementNetwork']['data']['parent'])
+    vnet = az.network.vnet.get(edge["infrastructure"]["managementNetwork"]["data"]["parent"])
     cidr = _calculate_cidr(vnet)
-    log.info('Calculated network address: %s', cidr)
+    log.info("Calculated network address: %s", cidr)
     return {
-        'location': region,
-        'cidr': cidr,
-        'vNet': vnet,
-        'provider': {
-            'id': provider_id,
-            'subscriptionId': subscription_id
-        },
-        'template': template,
-        'number_of_users': number_of_users,
-        'orgIdpMap': org_idp_map
+        "location": region,
+        "cidr": cidr,
+        "vNet": vnet,
+        "provider": {"id": provider_id, "subscriptionId": subscription_id},
+        "template": template,
+        "orgIdpMap": org_idp_map,
     }
 
+
 def _generate_password():
     from random import choice
+
     upper_chars = "ABCDEFGHJKLMNPQRSTUVWXY"
     readable_chars = "abcdefghjklmnpqrstuvwxy3456789"
     special_chars = "!@#$%_"
-    return '' + choice(upper_chars) + ''.join(choice(readable_chars) for i in range(12)) + choice(special_chars)
+    return "" + choice(upper_chars) + "".join(choice(readable_chars) for i in range(12)) + choice(special_chars)
+
 
 def _calculate_cidr(vnet):
-    vnet_cidrs = vnet['addressSpace']['addressPrefixes']
+    vnet_cidrs = vnet["addressSpace"]["addressPrefixes"]
     used_cidrs = []
-    for subnet in vnet['subnets']:
-        used_cidrs.append(subnet['addressPrefix'])
+    for subnet in vnet["subnets"]:
+        used_cidrs.append(subnet["addressPrefix"])
     # https://confluence.eng.vmware.com/display/HCS/Titan+Lite+-+BOM#TitanLiteBOM-AddressSpaces
     infra_cidr = None
     for c in vnet_cidrs:
         if not c.endswith(".0/16"):
             continue
         infra_cidr = c
         break
     if not infra_cidr:
         raise PluginException("No /16 CIDR found in vNet.")
-    
-    prefix = infra_cidr[:infra_cidr.rindex('.')]
-    reserved_cidr = prefix + '.0/24'
+
+    prefix = infra_cidr[: infra_cidr.rindex(".")]
+    reserved_cidr = prefix + ".0/24"
     used_cidrs.append(reserved_cidr)
     tenant_cidr = find_available_cidr_24(vnet_cidrs, used_cidrs, [infra_cidr])
     if not tenant_cidr:
-        raise PluginException("Unable to find usable subnet address space for the tenant. Consider adding new address space to the config via 'hcs daas infra plan', and/or add new spaces in vnet.")
+        raise PluginException(
+            "Unable to find usable subnet address space for the tenant. Consider adding new address space to the config via 'hcs daas infra plan', and/or add new spaces in vnet."
+        )
     return tenant_cidr
 
-def destroy(data: dict, state: dict):
+
+def destroy(data: dict, state: dict, force: bool):
     return
 
+
 def eta(action: str, data: dict, state: dict):
-    return '1m'
+    return "1m"
```

### Comparing `hcs-cli-0.1.48/vhcs/support/profile.py` & `hcs-cli-0.1.50/vhcs/support/profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,73 +9,78 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.common import util
-from vhcs.common.ctxp import config, profile, CtxpException
+from vhcs.ctxp import data_util
+from vhcs.ctxp import config, profile, CtxpException
 
 _hcs_envs = config.get("hcs-deployments.yaml")
 
+
 def _is_production_env(hdc_url: str) -> bool:
     for env in _hcs_envs["prod"]:
         if env.hdc.url == hdc_url:
             return True
 
 
 def _get_csp_url(hdc_url: str) -> str:
     if _is_production_env(hdc_url):
         return "https://console.cloud.vmware.com"
     return "https://console-stg.cloud.vmware.com"
 
 
 def ensure_default_production_profile():
     doc = get_default_profile_template()
-    _ensure_profile('default', doc, interactive=False)
+    _ensure_profile("default", doc, interactive=False)
+
 
 def get_default_profile_template():
-    stack_name = 'prod-na-cp102'
+    stack_name = "prod-na-cp102"
     for stack in _hcs_envs["prod"]:
         if stack.env == stack_name:
             return _profile_data_from_stack(stack)
-    raise CtxpException('Production configuration not found: ' + stack_name)
+    raise CtxpException("Production configuration not found: " + stack_name)
+
 
 def _profile_data_from_stack(stack):
     return {
         "hcs": {"url": stack.hdc.url, "regions": stack.regions},
         "csp": {
-            "url": _get_csp_url(stack.hdc.url), 
+            "url": _get_csp_url(stack.hdc.url),
             "orgId": None,
             "apiToken": None,
-            "clientId": None, 
-            "clientSecret": None
+            "clientId": None,
+            "clientSecret": None,
         },
     }
 
-def _ensure_profile(name, data, interactive:bool=True):
+
+def _ensure_profile(name, data, interactive: bool = True):
     existing = profile.get(name)
     if existing:
-        if util.deep_apply_defaults(existing, data):
+        if data_util.deep_apply_defaults(existing, data):
             profile.save(name, existing)
             if interactive:
-                print('Profile created: ' + name)
+                print("Profile created: " + name)
         else:
             if interactive:
-                print('Profile unchanged: ' + name)
+                print("Profile unchanged: " + name)
     else:
         profile.create(name, data, False)
         if interactive:
-            print('Profile created: ' + name)
+            print("Profile created: " + name)
+
 
 def ensure_dev_profiles():
     items = []
     items += _hcs_envs["prod"]
     items += _hcs_envs["staging"]
     items += _hcs_envs["dev"]
 
     for stack in items:
         name = stack.alias or stack.env
         doc = _profile_data_from_stack(stack)
         _ensure_profile(name, doc)
-    _ensure_profile('nightly', profile.get('integration'))
+    _ensure_profile("nightly", profile.get("integration"))
```

### Comparing `hcs-cli-0.1.48/vhcs/util/check_license.py` & `hcs-cli-0.1.50/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/util/duration.py` & `hcs-cli-0.1.50/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/util/pki_util.py` & `hcs-cli-0.1.50/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.48/vhcs/util/query_util.py` & `hcs-cli-0.1.50/vhcs/util/query_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,43 +25,42 @@
             del obj[k]
     return obj
 
 
 def with_query(url: str, **kwargs: Any) -> str:
     qs = urlencode(_remove_none(dict(kwargs)))
     if qs:
-        if url.find('?') < 0:
-            url += '?'
+        if url.find("?") < 0:
+            url += "?"
         url += qs
     return url
 
 
 class PageRequest:
     def __init__(self, fn_get_page: Callable, **kwargs):
-        limit = kwargs.get('limit')
+        limit = kwargs.get("limit")
         self.limit = int(limit) if limit else 10
         self.fn_get_page = fn_get_page
         self.query = _remove_none(dict(kwargs))
         if int(self.query.get("size", 0)) < 1:
-            self.query['size'] = 20
-        
+            self.query["size"] = 20
 
     def get(self) -> list:
         ret = []
         page_index = 0
 
         while True:
             self.query["page"] = page_index
-            
+
             query_string = urlencode(self.query)
             page = self.fn_get_page(query_string)
             if not page or not page.content:
                 break
             ret += page.content
             if len(ret) > self.limit:
-                ret = ret[:self.limit]
+                ret = ret[: self.limit]
                 break
-            if len(page.content) < self.query['size']:
+            if len(page.content) < self.query["size"]:
                 break
             page_index += 1
 
         return ret
```

### Comparing `hcs-cli-0.1.48/vhcs/util/versions.py` & `hcs-cli-0.1.50/vhcs/util/versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import logging
 import httpx
 import time
-import vhcs.common.ctxp as ctxp
+import vhcs.ctxp as ctxp
 
 import pkg_resources
 from packaging.version import Version
 
 log = logging.getLogger(__name__)
```

