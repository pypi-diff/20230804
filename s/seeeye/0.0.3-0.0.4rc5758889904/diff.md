# Comparing `tmp/seeeye-0.0.3-py3-none-any.whl.zip` & `tmp/seeeye-0.0.4rc5758889904-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,73 +1,82 @@
-Zip file size: 38033 bytes, number of entries: 71
--rw-r--r--  2.0 unx      165 b- defN 23-Jul-28 01:25 cicd/cli.py
--rw-r--r--  2.0 unx      174 b- defN 23-Jul-28 01:25 cicd/core/action.py
--rw-r--r--  2.0 unx     3100 b- defN 23-Jul-28 01:25 cicd/core/client.py
--rw-r--r--  2.0 unx      131 b- defN 23-Jul-28 01:25 cicd/core/env.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Jul-28 01:25 cicd/core/logger.py
--rw-r--r--  2.0 unx      333 b- defN 23-Jul-28 01:25 cicd/core/_cli/opts.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jul-28 01:25 cicd/core/mixin/core.py
--rw-r--r--  2.0 unx      282 b- defN 23-Jul-28 01:25 cicd/core/mixin/git.py
--rw-r--r--  2.0 unx      115 b- defN 23-Jul-28 01:25 cicd/core/mixin/logger.py
--rw-r--r--  2.0 unx     1552 b- defN 23-Jul-28 01:25 cicd/core/mixin/provider.py
--rw-r--r--  2.0 unx      261 b- defN 23-Jul-28 01:25 cicd/core/mixin/step.py
--rw-r--r--  2.0 unx     1237 b- defN 23-Jul-28 01:25 cicd/core/provider/client.py
--rw-r--r--  2.0 unx     1261 b- defN 23-Jul-28 01:25 cicd/core/provider/info.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jul-28 01:25 cicd/core/provider/models/api.py
--rw-r--r--  2.0 unx     1878 b- defN 23-Jul-28 01:25 cicd/core/provider/models/base.py
--rw-r--r--  2.0 unx      158 b- defN 23-Jul-28 01:25 cicd/core/provider/models/pr.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-28 01:25 cicd/core/provider/models/project.py
--rw-r--r--  2.0 unx     1929 b- defN 23-Jul-28 01:25 cicd/core/syntax/data_represented.py
--rw-r--r--  2.0 unx      563 b- defN 23-Jul-28 01:25 cicd/core/syntax/json.py
--rw-r--r--  2.0 unx      253 b- defN 23-Jul-28 01:25 cicd/core/syntax/yaml.py
--rw-r--r--  2.0 unx      827 b- defN 23-Jul-28 01:25 cicd/core/utils/cli_group.py
--rw-r--r--  2.0 unx      534 b- defN 23-Jul-28 01:25 cicd/core/utils/file.py
--rw-r--r--  2.0 unx     1708 b- defN 23-Jul-28 01:25 cicd/core/utils/sh.py
--rw-r--r--  2.0 unx      369 b- defN 23-Jul-28 01:25 cicd/core/utils/step.py
--rw-r--r--  2.0 unx      970 b- defN 23-Jul-28 01:25 cicd/core/utils/timeout.py
--rw-r--r--  2.0 unx     3352 b- defN 23-Jul-28 01:25 cicd/ios/cli.py
--rw-r--r--  2.0 unx     2482 b- defN 23-Jul-28 01:25 cicd/ios/actions/base.py
--rw-r--r--  2.0 unx      690 b- defN 23-Jul-28 01:25 cicd/ios/actions/cov.py
--rw-r--r--  2.0 unx     1170 b- defN 23-Jul-28 01:25 cicd/ios/actions/test_extraction.py
--rw-r--r--  2.0 unx       84 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/__init__.py
--rw-r--r--  2.0 unx     3413 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/archive.py
--rw-r--r--  2.0 unx     5150 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/base.py
--rw-r--r--  2.0 unx      583 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/build.py
--rw-r--r--  2.0 unx     1102 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/test.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jul-28 01:25 cicd/ios/cov/__init__.py
--rw-r--r--  2.0 unx      378 b- defN 23-Jul-28 01:25 cicd/ios/cov/config.py
--rw-r--r--  2.0 unx      767 b- defN 23-Jul-28 01:25 cicd/ios/cov/cov.py
--rw-r--r--  2.0 unx     2273 b- defN 23-Jul-28 01:25 cicd/ios/cov/report.py
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-28 01:25 cicd/ios/mixin/archive.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-28 01:25 cicd/ios/mixin/base_ios.py
--rw-r--r--  2.0 unx      389 b- defN 23-Jul-28 01:25 cicd/ios/mixin/build.py
--rw-r--r--  2.0 unx      566 b- defN 23-Jul-28 01:25 cicd/ios/mixin/cocoapods.py
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-28 01:25 cicd/ios/mixin/cov.py
--rw-r--r--  2.0 unx      186 b- defN 23-Jul-28 01:25 cicd/ios/mixin/metadata.py
--rw-r--r--  2.0 unx      212 b- defN 23-Jul-28 01:25 cicd/ios/mixin/mono.py
--rw-r--r--  2.0 unx      469 b- defN 23-Jul-28 01:25 cicd/ios/mixin/simulator.py
--rw-r--r--  2.0 unx      603 b- defN 23-Jul-28 01:25 cicd/ios/mixin/test.py
--rw-r--r--  2.0 unx     1267 b- defN 23-Jul-28 01:25 cicd/ios/mixin/test_sharding.py
--rw-r--r--  2.0 unx     2022 b- defN 23-Jul-28 01:25 cicd/ios/project/metadata.py
--rw-r--r--  2.0 unx     1967 b- defN 23-Jul-28 01:25 cicd/ios/runner/base.py
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/__init__.py
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/archive.py
--rw-r--r--  2.0 unx      279 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/build.py
--rw-r--r--  2.0 unx      623 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/test.py
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-28 01:25 cicd/ios/simulator/__init__.py
--rw-r--r--  2.0 unx     5181 b- defN 23-Jul-28 01:25 cicd/ios/simulator/simulator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/ios/syntax/__init__.py
--rw-r--r--  2.0 unx     4600 b- defN 23-Jul-28 01:25 cicd/ios/syntax/xcresult.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/providers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/providers/github/__init__.py
--rw-r--r--  2.0 unx      929 b- defN 23-Jul-28 01:25 cicd/providers/github/client.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jul-28 01:25 cicd/providers/github/env.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/providers/gitlab/__init__.py
--rw-r--r--  2.0 unx      134 b- defN 23-Jul-28 01:25 cicd/providers/gitlab/client.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jul-28 01:25 cicd/providers/gitlab/env.py
--rw-r--r--  2.0 unx     1092 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2941 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5874 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/RECORD
-71 files, 73171 bytes uncompressed, 28721 bytes compressed:  60.7%
+Zip file size: 43480 bytes, number of entries: 80
+-rw-r--r--  2.0 unx      240 b- defN 23-Aug-04 05:47 cicd/cli.py
+-rw-r--r--  2.0 unx      174 b- defN 23-Aug-04 05:47 cicd/core/action.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Aug-04 05:47 cicd/core/cli.py
+-rw-r--r--  2.0 unx     3100 b- defN 23-Aug-04 05:47 cicd/core/client.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Aug-04 05:47 cicd/core/env.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Aug-04 05:47 cicd/core/logger.py
+-rw-r--r--  2.0 unx       74 b- defN 23-Aug-04 05:47 cicd/core/typing.py
+-rw-r--r--  2.0 unx      332 b- defN 23-Aug-04 05:47 cicd/core/_cli/opts.py
+-rw-r--r--  2.0 unx     2605 b- defN 23-Aug-04 05:47 cicd/core/cipher/cipher.py
+-rw-r--r--  2.0 unx      839 b- defN 23-Aug-04 05:47 cicd/core/cipher/cli.py
+-rw-r--r--  2.0 unx      163 b- defN 23-Aug-04 05:47 cicd/core/mixin/core.py
+-rw-r--r--  2.0 unx      282 b- defN 23-Aug-04 05:47 cicd/core/mixin/git.py
+-rw-r--r--  2.0 unx      115 b- defN 23-Aug-04 05:47 cicd/core/mixin/logger.py
+-rw-r--r--  2.0 unx     1552 b- defN 23-Aug-04 05:47 cicd/core/mixin/provider.py
+-rw-r--r--  2.0 unx      261 b- defN 23-Aug-04 05:47 cicd/core/mixin/step.py
+-rw-r--r--  2.0 unx     1237 b- defN 23-Aug-04 05:47 cicd/core/provider/client.py
+-rw-r--r--  2.0 unx     1261 b- defN 23-Aug-04 05:47 cicd/core/provider/info.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Aug-04 05:47 cicd/core/provider/models/api.py
+-rw-r--r--  2.0 unx     1878 b- defN 23-Aug-04 05:47 cicd/core/provider/models/base.py
+-rw-r--r--  2.0 unx      158 b- defN 23-Aug-04 05:47 cicd/core/provider/models/pr.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Aug-04 05:47 cicd/core/provider/models/project.py
+-rw-r--r--  2.0 unx     1848 b- defN 23-Aug-04 05:47 cicd/core/security/keychain.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Aug-04 05:47 cicd/core/syntax/data_represented.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Aug-04 05:47 cicd/core/syntax/json.py
+-rw-r--r--  2.0 unx      253 b- defN 23-Aug-04 05:47 cicd/core/syntax/yaml.py
+-rw-r--r--  2.0 unx      827 b- defN 23-Aug-04 05:47 cicd/core/utils/cli_group.py
+-rw-r--r--  2.0 unx      523 b- defN 23-Aug-04 05:47 cicd/core/utils/file.py
+-rw-r--r--  2.0 unx     1708 b- defN 23-Aug-04 05:47 cicd/core/utils/sh.py
+-rw-r--r--  2.0 unx      369 b- defN 23-Aug-04 05:47 cicd/core/utils/step.py
+-rw-r--r--  2.0 unx      970 b- defN 23-Aug-04 05:47 cicd/core/utils/timeout.py
+-rw-r--r--  2.0 unx     3449 b- defN 23-Aug-04 05:47 cicd/ios/cli.py
+-rw-r--r--  2.0 unx     2506 b- defN 23-Aug-04 05:47 cicd/ios/actions/base.py
+-rw-r--r--  2.0 unx      690 b- defN 23-Aug-04 05:47 cicd/ios/actions/cov.py
+-rw-r--r--  2.0 unx     1170 b- defN 23-Aug-04 05:47 cicd/ios/actions/test_extraction.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Aug-04 05:47 cicd/ios/actions/xcodebuild/__init__.py
+-rw-r--r--  2.0 unx     3413 b- defN 23-Aug-04 05:47 cicd/ios/actions/xcodebuild/archive.py
+-rw-r--r--  2.0 unx     5150 b- defN 23-Aug-04 05:47 cicd/ios/actions/xcodebuild/base.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Aug-04 05:47 cicd/ios/actions/xcodebuild/build.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Aug-04 05:47 cicd/ios/actions/xcodebuild/test.py
+-rw-r--r--  2.0 unx      520 b- defN 23-Aug-04 05:47 cicd/ios/codesign/cert.py
+-rw-r--r--  2.0 unx     1057 b- defN 23-Aug-04 05:47 cicd/ios/codesign/cli.py
+-rw-r--r--  2.0 unx     1915 b- defN 23-Aug-04 05:47 cicd/ios/codesign/codesign.py
+-rw-r--r--  2.0 unx      551 b- defN 23-Aug-04 05:47 cicd/ios/codesign/profile.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Aug-04 05:47 cicd/ios/cov/__init__.py
+-rw-r--r--  2.0 unx      378 b- defN 23-Aug-04 05:47 cicd/ios/cov/config.py
+-rw-r--r--  2.0 unx      767 b- defN 23-Aug-04 05:47 cicd/ios/cov/cov.py
+-rw-r--r--  2.0 unx     2273 b- defN 23-Aug-04 05:47 cicd/ios/cov/report.py
+-rw-r--r--  2.0 unx      449 b- defN 23-Aug-04 05:47 cicd/ios/mixin/archive.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Aug-04 05:47 cicd/ios/mixin/base_ios.py
+-rw-r--r--  2.0 unx      389 b- defN 23-Aug-04 05:47 cicd/ios/mixin/build.py
+-rw-r--r--  2.0 unx      566 b- defN 23-Aug-04 05:47 cicd/ios/mixin/cocoapods.py
+-rw-r--r--  2.0 unx      190 b- defN 23-Aug-04 05:47 cicd/ios/mixin/cov.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Aug-04 05:47 cicd/ios/mixin/metadata.py
+-rw-r--r--  2.0 unx      212 b- defN 23-Aug-04 05:47 cicd/ios/mixin/mono.py
+-rw-r--r--  2.0 unx      469 b- defN 23-Aug-04 05:47 cicd/ios/mixin/simulator.py
+-rw-r--r--  2.0 unx      603 b- defN 23-Aug-04 05:47 cicd/ios/mixin/test.py
+-rw-r--r--  2.0 unx     1267 b- defN 23-Aug-04 05:47 cicd/ios/mixin/test_sharding.py
+-rw-r--r--  2.0 unx     2022 b- defN 23-Aug-04 05:47 cicd/ios/project/metadata.py
+-rw-r--r--  2.0 unx     1967 b- defN 23-Aug-04 05:47 cicd/ios/runner/base.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Aug-04 05:47 cicd/ios/runner/xcodebuild/__init__.py
+-rw-r--r--  2.0 unx      291 b- defN 23-Aug-04 05:47 cicd/ios/runner/xcodebuild/archive.py
+-rw-r--r--  2.0 unx      279 b- defN 23-Aug-04 05:47 cicd/ios/runner/xcodebuild/build.py
+-rw-r--r--  2.0 unx      623 b- defN 23-Aug-04 05:47 cicd/ios/runner/xcodebuild/test.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Aug-04 05:47 cicd/ios/simulator/__init__.py
+-rw-r--r--  2.0 unx     5181 b- defN 23-Aug-04 05:47 cicd/ios/simulator/simulator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 05:47 cicd/ios/syntax/__init__.py
+-rw-r--r--  2.0 unx     4600 b- defN 23-Aug-04 05:47 cicd/ios/syntax/xcresult.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 05:47 cicd/providers/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 05:47 cicd/providers/github/__init__.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Aug-04 05:47 cicd/providers/github/client.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Aug-04 05:47 cicd/providers/github/env.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 05:47 cicd/providers/gitlab/__init__.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Aug-04 05:47 cicd/providers/gitlab/client.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Aug-04 05:47 cicd/providers/gitlab/env.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-Aug-04 05:48 seeeye-0.0.4rc5758889904.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3116 b- defN 23-Aug-04 05:48 seeeye-0.0.4rc5758889904.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 05:48 seeeye-0.0.4rc5758889904.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 23-Aug-04 05:48 seeeye-0.0.4rc5758889904.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-04 05:48 seeeye-0.0.4rc5758889904.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6673 b- defN 23-Aug-04 05:48 seeeye-0.0.4rc5758889904.dist-info/RECORD
+80 files, 83920 bytes uncompressed, 32900 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,25 +1,37 @@
 Filename: cicd/cli.py
 Comment: 
 
 Filename: cicd/core/action.py
 Comment: 
 
