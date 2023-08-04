# Comparing `tmp/seaplane-0.3.9.tar.gz` & `tmp/seaplane-0.3.90b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.3.9.tar", max compression
+gzip compressed data, was "seaplane-0.3.90b0.tar", max compression
```

## Comparing `seaplane-0.3.9.tar` & `seaplane-0.3.90b0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.9/README.md
--rw-r--r--   0        0        0     2682 2023-06-08 16:33:33.572139 seaplane-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     1178 2023-06-08 15:19:56.475350 seaplane-0.3.9/src/seaplane/__init__.py
--rw-r--r--   0        0        0      106 2023-06-07 13:57:55.120996 seaplane-0.3.9/src/seaplane/api/__init__.py
--rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.9/src/seaplane/api/api_http.py
--rw-r--r--   0        0        0     2558 2023-06-07 11:17:31.773475 seaplane-0.3.9/src/seaplane/api/api_request.py
--rw-r--r--   0        0        0     2987 2023-06-07 11:17:31.773747 seaplane-0.3.9/src/seaplane/api/compute_api.py
--rw-r--r--   0        0        0     3158 2023-06-07 11:17:31.774043 seaplane-0.3.9/src/seaplane/api/formation_configuration_api.py
--rw-r--r--   0        0        0     7410 2023-06-07 11:17:31.774348 seaplane-0.3.9/src/seaplane/api/lock_api.py
--rw-r--r--   0        0        0     5806 2023-06-07 11:17:31.774586 seaplane-0.3.9/src/seaplane/api/metadata_api.py
--rw-r--r--   0        0        0     7724 2023-06-07 11:17:31.774882 seaplane-0.3.9/src/seaplane/api/restrict_api.py
--rw-r--r--   0        0        0     1552 2023-06-07 11:17:31.775138 seaplane-0.3.9/src/seaplane/api/sql_api.py
--rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.9/src/seaplane/api/token_api.py
--rw-r--r--   0        0        0       57 2023-06-08 15:27:56.714791 seaplane-0.3.9/src/seaplane/carrier/__init__.py
--rw-r--r--   0        0        0     2401 2023-06-08 15:27:17.021086 seaplane-0.3.9/src/seaplane/carrier/processor.py
--rw-r--r--   0        0        0     8148 2023-06-08 16:06:32.018960 seaplane-0.3.9/src/seaplane/configuration.py
--rw-r--r--   0        0        0     1818 2023-06-05 16:13:40.927293 seaplane-0.3.9/src/seaplane/logging/__init__.py
--rw-r--r--   0        0        0      334 2023-06-07 13:57:55.121524 seaplane-0.3.9/src/seaplane/model/__init__.py
--rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.9/src/seaplane/model/compute/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.9/src/seaplane/model/compute/formation_configuration.py
--rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.9/src/seaplane/model/compute/formation_metadata.py
--rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.9/src/seaplane/model/errors.py
--rw-r--r--   0        0        0     3077 2023-06-07 11:17:31.775418 seaplane-0.3.9/src/seaplane/model/locks/__init__.py
--rw-r--r--   0        0        0     3560 2023-06-07 11:17:31.775652 seaplane-0.3.9/src/seaplane/model/metadata/__init__.py
--rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.9/src/seaplane/model/provider.py
--rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.9/src/seaplane/model/region.py
--rw-r--r--   0        0        0     4221 2023-06-07 11:17:31.775895 seaplane-0.3.9/src/seaplane/model/restrict/__init__.py
--rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.9/src/seaplane/model/sql/__init__.py
--rw-r--r--   0        0        0      313 2023-06-08 15:19:30.007796 seaplane-0.3.9/src/seaplane/smartpipes/__init__.py
--rw-r--r--   0        0        0     1521 2023-06-08 15:18:22.874342 seaplane-0.3.9/src/seaplane/smartpipes/build.py
--rw-r--r--   0        0        0     2756 2023-06-07 14:00:21.738111 seaplane-0.3.9/src/seaplane/smartpipes/coprocessor.py
--rw-r--r--   0        0        0      166 2023-06-07 13:57:55.122029 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/__init__.py
--rw-r--r--   0        0        0     1827 2023-06-07 13:57:55.122241 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/bloom.py
--rw-r--r--   0        0        0     3242 2023-06-07 13:57:55.122396 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/openai.py
--rw-r--r--   0        0        0     4054 2023-06-07 13:57:55.122622 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/pinecone.py
--rw-r--r--   0        0        0     3164 2023-06-07 13:57:55.122771 seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/replicate.py
--rw-r--r--   0        0        0     7131 2023-06-08 06:15:04.301952 seaplane-0.3.9/src/seaplane/smartpipes/decorators.py
--rw-r--r--   0        0        0     6081 2023-06-08 16:19:46.270911 seaplane-0.3.9/src/seaplane/smartpipes/deploy.py
--rw-r--r--   0        0        0     2364 2023-06-07 14:02:48.693793 seaplane-0.3.9/src/seaplane/smartpipes/event_handler.py
--rw-r--r--   0        0        0     1639 2023-06-07 14:17:11.058070 seaplane-0.3.9/src/seaplane/smartpipes/executor.py
--rw-r--r--   0        0        0     3495 2023-06-08 16:33:17.244291 seaplane-0.3.9/src/seaplane/smartpipes/smartapi.py
--rw-r--r--   0        0        0     2090 2023-06-07 13:59:40.996093 seaplane-0.3.9/src/seaplane/smartpipes/smartpipe.py
--rw-r--r--   0        0        0       33 2023-06-05 16:13:40.929884 seaplane-0.3.9/src/seaplane/smartpipes/website/.gitignore
--rw-r--r--   0        0        0     1750 2023-06-05 16:13:40.930353 seaplane-0.3.9/src/seaplane/smartpipes/website/README.md
--rw-r--r--   0        0        0       77 2023-06-05 16:13:40.930859 seaplane-0.3.9/src/seaplane/smartpipes/website/jsconfig.json
--rw-r--r--   0        0        0      118 2023-06-05 16:13:40.931524 seaplane-0.3.9/src/seaplane/smartpipes/website/next.config.js
--rw-r--r--   0        0        0      650 2023-06-05 16:13:40.932082 seaplane-0.3.9/src/seaplane/smartpipes/website/package.json
--rw-r--r--   0        0        0       82 2023-06-05 16:13:40.932489 seaplane-0.3.9/src/seaplane/smartpipes/website/postcss.config.js
--rw-r--r--   0        0        0      717 2023-06-05 16:13:40.933215 seaplane-0.3.9/src/seaplane/smartpipes/website/public/favicon.ico
--rw-r--r--   0        0        0     1375 2023-06-05 16:13:40.933596 seaplane-0.3.9/src/seaplane/smartpipes/website/public/next.svg
--rw-r--r--   0        0        0    39147 2023-06-05 16:13:40.934215 seaplane-0.3.9/src/seaplane/smartpipes/website/public/openai.png
--rw-r--r--   0        0        0    11580 2023-06-05 16:13:40.934926 seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo.svg
--rw-r--r--   0        0        0     2296 2023-06-05 16:13:40.935333 seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
--rw-r--r--   0        0        0   195272 2023-06-05 16:13:40.938647 seaplane-0.3.9/src/seaplane/smartpipes/website/public/stabilityai.png
--rw-r--r--   0        0        0      629 2023-06-05 16:13:40.939528 seaplane-0.3.9/src/seaplane/smartpipes/website/public/vercel.svg
--rw-r--r--   0        0        0     3691 2023-06-05 16:13:40.943187 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/Header.jsx
--rw-r--r--   0        0        0    10990 2023-06-05 16:13:40.944429 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
--rw-r--r--   0        0        0     4317 2023-06-07 13:59:40.996261 seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
--rw-r--r--   0        0        0      127 2023-06-05 16:13:40.945730 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/_app.js
--rw-r--r--   0        0        0      231 2023-06-05 16:13:40.946888 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/_document.js
--rw-r--r--   0        0        0     1962 2023-06-05 16:13:40.947276 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/index.js
--rw-r--r--   0        0        0     2643 2023-06-07 13:57:55.123829 seaplane-0.3.9/src/seaplane/smartpipes/website/src/pages/tutorial.js
--rw-r--r--   0        0        0      228 2023-06-05 16:13:40.947900 seaplane-0.3.9/src/seaplane/smartpipes/website/src/styles/globals.css
--rw-r--r--   0        0        0      528 2023-06-05 16:13:40.948083 seaplane-0.3.9/src/seaplane/smartpipes/website/tailwind.config.js
--rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.9/src/seaplane/util/__init__.py
--rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.9/src/seaplane/util/base64url.py
--rw-r--r--   0        0        0     5883 2023-06-08 16:34:11.748651 seaplane-0.3.9/setup.py
--rw-r--r--   0        0        0     3182 2023-06-08 16:34:11.748974 seaplane-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-07-21 14:25:12.219270 seaplane-0.3.90b0/README.md
+-rw-r--r--   0        0        0     2931 2023-08-04 12:14:03.264908 seaplane-0.3.90b0/pyproject.toml
+-rw-r--r--   0        0        0      778 2023-08-03 12:08:20.493524 seaplane-0.3.90b0/src/seaplane/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-21 14:25:14.742200 seaplane-0.3.90b0/src/seaplane/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-26 11:44:50.864621 seaplane-0.3.90b0/src/seaplane/api/__init__.py
+-rw-r--r--   0        0        0      527 2023-07-21 14:25:14.717240 seaplane-0.3.90b0/src/seaplane/api/api_http.py
+-rw-r--r--   0        0        0     2797 2023-07-21 14:25:14.717997 seaplane-0.3.90b0/src/seaplane/api/api_request.py
+-rw-r--r--   0        0        0     1499 2023-08-03 12:08:20.493756 seaplane-0.3.90b0/src/seaplane/api/api_substation.py
+-rw-r--r--   0        0        0     5806 2023-07-21 14:25:14.717640 seaplane-0.3.90b0/src/seaplane/api/metadata_api.py
+-rw-r--r--   0        0        0     1552 2023-07-21 14:25:14.722296 seaplane-0.3.90b0/src/seaplane/api/sql_api.py
+-rw-r--r--   0        0        0     3487 2023-07-21 14:25:14.717435 seaplane-0.3.90b0/src/seaplane/api/token_api.py
+-rw-r--r--   0        0        0      252 2023-08-03 12:08:20.494053 seaplane-0.3.90b0/src/seaplane/apps/__init__.py
+-rw-r--r--   0        0        0     1939 2023-07-21 14:25:14.740411 seaplane-0.3.90b0/src/seaplane/apps/app.py
+-rw-r--r--   0        0        0     2511 2023-07-21 14:25:14.727611 seaplane-0.3.90b0/src/seaplane/apps/build.py
+-rw-r--r--   0        0        0     3121 2023-07-21 14:25:14.740237 seaplane-0.3.90b0/src/seaplane/apps/cli.py
+-rw-r--r--   0        0        0     2952 2023-08-03 12:08:20.494339 seaplane-0.3.90b0/src/seaplane/apps/datasources/__init__.py
+-rw-r--r--   0        0        0     1883 2023-07-21 14:25:14.727419 seaplane-0.3.90b0/src/seaplane/apps/datasources/request_data_source.py
+-rw-r--r--   0        0        0     2368 2023-07-21 14:25:14.725497 seaplane-0.3.90b0/src/seaplane/apps/datasources/sql_executor.py
+-rw-r--r--   0        0        0     6179 2023-08-03 12:08:20.494639 seaplane-0.3.90b0/src/seaplane/apps/decorators.py
+-rw-r--r--   0        0        0    12169 2023-08-03 12:12:54.088157 seaplane-0.3.90b0/src/seaplane/apps/deploy.py
+-rw-r--r--   0        0        0       52 2023-07-21 14:25:14.740972 seaplane-0.3.90b0/src/seaplane/apps/entry_points/__init__.py
+-rw-r--r--   0        0        0     9553 2023-07-26 11:44:50.865394 seaplane-0.3.90b0/src/seaplane/apps/entry_points/entry_point.py
+-rw-r--r--   0        0        0     2194 2023-07-21 14:25:14.730843 seaplane-0.3.90b0/src/seaplane/apps/event_handler.py
+-rw-r--r--   0        0        0     1947 2023-07-21 14:25:14.741836 seaplane-0.3.90b0/src/seaplane/apps/executor.py
+-rw-r--r--   0        0        0     3583 2023-08-03 12:08:20.495109 seaplane-0.3.90b0/src/seaplane/apps/task.py
+-rw-r--r--   0        0        0      217 2023-08-03 12:08:20.495361 seaplane-0.3.90b0/src/seaplane/apps/tasks/__init__.py
+-rw-r--r--   0        0        0     3230 2023-07-21 14:25:14.730035 seaplane-0.3.90b0/src/seaplane/apps/tasks/openai.py
+-rw-r--r--   0        0        0     3150 2023-07-21 14:25:14.728391 seaplane-0.3.90b0/src/seaplane/apps/tasks/replicate.py
+-rw-r--r--   0        0        0     1094 2023-07-21 14:25:14.730325 seaplane-0.3.90b0/src/seaplane/apps/tasks/sql.py
+-rw-r--r--   0        0        0     1144 2023-08-04 12:13:29.912736 seaplane-0.3.90b0/src/seaplane/apps/tasks/substation.py
+-rw-r--r--   0        0        0     3102 2023-08-03 12:08:20.495725 seaplane-0.3.90b0/src/seaplane/apps/tasks/vectordb.py
+-rw-r--r--   0        0        0       33 2023-07-21 14:25:14.733884 seaplane-0.3.90b0/src/seaplane/apps/website/.gitignore
+-rw-r--r--   0        0        0     1750 2023-07-21 14:25:14.732095 seaplane-0.3.90b0/src/seaplane/apps/website/README.md
+-rw-r--r--   0        0        0       77 2023-07-21 14:25:14.731529 seaplane-0.3.90b0/src/seaplane/apps/website/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-07-21 14:25:14.731911 seaplane-0.3.90b0/src/seaplane/apps/website/next.config.js
+-rw-r--r--   0        0        0      644 2023-07-21 14:25:14.734019 seaplane-0.3.90b0/src/seaplane/apps/website/package.json
+-rw-r--r--   0        0        0       82 2023-07-21 14:25:14.734168 seaplane-0.3.90b0/src/seaplane/apps/website/postcss.config.js
+-rw-r--r--   0        0        0      717 2023-07-21 14:25:14.732539 seaplane-0.3.90b0/src/seaplane/apps/website/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2023-07-21 14:25:14.733701 seaplane-0.3.90b0/src/seaplane/apps/website/public/next.svg
+-rw-r--r--   0        0        0    39147 2023-07-21 14:25:14.732701 seaplane-0.3.90b0/src/seaplane/apps/website/public/openai.png
+-rw-r--r--   0        0        0    11580 2023-07-21 14:25:14.732841 seaplane-0.3.90b0/src/seaplane/apps/website/public/seaplane_logo.svg
+-rw-r--r--   0        0        0     2296 2023-07-21 14:25:14.732974 seaplane-0.3.90b0/src/seaplane/apps/website/public/seaplane_logo_mark.svg
+-rw-r--r--   0        0        0   195272 2023-07-21 14:25:14.733365 seaplane-0.3.90b0/src/seaplane/apps/website/public/stabilityai.png
+-rw-r--r--   0        0        0      629 2023-07-21 14:25:14.733551 seaplane-0.3.90b0/src/seaplane/apps/website/public/vercel.svg
+-rw-r--r--   0        0        0     3691 2023-07-21 14:25:14.736701 seaplane-0.3.90b0/src/seaplane/apps/website/src/components/Header.jsx
+-rw-r--r--   0        0        0    10691 2023-07-21 14:25:14.736851 seaplane-0.3.90b0/src/seaplane/apps/website/src/components/SmartPipe.jsx
+-rw-r--r--   0        0        0     4191 2023-07-21 14:25:14.736999 seaplane-0.3.90b0/src/seaplane/apps/website/src/components/SmartPipesList.jsx
+-rw-r--r--   0        0        0      127 2023-07-21 14:25:14.737294 seaplane-0.3.90b0/src/seaplane/apps/website/src/pages/_app.js
+-rw-r--r--   0        0        0      231 2023-07-21 14:25:14.737714 seaplane-0.3.90b0/src/seaplane/apps/website/src/pages/_document.js
+-rw-r--r--   0        0        0     1841 2023-07-21 14:25:14.737434 seaplane-0.3.90b0/src/seaplane/apps/website/src/pages/index.js
+-rw-r--r--   0        0        0     2377 2023-07-21 14:25:14.737575 seaplane-0.3.90b0/src/seaplane/apps/website/src/pages/tutorial.js
+-rw-r--r--   0        0        0      228 2023-07-21 14:25:14.736265 seaplane-0.3.90b0/src/seaplane/apps/website/src/styles/globals.css
+-rw-r--r--   0        0        0      528 2023-07-21 14:25:14.731769 seaplane-0.3.90b0/src/seaplane/apps/website/tailwind.config.js
+-rw-r--r--   0        0        0       58 2023-07-21 14:25:14.723206 seaplane-0.3.90b0/src/seaplane/carrier/__init__.py
+-rw-r--r--   0        0        0     4463 2023-07-21 14:25:14.723452 seaplane-0.3.90b0/src/seaplane/carrier/processor.py
+-rw-r--r--   0        0        0     9173 2023-08-03 12:08:20.495934 seaplane-0.3.90b0/src/seaplane/configuration.py
+-rw-r--r--   0        0        0     2480 2023-08-03 12:08:20.496096 seaplane-0.3.90b0/src/seaplane/integrations/langchain.py
+-rw-r--r--   0        0        0     1815 2023-07-21 14:25:14.742466 seaplane-0.3.90b0/src/seaplane/logging/__init__.py
+-rw-r--r--   0        0        0      267 2023-08-03 12:08:20.496277 seaplane-0.3.90b0/src/seaplane/model/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-21 14:25:14.715240 seaplane-0.3.90b0/src/seaplane/model/errors.py
+-rw-r--r--   0        0        0     3560 2023-07-21 14:25:14.715566 seaplane-0.3.90b0/src/seaplane/model/metadata/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-21 14:25:14.711223 seaplane-0.3.90b0/src/seaplane/model/region.py
+-rw-r--r--   0        0        0       86 2023-07-26 11:44:50.865910 seaplane-0.3.90b0/src/seaplane/model/secrets/__init__.py
+-rw-r--r--   0        0        0      530 2023-07-21 14:25:14.716316 seaplane-0.3.90b0/src/seaplane/model/sql/__init__.py
+-rw-r--r--   0        0        0      393 2023-08-03 12:08:20.496425 seaplane-0.3.90b0/src/seaplane/model/vector/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-21 14:25:14.704688 seaplane-0.3.90b0/src/seaplane/util/__init__.py
+-rw-r--r--   0        0        0      318 2023-07-21 14:25:14.704383 seaplane-0.3.90b0/src/seaplane/util/base64url.py
+-rw-r--r--   0        0        0       67 2023-08-03 12:08:20.496559 seaplane-0.3.90b0/src/seaplane/vector/__init__.py
+-rw-r--r--   0        0        0     4414 2023-08-03 12:08:20.496697 seaplane-0.3.90b0/src/seaplane/vector/vector_store.py
+-rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 seaplane-0.3.90b0/PKG-INFO
```

### Comparing `seaplane-0.3.9/README.md` & `seaplane-0.3.90b0/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/pyproject.toml` & `seaplane-0.3.90b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.3.9"
+version = "0.3.90-beta.0"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 
 
 [tool.poetry.dependencies]
