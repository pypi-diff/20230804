# Comparing `tmp/jupyterlab_pachyderm-2.7.0rc1.tar.gz` & `tmp/jupyterlab_pachyderm-2.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.7.0rc1.tar", last modified: Wed Jul 26 23:18:54 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.7.0rc2.tar", last modified: Fri Aug  4 16:07:55 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.7.0rc1.tar` & `jupyterlab_pachyderm-2.7.0rc2.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.120399 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.128399 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.128399 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.132399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.132399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4409 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.136399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   163203 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/199.6f6cc83faa1bc2d85def.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8290 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/remoteEntry.62cd8a8c852e71b919b6.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-07-26 23:18:41.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-07-26 23:18:52.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11122 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10621 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17660 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.132399 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 23:18:25.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-26 23:18:54.000000 jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-07-26 23:16:19.000000 jupyterlab_pachyderm-2.7.0rc1/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.140399 jupyterlab_pachyderm-2.7.0rc1/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.144399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8762 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Pipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Splash.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5160 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2920 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.124399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.148399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 23:18:54.152399 jupyterlab_pachyderm-2.7.0rc1/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-07-26 23:16:18.000000 jupyterlab_pachyderm-2.7.0rc1/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.334130 jupyterlab_pachyderm-2.7.0rc2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-08-04 16:07:55.334130 jupyterlab_pachyderm-2.7.0rc2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.306130 jupyterlab_pachyderm-2.7.0rc2/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.314130 jupyterlab_pachyderm-2.7.0rc2/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.314130 jupyterlab_pachyderm-2.7.0rc2/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.318130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.318130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4409 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.306130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.318130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-08-04 16:07:42.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-08-04 16:07:42.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-08-04 16:07:42.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-08-04 16:07:42.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-08-04 16:07:42.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.322130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163203 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/199.6f6cc83faa1bc2d85def.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8290 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/remoteEntry.e5d243832cca43abee35.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-08-04 16:07:42.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-08-04 16:07:52.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11122 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10621 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.322130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.322130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17660 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.318130 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-08-04 16:07:55.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-08-04 16:07:55.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-04 16:07:55.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-04 16:07:25.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-08-04 16:07:55.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-04 16:07:55.000000 jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-08-04 16:05:22.000000 jupyterlab_pachyderm-2.7.0rc2/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-08-04 16:07:55.334130 jupyterlab_pachyderm-2.7.0rc2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.310130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.310130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.326130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8762 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/Pipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/Splash.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5160 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2920 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.310130 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.330130 jupyterlab_pachyderm-2.7.0rc2/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.334130 jupyterlab_pachyderm-2.7.0rc2/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.334130 jupyterlab_pachyderm-2.7.0rc2/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-04 16:07:55.334130 jupyterlab_pachyderm-2.7.0rc2/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-08-04 16:05:21.000000 jupyterlab_pachyderm-2.7.0rc2/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/LICENSE` & `jupyterlab_pachyderm-2.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/MANIFEST.in` & `jupyterlab_pachyderm-2.7.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/PKG-INFO` & `jupyterlab_pachyderm-2.7.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.7.0rc1
+Version: 2.7.0rc2
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/README.md` & `jupyterlab_pachyderm-2.7.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758597883597885%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e5d243832cca43abee35.js'}}",*

 * * "'version'": "'2.7.0-rc.2'"}*

```diff
@@ -68,15 +68,15 @@
                 "npm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.62cd8a8c852e71b919b6.js",
+            "load": "static/remoteEntry.e5d243832cca43abee35.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
@@ -133,9 +133,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-rc.1"
+    "version": "2.7.0-rc.2"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.7.0-rc.2'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-rc.1"
+    "version": "2.7.0-rc.2"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/199.6f6cc83faa1bc2d85def.js` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/199.6f6cc83faa1bc2d85def.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/remoteEntry.62cd8a8c852e71b919b6.js` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/remoteEntry.e5d243832cca43abee35.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -116,15 +116,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-rc.1", (() => Promise.all([j.e(371), j.e(199)]).then((() => () => j(843))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-rc.2", (() => Promise.all([j.e(371), j.e(199)]).then((() => () => j(843))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/mount_server_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/pps_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-pachyderm
-Version: 2.7.0rc1
+Version: 2.7.0rc2
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.7.0rc2/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.62cd8a8c852e71b919b6.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.e5d243832cca43abee35.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 jupyterlab_pachyderm/tests/data/requirements.txt
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/package.json` & `jupyterlab_pachyderm-2.7.0rc2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.7.0-rc.2'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-rc.1"
+    "version": "2.7.0-rc.2"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0rc1/pyproject.toml` & `jupyterlab_pachyderm-2.7.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/setup.cfg` & `jupyterlab_pachyderm-2.7.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/setup.py` & `jupyterlab_pachyderm-2.7.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/handler.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/Splash.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/Splash.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/mount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/mount/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/src/utils/icons.ts` & `jupyterlab_pachyderm-2.7.0rc2/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/style/base.css` & `jupyterlab_pachyderm-2.7.0rc2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/style/components/button.css` & `jupyterlab_pachyderm-2.7.0rc2/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/style/icons/file.svg` & `jupyterlab_pachyderm-2.7.0rc2/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/style/icons/info.svg` & `jupyterlab_pachyderm-2.7.0rc2/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.7.0rc2/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0rc1/style/icons/repo.svg` & `jupyterlab_pachyderm-2.7.0rc2/style/icons/repo.svg`

 * *Files identical despite different names*