+Filename: cicd/core/cli.py
+Comment: 
+
 Filename: cicd/core/client.py
 Comment: 
 
 Filename: cicd/core/env.py
 Comment: 
 
 Filename: cicd/core/logger.py
 Comment: 
 
+Filename: cicd/core/typing.py
+Comment: 
+
 Filename: cicd/core/_cli/opts.py
 Comment: 
 
+Filename: cicd/core/cipher/cipher.py
+Comment: 
+
+Filename: cicd/core/cipher/cli.py
+Comment: 
+
 Filename: cicd/core/mixin/core.py
 Comment: 
 
 Filename: cicd/core/mixin/git.py
 Comment: 
 
 Filename: cicd/core/mixin/logger.py
@@ -45,14 +57,17 @@
 
 Filename: cicd/core/provider/models/pr.py
 Comment: 
 
 Filename: cicd/core/provider/models/project.py
 Comment: 
 
+Filename: cicd/core/security/keychain.py
+Comment: 
+
 Filename: cicd/core/syntax/data_represented.py
 Comment: 
 
 Filename: cicd/core/syntax/json.py
 Comment: 
 
 Filename: cicd/core/syntax/yaml.py
@@ -96,14 +111,26 @@
 
 Filename: cicd/ios/actions/xcodebuild/build.py
 Comment: 
 
 Filename: cicd/ios/actions/xcodebuild/test.py
 Comment: 
 