-python = ">=3.10.*,<4.0"
-attrs = "21.4.0"
-certifi = "2022.6.15"
-charset-normalizer = "2.1.0"
-idna = "3.3"
-iniconfig = "1.1.1"
-packaging = "21.3"
-pluggy = "1.0.0"
-py = "1.11.0"
-pyparsing = "3.0.9"
-requests = "2.28.1"
-tomli = "2.0.1"
-urllib3 = "1.26.9"
+python = ">=3.10,<3.12"
+attrs = "^22.2.0"
+certifi = "^2022.6.15"
+charset-normalizer = "^2.1.0"
+idna = "^3.3"
+iniconfig = "^1.1.1"
+packaging = "^21.3"
+pluggy = "^1.0.0"
+py = "^1.11.0"
+pyparsing = "^3.0.9"
+requests = "^2.31.0"
+tomli = "^2.0.1"
 types-requests = "^2.28.0"
 returns = "^0.19.0"
 requests-mock = "^1.9.3"
 simplejson = "^3.17.6"
 types-simplejson = "^3.17.7"
 Flask-Cors = "^3.0.10"
 Flask-SocketIO = "^5.3.4"
 openai = "^0.27.7"
 tqdm = "^4.65.0"
-pinecone-client = "^2.2.1"
 tiktoken = "^0.4.0"
 pypdf = "^3.9.0"
