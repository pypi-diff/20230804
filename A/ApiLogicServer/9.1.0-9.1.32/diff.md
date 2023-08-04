# Comparing `tmp/ApiLogicServer-9.1.0.tar.gz` & `tmp/ApiLogicServer-9.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApiLogicServer-9.1.0.tar", last modified: Tue Jul  4 23:54:48 2023, max compression
+gzip compressed data, was "ApiLogicServer-9.1.32.tar", last modified: Fri Aug  4 15:21:07 2023, max compression
```

## Comparing `ApiLogicServer-9.1.0.tar` & `ApiLogicServer-9.1.32.tar`

### file list

```diff
@@ -1,668 +1,695 @@
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.813248 ApiLogicServer-9.1.0/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.620566 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/
--rw-r--r--   0 val        (502) staff       (20)    15093 2023-07-04 23:54:48.000000 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    48386 2023-07-04 23:54:48.000000 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/SOURCES.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-07-04 23:54:48.000000 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/dependency_links.txt
--rw-r--r--   0 val        (502) staff       (20)       66 2023-07-04 23:54:48.000000 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/entry_points.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-07-04 23:54:48.000000 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/not-zip-safe
--rw-r--r--   0 val        (502) staff       (20)      662 2023-07-04 23:54:48.000000 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/requires.txt
--rw-r--r--   0 val        (502) staff       (20)       21 2023-07-04 23:54:48.000000 ApiLogicServer-9.1.0/ApiLogicServer.egg-info/top_level.txt
--rw-r--r--   0 val        (502) staff       (20)     1485 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/LICENSE
--rw-r--r--   0 val        (502) staff       (20)      804 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/MANIFEST.in
--rw-r--r--   0 val        (502) staff       (20)    15093 2023-07-04 23:54:48.813059 ApiLogicServer-9.1.0/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    14087 2023-07-04 21:58:20.000000 ApiLogicServer-9.1.0/README.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.621985 ApiLogicServer-9.1.0/api_logic_server_cli/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    62350 2023-07-04 22:12:02.000000 ApiLogicServer-9.1.0/api_logic_server_cli/api_logic_server.py
--rw-r--r--   0 val        (502) staff       (20)      133 2023-07-04 23:39:59.000000 ApiLogicServer-9.1.0/api_logic_server_cli/api_logic_server_info.yaml
--rw-r--r--   0 val        (502) staff       (20)    35169 2023-06-24 17:51:10.000000 ApiLogicServer-9.1.0/api_logic_server_cli/cli.py
--rw-r--r--   0 val        (502) staff       (20)     1887 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/cli_args_base.py
--rw-r--r--   0 val        (502) staff       (20)     3303 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/cli_args_project.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.623306 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.626373 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      235 2023-06-23 14:12:03.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     5355 2023-06-23 14:12:05.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    14572 2023-07-04 14:10:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    35464 2023-06-23 14:12:03.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    37429 2023-06-23 14:12:05.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2676 2023-07-04 14:10:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     5301 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
--rw-r--r--   0 val        (502) staff       (20)    12877 2023-07-03 17:44:56.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py
--rw-r--r--   0 val        (502) staff       (20)    34482 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/model_creation_services.py
--rw-r--r--   0 val        (502) staff       (20)     6127 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.630625 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
--rwxr-xr-x   0 val        (502) staff       (20)    15430 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.630930 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
--rwxr-xr-x   0 val        (502) staff       (20)  1145966 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
--rwxr-xr-x   0 val        (502) staff       (20)     3870 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
--rwxr-xr-x   0 val        (502) staff       (20)      692 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
--rwxr-xr-x   0 val        (502) staff       (20)     5347 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
--rwxr-xr-x   0 val        (502) staff       (20)     9664 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
--rwxr-xr-x   0 val        (502) staff       (20)      492 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
--rwxr-xr-x   0 val        (502) staff       (20)       67 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.612031 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.633742 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
--rwxr-xr-x   0 val        (502) staff       (20)    86781 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
--rwxr-xr-x   0 val        (502) staff       (20)   166928 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
--rwxr-xr-x   0 val        (502) staff       (20)      211 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
--rwxr-xr-x   0 val        (502) staff       (20)      516 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.731611 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
--rwxr-xr-x   0 val        (502) staff       (20)     1576 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     3197 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     9011 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    21905 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2921 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     7103 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     1004 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     2792 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     7546 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    17381 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    33520 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    71153 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    14043 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    36857 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5595 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    14138 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     6135 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    14288 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2280 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     5953 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3747 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8068 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4407 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    10552 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2156 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     5783 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    11957 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    24504 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5499 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    13356 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4187 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    10856 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     7001 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    17447 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3591 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8746 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3747 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     9475 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3140 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     7634 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4056 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     9168 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     8184 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    18882 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4068 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     9104 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    14317 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    32894 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3963 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     9547 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3152 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8052 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     8662 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    20172 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4982 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    13442 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     6569 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    15183 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2002 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     4736 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2974 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     7499 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     1967 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     5172 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5948 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    13558 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    10454 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    23458 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     1255 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     3229 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4128 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    10303 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    17096 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    31009 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     7760 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    18142 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     9800 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    21207 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3420 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8828 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3820 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    10430 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    41393 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)   145206 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5605 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    13185 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     8412 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    19971 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     9916 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    22155 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     6545 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    16602 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4681 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    11819 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3545 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8963 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3710 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     9146 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     1924 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     4864 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5069 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    11830 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3092 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8217 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2417 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     6013 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     7472 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    16988 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2342 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     6267 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)  3310604 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      576 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20) 10838575 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    35620 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)   121512 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    17547 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    39845 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2594 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     6567 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2814 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     7255 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    18754 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    38065 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2736 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     7008 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2693 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     6865 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3378 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8159 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2709 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     6645 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4619 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    10592 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4203 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    10608 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2559 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     6522 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5926 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    96741 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     1840 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     5116 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     8013 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    19497 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3725 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     9025 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3288 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8254 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2026 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     5528 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    13558 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    26650 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     9201 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    21765 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5069 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    11826 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    34921 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)   119930 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4669 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    10814 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     4316 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    10868 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)    11414 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    24817 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     2622 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)     7016 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     5259 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)    13615 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     7391 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)    17258 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     1986 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     4960 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)     3230 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
--rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)     8177 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
--rwxr-xr-x   0 val        (502) staff       (20)  1384276 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
--rwxr-xr-x   0 val        (502) staff       (20)     3014 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
--rwxr-xr-x   0 val        (502) staff       (20)  5552838 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.736029 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
--rwxr-xr-x   0 val        (502) staff       (20)    72504 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.740251 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.740872 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/
--rw-r--r--   0 val        (502) staff       (20)       55 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
--rw-r--r--   0 val        (502) staff       (20)      389 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.741293 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
--rw-r--r--   0 val        (502) staff       (20)      742 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
--rw-r--r--   0 val        (502) staff       (20)      276 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.741568 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
--rw-r--r--   0 val        (502) staff       (20)      124 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.612385 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.612429 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.741948 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 val        (502) staff       (20)      483 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 val        (502) staff       (20)      727 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 val        (502) staff       (20)      938 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.742413 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
--rw-r--r--   0 val        (502) staff       (20)       64 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
--rw-r--r--   0 val        (502) staff       (20)      662 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
--rw-r--r--   0 val        (502) staff       (20)     3669 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
--rw-r--r--   0 val        (502) staff       (20)       68 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
--rw-r--r--   0 val        (502) staff       (20)      556 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/create_admin.sh
--rw-r--r--   0 val        (502) staff       (20)      624 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/fab_config.py
--rw-r--r--   0 val        (502) staff       (20)     2683 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/home.js
--rw-r--r--   0 val        (502) staff       (20)     3121 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js
--rw-r--r--   0 val        (502) staff       (20)    35986 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/ui_admin_creator.py
--rw-r--r--   0 val        (502) staff       (20)     2260 2023-07-03 20:17:33.000000 ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/uri_info.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.755336 ApiLogicServer-9.1.0/api_logic_server_cli/database/
--rw-r--r--   0 val        (502) staff       (20)  1067008 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite
--rw-r--r--   0 val        (502) staff       (20)       60 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/__init__.py
--rw-r--r--   0 val        (502) staff       (20)   545792 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/allocation.sqlite
--rw-r--r--   0 val        (502) staff       (20)    45056 2023-06-27 01:00:21.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/authentication.sqlite
--rw-r--r--   0 val        (502) staff       (20)    53248 2023-06-28 14:25:55.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/authentication_doc.sqlite
--rw-r--r--   0 val        (502) staff       (20)   413696 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/classicmodels.sqlite
--rw-r--r--   0 val        (502) staff       (20)      122 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)    16384 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/new.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/nw-gold-plus.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)   496640 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/nw.sqlite
--rw-r--r--   0 val        (502) staff       (20)    32768 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/table_filters_tests.sqlite
--rw-r--r--   0 val        (502) staff       (20)       53 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/table_filters_tests.yml
--rw-r--r--   0 val        (502) staff       (20)       23 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/table_filters_tests_nw.yml
--rw-r--r--   0 val        (502) staff       (20)       25 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/table_filters_tests_nw_1.yml
--rw-r--r--   0 val        (502) staff       (20)       21 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/table_filters_tests_typical.yml
--rw-r--r--   0 val        (502) staff       (20)    16384 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/database/todos.sqlite
--rw-r--r--   0 val        (502) staff       (20)    13761 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/extended_builder.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.756608 ApiLogicServer-9.1.0/api_logic_server_cli/fragments/
--rw-r--r--   0 val        (502) staff       (20)     1431 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
--rw-r--r--   0 val        (502) staff       (20)     1956 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/fragments/configZZ.py
--rw-r--r--   0 val        (502) staff       (20)       63 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/fragments/db_typesZZ.txt
--rw-r--r--   0 val        (502) staff       (20)    12053 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/fragments/modelsZZ.py
--rw-r--r--   0 val        (502) staff       (20)      888 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/fragments/nw_virtual_attrs.py
--rw-r--r--   0 val        (502) staff       (20)      870 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
--rw-r--r--   0 val        (502) staff       (20)     1006 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.759003 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.759635 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      438 2023-07-04 21:48:28.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      106 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.612846 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.760711 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     1127 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
--rw-r--r--   0 val        (502) staff       (20)     1306 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1196 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1205 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1193 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
--rw-r--r--   0 val        (502) staff       (20)     2444 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.761178 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     7676 2023-07-01 02:50:31.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      368 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.761994 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     2053 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/customize_api.py
--rw-r--r--   0 val        (502) staff       (20)      316 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/expose_api_models.py
--rw-r--r--   0 val        (502) staff       (20)      521 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/json_encoder.py
--rw-r--r--   0 val        (502) staff       (20)     4286 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/readme_customize_api.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.613057 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/system/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.762311 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/system/opt_locking/
--rw-r--r--   0 val        (502) staff       (20)     5467 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/system/opt_locking/opt_locking.py
--rw-r--r--   0 val        (502) staff       (20)     6760 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/system/opt_locking/readme.md
--rw-r--r--   0 val        (502) staff       (20)    17475 2023-07-01 17:44:23.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api_logic_server_run.py
--rw-r--r--   0 val        (502) staff       (20)     4108 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.763089 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.763470 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/
--rw-r--r--   0 val        (502) staff       (20)     2101 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/env.py
--rw-r--r--   0 val        (502) staff       (20)     1967 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/readme.md
--rw-r--r--   0 val        (502) staff       (20)      494 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.763638 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/versions/
--rw-r--r--   0 val        (502) staff       (20)       60 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
--rw-r--r--   0 val        (502) staff       (20)     3027 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic.ini
--rw-r--r--   0 val        (502) staff       (20)      537 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/bind_databases.py
--rw-r--r--   0 val        (502) staff       (20)      469 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)     1029 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/db_debug.py
--rw-r--r--   0 val        (502) staff       (20)      588 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/multi_db.py
--rw-r--r--   0 val        (502) staff       (20)      139 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/default.env
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.763792 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.764424 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/
--rw-r--r--   0 val        (502) staff       (20)     2381 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
--rw-r--r--   0 val        (502) staff       (20)     3643 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
--rw-r--r--   0 val        (502) staff       (20)      331 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     2079 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
--rw-r--r--   0 val        (502) staff       (20)      876 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.764571 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/python-anywhere/
--rw-r--r--   0 val        (502) staff       (20)     3820 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py
--rw-r--r--   0 val        (502) staff       (20)     1943 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.764803 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/logic/
--rw-r--r--   0 val        (502) staff       (20)     1610 2023-06-28 15:01:50.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)     6210 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
--rw-r--r--   0 val        (502) staff       (20)      568 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/mypy.ini
--rw-r--r--   0 val        (502) staff       (20)     7768 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)      801 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/run.ps1
--rwxr-xr-x   0 val        (502) staff       (20)     1057 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/run.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.765028 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.765224 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
--rw-r--r--   0 val        (502) staff       (20)      580 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.765463 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
--rw-r--r--   0 val        (502) staff       (20)     4355 2023-06-28 15:01:50.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)     2907 2023-06-28 15:01:50.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.613803 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.765577 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
--rw-r--r--   0 val        (502) staff       (20)     2165 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)      753 2023-06-28 15:01:50.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.766000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/notes_temp/
--rw-r--r--   0 val        (502) staff       (20)     1403 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
--rw-r--r--   0 val        (502) staff       (20)     1156 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
--rw-r--r--   0 val        (502) staff       (20)     1364 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.766414 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/system/
--rw-r--r--   0 val        (502) staff       (20)     3425 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/system/authentication.py
--rw-r--r--   0 val        (502) staff       (20)     6004 2023-06-28 15:01:50.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/system/authorization.py
--rw-r--r--   0 val        (502) staff       (20)     1705 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.766569 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/templates/
--rw-r--r--   0 val        (502) staff       (20)     3765 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/templates/index.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.766709 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.767015 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     9969 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
--rw-r--r--   0 val        (502) staff       (20)     1026 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.767140 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      414 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.767416 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      416 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     2163 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.767829 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
--rw-r--r--   0 val        (502) staff       (20)      147 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
--rw-r--r--   0 val        (502) staff       (20)    65295 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.768090 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/basic/
--rw-r--r--   0 val        (502) staff       (20)      735 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/basic/server_test.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.768207 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.768416 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)     6671 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
--rw-r--r--   0 val        (502) staff       (20)     2750 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/admin/home.js
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.614715 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.770014 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3778 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
--rw-r--r--   0 val        (502) staff       (20)     3719 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.771192 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/
--rw-r--r--   0 val        (502) staff       (20)     6054 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.771339 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/templates/
--rw-r--r--   0 val        (502) staff       (20)       26 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/templates/content.html
--rw-r--r--   0 val        (502) staff       (20)     9262 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/util.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.772164 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/
--rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/py.py
--rw-r--r--   0 val        (502) staff       (20)      738 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
--rw-r--r--   0 val        (502) staff       (20)      579 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
--rw-r--r--   0 val        (502) staff       (20)      900 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
--rw-r--r--   0 val        (502) staff       (20)      698 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
--rw-r--r--   0 val        (502) staff       (20)      893 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.772305 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/
--rw-r--r--   0 val        (502) staff       (20)     7733 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/Logic-Allocation.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.615115 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/images/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.773753 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/images/allocation/
--rw-r--r--   0 val        (502) staff       (20)   670261 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/images/allocation/db.png
--rw-r--r--   0 val        (502) staff       (20)  1035433 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/images/allocation/logic-diagram.png
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.775139 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/logic/
--rw-r--r--   0 val        (502) staff       (20)     1398 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.775242 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/test/
--rw-r--r--   0 val        (502) staff       (20)      583 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/test/test.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.777013 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/
--rw-r--r--   0 val        (502) staff       (20)    15287 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/Tutorial.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.777224 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/
--rw-r--r--   0 val        (502) staff       (20)    10062 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.777539 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/
--rw-r--r--   0 val        (502) staff       (20)    34142 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
--rw-r--r--   0 val        (502) staff       (20)      650 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.777823 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/database/
--rw-r--r--   0 val        (502) staff       (20)     2665 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)     2126 2023-06-30 16:43:54.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/database/db_debug.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.777936 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/logic/
--rw-r--r--   0 val        (502) staff       (20)    11735 2023-06-30 02:27:42.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)      241 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.778049 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/security/
--rw-r--r--   0 val        (502) staff       (20)     1212 2023-06-28 15:01:50.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.778250 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.778514 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.779307 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      187 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
--rw-r--r--   0 val        (502) staff       (20)      285 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
--rw-r--r--   0 val        (502) staff       (20)      521 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/opt_locking.feature
--rw-r--r--   0 val        (502) staff       (20)     1281 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
--rw-r--r--   0 val        (502) staff       (20)      473 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.779963 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      450 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     2130 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
--rw-r--r--   0 val        (502) staff       (20)     2795 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/opt_locking.py
--rw-r--r--   0 val        (502) staff       (20)    16830 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
--rw-r--r--   0 val        (502) staff       (20)     4722 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.780083 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
--rw-r--r--   0 val        (502) staff       (20)     4356 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.781497 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
--rw-r--r--   0 val        (502) staff       (20)     5070 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     5794 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     2568 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
--rw-r--r--   0 val        (502) staff       (20)     8481 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
--rw-r--r--   0 val        (502) staff       (20)     8445 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
--rw-r--r--   0 val        (502) staff       (20)     2561 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.782202 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.783942 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/
--rw-r--r--   0 val        (502) staff       (20)     5070 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
--rw-r--r--   0 val        (502) staff       (20)    16926 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
--rw-r--r--   0 val        (502) staff       (20)      840 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
--rw-r--r--   0 val        (502) staff       (20)     1381 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
--rw-r--r--   0 val        (502) staff       (20)      831 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
--rw-r--r--   0 val        (502) staff       (20)     8405 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
--rw-r--r--   0 val        (502) staff       (20)    13497 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
--rw-r--r--   0 val        (502) staff       (20)     1543 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
--rw-r--r--   0 val        (502) staff       (20)      447 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/readme_test.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.616545 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.784422 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)    17252 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     3443 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
--rw-r--r--   0 val        (502) staff       (20)     8798 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.616690 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.785559 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/
--rw-r--r--   0 val        (502) staff       (20)     6054 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.787220 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3719 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
--rw-r--r--   0 val        (502) staff       (20)     3778 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.787376 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw_no_cust/
--rw-r--r--   0 val        (502) staff       (20)     5431 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.788458 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-06-24 17:45:45.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.789468 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      444 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      254 2023-06-25 00:43:10.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.789923 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     8343 2023-06-24 20:07:24.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      368 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.792156 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-06-24 17:45:46.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.792516 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
--rw-r--r--   0 val        (502) staff       (20)     3858 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
--rw-r--r--   0 val        (502) staff       (20)     2058 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.793992 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
--rw-r--r--   0 val        (502) staff       (20)    11945 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
--rw-r--r--   0 val        (502) staff       (20)     1470 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
--rw-r--r--   0 val        (502) staff       (20)     1302 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
--rw-r--r--   0 val        (502) staff       (20)     7877 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.794146 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/test/
--rw-r--r--   0 val        (502) staff       (20)      786 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/test/server_test.py
--rw-r--r--   0 val        (502) staff       (20)     9219 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
--rw-r--r--   0 val        (502) staff       (20)    22117 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/sample_db.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.797474 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/
--rw-r--r--   0 val        (502) staff       (20)      369 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.797952 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      237 2023-06-23 14:12:04.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    22604 2023-06-30 13:39:12.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    53944 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
--rw-r--r--   0 val        (502) staff       (20)       54 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.800729 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)     1850 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
--rw-r--r--   0 val        (502) staff       (20)     2593 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
--rw-r--r--   0 val        (502) staff       (20)     3865 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.801066 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      249 2023-06-23 14:12:04.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)       87 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
--rw-r--r--   0 val        (502) staff       (20)     1399 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)      196 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.802234 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.803013 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      261 2023-06-23 14:12:04.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    78750 2023-07-01 17:26:19.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.804333 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.806616 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/
--rw-r--r--   0 val        (502) staff       (20)     7373 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_ga.py
--rw-r--r--   0 val        (502) staff       (20)    11978 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_gen.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.807314 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/
--rw-r--r--   0 val        (502) staff       (20)    60629 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegen.py
--rw-r--r--   0 val        (502) staff       (20)    60755 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX-merged.py
--rw-r--r--   0 val        (502) staff       (20)    59103 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX.py
--rw-r--r--   0 val        (502) staff       (20)    59100 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenZ.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.808257 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/
--rw-r--r--   0 val        (502) staff       (20)    21919 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models.py
--rw-r--r--   0 val        (502) staff       (20)    21992 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models_rc2.py
--rw-r--r--   0 val        (502) staff       (20)     1066 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze.txt
--rw-r--r--   0 val        (502) staff       (20)     1100 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze_rc2.txt
--rw-r--r--   0 val        (502) staff       (20)    16390 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/delete_log.txt
--rw-r--r--   0 val        (502) staff       (20)     3991 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/notes.txt
--rw-r--r--   0 val        (502) staff       (20)     7159 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/nw-schema.txt
--rw-r--r--   0 val        (502) staff       (20)    65200 2023-07-01 02:46:07.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
--rw-r--r--   0 val        (502) staff       (20)     3252 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.808465 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
--rw-r--r--   0 val        (502) staff       (20)    33384 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
--rw-r--r--   0 val        (502) staff       (20)      440 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
--rwxr-xr-x   0 val        (502) staff       (20)    18938 2023-06-30 02:27:42.000000 ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-07-04 23:54:48.812749 ApiLogicServer-9.1.0/api_logic_server_cli/templates/
--rw-r--r--   0 val        (502) staff       (20)    14864 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/templates/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     1221 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/templates/app_fiddle.md
--rw-r--r--   0 val        (502) staff       (20)     3322 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/templates/app_fiddle.txt
--rw-r--r--   0 val        (502) staff       (20)     3765 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/templates/index.html
--rw-r--r--   0 val        (502) staff       (20)      900 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/templates/login_endpoint.txt
--rw-r--r--   0 val        (502) staff       (20)      205 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/templates/login_endpoint_imports.txt
--rw-r--r--   0 val        (502) staff       (20)      479 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.0/api_logic_server_cli/templates/opt_locking.txt
--rw-r--r--   0 val        (502) staff       (20)       38 2023-07-04 23:54:48.813289 ApiLogicServer-9.1.0/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)     3709 2023-07-04 22:18:58.000000 ApiLogicServer-9.1.0/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.908190 ApiLogicServer-9.1.32/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.801200 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/
+-rw-r--r--   0 val        (502) staff       (20)    15094 2023-08-04 15:21:07.000000 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    49965 2023-08-04 15:21:07.000000 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-08-04 15:21:07.000000 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (502) staff       (20)       66 2023-08-04 15:21:07.000000 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/entry_points.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-08-04 15:21:07.000000 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/not-zip-safe
+-rw-r--r--   0 val        (502) staff       (20)      662 2023-08-04 15:21:07.000000 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/requires.txt
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-08-04 15:21:07.000000 ApiLogicServer-9.1.32/ApiLogicServer.egg-info/top_level.txt
+-rw-r--r--   0 val        (502) staff       (20)     1485 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/LICENSE
+-rw-r--r--   0 val        (502) staff       (20)      804 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/MANIFEST.in
+-rw-r--r--   0 val        (502) staff       (20)    15094 2023-08-04 15:21:07.907908 ApiLogicServer-9.1.32/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    14087 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/README.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.802487 ApiLogicServer-9.1.32/api_logic_server_cli/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    64040 2023-08-04 15:14:32.000000 ApiLogicServer-9.1.32/api_logic_server_cli/api_logic_server.py
+-rw-r--r--   0 val        (502) staff       (20)      135 2023-08-04 13:47:15.000000 ApiLogicServer-9.1.32/api_logic_server_cli/api_logic_server_info.yaml
+-rw-r--r--   0 val        (502) staff       (20)    35571 2023-08-02 21:55:28.000000 ApiLogicServer-9.1.32/api_logic_server_cli/cli.py
+-rw-r--r--   0 val        (502) staff       (20)     1887 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/cli_args_base.py
+-rw-r--r--   0 val        (502) staff       (20)     3303 2023-08-02 22:02:38.000000 ApiLogicServer-9.1.32/api_logic_server_cli/cli_args_project.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.803738 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.804507 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      235 2023-06-23 14:12:03.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5355 2023-06-23 14:12:05.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    14644 2023-08-02 22:18:34.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    35464 2023-06-23 14:12:03.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    37429 2023-06-23 14:12:05.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2676 2023-07-20 00:20:47.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5301 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
+-rw-r--r--   0 val        (502) staff       (20)    12990 2023-08-02 22:18:32.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/api_logic_server_utils.py
+-rw-r--r--   0 val        (502) staff       (20)    34482 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/model_creation_services.py
+-rw-r--r--   0 val        (502) staff       (20)     6127 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.805354 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
+-rwxr-xr-x   0 val        (502) staff       (20)    15430 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.805474 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
+-rwxr-xr-x   0 val        (502) staff       (20)  1145966 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
+-rwxr-xr-x   0 val        (502) staff       (20)     3870 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
+-rwxr-xr-x   0 val        (502) staff       (20)      692 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
+-rwxr-xr-x   0 val        (502) staff       (20)     5347 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
+-rwxr-xr-x   0 val        (502) staff       (20)     9664 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
+-rwxr-xr-x   0 val        (502) staff       (20)      492 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
+-rwxr-xr-x   0 val        (502) staff       (20)       67 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.793222 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.806743 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
+-rwxr-xr-x   0 val        (502) staff       (20)    86781 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
+-rwxr-xr-x   0 val        (502) staff       (20)   166928 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
+-rwxr-xr-x   0 val        (502) staff       (20)      211 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
+-rwxr-xr-x   0 val        (502) staff       (20)      516 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.854297 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
+-rwxr-xr-x   0 val        (502) staff       (20)     1576 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     3197 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     9011 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    21905 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2921 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     7103 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     1004 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     2792 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     7546 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    17381 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    33520 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    71153 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    14043 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    36857 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5595 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    14138 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     6135 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    14288 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2280 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     5953 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3747 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8068 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4407 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    10552 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2156 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     5783 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    11957 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    24504 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5499 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    13356 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4187 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    10856 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     7001 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    17447 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3591 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8746 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3747 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     9475 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3140 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     7634 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4056 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     9168 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     8184 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    18882 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4068 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     9104 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    14317 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    32894 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3963 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     9547 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3152 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8052 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     8662 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    20172 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4982 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    13442 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     6569 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    15183 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2002 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     4736 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2974 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     7499 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     1967 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     5172 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5948 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    13558 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    10454 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    23458 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     1255 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     3229 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4128 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    10303 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    17096 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    31009 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     7760 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    18142 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     9800 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    21207 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3420 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8828 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3820 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    10430 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    41393 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)   145206 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5605 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    13185 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     8412 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    19971 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     9916 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    22155 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     6545 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    16602 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4681 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    11819 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3545 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8963 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3710 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     9146 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     1924 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     4864 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5069 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    11830 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3092 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8217 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2417 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     6013 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     7472 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    16988 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2342 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     6267 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)  3310604 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      576 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20) 10838575 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    35620 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)   121512 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    17547 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    39845 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2594 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     6567 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2814 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     7255 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    18754 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    38065 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2736 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     7008 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2693 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     6865 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3378 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8159 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2709 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     6645 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4619 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    10592 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4203 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    10608 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2559 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     6522 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5926 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    96741 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     1840 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     5116 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     8013 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    19497 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3725 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     9025 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3288 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8254 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2026 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     5528 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    13558 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    26650 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     9201 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    21765 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5069 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    11826 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    34921 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)   119930 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4669 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    10814 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     4316 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    10868 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)    11414 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    24817 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     2622 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)     7016 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     5259 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)    13615 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     7391 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)    17258 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     1986 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     4960 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)     3230 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
+-rwxr-xr-x   0 val        (502) staff       (20)      387 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)     8177 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
+-rwxr-xr-x   0 val        (502) staff       (20)  1384276 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
+-rwxr-xr-x   0 val        (502) staff       (20)     3014 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
+-rwxr-xr-x   0 val        (502) staff       (20)  5552838 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.857209 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
+-rwxr-xr-x   0 val        (502) staff       (20)    72504 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.857817 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.860114 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/
+-rw-r--r--   0 val        (502) staff       (20)       55 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
+-rw-r--r--   0 val        (502) staff       (20)      389 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.860545 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
+-rw-r--r--   0 val        (502) staff       (20)      742 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)      276 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.860859 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
+-rw-r--r--   0 val        (502) staff       (20)      124 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.793539 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.793580 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.862332 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 val        (502) staff       (20)      483 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 val        (502) staff       (20)      727 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 val        (502) staff       (20)      938 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.862701 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
+-rw-r--r--   0 val        (502) staff       (20)       64 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
+-rw-r--r--   0 val        (502) staff       (20)      662 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
+-rw-r--r--   0 val        (502) staff       (20)     3669 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
+-rw-r--r--   0 val        (502) staff       (20)       68 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
+-rw-r--r--   0 val        (502) staff       (20)      556 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/create_admin.sh
+-rw-r--r--   0 val        (502) staff       (20)      624 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/fab_config.py
+-rw-r--r--   0 val        (502) staff       (20)     2683 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/home.js
+-rw-r--r--   0 val        (502) staff       (20)     3121 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/react_admin_component.js
+-rw-r--r--   0 val        (502) staff       (20)    35986 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/ui_admin_creator.py
+-rw-r--r--   0 val        (502) staff       (20)     2260 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/uri_info.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.867162 ApiLogicServer-9.1.32/api_logic_server_cli/database/
+-rw-r--r--   0 val        (502) staff       (20)  1067008 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/Chinook_Sqlite.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       60 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)   545792 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/allocation.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    45056 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/authentication.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    53248 2023-06-28 14:25:55.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/authentication_doc.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   413696 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/classicmodels.sqlite
+-rw-r--r--   0 val        (502) staff       (20)      122 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)    16384 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/new.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/nw-gold-plus.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   496640 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/nw.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    32768 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/table_filters_tests.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       53 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/table_filters_tests.yml
+-rw-r--r--   0 val        (502) staff       (20)       23 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/table_filters_tests_nw.yml
+-rw-r--r--   0 val        (502) staff       (20)       25 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/table_filters_tests_nw_1.yml
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/table_filters_tests_typical.yml
+-rw-r--r--   0 val        (502) staff       (20)    16384 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/database/todos.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    13761 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/extended_builder.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.867861 ApiLogicServer-9.1.32/api_logic_server_cli/fragments/
+-rw-r--r--   0 val        (502) staff       (20)     1431 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
+-rw-r--r--   0 val        (502) staff       (20)     1956 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/fragments/configZZ.py
+-rw-r--r--   0 val        (502) staff       (20)       63 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/fragments/db_typesZZ.txt
+-rw-r--r--   0 val        (502) staff       (20)    12053 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/fragments/modelsZZ.py
+-rw-r--r--   0 val        (502) staff       (20)      888 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/fragments/nw_virtual_attrs.py
+-rw-r--r--   0 val        (502) staff       (20)      870 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
+-rw-r--r--   0 val        (502) staff       (20)     1006 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.870887 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-07-31 01:58:47.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.871229 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      438 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     2114 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      310 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      132 2023-08-02 04:42:08.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.793935 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.872594 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     1127 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
+-rw-r--r--   0 val        (502) staff       (20)     1306 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1196 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1205 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1193 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
+-rw-r--r--   0 val        (502) staff       (20)     2444 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.872969 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     8505 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      368 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.874076 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     2053 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/customize_api.py
+-rw-r--r--   0 val        (502) staff       (20)      316 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/expose_api_models.py
+-rw-r--r--   0 val        (502) staff       (20)      521 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/json_encoder.py
+-rw-r--r--   0 val        (502) staff       (20)     4286 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/readme_customize_api.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.794151 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/system/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.874384 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/system/opt_locking/
+-rw-r--r--   0 val        (502) staff       (20)     5471 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/system/opt_locking/opt_locking.py
+-rw-r--r--   0 val        (502) staff       (20)     6760 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/system/opt_locking/readme.md
+-rw-r--r--   0 val        (502) staff       (20)    13121 2023-07-30 00:40:03.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api_logic_server_run.py
+-rw-r--r--   0 val        (502) staff       (20)    17249 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.876440 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.876939 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/
+-rw-r--r--   0 val        (502) staff       (20)     2101 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/env.py
+-rw-r--r--   0 val        (502) staff       (20)     1967 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/readme.md
+-rw-r--r--   0 val        (502) staff       (20)      494 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.877088 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/versions/
+-rw-r--r--   0 val        (502) staff       (20)       60 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     3027 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic.ini
+-rw-r--r--   0 val        (502) staff       (20)      537 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/bind_databases.py
+-rw-r--r--   0 val        (502) staff       (20)      469 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)     1029 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/db_debug.py
+-rw-r--r--   0 val        (502) staff       (20)      588 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/multi_db.py
+-rw-r--r--   0 val        (502) staff       (20)      139 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/default.env
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.877893 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-08-01 16:36:11.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.878332 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/auth-db/
+-rw-r--r--   0 val        (502) staff       (20)     2381 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/auth-db/authdb_mysql.Dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     3648 2023-08-02 20:56:16.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/auth-db/authdb_mysql.sql
+-rw-r--r--   0 val        (502) staff       (20)     1161 2023-07-28 03:22:15.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/auth-db/authdb_postgres.sql
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.879374 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-07-28 02:48:16.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)      374 2023-07-31 16:22:34.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/Dockerfile.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1130 2023-08-01 15:50:23.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/docker-compose.ps1
+-rw-r--r--   0 val        (502) staff       (20)      863 2023-07-31 18:48:55.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/docker-compose.sh
+-rw-r--r--   0 val        (502) staff       (20)     2591 2023-08-04 13:57:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/docker-compose.yml
+-rw-r--r--   0 val        (502) staff       (20)       18 2023-08-01 16:34:33.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/env-docker-compose.env
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.879496 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/etc/
+-rw-r--r--   0 val        (502) staff       (20)     1018 2023-08-02 04:40:53.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/etc/nginx.conf
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.794844 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/etc/ssl/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.879629 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/etc/ssl/certs/
+-rw-r--r--   0 val        (502) staff       (20)     1874 2023-08-02 04:40:53.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/etc/ssl/certs/example.com.crt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.879790 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/etc/ssl/private/
+-rw-r--r--   0 val        (502) staff       (20)     3272 2023-08-02 04:40:53.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/etc/ssl/private/example.com.key
+-rw-r--r--   0 val        (502) staff       (20)      499 2023-08-03 21:43:01.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/install-webapp.sh
+-rw-r--r--   0 val        (502) staff       (20)      638 2023-08-03 14:54:46.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/readme-docker-compose.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.880204 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/unused/
+-rw-r--r--   0 val        (502) staff       (20)     3737 2023-07-31 15:08:49.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/unused/unused-docker-compose.py
+-rw-r--r--   0 val        (502) staff       (20)      742 2023-07-31 14:08:59.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/unused/unused-get_ip.py
+-rw-r--r--   0 val        (502) staff       (20)       14 2023-07-27 02:59:22.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/unused/unused-requirements-slim.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.880819 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-image/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-07-25 02:53:01.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-image/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)      491 2023-07-31 02:04:54.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-image/build_image.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1972 2023-07-29 23:13:53.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-image/build_image.sh
+-rw-r--r--   0 val        (502) staff       (20)     1463 2023-08-03 14:53:09.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-image/env.list
+-rw-r--r--   0 val        (502) staff       (20)      901 2023-07-29 23:19:06.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-image/run_image.sh
+-rw-r--r--   0 val        (502) staff       (20)      876 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.880972 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/python-anywhere/
+-rw-r--r--   0 val        (502) staff       (20)     3820 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py
+-rw-r--r--   0 val        (502) staff       (20)     2080 2023-08-04 13:40:27.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.881265 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/logic/
+-rw-r--r--   0 val        (502) staff       (20)     1610 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)     6210 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
+-rw-r--r--   0 val        (502) staff       (20)      568 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/mypy.ini
+-rw-r--r--   0 val        (502) staff       (20)     7768 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)      801 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/run.ps1
+-rwxr-xr-x   0 val        (502) staff       (20)     1057 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/run.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.881540 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.881745 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)      580 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.881972 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
+-rw-r--r--   0 val        (502) staff       (20)     4355 2023-07-20 18:41:20.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)     2907 2023-07-20 18:41:20.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.795436 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.882090 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
+-rw-r--r--   0 val        (502) staff       (20)     2760 2023-08-04 13:42:49.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)      753 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.882433 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/notes_temp/
+-rw-r--r--   0 val        (502) staff       (20)     1403 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
+-rw-r--r--   0 val        (502) staff       (20)     1156 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
+-rw-r--r--   0 val        (502) staff       (20)     1364 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.882822 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/system/
+-rw-r--r--   0 val        (502) staff       (20)     3543 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/system/authentication.py
+-rw-r--r--   0 val        (502) staff       (20)     5998 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/system/authorization.py
+-rw-r--r--   0 val        (502) staff       (20)     1705 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.882943 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/templates/
+-rw-r--r--   0 val        (502) staff       (20)     3765 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/templates/index.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.883054 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.883346 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     9969 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
+-rw-r--r--   0 val        (502) staff       (20)     1268 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.883466 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      414 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.883720 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      416 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     2225 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.884063 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
+-rw-r--r--   0 val        (502) staff       (20)      147 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
+-rw-r--r--   0 val        (502) staff       (20)    65295 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.884222 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)      735 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/basic/server_test.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.884350 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.884575 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)     7356 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
+-rw-r--r--   0 val        (502) staff       (20)     2750 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/admin/home.js
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.796237 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.886721 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3778 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3719 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.887689 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.887805 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/templates/
+-rw-r--r--   0 val        (502) staff       (20)       26 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/templates/content.html
+-rw-r--r--   0 val        (502) staff       (20)     9476 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/util.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.888522 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/
+-rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/py.py
+-rw-r--r--   0 val        (502) staff       (20)      738 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
+-rw-r--r--   0 val        (502) staff       (20)      579 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
+-rw-r--r--   0 val        (502) staff       (20)      698 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
+-rw-r--r--   0 val        (502) staff       (20)      893 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/venv.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.888646 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/
+-rw-r--r--   0 val        (502) staff       (20)     7733 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/Logic-Allocation.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.796489 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/images/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.889266 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/images/allocation/
+-rw-r--r--   0 val        (502) staff       (20)   670261 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/images/allocation/db.png
+-rw-r--r--   0 val        (502) staff       (20)  1035433 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/images/allocation/logic-diagram.png
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.889922 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/logic/
+-rw-r--r--   0 val        (502) staff       (20)     1398 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.890037 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/test/
+-rw-r--r--   0 val        (502) staff       (20)      583 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/test/test.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.890278 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/
+-rw-r--r--   0 val        (502) staff       (20)    15287 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/Tutorial.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.890408 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/
+-rw-r--r--   0 val        (502) staff       (20)     9885 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/customize_api.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.890721 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/multi-table-example/
+-rw-r--r--   0 val        (502) staff       (20)    34142 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
+-rw-r--r--   0 val        (502) staff       (20)      650 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.891027 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/database/
+-rw-r--r--   0 val        (502) staff       (20)     2665 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)     2126 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/database/db_debug.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.891153 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/logic/
+-rw-r--r--   0 val        (502) staff       (20)    11841 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)      241 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.891276 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/security/
+-rw-r--r--   0 val        (502) staff       (20)     1212 2023-07-25 02:53:35.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.891490 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.891610 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.892171 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      187 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
+-rw-r--r--   0 val        (502) staff       (20)      285 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
+-rw-r--r--   0 val        (502) staff       (20)      521 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/opt_locking.feature
+-rw-r--r--   0 val        (502) staff       (20)     1281 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
+-rw-r--r--   0 val        (502) staff       (20)      473 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.892821 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      450 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     2130 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
+-rw-r--r--   0 val        (502) staff       (20)     2795 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/opt_locking.py
+-rw-r--r--   0 val        (502) staff       (20)    16830 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
+-rw-r--r--   0 val        (502) staff       (20)     4722 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.892953 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
+-rw-r--r--   0 val        (502) staff       (20)     4356 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.894139 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     5794 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     2568 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
+-rw-r--r--   0 val        (502) staff       (20)     8481 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
+-rw-r--r--   0 val        (502) staff       (20)     8445 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
+-rw-r--r--   0 val        (502) staff       (20)     2561 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.894609 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.895888 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
+-rw-r--r--   0 val        (502) staff       (20)    16926 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
+-rw-r--r--   0 val        (502) staff       (20)      840 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
+-rw-r--r--   0 val        (502) staff       (20)     1381 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
+-rw-r--r--   0 val        (502) staff       (20)      831 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
+-rw-r--r--   0 val        (502) staff       (20)     8405 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
+-rw-r--r--   0 val        (502) staff       (20)    13497 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
+-rw-r--r--   0 val        (502) staff       (20)     1543 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
+-rw-r--r--   0 val        (502) staff       (20)      447 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/readme_test.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.797566 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.896242 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)    17252 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     3443 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
+-rw-r--r--   0 val        (502) staff       (20)     8798 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.797671 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.897291 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.898361 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3719 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3778 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.898476 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw_no_cust/
+-rw-r--r--   0 val        (502) staff       (20)     5431 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.899093 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-06-24 17:45:45.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.899787 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      444 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     2114 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      254 2023-06-25 00:43:10.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.900071 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     8295 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      368 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.900886 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-06-24 17:45:46.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.901021 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
+-rw-r--r--   0 val        (502) staff       (20)     3858 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
+-rw-r--r--   0 val        (502) staff       (20)     2058 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.901705 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)    11945 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
+-rw-r--r--   0 val        (502) staff       (20)     1470 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
+-rw-r--r--   0 val        (502) staff       (20)     1302 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)     7877 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.901842 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/test/
+-rw-r--r--   0 val        (502) staff       (20)      786 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/test/server_test.py
+-rw-r--r--   0 val        (502) staff       (20)     9219 2023-06-24 17:39:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
+-rw-r--r--   0 val        (502) staff       (20)    22117 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/sample_db.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.902433 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/
+-rw-r--r--   0 val        (502) staff       (20)      369 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.902702 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      237 2023-06-23 14:12:04.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    22604 2023-07-20 00:20:47.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    53944 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
+-rw-r--r--   0 val        (502) staff       (20)       54 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.903634 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)     1850 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
+-rw-r--r--   0 val        (502) staff       (20)     2593 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
+-rw-r--r--   0 val        (502) staff       (20)     3865 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.903774 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      249 2023-06-23 14:12:04.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)       87 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
+-rw-r--r--   0 val        (502) staff       (20)     1399 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)      196 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.904185 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.904424 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      261 2023-06-23 14:12:04.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    78750 2023-07-20 00:20:47.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.904873 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.905117 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/
+-rw-r--r--   0 val        (502) staff       (20)     7373 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_ga.py
+-rw-r--r--   0 val        (502) staff       (20)    11978 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_gen.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.905939 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/
+-rw-r--r--   0 val        (502) staff       (20)    60629 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegen.py
+-rw-r--r--   0 val        (502) staff       (20)    60755 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX-merged.py
+-rw-r--r--   0 val        (502) staff       (20)    59103 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX.py
+-rw-r--r--   0 val        (502) staff       (20)    59100 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenZ.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.906654 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/
+-rw-r--r--   0 val        (502) staff       (20)    21919 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models.py
+-rw-r--r--   0 val        (502) staff       (20)    21992 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models_rc2.py
+-rw-r--r--   0 val        (502) staff       (20)     1066 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze.txt
+-rw-r--r--   0 val        (502) staff       (20)     1100 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze_rc2.txt
+-rw-r--r--   0 val        (502) staff       (20)    16390 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/delete_log.txt
+-rw-r--r--   0 val        (502) staff       (20)     3991 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/notes.txt
+-rw-r--r--   0 val        (502) staff       (20)     7159 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/nw-schema.txt
+-rw-r--r--   0 val        (502) staff       (20)    65200 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
+-rw-r--r--   0 val        (502) staff       (20)     3252 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.906784 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
+-rw-r--r--   0 val        (502) staff       (20)    33384 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
+-rw-r--r--   0 val        (502) staff       (20)      440 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
+-rwxr-xr-x   0 val        (502) staff       (20)    18938 2023-07-20 00:16:51.000000 ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-08-04 15:21:07.907643 ApiLogicServer-9.1.32/api_logic_server_cli/templates/
+-rw-r--r--   0 val        (502) staff       (20)    14864 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/templates/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     1221 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/templates/app_fiddle.md
+-rw-r--r--   0 val        (502) staff       (20)     3322 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/templates/app_fiddle.txt
+-rw-r--r--   0 val        (502) staff       (20)     3765 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/templates/index.html
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/templates/login_endpoint.txt
+-rw-r--r--   0 val        (502) staff       (20)      205 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/templates/login_endpoint_imports.txt
+-rw-r--r--   0 val        (502) staff       (20)      479 2023-06-23 14:02:17.000000 ApiLogicServer-9.1.32/api_logic_server_cli/templates/opt_locking.txt
+-rw-r--r--   0 val        (502) staff       (20)       38 2023-08-04 15:21:07.908226 ApiLogicServer-9.1.32/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)     3909 2023-08-04 15:14:09.000000 ApiLogicServer-9.1.32/setup.py
```

### Comparing `ApiLogicServer-9.1.0/ApiLogicServer.egg-info/PKG-INFO` & `ApiLogicServer-9.1.32/ApiLogicServer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 9.1.0
+Version: 9.1.32
 Summary: Create JSON:API and Admin Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/ApiLogicServer/ApiLogicServer-src
 Author: Val Huber
 Author-email: apilogicserver@gmail.com
 License: BSD
 Project-URL: Docs, https://apilogicserver.github.io/Docs/
 Platform: any
