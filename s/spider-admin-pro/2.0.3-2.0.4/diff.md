# Comparing `tmp/spider-admin-pro-2.0.3.tar.gz` & `tmp/spider-admin-pro-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-admin-pro-2.0.3.tar", last modified: Fri Feb 24 03:15:36 2023, max compression
+gzip compressed data, was "spider-admin-pro-2.0.4.tar", last modified: Fri Aug  4 09:13:35 2023, max compression
```

## Comparing `spider-admin-pro-2.0.3.tar` & `spider-admin-pro-2.0.4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.667858 spider-admin-pro-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      296 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-02-24 03:15:36.667858 spider-admin-pro-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 03:15:36.667858 spider-admin-pro-2.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2211 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.655858 spider-admin-pro-2.0.3/spider_admin_pro/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api/action_history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api/schedule_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api/scrapyd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api/stats_collection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api/system_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/api_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/config/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/config/detault_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/config/yaml_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/exceptions/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/exceptions/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/model/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/model/login_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/model/schedule_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/model/stats_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/service/action_history_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/service/schedule_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/service/scrapyd_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/service/stats_collection_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/service/system_data_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/flask_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/jwt_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/scheduler_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/system_info_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/utils/time_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/web/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/web/public/
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.659858 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.663858 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/app.542ee7ed.css
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/app.d8e03581.css
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-30e10370.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-509e3c38.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-5fb2979b.71e917d9.css
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-7a44da90.7e3f4dc7.css
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-86cca1a8.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-b6dae904.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (123)   239725 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.663858 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    28200 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff
--rw-r--r--   0 runner    (1001) docker     (123)    55956 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.663858 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)    98071 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/404.a57b6f31.png
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/default.343756e6.png
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.667858 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    84762 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/app.002b3c3b.js
--rw-r--r--   0 runner    (1001) docker     (123)    84737 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/app.3697bf85.js
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js
--rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js
--rw-r--r--   0 runner    (1001) docker     (123)    20964 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js
--rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    20985 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js
--rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js
--rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js
--rw-r--r--   0 runner    (1001) docker     (123)   686796 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js
--rw-r--r--   0 runner    (1001) docker     (123)  1082917 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js
--rw-r--r--   0 runner    (1001) docker     (123)   387803 2023-02-24 03:15:28.000000 spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:15:36.655858 spider-admin-pro-2.0.3/spider_admin_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-02-24 03:15:36.000000 spider-admin-pro-2.0.3/spider_admin_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-02-24 03:15:36.000000 spider-admin-pro-2.0.3/spider_admin_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 03:15:36.000000 spider-admin-pro-2.0.3/spider_admin_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-24 03:15:36.000000 spider-admin-pro-2.0.3/spider_admin_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-24 03:15:36.000000 spider-admin-pro-2.0.3/spider_admin_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 03:15:36.000000 spider-admin-pro-2.0.3/spider_admin_pro.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.556954 spider-admin-pro-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      296 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-08-04 09:13:35.556954 spider-admin-pro-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:13:35.556954 spider-admin-pro-2.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2211 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.544953 spider-admin-pro-2.0.4/spider_admin_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.544953 spider-admin-pro-2.0.4/spider_admin_pro/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api/action_history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api/schedule_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api/scrapyd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api/stats_collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api/system_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/api_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.544953 spider-admin-pro-2.0.4/spider_admin_pro/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/config/detault_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/config/yaml_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.544953 spider-admin-pro-2.0.4/spider_admin_pro/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/exceptions/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/exceptions/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.544953 spider-admin-pro-2.0.4/spider_admin_pro/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/model/login_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/model/schedule_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/model/stats_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/service/action_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/service/schedule_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/service/scrapyd_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/service/stats_collection_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/service/system_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/flask_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/jwt_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/scheduler_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/system_info_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/utils/time_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/web/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/app.542ee7ed.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/app.d8e03581.css
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-30e10370.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-509e3c38.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-5fb2979b.71e917d9.css
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-7a44da90.7e3f4dc7.css
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-86cca1a8.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-b6dae904.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (123)   239725 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.548953 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    28200 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    55956 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.552953 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    98071 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/404.a57b6f31.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/default.343756e6.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.556954 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    84762 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/app.002b3c3b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    84737 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/app.3697bf85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20964 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20985 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   686796 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1082917 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   387803 2023-08-04 09:13:24.000000 spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:13:35.544953 spider-admin-pro-2.0.4/spider_admin_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-08-04 09:13:35.000000 spider-admin-pro-2.0.4/spider_admin_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-04 09:13:35.000000 spider-admin-pro-2.0.4/spider_admin_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:13:35.000000 spider-admin-pro-2.0.4/spider_admin_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-04 09:13:35.000000 spider-admin-pro-2.0.4/spider_admin_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 09:13:35.000000 spider-admin-pro-2.0.4/spider_admin_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:13:35.000000 spider-admin-pro-2.0.4/spider_admin_pro.egg-info/zip-safe
```

### Comparing `spider-admin-pro-2.0.3/LICENSE` & `spider-admin-pro-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/PKG-INFO` & `spider-admin-pro-2.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-admin-pro
-Version: 2.0.3
+Version: 2.0.4
 Summary: a spider admin based vue, scrapyd api and APScheduler
 Home-page: https://github.com/mouday/spider-admin-pro
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: spider admin scrapy scrapyd scheduler
 Classifier: Programming Language :: Python :: 3.7