-langchain = "^0.0.183"
-boto3 = "^1.26.142"
+langchain = "^0.0.195"
+nats-py="^2.3.1"
+psycopg2-binary = "^2.9.6"
+nkeys = "^0.1.0"
+toml = "^0.10.2"
+cookiecutter = "^2.1.1"
+types-toml = "^0.10.8.6"
+urllib3 = "^1.26.16"
+python-dotenv = "^1.0.0"
+qdrant-client = "^1.3.2"
+langchainplus-sdk = "^0.0.20"
+
+[tool.poetry.scripts]
+seaplane = "seaplane.apps.cli:main"
 
 [tool.poetry.dev-dependencies]
 nox-poetry = "*"
 
 # Testing.
 pytest = "*"
 pytest-cov = "*"
@@ -51,24 +61,23 @@
 # Linting.
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-broken-line = "*"
 flake8-comprehensions = "*"
 pep8-naming = "*"
 # TODO: Remove this when flake8 adds native support for pyproject.toml.
-pyproject-flake8 = "*"
+pyproject-flake8 = "^6.0.0.post1"
 
 # Formatting.
 black = "*"
 isort = "*"
 Sphinx = "^5.2.3"
 sphinx-autodoc-typehints = "^1.19.4"
 myst-parser = "^0.18.1"
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
```

### Comparing `seaplane-0.3.9/src/seaplane/api/api_http.py` & `seaplane-0.3.90b0/src/seaplane/api/api_http.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/api/api_request.py` & `seaplane-0.3.90b0/src/seaplane/api/api_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,21 @@
     """
 
     def handle_request(request: Callable[[str], Response], token: str) -> Result[Any, HTTPError]:
         try:
             response = request(token)
 
             if response.ok:
-                return Success(response.json())
+                data = None
+                if response.headers.get("content-type") == "application/json":
+                    data = response.json()
+                else:
+                    data = response.text
+
+                return Success(data)
             else:
                 body_error = response.text
                 log.error(f"Request Error: {body_error}")
                 return Failure(HTTPError(response.status_code, body_error))
         except requests.exceptions.RequestException as err:
             log.error(f"Request exception: {str(err)}")
             return Failure(HTTPError(SDK_HTTP_ERROR_CODE, str(err)))
@@ -61,14 +67,14 @@
 
     def req(request: Callable[[str], Response]) -> Result[Any, HTTPError]:
         access_token: Result[str, HTTPError]
 
         if token_api.access_token is not None:
             access_token = Success(token_api.access_token)
         else:
-            access_token = token_api._request_access_token()
+            access_token = token_api._request_access_token().map(lambda result: result["token"])
 
         return access_token.bind(lambda token: handle_request(request, token)).lash(
             lambda error: renew_if_fails(token_api, request, error)
         )
 
     return req
```

### Comparing `seaplane-0.3.9/src/seaplane/api/lock_api.py` & `seaplane-0.3.90b0/src/seaplane/api/metadata_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,226 +1,175 @@
 from typing import Any, Dict, List, Optional
 
 import requests
 
 from ..configuration import Configuration, config
-from ..model.locks import HeldLock, Lock, LockPage, Name, to_held_lock, to_lock, to_lock_page
+from ..model.metadata import Key, KeyValue, KeyValuePage, to_key_value, to_key_value_page
 from ..util import unwrap
 from ..util.base64url import base64url_encode_from_bytes
 from .api_http import headers
 from .api_request import provision_req
 
 
-class LockAPI:
+class MetadataAPI:
     """
-    Class for handle Lock API calls.
+    Class for handle Metadata API calls.
     """
 
     def __init__(self, configuration: Configuration = config) -> None:
-        self.url = f"{configuration.coordination_endpoint}/locks"
+        self.url = f"{configuration.coordination_endpoint}/config"
         self.req = provision_req(configuration._token_api)
 
-    def get(self, name: Name) -> Lock:
-        """Gets information about a single lock.
+    def set(self, key_value: KeyValue) -> bool:
+        """Adds a value to the store at the given key.
 
         Parameters
         ----------
-        name : Name
-            Name of the lock.
+        key_value : KeyValue
+            key-value pair to be set, for example, key=foo/bar, value=hello
 
         Returns
         -------
-        Lock
-            Returns Lock if successful or it will raise an HTTPError otherwise.
+        boolean
+            Returns true if successful or it will raise an HTTPError otherwise.
         """
-        _url = f"{self.url}/base64:{base64url_encode_from_bytes(name.name)}"
+        url = f"{self.url}/base64:{base64url_encode_from_bytes(key_value.key)}"
 