+Filename: cicd/ios/codesign/cert.py
+Comment: 
+
+Filename: cicd/ios/codesign/cli.py
+Comment: 
+
+Filename: cicd/ios/codesign/codesign.py
+Comment: 
+
+Filename: cicd/ios/codesign/profile.py
+Comment: 
+
 Filename: cicd/ios/cov/__init__.py
 Comment: 
 
 Filename: cicd/ios/cov/config.py
 Comment: 
 
 Filename: cicd/ios/cov/cov.py
@@ -189,26 +216,26 @@
 
 Filename: cicd/providers/gitlab/client.py
 Comment: 
 
 Filename: cicd/providers/gitlab/env.py
 Comment: 
 
-Filename: seeeye-0.0.3.dist-info/LICENSE
+Filename: seeeye-0.0.4rc5758889904.dist-info/LICENSE
 Comment: 
 
-Filename: seeeye-0.0.3.dist-info/METADATA
+Filename: seeeye-0.0.4rc5758889904.dist-info/METADATA
 Comment: 
 
-Filename: seeeye-0.0.3.dist-info/WHEEL
+Filename: seeeye-0.0.4rc5758889904.dist-info/WHEEL
 Comment: 
 
-Filename: seeeye-0.0.3.dist-info/entry_points.txt
+Filename: seeeye-0.0.4rc5758889904.dist-info/entry_points.txt
 Comment: 
 
