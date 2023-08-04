# Comparing `tmp/periflow_client-0.1.4.tar.gz` & `tmp/periflow_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periflow_client-0.1.4.tar", max compression
+gzip compressed data, was "periflow_client-0.1.5.tar", max compression
```

## Comparing `periflow_client-0.1.4.tar` & `periflow_client-0.1.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    10173 2023-08-03 04:10:39.047104 periflow_client-0.1.4/LICENSE
--rw-r--r--   0        0        0     7938 2023-08-03 04:10:39.047445 periflow_client-0.1.4/README.md
--rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.4/periflow/__init__.py
--rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.4/periflow/auth.py
--rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.4/periflow/cli/__init__.py
--rw-r--r--   0        0        0    19433 2023-08-03 04:10:39.048824 periflow_client-0.1.4/periflow/cli/checkpoint.py
--rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.4/periflow/cli/credential.py
--rw-r--r--   0        0        0    18875 2023-07-26 11:08:22.668089 periflow_client-0.1.4/periflow/cli/deployment.py
--rw-r--r--   0        0        0     5142 2023-07-26 09:29:06.022605 periflow_client-0.1.4/periflow/cli/group.py
--rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.4/periflow/cli/key.py
--rw-r--r--   0        0        0     6095 2023-08-03 04:10:39.049149 periflow_client-0.1.4/periflow/cli/main.py
--rw-r--r--   0        0        0     9526 2023-07-26 09:29:06.023043 periflow_client-0.1.4/periflow/cli/project.py
--rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.4/periflow/cli/vm.py
--rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.4/periflow/client/__init__.py
--rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.4/periflow/client/base.py
--rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.4/periflow/client/checkpoint.py
--rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.4/periflow/client/credential.py
--rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.4/periflow/client/deployment.py
--rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.4/periflow/client/file.py
--rw-r--r--   0        0        0     5332 2023-07-26 09:29:06.023358 periflow_client-0.1.4/periflow/client/group.py
--rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.4/periflow/client/project.py
--rw-r--r--   0        0        0     7003 2023-07-26 09:29:06.023578 periflow_client-0.1.4/periflow/client/user.py
--rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.4/periflow/cloud/__init__.py
--rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.4/periflow/cloud/storage.py
--rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.4/periflow/configurator/__init__.py
--rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.4/periflow/configurator/base.py
--rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.4/periflow/configurator/credential.py
--rw-r--r--   0        0        0     3108 2023-08-03 04:10:39.049617 periflow_client-0.1.4/periflow/configurator/deployment.py
--rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.4/periflow/context.py
--rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.4/periflow/converter/__init__.py
--rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.4/periflow/converter/base.py
--rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.4/periflow/converter/interface.py
--rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.4/periflow/converter/maps.py
--rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.4/periflow/converter/models/blenderbot.py
--rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.4/periflow/converter/models/bloom.py
--rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.4/periflow/converter/models/codegen.py
--rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.4/periflow/converter/models/falcon.py
--rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.4/periflow/converter/models/gpt2.py
--rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.4/periflow/converter/models/gpt_neox.py
--rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.4/periflow/converter/models/gptj.py
--rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.4/periflow/converter/models/llama.py
--rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.4/periflow/converter/models/mpt.py
--rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.4/periflow/converter/models/opt.py
--rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.4/periflow/converter/models/t5.py
--rw-r--r--   0        0        0     4653 2023-08-03 04:10:39.050057 periflow_client-0.1.4/periflow/converter/utils.py
--rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.4/periflow/enums.py
--rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.4/periflow/errors.py
--rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.4/periflow/formatter.py
--rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.4/periflow/logging.py
--rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.4/periflow/schema/__init__.py
--rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.4/periflow/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.4/periflow/schema/api/v1/__init__.py
--rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.4/periflow/schema/api/v1/completion.py
--rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.4/periflow/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.4/periflow/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.4/periflow/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.4/periflow/schema/resource/v1/checkpoint.py
--rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.4/periflow/schema/resource/v1/credential.py
--rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.4/periflow/schema/resource/v1/deployment.py
--rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.4/periflow/sdk/__init__.py
--rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.4/periflow/sdk/api/__init__.py
--rw-r--r--   0        0        0     5757 2023-07-26 11:08:22.668388 periflow_client-0.1.4/periflow/sdk/api/base.py
--rw-r--r--   0        0        0    25710 2023-07-26 11:08:22.668715 periflow_client-0.1.4/periflow/sdk/api/completion.py
--rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.4/periflow/sdk/init.py
--rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.4/periflow/sdk/resource/__init__.py
--rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.4/periflow/sdk/resource/base.py
--rw-r--r--   0        0        0    31434 2023-08-03 04:10:39.050373 periflow_client-0.1.4/periflow/sdk/resource/checkpoint.py
--rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.4/periflow/sdk/resource/credential.py
--rw-r--r--   0        0        0    18055 2023-08-03 04:10:39.050794 periflow_client-0.1.4/periflow/sdk/resource/deployment.py
--rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.4/periflow/utils/__init__.py
--rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.4/periflow/utils/format.py
--rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.4/periflow/utils/fs.py
--rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.4/periflow/utils/maps.py
--rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.4/periflow/utils/prompt.py
--rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.4/periflow/utils/request.py
--rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.4/periflow/utils/testing.py
--rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.4/periflow/utils/url.py
--rw-r--r--   0        0        0     3938 2023-08-03 04:10:39.051071 periflow_client-0.1.4/periflow/utils/validate.py
--rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.4/periflow/utils/version.py
--rw-r--r--   0        0        0     3417 2023-08-03 04:10:34.206346 periflow_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9673 1970-01-01 00:00:00.000000 periflow_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-08-03 04:10:39.047104 periflow_client-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8240 2023-08-04 03:16:55.492601 periflow_client-0.1.5/README.md
+-rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.5/periflow/__init__.py
+-rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.5/periflow/auth.py
+-rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.5/periflow/cli/__init__.py
+-rw-r--r--   0        0        0    19373 2023-08-04 04:33:07.704594 periflow_client-0.1.5/periflow/cli/checkpoint.py
+-rw-r--r--   0        0        0    10309 2023-08-04 04:33:07.704989 periflow_client-0.1.5/periflow/cli/credential.py
+-rw-r--r--   0        0        0    18875 2023-07-26 11:08:22.668089 periflow_client-0.1.5/periflow/cli/deployment.py
+-rw-r--r--   0        0        0     5142 2023-07-26 09:29:06.022605 periflow_client-0.1.5/periflow/cli/group.py
+-rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.5/periflow/cli/key.py
+-rw-r--r--   0        0        0     6095 2023-08-04 02:45:33.047398 periflow_client-0.1.5/periflow/cli/main.py
+-rw-r--r--   0        0        0     9501 2023-08-04 04:33:07.705242 periflow_client-0.1.5/periflow/cli/project.py
+-rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.5/periflow/cli/vm.py
+-rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.5/periflow/client/__init__.py
+-rw-r--r--   0        0        0    15578 2023-08-04 04:33:07.705754 periflow_client-0.1.5/periflow/client/base.py
+-rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.5/periflow/client/checkpoint.py
+-rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.5/periflow/client/credential.py
+-rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.5/periflow/client/deployment.py
+-rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.5/periflow/client/file.py
+-rw-r--r--   0        0        0     5332 2023-07-26 09:29:06.023358 periflow_client-0.1.5/periflow/client/group.py
+-rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.5/periflow/client/project.py
+-rw-r--r--   0        0        0     7003 2023-07-26 09:29:06.023578 periflow_client-0.1.5/periflow/client/user.py
+-rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.5/periflow/cloud/__init__.py
+-rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.5/periflow/cloud/storage.py
+-rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.5/periflow/configurator/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.5/periflow/configurator/base.py
+-rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.5/periflow/configurator/credential.py
+-rw-r--r--   0        0        0     3108 2023-08-03 04:10:39.049617 periflow_client-0.1.5/periflow/configurator/deployment.py
+-rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.5/periflow/context.py
+-rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.5/periflow/converter/__init__.py
+-rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.5/periflow/converter/base.py
+-rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.5/periflow/converter/interface.py
+-rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.5/periflow/converter/maps.py
+-rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.5/periflow/converter/models/blenderbot.py
+-rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.5/periflow/converter/models/bloom.py
+-rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.5/periflow/converter/models/codegen.py
+-rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.5/periflow/converter/models/falcon.py
+-rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.5/periflow/converter/models/gpt2.py
+-rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.5/periflow/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.5/periflow/converter/models/gptj.py
+-rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.5/periflow/converter/models/llama.py
+-rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.5/periflow/converter/models/mpt.py
+-rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.5/periflow/converter/models/opt.py
+-rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.5/periflow/converter/models/t5.py
+-rw-r--r--   0        0        0     4653 2023-08-04 02:45:33.048315 periflow_client-0.1.5/periflow/converter/utils.py
+-rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.5/periflow/enums.py
+-rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.5/periflow/errors.py
+-rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.5/periflow/formatter.py
+-rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.5/periflow/logging.py
+-rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.5/periflow/schema/__init__.py
+-rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.5/periflow/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.5/periflow/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.5/periflow/schema/api/v1/completion.py
+-rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.5/periflow/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.5/periflow/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     4215 2023-08-04 03:16:55.494228 periflow_client-0.1.5/periflow/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.5/periflow/schema/resource/v1/checkpoint.py
+-rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.5/periflow/schema/resource/v1/credential.py
+-rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.5/periflow/schema/resource/v1/deployment.py
+-rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.5/periflow/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.5/periflow/sdk/api/__init__.py
+-rw-r--r--   0        0        0     5757 2023-07-26 11:08:22.668388 periflow_client-0.1.5/periflow/sdk/api/base.py
+-rw-r--r--   0        0        0    25710 2023-07-26 11:08:22.668715 periflow_client-0.1.5/periflow/sdk/api/completion.py
+-rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.5/periflow/sdk/init.py
+-rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.5/periflow/sdk/resource/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.5/periflow/sdk/resource/base.py
+-rw-r--r--   0        0        0    31434 2023-08-04 02:45:33.048859 periflow_client-0.1.5/periflow/sdk/resource/checkpoint.py
+-rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.5/periflow/sdk/resource/credential.py
+-rw-r--r--   0        0        0    18055 2023-08-03 04:10:39.050794 periflow_client-0.1.5/periflow/sdk/resource/deployment.py
+-rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.5/periflow/utils/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.5/periflow/utils/format.py
+-rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.5/periflow/utils/fs.py
+-rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.5/periflow/utils/maps.py
+-rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.5/periflow/utils/prompt.py
+-rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.5/periflow/utils/request.py
+-rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.5/periflow/utils/testing.py
+-rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.5/periflow/utils/url.py
+-rw-r--r--   0        0        0     3938 2023-08-04 02:45:33.049462 periflow_client-0.1.5/periflow/utils/validate.py
+-rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.5/periflow/utils/version.py
+-rw-r--r--   0        0        0     3417 2023-08-04 04:32:54.507659 periflow_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9975 1970-01-01 00:00:00.000000 periflow_client-0.1.5/PKG-INFO
```

### Comparing `periflow_client-0.1.4/LICENSE` & `periflow_client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/README.md` & `periflow_client-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,20 @@
 
 ## Installation
 
 ```sh
 pip install periflow-client
 ```
 