-        return unwrap(
-            self.req(lambda access_token: requests.get(_url, headers=headers(access_token))).map(
-                lambda lock_response: to_lock(lock_response)
-            )
-        )
-
-    def acquire(self, name: Name, client_id: str, ttl: int) -> HeldLock:
-        """Attempts to acquire the lock with the given lock name with the given TTL.
-        Client-ID should identify the client making the request for debugging purposes.
-
-        Parameters
-        ----------
-        name : Name
-            Name of the lock.
-        client_id : Name
-            client_id is an identifier showing who is currently holding the lock.
-        ttl: int
-            This is the requested time to live, in seconds.
-
-        Returns
-        -------
-        HeldLock
-            Returns HeldLock if successful or it will raise an HTTPError otherwise.
-        """
-        _url = f"{self.url}/base64:{base64url_encode_from_bytes(name.name)}"
-
-        params: Dict[str, Any] = {}
-        params["client-id"] = client_id
-        params["ttl"] = ttl
-
-        return unwrap(
+        set_result = unwrap(
             self.req(
-                lambda access_token: requests.post(
-                    _url, params=params, headers=headers(access_token)
+                lambda access_token: requests.put(
+                    url,
+                    data=base64url_encode_from_bytes(key_value.value),
+                    headers=headers(access_token),
                 )
-            ).map(lambda held_lock_response: to_held_lock(held_lock_response))
+            )
         )
 
-    def release(self, name: Name, id: str) -> bool:
-        """Attempts to release the given lock.
+        return bool(set_result == "Ok")  # mypy bug, mypy can't know the
+
+    def get(self, key: Key) -> KeyValue:
+        """Returns the key value pair associated with the set key.
 
         Parameters
         ----------
-        name : Name
-            Name of the lock.
-        id: str
-            ID which allows for the renewal/release of a lock, represents "holding"
-            the lock, this is usually only seen by the original acquirer of the lock
-            but may be leaked by listing the locks.
+        key : Key
+            The key from a key-value previously set, for example, key=foo/bar
 
         Returns
         -------
-        bool
-            Returns bool if successful or it will raise an HTTPError otherwise.
+        KeyValue
+            Returns KeyValue if successful or it will raise an HTTPError otherwise.
         """
-        _url = f"{self.url}/base64:{base64url_encode_from_bytes(name.name)}"
-
-        params: Dict[str, Any] = {}
-        params["id"] = id
+        url = f"{self.url}/base64:{base64url_encode_from_bytes(key.key)}"
 
-        release_result = unwrap(
-            self.req(
-                lambda access_token: requests.delete(
-                    _url, params=params, headers=headers(access_token)
-                )
+        return unwrap(
+            self.req(lambda access_token: requests.get(url, headers=headers(access_token))).map(
+                lambda key_value: to_key_value(key_value)
             )
         )
 
-        return bool(release_result == "OK")  # mypy bug, mypy can't know the
-
-    def renew(self, name: Name, id: str, ttl: int) -> bool:
-        """Attempts to renew the given lock.
+    def delete(self, key: Key) -> bool:
+        """Deletes the key value pair at from a given key.
 
         Parameters
         ----------
-        name : Name
-            Name of the lock.
-        id: str
-            ID which allows for the renewal/release of a lock, represents "holding"
-            the lock, this is usually only seen by the original acquirer of the lock
-            but may be leaked by listing the locks.
-        ttl: int
-            This is the requested time to live, in seconds.
+        directory : Key
+            The key from a key-value previously set, for example, key=foo/bar
 
         Returns
         -------
-        bool
-            Returns bool if successful or it will raise an HTTPError otherwise.
+        boolean
+            Returns true if successful or it will raise an HTTPError otherwise.
         """
-        _url = f"{self.url}/base64:{base64url_encode_from_bytes(name.name)}"
-
-        params: Dict[str, Any] = {}
-        params["id"] = id
-        params["ttl"] = ttl
+        url = f"{self.url}/base64:{base64url_encode_from_bytes(key.key)}"
 
-        renew_result = unwrap(
-            self.req(
-                lambda access_token: requests.patch(
-                    _url, params=params, headers=headers(access_token)
-                )
-            )
+        delete_result = unwrap(
+            self.req(lambda access_token: requests.delete(url, headers=headers(access_token)))
         )
 
-        return bool(renew_result == "OK")
+        return bool(delete_result == "Ok")  # mypy bug, mypy can't know the
 
     def get_page(
         self,
-        directory: Optional[Name] = None,
-        from_lock: Optional[Name] = None,
-    ) -> LockPage:
-        """Returns a single page of lock information for the given directory,
-        beginning with the `from_lock` key.
+        directory: Optional[Key] = None,
+        next_key: Optional[Key] = None,
+    ) -> KeyValuePage:
+        """Returns a single page of key value pairs for the given directory,
+        beginning with the `next_key` key.
 
         If no directory is given, the root directory is used.
-        If no `from_lock` is given, the range begins from the start.
+        If no `next_key` is given, the range begins from the start.
 
         Parameters
         ----------
-        directory : Optional[Name]
+        directory : Optional[Key]
             The metadata key-value store supports the use of directories.
             Directories are important tools to set up region and provider restrictions
             for groups of key-value pairs.
-        from_lock : Optional[Name]
+        next_key : Optional[Key]
             If more pages are desired, perform another range request using
-            the `from_lock` value from the first request as the `from_lock` value of
+            the `next_key` value from the first request as the `next_key` value of
             the following request.
 
         Returns
         -------
-        LockPage
-            Returns LockPage if successful or it will raise an HTTPError otherwise.
+        KeyValuePage
+            Returns KeyValuePage if successful or it will raise an HTTPError otherwise.
         """
 
         _url = self.url
 
         if directory is not None:
-            _url = f"{self.url}/base64:{base64url_encode_from_bytes(directory.name)}/"
+            _url = f"{self.url}/base64:{base64url_encode_from_bytes(directory.key)}/"
 
         params: Dict[str, Any] = {}
-        if from_lock is not None:
-            params["from"] = f"base64:{base64url_encode_from_bytes(from_lock.name)}"
+        if next_key is not None:
+            params["from"] = f"base64:{base64url_encode_from_bytes(next_key.key)}"
 
         return unwrap(
             self.req(
                 lambda access_token: requests.get(
                     _url, params=params, headers=headers(access_token)
                 )
-            ).map(lambda lock_range: to_lock_page(lock_range))
+            ).map(lambda key_value_range: to_key_value_page(key_value_range))
         )
 
     def get_all_pages(
         self,
-        directory: Optional[Name] = None,
-        from_lock: Optional[Name] = None,
-    ) -> List[Lock]:
-        """Returns all held lock information for the given directory,
-        from the `from_lock` key onwards. May perform multiple requests.
+        directory: Optional[Key] = None,
+        next_key: Optional[Key] = None,
+    ) -> List[KeyValue]:
+        """Returns all key value pair for the given directory, from the `next_key` key onwards.
+        May perform multiple requests.
 
         If no directory is given, the root directory is used.
-        If no `from_lock` is given, the range begins from the start.
+        If no `next_key` is given, the range begins from the start.
 
         Parameters
         ----------
-        directory : Optional[Name]
+        directory : Optional[Key]
             The metadata key-value store supports the use of directories.
             Directories are important tools to set up region and provider restrictions
             for groups of key-value pairs.
-        from_lock : Optional[Name]
-            It begins from from_lock in advance until the last page,
+        next_key : Optional[Key]
+            It begins from next_key in advance until the last page,
             if you don't want to begin from the start.
 
         Returns
         -------
-        List[Lock]
-            Returns a List of Locks if successful or it will raise an HTTPError otherwise.
+        List[KeyValue]
+            Returns a key value pair list if successful or it will raise an HTTPError otherwise.
         """
 
-        pages: List[Lock] = []
-        _from_lock = from_lock
+        pages: List[KeyValue] = []
+        _next_lock = next_key
 
         while True:
-            page_result = self.get_page(directory, _from_lock)
+            page_result = self.get_page(directory, _next_lock)
 
-            page: LockPage = page_result
-            pages.extend(page.locks)
+            page: KeyValuePage = page_result
+            pages.extend(page.key_value_pairs)
 
-            if page.next_lock is not None:
-                _from_lock = page.next_lock
+            if page.next_key is not None:
+                _next_lock = page.next_key
             else:
                 return pages
```

### Comparing `seaplane-0.3.9/src/seaplane/api/sql_api.py` & `seaplane-0.3.90b0/src/seaplane/api/sql_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/api/token_api.py` & `seaplane-0.3.90b0/src/seaplane/api/token_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Dict, Optional
 
 import requests
 from returns.result import Failure, Result, Success
 
 from ..logging import log
 from ..model.errors import HTTPError
 from ..util import unwrap
@@ -21,14 +21,15 @@
     """
 
     def __init__(self, configuration) -> None:  # type: ignore
         self.url = f"{configuration.identify_endpoint}/token"
         self.api_key = configuration.seaplane_api_key
         self.access_token = configuration._current_access_token
         self.auto_renew = configuration._token_auto_renew
+        self.tenant: Optional[str] = None
 
     def set_url(self, url: str) -> None:
         self.url = url
 
     def set_token(self, access_token: Optional[str]) -> None:
         """Set a valid Seaplane Token.
 
@@ -68,33 +69,44 @@
         """Request a new token.
 
         Returns
         -------
         str
             Returns the token.
         """
-        return unwrap(self._request_access_token())
+        return unwrap(self._request_access_token())["token"]
 
-    def _request_access_token(self) -> Result[str, HTTPError]:
+    def get_tenant(self) -> str:
+        """Request the current tenant
+
+        Returns
+        -------
+        str
+            Returns the tenant.
+        """
+        return self.tenant if self.tenant else unwrap(self._request_access_token())["tenant"]
+
+    def _request_access_token(self) -> Result[Dict[str, str], HTTPError]:
         try:
             log.info("Requesting access token...")
+            if not self.api_key:
+                log.error("API KEY not set, use sea.config.set_api_key")
+
             response = requests.post(self.url, json={}, headers=headers(self.api_key))
 
             if response.ok:
-                token = response.json()["token"]
-                self.access_token = token
+                token = response.json()
+                self.access_token = token["token"]
+                self.tenant = token["tenant"]
                 return Success(token)
             else:
                 self._current_access_token = None
-                error_body = response.json()
+                error_body = response.text
                 log.error(
                     f"Bad Access token request code {response.status_code}, error {error_body}"
                 )
                 return Failure(HTTPError(response.status_code, error_body))
 
         except requests.exceptions.RequestException as err:
             self._current_access_token = None
-            if not self.api_key:
-                log.error("API KEY not set, use sea.config.set_api_key")
-            else:
-                log.error(f"Request access token exception: {str(err)}")
+            log.error(f"Request access token exception: {str(err)}")
             return Failure(HTTPError(SDK_HTTP_ERROR_CODE, str(err)))
```

### Comparing `seaplane-0.3.9/src/seaplane/configuration.py` & `seaplane-0.3.90b0/src/seaplane/configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 import os
 from typing import Dict, Optional
 
+from dotenv import load_dotenv
+
 from .api.token_api import TokenAPI
 from .logging import log
 from .model.errors import SeaplaneError
 
+env_file = load_dotenv("./.env")
+if env_file:
+    log.debug("👀 Found .env config file")
+
 _SEAPLANE_COMPUTE_API_ENDPOINT = "https://compute.cplane.cloud/v2beta"
 _SEAPLANE_COORDINATION_API_ENDPOINT = "https://metadata.cplane.cloud/v1"
 _SEAPLANE_IDENTIFY_API_ENDPOINT = "https://flightdeck.cplane.cloud/v1"
 _SEAPLANE_GLOBAL_SQL_API_ENDPOINT = "https://sql.cplane.cloud/v1"
-_SEAPLANE_CARRIER_API_ENDPOINT = "https://carrier.staging.cplane.dev/v1"
+_SEAPLANE_CARRIER_API_ENDPOINT = "https://carrier.cplane.cloud/v1"
 _SEAPLANE_SUBSTATION_API_ENDPOINT = "https://substation.dev.cplane.cloud/v1"
+_SEAPLANE_SUBSTATION_EMBED_API_ENDPOINT = "https://embed.substation.cplane.cloud/v1/embed"
+_SEAPLANE_VECTOR_DB_API_ENDPOINT = "https://vector.cplane.cloud"
+
+_SEAPLANE_ENV_VAR_PRODUCTION = "SEAPLANE_APPS_PRODUCTION"
 
-_SEAPLANE_ENV_VAR_PRODUCTION = "SMARTPIPES_PRODUCTION"
+api_key_names = ["SEAPLANE_API_KEY", "OPENAI_API_KEY", "REPLICATE_API_KEY"]
 
 
-def get_env(key: str) -> str:
+def get_env(key: str) -> Optional[str]:
     env = os.getenv(key)
 
     if not env:
-        return ""
+        return None
     else:
         return env
 
 
+def get_api_keys() -> Dict[str, str]:
+    api_keys = {}
+
+    for api_key_env_name in api_key_names:
+        api_key = get_env(api_key_env_name)
+        if api_key:
+            api_keys[api_key_env_name] = api_key
+
+    return api_keys
+
+
 class Configuration:
     """
     Seaplane SDK Configuration.
 
     Everytime the configuration is changed,
     It'll clear local configurations to the default Auth module.
     """
@@ -36,23 +57,20 @@
         self.seaplane_api_key: Optional[str] = None
         self.identify_endpoint = _SEAPLANE_IDENTIFY_API_ENDPOINT
         self.compute_endpoint = _SEAPLANE_COMPUTE_API_ENDPOINT
         self.coordination_endpoint = _SEAPLANE_COORDINATION_API_ENDPOINT
         self.global_sql_endpoint = _SEAPLANE_GLOBAL_SQL_API_ENDPOINT
         self.substation_endpoint = _SEAPLANE_SUBSTATION_API_ENDPOINT
         self.carrier_endpoint = _SEAPLANE_CARRIER_API_ENDPOINT
+        self.vector_db_endpoint = _SEAPLANE_VECTOR_DB_API_ENDPOINT
+        self.substation_embed_endpoint = _SEAPLANE_SUBSTATION_EMBED_API_ENDPOINT
         self._current_access_token: Optional[str] = None
         self._token_auto_renew = True
-        self._api_keys: Dict[str, str] = {
-            "SEAPLANE_API_KEY": get_env("SEAPLANE_API_KEY"),
-            "OPENAI_API_KEY": get_env("OPENAI_API_KEY"),
-            "REPLICATE_API_KEY": get_env("REPLICATE_API_KEY"),
-            "PINECONE_API_KEY": get_env("PINECONE_API_KEY"),
-            "PINECONE_API_ENV": get_env("PINECONE_API_ENV"),
-        }
+        self.seaplane_api_key = get_env("SEAPLANE_API_KEY")
+        self._api_keys: Dict[str, str] = get_api_keys()
         self._production = False
         self._update_token_api()
 
     def set_api_key(self, api_key: str) -> None:
         """Set the Seaplane API Key.
 
         The API Key is needed for the Seaplane Python SDK usage.
@@ -62,25 +80,25 @@
         api_key : str
             Seaplane API Key.
         """
         self.seaplane_api_key = api_key
         self._update_token_api()
 
     def set_api_keys(self, api_keys: Dict[str, str]) -> None:
-        """Set the Seaplane API Keys for SmartPipes.
+        """Set the Seaplane API Keys for Apps.
 
-        The API Keys is needed for some of the Coprocessors.
+        The API Keys is needed for some of the Tasks.
 
-        Supported Coprocessors API Keys:
+        Supported Tasks API Keys:
 
         Seaplane: SEAPLANE_API_KEY
         Open AI: OPENAI_API_KEY
         Replicate: REPLICATE_API_KEY
 
-        For example, for use an OpenAI Coprocessor,
+        For example, for use an OpenAI Task,
         you need to provide the Key - Value, of the API Key.
 
             $ from seaplane import sea
 
             $ api_keys = {"OPENAI_API_KEY": "sp-api-key-test" }
             $ sea.config.set_api_keys(api_keys)
 
@@ -194,14 +212,30 @@
         if endpoint[-1] == "/":
             self.carrier_endpoint = endpoint.rstrip(endpoint[-1])
         else:
             self.carrier_endpoint = endpoint
 
         self._update_token_api()
 
+    def set_vector_endpoint(self, endpoint: str) -> None:
+        if endpoint[-1] == "/":
+            self.vector_db_endpoint = endpoint.rstrip(endpoint[-1])
+        else:
+            self.vector_db_endpoint = endpoint
+
+        self._update_token_api()
+
+    def set_substation_embed_endpoint(self, endpoint: str) -> None:
+        if endpoint[-1] == "/":
+            self.substation_embed_endpoint = endpoint.rstrip(endpoint[-1])
+        else:
+            self.substation_embed_endpoint = endpoint
+
+        self._update_token_api()
+
     def _update_token_api(self) -> None:
         self._token_api = TokenAPI(self)
 
     def log_level(self, level: int) -> None:
         """Change logging level.
 
         Seaplane uses Python logging module for internal logs.
@@ -237,15 +271,15 @@
         if enable:
             log.enable()
         else:
             log.disable()
 
     def is_production(self) -> bool:
         if not self._production:
-            return os.getenv(_SEAPLANE_ENV_VAR_PRODUCTION) is not None
+            return os.getenv(_SEAPLANE_ENV_VAR_PRODUCTION, "").lower() == "true"
 
         return self._production
 
     def set_production(self, is_production: bool) -> None:
         self._production = is_production
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `seaplane-0.3.9/src/seaplane/logging/__init__.py` & `seaplane-0.3.90b0/src/seaplane/logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     INFO = logging.INFO
     DEBUG = logging.DEBUG
     NOTSET = logging.NOTSET
 
     def __init__(self) -> None:
         logging.basicConfig(format=self.FORMAT)
         self.logger = logging.getLogger("Seaplane")
-        self.logger.setLevel(logging.WARNING)
+        self.logger.setLevel(logging.INFO)
 
     def debug(self, message: str) -> None:
         self.logger.debug(message)
 
     def info(self, message: str) -> None:
         self.logger.info(message)
```

### Comparing `seaplane-0.3.9/src/seaplane/model/metadata/__init__.py` & `seaplane-0.3.90b0/src/seaplane/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/model/sql/__init__.py` & `seaplane-0.3.90b0/src/seaplane/model/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/coprocessor.py` & `seaplane-0.3.90b0/src/seaplane/apps/task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,110 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from ..logging import log
-from .coprocessors import Bloom, OpenAI, Replicate, Store
+from ..model.errors import SeaplaneError
+from .tasks import OpenAI, Replicate, Sql, Store, SubstationTask
 
 
-class CoprocessorEvent:
+class TaskEvent:
     def __init__(self, id: str, input: Any) -> None:
         self.id = id
         self.status = "in_progress"
         self.input = input
         self.output: Optional[Any] = None
         self.error: Optional[Any] = None
 
-    def set_ouput(self, output: Any) -> None:
+    def set_output(self, output: Any) -> None:
         self.output = output
         self.status = "completed"
 
     def set_error(self, error: Any) -> None:
         self.error = error
         self.status = "error"
 
 
 SEAPLANE_API_KEY_NAME = "SEAPLANE_API_KEY"
 OPENAI_API_KEY_NAME = "OPENAI_API_KEY"
 REPLICATE_API_KEY_NAME = "REPLICATE_API_KEY"
 
 
-class Coprocessor:
+class Task:
     def __init__(
-        self, func: Callable[[Any], Any], type: str, id: Optional[str], model: Optional[str]
+        self,
+        func: Callable[[Any], Any],
+        type: str,
+        id: Optional[str] = None,
+        model: Optional[str] = None,
+        sql_access: Optional[Dict[str, str]] = None,
+        index_name: Optional[str] = None,
     ) -> None:
         self.func = func
         self.args: Optional[Tuple[Any, ...]] = None
         self.kwargs: Optional[Dict[str, Any]] = None
         self.type = type
         self.model = model
         self.sources: List[str] = []
+        self.sql_access = sql_access
+        self.sql: Optional[Sql] = None
         self.name = func.__name__
+        self.index_name = index_name
 
         if id is not None:
             self.id = id
         else:
             self.id = func.__name__
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.args = args
         self.kwargs = kwargs
 
-        log.info(f"Coprocessor type '{self.type}' Model ID {self.model}")
+        log.info(f"Task type '{self.type}' Model ID {self.model}")
+
+        if self.type == "sql":
+            if self.sql_access is None:
+                raise SeaplaneError("Task of type SQL without sql attribute.")
+
+            if not self.sql:
+                self.sql = Sql(self.func, self.id, self.sql_access)
+
+            return self.sql.process(*self.args, **self.kwargs)
 
         if self.type == "vectordb":
-            log.info("Accessing Vector DB coprocessor...")
-            self.args = self.args + (Store(),)
+            log.info("Accessing Vector DB task...")
+
+            if not self.index_name:
+                raise SeaplaneError("Missing index_name attribute on vectordb Task.")
+
+            self.args = self.args + (Store(self.index_name),)
             return self.func(*self.args, **self.kwargs)
 
-        if self.model == "bloom":
-            bloom = Bloom(self.func, self.id, self.model)
-            return bloom.process(*self.args, **self.kwargs)
-        elif self.model == "gpt-3.5":
-            openai = OpenAI(self.func, self.id, self.model)
+        model = None
+
+        if self.model:
+            model = self.model.lower()
+        else:
+            model = self.model
+
+        if model == "mpt-30b":
+            substation = SubstationTask(self.func, self.id, model)
+            return substation.process(*self.args, **self.kwargs)
+        elif model == "gpt-3.5":
+            openai = OpenAI(self.func, self.id, model)
             return openai.process(*self.args, **self.kwargs)
-        elif self.model == "gpt-3":
-            openai = OpenAI(self.func, self.id, self.model)
+        elif model == "gpt-3":
+            openai = OpenAI(self.func, self.id, model)
             return openai.process(*self.args, **self.kwargs)
-        elif self.model == "stable-diffusion":
-            replicate = Replicate(self.func, self.type, self.id, self.model)
+        elif model == "stable-diffusion":
+            replicate = Replicate(self.func, self.type, self.id, model)
             return replicate.process(*self.args, **self.kwargs)
-        elif self.model:
-            replicate = Replicate(self.func, self.type, self.id, self.model)
+        elif model:
+            replicate = Replicate(self.func, self.type, self.id, model)
             return replicate.process(*self.args, **self.kwargs)
         else:
-            log.info("Unknown coprocessor...")
+            log.info("Compute task type...")
             return self.func(*self.args, **self.kwargs)
 
     def called_from(self, sources: List[str]) -> None:
         self.sources = sources
 
     def print(self) -> None:
         log.info(f"id: {self.id}, type: {self.type}, model: {self.model}")
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/bloom.py` & `seaplane-0.3.90b0/src/seaplane/apps/tasks/openai.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,111 @@
 from typing import Any, Callable, Dict, Optional, Tuple
 
 import requests
 
 from ...api.api_http import headers
-from ...api.api_request import provision_req
+from ...api.api_request import handle_request
 from ...configuration import config
 from ...logging import log
 from ...model.errors import SeaplaneError
 from ...util import unwrap
 
-SEAPLANE_API_KEY_NAME = "SEAPLANE_API_KEY"
+OPENAI_API_KEY_NAME = "OPENAI_API_KEY"
+OPENAI_URL = "https://api.openai.com"
 
 
-def _check_seaplane_api_key() -> None:
-    if config.seaplane_api_key is None:
+def _check_openai_api_keys() -> None:
+    if config._api_keys is None:
         raise SeaplaneError(
-            f"Seaplane API Key `{SEAPLANE_API_KEY_NAME}` is not set,\
-                  use `sea.config.set_api_key`."
+            f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, \
+                  use `sea.config.set_api_keys`."
+        )
+    elif not config._api_keys.get(OPENAI_API_KEY_NAME, None):
+        raise SeaplaneError(
+            f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set,\
+                  use `sea.config.set_api_keys`."
+        )
+
+
+def _gpt_3() -> Callable[[Dict[str, Any]], Any]:
+    def model(payload: Dict[str, Any]) -> Any:
+        """
+        The OpenAI GPT-3 payload.
+
+        payload = {"model": "text-davinci-003", "prompt": prompt, "temperature": 0}
+        """
+        _check_openai_api_keys()
+
+        url = f"{OPENAI_URL}/v1/completions"
+
+        return unwrap(
+            handle_request(
+                lambda: requests.post(
+                    url,
+                    json=payload,
+                    headers=headers(config._api_keys[OPENAI_API_KEY_NAME]),
+                )
+            )
         )
 
+    return model
 
-def bloom() -> Callable[[Dict[str, Any]], Any]:
-    def model(input: Dict[str, Any]) -> Any:
-        _check_seaplane_api_key()
 
-        url = f"{config.substation_endpoint}/completions"
-        req = provision_req(config._token_api)
+def _gpt_3_5() -> Callable[[Dict[str, Any]], Any]:
+    def model(payload: Dict[str, Any]) -> Any:
+        """
+        The OpenAI GPT-3.5 payload.
+
+         payload = {
+           "model": "gpt-3.5-turbo",
+           "messages": [{"role": "user", "content": "Any prompt here.."}],
+           "temperature": 0.7,
+         }
+        """
+        _check_openai_api_keys()
 
-        payload = {"prompt": input}
+        url = f"{OPENAI_URL}/v1/chat/completions"
 
         return unwrap(
-            req(
-                lambda access_token: requests.post(
+            handle_request(
+                lambda: requests.post(
                     url,
                     json=payload,
-                    headers=headers(access_token),
+                    headers=headers(config._api_keys[OPENAI_API_KEY_NAME]),
                 )
             )
         )
 
     return model
 
 
-class Bloom:
+class OpenAI:
     def __init__(self, func: Callable[[Any], Any], id: str, model: Optional[str]) -> None:
         self.func = func
         self.args: Optional[Tuple[Any, ...]] = None
         self.kwargs: Optional[Dict[str, Any]] = None
         self.type = "inference"
         self.model = model
         self.id = id
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.args = args
         self.kwargs = kwargs
 
-        if self.model == "bloom":
-            log.info("Processing Bloom Model...")
-            self.args = self.args + (bloom(),)
+        if self.model == "gpt-3.5":
+            log.info("Processing GPT-3.5 Model...")
+            self.args = self.args + (_gpt_3_5(),)
+
+            return self.func(*self.args, **self.kwargs)
+        elif self.model == "gpt-3":
+            log.info("Processing GPT-3 Model...")
+            self.args = self.args + (_gpt_3(),)
 
             return self.func(*self.args, **self.kwargs)
+        else:
+            raise SeaplaneError(
+                "OPENAI Task Not recognised , the model \
+                    doesn't match with any current OPEN AI task."
+            )
 
     def print(self) -> None:
         log.info(f"id: {self.id}, type: {self.type}, model: {self.model}")
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/coprocessors/replicate.py` & `seaplane-0.3.90b0/src/seaplane/apps/tasks/replicate.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,21 @@
         self.id = id
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.args = args
         self.kwargs = kwargs
 
         if self.model == "stable-diffusion":
-            log.info("Accessing Replicate stable-diffusion coprocessor...")
+            log.info("Accessing Replicate stable-diffusion task...")
             self.args = self.args + (
                 inference("27b93a2413e7f36cd83da926f3656280b2931564ff050bf9575f1fdf9bcd7478"),
             )
 
             return self.func(*self.args, **self.kwargs)
         elif self.model:
-            log.info(f"Accessing Replicate {self.model} coprocessor...")
+            log.info(f"Accessing Replicate {self.model} task...")
             self.args = self.args + (inference(self.model),)
 
             return self.func(*self.args, **self.kwargs)
 
     def print(self) -> None:
         log.info(f"id: {self.id}, type: {self.type}, model: {self.model}")
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/event_handler.py` & `seaplane-0.3.90b0/src/seaplane/apps/event_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,71 @@
 import traceback
 from typing import Any, Callable, Dict, List, Optional
 
-from .coprocessor import CoprocessorEvent
-from .smartpipe import SmartPipeEvent
+from .app import AppEvent
+from .task import TaskEvent
 
 
 def format_exception(e: Optional[Exception]) -> Optional[List[str]]:
     if e is None:
         return None
 
     return traceback.format_exception(type(e), e, e.__traceback__)
 
 
-def coprocessor_event_json(event: CoprocessorEvent) -> Dict[str, Any]:
+def task_event_json(event: TaskEvent) -> Dict[str, Any]:
     return {
         "id": event.id,
         "input": event.input,
         "status": event.status,
         "output": event.output,
         "error": format_exception(event.error),
     }
 
 
-def event_json(event: SmartPipeEvent) -> Dict[str, Any]:
+def event_json(event: AppEvent) -> Dict[str, Any]:
     return {
         "id": event.id,
-        "smart_pipe_id": event.smart_pipe_id,
+        "app_id": event.app_id,
         "input": event.input,
         "status": event.status,
         "output": event.output,
         "error": format_exception(event.error),
-        "coprocessors": [
-            coprocessor_event_json(coprocessor) for coprocessor in event.coprocessors
-        ],
+        "tasks": [task_event_json(task) for task in event.tasks],
     }
 
 
 class EventHandler:
     def __init__(self) -> None:
         self.on_change_event: Callable[[Dict[str, Any]], None] = lambda x: None
-        self.events: List[SmartPipeEvent] = []
+        self.events: List[AppEvent] = []
         self.active_event: List[str] = ["none"]
 
     def set_event(self, callback: Callable[[Dict[str, Any]], None]) -> None:
         self.on_change_event = callback
 
     def on_change(self, message: Dict[str, Any]) -> None:
         self.on_change_event(message)
 
-    def add_event(self, event: SmartPipeEvent) -> None:
+    def add_event(self, event: AppEvent) -> None:
         self.active_event[0] = event.id
         self.events.append(event)
 
         self.on_change_event({"type": "add_request", "payload": event_json(event)})
 
-    def update_event(self, event: SmartPipeEvent) -> None:
+    def update_event(self, event: AppEvent) -> None:
         for i, e in enumerate(self.events):
             if e.id == self.active_event[0]:
                 self.events[i] = event
 
                 self.on_change_event({"type": "update_request", "payload": event_json(event)})
                 break
 
-    def coprocessor_event(self, coprocessor_event: CoprocessorEvent) -> None:
+    def task_event(self, task_event: TaskEvent) -> None:
         for i, event in enumerate(self.events):
             if event.id == self.active_event[0]:
-                event.add_coprocessor_event(coprocessor_event)
+                event.add_task_event(task_event)
 
                 self.events[i] = event
 
                 self.on_change_event({"type": "update_request", "payload": event_json(event)})
                 break
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/executor.py` & `seaplane-0.3.90b0/src/seaplane/apps/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 import json
 from typing import Any
 
 from ..logging import log
 from ..model.errors import HTTPError
-from .coprocessor import Coprocessor, CoprocessorEvent
+from .app import App
 from .event_handler import EventHandler
+from .task import Task, TaskEvent
 
 
-class CoprocessorExecutor:
-    def execute(self, coprocessor: Coprocessor, *args: Any, **kwargs: Any) -> Any:
+class TaskExecutor:
+    def execute(self, task: Task, *args: Any, **kwargs: Any) -> Any:
         pass
 
 
-class RealCoProcessorExecutor(CoprocessorExecutor):
+class RealTaskExecutor(TaskExecutor):
     def __init__(self, event_handler: EventHandler) -> None:
         self.event_handler = event_handler
 
-    def execute(self, coprocessor: Coprocessor, *args: Any, **kwargs: Any) -> Any:
+    def execute(self, task: Task, *args: Any, **kwargs: Any) -> Any:
         args_str = tuple(arg.decode() if isinstance(arg, bytes) else arg for arg in args)
         args_json = json.dumps(args_str)
 
-        event = CoprocessorEvent(coprocessor.id, args_json)
-        self.event_handler.coprocessor_event(event)
+        event = TaskEvent(task.id, args_json)
+        self.event_handler.task_event(event)
         result = None
 
         try:
-            result = coprocessor.process(*args, **kwargs)
-            event.set_ouput(result)
+            result = task.process(*args, **kwargs)
+            event.set_output(result)
         except HTTPError as err:
-            log.error(f"Coprocessor HTTPError: {err}")
+            log.error(f"Task HTTPError: {err}")
             event.set_error(err)
         except Exception as e:
-            log.error(f"Coprocessor error: {e}")
+            log.error(f"Task error: {e}")
             event.set_error(e)
 
-        self.event_handler.coprocessor_event(event)
+        self.event_handler.task_event(event)
 
         if event.error is not None:
             raise event.error
 
         return result
 
 
-class SchemaExecutor(CoprocessorExecutor):
+class SchemaExecutor(TaskExecutor):
     def __init__(self) -> None:
         ...
 
-    def execute(self, coprocessor: Coprocessor, *args: Any, **kwargs: Any) -> Any:
+    def execute(self, task: Task, *args: Any, **kwargs: Any) -> Any:
         arguments = []
         for arg in args:
             arguments.append(arg)
 
-        coprocessor.called_from(arguments)
-        return coprocessor.id
+        task.called_from(arguments)
+        return task.id
+
+
+class AppExecutor:
+    def execute(self, app: App, *args: Any, **kwargs: Any) -> Any:
+        pass
+
+
+class ProductionAppExecutor(AppExecutor):
+    def __init__(self) -> None:
+        ...
+
+    def execute(self, app: App, *args: Any, **kwargs: Any) -> Any:
+        pass
+
+
+class DevelopmentAppExecutor(AppExecutor):
+    def __init__(self) -> None:
+        ...
+
+    def execute(self, app: App, *args: Any, **kwargs: Any) -> Any:
+        pass
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/smartpipe.py` & `seaplane-0.3.90b0/src/seaplane/apps/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 import secrets
 import string
 from typing import Any, Callable, List, Optional
 
 from ..logging import log
-from .coprocessor import Coprocessor, CoprocessorEvent
+from .task import Task, TaskEvent
 
 
 def random_id() -> str:
     alphabet = string.ascii_letters + string.digits
     random_string = "".join(secrets.choice(alphabet) for i in range(10))
     return random_string
 
 
-class SmartPipeEvent:
-    def __init__(self, smart_pipe_id: str, input: Any) -> None:
+class AppEvent:
+    def __init__(self, app_id: str, input: Any) -> None:
         self.id = random_id()
-        self.smart_pipe_id = smart_pipe_id
+        self.app_id = app_id
         self.status = "in_progress"
         self.input: Any = input
         self.output: Optional[Any] = None
-        self.coprocessors: List[CoprocessorEvent] = []
+        self.tasks: List[TaskEvent] = []
         self.error: Optional[Any] = None
 
-    def add_coprocessor_event(self, event: CoprocessorEvent) -> None:
-        for i, cp in enumerate(self.coprocessors):
+    def add_task_event(self, event: TaskEvent) -> None:
+        for i, cp in enumerate(self.tasks):
             if cp.id == event.id:
-                self.coprocessors[i] = event
+                self.tasks[i] = event
                 return
-        self.coprocessors.append(event)
+        self.tasks.append(event)
 
-    def set_ouput(self, output: Any) -> None:
+    def set_output(self, output: Any) -> None:
         self.output = output
         self.status = "completed"
 
     def set_error(self, error: Any) -> None:
         self.error = error
         self.status = "error"
 
 
-class SmartPipe:
+class App:
     def __init__(
         self,
         func: Callable[[Any], Any],
         path: str,
         method: str,
         id: str,
         parameters: Optional[List[str]],
     ) -> None:
         self.func = func
         self.path = path
         self.method = method
         self.id = id
         self.parameters = parameters
-        self.coprocessors: List[Coprocessor] = []
-        self.events: List[SmartPipeEvent] = []
+        self.tasks: List[Task] = []
+        self.events: List[AppEvent] = []
+        self.return_source = None
 
     def process(self, *args: Any, **kwargs: Any) -> Any:
         self.func(*args, *kwargs)
 
-    def add_coprocessor(self, coprocessor: Coprocessor) -> None:
-        for i, cp in enumerate(self.coprocessors):
-            if cp.id == coprocessor.id:
-                self.coprocessors[i] = coprocessor
+    def add_task(self, task: Task) -> None:
+        for i, cp in enumerate(self.tasks):
+            if cp.id == task.id:
+                self.tasks[i] = task
                 return
-        self.coprocessors.append(coprocessor)
+        self.tasks.append(task)
 
     def print(self) -> None:
         log.info(f"id: {self.id}, path: {self.path}, method: {self.method}")
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/README.md` & `seaplane-0.3.90b0/src/seaplane/apps/website/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/package.json` & `seaplane-0.3.90b0/src/seaplane/apps/website/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'name'": "'apps'"}*

```diff
@@ -11,15 +11,15 @@
         "react": "18.2.0",
         "react-dom": "18.2.0",
         "react-markdown": "^8.0.7",
         "react-syntax-highlighter": "^15.5.0",
         "socket.io-client": "^4.6.1",
         "tailwindcss": "3.3.2"
     },
-    "name": "smartpipes",
+    "name": "apps",
     "private": true,
     "scripts": {
         "build": "next build",
         "dev": "next dev",
         "lint": "next lint",
         "start": "next start"
     },
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/public/favicon.ico` & `seaplane-0.3.90b0/src/seaplane/apps/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/public/next.svg` & `seaplane-0.3.90b0/src/seaplane/apps/website/public/next.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/public/openai.png` & `seaplane-0.3.90b0/src/seaplane/apps/website/public/openai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo.svg` & `seaplane-0.3.90b0/src/seaplane/apps/website/public/seaplane_logo.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg` & `seaplane-0.3.90b0/src/seaplane/apps/website/public/seaplane_logo_mark.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/public/stabilityai.png` & `seaplane-0.3.90b0/src/seaplane/apps/website/public/stabilityai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/public/vercel.svg` & `seaplane-0.3.90b0/src/seaplane/apps/website/public/vercel.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/Header.jsx` & `seaplane-0.3.90b0/src/seaplane/apps/website/src/components/Header.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx` & `seaplane-0.3.90b0/src/seaplane/apps/website/src/components/SmartPipe.jsx`

 * *Files 11% similar despite different names*

```diff
@@ -61,18 +61,18 @@
   return error.reduce((prev, cur) => prev + cur + "\n", "")
 }
 
 function classNames(...classes) {
   return classes.filter(Boolean).join(' ')
 }
 
-const onClick = (smartPipe, body) => {
-  console.log(`Request to ${smartPipe.path} with body: ${JSON.stringify(body)}`)
-  fetch(`http://localhost:1337${smartPipe.path}`, {
-    method: smartPipe.method,    
+const onClick = (app, body) => {
+  console.log(`Request to ${app.path} with body: ${JSON.stringify(body)}`)
+  fetch(`http://localhost:1337${app.path}`, {
+    method: app.method,    
     headers: {
       'Content-Type': 'application/json'
     },
     body: body ? JSON.stringify(body) : null
   })
   .then((res) => console.log(res))
 }
@@ -82,30 +82,30 @@
   POST: 'text-purple-700 bg-purple-50 ring-purple-600/20',
   in_progress: 'text-gray-600 bg-gray-50 ring-gray-500/10',
   GET: 'text-yellow-800 bg-yellow-50 ring-yellow-600/20',  
   error: 'text-red-800 bg-red-50 ring-red-600/20',  
   completed: 'text-green-800 bg-green-50 ring-green-600/20',  
 }
 
-const getCoprocessorEvent = (currentRequest, coprocessor) => {  
+const getTaskEvent = (currentRequest, task) => {  
   if(currentRequest === undefined) return undefined
 
-  const res = currentRequest.coprocessors.filter(co => co.id === coprocessor.id)
+  const res = currentRequest.tasks.filter(co => co.id === task.id)
   return res.length > 0 ? res[0] : undefined
 }
 
-export default function SmartPipe({currentRequest, smartPipe}) {
+export default function App({currentRequest, app}) {
   const [body, setBody] = useState(undefined)
 
   return (
     <div className="flow-root">
         
-      {smartPipe?.method === 'POST' ? (<div className='mb-4'>
+      {app?.method === 'POST' ? (<div className='mb-4'>
         <label htmlFor="comment" className="block text-sm font-medium leading-6 text-gray-900">
-          Make a request to {smartPipe.method} {smartPipe.path} 
+          Make a request to {app.method} {app.path} 
         </label>
         <div className="mt-2">
           <textarea
             rows={3}
             name="comment"
             id="comment"
             placeholder=' POST body request'
@@ -114,22 +114,22 @@
             defaultValue={''}
           />
         </div>
       </div>) : null}
       <div className="flex mb-10 justify-end">        
            
                   <a
-                        onClick={() => {onClick(smartPipe, body)}}
+                        onClick={() => {onClick(app, body)}}
                         className="hidden rounded-md bg-[#00bda5] px-2.5 py-1.5 text-sm font-semibold text-white shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50 hover:text-black sm:block"
                       >
                         Make Request
                       </a>            
         </div>
       <ul role="list" className="-mb-8">
-      <li key={smartPipe.id}>
+      <li key={app.id}>
             <div className="relative pb-8">
               <span className="absolute left-4 top-4 -ml-px h-full w-0.5 bg-gray-200" aria-hidden="true" />
               <div className="relative flex space-x-3">
                 <div>
                   <span
                     className={classNames(
                       'bg-[#00bda5]',
@@ -140,21 +140,21 @@
                   </span>
                 </div>
                 <div className="flex min-w-0 flex-1 justify-between space-x-4 pt-1.5">
                   <div>                    
                     <div className="flex items-start gap-x-3">                      
                         <p
                           className={classNames(
-                            statuses[smartPipe.method],
+                            statuses[app.method],
                             'rounded-md whitespace-nowrap mt-0.5 px-1.5 py-0.5 text-xs font-medium ring-1 ring-inset'
                           )}
                         >
-                          {smartPipe.method}
+                          {app.method}
                         </p>                        
-                        <p className="text-sm font-semibold leading-6 text-gray-900">{' '+ smartPipe.id }</p>
+                        <p className="text-sm font-semibold leading-6 text-gray-900">{' '+ app.id }</p>
                                                
                       </div>                      
                       {currentRequest !== undefined ? (
                         <div className="flex my-5">
                           <p>Request input: {currentRequest.input}</p>                          
                         </div>
                       ): null}                      
@@ -169,70 +169,70 @@
                             {currentRequest.status}
                           </p>                                                  
                         </div>) : null}
                 </div>
               </div>
             </div>
           </li>
-        {smartPipe.coprocessors.map((coprocessor, eventIdx) => (
-          <li key={coprocessor.id}>
+        {app.tasks.map((task, eventIdx) => (
+          <li key={task.id}>
             <div className="relative pb-8">
-              {eventIdx !== smartPipe.coprocessors.length - 1 ? (
+              {eventIdx !== app.tasks.length - 1 ? (
                 <span className="absolute left-4 top-4 -ml-px h-full w-0.5 bg-gray-200" aria-hidden="true" />
               ) : null}
               <div className="relative flex space-x-3">
                 <div>
                   <span
                     className={classNames(
-                      icons(coprocessor.model).color,
+                      icons(task.model).color,
                       'h-8 w-8 rounded-full flex items-center justify-center ring-8 ring-white'
                     )}
                   >
-                    <Image src={icons(coprocessor.model).icon} width={24} height={24} alt="OpenAI logo" />
+                    <Image src={icons(task.model).icon} width={24} height={24} alt="OpenAI logo" />
                   </span>
                 </div>
                 <div className="flex min-w-0 flex-1 justify-between space-x-4 pt-1.5">                  
                   <div>                                                               
                     <p className="text-sm text-gray-500">
-                      {coprocessor.type === 'compute' ? 'Compute' : <span className='text-sm font-semibold'>{'Model: ' + coprocessor.model}</span> }{' '}<span className='text-sm font-semibold'>{'ID: ' + coprocessor.id} </span>
+                      {task.type === 'compute' ? 'Compute' : <span className='text-sm font-semibold'>{'Model: ' + task.model}</span> }{' '}<span className='text-sm font-semibold'>{'ID: ' + task.id} </span>
                     </p>                                                       
-                    {getCoprocessorEvent(currentRequest, coprocessor) !== undefined ? (
+                    {getTaskEvent(currentRequest, task) !== undefined ? (
                         <div>                          
                           <div className="my-5">
                             <p className="font-semibold">Input:</p>
                             <div className="bg-white border rounded-md p-4">
-                              <p className="">{getCoprocessorEvent(currentRequest, coprocessor).input}</p>
+                              <p className="">{getTaskEvent(currentRequest, task).input}</p>
                             </div>
                           </div>                           
-                          {getCoprocessorEvent(currentRequest, coprocessor).status !== 'error' ? (
+                          {getTaskEvent(currentRequest, task).status !== 'error' ? (
                             <div className="my-5">
                             <p className="font-semibold">Output:</p>
                             <div className="bg-white border rounded-md p-4">
-                              <p className="">{JSON.stringify(getCoprocessorEvent(currentRequest, coprocessor).output, null, 2)}</p>
+                              <p className="">{JSON.stringify(getTaskEvent(currentRequest, task).output, null, 2)}</p>
                             </div>
                           </div>                         
                           ): (<div className="my-5">
                           <p className="text-red-500 font-semibold">Error:</p>
                           <div className="bg-gray-300 border rounded-md p-4">
-                            <pre className="whitespace-pre-wrap break-word">{showError(getCoprocessorEvent(currentRequest, coprocessor).error)}</pre>
+                            <pre className="whitespace-pre-wrap break-word">{showError(getTaskEvent(currentRequest, task).error)}</pre>
                           </div>
                         </div>)}
                           
                         </div>
                       ): null}    
                   </div>                  
                   <div className="whitespace-nowrap text-right text-sm text-gray-500">
-                    {getCoprocessorEvent(currentRequest, coprocessor) !== undefined ?  (<div className="whitespace-nowrap text-right text-sm text-gray-500">
+                    {getTaskEvent(currentRequest, task) !== undefined ?  (<div className="whitespace-nowrap text-right text-sm text-gray-500">
                           <p
                             className={classNames(
-                              statuses[getCoprocessorEvent(currentRequest, coprocessor).status],
+                              statuses[getTaskEvent(currentRequest, task).status],
                               'rounded-md whitespace-nowrap mt-0.5 px-1.5 py-0.5 text-xs font-medium ring-1 ring-inset'
                             )}
                           >
-                            {getCoprocessorEvent(currentRequest, coprocessor).status}
+                            {getTaskEvent(currentRequest, task).status}
                           </p>                                                  
                         </div>) : null} 
                   </div>
                 </div>
               </div>
             </div>
           </li>
```

### Comparing `seaplane-0.3.9/src/seaplane/smartpipes/website/tailwind.config.js` & `seaplane-0.3.90b0/src/seaplane/apps/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.9/PKG-INFO` & `seaplane-0.3.90b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.3.9
+Version: 0.3.90b0
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-SocketIO (>=5.3.4,<6.0.0)
-Requires-Dist: attrs (==21.4.0)
-Requires-Dist: boto3 (>=1.26.142,<2.0.0)
-Requires-Dist: certifi (==2022.6.15)
-Requires-Dist: charset-normalizer (==2.1.0)
-Requires-Dist: idna (==3.3)
-Requires-Dist: iniconfig (==1.1.1)
-Requires-Dist: langchain (>=0.0.183,<0.0.184)
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: certifi (>=2022.6.15,<2023.0.0)
+Requires-Dist: charset-normalizer (>=2.1.0,<3.0.0)
+Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
+Requires-Dist: idna (>=3.3,<4.0)
+Requires-Dist: iniconfig (>=1.1.1,<2.0.0)
+Requires-Dist: langchain (>=0.0.195,<0.0.196)
+Requires-Dist: langchainplus-sdk (>=0.0.20,<0.0.21)
+Requires-Dist: nats-py (>=2.3.1,<3.0.0)
+Requires-Dist: nkeys (>=0.1.0,<0.2.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
-Requires-Dist: packaging (==21.3)
-Requires-Dist: pinecone-client (>=2.2.1,<3.0.0)
-Requires-Dist: pluggy (==1.0.0)
-Requires-Dist: py (==1.11.0)
-Requires-Dist: pyparsing (==3.0.9)
+Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: pluggy (>=1.0.0,<2.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: py (>=1.11.0,<2.0.0)
+Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Requires-Dist: pypdf (>=3.9.0,<4.0.0)
-Requires-Dist: requests (==2.28.1)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: qdrant-client (>=1.3.2,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-mock (>=1.9.3,<2.0.0)
 Requires-Dist: returns (>=0.19.0,<0.20.0)
 Requires-Dist: simplejson (>=3.17.6,<4.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
-Requires-Dist: tomli (==2.0.1)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: types-requests (>=2.28.0,<3.0.0)
 Requires-Dist: types-simplejson (>=3.17.7,<4.0.0)
-Requires-Dist: urllib3 (==1.26.9)
+Requires-Dist: types-toml (>=0.10.8.6,<0.11.0.0)
+Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Documentation, https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 Project-URL: Repository, https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 Description-Content-Type: text/markdown
 
 # Seaplane Python SDK
 [![PyPI](https://badge.fury.io/py/seaplane.svg)](https://badge.fury.io/py/seaplane)
 [![Python](https://img.shields.io/pypi/pyversions/seaplane.svg?style=plastic)](https://badge.fury.io/py/seaplane)
```