-Filename: seeeye-0.0.3.dist-info/top_level.txt
+Filename: seeeye-0.0.4rc5758889904.dist-info/top_level.txt
 Comment: 
 
-Filename: seeeye-0.0.3.dist-info/RECORD
+Filename: seeeye-0.0.4rc5758889904.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cicd/cli.py

```diff
@@ -1,15 +1,17 @@
 import click
 
+from cicd.core.cli import main as core
 from cicd.ios.cli import main as ios
 
 
 @click.group()
 def main():
     pass
 
 
+main.add_command(core, name='core')
 main.add_command(ios, name='ios')
 
 
 if __name__ == '__main__':
     main()
```

## cicd/core/_cli/opts.py

```diff
@@ -8,8 +8,8 @@
     def use(self, *keys):
         def decorator(func):
             return reduce(lambda f, key: self.get(key)(f), keys, func)
 
         return decorator
 
     def use_all(self):
-        return self.uses(*self.keys())
+        return self.use(*self.keys())
```

## cicd/core/utils/file.py

```diff
@@ -1,15 +1,14 @@
 import os
 import shutil
 import tempfile
-import typing as t
 from contextlib import contextmanager
 from pathlib import Path
 
-StrPath = t.Union[str, Path]
+from cicd.core.typing import StrPath
 
 
 class FileUtils:
     @contextmanager
     @staticmethod
     def tempdir() -> Path:
         dir = tempfile.mkdtemp()
```