```

### Comparing `ApiLogicServer-9.1.0/ApiLogicServer.egg-info/SOURCES.txt` & `ApiLogicServer-9.1.32/ApiLogicServer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -324,14 +324,15 @@
 api_logic_server_cli/database/todos.sqlite
 api_logic_server_cli/fragments/Todo_modelsZZ.py.py
 api_logic_server_cli/fragments/configZZ.py
 api_logic_server_cli/fragments/db_typesZZ.txt
 api_logic_server_cli/fragments/modelsZZ.py
 api_logic_server_cli/fragments/nw_virtual_attrs.py
 api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
+api_logic_server_cli/project_prototype/.DS_Store
 api_logic_server_cli/project_prototype/.gitignore
 api_logic_server_cli/project_prototype/api_logic_server_run.py
 api_logic_server_cli/project_prototype/config.py
 api_logic_server_cli/project_prototype/default.env
 api_logic_server_cli/project_prototype/logging.yml
 api_logic_server_cli/project_prototype/mypy.ini
 api_logic_server_cli/project_prototype/readme.md
@@ -363,19 +364,38 @@
 api_logic_server_cli/project_prototype/database/customize_models.py
 api_logic_server_cli/project_prototype/database/db_debug.py
 api_logic_server_cli/project_prototype/database/multi_db.py
 api_logic_server_cli/project_prototype/database/alembic/env.py
 api_logic_server_cli/project_prototype/database/alembic/readme.md
 api_logic_server_cli/project_prototype/database/alembic/script.py.mako
 api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