+If you have a Hugging Face checkpoint and want to convert it to a PeriFlow-compatible format, you need to install the package with the necessary machine learing library (`mllib`) dependencies. In this case, install the package with the following command:
+
+```sh
+pip install periflow-client[mllib]
+```
+
 ## Examples
 
 This example shows how to create a deployment and send a completion API request to the created deployment with Python SDK.
 
 ```python
 import periflow as pf
```

#### html2text {}

```diff
@@ -47,20 +47,24 @@
 currently deployed model, allowing users a more stable model serving
 experience. When the number of requests sent to the deployed model increases,
 PeriFlow cloud automatically assigns more resources (GPU VMs) to the model,
 while it reduces resource usage when there are not as many requests.
 Furthermore, if a certain resource malfunctions, PeriFlow cloud proceeds with
 recovery based on the monitoring results. # ð¹ï¸ PeriFlow Client Check out
 [PeriFlow Client Docs](https://docs.periflow.ai/) to learn more. ##
-Installation ```sh pip install periflow-client ``` ## Examples This example
-shows how to create a deployment and send a completion API request to the
-created deployment with Python SDK. ```python import periflow as pf # Set up
-PeriFlow context. pf.init( api_key="YOUR_PERIFLOW_API_KEY", project_name="my-
-project", ) # Create a deployment at GCP asia-northest3 region wtih one A100
-GPU. deployment = pf.Deployment.create( checkpoint_id="YOUR_CHECKPOINT_ID",
+Installation ```sh pip install periflow-client ``` If you have a Hugging Face
+checkpoint and want to convert it to a PeriFlow-compatible format, you need to
+install the package with the necessary machine learing library (`mllib`)
+dependencies. In this case, install the package with the following command:
+```sh pip install periflow-client[mllib] ``` ## Examples This example shows how
+to create a deployment and send a completion API request to the created
+deployment with Python SDK. ```python import periflow as pf # Set up PeriFlow
+context. pf.init( api_key="YOUR_PERIFLOW_API_KEY", project_name="my-project", )
+# Create a deployment at GCP asia-northest3 region wtih one A100 GPU.
+deployment = pf.Deployment.create( checkpoint_id="YOUR_CHECKPOINT_ID",
 name="my-deployment", cloud="gcp", region="asia-northeast3", vm_type="a2-
 highgpu-1g", ... ) ``` When the deployment becomes the "Healthy" status and
 ready to process inference requests, you can generate a completion with:
 ```python # Generate a completion by sending an inference request to the
 deployment created above. api = pf.Completion
 (deployment_id=deployment.deployment_id) completion = api.create
 ( options=pf.V1CompletionOptions( prompt="Python is a popular language for",
```

### Comparing `periflow_client-0.1.4/periflow/__init__.py` & `periflow_client-0.1.5/periflow/__init__.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/auth.py` & `periflow_client-0.1.5/periflow/auth.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/cli/checkpoint.py` & `periflow_client-0.1.5/periflow/cli/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,15 +381,15 @@
     """Deletes the existing checkpoint.
 
     :::info
     Deleting linked checkpoints created with `pf checkpoint create` simply unlinks the
     checkpoint from the PeriFlow system. That is, it does not physically delete the
     checkpoint objects from the source cloud storage (your cloud storage).
 
-    Checkpoints that are uploaded or generated from training jobs are physically deleted.
+    Uploaded checkpoints are physically deleted.
     :::
 
     """
     targets_str = ""
     for checkpoint_id in checkpoint_ids:
         targets_str += str(checkpoint_id)
         targets_str += "\n"
@@ -605,18 +605,17 @@
 
 @app.command()
 def restore(
     checkpoint_id: UUID = typer.Argument(..., help="ID of checkpoint to restore.")
 ):
     """Restores deleted checkpoint (available within 24 hours from the deletion).
 
-    When a checkpoint that is uploaded or generated from the training job is deleted,
-    it is not physically deleted right away. Instead, it is soft-deleted and can be
-    restored within 24 hours after the deletion. After the 24-hour retention period, it
-    is hard-deleted and cannot be restored.
+    When a uploaded checkpoint is deleted, it is not physically deleted right away.
+    Instead, it is soft-deleted and can be restored within 24 hours after the deletion.
+    After the 24-hour retention period, it is hard-deleted and cannot be restored.
 
     :::caution
     When you delete a linked checkpoint, you cannot restore it. Instead, relink the
     original checkpoint using `pf checkpoint create`.
     :::
 
     """
@@ -672,19 +671,18 @@
         "attr.yaml",
         "--output-attr-filename",
         help="Name of the checkpoint attribute file.",
     ),
 ):
     """Convert huggingface's model checkpoint to PeriFlow format.
 
-    ::: info
-    When a checkpoint has Hugging Face format, it cannot be served right away. Instead,
-    it needs to be converted to PeriFlow format for serving. From the orignal checkpoint,
-    it is copied and converted to Periflow format checkpoint(*.h5).
-    :::
+    When a checkpoint is in the Hugging Face format, it cannot be directly served;
+    rather, it requires conversion to the PeriFlow format for serving. The conversion
+    process involves copying the original checkpoint and transforming it into a
+    checkpoint in the PeriFlow format (*.h5).
 
     :::caution
     The `pf checkpoint convert` is available only when the package is installed with
     `pip install periflow-client[mllib]`.
     :::
 
     """