## cicd/ios/cli.py

```diff
@@ -1,10 +1,11 @@
 import click
 
 from cicd.core._cli.opts import Opts
+from cicd.ios.codesign.cli import main as codesign
 from cicd.ios.mixin.mono import MonoMixin as Mixin
 
 opts = Opts(
     workspace=click.option('--workspace', type=str, help='Path to the xcworkspace'),
     scheme=click.option('--scheme', type=str, help='Scheme'),
     project=click.option('--project', type=str, help='Path to the xcodeproj'),
     target=click.option('--target', type=str, help='Target'),
@@ -102,9 +103,12 @@
 @click.option('--config', help='Path to config file (default: .cov.yml)')
 @click.option('--export', help='Path to export cov json data')
 @opts.use('timeout', 'derived_data_path')
 def cov(**kwargs):
     Mixin(**kwargs).start_parsing_cov()
 
 
+main.add_command(codesign, name='codesign')
+
+
 if __name__ == '__main__':
     main()
```

## cicd/ios/actions/base.py

```diff
@@ -37,43 +37,43 @@
         before = find_paths() if new_only else []
         try:
             yield
         finally:
             after = find_paths()
             paths = list(set(after).difference(before))
             if len(paths) == 0:
-                raise RuntimeError(
+                self.logger.warning(
                     f'Cannot detect any {name} matching: {base_path / pattern}'
                 )
             elif len(paths) > 1:
                 self.logger.warning(f'Detected more than one {name}: {paths}')
             else:
                 self.logger.info(f'Detected {name}: {paths}')
             on_detected(paths)
 
     @contextmanager
     def collect_xcresults(self, new_only=True) -> XCResult:
         '''Collect the xcresults generated after an action.'''
 
         def save(paths):
-            self.xcresult = XCResult(paths[0])
+            self.xcresult = XCResult(paths[0]) if paths else None
 
         with self.collect_artifacts(
             name='xcresult',
             base_path=self.derived_data_path,
             pattern='Logs/Test/*.xcresult',
             on_detected=save,
             new_only=new_only,
         ):
             yield
 
     @contextmanager
-    def collect_xcarchives(self, new_only=True) -> t.List[Path]:
+    def collect_xcarchives(self) -> t.List[Path]:
         def save(paths):
-            self.xcarchive_path = paths[0]
+            self.xcarchive_path = paths[0] if paths else None
 
         with self.collect_artifacts(
             name='xcarchive',
             base_path=self.archive_path,
             pattern='**/*.xcarchive',
             on_detected=save,
         ):
```

## Comparing `seeeye-0.0.3.dist-info/LICENSE` & `seeeye-0.0.4rc5758889904.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `seeeye-0.0.3.dist-info/METADATA` & `seeeye-0.0.4rc5758889904.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeeye
-Version: 0.0.3
+Version: 0.0.4rc5758889904
 Summary: CI/CD toolkits for mobile apps
 Author-email: Thuyen Trinh <trinhngocthuyen@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/trinhngocthuyen/seeeye
 Keywords: ci,cd,ci/cd,mobile,ios
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -18,14 +18,15 @@
 Requires-Dist: colorlog
 Requires-Dist: retry
 Requires-Dist: PyYAML
 Requires-Dist: click
 Requires-Dist: GitPython
 Requires-Dist: requests
 Requires-Dist: pydantic