+api_logic_server_cli/project_prototype/devops/.DS_Store
 api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
-api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
-api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
-api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
-api_logic_server_cli/project_prototype/devops/docker/build_image.sh
+api_logic_server_cli/project_prototype/devops/auth-db/authdb_mysql.Dockerfile
+api_logic_server_cli/project_prototype/devops/auth-db/authdb_mysql.sql
+api_logic_server_cli/project_prototype/devops/auth-db/authdb_postgres.sql
+api_logic_server_cli/project_prototype/devops/docker-compose/.DS_Store
+api_logic_server_cli/project_prototype/devops/docker-compose/Dockerfile.dockerfile
+api_logic_server_cli/project_prototype/devops/docker-compose/docker-compose.ps1
+api_logic_server_cli/project_prototype/devops/docker-compose/docker-compose.sh
+api_logic_server_cli/project_prototype/devops/docker-compose/docker-compose.yml
+api_logic_server_cli/project_prototype/devops/docker-compose/env-docker-compose.env
+api_logic_server_cli/project_prototype/devops/docker-compose/install-webapp.sh
+api_logic_server_cli/project_prototype/devops/docker-compose/readme-docker-compose.md
+api_logic_server_cli/project_prototype/devops/docker-compose/etc/nginx.conf
+api_logic_server_cli/project_prototype/devops/docker-compose/etc/ssl/certs/example.com.crt
+api_logic_server_cli/project_prototype/devops/docker-compose/etc/ssl/private/example.com.key
+api_logic_server_cli/project_prototype/devops/docker-compose/unused/unused-docker-compose.py
+api_logic_server_cli/project_prototype/devops/docker-compose/unused/unused-get_ip.py
+api_logic_server_cli/project_prototype/devops/docker-compose/unused/unused-requirements-slim.txt
+api_logic_server_cli/project_prototype/devops/docker-image/.DS_Store
+api_logic_server_cli/project_prototype/devops/docker-image/build_image.dockerfile
+api_logic_server_cli/project_prototype/devops/docker-image/build_image.sh
+api_logic_server_cli/project_prototype/devops/docker-image/env.list
+api_logic_server_cli/project_prototype/devops/docker-image/run_image.sh
 api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py
 api_logic_server_cli/project_prototype/logic/declare_logic.py
 api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
 api_logic_server_cli/project_prototype/security/__init__.py
 api_logic_server_cli/project_prototype/security/declare_security.py
 api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
 api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
```

### Comparing `ApiLogicServer-9.1.0/ApiLogicServer.egg-info/requires.txt` & `ApiLogicServer-9.1.32/ApiLogicServer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/LICENSE` & `ApiLogicServer-9.1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/MANIFEST.in` & `ApiLogicServer-9.1.32/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/PKG-INFO` & `ApiLogicServer-9.1.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 9.1.0
+Version: 9.1.32
 Summary: Create JSON:API and Admin Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/ApiLogicServer/ApiLogicServer-src
 Author: Val Huber
 Author-email: apilogicserver@gmail.com
 License: BSD
 Project-URL: Docs, https://apilogicserver.github.io/Docs/
 Platform: any