```

### Comparing `periflow_client-0.1.4/periflow/cli/credential.py` & `periflow_client-0.1.5/periflow/cli/credential.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     service_account_key_file: typer.FileText = typer.Option(
         ...,
         help=f"[GCP] Path to GCP Service Account Key JSON file. Please refer to {GCP_DOC_LINK}.",
     ),
 ):
     r"""Creates a credential for Google Cloud Storage.
 
-    To use checkpoints or datasets in the Google Cloud Storage, you must create a
+    To use checkpoints in the Google Cloud Storage, you must create a
     credential to access the GCS buckets.
 
 
     :::tip
     How to get a JSON file containing your GCP service account key for the `--service-account-key-file` option:
 
     1. Go to Google Cloud Platform Console, and sign in.
```

### Comparing `periflow_client-0.1.4/periflow/cli/deployment.py` & `periflow_client-0.1.5/periflow/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/cli/group.py` & `periflow_client-0.1.5/periflow/cli/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/cli/key.py` & `periflow_client-0.1.5/periflow/cli/key.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/cli/main.py` & `periflow_client-0.1.5/periflow/cli/main.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/cli/project.py` & `periflow_client-0.1.5/periflow/cli/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 
 @app.command()
 def create(name: str = typer.Argument(..., help="Name of project to create")):
     """Create a new project.
 
     :::info