+Requires-Dist: cryptography
 Provides-Extra: dev
 Requires-Dist: setuptools (>=61.0.0) ; extra == 'dev'
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: autoflake ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
@@ -35,15 +36,15 @@
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
 
 seeeye (CI/CD toolkits for mobile apps)
 =======================================
 
 .. _readthedocs: https://seeeye.readthedocs.io/
-.. _contributing guidelines: https://seeeye.readthedocs.io/en/latest/contributing.html
+.. _contributing guidelines: /contributing.html
 .. _fastlane: https://fastlane.tools
 
 .. image:: https://github.com/trinhngocthuyen/seeeye/workflows/test/badge.svg
     :target: https://github.com/trinhngocthuyen/seeeye/actions/workflows/test.yml
 
 .. image:: https://img.shields.io/pypi/v/seeeye.svg
     :target: https://pypi.org/project/seeeye
@@ -52,33 +53,39 @@
     :target: https://codecov.io/gh/trinhngocthuyen/seeeye
 
 .. image:: https://img.shields.io/pypi/l/seeeye.svg
     :target: https://github.com/trinhngocthuyen/seeeye/blob/main/LICENSE
 
 ``seeeye`` is a Python package providing various CI/CD toolkits for mobile projects, especially iOS projects. While many iOS projects favor fastlane_, this package attempts to brings convenient usages to projects where Python is the favorable choice for scripting.
 
+.. image:: _static/cli.gif
+
 Installation
 ------------
 
 ``seeeye`` is `available on PyPI (Python Package Index)
 <https://pypi.org/project/seeeye>`_. You can install with with ``pip``:
 
 .. code-block:: console
 
    $ pip install --upgrade seeeye
 
 Usage
 -----
 
-Kindly check out the related docs on readthedocs_.
+Kindly check out the related docs on readthedocs_:
+
+- `Usage <https://seeeye.readthedocs.io/en/latest/usage.html>`_
 
 Documentation
 -------------
 
-Kindly check out the related docs on readthedocs_.
+Kindly check out the related docs on readthedocs_:
+
+- `API Reference <https://seeeye.readthedocs.io/en/latest/api/reference.html>`_
 
 .. Supported CI/CD Providers
 .. -------------------------
 
 .. - [x] Github Actions
 .. - [ ] CircleCI (planning)
 .. - [ ] Gitlab CI/CD (planning)
```

## Comparing `seeeye-0.0.3.dist-info/RECORD` & `seeeye-0.0.4rc5758889904.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-cicd/cli.py,sha256=0fjlMdwR2DZ1OgvsJFvoyHv5T002KDDtnhcSq0-mqZA,165
+cicd/cli.py,sha256=ihutniadJLB4LFiazrKv8w9vi0yFODHJ8r3DsIuYZoU,240
 cicd/core/action.py,sha256=XeqZCDSZdcDsdZ2OwiiceoDrzqs5X_b9XdftyksIT3Y,174
+cicd/core/cli.py,sha256=RFKbVGHG8eE3fmSl0nM0mjnDPUNbrW5Y7JLJyAY6DC8,182
 cicd/core/client.py,sha256=PznhG9LAlpXJ3g9ekdDoaYL0rOpZPAk0RVwBosBwqnA,3100
 cicd/core/env.py,sha256=r2u3vcAb_M2eiwDNXCgk-vWojfqqezM0J8-94_4HUL4,131
 cicd/core/logger.py,sha256=ldpHJEMlOdTd3KdOW8szewaNt1u6DEjNcerOay3_5t4,1071