```

### Comparing `ApiLogicServer-9.1.0/README.md` & `ApiLogicServer-9.1.32/README.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/api_logic_server.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/api_logic_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,18 @@
         * api/expose_api_models.py for a safrs api  - using introspected models.py
     * Special provisions for NW Sample, to show customizations.
     * See end for key_module_map() quick links
 
 Called from api_logic_server_cli.py, by instantiating the ProjectRun object.
 '''
 
-__version__ = "09.01.00"
+__version__ = "09.01.32"
 recent_changes = \
     f'\n\nRecent Changes:\n' +\
+    "\t08/04/2023 - 09.01.32: Issue 01 - arch-based .devcontainer, behave msgs, win rpt, env objs > config w/ home, dockerbldx m1, client_uri \n"\
     "\t07/04/2023 - 09.01.00: SQLAlchemy 2 typed-relns/attrs, Docker: Python 3.11.4 & odbc18 \n"\
     "\t06/24/2023 - 09.00.01: PyMysql \n"\
     "\t06/22/2023 - 09.00.00: Optimistic Locking, safrs 310, SQLAlchemy 2.0.15 \n"\
     "\t05/01/2023 - 08.03.06: allocation sample \n"\
     "\t04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, readme updates, LogicBank 1.8.4 \n"\
     "\t04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65) \n"\
     "\t04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships \n"\
@@ -54,14 +55,15 @@
 import importlib.util
 from flask import Flask
 import logging, logging.config
 import datetime
 from typing import NewType
 import sys
 import os
+import platform
 import importlib
 
 
 def is_docker() -> bool:
     """ running docker?  dir exists: /home/api_logic_server """
     path = '/home/api_logic_server'
     path_result = os.path.isdir(path)  # this *should* exist only on docker
@@ -337,23 +339,22 @@
                             in_file=f'{project.project_directory}/readme.md')
         create_utils.replace_string_in_file(search_for="replace_opt_locking",
                             replace_with=f'{project.opt_locking}',
                             in_file=f'{project.project_directory}/config.py')
         create_utils.replace_string_in_file(search_for="replace_opt_locking_attr",
                             replace_with=f'{project.opt_locking_attr}',
                             in_file=f'{project.project_directory}/api/system/opt_locking/opt_locking.py')
-
-        do_fix_docker_for_vscode_dockerfile = True
-        """
+        do_fix_docker_for_vscode_dockerfile = False  # not required - multi-arch docker
         if do_fix_docker_for_vscode_dockerfile:
-            if arch.get_platform():
+            # print(f'\n> Created for platform.machine(): {platform.machine()}\n')
+            if platform.machine() in('arm64', 'aarch64'):  #  in ("i386", "AMD64", "x86_64")
+                log.debug(f'\n>> .. arm - {platform.machine()}\n')
                 create_utils.replace_string_in_file(search_for="apilogicserver/api_logic_server",
-                                    replace_with=f'apilogicserver/arm-slim',
-                                    in_file=f'{project_directory}/For_VSCode.dockerfile')
-        """
+                                    replace_with=f'apilogicserver/api_logic_server_arm',
+                                    in_file=f'{project.project_directory}/.devcontainer/For_VSCode.dockerfile')
 
         return_abs_db_url = project.abs_db_url
         copy_sqlite = True
         if copy_sqlite == False or "sqlite" not in project.abs_db_url:
             db_uri = get_windows_path_with_slashes(project.abs_db_url)
             create_utils.replace_string_in_file(search_for="replace_db_url",
                                 replace_with=db_uri,
@@ -489,15 +490,15 @@
         log.debug(f' b.   Update api_logic_server_run.py with '
               f'project_name={project.project_name} and api_name, host, port')
         
         update_api_logic_server_run(project)
 
         fix_host_and_ports(" c.   Fixing api/expose_services - port, host", project)
 
-        fix_build_docker_image(" d.   Fixing devops/docker/build_image.sh - project name", project)
+        fix_build_docker_image(" d.   Fixing devops/docker-image/build_image.sh - project name", project)
 
         api_logic_server_info_file_dict["last_created_project_name"] = project.project_directory  # project_name - twiddle
         api_logic_server_info_file_dict["last_created_date"] = str(datetime.datetime.now().strftime("%B %d, %Y %H:%M:%S"))
         api_logic_server_info_file_dict["last_created_version"] = __version__
         with open(api_logic_server_info_file_name, 'w') as api_logic_server_info_file_file:
             yaml.dump(api_logic_server_info_file_dict, api_logic_server_info_file_file, default_flow_style=False)
     return
@@ -510,19 +511,20 @@
     models_file = open(models_file_name, 'a')
     models_file.write("\n\nfrom database import customize_models\n")
     models_file.close()
 
 
 def update_api_logic_server_run(project):
     """
-    Updates project_name, ApiLogicServer hello, project_dir in api_logic_server_run_py
+    Updates project_name, ApiLogicServer hello, project_dir in config.py
 
     Note project_directory is from user, and may be relative (and same as project_name)
     """
     api_logic_server_run_py = f'{project.project_directory}/api_logic_server_run.py'
+    config_py = f'{project.project_directory}/config.py'
     create_utils.replace_string_in_file(search_for="\"api_logic_server_project_name\"",  # fix logic_bank_utils.add_python_path
                            replace_with='"' + os.path.basename(project.project_name) + '"',
                            in_file=api_logic_server_run_py)
     create_utils.replace_string_in_file(search_for="ApiLogicServer hello",
                            replace_with="ApiLogicServer generated at:" +
                                         str(datetime.datetime.now().strftime("%B %d, %Y %H:%M:%S")),
                            in_file=api_logic_server_run_py)
@@ -533,30 +535,37 @@
                            replace_with='"' + project_directory_fix + '"',
                            in_file=api_logic_server_run_py)
     create_utils.replace_string_in_file(search_for="api_logic_server_api_name",  # last node of server url
                            replace_with=project.api_name,
                            in_file=api_logic_server_run_py)
     create_utils.replace_string_in_file(search_for="api_logic_server_host",
                            replace_with=project.host,
-                           in_file=api_logic_server_run_py)
+                           in_file=config_py)
     create_utils.replace_string_in_file(search_for="api_logic_server_swagger_host",
                            replace_with=project.swagger_host,
-                           in_file=api_logic_server_run_py)
+                           in_file=config_py)
     replace_port = f', port="{project.port}"' if project.port else ""  # TODO: consider reverse proxy
 
     create_utils.replace_string_in_file(search_for="api_logic_server_version",
                            replace_with=__version__,
                            in_file=api_logic_server_run_py)
 
     create_utils.replace_string_in_file(search_for="api_logic_server_created_on",
                            replace_with=str(datetime.datetime.now().strftime("%B %d, %Y %H:%M:%S")),
                            in_file=api_logic_server_run_py)
 
     create_utils.replace_string_in_file(search_for="api_logic_server_port",   # server port
                            replace_with=project.port,
+                           in_file=config_py)
+
+    create_utils.replace_string_in_file(search_for="api_logic_server_port",   # server port
+                           replace_with=project.port,
+                           in_file=api_logic_server_run_py)
+    create_utils.replace_string_in_file(search_for="api_logic_server_host",
+                           replace_with=project.host,
                            in_file=api_logic_server_run_py)
     pass
 
 
 def fix_host_and_ports(msg, project):
     """ c.   Fixing api/expose_services - port, host """
     log.debug(msg)  # c.   Fixing api/expose_services - port, host
@@ -574,19 +583,23 @@
     create_utils.replace_string_in_file(search_for="python_anywhere_path",
                            replace_with=full_path,
                            in_file=f'{project.project_directory}/devops/python-anywhere/python_anywhere_wsgi.py')
     log.debug(f' e.   Updated python_anywhere_wsgi.py with {full_path}')
 
 
 def fix_build_docker_image(msg, project: Project):
-    """  d.   Fixing devops/docker/build_image.sh - project name """
-    log.debug(msg)  #  d.   Fixing devops/docker/build_image.sh - project name
+    """  d.   Fixing devops/docker-image/build_image.sh - project name """
+    log.debug(msg)  #  d.   Fixing devops/docker-image/build_image.sh - project name
     replace_port = f':{project.port}' if project.port else ""
     # replace_with = host + replace_port
-    in_file = f'{project.project_directory}/devops/docker/build_image.sh'
+    in_file = f'{project.project_directory}/devops/docker-image/build_image.sh'
+    create_utils.replace_string_in_file(search_for="apilogicserver_project_name_lower",
+                           replace_with=project.project_name_last_node.lower(),
+                           in_file=in_file)
+    in_file = f'{project.project_directory}/devops/docker-image/run_image.sh'
     create_utils.replace_string_in_file(search_for="apilogicserver_project_name_lower",
                            replace_with=project.project_name_last_node.lower(),
                            in_file=in_file)
 
 
 def start_open_with(open_with: str, project_name: str):
     """ Creation complete.  Opening {open_with} at {project_name} """
@@ -683,17 +696,14 @@
         self.infer_primary_key = infer_primary_key
         self.bind_key_url_separator = bind_key_url_separator
         self.command = command
         self.opt_locking = opt_locking
         self.opt_locking_attr = opt_locking_attr
         self.id_column_alias = id_column_alias
 
-        name_nodes = self.project_name.split("/") # type: str
-        self.project_name_last_node = name_nodes[len(name_nodes) - 1]
-
         if execute:
             self.create_project()
 
 
     def print_options(self):
         """ Creating ApiLogicProject with options: (or uri helo) """
         if self.db_url == "?":
@@ -855,41 +865,44 @@
             log.debug(f'.. ..Updated database/multi_db.py with {CONFIG_URI}...')
         else:
             log.debug(f'.. ..Not updating database/multi_db.py with {CONFIG_URI} (already present)')
 
         return return_abs_db_url
 
 
-    def add_sqlite_security(self, msg: str, is_nw: bool = False):
+    def add_auth(self, msg: str, is_nw: bool = False):
         """_summary_
 
-        1. add-db --db_url=auth
+        1. add-db --db_url= [ auth | db_url ]
 
         2. add user.login endpoint
 
         3. Set SECURITY_ENABLED in config.py
 
-        4. Adding Sample authorization to security/declare_security.py, or user TODO
+        4. Adding Sample authorization to security/declare_security.py, or user
 
         Args:
             msg (str): eg: ApiLogicProject customizable project created.  Adding Security:")
             is_nw (bool): is northwind, which means we add the nw security logic
         """
 
+        database_path = self.project_directory_path.joinpath("database")
         log.debug("\n\n==================================================================")
         if msg != "":
-            log.info(msg)
+            log.info(msg + f" to project: {str(database_path.parent)}")
             log.info("  1. ApiLogicServer add-db --db_url=auth --bind_key=authentication")
         log.debug("==================================================================5\n")
         save_run = self.run
         save_command = self.command
         save_db_url = self.db_url
         self.command = "add_db"
         self.bind_key = "authentication"
-        self.db_url = "auth"  # shorthand for api_logic_server_cli/database/auth...
+        is_northwind = is_nw or self.nw_db_status ==  "nw"  # nw_db_status altered in create_project
+        if is_northwind:  # is_nw or self.nw_db_status ==  "nw":
+            self.db_url = "auth"  # shorthand for api_logic_server_cli/database/auth...
         self.run = False
         self.create_project()  # not creating project, but using model creation svcs
         self.run = save_run
         self.command = save_command
         self.db_url = save_db_url
         
         log.debug("\n==================================================================")
@@ -915,45 +928,47 @@
         log.debug("\n==================================================================")
         if msg != "":
             log.info("  3. Set SECURITY_ENABLED in config.py")
         log.debug("==================================================================\n")
         create_utils.replace_string_in_file(search_for="SECURITY_ENABLED = False  #",
                             replace_with='SECURITY_ENABLED = True  #',
                             in_file=f'{self.project_directory}/config.py')
-        if is_nw:
+        if is_northwind:  # is_nw or self.nw_db_status ==  "nw":
             log.debug("\n==================================================================")
-        if msg != "":
             if msg != "":
-                log.info("  4. Adding Sample authorization to security/declare_security.py")
-            log.debug("==================================================================\n\n")
-            nw_declare_security_py_path = self.api_logic_server_dir_path.\
-                joinpath('project_prototype_nw/security/declare_security.py')
-            declare_security_py_path = self.project_directory_path.joinpath('security/declare_security.py')
-            shutil.copyfile(nw_declare_security_py_path, declare_security_py_path)
+                if msg != "":
+                    log.info("  4. Adding Sample authorization to security/declare_security.py")
+                log.debug("==================================================================\n\n")
+                nw_declare_security_py_path = self.api_logic_server_dir_path.\
+                    joinpath('project_prototype_nw/security/declare_security.py')
+                declare_security_py_path = self.project_directory_path.joinpath('security/declare_security.py')
+                shutil.copyfile(nw_declare_security_py_path, declare_security_py_path)
         else:
             log.debug("\n==================================================================")
             if msg != "":
                 log.info("  4. TODO: Declare authorization in security/declare_security.py")
             log.debug("==================================================================\n\n")
 
 
-    def add_nw_customizations(self, do_show_messages: bool = True):
+    def add_nw_customizations(self, do_show_messages: bool = True, do_security: bool = True):
         """_summary_
 
         1. add-sqlite-security
 
-        2. deep copy project_prototype_nw
+        2. deep copy project_prototype_nw (adds logic)
 
         Args:
         """
+
         log.debug("\n\n==================================================================")
         nw_messages = ""
-        if do_show_messages:
-            nw_messages = "Add northwind customizations - enabling security"
-        self.add_sqlite_security(is_nw=True, msg=nw_messages)
+        if do_security:
+            if do_show_messages:
+                nw_messages = "Add northwind customizations - enabling security"
+            self.add_auth(is_nw=True, msg=nw_messages)
 
         nw_path = (self.api_logic_server_dir_path).\
             joinpath('project_prototype_nw')  # /Users/val/dev/ApiLogicServer/api_logic_server_cli/project_prototype
         recursive_overwrite(nw_path, self.project_directory)
 
         create_nw_tutorial(self.project_directory, str(self.api_logic_server_dir_path))
 
@@ -1011,15 +1026,15 @@
         with_cust = str(target_project_path.joinpath(f"{create}/2. Customized"))
         shutil.copytree(dirs_exist_ok=True,
             src=no_cust,
             dst=with_cust)
         
         self.project_name = with_cust
         self.command = "add-cust"
-        self.add_nw_customizations(do_show_messages=False)
+        self.add_nw_customizations(do_show_messages=False, do_security=False)
         self.run = save_run
 
         log.info(f"\nCreating Logic\n")
         no_cust = self.project_name
         with_cust = str(target_project_path.joinpath(f"{create}/3. Logic"))
         shutil.copytree(dirs_exist_ok=True,
             src=no_cust,
@@ -1035,17 +1050,17 @@
             shutil.rmtree(str(target_project_path.joinpath(f"{create}/1. Instant_Creation")))
             shutil.rmtree(str(target_project_path.joinpath(f"{create}/2. Customized")))
             if os.path.isdir(target_project_path.joinpath(f"{create}/2. Learn JSON_API using API Logic Server")):
                 shutil.rmtree(str(target_project_path.joinpath(f"{create}/2. Learn JSON_API using API Logic Server")))
             shutil.move(src = str(target_project_path.joinpath(f"{create}/3. Logic")),
                         dst = str(target_project_path.joinpath(f"{create}/2. Learn JSON_API using API Logic Server")))
         else:
-            # remove logic and database customizations from "2. Customized"
-            shutil.rmtree(str(target_project_path.joinpath(f"{create}/2. Customized/logic")))
-            shutil.rmtree(str(target_project_path.joinpath(f"{create}/2. Customized/database")))
+            # remove logic and database customizations from "2. Customized" (win requires: ignore_errors=True)
+            shutil.rmtree(str(target_project_path.joinpath(f"{create}/2. Customized/logic")), ignore_errors=True)
+            shutil.rmtree(str(target_project_path.joinpath(f"{create}/2. Customized/database")), ignore_errors=True)
             shutil.copytree(dirs_exist_ok=True,
                 src=str(target_project_path.joinpath(f"{create}/1. Instant_Creation/logic")),
                 dst=str(target_project_path.joinpath(f"{create}/2. Customized/logic")))
             shutil.copytree(dirs_exist_ok=True,
                 src=str(target_project_path.joinpath(f"{create}/1. Instant_Creation/database")),
                 dst=str(target_project_path.joinpath(f"{create}/2. Customized/database")))
             create_utils.replace_string_in_file(search_for="SECURITY_ENABLED = True",
@@ -1087,14 +1102,18 @@
             log.debug(f'0. Using default extended_builder: {self.extended_builder}')
 
         self.project_directory, self.api_name, self.merge_into_prototype = \
             create_utils.get_project_directory_and_api_name(self)
         self.project_directory_actual = os.path.abspath(self.project_directory)  # make path absolute, not relative (no /../)
         self.project_directory_path = Path(self.project_directory_actual)
 
+        name_nodes = self.project_directory_actual.split("/") # type: str
+        self.project_name_last_node = name_nodes[len(name_nodes) - 1]  # for prototype, project_name='.'
+
+
         if self.command.startswith("rebuild") or self.command == "add_db":
             log.debug("1. Not Deleting Existing Project")
             log.debug("2. Using Existing Project")
             if self.command == "add_db":
                 self.abs_db_url = self.update_config_and_copy_sqlite_db(
                     f".. ..Adding Database [{self.bind_key}] to existing project")
         else:                                                                            # normal path - clone, [overlay nw]
@@ -1111,15 +1130,15 @@
 
         final_project_fixup("4. Final project fixup", self)
 
         if self.open_with != "":  # open project with open_with (vscode, charm, atom) -- NOT for docker!!
             start_open_with(open_with=self.open_with, project_name=self.project_name)
 
         if self.nw_db_status in ["nw", "nw+"] and self.command != "add_db":
-            self.add_sqlite_security("\nApiLogicProject customizable project created.  Adding Security:")
+            self.add_auth("\nApiLogicProject customizable project created.  Adding Security:")
             
         if self.command.startswith("add_"):
             pass  # keep silent for add-db, add-auth...
         elif self.is_tutorial:
             log.debug(f"\nTutorial created.  Next steps:\n")
             log.debug(f'  Establish your Python environment - see https://apilogicserver.github.io/Docs/IDE-Execute/#execute-prebuilt-launch-configurations\n')
         else:
@@ -1214,9 +1233,9 @@
         sqlacodegen_wrapper.create_models_py({})            # creates models.py via *sqlacodegen*
         sqlacodegen_wrapper.CodeGenerator.render_class()    # sqlacodegen - creates models_py as string
         model_creation_services.create_resource_list()      # creates resource_list via *dynamic import* of models.py
     invoke_creators(model_creation_services)                # creates api & ui, via create_from_model...
     api_expose_api_models_creator.create()                  # creates api/expose_api_models.py, key input to SAFRS        
     ui_admin_creator.create()                               # creates ui/admin/admin.yaml from resource_list
     ProjectRun.update_config_and_copy_sqlite_db()           # adds db (model, binds, api, app) to curr project
-    ProjectRun.add_sqlite_security()                        # add_db(auth), adds nw declare_security, upd config
+    ProjectRun.add_auth()                                   # add_db(auth), adds nw declare_security, upd config
     ProjectRun.tutorial()                                   # creates basic, nw, nw + cust
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/cli.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 # print("sys.path.append(get_api_logic_server_dir())\n",get_api_logic_server_dir())
 sys.path.append(get_api_logic_server_dir())  # e.g, on Docker: export PATH="/home/api_logic_server/api_logic_server_cli"
 api_logic_server_path = os.path.dirname(get_api_logic_server_dir())  # e.g: export PATH="/home/api_logic_server"
 sys.path.append(api_logic_server_path)
 from create_from_model.model_creation_services import ModelCreationServices
 import create_from_model.api_logic_server_utils as create_utils
 import api_logic_server_cli.create_from_model.uri_info as uri_info
-import api_logic_server_cli.api_logic_server as PR  # ProjectRun (main class)
+import api_logic_server_cli.api_logic_server as PR
+''' ProjectRun (main class) '''
 from api_logic_server_cli.cli_args_base import OptLocking
 
 api_logic_server_info_file_name = get_api_logic_server_dir() + "/api_logic_server_info.yaml"
 
 api_logic_server_info_file_dict = {}  # last-run (debug, etc) info
 """ contains last-run info, debug switches to show args, etc """
 
@@ -591,36 +592,39 @@
 @main.command("add-auth") 
 @click.option('--bind_key_url_separator',
               default=default_bind_key_url_separator,
               help="bindkey / class name url separator")
 @click.option('--project_name',
               default=f'',
               help="Project location")
+@click.option('--db_url',
+              default=f'auth',
+              prompt="SQLAlchemy Database URI",
+              help="SQLAlchemy Database URL - see above\n")
 @click.option('--api_name',
               default="api",
               help="api prefix name")
 @click.pass_context
-def add_security_cmd(ctx, bind_key_url_separator: str, api_name: str, project_name: str):
+def add_auth_cmd(ctx, bind_key_url_separator: str, db_url: str, project_name: str, api_name: str):
     """
     Adds authorization/authentication to curr project.
     
     example: 
 
     cd existing_project
 
-    ApiLogicServer add-auth
+    ApiLogicServer add-auth project_name=.
     
     """
     if project_name == "":
         project_name=os.getcwd()
         if project_name == get_api_logic_server_dir():  # for ApiLogicServer dev (from |> Run and Debug )
             project_name = str(
                 Path(project_name).parent.parent.joinpath("servers").joinpath("ApiLogicProject")
             )
-    db_url = "auth"
     bind_key = "authentication"
     project = PR.ProjectRun(command="add_security", 
               project_name=project_name, 
               api_name=api_name, 
               db_url=db_url, 
               bind_key=bind_key,
               bind_key_url_separator=bind_key_url_separator,
@@ -628,18 +632,22 @@
               )
     project.project_directory, project.api_name, project.merge_into_prototype = \
         create_utils.get_project_directory_and_api_name(project)
     project.project_directory_actual = os.path.abspath(project.project_directory)  # make path absolute, not relative (no /../)
     project.project_directory_path = Path(project.project_directory_actual)
     models_py_path = project.project_directory_path.joinpath('database/models.py')
     project.abs_db_url, project.nw_db_status, project.model_file_name = create_utils.get_abs_db_url("0. Using Sample DB", project)
+    if not models_py_path.exists():
+        log.info(f'... Error - does not appear to be a project: {str(project.project_directory_path)}')
+        log.info(f'... Typical usage - cd into project, use --project_name=. \n')
+        exit (1)
     is_nw = False
     if create_utils.does_file_contain(search_for="CategoryTableNameTest", in_file=models_py_path):
         is_nw = True
-    project.add_sqlite_security(msg="Adding Security", is_nw=is_nw)
+    project.add_auth(msg="Adding Security", is_nw=is_nw)
     log.info("")
 
 
 @main.command("add-cust") 
 @click.option('--bind_key_url_separator',
               default=default_bind_key_url_separator,
               help="bindkey / class name url separator")
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/cli_args_base.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/cli_args_base.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/cli_args_project.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/cli_args_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.default_fab_host = "localhost"
         self.default_bind_key_url_separator = "-"  # admin 
         self.is_tutorial = False
 
         self.project_name_last_node = "TBD"
 
         running_at = Path(__file__)
-        self.api_logic_server_dir_path = running_at.parent.absolute()  # ne abspath(f'{abspath(get_api_logic_server_dir())}'))
+        self.api_logic_server_dir_path = running_at.parent.absolute()  # no abspath(f'{abspath(get_api_logic_server_dir())}'))
 
         self.is_codespaces = os.getenv('CODESPACES')
 
 
     def print_options(self):
         """ Creating ApiLogicServer with options: (or uri helo) """
         if self.db_url == "?":  # can only test interactively, not from launch
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1809a364 (Mon Jul  3 17:44:56 2023 UTC)
-files sz: 12877
+moddate:  0x38d6ca64 (Wed Aug  2 22:18:32 2023 UTC)
+files sz: 12990
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -124,32 +124,32 @@
                202 LOAD_CONST              21 ('after')
                204 LOAD_NAME               18 (bool)
                206 BUILD_TUPLE              8
                208 LOAD_CONST              22 (<code object insert_lines_at, file "/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 182>)
                210 MAKE_FUNCTION            5 (defaults, annotations)
                212 STORE_NAME              21 (insert_lines_at)
    
-   202         214 LOAD_CONST               6 ('return')
+   204         214 LOAD_CONST               6 ('return')
                216 LOAD_NAME               13 (str)
                218 BUILD_TUPLE              2
-               220 LOAD_CONST              23 (<code object find_valid_python_name, file "/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 202>)
+               220 LOAD_CONST              23 (<code object find_valid_python_name, file "/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 204>)
                222 MAKE_FUNCTION            4 (annotations)
                224 STORE_NAME              22 (find_valid_python_name)
    
-   224         226 LOAD_CONST              30 ((None, '', False))
+   226         226 LOAD_CONST              30 ((None, '', False))
                228 LOAD_CONST              25 ('cmd')
                230 LOAD_NAME               13 (str)
                232 LOAD_CONST              26 ('msg')
                234 LOAD_NAME               13 (str)
                236 LOAD_CONST              27 ('new_line')
                238 LOAD_NAME               18 (bool)
                240 LOAD_CONST               6 ('return')
                242 LOAD_NAME               13 (str)
                244 BUILD_TUPLE              8
-               246 LOAD_CONST              28 (<code object run_command, file "/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 224>)
+               246 LOAD_CONST              28 (<code object run_command, file "/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py", line 226>)
                248 MAKE_FUNCTION            5 (defaults, annotations)
                250 STORE_NAME              23 (run_command)
                252 LOAD_CONST               1 (None)
                254 RETURN_VALUE
    consts
       0
       None
@@ -309,15 +309,15 @@
                      328 STORE_FAST               1 (rtn_project_directory)
          
           53         330 LOAD_CONST              10 (' <dev>')
                      332 STORE_FAST               4 (msg)
          
           54     >>  334 LOAD_GLOBAL             16 (log)
                      346 LOAD_METHOD              9 (debug)
-                     368 LOAD_CONST              11 ('1. Merge into project prototype: ')
+                     368 LOAD_CONST              11 ('1. Merge into project prototype / current project: ')
                      370 LOAD_FAST                1 (rtn_project_directory)
                      372 FORMAT_VALUE             0
                      374 LOAD_FAST                4 (msg)
                      376 FORMAT_VALUE             0
                      378 BUILD_STRING             3
                      380 PRECALL                  1
                      384 CALL                     1
@@ -363,15 +363,15 @@
             None
             '.'
             './'
             True
             ''
             'ApiLogicProject'
             ' <dev>'
-            '1. Merge into project prototype: '
+            '1. Merge into project prototype / current project: '
             -1
          names      ('project_name', 'api_name', 'startswith', 'str', 'Path', 'home', 'os_cwd', 'get_api_logic_server_dir', 'log', 'debug', 'parts', 'multi_api')
          varnames   ('project', 'rtn_project_directory', 'rtn_api_name', 'rtn_merge_into_prototype', 'msg', 'project_path', 'project_path_last_node')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'get_project_directory_and_api_name'
@@ -1280,29 +1280,30 @@
       'lines'
       'at'
       'file_name'
       'after'
       code
          argcount  : 4
          nlocals   : 9
-         stacksize : 6
+         stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000007c026401a6020000ab020000000000
             00000035007d047c04a00100000000000000000000000000000000000000
             00a6000000ab0000000000000000007d0564027d0664037d077c0544005d
             0f7d087c017c087600720464047d0601006e067c0764057a0d00007d078c
-            107c06731274050000000000000000000064067c019b009d02a6010000ab
-            01000000000000000082017c0372057c0764057a0000007d077c05a00300
-            000000000000000000000000000000000000007c077c00a6020000ab0200
-            0000000000000001007c04a0040000000000000000000000000000000000
-            0000006403a6010000ab01000000000000000001007c04a0050000000000
-            0000000000000000000000000000007c05a6010000ab0100000000000000
-            000100640764076407a6020000ab02000000000000000001006407530023
-            00310073047702780359007701010059000100010064075300
+            107c06731574050000000000000000000064067c019b0064077c029b009d
+            04a6010000ab01000000000000000082017c0372057c0764057a0000007d
+            077c05a00300000000000000000000000000000000000000007c077c00a6
+            020000ab02000000000000000001007c04a0040000000000000000000000
+            0000000000000000006403a6010000ab01000000000000000001007c04a0
+            0500000000000000000000000000000000000000007c05a6010000ab0100
+            000000000000000100640864086408a6020000ab02000000000000000001
+            006408530023003100730477027803590077010100590001000100640853
+            00
          182           0 RESUME                   0
          
          184           2 LOAD_GLOBAL              1 (NULL + open)
                       14 LOAD_FAST                2 (file_name)
                       16 LOAD_CONST               1 ('r+')
                       18 PRECALL                  2
                       22 CALL                     2
@@ -1340,99 +1341,107 @@
          192     >>  108 LOAD_FAST                7 (insert_line)
                      110 LOAD_CONST               5 (1)
                      112 BINARY_OP               13 (+=)
                      116 STORE_FAST               7 (insert_line)
                      118 JUMP_BACKWARD           16 (to 88)
          
          193     >>  120 LOAD_FAST                6 (found)
-                     122 POP_JUMP_FORWARD_IF_TRUE    18 (to 160)
+                     122 POP_JUMP_FORWARD_IF_TRUE    21 (to 166)
          
          194         124 LOAD_GLOBAL              5 (NULL + Exception)
-                     136 LOAD_CONST               6 ('Internal error - unable to find insert: ')
-                     138 LOAD_FAST                1 (at)
-                     140 FORMAT_VALUE             0
-                     142 BUILD_STRING             2
-                     144 PRECALL                  1
-                     148 CALL                     1
-                     158 RAISE_VARARGS            1
-         
-         195     >>  160 LOAD_FAST                3 (after)
-                     162 POP_JUMP_FORWARD_IF_FALSE     5 (to 174)
-         
-         196         164 LOAD_FAST                7 (insert_line)
-                     166 LOAD_CONST               5 (1)
-                     168 BINARY_OP                0 (+)
-                     172 STORE_FAST               7 (insert_line)
-         
-         197     >>  174 LOAD_FAST                5 (file_lines)
-                     176 LOAD_METHOD              3 (insert)
-                     198 LOAD_FAST                7 (insert_line)
-                     200 LOAD_FAST                0 (lines)
-                     202 PRECALL                  2
-                     206 CALL                     2
-                     216 POP_TOP
-         
-         198         218 LOAD_FAST                4 (fp)
-                     220 LOAD_METHOD              4 (seek)
-                     242 LOAD_CONST               3 (0)
-                     244 PRECALL                  1
-                     248 CALL                     1
-                     258 POP_TOP
-         
-         199         260 LOAD_FAST                4 (fp)
-                     262 LOAD_METHOD              5 (writelines)
-                     284 LOAD_FAST                5 (file_lines)
-                     286 PRECALL                  1
-                     290 CALL                     1
-                     300 POP_TOP
-         
-         184         302 LOAD_CONST               7 (None)
-                     304 LOAD_CONST               7 (None)
-                     306 LOAD_CONST               7 (None)
-                     308 PRECALL                  2
-                     312 CALL                     2
-                     322 POP_TOP
-                     324 LOAD_CONST               7 (None)
-                     326 RETURN_VALUE
-                 >>  328 PUSH_EXC_INFO
-                     330 WITH_EXCEPT_START
-                     332 POP_JUMP_FORWARD_IF_TRUE     4 (to 342)
-                     334 RERAISE                  2
-                 >>  336 COPY                     3
-                     338 POP_EXCEPT
-                     340 RERAISE                  1
-                 >>  342 POP_TOP
+                     136 LOAD_CONST               6 ('Internal error - unable to find insert:\n.. seeking ')
+         
+         195         138 LOAD_FAST                1 (at)
+         
+         194         140 FORMAT_VALUE             0
+                     142 LOAD_CONST               7 ('\n.. in ')
+         
+         196         144 LOAD_FAST                2 (file_name)
+         
+         194         146 FORMAT_VALUE             0
+                     148 BUILD_STRING             4
+                     150 PRECALL                  1
+                     154 CALL                     1
+                     164 RAISE_VARARGS            1
+         
+         197     >>  166 LOAD_FAST                3 (after)
+                     168 POP_JUMP_FORWARD_IF_FALSE     5 (to 180)
+         
+         198         170 LOAD_FAST                7 (insert_line)
+                     172 LOAD_CONST               5 (1)
+                     174 BINARY_OP                0 (+)
+                     178 STORE_FAST               7 (insert_line)
+         
+         199     >>  180 LOAD_FAST                5 (file_lines)
+                     182 LOAD_METHOD              3 (insert)
+                     204 LOAD_FAST                7 (insert_line)
+                     206 LOAD_FAST                0 (lines)
+                     208 PRECALL                  2
+                     212 CALL                     2
+                     222 POP_TOP
+         
+         200         224 LOAD_FAST                4 (fp)
+                     226 LOAD_METHOD              4 (seek)
+                     248 LOAD_CONST               3 (0)
+                     250 PRECALL                  1
+                     254 CALL                     1
+                     264 POP_TOP
+         
+         201         266 LOAD_FAST                4 (fp)
+                     268 LOAD_METHOD              5 (writelines)
+                     290 LOAD_FAST                5 (file_lines)
+                     292 PRECALL                  1
+                     296 CALL                     1
+                     306 POP_TOP
+         
+         184         308 LOAD_CONST               8 (None)
+                     310 LOAD_CONST               8 (None)
+                     312 LOAD_CONST               8 (None)
+                     314 PRECALL                  2
+                     318 CALL                     2
+                     328 POP_TOP
+                     330 LOAD_CONST               8 (None)
+                     332 RETURN_VALUE
+                 >>  334 PUSH_EXC_INFO
+                     336 WITH_EXCEPT_START
+                     338 POP_JUMP_FORWARD_IF_TRUE     4 (to 348)
+                     340 RERAISE                  2
+                 >>  342 COPY                     3
                      344 POP_EXCEPT
-                     346 POP_TOP
-                     348 POP_TOP
-                     350 LOAD_CONST               7 (None)
-                     352 RETURN_VALUE
+                     346 RERAISE                  1
+                 >>  348 POP_TOP
+                     350 POP_EXCEPT
+                     352 POP_TOP
+                     354 POP_TOP
+                     356 LOAD_CONST               8 (None)
+                     358 RETURN_VALUE
          ExceptionTable:
-           34 to 300 -> 328 [1] lasti
-           328 to 334 -> 336 [3] lasti
-           342 to 342 -> 336 [3] lasti
+           34 to 306 -> 334 [1] lasti
+           334 to 340 -> 342 [3] lasti
+           348 to 348 -> 342 [3] lasti
          consts
             ' insert <lines> into file_name after line with <str> '
             'r+'
             False
             0
             True
             1
-            'Internal error - unable to find insert: '
+            'Internal error - unable to find insert:\n.. seeking '
+            '\n.. in '
             None
          names      ('open', 'readlines', 'Exception', 'insert', 'seek', 'writelines')
          varnames   ('lines', 'at', 'file_name', 'after', 'fp', 'file_lines', 'found', 'insert_line', 'each_line')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'insert_lines_at'
          firstlineno 182
          lnotab
-            0x0202220128010401040108010801040104010c010401240104010a012c
-            012a012af1
+            0x0202220128010401040108010801040104010c0104010e0102ff040202
+            fe140304010a012c012a012aef
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
             0x970064017d0009007401000000000000000000006a0100000000000000
@@ -1440,103 +1449,103 @@
             030000ab0300000000000000007d016e5723007406000000000000000000
             002400724a7d0264017d0009007401000000000000000000006a01000000
             0000000000640564037400000000000000000000006a0200000000000000
             00ac04a6030000ab0300000000000000007d016e19230074060000000000
             00000000002400720c7d0364017d00590064067d037e036e0864067d037e
             037701770078035900770164037d00590064067d027e026e0864067d027e
             02770177007803590077017c0072026407530064085300
-         202           0 RESUME                   0
+         204           0 RESUME                   0
          
-         208           2 LOAD_CONST               1 (False)
+         210           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               0 (python3_worked)
          
-         209           6 NOP
+         211           6 NOP
          
-         210           8 LOAD_GLOBAL              1 (NULL + subprocess)
+         212           8 LOAD_GLOBAL              1 (NULL + subprocess)
                       20 LOAD_ATTR                1 (check_output)
                       30 LOAD_CONST               2 ('python --version')
                       32 LOAD_CONST               3 (True)
                       34 LOAD_GLOBAL              0 (subprocess)
                       46 LOAD_ATTR                2 (STDOUT)
                       56 KW_NAMES                 4
                       58 PRECALL                  3
                       62 CALL                     3
                       72 STORE_FAST               1 (result_b)
                       74 JUMP_FORWARD            87 (to 250)
                  >>   76 PUSH_EXC_INFO
          
-         211          78 LOAD_GLOBAL              6 (Exception)
+         213          78 LOAD_GLOBAL              6 (Exception)
                       90 CHECK_EXC_MATCH
                       92 POP_JUMP_FORWARD_IF_FALSE    74 (to 242)
                       94 STORE_FAST               2 (e)
          
-         212          96 LOAD_CONST               1 (False)
+         214          96 LOAD_CONST               1 (False)
                       98 STORE_FAST               0 (python3_worked)
          
-         213         100 NOP
+         215         100 NOP
          
-         214         102 LOAD_GLOBAL              1 (NULL + subprocess)
+         216         102 LOAD_GLOBAL              1 (NULL + subprocess)
                      114 LOAD_ATTR                1 (check_output)
                      124 LOAD_CONST               5 ('python3 --version')
                      126 LOAD_CONST               3 (True)
                      128 LOAD_GLOBAL              0 (subprocess)
                      140 LOAD_ATTR                2 (STDOUT)
                      150 KW_NAMES                 4
                      152 PRECALL                  3
                      156 CALL                     3
                      166 STORE_FAST               1 (result_b)
                      168 JUMP_FORWARD            25 (to 220)
                  >>  170 PUSH_EXC_INFO
          
-         215         172 LOAD_GLOBAL              6 (Exception)
+         217         172 LOAD_GLOBAL              6 (Exception)
                      184 CHECK_EXC_MATCH
                      186 POP_JUMP_FORWARD_IF_FALSE    12 (to 212)
                      188 STORE_FAST               3 (e1)
          
-         216         190 LOAD_CONST               1 (False)
+         218         190 LOAD_CONST               1 (False)
                      192 STORE_FAST               0 (python3_worked)
                      194 POP_EXCEPT
                      196 LOAD_CONST               6 (None)
                      198 STORE_FAST               3 (e1)
                      200 DELETE_FAST              3 (e1)
                      202 JUMP_FORWARD             8 (to 220)
                  >>  204 LOAD_CONST               6 (None)
                      206 STORE_FAST               3 (e1)
                      208 DELETE_FAST              3 (e1)
                      210 RERAISE                  1
          
-         215     >>  212 RERAISE                  0
+         217     >>  212 RERAISE                  0
                  >>  214 COPY                     3
                      216 POP_EXCEPT
                      218 RERAISE                  1
          
-         217     >>  220 LOAD_CONST               3 (True)
+         219     >>  220 LOAD_CONST               3 (True)
                      222 STORE_FAST               0 (python3_worked)
                      224 POP_EXCEPT
                      226 LOAD_CONST               6 (None)
                      228 STORE_FAST               2 (e)
                      230 DELETE_FAST              2 (e)
                      232 JUMP_FORWARD             8 (to 250)
                  >>  234 LOAD_CONST               6 (None)
                      236 STORE_FAST               2 (e)
                      238 DELETE_FAST              2 (e)
                      240 RERAISE                  1
          
-         211     >>  242 RERAISE                  0
+         213     >>  242 RERAISE                  0
                  >>  244 COPY                     3
                      246 POP_EXCEPT
                      248 RERAISE                  1
          
-         218     >>  250 LOAD_FAST                0 (python3_worked)
+         220     >>  250 LOAD_FAST                0 (python3_worked)
                      252 POP_JUMP_FORWARD_IF_FALSE     2 (to 258)
          
-         219         254 LOAD_CONST               7 ('python3')
+         221         254 LOAD_CONST               7 ('python3')
                      256 RETURN_VALUE
          
-         221     >>  258 LOAD_CONST               8 ('python')
+         223     >>  258 LOAD_CONST               8 ('python')
                      260 RETURN_VALUE
          ExceptionTable:
            8 to 72 -> 76 [0]
            76 to 94 -> 244 [1] lasti
            96 to 98 -> 234 [1] lasti
            102 to 166 -> 170 [1]
            168 to 168 -> 234 [1] lasti
@@ -1558,15 +1567,15 @@
             'python'
          names      ('subprocess', 'check_output', 'STDOUT', 'Exception')
          varnames   ('python3_worked', 'result_b', 'e', 'e1')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'find_valid_python_name'
-         firstlineno 202
+         firstlineno 204
          lnotab
             0x02060401020146011201040102014601120116ff080216fa0807040104
             02
       ''
       'cmd'
       'msg'
       'new_line'
@@ -1600,204 +1609,204 @@
             00000000007c0ba6010000ab01000000000000000064107a0a0000850219
             0000000000000000007d0b6411741b000000000000000000007c00a60100
             00ab0100000000000000007a0a00007d0c64067c0c7a0500007d0d7c0264
             056b020000000072016e307c0b64026b0300000000722a7c0b64126b0300
             0000007224740600000000000000000000a0040000000000000000000000
             0000000000000000007c059b0064067c009b0064137c0d9b007c0b9b009d
             06a6010000ab01000000000000000001007c0b5300
-         224           0 RESUME                   0
+         226           0 RESUME                   0
          
-         232           2 LOAD_FAST                0 (cmd)
+         234           2 LOAD_FAST                0 (cmd)
                        4 LOAD_METHOD              0 (startswith)
                       26 LOAD_CONST               1 ('python')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 POP_JUMP_FORWARD_IF_FALSE    36 (to 116)
          
-         233          44 LOAD_GLOBAL              3 (NULL + find_valid_python_name)
+         235          44 LOAD_GLOBAL              3 (NULL + find_valid_python_name)
                       56 PRECALL                  0
                       60 CALL                     0
                       70 STORE_FAST               4 (valid_python_name)
          
-         234          72 LOAD_FAST                0 (cmd)
+         236          72 LOAD_FAST                0 (cmd)
                       74 LOAD_METHOD              2 (replace)
                       96 LOAD_CONST               1 ('python')
                       98 LOAD_FAST                4 (valid_python_name)
                      100 PRECALL                  2
                      104 CALL                     2
                      114 STORE_FAST               0 (cmd)
          
-         235     >>  116 LOAD_CONST               2 ('')
+         237     >>  116 LOAD_CONST               2 ('')
                      118 STORE_FAST               5 (log_msg)
          
-         236         120 LOAD_FAST                2 (msg)
+         238         120 LOAD_FAST                2 (msg)
                      122 LOAD_CONST               3 ('Execute command:')
                      124 COMPARE_OP               3 (!=)
                      130 POP_JUMP_FORWARD_IF_FALSE     5 (to 142)
          
-         237         132 LOAD_FAST                2 (msg)
+         239         132 LOAD_FAST                2 (msg)
                      134 LOAD_CONST               4 (' with command:')
                      136 BINARY_OP                0 (+)
                      140 STORE_FAST               5 (log_msg)
          
-         238     >>  142 LOAD_FAST                2 (msg)
+         240     >>  142 LOAD_FAST                2 (msg)
                      144 LOAD_CONST               5 ('no-msg')
                      146 COMPARE_OP               2 (==)
                      152 POP_JUMP_FORWARD_IF_FALSE     3 (to 160)
          
-         239         154 LOAD_CONST               2 ('')
+         241         154 LOAD_CONST               2 ('')
                      156 STORE_FAST               5 (log_msg)
                      158 JUMP_FORWARD            31 (to 222)
          
-         241     >>  160 LOAD_GLOBAL              6 (log)
+         243     >>  160 LOAD_GLOBAL              6 (log)
                      172 LOAD_METHOD              4 (debug)
                      194 LOAD_FAST                5 (log_msg)
                      196 FORMAT_VALUE             0
                      198 LOAD_CONST               6 (' ')
                      200 LOAD_FAST                0 (cmd)
                      202 FORMAT_VALUE             0
                      204 BUILD_STRING             3
                      206 PRECALL                  1
                      210 CALL                     1
                      220 POP_TOP
          
-         242     >>  222 LOAD_FAST                3 (new_line)
+         244     >>  222 LOAD_FAST                3 (new_line)
                      224 POP_JUMP_FORWARD_IF_FALSE    26 (to 278)
          
-         243         226 LOAD_GLOBAL              6 (log)
+         245         226 LOAD_GLOBAL              6 (log)
                      238 LOAD_METHOD              4 (debug)
                      260 LOAD_CONST               2 ('')
                      262 PRECALL                  1
                      266 CALL                     1
                      276 POP_TOP
          
-         245     >>  278 LOAD_FAST                1 (env)
+         247     >>  278 LOAD_FAST                1 (env)
                      280 STORE_FAST               6 (use_env)
          
-         246         282 LOAD_FAST                1 (env)
+         248         282 LOAD_FAST                1 (env)
                      284 POP_JUMP_FORWARD_IF_NOT_NONE   101 (to 488)
          
-         247         286 LOAD_GLOBAL             11 (NULL + get_api_logic_server_dir)
+         249         286 LOAD_GLOBAL             11 (NULL + get_api_logic_server_dir)
                      298 PRECALL                  0
                      302 CALL                     0
                      312 STORE_FAST               7 (project_dir)
          
-         248         314 LOAD_GLOBAL             13 (NULL + str)
+         250         314 LOAD_GLOBAL             13 (NULL + str)
                      326 LOAD_FAST                7 (project_dir)
                      328 PRECALL                  1
                      332 CALL                     1
                      342 LOAD_CONST               8 ('/venv/lib/python3.9/site_packages')
                      344 BINARY_OP                0 (+)
                      348 STORE_FAST               8 (python_path)
          
-         249         350 LOAD_GLOBAL             14 (os)
+         251         350 LOAD_GLOBAL             14 (os)
                      362 LOAD_ATTR                8 (environ)
                      372 LOAD_METHOD              9 (copy)
                      394 PRECALL                  0
                      398 CALL                     0
                      408 STORE_FAST               6 (use_env)
          
-         251         410 LOAD_GLOBAL             21 (NULL + hasattr)
+         253         410 LOAD_GLOBAL             21 (NULL + hasattr)
                      422 LOAD_FAST                6 (use_env)
                      424 LOAD_CONST               9 ('PYTHONPATH')
                      426 PRECALL                  2
                      430 CALL                     2
                      440 POP_JUMP_FORWARD_IF_FALSE    18 (to 478)
          
-         252         442 LOAD_FAST                8 (python_path)
+         254         442 LOAD_FAST                8 (python_path)
                      444 LOAD_CONST              10 (':')
                      446 BINARY_OP                0 (+)
                      450 LOAD_FAST                6 (use_env)
                      452 LOAD_CONST               9 ('PYTHONPATH')
                      454 BINARY_SUBSCR
                      464 BINARY_OP                0 (+)
                      468 LOAD_FAST                6 (use_env)
                      470 LOAD_CONST               9 ('PYTHONPATH')
                      472 STORE_SUBSCR
                      476 JUMP_FORWARD             5 (to 488)
          
-         255     >>  478 LOAD_FAST                8 (python_path)
+         257     >>  478 LOAD_FAST                8 (python_path)
                      480 LOAD_FAST                6 (use_env)
                      482 LOAD_CONST               9 ('PYTHONPATH')
                      484 STORE_SUBSCR
          
-         257     >>  488 LOAD_CONST              11 (False)
+         259     >>  488 LOAD_CONST              11 (False)
                      490 STORE_FAST               9 (use_env_debug)
          
-         258         492 LOAD_FAST                9 (use_env_debug)
+         260         492 LOAD_FAST                9 (use_env_debug)
                      494 POP_JUMP_FORWARD_IF_FALSE    24 (to 544)
          
-         259         496 LOAD_GLOBAL             23 (NULL + subprocess)
+         261         496 LOAD_GLOBAL             23 (NULL + subprocess)
                      508 LOAD_ATTR               12 (check_output)
                      518 LOAD_FAST                0 (cmd)
                      520 LOAD_CONST              12 (True)
                      522 LOAD_FAST                6 (use_env)
                      524 KW_NAMES                13
                      526 PRECALL                  3
                      530 CALL                     3
                      540 STORE_FAST              10 (result_b)
                      542 JUMP_FORWARD            22 (to 588)
          
-         261     >>  544 LOAD_GLOBAL             23 (NULL + subprocess)
+         263     >>  544 LOAD_GLOBAL             23 (NULL + subprocess)
                      556 LOAD_ATTR               12 (check_output)
                      566 LOAD_FAST                0 (cmd)
                      568 LOAD_CONST              12 (True)
                      570 KW_NAMES                14
                      572 PRECALL                  2
                      576 CALL                     2
                      586 STORE_FAST              10 (result_b)
          
-         262     >>  588 LOAD_GLOBAL             13 (NULL + str)
+         264     >>  588 LOAD_GLOBAL             13 (NULL + str)
                      600 LOAD_FAST               10 (result_b)
                      602 PRECALL                  1
                      606 CALL                     1
                      616 STORE_FAST              11 (result)
          
-         263         618 LOAD_FAST               11 (result)
+         265         618 LOAD_FAST               11 (result)
                      620 LOAD_CONST              15 (2)
                      622 LOAD_GLOBAL             27 (NULL + len)
                      634 LOAD_FAST               11 (result)
                      636 PRECALL                  1
                      640 CALL                     1
                      650 LOAD_CONST              16 (3)
                      652 BINARY_OP               10 (-)
                      656 BUILD_SLICE              2
                      658 BINARY_SUBSCR
                      668 STORE_FAST              11 (result)
          
-         264         670 LOAD_CONST              17 (20)
+         266         670 LOAD_CONST              17 (20)
                      672 LOAD_GLOBAL             27 (NULL + len)
                      684 LOAD_FAST                0 (cmd)
                      686 PRECALL                  1
                      690 CALL                     1
                      700 BINARY_OP               10 (-)
                      704 STORE_FAST              12 (tab_to)
          
-         265         706 LOAD_CONST               6 (' ')
+         267         706 LOAD_CONST               6 (' ')
                      708 LOAD_FAST               12 (tab_to)
                      710 BINARY_OP                5 (*)
                      714 STORE_FAST              13 (spaces)
          
-         266         716 LOAD_FAST                2 (msg)
+         268         716 LOAD_FAST                2 (msg)
                      718 LOAD_CONST               5 ('no-msg')
                      720 COMPARE_OP               2 (==)
                      726 POP_JUMP_FORWARD_IF_FALSE     1 (to 730)
          
-         267         728 JUMP_FORWARD            48 (to 826)
+         269         728 JUMP_FORWARD            48 (to 826)
          
-         268     >>  730 LOAD_FAST               11 (result)
+         270     >>  730 LOAD_FAST               11 (result)
                      732 LOAD_CONST               2 ('')
                      734 COMPARE_OP               3 (!=)
                      740 POP_JUMP_FORWARD_IF_FALSE    42 (to 826)
                      742 LOAD_FAST               11 (result)
                      744 LOAD_CONST              18 ('Downloaded the skeleton app, good coding!')
                      746 COMPARE_OP               3 (!=)
                      752 POP_JUMP_FORWARD_IF_FALSE    36 (to 826)
          
-         269         754 LOAD_GLOBAL              6 (log)
+         271         754 LOAD_GLOBAL              6 (log)
                      766 LOAD_METHOD              4 (debug)
                      788 LOAD_FAST                5 (log_msg)
                      790 FORMAT_VALUE             0
                      792 LOAD_CONST               6 (' ')
                      794 LOAD_FAST                0 (cmd)
                      796 FORMAT_VALUE             0
                      798 LOAD_CONST              19 (' result: ')
@@ -1806,15 +1815,15 @@
                      804 LOAD_FAST               11 (result)
                      806 FORMAT_VALUE             0
                      808 BUILD_STRING             6
                      810 PRECALL                  1
                      814 CALL                     1
                      824 POP_TOP
          
-         270     >>  826 LOAD_FAST               11 (result)
+         272     >>  826 LOAD_FAST               11 (result)
                      828 RETURN_VALUE
          consts
             ' run shell command\n\n    :param cmd: string of command to execute\n    :param env:\n    :param msg: optional message (no-msg to suppress)\n    :return:\n    '
             'python'
             ''
             'Execute command:'
             ' with command:'
@@ -1835,15 +1844,15 @@
             ' result: '
          names      ('startswith', 'find_valid_python_name', 'replace', 'log', 'debug', 'get_api_logic_server_dir', 'str', 'os', 'environ', 'copy', 'hasattr', 'subprocess', 'check_output', 'len')
          varnames   ('cmd', 'env', 'msg', 'new_line', 'valid_python_name', 'log_msg', 'use_env', 'project_dir', 'python_path', 'use_env_debug', 'result_b', 'result', 'tab_to', 'spaces')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
          name       'run_command'
-         firstlineno 224
+         firstlineno 226
          lnotab
             0x02082a011c012c0104010c010a010c0106023e0104013402040104011c
             0124013c02200124030a020401040130022c011e01340124010a010c0102
             0118014801
       (False,)
       (None, '', False)
    names      ('subprocess', 'os', 'sys', 'pathlib', 'Path', 'os.path', 'abspath', 'api_logic_server_cli.cli_args_project', 'Project', 'logging', 'getLogger', '__name__', 'log', 'str', 'resolve_home', 'get_project_directory_and_api_name', 'get_abs_db_url', 'get_api_logic_server_dir', 'bool', 'does_file_contain', 'replace_string_in_file', 'insert_lines_at', 'find_valid_python_name', 'run_command')
@@ -1851,8 +1860,8 @@
    freevars   ()
    cellvars   ()
    filename   '/Users/val/dev/ApiLogicServer/ApiLogicServer-dev/org_git/ApiLogicServer-src/api_logic_server_cli/create_from_model/api_logic_server_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020318010c010c010c0108022004100d06250c590c0a140c14081a
-      140c16
+      160c16
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xdd2ca364 (Mon Jul  3 20:17:33 2023 UTC)
+moddate:  0xf37cb864 (Thu Jul 20 00:16:51 2023 UTC)
 files sz: 2260
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a0067006402a2015a01640384005a0264015300
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/api_logic_server_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if rtn_project_directory == '.' or rtn_project_directory == './':
         rtn_project_directory = project.os_cwd
         rtn_merge_into_prototype = True
         msg = ''
         if rtn_project_directory == get_api_logic_server_dir():
             rtn_project_directory = str( Path(get_api_logic_server_dir()) / 'ApiLogicProject' )
             msg = ' <dev>'
-        log.debug(f'1. Merge into project prototype: {rtn_project_directory}{msg}')
+        log.debug(f'1. Merge into project prototype / current project: {rtn_project_directory}{msg}')
     project_path = Path(rtn_project_directory)
     project_path_last_node = project_path.parts[-1]
     if project.multi_api or project.api_name == ".":
         rtn_api_name = project_path_last_node
     return rtn_project_directory, \
         rtn_api_name, \
         rtn_merge_into_prototype
@@ -187,15 +187,17 @@
         insert_line = 0
         for each_line in file_lines:
             if at in each_line:
                 found = True
                 break
             insert_line += 1
         if not found:
-            raise Exception(f'Internal error - unable to find insert: {at}')
+            raise Exception(f'Internal error - unable to find insert:\n'
+                            f'.. seeking {at}\n'
+                            f'.. in {file_name}')
         if after:
             insert_line = insert_line + 1
         file_lines.insert(insert_line, lines)  # you can use any index if you know the line index
         fp.seek(0)  # file pointer locates at the beginning to write the whole file again
         fp.writelines(file_lines)  # write whole list again to the same file
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/model_creation_services.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/model_creation_services.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/create_admin.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/create_admin.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/fab_config.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/fab_config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/home.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/templates/react_admin_component.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/ui_admin_creator.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/ui_admin_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/create_from_model/uri_info.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/create_from_model/uri_info.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/Chinook_Sqlite.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/allocation.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/allocation.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/authentication.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/authentication.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/authentication_doc.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/authentication_doc.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/classicmodels.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/classicmodels.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/new.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/new.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/nw-gold-plus.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/nw-gold-plus.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/nw-gold.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/nw-gold.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/nw.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/nw.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/table_filters_tests.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/table_filters_tests.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/database/todos.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/database/todos.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/extended_builder.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/extended_builder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/fragments/Todo_modelsZZ.py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/fragments/configZZ.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/fragments/configZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/fragments/modelsZZ.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/fragments/modelsZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/fragments/nw_virtual_attrs.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/fragments/nw_virtual_attrs.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/logging.yml` & `ApiLogicServer-9.1.32/api_logic_server_cli/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,30 @@
 	// Sets the run context to one level up instead of the .devcontainer folder.
 	"context": "..",
 
 	// Update the 'dockerFile' property if you aren't using the standard 'Dockerfile' filename.
 	"dockerFile": "For_VSCode.dockerfile",
 
 	// Set *default* container specific settings.json values on container create.
-	"settings": {},
+	// "settings": {},
 
 	// add network -- enable this as required, e.g., https://apilogicserver.github.io/Docs/Database-Connectivity/
 	// "runArgs": ["--network=dev-network"],
 
 	// Add the IDs of extensions you want installed when the container is created.
-	"extensions": ["ms-python.python"],
+	// "extensions": [],   **** Note - Python added in customizations (autoloads Python in devcontainer)
+
+	"customizations": {
+		// Configure properties specific to VS Code.
+		"vscode": {
+			// Set default container specific settings.json values on container create.
+			"settings": {},
+			"extensions": ["ms-python.python"]
+		}
+	},
 	
 	"portsAttributes": {
 		"5656": {
 			"label": "AdminApp"
 		}
 	},
 
@@ -29,22 +38,19 @@
 	
 	"features": {
 		"github-cli": "latest"
 	  },
 
 	"postAttachCommand": "/bin/bash .devcontainer/setup.sh"
 
-	// Use 'forwardPorts' to make a list of ports inside the container available locally.
-	// "forwardPorts": [],
-
 	// Uncomment the next line to run commands after the container is created - for example installing curl.
 	// "postCreateCommand": "apt-get update && apt-get install -y curl",
 
 	// Uncomment when using a ptrace-based debugger like C++, Go, and Rust
 	// "runArgs": [ "--cap-add=SYS_PTRACE", "--security-opt", "seccomp=unconfined" ],
 
 	// Uncomment to use the Docker CLI from inside the container. See https://aka.ms/vscode-remote/samples/docker-from-docker.
 	// "mounts": [ "source=/var/run/docker.sock,target=/var/run/docker.sock,type=bind" ],
 
 	// Uncomment to connect as a non-root user if you've added one. See https://aka.ms/vscode-remote/containers/non-root.
 	// "remoteUser": "vscode"
-}
+}
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/.vscode/launch.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/.vscode/launch.json`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,54 @@
     // Hover to view descriptions of existing attributes.
     // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
     "version": "0.2.0",
     "configurations": [
         {
             "name": "ApiLogicServer",
             "type": "python",
-            "env": {"PYTHONPATH": "", "PYTHONHASHSEED": "0", "APILOGICPROJECT_DEBUG": "False"},            "request": "launch",
+            "env": {
+                "PYTHONPATH": "", 
+                "PYTHONHASHSEED": "0", 
+                "APILOGICPROJECT_DEBUG": "False"},
+            "request": "launch",
             "program": "api_logic_server_run.py",
             "redirectOutput": true,
             "justMyCode": false,
             "args": ["--flask_host=localhost", "--port=5656", "--swagger_host=localhost", "--verbose=False"],
             "console": "internalConsole",
             "internalConsoleOptions": "openOnSessionStart"
         },
         {
             "name": "No Security ApiLogicServer (e.g., simpler swagger)",
             "type": "python",
             "request": "launch",
             "program": "api_logic_server_run.py",
             "redirectOutput": true,
-            "env": {"PYTHONPATH": "", "SECURITY_ENABLED": "False", "PYTHONHASHSEED": "0", "OPT_LOCKING": "optional"},
+            "env": {
+                "PYTHONPATH": "", 
+                "SECURITY_ENABLED": "False", 
+                "PYTHONHASHSEED": "0", 
+                "OPT_LOCKING": "optional"},
+            "justMyCode": false,
+            "args": ["--flask_host=localhost", "--port=5656", "--swagger_host=localhost", "--verbose=False"],
+            "console": "internalConsole",
+            "internalConsoleOptions": "openOnSessionStart"
+        },
+        {
+            "name": "No Security ApiLogicServer VERBOSE",
+            "type": "python",
+            "request": "launch",
+            "program": "api_logic_server_run.py",
+            "redirectOutput": true,
+            "env": {
+                "PYTHONPATH": "", 
+                "SECURITY_ENABLED": "False", 
+                "PYTHONHASHSEED": "0", 
+                "OPT_LOCKING": "optional",
+                "APILOGICPROJECT_VERBOSE": "True"},
             "justMyCode": false,
             "args": ["--flask_host=localhost", "--port=5656", "--swagger_host=localhost", "--verbose=False"],
             "console": "internalConsole",
             "internalConsoleOptions": "openOnSessionStart"
         },
         {
             "name": "Behave Run",
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/customize_api.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/customize_api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/json_encoder.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/readme_customize_api.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/readme_customize_api.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/system/opt_locking/opt_locking.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/system/opt_locking/opt_locking.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from safrs import SAFRSBase
 
 from safrs.util import classproperty
 from safrs.errors import JsonapiError
 from http import HTTPStatus
 
 from config import OptLocking
-from config import Config
+from config import Args as args
 
 logger = logging.getLogger(__name__)
 
 def opt_locking_setup(session):
     """
     Listen_for read events - set rows' CheckSum property for optimistic locking
 
@@ -129,11 +129,11 @@
     if hasattr(logic_row.row, "replace_opt_locking_attr"):
         as_read_checksum = logic_row.row.replace_opt_locking_attr
         old_row_checksum = checksum_old_row(logic_row)
         if as_read_checksum != old_row_checksum:
             logger.info(f"optimistic lock failure - as-read vs current: {as_read_checksum} vs {old_row_checksum}")
             raise ALSError(message="Sorry, row altered by another user - please note changes, cancel and retry")
     else:
-        if Config.OPT_LOCKING == OptLocking.OPTIONAL.value:
+        if args.opt_locking == OptLocking.OPTIONAL.value:
             logger.debug(f'No CheckSum -- ok, configured as optional')
         else:
             raise ALSError("Optimistic Locking error - required CheckSum not present")
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api/system/opt_locking/readme.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api/system/opt_locking/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/api_logic_server_run.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/api_logic_server_run.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,79 +27,78 @@
     print("venv probably not set")
     print("Please see https://apilogicserver.github.io/Docs/Project-Env/ \n")
     exit(1)
 
 from flask_sqlalchemy import SQLAlchemy
 import json
 from pathlib import Path
+from config import Args
 
 def is_docker() -> bool:
     """ running docker?  dir exists: /home/api_logic_server """
     path = '/home/api_logic_server'
     path_result = os.path.isdir(path)  # this *should* exist only on docker
     env_result = "DOCKER" == os.getenv('APILOGICSERVER_RUNNING')
     # assert path_result == env_result
     return path_result
 
 
-# =======================================
-#    Creation Defaults
-#
-#        Override as desired
-#         Or specify in CLI arguments
-# ======================================= 
-
-# defaults from ApiLogicServer create command...
-API_PREFIX = "/api"
-flask_host   = "api_logic_server_host"  # where clients find  the API (eg, cloud server addr)
-swagger_host = "api_logic_server_swagger_host"
-if swagger_host == "":
-    swagger_host = flask_host  # where swagger finds the API
-if is_docker() and flask_host == "localhost":
-    flask_host = "0.0.0.0"  # enables docker run.sh (where there are no args)
-port = "api_logic_server_port"
-swagger_port = port  # for codespaces - see values in launch config
-http_type = "http"
-
 current_path = os.path.abspath(os.path.dirname(__file__))
 sys.path.append(current_path)
+if is_docker():
+    sys.path.append(os.path.abspath('/home/api_logic_server'))
+
 project_dir = str(current_path)
 os.chdir(project_dir)  # so admin app can find images, code
 import util as util
 logic_logger_activate_debug = False
 """ True prints all rules on startup """
 
-
-
 args = ""
 arg_num = 0
 for each_arg in sys.argv:
     args += each_arg
     arg_num += 1
     if arg_num < len(sys.argv):
         args += ", "
 project_name = os.path.basename(os.path.normpath(current_path))
 
 from typing import TypedDict
 import safrs  # fails without venv - see https://apilogicserver.github.io/Docs/Project-Env/
+from safrs import ValidationError, SAFRSBase, SAFRSAPI as _SAFRSAPI
 from logic_bank.logic_bank import LogicBank
 from logic_bank.exec_row_logic.logic_row import LogicRow
 from logic_bank.rule_type.constraint import Constraint
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session
 import socket
 import warnings
 from flask import Flask, redirect, send_from_directory, send_file
 from safrs import ValidationError, SAFRSBase, SAFRSAPI
-from config import Config
-from ui.admin.admin_loader import admin_events
+import ui.admin.admin_loader as AdminLoader
 from security.system.authentication import configure_auth
 import database.multi_db as multi_db
 
 
+class SAFRSAPI(_SAFRSAPI):
+    """
+    Extends SAFRSAPI to handle client_uri
+
+    Args:
+        _SAFRSAPI (_type_): _description_
+    """
+
+    def __init__(self, *args, **kwargs):
+        client_uri = kwargs.pop('client_uri', None)
+        if client_uri:
+            kwargs['port'] = None
+            kwargs['host'] = client_uri
+        super().__init__(*args, **kwargs)
+
+
 
 # ==================================
 #       LOGGING SETUP
 # ================================== 
 
 current_path = os.path.abspath(os.path.dirname(__file__))
 with open(f'{current_path}/logging.yml','rt') as f:  # see also logic/declare_logic.py
@@ -111,15 +110,15 @@
 if debug_value is not None:  # > export APILOGICPROJECT_DEBUG=True
     debug_value = debug_value.upper()
     if debug_value.startswith("F") or debug_value.startswith("N"):
         app_logger.setLevel(logging.INFO)
     else:
         app_logger.setLevel(logging.DEBUG)
         app_logger.debug(f'\nDEBUG level set from env\n')
-app_logger.info(f'\nAPI Logic Project ({project_name}) Starting with args: \n.. {args}\n')
+app_logger.info(f'\nAPI Logic Project ({project_name}) Starting with CLI args: \n.. {args}\n')
 app_logger.info(f'Created api_logic_server_created_on at {str(current_path)}\n')
 
 
 class ValidationErrorExt(ValidationError):
     """
     This exception is raised when invalid input has been detected (client side input)
     Always send back the message to the client in the response
@@ -130,148 +129,51 @@
         self.error_attributes = error_attributes
         self.status_code = status_code
         self.message = message
         self.api_code = api_code
         self.detail: TypedDict = detail
 
 
-def get_args():
-    """
-    returns tuple of start args:
-    
-    (flask_host, swagger_host, port, swagger_port, http_type, verbose, create_and_run)
-    """
-
-    global flask_host, swagger_host, port, swagger_port, http_type, verbose, create_and_run
-
-    network_diagnostics = True
-    hostname = socket.gethostname()
-    try:
-        local_ip = socket.gethostbyname(hostname)
-    except:
-        local_ip = f"Warning - Failed local_ip = socket.gethostbyname(hostname) with hostname: {hostname}"
-        app_logger.debug(f"Failed local_ip = socket.gethostbyname(hostname) with hostname: {hostname}")
-
-    app_logger.debug(f"Getting args, with hostname={hostname} on local_ip={local_ip}")
-    verbose = False
-    create_and_run = False
-
-    def make_wide(formatter, w=120, h=36):
-        """ Return a wider HelpFormatter, if possible."""
-        try:
-            # https://stackoverflow.com/a/5464440
-            # beware: "Only the name of this class is considered a public API."
-            kwargs = {'width': w, 'max_help_position': h}
-            formatter(None, **kwargs)
-            return lambda prog: formatter(prog, **kwargs)
-        except TypeError:
-            warnings.warn("argparse help formatter failed, falling back.")
-            return formatter
-
-    if __name__ != "__main__":  
-        app_logger.debug(f"WSGI - no args, using creation default host/port..  sys.argv = {sys.argv}\n")
-    else:   # gunicorn-friendly host/port settings ()
-        # thanks to https://www.geeksforgeeks.org/command-line-arguments-in-python/#argparse
-        import argparse
-        # Initialize parser
-        if len(sys.argv) == 1:
-            app_logger.debug("No arguments - using creation default host/port")
-        else:
-            msg = "API Logic Project"
-            parser = argparse.ArgumentParser(
-                formatter_class=make_wide(argparse.ArgumentDefaultsHelpFormatter))
-            parser.add_argument("--port",
-                                help = f'port (Flask)', default = port)
-            parser.add_argument("--flask_host", 
-                                help = f'ip to which flask will be bound', 
-                                default = flask_host)
-            parser.add_argument("--swagger_host", 
-                                help = f'ip clients use to access API',
-                                default = swagger_host)
-            parser.add_argument("--swagger_port", 
-                                help = f'swagger port (eg, 443 for codespaces)',
-                                default = port)
-            parser.add_argument("--http_type", 
-                                help = f'http or https',
-                                default = "http")
-            parser.add_argument("--verbose", 
-                                help = f'for more logging',
-                                default = False)
-            parser.add_argument("--create_and_run", 
-                                help = f'system use - log how to open project',
-                                default = False)
-            
-            parser.add_argument("flask_host_p", nargs='?', default = flask_host)
-            parser.add_argument("port_p", nargs='?', default = port)
-            parser.add_argument("swagger_host_p", nargs='?', default = swagger_host)
-            
-            args = parser.parse_args()
-
-            """
-                accepting both positional (compatibility) and keyword args... 
-                cases that matter:
-                    no args
-                    kw only:        argv[1] starts with -
-                    pos only
-                positional values always override keyword, so decide which parsed values to use...
-            """
-            if sys.argv[1].startswith("-"):     # keyword arguments
-                port = args.port
-                flask_host = args.flask_host
-                swagger_host = args.swagger_host
-                swagger_port = args.swagger_port
-                http_type = args.http_type
-                verbose = args.verbose in ["True", "true"]
-                create_and_run = args.create_and_run
-            else:                               # positional arguments (compatibility)
-                port = args.port_p
-                flask_host = args.flask_host_p
-                swagger_host = args.swagger_host_p
-        if swagger_host.startswith("https://"):
-            swagger_host = swagger_host[8:]
-        if swagger_host.endswith("/"):
-            swagger_host = swagger_host[0:len(swagger_host)-1]
-
-    use_codespace_defaulting = True  # experimental support to run default launch config
-    if use_codespace_defaulting and os.getenv('CODESPACES') and swagger_host == 'localhost':
-        app_logger.info('\n Applying Codespaces default port settings')
-        swagger_host = os.getenv('CODESPACE_NAME') + '-5656.githubpreview.dev'
-        swagger_port = 443
-        http_type = 'https'
-
-    return flask_host, swagger_host, port, swagger_port, http_type, verbose, create_and_run
-
-
 # ==========================================================
-# Creates flask_app, starts server after setup:
+# API Logic Server Setup
 #   - Opens Database(s)
 #   - Setup API, Logic, Security, Optimistic Locking 
 # ==========================================================
 
-def create_app(swagger_host: str = "localhost", swagger_port: str = "5656"):
-    """ Creates flask_app, Opens Database, Activates API and Logic """ 
+def api_logic_server_setup(flask_app: Flask, args: Args):
+    """
+    API Logic Server Setup
+
+    1. Opens Database(s)
+    2. Setup API, Logic, Security, Optimistic Locking
+
+
+    Args:
+        flask_app (_type_): configured flask_app (servers, ports, db uri's)
+        args (_type_): typed access to flask_app.config
+
+    Raises:
+        ValidationErrorExt: rebadge LogicBank errors for SAFRS API
+    """
 
     from sqlalchemy import exc as sa_exc
 
     global logic_logger_activate_debug
 
     with warnings.catch_warnings():
 
-        flask_app = Flask("API Logic Server", template_folder='ui/templates')  # templates to load ui/admin/admin.yaml
-
         safrs_log_level = safrs.log.getEffectiveLevel()
         db_logger = logging.getLogger('sqlalchemy')
         db_log_level = db_logger.getEffectiveLevel()
         safrs_init_logger = logging.getLogger("safrs.safrs_init")
-        do_hide_chatty_logging = True and not verbose
+        do_hide_chatty_logging = True and not args.verbose
         if do_hide_chatty_logging and app_logger.getEffectiveLevel() <= logging.INFO:
             safrs.log.setLevel(logging.WARN)  # notset 0, debug 10, info 20, warn 30, error 40, critical 50
             db_logger.setLevel(logging.WARN)
             safrs_init_logger.setLevel(logging.WARN)
-        flask_app.config.from_object("config.Config")
 
         multi_db.bind_dbs(flask_app)
 
         # https://stackoverflow.com/questions/34674029/sqlalchemy-query-raises-unnecessary-warning-about-sqlite-and-decimal-how-to-spe
         warnings.simplefilter("ignore", category=sa_exc.SAWarning)  # alert - disable for safety msgs
 
         def constraint_handler(message: str, constraint: Constraint, logic_row: LogicRow):
@@ -290,15 +192,16 @@
 
         db = SQLAlchemy()
         db.init_app(flask_app)
         with flask_app.app_context():
 
             with open(Path(current_path).joinpath('security/system/custom_swagger.json')) as json_file:
                 custom_swagger = json.load(json_file)
-            safrs_api = SAFRSAPI(flask_app, app_db= db, host=swagger_host, port=swagger_port, prefix = API_PREFIX, custom_swagger=custom_swagger)
+            safrs_api = SAFRSAPI(flask_app, app_db= db, host=args.swagger_host, port=args.swagger_port, client_uri=args.client_uri,
+                                 prefix = args.api_prefix, custom_swagger=custom_swagger)
 
             db = safrs.DB  # valid only after is initialized, above
             session: Session = db.session
 
             if admin_enabled:  # unused (internal dev use)
                 db.create_all()
                 db.create_all(bind='admin')
@@ -320,85 +223,97 @@
             logic_logger.setLevel(logic_logger_level)
             app_logger.info("Declare   Logic complete - logic/declare_logic.py (rules + code)"
                 + f' -- {len(database.models.metadata.tables)} tables loaded\n')  # db opened 1st access
             
             method_decorators : list = []
             safrs_init_logger.setLevel(logging.WARN)
             expose_api_models.expose_models(safrs_api, method_decorators)
-            app_logger.info(f'Declare   API - api/expose_api_models, endpoint for each table on {swagger_host}:{swagger_port}, customizing...')
-            customize_api.expose_services(flask_app, safrs_api, project_dir, swagger_host=swagger_host, PORT=port)  # custom services
+            app_logger.info(f'Declare   API - api/expose_api_models, endpoint for each table on {args.swagger_host}:{args.swagger_port}, customizing...')
+            customize_api.expose_services(flask_app, safrs_api, project_dir, swagger_host=args.swagger_host, PORT=args.port)  # custom services
 
-            if Config.SECURITY_ENABLED:
+            if args.security_enabled:
                 configure_auth(flask_app, database, method_decorators)
 
             multi_db.expose_db_apis(flask_app, session, safrs_api, method_decorators)
 
-            if Config.SECURITY_ENABLED:
+            if args.security_enabled:
                 from security import declare_security  # activate security
                 app_logger.info("..declare security - security/declare_security.py"
-                    + f' -- {len(database.authentication_models.metadata.tables)} authentication tables loaded')
+                    # not accurate: + f' -- {len(database.authentication_models.metadata.tables)}'
+                    + ' authentication tables loaded')
 
             from api.system.opt_locking import opt_locking
             from config import OptLocking
-            if Config.OPT_LOCKING == OptLocking.IGNORED.value:
+            if args.opt_locking == OptLocking.IGNORED.value:
                 app_logger.info("\nOptimistic Locking: ignored")
             else:
                 opt_locking.opt_locking_setup(session)
 
             SAFRSBase._s_auto_commit = False
             session.close()
         
         safrs.log.setLevel(safrs_log_level)
         db_logger.setLevel(db_log_level)
-        return flask_app
 
 
 # ==================================
 #        MAIN CODE
 # ================================== 
 
-(flask_host, swagger_host, port, swagger_port, http_type, verbose, create_and_run) = get_args()
-if os.getenv('SWAGGER_HOST'):
-    swagger_host = os.getenv('SWAGGER_HOST')  # type: ignore # type: str
-if os.getenv('VERBOSE'):
-    verbose = True  # type: ignore # type: str
 
-if verbose:
+flask_app = Flask("API Logic Server", template_folder='ui/templates')  # templates to load ui/admin/admin.yaml
+
+args = Args(flask_app=flask_app)                                # creation defaults
+
+flask_app.config.from_object("config.Config")
+app_logger.debug(f"\nConfig args: \n{args}")                    # config file (e.g., db uri's)
+
+args.get_cli_args(dunder_name=__name__, args=args)
+app_logger.debug(f"\nCLI args: \n{args}")                       # api_logic_server_run cl args
+
+flask_app.config.from_prefixed_env(prefix="APILOGICPROJECT")    # env overrides (e.g., docker)
+app_logger.debug(f"\nENV args: \n{args}\n\n")
+
+if args.verbose:
     app_logger.setLevel(logging.DEBUG)
     safrs.log.setLevel(logging.DEBUG)  # notset 0, debug 10, info 20, warn 30, error 40, critical 50
-if app_logger.getEffectiveLevel() == logging.DEBUG:
-    util.sys_info()
+if app_logger.getEffectiveLevel() <= logging.DEBUG:
+    util.sys_info(flask_app.config)
+app_logger.debug(f"\nENV args: \n{args}\n\n")
 
-flask_app = create_app(swagger_host = swagger_host, swagger_port = swagger_port)
+api_logic_server_setup(flask_app, args)
 
-admin_events(flask_app = flask_app, swagger_host = swagger_host, swagger_port = swagger_port,
-    API_PREFIX=API_PREFIX, validation_error=ValidationError, http_type = http_type)
+AdminLoader.admin_events(flask_app = flask_app, args = args, validation_error = ValidationError)
 
 if __name__ == "__main__":
     msg = f'API Logic Project loaded (not WSGI), version api_logic_server_version\n'
     if is_docker():
-        msg += f' (running from docker container at flask_host: {flask_host} - may require refresh)\n'
+        msg += f' (running from docker container at flask_host: {args.flask_host} - may require refresh)\n'
     else:
-        msg += f' (running locally at flask_host: {flask_host})\n'
+        msg += f' (running locally at flask_host: {args.flask_host})\n'
     app_logger.info(f'\n{msg}')
 
-    if create_and_run:
+    if args.create_and_run:
         app_logger.info(f'==> Customizable API Logic Project created and running:\n'
                     f'..Open it with your IDE at {project_dir}\n')
 
     if os.getenv('CODESPACES'):
         app_logger.info(f'API Logic Project (name: {project_name}) starting on Codespaces:\n'
-                f'..Explore data and API on codespaces, swagger_host: {http_type}://{swagger_host}/\n')
+                f'..Explore data and API on codespaces, swagger_host: {args.http_scheme}://{args.swagger_host}/\n')
     else:
         app_logger.info(f'API Logic Project (name: {project_name}) starting:\n'
-                f'..Explore data and API at swagger_host: {http_type}://{swagger_host}:{port}/\n')
+                f'..Explore data and API at http_scheme://swagger_host:port {args.http_scheme}://{args.swagger_host}:{args.port}\n'
+                f'.... with flask_host: {args.flask_host}\n'
+                f'.... and  swagger_port: {args.swagger_port}')
 
-    flask_app.run(host=flask_host, threaded=True, port=port)
+    flask_app.run(host=args.flask_host, threaded=True, port=args.port)
 else:
     msg = f'API Logic Project Loaded (WSGI), version api_logic_server_version\n'
     if is_docker():
-        msg += f' (running from docker container at {flask_host} - may require refresh)\n'
+        msg += f' (running from docker container at {args.flask_host} - may require refresh)\n'
     else:
-        msg += f' (running locally at flask_host: {flask_host})\n'
+        msg += f' (running locally at flask_host: {args.flask_host})\n'
     app_logger.info(f'\n{msg}')
     app_logger.info(f'API Logic Project (name: {project_name}) starting:\n'
-            f'..Explore data and API at swagger_host: {http_type}://{swagger_host}:{port}/\n')
+                f'..Explore data and API at http_scheme://swagger_host:port {args.http_scheme}://{args.swagger_host}:{args.port}\n'
+                f'.... with flask_host: {args.flask_host}\n'
+                f'.... and  swagger_port: {args.swagger_port}')
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/env.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic/readme.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/alembic.ini` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/alembic.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/bind_databases.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/bind_databases.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/db_debug.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/db_debug.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/database/multi_db.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/database/multi_db.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/auth-db/authdb_mysql.Dockerfile`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/auth-db/authdb_mysql.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 -- MySQL dump 10.13  Distrib 8.0.32, for Linux (aarch64)
 --
 -- Host: localhost    Database: authdb
 -- ------------------------------------------------------
 -- Server version	8.0.32
 
+-- mysql -u root -p
+-- use authdb
+-- 
+
 DROP DATABASE IF EXISTS `authdb`;
 CREATE DATABASE `authdb`;
 USE `authdb`;
 
 /*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
 /*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
 /*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
@@ -47,30 +51,29 @@
 
 DROP TABLE IF EXISTS `User`;
 /*!40101 SET @saved_cs_client     = @@character_set_client */;
 /*!50503 SET character_set_client = utf8mb4 */;
 CREATE TABLE `User` (
   `name` varchar(128) DEFAULT NULL,
   `notes` text,
-  `client_id` int DEFAULT NULL,
   `id` varchar(64) NOT NULL,
   `username` varchar(128) DEFAULT NULL,
   `email` varchar(128) DEFAULT NULL,
   `password_hash` varchar(200) DEFAULT NULL,
   PRIMARY KEY (`id`)
 ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
 /*!40101 SET character_set_client = @saved_cs_client */;
 
 --
 -- Dumping data for table `User`
 --
 
 LOCK TABLES `User` WRITE;
 /*!40000 ALTER TABLE `User` DISABLE KEYS */;
-INSERT INTO `User` VALUES ('Administrator',NULL,1,'admin','Admin User','admin@corp.com','p');
+INSERT INTO `User` VALUES ('Administrator',NULL,'admin','Admin User','admin@corp.com','p');
 /*!40000 ALTER TABLE `User` ENABLE KEYS */;
 UNLOCK TABLES;
 
 --
 -- Table structure for table `UserRole`
 --
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-image/build_image.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/bin/bash
 
 # To build container for your ApiLogicProject:
-#    create / customize your project as your normally would
+#    create / customize your project as you normally would
 #    edit this file: change your_account/your_repository as appropriate
-#    in terminal (not in VSCode docker - docker is not installed there), cd to your project
-#    build a container for your project: `sh build_container.sh`
+#    in terminal (not in VSCode docker - docker is not installed there)
+#    $ cd <your project>
+#    $ sh devops/docker-image/build_image.sh
 
 projectname="apilogicserver_project_name_lower"  # lower case, only
 repositoryname="apilogicserver"
 version="1.0.0"
 
 debug() {
   debug="disabled"
   # echo "$1"
 }
 
 debug "\n"
 debug "build_image here 1.0"
 if [ $# -eq 0 ]; then
   echo "\nBuilds docker image for API Logic Project\n"
-  echo "  cd devops/docker"
-  echo "  sh build_container.sh [ . | <docker-id> ]"
+  echo "  cd <project home directory>"
+  echo "  sh devops/docker/build_image.sh [ . | <docker-id> ]"
   echo "    . means use defaults:"
   echo "        ${repositoryname}/${projectname}:${version}"
   echo "    <docker-id> means use explicit args: <repository-name> <project-name> <version> eg,"
   echo "        sh build_image.sh myrepository myproject 1.0.1"
   echo " "
   exit 0
 fi
@@ -35,27 +36,28 @@
 else
   debug "using arg overrides"
   repositoryname="$1"
   projectname="$2"
   version="$3"
 fi
 
-docker build -f build_image.dockerfile -t ${repositoryname}/${projectname} --rm .
+docker build -f devops/docker-image/build_image.dockerfile -t ${repositoryname}/${projectname} --rm .
 
 status=$?
 if [ $status -eq 0 ]; then
-  echo "\nImage built successfully.. test (omit bash to run directly):\n"
-  echo "  docker run -it --name ${projectname} --rm --net dev-network -p 5656:5656 -p 5002:5002 -v ${PWD}:/localhost ${repositoryname}/${projectname}:${version} bash"
+  echo "\nImage built successfully.. test:\n"
+  echo "  sh devops/docker-image/run_image.sh"
+  echo " "
   echo "\nNext steps:"
   echo "  docker tag ${repositoryname}/${projectname} ${repositoryname}/${projectname}:${version}"
   echo "  docker push ${repositoryname}/${projectname}:${version}  # requires docker login"\"
   echo " "
   echo "  docker tag ${repositoryname}/${projectname} ${repositoryname}/${projectname}:latest"
   echo "  docker push ${repositoryname}/${projectname}:latest"
   echo " "
   echo "Image ready to deploy; e.g. on Azure: https://apilogicserver.github.io/Docs/DevOps-Containers-Deploy"
 else
-  echo "command unsuccessful\n"
+  echo "docker build unsuccessful\n"
   exit 1
 fi
 echo " "
 exit 0
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/logging.yml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/logging.yml`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,19 @@
         propagate: no
 
     security.system.authorization:   
 #        level: DEBUG
         handlers: [console]
         propagate: no
 
+    security.authentication_provider.sql.sqlite.auth_provider:   
+        level: INFO
+        handlers: [console]
+        propagate: no
+
     ui.admin.admin_loader:   
 #        level: DEBUG
         handlers: [console]
         propagate: no
 
     util:   
         level: INFO
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/logic/declare_logic.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/mypy.ini` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/mypy.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/readme.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/run.ps1` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/run.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/run.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/run.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 from security.authentication_provider.abstract_authentication_provider import Abstract_Authentication_Provider
 import sqlalchemy as sqlalchemy
 import database.authentication_models as authentication_models
 from flask import Flask
 import safrs
+from safrs.errors import JsonapiError
 from dotmap import DotMap  # a dict, but you can say aDict.name instead of aDict['name']... like a row
 from sqlalchemy import inspect
+from http import HTTPStatus
+import logging
 
 # **********************
 # sql auth provider
 # **********************
 
 db = None
 session = None
 
+logger = logging.getLogger(__name__)
+
+class ALSError(JsonapiError):
+    
+    def __init__(self, message, status_code=HTTPStatus.BAD_REQUEST):
+        super().__init__()
+        self.message = message
+        self.status_code = status_code
+
+
 class Authentication_Provider(Abstract_Authentication_Provider):
 
     @staticmethod
     def get_user(id: str, password: str = "") -> object:
         """
         Must return a row object with attributes:
         
@@ -43,15 +56,21 @@
             return rtn_dotmap
 
         global db, session
         if db is None:
             db = safrs.DB         # Use the safrs.DB for database access
             session = db.session  # sqlalchemy.orm.scoping.scoped_session
 
-        user = session.query(authentication_models.User).filter(authentication_models.User.id == id).one()
+        try:
+            user = session.query(authentication_models.User).filter(authentication_models.User.id == id).one()
+        except Exception as e:
+            logger.info(f'*****\nauth_provider FAILED looking for: {id}\n*****\n')
+            logger.info(f'excp: {str(e)}\n')
+            # raise e
+            raise ALSError(f"User {id} is not authorized for this system")
         use_db_row = True
         if use_db_row:
             return user
         else:
             pass
             rtn_user = row_to_dotmap(user, authentication_models.User)
             rtn_user.UserRoleList = []
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/declare_security.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/notes_temp/token.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/system/authentication.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/system/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 from flask import jsonify, request
 from flask_jwt_extended import JWTManager
 from flask_jwt_extended import jwt_required as jwt_required_ori
 from flask_jwt_extended import create_access_token
 from datetime import timedelta
 from functools import wraps
 import config
+from config import Args
 from security.authentication_provider.abstract_authentication_provider import Abstract_Authentication_Provider
 
 authentication_provider : Abstract_Authentication_Provider = config.Config.SECURITY_PROVIDER  # type: ignore
+# note: direct config access is disparaged, but used since args not set up when this imported
 
 security_logger = logging.getLogger(__name__)
 
 JWT_EXCLUDE = 'jwt_exclude'
 
 def jwt_required(*args, **kwargs):
     from flask import request
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/system/authorization.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/system/authorization.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from sqlalchemy import event, MetaData
 from sqlalchemy.orm import with_loader_criteria, DeclarativeMeta
 import logging, sys
 
 
 from flask_jwt_extended import current_user
 
-from config import Config
-authentication_provider = Config.SECURITY_PROVIDER
+from config import Args
+authentication_provider = Args.security_provider
 
 security_logger = logging.getLogger(__name__)
 
 security_logger.debug(f'\nAuthorization loaded via api_logic_server_run.py -- import \n')
 
 
 db = safrs.DB         # Use the safrs.DB, not db!
@@ -143,15 +143,15 @@
         else:
             security_logger.debug(f"No Grants for {table_name}")
 
 @event.listens_for(session, 'do_orm_execute')
 def receive_do_orm_execute(orm_execute_state):
     "listen for the 'do_orm_execute' event from SQLAlchemy"
     if (
-        Config.SECURITY_ENABLED
+        Args.security_enabled
         and orm_execute_state.is_select
         and not orm_execute_state.is_column_load
         and not orm_execute_state.is_relationship_load
     ):            
         security_logger.debug(f'receive_do_orm_execute alive')
         mapper = orm_execute_state.bind_arguments['mapper']
         table_name = mapper.persist_selectable.fullname   # mapper.mapped_table.fullname disparaged
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/security/system/custom_swagger.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/templates/index.html` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     if test is not None and len(test) >= 26:
         test_val = test[0:25]
     msg_url = f'http://localhost:5656/server_log?msg={msg}&test={test}&dir=test/api_logic_server_behave/logs/scenario_logic_logs'
     r = requests.get(msg_url)
 
 SECURITY_ENABLED = True  # you must also: ApiLogicServer add-db --db_url=auth --bind_key=authentication
 if os.getenv('SECURITY_ENABLED'):  # e.g. export SECURITY_ENABLED=true
+    # config.Args not available - config not loaded, no Flask
     security_export = os.getenv('SECURITY_ENABLED')  # type: ignore # type: str
     security_export = security_export.lower()  # type: ignore
     if security_export in ["false", "no"]:  # NO SEC
         SECURITY_ENABLED = False
     else:
         SECURITY_ENABLED = True
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/test/basic/server_test.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,68 +2,75 @@
         * return minified app
         * return admin.yaml file
 """
 
 import logging, sys, io
 from flask import Flask, redirect, send_from_directory, send_file
 from config import Config
+from config import Args
 from pathlib import Path
 import os, inspect
 from safrs import ValidationError
 
 admin_logger = logging.getLogger(__name__)  # log levels: critical < error < warning(20) < info(30) < debug
 
 did_send_spa = False
 
-def get_sra_directory() -> str:
+def get_sra_directory(args: Args) -> str:
     """
     return location of minified sra, which can be...
 
     1. in the venv (from install or Docker) -- the normal case (small projects, less git)
     2. local to project: ui/safrs-react-admin
-    3. for internal dev use, in env(APILOGICSERVER_HOME) (dev venv does not contain ALS)
+    3. in env(APILOGICSERVER_HOME | APILOGICPROJECT_APILOGICSERVER_HOME)
+    
+    This enables the sra code to be re-used, reducing app size 32MB -> 2.5 MB
     """
     directory = 'ui/safrs-react-admin'  # local project sra typical API Logic Server path (index.yaml)
     if Path(directory).joinpath('robots.txt').is_file():
         admin_logger.debug("return_spa - using local directory")
     else:     # else use installed sra - from venv, or, for dev, in APILOGICSERVER_HOME
         try:  # works for installed, docker, codespaces.  not Azure
             from api_logic_server_cli.create_from_model import api_logic_server_utils as api_logic_server_utils
         except:
             dev_home = os.getenv('APILOGICSERVER_HOME')
             if dev_home:
                 admin_logger.debug("ApiLogicServer not in venv, trying APILOGICSERVER_HOME")
             else:
-                dev_home = os.getenv('HOME')
-                if not dev_home:
-                    raise Exception('ApiLogicServer not in venv, env APILOGICSERVER_HOME or HOME must be set')
+                dev_home = args.api_logic_server_home
+                if dev_home:
+                    admin_logger.debug("ApiLogicServer not in venv, trying APILOGICPROJECT_APILOGICSERVER_HOME")
+                else:
+                    dev_home = os.getenv('HOME')
+                    if not dev_home:
+                        raise Exception('ApiLogicServer not in venv, env APILOGICSERVER_HOME or HOME must be set')
             sys.path.append(dev_home)
             from api_logic_server_cli.create_from_model import api_logic_server_utils as api_logic_server_utils
         admin_logger.debug("return_spa - install directory")
         utils_str = inspect.getfile(api_logic_server_utils)
         sra_path = Path(utils_str).parent.joinpath('safrs-react-admin-npm-build')
         directory = str(sra_path)
     return directory
 
 
-def admin_events(flask_app: Flask, swagger_host: str, swagger_port: str, API_PREFIX: str, validation_error: ValidationError, http_type: str):
+def admin_events(flask_app: Flask, args: Args, validation_error: ValidationError):
     """ events for serving minified safrs-admin, using admin.yaml
     """
 
     @flask_app.route("/admin/<path:path>")
     def start_custom_app_return_spa(path=None):
         """ Step 1 - Start Custom App, and return minified safrs-react-admin app (acquired from safrs-react-admin/build) 
             Custom url: http://localhost:5656/admin/custom_app
         """
         global did_send_spa
         admin_logger.debug(f'API Logic Server - Start Custom App, return minified sra')
         if True or not did_send_spa:
             did_send_spa = True
             admin_logger.info(f'\nStart Custom App ({path}): return spa "ui/safrs-react-admin", "index.html"\n')
-        directory = get_sra_directory()
+        directory = get_sra_directory(args)
         return send_from_directory(directory, 'index.html')  # unsure how admin finds custom url
 
     @flask_app.route('/')
     def start_default_app():
         """ Step 1 - Start default Admin App 
             Default URL: http://localhost:5656/ 
         """
@@ -74,40 +81,49 @@
     def return_spa(path=None):
         """ Step 2 - return minified sra for default admin app
         """
         global did_send_spa
         if path == "home.js":
             directory = "ui/admin"
         else:
-            directory = get_sra_directory()
+            directory = get_sra_directory(args)
 
         if not did_send_spa:
             did_send_spa = True
             admin_logger.debug(f'return_spa - directory = {directory}, path= {path}')
 
         return send_from_directory(directory, path)
 
 
     @flask_app.route('/ui/admin/<path:path>')
     def admin_yaml(path=None):
         """ Step 3 - return admin file response (to now-running safrs-react-admin app)
             and text-substitutes to get url args from startup args (avoid specify twice for *both* server & admin.yaml)
 
-            api_root: {http_type}://{swagger_host}:{swagger_port} (from ui_admin_creator)
+            api_root: {http_type}://{swagger_host}:{port}/{api} (from ui_admin_creator)
+
+            auth/endpoint: {http_type}://{swagger_host}:{port}/api/auth/login
 
             e.g. http://localhost:5656/ui/admin/admin.yaml
         """
         use_type = "mem"
         if use_type == "mem":
             with open(f'ui/admin/{path}', "r") as f:  # path is admin.yaml for default url/app
                 content = f.read()
-            content = content.replace("{http_type}", http_type)
-            content = content.replace("{swagger_host}", swagger_host)
-            content = content.replace("{port}", str(swagger_port))  # note - codespaces requires 443 here (typically via args)
-            content = content.replace("{api}", API_PREFIX[1:])
+            if args.client_uri is not None:
+                content = content.replace(
+                    '{http_type}://{swagger_host}:{port}',
+                    args.client_uri
+                )
+                content = content.replace("{api}", args.api_prefix[1:])
+            else:
+                content = content.replace("{http_type}", args.http_scheme)
+                content = content.replace("{swagger_host}", args.swagger_host)
+                content = content.replace("{port}", str(args.swagger_port))  # note - codespaces requires 443 here (typically via args)
+                content = content.replace("{api}", args.api_prefix[1:])
             if Config.SECURITY_ENABLED == False:
                 content = content.replace("authentication", 'no-authentication')
             admin_logger.debug(f'loading ui/admin/admin.yaml')
             mem = io.BytesIO(str.encode(content))
             return send_file(mem, mimetype='text/yaml')
         else:
             response = send_file("ui/admin/admin.yaml", mimetype='text/yaml')
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/admin/home.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/util.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,19 +214,19 @@
         list of rows as dicts
     """
     rows = []
     for each_row in result:
         row_as_dict = {}
         log(f'type(each_row): {type(each_row)}')
         if isinstance (each_row, sqlalchemy.engine.row.Row):  # raw sql, eg, sample catsql
-            key_to_index = each_row._key_to_index             # note: SQLAlchemy 2 specific
+            key_to_index = each_row._key_to_index  # note: SQLAlchemy 2 specific
             for name, value in key_to_index.items():
                 row_as_dict[name] = each_row[value]
         else:
-            row_as_dict = each_row.to_dict()                  # safrs helper
+            row_as_dict = each_row.to_dict()
         rows.append(row_as_dict)
     return rows
 
 
 def sys_info():  
     """
     Print env and path
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/py.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/venv.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/venv_setup/venv.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/Logic-Allocation.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/Logic-Allocation.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/images/allocation/db.png` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/images/allocation/db.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/images/allocation/logic-diagram.png` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/images/allocation/logic-diagram.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_allocation/test/test.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_allocation/test/test.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/Tutorial.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/customize_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,33 +82,31 @@
         msg = request.args.get('msg')
         app_logger.info(f'\nStopped server: {msg}\n')
 
         os.kill(os.getpid(), signal.SIGINT)
         return jsonify({ "success": True, "message": "Server is shutting down..." })
 
 
-    def admin_required():
+    def bypass_security():
         """
         Support option to bypass security (see cats, below).
-
-        See: https://flask-jwt-extended.readthedocs.io/en/stable/custom_decorators/
         """
         def wrapper(fn):
             @wraps(fn)
             def decorator(*args, **kwargs):
                 if Config.SECURITY_ENABLED == False:
                     return fn(*args, **kwargs)
                 verify_jwt_in_request(True)  # must be issued if security enabled
                 return fn(*args, **kwargs)
             return decorator
         return wrapper
 
 
     @app.route('/filters_cats')
-    @admin_required()
+    @bypass_security()
     def filters_cats():
         """
         Illustrates:
         * Explore SQLAlchemy and/or filters.
         
         Test (returns rows 2-5) (no auth):
             curl -X GET "http://localhost:5656/filters_cats" [no-filter | simple-filter]"
@@ -116,15 +114,15 @@
 
         from sqlalchemy import and_, or_
         filter_type = request.args.get('filter')
         if filter_type is None:
             filter_type = "multiple filters"
         db = safrs.DB           # Use the safrs.DB, not db!
         session = db.session    # sqlalchemy.orm.scoping.scoped_session
-        Security.set_user_sa()  # an endpoint that requires no auth header (see also @admin_required)
+        Security.set_user_sa()  # an endpoint that requires no auth header (see also @bypass_security)
 
         if filter_type.startswith("n"):
             results = session.query(models.Category)    # .filter(models.Category.Id > 1)
         elif filter_type.startswith("s"):               # normally coded like this
             results = session.query(models.Category) \
                 .filter(models.Category.Id > 1) \
                 .filter(or_((models.Category.Client_id == 2), (models.Category.Id == 5)))
@@ -139,15 +137,15 @@
         for each_result in results:
             row = { 'id': each_result.Id, 'name': each_result.CategoryName}
             return_result.append(row)
         return jsonify({ "success": True, "result":  return_result})
 
 
     @app.route('/raw_sql_cats')
-    @admin_required()
+    @bypass_security()
     def raw_sql_cats():
         """
         Illustrates:
         * "Raw" SQLAlchemy table queries (non-mapped objects)
         * Observe phyical column name: CategoryName_ColumnName
               * Contrast to models.py, get_cats()
         
@@ -256,15 +254,14 @@
 
     @staticmethod
     @jwt_required()
     @jsonapi_rpc(http_methods=['POST'], valid_jsonapi=False)
     def get_cats():
         db = safrs.DB
         session = db.session
-        # Security.set_user_sa()  # use to bypass authorization (also requires @admin_required)
 
         result = session.query(models.Category)
         for each_row in result:
             app_logger.debug(f'each_row: {each_row}')
         rows = util.rows_to_dict(result)
         response = {"result": rows}
         return response
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/database/customize_models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/database/db_debug.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/database/db_debug.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,17 @@
                 logic_row.log("no salesrep for this order")
             elif sales_rep.Manager is None:
                 logic_row.log("no manager for this order's salesrep")
             else:
                 logic_row.log(f'Hi, {sales_rep.Manager.FirstName} - '
                               f'Congratulate {sales_rep.FirstName} on their new order')
             category_1 = logic_row.session.query(models.Category).filter(models.Category.Id == 1).one()
-            logic_row.log("Illustrate database access (not subject to authorization)")  # not granted for user: u2
+            logic_row.log("Illustrate database access")  # not granted for user: u2
+            # Note: *Client* access is subject to authorization
+            #       *Logic* is system code, not subject to authorization
 
     Rule.commit_row_event(on_class=models.Order, calling=congratulate_sales_rep)
 
 
     """
         Simplify data entry with defaults 
     """
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/opt_locking.feature` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/opt_locking.feature`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/opt_locking.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/opt_locking.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype_nw_no_cust/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.DS_Store` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,30 @@
 	// Sets the run context to one level up instead of the .devcontainer folder.
 	"context": "..",
 
 	// Update the 'dockerFile' property if you aren't using the standard 'Dockerfile' filename.
 	"dockerFile": "For_VSCode.dockerfile",
 
 	// Set *default* container specific settings.json values on container create.
-	"settings": {},
+	// "settings": {},
 
 	// add network -- enable this as required, e.g., https://apilogicserver.github.io/Docs/Database-Connectivity/
 	// "runArgs": ["--network=dev-network"],
 
 	// Add the IDs of extensions you want installed when the container is created.
-	"extensions": ["ms-python.python"],
+	// "extensions": [],   **** Note - Python added in customizations (autoloads Python in devcontainer)
+
+	"customizations": {
+		// Configure properties specific to VS Code.
+		"vscode": {
+			// Set default container specific settings.json values on container create.
+			"settings": {},
+			"extensions": ["ms-python.python"]
+		}
+	},
 	
 	"portsAttributes": {
 		"5656": {
 			"label": "AdminApp"
 		}
 	},
 
@@ -29,22 +38,19 @@
 	
 	"features": {
 		"github-cli": "latest"
 	  },
 
 	"postAttachCommand": "/bin/bash .devcontainer/setup.sh"
 
-	// Use 'forwardPorts' to make a list of ports inside the container available locally.
-	// "forwardPorts": [],
-
 	// Uncomment the next line to run commands after the container is created - for example installing curl.
 	// "postCreateCommand": "apt-get update && apt-get install -y curl",
 
 	// Uncomment when using a ptrace-based debugger like C++, Go, and Rust
 	// "runArgs": [ "--cap-add=SYS_PTRACE", "--security-opt", "seccomp=unconfined" ],
 
 	// Uncomment to use the Docker CLI from inside the container. See https://aka.ms/vscode-remote/samples/docker-from-docker.
 	// "mounts": [ "source=/var/run/docker.sock,target=/var/run/docker.sock,type=bind" ],
 
 	// Uncomment to connect as a non-root user if you've added one. See https://aka.ms/vscode-remote/containers/non-root.
 	// "remoteUser": "vscode"
-}
+}
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/.vscode/launch.json` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/.vscode/launch.json`

 * *Files 2% similar despite different names*

```diff
@@ -134,40 +134,40 @@
             "console": "internalConsole",
             "internalConsoleOptions": "openOnSessionStart"
         },
         {
             "name": "Behave Run",
             "type": "python",
             "request": "launch",
-            "cwd": "${workspaceFolder}/3. ApiLogicProject_Logic/test/api_logic_server_behave",
+            "cwd": "${workspaceFolder}/3. Logic/test/api_logic_server_behave",
             "program": "behave_run.py",
             "redirectOutput": true,
             "args": [ "--outfile=logs/behave.log"],
             "justMyCode": false,            
             "console": "internalConsole",
             "internalConsoleOptions": "openOnSessionStart"
         },
         {
             "name": "Behave Scenario",
             "type": "python",
             "request": "launch",
-            "cwd": "${workspaceFolder}/3. ApiLogicProject_Logic/test/api_logic_server_behave",
+            "cwd": "${workspaceFolder}/3. Logic/test/api_logic_server_behave",
             "program": "behave_run.py",
             "redirectOutput": true,
             "args": [ "--outfile=logs/behave.log",
                 "--name=Clone Existing Order"],
             "justMyCode": false,            
             "console": "internalConsole",
             "internalConsoleOptions": "openOnSessionStart"
         },
         {
             "name": "Behave Logic Report",
             "type": "python",
             "request": "launch",
-            "cwd": "${workspaceFolder}/3. ApiLogicProject_Logic/test/api_logic_server_behave",
+            "cwd": "${workspaceFolder}/3. Logic/test/api_logic_server_behave",
             "program": "behave_logic_report.py",
             "redirectOutput": true,
             "justMyCode": false,            
             "args": ["run"
                 ,"--prepend_wiki=reports/Behave Logic Report Intro.md"
                 ,"--wiki=reports/Behave Logic Report.md"
             ],
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/devops/docker-compose/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/test/server_test.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/0. App_Fiddle/test/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_prototype/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,35 +214,40 @@
         list of rows as dicts
     """
     rows = []
     for each_row in result:
         row_as_dict = {}
         log(f'type(each_row): {type(each_row)}')
         if isinstance (each_row, sqlalchemy.engine.row.Row):  # raw sql, eg, sample catsql
-            key_to_index = each_row._key_to_index  # note: SQLAlchemy 2 specific
+            key_to_index = each_row._key_to_index             # note: SQLAlchemy 2 specific
             for name, value in key_to_index.items():
                 row_as_dict[name] = each_row[value]
         else:
-            row_as_dict = each_row.to_dict()
+            row_as_dict = each_row.to_dict()                  # safrs helper
         rows.append(row_as_dict)
     return rows
 
 
-def sys_info():  
+def sys_info(flask_app_config):  
     """
     Print env and path
     """  
     import os, socket
     print("\n\nsys_info here")
     print("\nEnvironment Variables...")
     env = os.environ
     for each_variable in os.environ:
             print(f'.. {each_variable} = {env[each_variable]}')
 
-    print("\nPYTHONPATH..")
+    print(f'\n\nflask_app.config: \n\t')
+    flask_app_config_str = str(flask_app_config)
+    flask_app_config_str = flask_app_config_str.replace(', ', ',\n\t')
+    print((flask_app_config_str))
+
+    print("\n\nPYTHONPATH..")
     for p in sys.path:
         print(".." + p)
         
     print("")
     print(f'sys.prefix (venv): {sys.prefix}\n')
 
     print("")
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/readme.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/project_tutorial/sample_db.sqlite` & `ApiLogicServer-9.1.32/api_logic_server_cli/project_tutorial/sample_db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9e3d9e64 (Fri Jun 30 02:27:42 2023 UTC)
+moddate:  0xf37cb864 (Thu Jul 20 00:16:51 2023 UTC)
 files sz: 18938
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6f939f64 (Sat Jul  1 02:46:07 2023 UTC)
+moddate:  0xf37cb864 (Thu Jul 20 00:16:51 2023 UTC)
 files sz: 65200
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_ga.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_ga.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_gen.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/classic_models/models_gen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegen.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX-merged.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX-merged.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenX.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenZ.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/codegen/codegenZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models_rc2.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/models_rc2.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze_rc2.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/compare_gen_vs_rc2/pip_freeze_rc2.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/delete_log.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/delete_log.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/notes.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/notes.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/nw-schema.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/als_safrs_310/nw-schema.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py` & `ApiLogicServer-9.1.32/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/templates/admin.yaml` & `ApiLogicServer-9.1.32/api_logic_server_cli/templates/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/templates/app_fiddle.md` & `ApiLogicServer-9.1.32/api_logic_server_cli/templates/app_fiddle.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/templates/app_fiddle.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/templates/app_fiddle.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/templates/index.html` & `ApiLogicServer-9.1.32/api_logic_server_cli/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/api_logic_server_cli/templates/login_endpoint.txt` & `ApiLogicServer-9.1.32/api_logic_server_cli/templates/login_endpoint.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-9.1.0/setup.py` & `ApiLogicServer-9.1.32/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,18 @@
         "Flask-Admin==1.5.7",
         "Flask-JWT-Extended==4.4.4",
         "Flask-Login==0.6.2",
         "Flask-OpenID==1.3.0",
         "python-dotenv==0.15.0",
         "email-validator==1.1.1",
         "LogicBank>=1.08.04",
-        "PyMySQL==1.0.3",
+        # https://stackoverflow.com/questions/71354710/cryptography-package-is-required-for-sha256-password-or-caching-sha2-password
+        # "PyMySQL==1.0.3[rsa]", 
+        # "PyMySQL==1.0.3+rsa",
+        "PyMySQL==1.0.3", 
         "requests==2.27.1",
         "gunicorn==20.1.0",
         "psycopg2-binary==2.9.5",
         "dotmap==1.3.25",
         "WTForms==2.3.3",
         "behave==1.2.6",
         "alembic==1.7.7",
```