-    Every resource within a project, such as datasets, checkpoints, and jobs,
+    Every resource within a project, such as credentials, checkpoints, and deployments,
     is shared with project members.
     :::
 
     """
     client = GroupProjectClient()
     project_detail = client.create_project(name)
     project_panel_formatter.render(project_detail)
@@ -266,18 +266,18 @@
 
     | | Admin | Maintainer | Developer | Guest |
     |-|-|-|-|-|
     | Add organization members to the project | ✓ | ✗ | ✗ | ✗ |
     | Assign project roles | ✓ | ✗ | ✗ | ✗ |
     | Delete project | ✓ | ✗ | ✗ | ✗ |
     | Delete & edit checkpoints | ✓ | ✗ | ✗ | ✗ |
-    | Delete & edit datasets, credentials, jobs | ✓ | ✓ | ✗ | ✗ |
-    | Creaete datasets, credentials | ✓ | ✓ | ✗ | ✗ |
-    | Create checkpoints, deployments, jobs | ✓ | ✓ | ✓ | ✗ |
-    | Read checkpoints, datasets, credentials, deployments, jobs | ✓ | ✓ | ✓ | ✓ |
+    | Delete & edit credentials, deployments | ✓ | ✓ | ✗ | ✗ |
+    | Creaete credentials | ✓ | ✓ | ✗ | ✗ |
+    | Create checkpoints, deployments | ✓ | ✓ | ✓ | ✗ |
+    | Read checkpoints, credentials, deployments | ✓ | ✓ | ✓ | ✓ |
     | Send inference requests to deployments | ✓ | ✓ | ✓ | ✓ |
 
     :::info
     Only the **Admin** users can assign roles to project members:
     :::
 
     :::info
```

### Comparing `periflow_client-0.1.4/periflow/cli/vm.py` & `periflow_client-0.1.5/periflow/cli/vm.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/client/base.py` & `periflow_client-0.1.5/periflow/client/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 
     def get_mpu_urls(
         self,
         obj_id: T,
         local_paths: List[str],
         storage_paths: List[str],
     ) -> List[Dict[str, Any]]:
-        """Get multipart upload URLs for multiple datasets.
+        """Get multipart upload URLs for multiple file-like objects.
 
         Args:
             obj_id (T): Uploadable object ID
             local_paths (List[str]): A list local paths to target files. The path can be
                 either absolute or relative.
             storage_paths (List[str]): A list of storage paths to target files.
 
@@ -406,15 +406,15 @@
         max_workers: int = min(
             32, (os.cpu_count() or 1) + 4
         ),  # default of ``ThreadPoolExecutor``
     ) -> None:
         """Upload files.
 
         Args:
-            obj_id (T): PeriFlow resource(i.e., dataset, checkpoint) object ID.
+            obj_id (T): PeriFlow resource(i.e., checkpoint) object ID.
             spu_url_dicts (List[Dict[str, str]]): Single-part upload URL info.
             mpu_url_dicts (List[Dict[str, Any]]): Multi-part upload URL info.
             source_path (Path): Path to the local source directory.
             max_workers (int, optional): Max number of workers for the concurrent uploading.
 
         """
         spu_local_paths = [
```

### Comparing `periflow_client-0.1.4/periflow/client/checkpoint.py` & `periflow_client-0.1.5/periflow/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/client/credential.py` & `periflow_client-0.1.5/periflow/client/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/client/deployment.py` & `periflow_client-0.1.5/periflow/client/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/client/file.py` & `periflow_client-0.1.5/periflow/client/file.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/client/group.py` & `periflow_client-0.1.5/periflow/client/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/client/project.py` & `periflow_client-0.1.5/periflow/client/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/client/user.py` & `periflow_client-0.1.5/periflow/client/user.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/cloud/storage.py` & `periflow_client-0.1.5/periflow/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/configurator/base.py` & `periflow_client-0.1.5/periflow/configurator/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/configurator/credential.py` & `periflow_client-0.1.5/periflow/configurator/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/configurator/deployment.py` & `periflow_client-0.1.5/periflow/configurator/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/context.py` & `periflow_client-0.1.5/periflow/context.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/base.py` & `periflow_client-0.1.5/periflow/converter/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/interface.py` & `periflow_client-0.1.5/periflow/converter/interface.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/maps.py` & `periflow_client-0.1.5/periflow/converter/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/blenderbot.py` & `periflow_client-0.1.5/periflow/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/bloom.py` & `periflow_client-0.1.5/periflow/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/codegen.py` & `periflow_client-0.1.5/periflow/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/falcon.py` & `periflow_client-0.1.5/periflow/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/gpt2.py` & `periflow_client-0.1.5/periflow/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/gpt_neox.py` & `periflow_client-0.1.5/periflow/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/gptj.py` & `periflow_client-0.1.5/periflow/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/llama.py` & `periflow_client-0.1.5/periflow/converter/models/llama.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/mpt.py` & `periflow_client-0.1.5/periflow/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/opt.py` & `periflow_client-0.1.5/periflow/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/models/t5.py` & `periflow_client-0.1.5/periflow/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/converter/utils.py` & `periflow_client-0.1.5/periflow/converter/utils.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/enums.py` & `periflow_client-0.1.5/periflow/enums.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/errors.py` & `periflow_client-0.1.5/periflow/errors.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/formatter.py` & `periflow_client-0.1.5/periflow/formatter.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/logging.py` & `periflow_client-0.1.5/periflow/logging.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/schema/api/v1/completion.py` & `periflow_client-0.1.5/periflow/schema/api/v1/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/schema/resource/v1/attributes.py` & `periflow_client-0.1.5/periflow/schema/resource/v1/attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,27 @@
     num_heads: int
     num_layers: int
     max_length: int
     vocab_size: int
     eos_token: int
 
 
+class V1GPTNeoXHFAttributes(V1CommonAttributes):
+    """V1 GPT-NeoX HF attributes schema."""
+
+    model_type: Literal["gpt-neox-hf"]
+    head_size: int
+    rotary_dim: int
+    num_heads: int
+    num_layers: int
+    max_length: int
+    vocab_size: int
+    eos_token: int
+
+
 class V1LlamaAttributes(V1CommonAttributes):
     """V1 LLaMA attributes schema."""
 
     model_type: Literal["llama"]
     head_size: int
     rotary_dim: int
     num_heads: int
@@ -164,14 +177,15 @@
     Union[
         V1BlenderbotAttributes,
         V1BloomAttributes,
         V1FalconAttributes,
         V1GPTAttributes,
         V1GPTJAttributes,
         V1GPTNeoXAttributes,
+        V1GPTNeoXHFAttributes,
         V1LlamaAttributes,
         V1MPTAttributes,
         V1OPTAttributes,
         V1T5Attributes,
     ],
     Field(discriminator="model_type"),
 ]
```

### Comparing `periflow_client-0.1.4/periflow/schema/resource/v1/checkpoint.py` & `periflow_client-0.1.5/periflow/schema/resource/v1/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/schema/resource/v1/credential.py` & `periflow_client-0.1.5/periflow/schema/resource/v1/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/schema/resource/v1/deployment.py` & `periflow_client-0.1.5/periflow/schema/resource/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/sdk/api/base.py` & `periflow_client-0.1.5/periflow/sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/sdk/api/completion.py` & `periflow_client-0.1.5/periflow/sdk/api/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/sdk/init.py` & `periflow_client-0.1.5/periflow/sdk/init.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/sdk/resource/base.py` & `periflow_client-0.1.5/periflow/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/sdk/resource/checkpoint.py` & `periflow_client-0.1.5/periflow/sdk/resource/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/sdk/resource/credential.py` & `periflow_client-0.1.5/periflow/sdk/resource/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/sdk/resource/deployment.py` & `periflow_client-0.1.5/periflow/sdk/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/format.py` & `periflow_client-0.1.5/periflow/utils/format.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/fs.py` & `periflow_client-0.1.5/periflow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/maps.py` & `periflow_client-0.1.5/periflow/utils/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/prompt.py` & `periflow_client-0.1.5/periflow/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/request.py` & `periflow_client-0.1.5/periflow/utils/request.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/testing.py` & `periflow_client-0.1.5/periflow/utils/testing.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/url.py` & `periflow_client-0.1.5/periflow/utils/url.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/validate.py` & `periflow_client-0.1.5/periflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/periflow/utils/version.py` & `periflow_client-0.1.5/periflow/utils/version.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.4/pyproject.toml` & `periflow_client-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "periflow-client"
-version = "0.1.4"
+version = "0.1.5"
 description = "Client of PeriFlow, the fastest generative AI serving available."
 license = "Apache-2.0"
 authors = ["PeriFlow teams <eng@friendli.ai>"]
 packages = [
     { include = "periflow" },
 ]
 readme = "README.md"
```

### Comparing `periflow_client-0.1.4/PKG-INFO` & `periflow_client-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periflow-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Client of PeriFlow, the fastest generative AI serving available.
 Home-page: https://docs.periflow.ai/
 License: Apache-2.0
 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams
 Author-email: eng@friendli.ai
 Requires-Python: >=3.8,<4.0
@@ -103,14 +103,20 @@
 
 ## Installation
 
 ```sh
 pip install periflow-client
 ```
 
+If you have a Hugging Face checkpoint and want to convert it to a PeriFlow-compatible format, you need to install the package with the necessary machine learing library (`mllib`) dependencies. In this case, install the package with the following command:
+
+```sh
+pip install periflow-client[mllib]
+```
+
 ## Examples
 
 This example shows how to create a deployment and send a completion API request to the created deployment with Python SDK.
 
 ```python
 import periflow as pf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: periflow-client Version: 0.1.4 Summary: Client of
+Metadata-Version: 2.1 Name: periflow-client Version: 0.1.5 Summary: Client of
 PeriFlow, the fastest generative AI serving available. Home-page: https://
 docs.periflow.ai/ License: Apache-2.0 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams Author-email: eng@friendli.ai Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -70,20 +70,24 @@
 currently deployed model, allowing users a more stable model serving
 experience. When the number of requests sent to the deployed model increases,
 PeriFlow cloud automatically assigns more resources (GPU VMs) to the model,
 while it reduces resource usage when there are not as many requests.
 Furthermore, if a certain resource malfunctions, PeriFlow cloud proceeds with
 recovery based on the monitoring results. # ð¹ï¸ PeriFlow Client Check out
 [PeriFlow Client Docs](https://docs.periflow.ai/) to learn more. ##
-Installation ```sh pip install periflow-client ``` ## Examples This example
-shows how to create a deployment and send a completion API request to the
-created deployment with Python SDK. ```python import periflow as pf # Set up
-PeriFlow context. pf.init( api_key="YOUR_PERIFLOW_API_KEY", project_name="my-
-project", ) # Create a deployment at GCP asia-northest3 region wtih one A100
-GPU. deployment = pf.Deployment.create( checkpoint_id="YOUR_CHECKPOINT_ID",
+Installation ```sh pip install periflow-client ``` If you have a Hugging Face
+checkpoint and want to convert it to a PeriFlow-compatible format, you need to
+install the package with the necessary machine learing library (`mllib`)
+dependencies. In this case, install the package with the following command:
+```sh pip install periflow-client[mllib] ``` ## Examples This example shows how
+to create a deployment and send a completion API request to the created
+deployment with Python SDK. ```python import periflow as pf # Set up PeriFlow
+context. pf.init( api_key="YOUR_PERIFLOW_API_KEY", project_name="my-project", )
+# Create a deployment at GCP asia-northest3 region wtih one A100 GPU.
+deployment = pf.Deployment.create( checkpoint_id="YOUR_CHECKPOINT_ID",
 name="my-deployment", cloud="gcp", region="asia-northeast3", vm_type="a2-
 highgpu-1g", ... ) ``` When the deployment becomes the "Healthy" status and
 ready to process inference requests, you can generate a completion with:
 ```python # Generate a completion by sending an inference request to the
 deployment created above. api = pf.Completion
 (deployment_id=deployment.deployment_id) completion = api.create
 ( options=pf.V1CompletionOptions( prompt="Python is a popular language for",
```