-cicd/core/_cli/opts.py,sha256=rcLrpeopmU95fFDnNIWLg59BBgyq74-8HJa-mymqblU,333
+cicd/core/typing.py,sha256=aASoMXuNCAb-r_FKk5-DnoCcZuPQKHZoaADGlG-QCIo,74
+cicd/core/_cli/opts.py,sha256=SAH5QaHu5ydLzR9OeuX-OAcWPzPAQGDShiEIPL05_Jg,332
+cicd/core/cipher/cipher.py,sha256=RSPkRM6eD1mZjsxaKbXI_yOqvpba1kv_HqOu7tJRBeI,2605
+cicd/core/cipher/cli.py,sha256=MDQzItBvlSIvDTI3akteQC3e08SLEf7oMqreJv7wSMc,839
 cicd/core/mixin/core.py,sha256=LSNMmW3YGsqehkw-zuhqwjziOczsqnA6Wk4JfvbIZMY,163
 cicd/core/mixin/git.py,sha256=3EdZJDDXZH2hYjXJj65awwcqErOWzWAPLupQ4Va8_aM,282
 cicd/core/mixin/logger.py,sha256=ZRtjnP_gxSvsq9NAAjgZr8TCufOvCXJLO0Yhy_ArcZQ,115
 cicd/core/mixin/provider.py,sha256=7IMIVB2qgjAmg58kp5RJRWIQX5rCU4ejc16QYcMrY94,1552
 cicd/core/mixin/step.py,sha256=IgLhTgPG4fP7gQXa6gXq8MRfp-iQu7KIS0AJ0ADm7NM,261
 cicd/core/provider/client.py,sha256=yGv2CZM0AQGmzLh3jWt0tGLZYayoW-2bGYlhlPwAmdw,1237
 cicd/core/provider/info.py,sha256=OFMG2VmpLnf7BLjtReubiwPiz62GA0_X478RZZ4G10U,1261
 cicd/core/provider/models/api.py,sha256=BZbjb_f6FeWlJn96DoN32exkVls73jeXgtdmD1K6i1Q,406
 cicd/core/provider/models/base.py,sha256=ViBnjKvXC1yMq3rhGwZoUFZ71F7-6AVN4UnMtr_9T7c,1878
 cicd/core/provider/models/pr.py,sha256=d_-2EezDN4zUQHUOEwAu2i1SyrFK6iLf7rMOH3mE0Gw,158
 cicd/core/provider/models/project.py,sha256=t-M-75onuYW8FVDHlqh8-HouWBy7d6M7J09kewIET5A,982
+cicd/core/security/keychain.py,sha256=SF0hQNwV9z-BTfRUHTnb2xU8ox89VzyZ5mMMUg1tksQ,1848
 cicd/core/syntax/data_represented.py,sha256=ZxVUffqNaWW4lYNZvoNMj5F3HTr0XeuOIbg2nwcTWrE,1929
 cicd/core/syntax/json.py,sha256=w4JcdxFFXf2GhQOHhZSBI7cM_QIDMhaueSLrpGPtejU,563
 cicd/core/syntax/yaml.py,sha256=XXra6E7hHdnri-y470kp3DQ7BTT6iXz5m0a0UES76ZA,253
 cicd/core/utils/cli_group.py,sha256=fPwV3Ry4ni49P5f_eph-_roX-KJh0DodrdwZ0_RMEYo,827
-cicd/core/utils/file.py,sha256=mA8OLqAolOHdp_AbIRecqqHDeHbh4IHdqoW_cbi8LrI,534
+cicd/core/utils/file.py,sha256=Oum6emk-NpUJHaIEMfH4yYY2hcn4lmoDguUp645HWSM,523
 cicd/core/utils/sh.py,sha256=GdeTxGmHnE6U24_AiZPHmJkuoJ7_VWQYMg52XZSrfak,1708
 cicd/core/utils/step.py,sha256=em3xuJLvkZJf1T9muYpkvcm2QnxPWNGajRjSZ92w3yY,369
 cicd/core/utils/timeout.py,sha256=OX4Cd6BedrAC8eHuM4wyBlYgnXYgtZTU7nTax6lpifo,970
-cicd/ios/cli.py,sha256=r0PuM9Pos34RwQD-OZXj5Hpkbu2HPC5IQG6X2nBiqJI,3352
-cicd/ios/actions/base.py,sha256=KLux4boKXXq_LUItu47IXHGpQhBUb7FOBGPLRewL8EU,2482
+cicd/ios/cli.py,sha256=LfJM56OCdlKL-nqZQp15tD75HrP-LpB2o8fwlhXVIUs,3449
+cicd/ios/actions/base.py,sha256=z1CiddeKXsNIfMKqxcQaIriuGdGR8X45H0MLHOVEW_w,2506
 cicd/ios/actions/cov.py,sha256=3iPTg0Q17o8XRoNd3e_qw2E7L_EkjTR3l_VQncjRwOo,690
 cicd/ios/actions/test_extraction.py,sha256=YuYhVrCDxD7PHY9GKp3mInLP5-5pf03Y4jaGK3dLLIU,1170
 cicd/ios/actions/xcodebuild/__init__.py,sha256=8R3lS89ufp3xSOvEafgApMLdd3_jU2Ays43VjX702mI,84
 cicd/ios/actions/xcodebuild/archive.py,sha256=6mc48ds277X_v9zw5HIuGJsY6jYa9KF5Rlce8WWP7bQ,3413
 cicd/ios/actions/xcodebuild/base.py,sha256=ikZ3PYgAASoZC2oHR8o7ngQ7XSLlKNnqo-3XDfUM6Qs,5150
 cicd/ios/actions/xcodebuild/build.py,sha256=D5G9Wg2JELzgLs9x9ktaaNitPQ-Z_QMAC0g5RLeIXb4,583
 cicd/ios/actions/xcodebuild/test.py,sha256=qwW73vYxEzHBNZtvSGjEmjxauxrA85APnIlwjPRBbyQ,1102