@@ -21,41 +21,31 @@
 [![Build Status](https://app.travis-ci.com/mouday/spider-admin-pro.svg?branch=master)](https://app.travis-ci.com/mouday/spider-admin-pro)
 [![PyPI - License](https://img.shields.io/pypi/l/spider-admin-pro)](https://github.com/mouday/spider-admin-pro/blob/master/LICENSE)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/logo.png)
 
 ## 简介
 
-Spider Admin Pro 是[Spider Admin](https://github.com/mouday/SpiderAdmin)的升级版
+Spider Admin Pro 是[Spider Admin](https://github.com/mouday/SpiderAdmin)的升级版，一个可视化的Scrapy爬虫管理平台，依赖于Scrapyd
 
-1. 简化了一些功能；
-2. 优化了前端界面，基于Vue的组件化开发；
-3. 优化了后端接口，对后端项目进行了目录划分；
-4. 整体代码利于升级维护。
-5. 目前仅对Python3进行了支持
-6. 路由统一管理
-7. 全局异常捕获
-8. 接口统一返回
-9. 前后端分离
-10. 可视化参数配置
-
-Github: [https://github.com/mouday/spider-admin-pro](https://github.com/mouday/spider-admin-pro)
-
-Gitee: [https://gitee.com/mouday/spider-admin-pro](https://gitee.com/mouday/spider-admin-pro)
+- Github: [https://github.com/mouday/spider-admin-pro](https://github.com/mouday/spider-admin-pro)
+- Gitee: [https://gitee.com/mouday/spider-admin-pro](https://gitee.com/mouday/spider-admin-pro)
 
-Pypi: [https://pypi.org/project/spider-admin-pro](https://pypi.org/project/spider-admin-pro)
-
-Docker: [https://hub.docker.com/r/mouday/spider-admin-pro](https://hub.docker.com/r/mouday/spider-admin-pro)
+- Pypi: [https://pypi.org/project/spider-admin-pro](https://pypi.org/project/spider-admin-pro)
+- Docker: [https://hub.docker.com/r/mouday/spider-admin-pro](https://hub.docker.com/r/mouday/spider-admin-pro)
+- releases: [https://github.com/mouday/spider-admin-pro/releases](https://github.com/mouday/spider-admin-pro/releases)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/spider-admin-pro.png)
 
 ## 安装启动
 
 本项目基于Python3.7.0 开发，所以推荐使用Python3.7.0及其以上版本
 
+运行项目前，请先确保[scrapyd](https://pengshiyu.blog.csdn.net/article/details/79842514)服务已经启动
+
 方式一：
 
 ```bash
 $ python3 --version
 Python 3.7.0
 
 # 创建名为 venv 的虚拟环境
@@ -95,16 +85,14 @@
 # windows 以开发模式运行
 $ python3 dev.py
 
 # 以生产模式运行
 $ make pro
 ```
 
-运行项目前，请先确保[scrapyd](https://pengshiyu.blog.csdn.net/article/details/79842514)服务已经启动
-
 安装 scrapy 全家桶`[可选]`
 
 ```bash
 pip install scrapy scrapyd scrapyd-client
 ```
 
 方式三：
@@ -118,39 +106,34 @@
 > - v2.0版本移除了`.env`环境变量配置方式，仅支持yaml格式配置
 > - v2.0版本移除了`PORT`和`HOST`配置项，推荐统一采用gunicorn 管理
 
 [Spider Admin Pro V1版本文档看这里](README-v1.md)
 
 自定义配置
 
-在运行目录下新建`config.yml` 文件，运行时会自动读取该配置文件
+在运行目录下新建`config.yml` 文件，也就是执行启动命令的目录，运行时会自动读取该配置文件
+
+例如
+```bash
+$ ls
+config.yml
 
+$ gunicorn 'spider_admin_pro.main:app'
+```
 > 强烈建议：修改密码和秘钥项
 
 eg:
 
 ```yaml
 # 登录账号密码
 USERNAME: admin
 PASSWORD: "123456"
-JWT_KEY: "FU0qnuV4t8rr1pvg93NZL3DLn6sHrR1sCQqRzachbo0="
-
-# token过期时间，单位天
-EXPIRES: 7
 
 # scrapyd地址, 结尾不要加斜杆
 SCRAPYD_SERVER: "http://127.0.0.1:6800"
-
-# 日志文件夹
-LOG_DIR: 'logs'
-```
-
-生成jwt key
-```
-$ python -c 'import base64;import os;print(base64.b64encode(os.urandom(32)).decode())'
 ```
 
 ## 使用扩展
 
 收集运行日志：[scrapy-util](https://github.com/mouday/scrapy-util) 可以帮助你收集到程序运行的统计数据
 
 ## 技术栈：
@@ -228,29 +211,35 @@
 
 [x]10. 定时任务备份，不小心把任务清空
 
 [x]11. 希望能加入更好的定时方式,类似 scrapyd_web那种定时
 
 [x]12. 简单的爬虫不用非要去打包，比如我自己上传一个py文件，可以定时任务，脚本的方式运行
 
+[x]13. 爬虫能配置带参数运行
+
 ## 交流沟通
 
 关注本项目的小伙伴越来越多，为了更好地交流沟通，可以加入群聊
 
+- 一群: 1074075691（已满）
+- 二群: 864983297
+
 问题：邀请码 答案：SpiderAdmin
 
-<img src="https://github.com/mouday/spider-admin-pro/raw/master/doc/img/qq.jpg" width="300"/>
+<img src="https://github.com/mouday/spider-admin-pro/raw/master/doc/img/qq-2.jpg" width="300"/>
 
 ## 项目赞助
 
 | 日期 | 姓名 | 金额 | 
 | - | - | - |
 | 2022-04-16 | [@realhellosunsun](https://github.com/realhellosunsun) | ￥188.00
 | 2022-08-30 | [@yangxiaozhe13](https://github.com/yangxiaozhe13) | ￥88.00
 | 2022-09-01 | [@robot-2233](https://github.com/robot-2233) | ￥88.00
+| 2023-05-09 | 埃菲尔没有塔尖 | ￥68.80
 
 ## 项目截图
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/dashboard.png)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/project.png)
 
@@ -284,28 +273,61 @@
 
 同一个ip可能有被封的风险，可以使用代理ip去请求，有免费和付费。
 
 如果是个人使用，可以找一些免费的ip临时使用
 
 如果是企业项目，可以使用付费代理ip
 
-某爬虫大佬也推荐过一个不错的动态代理 [云立方](http://www.yunlifang.cn/?from=spider-admin-pro)
+某爬虫大佬也推荐过一个不错的动态代理 [云立方](http://www.yunlifang.cn?u=mouday)
 
 <a href="http://www.yunlifang.cn?u=mouday" target="_blank" style="display: inline-block; background-color: #000;">
 <img src="https://www.yunlifang.cn/user/img/720X90.png">
 </a>
 
 找客服发送暗号：【爬虫推广】可以获取打折优惠
 
 具体搭建方法在大佬的博客中有详尽说明：
 
 [使用 Tornado+Redis 维护 ADSL 拨号服务器代理池](https://cuiqingcai.com/4596.html)
 
 如果有问题，可以加QQ群，群里的小伙伴会积极解答喔
 
+3、为什么外网访问不到，如何修改端口号
+
+增加`--bind` 参数
+
+格式
+
+```bash
+--bind 监听地址:监听端口号
+```
+
+例如
+
+```bash
+# 启动运行
+$ gunicorn 'spider_admin_pro.main:app'
+
+# 支持外网可访问，云服务器（阿里云或腾讯云）需要设置安全组 
+# 默认内网访问 --bind 127.0.0.1:8000
+$ gunicorn --bind '0.0.0.0:8000' 'spider_admin_pro.main:app'
+```
+
+更多设置，可参考[gunicorn](https://docs.gunicorn.org/en/stable/index.html)
+
+4、提示缺少libfile
+
+群友 `@Yuan、红尘美` 提供的解决方法
+
+安装依赖
+
+```bash
+yum install libffi-devel -y
+```
+
 ## 更新日志
 
 - v2.0.3
     - 修复mysql作为后端存储的文档和登录bug
 
 - v2.0.2
     - 优化文档
@@ -335,7 +357,20 @@
 
 
 ## 社区其他优秀工具推荐
 
 - https://github.com/DormyMo/SpiderKeeper
 - https://github.com/my8100/scrapydweb
 - https://github.com/ouqiang/gocron 使用Go语言开发的轻量级定时任务集中调度和管理系统, 用于替代Linux-crontab
+
+## Spider Admin Pro vs. Spider Admin
+
+1. 简化了一些功能；
+2. 优化了前端界面，基于Vue的组件化开发；
+3. 优化了后端接口，对后端项目进行了目录划分；
+4. 整体代码利于升级维护。
+5. 目前仅对Python3进行了支持
+6. 路由统一管理
+7. 全局异常捕获
+8. 接口统一返回
+9. 前后端分离
+10. 可视化参数配置
```

### Comparing `spider-admin-pro-2.0.3/README.md` & `spider-admin-pro-2.0.4/spider_admin_pro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,51 @@
+Metadata-Version: 2.1
+Name: spider-admin-pro
+Version: 2.0.4
+Summary: a spider admin based vue, scrapyd api and APScheduler
+Home-page: https://github.com/mouday/spider-admin-pro
+Author: Peng Shiyu
+Author-email: pengshiyuyx@gmail.com
+License: MIT
+Keywords: spider admin scrapy scrapyd scheduler
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Spider Admin Pro
 
 [![PyPI](https://img.shields.io/pypi/v/spider-admin-pro.svg)](https://pypi.org/project/spider-admin-pro)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/spider-admin-pro)](https://pypi.org/project/spider-admin-pro)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spider-admin-pro)](https://pypi.org/project/spider-admin-pro)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/mouday/spider-admin-pro?label=docker%20version&sort=semver)](https://hub.docker.com/r/mouday/spider-admin-pro)
 [![Docker Pulls](https://img.shields.io/docker/pulls/mouday/spider-admin-pro)](https://app.travis-ci.com/mouday/spider-admin-pro)
 [![Build Status](https://app.travis-ci.com/mouday/spider-admin-pro.svg?branch=master)](https://app.travis-ci.com/mouday/spider-admin-pro)
 [![PyPI - License](https://img.shields.io/pypi/l/spider-admin-pro)](https://github.com/mouday/spider-admin-pro/blob/master/LICENSE)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/logo.png)
 
 ## 简介
 
-Spider Admin Pro 是[Spider Admin](https://github.com/mouday/SpiderAdmin)的升级版
+Spider Admin Pro 是[Spider Admin](https://github.com/mouday/SpiderAdmin)的升级版，一个可视化的Scrapy爬虫管理平台，依赖于Scrapyd
 
-1. 简化了一些功能；
-2. 优化了前端界面，基于Vue的组件化开发；
-3. 优化了后端接口，对后端项目进行了目录划分；
-4. 整体代码利于升级维护。
-5. 目前仅对Python3进行了支持
-6. 路由统一管理
-7. 全局异常捕获
-8. 接口统一返回
-9. 前后端分离
-10. 可视化参数配置
-
-Github: [https://github.com/mouday/spider-admin-pro](https://github.com/mouday/spider-admin-pro)
+- Github: [https://github.com/mouday/spider-admin-pro](https://github.com/mouday/spider-admin-pro)
+- Gitee: [https://gitee.com/mouday/spider-admin-pro](https://gitee.com/mouday/spider-admin-pro)
 
-Gitee: [https://gitee.com/mouday/spider-admin-pro](https://gitee.com/mouday/spider-admin-pro)
-
-Pypi: [https://pypi.org/project/spider-admin-pro](https://pypi.org/project/spider-admin-pro)
-
-Docker: [https://hub.docker.com/r/mouday/spider-admin-pro](https://hub.docker.com/r/mouday/spider-admin-pro)
+- Pypi: [https://pypi.org/project/spider-admin-pro](https://pypi.org/project/spider-admin-pro)
+- Docker: [https://hub.docker.com/r/mouday/spider-admin-pro](https://hub.docker.com/r/mouday/spider-admin-pro)
+- releases: [https://github.com/mouday/spider-admin-pro/releases](https://github.com/mouday/spider-admin-pro/releases)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/spider-admin-pro.png)
 
 ## 安装启动
 
 本项目基于Python3.7.0 开发，所以推荐使用Python3.7.0及其以上版本
 
+运行项目前，请先确保[scrapyd](https://pengshiyu.blog.csdn.net/article/details/79842514)服务已经启动
+
 方式一：
 
 ```bash
 $ python3 --version
 Python 3.7.0
 
 # 创建名为 venv 的虚拟环境
@@ -82,16 +85,14 @@
 # windows 以开发模式运行
 $ python3 dev.py
 
 # 以生产模式运行
 $ make pro
 ```
 
-运行项目前，请先确保[scrapyd](https://pengshiyu.blog.csdn.net/article/details/79842514)服务已经启动
-
 安装 scrapy 全家桶`[可选]`
 
 ```bash
 pip install scrapy scrapyd scrapyd-client
 ```
 
 方式三：
@@ -105,39 +106,34 @@
 > - v2.0版本移除了`.env`环境变量配置方式，仅支持yaml格式配置
 > - v2.0版本移除了`PORT`和`HOST`配置项，推荐统一采用gunicorn 管理
 
 [Spider Admin Pro V1版本文档看这里](README-v1.md)
 
 自定义配置
 
-在运行目录下新建`config.yml` 文件，运行时会自动读取该配置文件
+在运行目录下新建`config.yml` 文件，也就是执行启动命令的目录，运行时会自动读取该配置文件
+
+例如
+```bash
+$ ls
+config.yml
 
+$ gunicorn 'spider_admin_pro.main:app'
+```
 > 强烈建议：修改密码和秘钥项
 
 eg:
 
 ```yaml
 # 登录账号密码
 USERNAME: admin
 PASSWORD: "123456"
-JWT_KEY: "FU0qnuV4t8rr1pvg93NZL3DLn6sHrR1sCQqRzachbo0="
-
-# token过期时间，单位天
-EXPIRES: 7
 
 # scrapyd地址, 结尾不要加斜杆
 SCRAPYD_SERVER: "http://127.0.0.1:6800"
-
-# 日志文件夹
-LOG_DIR: 'logs'
-```
-
-生成jwt key
-```
-$ python -c 'import base64;import os;print(base64.b64encode(os.urandom(32)).decode())'
 ```
 
 ## 使用扩展
 
 收集运行日志：[scrapy-util](https://github.com/mouday/scrapy-util) 可以帮助你收集到程序运行的统计数据
 
 ## 技术栈：
@@ -215,29 +211,35 @@
 
 [x]10. 定时任务备份，不小心把任务清空
 
 [x]11. 希望能加入更好的定时方式,类似 scrapyd_web那种定时
 
 [x]12. 简单的爬虫不用非要去打包，比如我自己上传一个py文件，可以定时任务，脚本的方式运行
 
+[x]13. 爬虫能配置带参数运行
+
 ## 交流沟通
 
 关注本项目的小伙伴越来越多，为了更好地交流沟通，可以加入群聊
 
+- 一群: 1074075691（已满）
+- 二群: 864983297
+
 问题：邀请码 答案：SpiderAdmin
 
-<img src="https://github.com/mouday/spider-admin-pro/raw/master/doc/img/qq.jpg" width="300"/>
+<img src="https://github.com/mouday/spider-admin-pro/raw/master/doc/img/qq-2.jpg" width="300"/>
 
 ## 项目赞助
 
 | 日期 | 姓名 | 金额 | 
 | - | - | - |
 | 2022-04-16 | [@realhellosunsun](https://github.com/realhellosunsun) | ￥188.00
 | 2022-08-30 | [@yangxiaozhe13](https://github.com/yangxiaozhe13) | ￥88.00
 | 2022-09-01 | [@robot-2233](https://github.com/robot-2233) | ￥88.00
+| 2023-05-09 | 埃菲尔没有塔尖 | ￥68.80
 
 ## 项目截图
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/dashboard.png)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/project.png)
 
@@ -271,28 +273,61 @@
 
 同一个ip可能有被封的风险，可以使用代理ip去请求，有免费和付费。
 
 如果是个人使用，可以找一些免费的ip临时使用
 
 如果是企业项目，可以使用付费代理ip
 
-某爬虫大佬也推荐过一个不错的动态代理 [云立方](http://www.yunlifang.cn/?from=spider-admin-pro)
+某爬虫大佬也推荐过一个不错的动态代理 [云立方](http://www.yunlifang.cn?u=mouday)
 
 <a href="http://www.yunlifang.cn?u=mouday" target="_blank" style="display: inline-block; background-color: #000;">
 <img src="https://www.yunlifang.cn/user/img/720X90.png">
 </a>
 
 找客服发送暗号：【爬虫推广】可以获取打折优惠
 
 具体搭建方法在大佬的博客中有详尽说明：
 
 [使用 Tornado+Redis 维护 ADSL 拨号服务器代理池](https://cuiqingcai.com/4596.html)
 
 如果有问题，可以加QQ群，群里的小伙伴会积极解答喔
 
+3、为什么外网访问不到，如何修改端口号
+
+增加`--bind` 参数
+
+格式
+
+```bash
+--bind 监听地址:监听端口号
+```
+
+例如
+
+```bash
+# 启动运行
+$ gunicorn 'spider_admin_pro.main:app'
+
+# 支持外网可访问，云服务器（阿里云或腾讯云）需要设置安全组 
+# 默认内网访问 --bind 127.0.0.1:8000
+$ gunicorn --bind '0.0.0.0:8000' 'spider_admin_pro.main:app'
+```
+
+更多设置，可参考[gunicorn](https://docs.gunicorn.org/en/stable/index.html)
+
+4、提示缺少libfile
+
+群友 `@Yuan、红尘美` 提供的解决方法
+
+安装依赖
+
+```bash
+yum install libffi-devel -y
+```
+
 ## 更新日志
 
 - v2.0.3
     - 修复mysql作为后端存储的文档和登录bug
 
 - v2.0.2
     - 优化文档
@@ -322,7 +357,20 @@
 
 
 ## 社区其他优秀工具推荐
 
 - https://github.com/DormyMo/SpiderKeeper
 - https://github.com/my8100/scrapydweb
 - https://github.com/ouqiang/gocron 使用Go语言开发的轻量级定时任务集中调度和管理系统, 用于替代Linux-crontab
+
+## Spider Admin Pro vs. Spider Admin
+
+1. 简化了一些功能；
+2. 优化了前端界面，基于Vue的组件化开发；
+3. 优化了后端接口，对后端项目进行了目录划分；
+4. 整体代码利于升级维护。
+5. 目前仅对Python3进行了支持
+6. 路由统一管理
+7. 全局异常捕获
+8. 接口统一返回
+9. 前后端分离
+10. 可视化参数配置
```

### Comparing `spider-admin-pro-2.0.3/setup.py` & `spider-admin-pro-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/api/action_history_api.py` & `spider-admin-pro-2.0.4/spider_admin_pro/api/action_history_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/api/auth_api.py` & `spider-admin-pro-2.0.4/spider_admin_pro/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/api/schedule_api.py` & `spider-admin-pro-2.0.4/spider_admin_pro/api/schedule_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/api/scrapyd_api.py` & `spider-admin-pro-2.0.4/spider_admin_pro/api/scrapyd_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/api/stats_collection_api.py` & `spider-admin-pro-2.0.4/spider_admin_pro/api/stats_collection_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/api/system_info_api.py` & `spider-admin-pro-2.0.4/spider_admin_pro/api/system_info_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/api_result.py` & `spider-admin-pro-2.0.4/spider_admin_pro/api_result.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/config/detault_config.py` & `spider-admin-pro-2.0.4/spider_admin_pro/config/detault_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 
 #################################
 # 默认变量
 #################################
 
 # 登录账号密码
+from spider_admin_pro.utils import secret_util
+
 BASIC_AUTH_USERNAME = "admin"
 BASIC_AUTH_PASSWORD = "123456"
-BASIC_AUTH_JWT_KEY = 'FU0qnuV4t8rr1pvg93NZL3DLn6sHrR1sCQqRzachbo0='
+BASIC_AUTH_JWT_KEY = secret_util.get_random_secret()
 
 # token过期时间，单位天
 BASIC_AUTH_EXPIRES = 7
 
 # scrapyd地址, 结尾不要加斜杆
 SCRAPYD_SERVER = 'http://127.0.0.1:6800'
```

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/config/yaml_config.py` & `spider-admin-pro-2.0.4/spider_admin_pro/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/main.py` & `spider-admin-pro-2.0.4/spider_admin_pro/main.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/model/base.py` & `spider-admin-pro-2.0.4/spider_admin_pro/model/base.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/model/login_history_model.py` & `spider-admin-pro-2.0.4/spider_admin_pro/model/login_history_model.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/model/schedule_history_model.py` & `spider-admin-pro-2.0.4/spider_admin_pro/model/schedule_history_model.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/model/stats_collection_model.py` & `spider-admin-pro-2.0.4/spider_admin_pro/model/stats_collection_model.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/router.py` & `spider-admin-pro-2.0.4/spider_admin_pro/router.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/service/action_history_service.py` & `spider-admin-pro-2.0.4/spider_admin_pro/service/action_history_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/service/auth_service.py` & `spider-admin-pro-2.0.4/spider_admin_pro/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/service/schedule_service.py` & `spider-admin-pro-2.0.4/spider_admin_pro/service/schedule_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 make_sqlite_dir(JOB_STORES_DATABASE_URL)
 
 JOBSTORES = {
     'default': SQLAlchemyJobStore(url=JOB_STORES_DATABASE_URL)
 }
 
 JOB_DEFAULTS = {
+    'misfire_grace_time': None,
     'coalesce': True,
     'max_instances': 1
 }
 
 scheduler = BackgroundScheduler(jobstores=JOBSTORES, job_defaults=JOB_DEFAULTS)
 
 scheduler.start()
```

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/service/scrapyd_service.py` & `spider-admin-pro-2.0.4/spider_admin_pro/service/scrapyd_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/service/stats_collection_service.py` & `spider-admin-pro-2.0.4/spider_admin_pro/service/stats_collection_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/service/system_data_service.py` & `spider-admin-pro-2.0.4/spider_admin_pro/service/system_data_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/utils/flask_ext/flask_app.py` & `spider-admin-pro-2.0.4/spider_admin_pro/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/utils/jwt_util.py` & `spider-admin-pro-2.0.4/spider_admin_pro/utils/jwt_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/utils/scheduler_util.py` & `spider-admin-pro-2.0.4/spider_admin_pro/utils/scheduler_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/utils/sqlite_util.py` & `spider-admin-pro-2.0.4/spider_admin_pro/utils/sqlite_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/utils/system_info_util.py` & `spider-admin-pro-2.0.4/spider_admin_pro/utils/system_info_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/utils/time_util.py` & `spider-admin-pro-2.0.4/spider_admin_pro/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/index.html` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/index.html`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/app.542ee7ed.css` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/app.542ee7ed.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/app.d8e03581.css` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/app.d8e03581.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/favicon.ico` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/404.a57b6f31.png` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/404.a57b6f31.png`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/default.343756e6.png` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/default.343756e6.png`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/app.002b3c3b.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/app.002b3c3b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/app.3697bf85.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/app.3697bf85.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js` & `spider-admin-pro-2.0.4/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro.egg-info/PKG-INFO` & `spider-admin-pro-2.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,38 @@
-Metadata-Version: 2.1
-Name: spider-admin-pro
-Version: 2.0.3
-Summary: a spider admin based vue, scrapyd api and APScheduler
-Home-page: https://github.com/mouday/spider-admin-pro
-Author: Peng Shiyu
-Author-email: pengshiyuyx@gmail.com
-License: MIT
-Keywords: spider admin scrapy scrapyd scheduler
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Spider Admin Pro
 
 [![PyPI](https://img.shields.io/pypi/v/spider-admin-pro.svg)](https://pypi.org/project/spider-admin-pro)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/spider-admin-pro)](https://pypi.org/project/spider-admin-pro)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spider-admin-pro)](https://pypi.org/project/spider-admin-pro)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/mouday/spider-admin-pro?label=docker%20version&sort=semver)](https://hub.docker.com/r/mouday/spider-admin-pro)
 [![Docker Pulls](https://img.shields.io/docker/pulls/mouday/spider-admin-pro)](https://app.travis-ci.com/mouday/spider-admin-pro)
 [![Build Status](https://app.travis-ci.com/mouday/spider-admin-pro.svg?branch=master)](https://app.travis-ci.com/mouday/spider-admin-pro)
 [![PyPI - License](https://img.shields.io/pypi/l/spider-admin-pro)](https://github.com/mouday/spider-admin-pro/blob/master/LICENSE)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/logo.png)
 
 ## 简介
 
-Spider Admin Pro 是[Spider Admin](https://github.com/mouday/SpiderAdmin)的升级版
+Spider Admin Pro 是[Spider Admin](https://github.com/mouday/SpiderAdmin)的升级版，一个可视化的Scrapy爬虫管理平台，依赖于Scrapyd
 
-1. 简化了一些功能；
-2. 优化了前端界面，基于Vue的组件化开发；
-3. 优化了后端接口，对后端项目进行了目录划分；
-4. 整体代码利于升级维护。
-5. 目前仅对Python3进行了支持
-6. 路由统一管理
-7. 全局异常捕获
-8. 接口统一返回
-9. 前后端分离
-10. 可视化参数配置
-
-Github: [https://github.com/mouday/spider-admin-pro](https://github.com/mouday/spider-admin-pro)
+- Github: [https://github.com/mouday/spider-admin-pro](https://github.com/mouday/spider-admin-pro)
+- Gitee: [https://gitee.com/mouday/spider-admin-pro](https://gitee.com/mouday/spider-admin-pro)
 
-Gitee: [https://gitee.com/mouday/spider-admin-pro](https://gitee.com/mouday/spider-admin-pro)
-
-Pypi: [https://pypi.org/project/spider-admin-pro](https://pypi.org/project/spider-admin-pro)
-
-Docker: [https://hub.docker.com/r/mouday/spider-admin-pro](https://hub.docker.com/r/mouday/spider-admin-pro)
+- Pypi: [https://pypi.org/project/spider-admin-pro](https://pypi.org/project/spider-admin-pro)
+- Docker: [https://hub.docker.com/r/mouday/spider-admin-pro](https://hub.docker.com/r/mouday/spider-admin-pro)
+- releases: [https://github.com/mouday/spider-admin-pro/releases](https://github.com/mouday/spider-admin-pro/releases)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/spider-admin-pro.png)
 
 ## 安装启动
 
 本项目基于Python3.7.0 开发，所以推荐使用Python3.7.0及其以上版本
 
+运行项目前，请先确保[scrapyd](https://pengshiyu.blog.csdn.net/article/details/79842514)服务已经启动
+
 方式一：
 
 ```bash
 $ python3 --version
 Python 3.7.0
 
 # 创建名为 venv 的虚拟环境
@@ -95,16 +72,14 @@
 # windows 以开发模式运行
 $ python3 dev.py
 
 # 以生产模式运行
 $ make pro
 ```
 
-运行项目前，请先确保[scrapyd](https://pengshiyu.blog.csdn.net/article/details/79842514)服务已经启动
-
 安装 scrapy 全家桶`[可选]`
 
 ```bash
 pip install scrapy scrapyd scrapyd-client
 ```
 
 方式三：
@@ -118,39 +93,34 @@
 > - v2.0版本移除了`.env`环境变量配置方式，仅支持yaml格式配置
 > - v2.0版本移除了`PORT`和`HOST`配置项，推荐统一采用gunicorn 管理
 
 [Spider Admin Pro V1版本文档看这里](README-v1.md)
 
 自定义配置
 
-在运行目录下新建`config.yml` 文件，运行时会自动读取该配置文件
+在运行目录下新建`config.yml` 文件，也就是执行启动命令的目录，运行时会自动读取该配置文件
+
+例如
+```bash
+$ ls
+config.yml
 
+$ gunicorn 'spider_admin_pro.main:app'
+```
 > 强烈建议：修改密码和秘钥项
 
 eg:
 
 ```yaml
 # 登录账号密码
 USERNAME: admin
 PASSWORD: "123456"
-JWT_KEY: "FU0qnuV4t8rr1pvg93NZL3DLn6sHrR1sCQqRzachbo0="
-
-# token过期时间，单位天
-EXPIRES: 7
 
 # scrapyd地址, 结尾不要加斜杆
 SCRAPYD_SERVER: "http://127.0.0.1:6800"
-
-# 日志文件夹
-LOG_DIR: 'logs'
-```
-
-生成jwt key
-```
-$ python -c 'import base64;import os;print(base64.b64encode(os.urandom(32)).decode())'
 ```
 
 ## 使用扩展
 
 收集运行日志：[scrapy-util](https://github.com/mouday/scrapy-util) 可以帮助你收集到程序运行的统计数据
 
 ## 技术栈：
@@ -228,29 +198,35 @@
 
 [x]10. 定时任务备份，不小心把任务清空
 
 [x]11. 希望能加入更好的定时方式,类似 scrapyd_web那种定时
 
 [x]12. 简单的爬虫不用非要去打包，比如我自己上传一个py文件，可以定时任务，脚本的方式运行
 
+[x]13. 爬虫能配置带参数运行
+
 ## 交流沟通
 
 关注本项目的小伙伴越来越多，为了更好地交流沟通，可以加入群聊
 
+- 一群: 1074075691（已满）
+- 二群: 864983297
+
 问题：邀请码 答案：SpiderAdmin
 
-<img src="https://github.com/mouday/spider-admin-pro/raw/master/doc/img/qq.jpg" width="300"/>
+<img src="https://github.com/mouday/spider-admin-pro/raw/master/doc/img/qq-2.jpg" width="300"/>
 
 ## 项目赞助
 
 | 日期 | 姓名 | 金额 | 
 | - | - | - |
 | 2022-04-16 | [@realhellosunsun](https://github.com/realhellosunsun) | ￥188.00
 | 2022-08-30 | [@yangxiaozhe13](https://github.com/yangxiaozhe13) | ￥88.00
 | 2022-09-01 | [@robot-2233](https://github.com/robot-2233) | ￥88.00
+| 2023-05-09 | 埃菲尔没有塔尖 | ￥68.80
 
 ## 项目截图
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/dashboard.png)
 
 ![](https://github.com/mouday/spider-admin-pro/raw/master/doc/img/project.png)
 
@@ -284,28 +260,61 @@
 
 同一个ip可能有被封的风险，可以使用代理ip去请求，有免费和付费。
 
 如果是个人使用，可以找一些免费的ip临时使用
 
 如果是企业项目，可以使用付费代理ip
 
-某爬虫大佬也推荐过一个不错的动态代理 [云立方](http://www.yunlifang.cn/?from=spider-admin-pro)
+某爬虫大佬也推荐过一个不错的动态代理 [云立方](http://www.yunlifang.cn?u=mouday)
 
 <a href="http://www.yunlifang.cn?u=mouday" target="_blank" style="display: inline-block; background-color: #000;">
 <img src="https://www.yunlifang.cn/user/img/720X90.png">
 </a>
 
 找客服发送暗号：【爬虫推广】可以获取打折优惠
 
 具体搭建方法在大佬的博客中有详尽说明：
 
 [使用 Tornado+Redis 维护 ADSL 拨号服务器代理池](https://cuiqingcai.com/4596.html)
 
 如果有问题，可以加QQ群，群里的小伙伴会积极解答喔
 
+3、为什么外网访问不到，如何修改端口号
+
+增加`--bind` 参数
+
+格式
+
+```bash
+--bind 监听地址:监听端口号
+```
+
+例如
+
+```bash
+# 启动运行
+$ gunicorn 'spider_admin_pro.main:app'
+
+# 支持外网可访问，云服务器（阿里云或腾讯云）需要设置安全组 
+# 默认内网访问 --bind 127.0.0.1:8000
+$ gunicorn --bind '0.0.0.0:8000' 'spider_admin_pro.main:app'
+```
+
+更多设置，可参考[gunicorn](https://docs.gunicorn.org/en/stable/index.html)
+
+4、提示缺少libfile
+
+群友 `@Yuan、红尘美` 提供的解决方法
+
+安装依赖
+
+```bash
+yum install libffi-devel -y
+```
+
 ## 更新日志
 
 - v2.0.3
     - 修复mysql作为后端存储的文档和登录bug
 
 - v2.0.2
     - 优化文档
@@ -335,7 +344,20 @@
 
 
 ## 社区其他优秀工具推荐
 
 - https://github.com/DormyMo/SpiderKeeper
 - https://github.com/my8100/scrapydweb
 - https://github.com/ouqiang/gocron 使用Go语言开发的轻量级定时任务集中调度和管理系统, 用于替代Linux-crontab
+
+## Spider Admin Pro vs. Spider Admin
+
+1. 简化了一些功能；
+2. 优化了前端界面，基于Vue的组件化开发；
+3. 优化了后端接口，对后端项目进行了目录划分；
+4. 整体代码利于升级维护。
+5. 目前仅对Python3进行了支持
+6. 路由统一管理
+7. 全局异常捕获
+8. 接口统一返回
+9. 前后端分离
+10. 可视化参数配置
```

### Comparing `spider-admin-pro-2.0.3/spider_admin_pro.egg-info/SOURCES.txt` & `spider-admin-pro-2.0.4/spider_admin_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