+cicd/ios/codesign/cert.py,sha256=xAt5ofIPfIBNCbFXuOWrPynkmj4qGABeXPgO_uGhrkU,520
+cicd/ios/codesign/cli.py,sha256=gnfpU8Evc6OKVzn5dR4PVTrKNtUBSzGB9dLKtZa1lDk,1057
+cicd/ios/codesign/codesign.py,sha256=a7LDo_sa-oN59i4ci0r6QdAjye_RbRILrMbo2MHWV0Q,1915
+cicd/ios/codesign/profile.py,sha256=XwJiEBldB9q7EYTjnESEWW83YgsszEjqlh_NOW7H3x4,551
 cicd/ios/cov/__init__.py,sha256=V73S1UnY2lzUJitrRRLF3a4lhb0igeVFASBgh_QlCKs,63
 cicd/ios/cov/config.py,sha256=S8i9exRBS39LVVjxKYYCUiN3sNUKywv3FwkBtL3WsNA,378
 cicd/ios/cov/cov.py,sha256=grPe6FXhBvguAIk9E25xyl7t9O-g-KxZZ5mNHbwA0K0,767
 cicd/ios/cov/report.py,sha256=K5UvOngLDYZXH8J_8SnAx1vRez6_gVbE_Ef7L1JVizg,2273
 cicd/ios/mixin/archive.py,sha256=uqf1EQ1kQI7RVFs1nklD3xo0E9KAiRxIZ2LNt6wE-bQ,449
 cicd/ios/mixin/base_ios.py,sha256=chc8YCy36Y6EzjznbnJPedpHPjkKASmZacR1_AlK5OQ,627
 cicd/ios/mixin/build.py,sha256=wbCzckqLVS5OcuYEXTEdlr8N8_pLQEHje0oWj26IZn4,389
@@ -59,13 +68,13 @@
 cicd/providers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cicd/providers/github/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cicd/providers/github/client.py,sha256=uhfzAn8LFYqlfXxVzwOMcj_XnEM8RaTgr1E9sndK6YI,929
 cicd/providers/github/env.py,sha256=6d0JqBare1z_hILN-RG3fhEaD1QQ2udcp3nI1mZc5oM,63
 cicd/providers/gitlab/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cicd/providers/gitlab/client.py,sha256=VFM96sLw-QIB50h6k_swV1GMftv-IgXMUqbUeyCvv78,134
 cicd/providers/gitlab/env.py,sha256=8oTranPx1OS5skABEHkuBVmtLfjYP5radk1SpTWFODc,63
-seeeye-0.0.3.dist-info/LICENSE,sha256=kVdhDldPTgkI0N-t0mNlqix21PXulpLy6pT71bkscTQ,1092
-seeeye-0.0.3.dist-info/METADATA,sha256=9UvlhB0H96JTczrUSCgweKddFSlwAAPROITDhN8U_nE,2941
-seeeye-0.0.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-seeeye-0.0.3.dist-info/entry_points.txt,sha256=AvnV-B3vp5CsY752DIbcr0s22d3VA3XHzdZHT5WcniQ,39
-seeeye-0.0.3.dist-info/top_level.txt,sha256=JqUP3rOzYUVQV4g4zKPF7kt3EoB7tiVgcWDINQmDIW4,5
-seeeye-0.0.3.dist-info/RECORD,,
+seeeye-0.0.4rc5758889904.dist-info/LICENSE,sha256=kVdhDldPTgkI0N-t0mNlqix21PXulpLy6pT71bkscTQ,1092
+seeeye-0.0.4rc5758889904.dist-info/METADATA,sha256=JAj1dnDvcRuVbnS2yTzELnNl45VpZEsx8X1-YJrszIQ,3116
+seeeye-0.0.4rc5758889904.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+seeeye-0.0.4rc5758889904.dist-info/entry_points.txt,sha256=AvnV-B3vp5CsY752DIbcr0s22d3VA3XHzdZHT5WcniQ,39
+seeeye-0.0.4rc5758889904.dist-info/top_level.txt,sha256=JqUP3rOzYUVQV4g4zKPF7kt3EoB7tiVgcWDINQmDIW4,5
+seeeye-0.0.4rc5758889904.dist-info/RECORD,,
```

