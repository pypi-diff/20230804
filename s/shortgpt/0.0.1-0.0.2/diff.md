# Comparing `tmp/ShortGPT-0.0.1.tar.gz` & `tmp/shortgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShortGPT-0.0.1.tar", last modified: Tue Jul 11 17:37:07 2023, max compression
+gzip compressed data, was "shortgpt-0.0.2.tar", last modified: Fri Aug  4 07:45:45 2023, max compression
```

## Comparing `ShortGPT-0.0.1.tar` & `shortgpt-0.0.2.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:06.970000 ShortGPT-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-07-11 17:14:50.000000 ShortGPT-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     9545 2023-07-11 17:37:08.000000 ShortGPT-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8723 2023-07-11 17:14:50.000000 ShortGPT-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.030000 ShortGPT-0.0.1/ShortGPT.egg-info/
--rw-rw-rw-   0        0        0     9545 2023-07-11 17:37:08.000000 ShortGPT-0.0.1/ShortGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1495 2023-07-11 17:37:08.000000 ShortGPT-0.0.1/ShortGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:37:08.000000 ShortGPT-0.0.1/ShortGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2023-07-11 17:37:08.000000 ShortGPT-0.0.1/ShortGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 17:37:08.000000 ShortGPT-0.0.1/ShortGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:37:08.000000 ShortGPT-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1629 2023-07-11 17:36:36.000000 ShortGPT-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.050000 ShortGPT-0.0.1/shortGPT/
--rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 ShortGPT-0.0.1/shortGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.080000 ShortGPT-0.0.1/shortGPT/api_utils/
--rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 ShortGPT-0.0.1/shortGPT/api_utils/__init__.py
--rw-rw-rw-   0        0        0     1969 2023-07-05 21:00:14.000000 ShortGPT-0.0.1/shortGPT/api_utils/eleven_api.py
--rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 ShortGPT-0.0.1/shortGPT/api_utils/image_api.py
--rw-rw-rw-   0        0        0     2211 2023-07-08 06:01:18.000000 ShortGPT-0.0.1/shortGPT/api_utils/pexels_api.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.110000 ShortGPT-0.0.1/shortGPT/audio/
--rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 ShortGPT-0.0.1/shortGPT/audio/__init__.py
--rw-rw-rw-   0        0        0     3292 2023-06-18 23:27:10.000000 ShortGPT-0.0.1/shortGPT/audio/audio_duration.py
--rw-rw-rw-   0        0        0     2546 2023-07-06 06:14:00.000000 ShortGPT-0.0.1/shortGPT/audio/audio_utils.py
--rw-rw-rw-   0        0        0     1348 2023-07-08 23:34:28.000000 ShortGPT-0.0.1/shortGPT/audio/eleven_voice_module.py
--rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 ShortGPT-0.0.1/shortGPT/audio/voice_module.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.150000 ShortGPT-0.0.1/shortGPT/config/
--rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 ShortGPT-0.0.1/shortGPT/config/__init__.py
--rw-rw-rw-   0        0        0      342 2023-07-05 03:24:20.000000 ShortGPT-0.0.1/shortGPT/config/api_db.py
--rw-rw-rw-   0        0        0     9501 2023-07-07 19:46:56.000000 ShortGPT-0.0.1/shortGPT/config/asset_db.py
--rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 ShortGPT-0.0.1/shortGPT/config/config.py
--rw-rw-rw-   0        0        0      242 2023-07-09 16:18:06.000000 ShortGPT-0.0.1/shortGPT/config/languages.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.170000 ShortGPT-0.0.1/shortGPT/database/
--rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 ShortGPT-0.0.1/shortGPT/database/__init__.py
--rw-rw-rw-   0        0        0      765 2023-07-02 23:41:12.000000 ShortGPT-0.0.1/shortGPT/database/content_data_manager.py
--rw-rw-rw-   0        0        0     1167 2023-07-03 05:23:16.000000 ShortGPT-0.0.1/shortGPT/database/content_database.py
--rw-rw-rw-   0        0        0     3347 2023-07-05 03:21:50.000000 ShortGPT-0.0.1/shortGPT/database/db_document.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.190000 ShortGPT-0.0.1/shortGPT/editing_utils/
--rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 ShortGPT-0.0.1/shortGPT/editing_utils/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-07-02 01:39:04.000000 ShortGPT-0.0.1/shortGPT/editing_utils/captions.py
--rw-rw-rw-   0        0        0      781 2023-06-25 18:15:36.000000 ShortGPT-0.0.1/shortGPT/editing_utils/editing_images.py
--rw-rw-rw-   0        0        0     2889 2023-07-02 23:52:42.000000 ShortGPT-0.0.1/shortGPT/editing_utils/handle_videos.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.220000 ShortGPT-0.0.1/shortGPT/engine/
--rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 ShortGPT-0.0.1/shortGPT/engine/__init__.py
--rw-rw-rw-   0        0        0     3341 2023-07-09 16:16:18.000000 ShortGPT-0.0.1/shortGPT/engine/abstract_content_engine.py
--rw-rw-rw-   0        0        0     8490 2023-07-11 17:10:48.000000 ShortGPT-0.0.1/shortGPT/engine/content_short_engine.py
--rw-rw-rw-   0        0        0     7711 2023-07-11 06:00:16.000000 ShortGPT-0.0.1/shortGPT/engine/content_video_engine.py
--rw-rw-rw-   0        0        0      919 2023-07-09 16:16:54.000000 ShortGPT-0.0.1/shortGPT/engine/facts_short_engine.py
--rw-rw-rw-   0        0        0     5759 2023-07-11 06:00:16.000000 ShortGPT-0.0.1/shortGPT/engine/reddit_short_engine.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.240000 ShortGPT-0.0.1/shortGPT/gpt/
--rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 ShortGPT-0.0.1/shortGPT/gpt/__init__.py
--rw-rw-rw-   0        0        0      921 2023-07-10 23:09:28.000000 ShortGPT-0.0.1/shortGPT/gpt/facts_gpt.py
--rw-rw-rw-   0        0        0     1275 2023-07-10 23:09:14.000000 ShortGPT-0.0.1/shortGPT/gpt/gpt_chat_video.py
--rw-rw-rw-   0        0        0     1788 2023-07-10 23:09:24.000000 ShortGPT-0.0.1/shortGPT/gpt/gpt_editing.py
--rw-rw-rw-   0        0        0      386 2023-07-10 23:08:12.000000 ShortGPT-0.0.1/shortGPT/gpt/gpt_translate.py
--rw-rw-rw-   0        0        0     3398 2023-07-11 00:39:42.000000 ShortGPT-0.0.1/shortGPT/gpt/gpt_utils.py
--rw-rw-rw-   0        0        0      389 2023-07-10 23:35:14.000000 ShortGPT-0.0.1/shortGPT/gpt/gpt_voice.py
--rw-rw-rw-   0        0        0      822 2023-07-10 23:09:42.000000 ShortGPT-0.0.1/shortGPT/gpt/gpt_yt.py
--rw-rw-rw-   0        0        0     2255 2023-07-11 00:44:32.000000 ShortGPT-0.0.1/shortGPT/gpt/reddit_gpt.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:37:07.260000 ShortGPT-0.0.1/shortGPT/tracking/
--rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 ShortGPT-0.0.1/shortGPT/tracking/__init__.py
--rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 ShortGPT-0.0.1/shortGPT/tracking/api_tracking.py
--rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 ShortGPT-0.0.1/shortGPT/tracking/cost_analytics.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.790000 shortgpt-0.0.2/
+-rw-rw-rw-   0        0        0     2446 2023-07-28 20:38:40.000000 shortgpt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    11354 2023-08-04 07:45:46.000000 shortgpt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10523 2023-08-04 05:22:42.000000 shortgpt-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:45:46.000000 shortgpt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1680 2023-08-04 07:38:44.000000 shortgpt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.820000 shortgpt-0.0.2/shortGPT/
+-rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 shortgpt-0.0.2/shortGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.850000 shortgpt-0.0.2/shortGPT/api_utils/
+-rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 shortgpt-0.0.2/shortGPT/api_utils/__init__.py
+-rw-rw-rw-   0        0        0     2150 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/api_utils/eleven_api.py
+-rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 shortgpt-0.0.2/shortGPT/api_utils/image_api.py
+-rw-rw-rw-   0        0        0     2231 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/api_utils/pexels_api.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.870000 shortgpt-0.0.2/shortGPT/audio/
+-rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 shortgpt-0.0.2/shortGPT/audio/__init__.py
+-rw-rw-rw-   0        0        0     2684 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/audio/audio_duration.py
+-rw-rw-rw-   0        0        0     3515 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/audio/audio_utils.py
+-rw-rw-rw-   0        0        0     1874 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/audio/edge_voice_module.py
+-rw-rw-rw-   0        0        0     1490 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/audio/eleven_voice_module.py
+-rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 shortgpt-0.0.2/shortGPT/audio/voice_module.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.880000 shortgpt-0.0.2/shortGPT/config/
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 shortgpt-0.0.2/shortGPT/config/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/config/api_db.py
+-rw-rw-rw-   0        0        0    11301 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/config/asset_db.py
+-rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 shortgpt-0.0.2/shortGPT/config/config.py
+-rw-rw-rw-   0        0        0    11200 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/config/languages.py
+-rw-rw-rw-   0        0        0     1144 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/config/path_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.900000 shortgpt-0.0.2/shortGPT/database/
+-rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.0.2/shortGPT/database/__init__.py
+-rw-rw-rw-   0        0        0      784 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/database/content_data_manager.py
+-rw-rw-rw-   0        0        0     1167 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/database/content_database.py
+-rw-rw-rw-   0        0        0     3914 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/database/db_document.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.920000 shortgpt-0.0.2/shortGPT/editing_utils/
+-rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 shortgpt-0.0.2/shortGPT/editing_utils/__init__.py
+-rw-rw-rw-   0        0        0     2455 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/editing_utils/captions.py
+-rw-rw-rw-   0        0        0      781 2023-07-11 20:20:28.000000 shortgpt-0.0.2/shortGPT/editing_utils/editing_images.py
+-rw-rw-rw-   0        0        0     3423 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/editing_utils/handle_videos.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.940000 shortgpt-0.0.2/shortGPT/engine/
+-rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 shortgpt-0.0.2/shortGPT/engine/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/engine/abstract_content_engine.py
+-rw-rw-rw-   0        0        0     8322 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/engine/content_short_engine.py
+-rw-rw-rw-   0        0        0     7831 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/engine/content_translation_engine.py
+-rw-rw-rw-   0        0        0     7801 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/engine/content_video_engine.py
+-rw-rw-rw-   0        0        0     1023 2023-07-29 19:03:56.000000 shortgpt-0.0.2/shortGPT/engine/facts_short_engine.py
+-rw-rw-rw-   0        0        0     8283 2023-07-31 18:40:34.000000 shortgpt-0.0.2/shortGPT/engine/multi_language_translation_engine.py
+-rw-rw-rw-   0        0        0     5730 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/engine/reddit_short_engine.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.960000 shortgpt-0.0.2/shortGPT/gpt/
+-rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 shortgpt-0.0.2/shortGPT/gpt/__init__.py
+-rw-rw-rw-   0        0        0      921 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/facts_gpt.py
+-rw-rw-rw-   0        0        0     1275 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/gpt_chat_video.py
+-rw-rw-rw-   0        0        0     1788 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/gpt_editing.py
+-rw-rw-rw-   0        0        0      516 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/gpt_translate.py
+-rw-rw-rw-   0        0        0     3502 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/gpt_utils.py
+-rw-rw-rw-   0        0        0      389 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/gpt_voice.py
+-rw-rw-rw-   0        0        0      806 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/gpt_yt.py
+-rw-rw-rw-   0        0        0     2255 2023-07-28 20:38:42.000000 shortgpt-0.0.2/shortGPT/gpt/reddit_gpt.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:44.980000 shortgpt-0.0.2/shortGPT/tracking/
+-rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 shortgpt-0.0.2/shortGPT/tracking/__init__.py
+-rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 shortgpt-0.0.2/shortGPT/tracking/api_tracking.py
+-rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 shortgpt-0.0.2/shortGPT/tracking/cost_analytics.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:45:45.000000 shortgpt-0.0.2/shortgpt.egg-info/
+-rw-rw-rw-   0        0        0    11354 2023-08-04 07:45:46.000000 shortgpt-0.0.2/shortgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2023-08-04 07:45:46.000000 shortgpt-0.0.2/shortgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:45:46.000000 shortgpt-0.0.2/shortgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      199 2023-08-04 07:45:46.000000 shortgpt-0.0.2/shortgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-04 07:45:46.000000 shortgpt-0.0.2/shortgpt.egg-info/top_level.txt
```

### Comparing `ShortGPT-0.0.1/PKG-INFO` & `shortgpt-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,150 +1,159 @@
 Metadata-Version: 2.1
-Name: ShortGPT
-Version: 0.0.1
+Name: shortgpt
+Version: 0.0.2
 Summary: Automating video and short content creation with AI
 Author: RayVentura
 Author-email: 
 Keywords: python,video,content creation,AI,automation,editing,voiceover synthesis,video captions,asset sourcing,tinyDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-
-# 🎬🚀 ShortGPT
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+# 🚀🎬 ShortGPT
 [![](https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R)
+[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ)
 [![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/shortgpt)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ) 
 <div align="center">
-    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/d9f87cf2-021d-4b8d-bb86-b3a7af1d80d4" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
+    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
 </div>
-
 <div align="center">
   <a href="https://discord.gg/uERx39ru3R">
     <img src="https://img.shields.io/badge/discord-join%20chat-blue.svg" alt="Join our Discord" height="34">
   </a>
 </div>
 
+<div align="center">
 ⚡ Automating video and short content creation with AI ⚡
+</div>
+
+## 🎥 Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U))
+
+https://github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-6365c27ea5fe
+## 🎥 Voice Dubbing
+
+
+https://github.com/RayVentura/ShortGPT/assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef
 
+## 🌟 Show Your Support
+We hope you find ShortGPT helpful! If you do, let us know by giving us a star ⭐ on the repo. It's easy, just click on the 'Star' button at the top right of the page. Your support means a lot to us and keeps us motivated to improve and expand ShortGPT. Thank you and happy content creating! 🎉 
+
+[![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://github.com/RayVentura/ShortGPT/stargazers)
+## 🛠️ How it works
+![alt text](https://github.com/RayVentura/ShortGPT/assets/121462835/fcee74d4-f856-4481-949f-244558bf3bfa)
 ## 📝 Introduction to ShortGPT 
-ShortGPT is a powerful tool for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
+ShortGPT is a powerful framework for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
 
 - 🎞️ **Automated editing framework**: Streamlines the video creation process with an LLM oriented video editing language.
 
 - 📃 **Scripts and Prompts**: Provides ready-to-use scripts and prompts for various LLM automated editing processes.
 
 - 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, and Portuguese 🇵🇹.
 
 - 🔗 **Caption Generation**: Automates the generation of video captions.
 
 - 🌐🎥 **Asset Sourcing**: Sources images and video footage from the internet, connecting with the web and Pexels API as necessary.
 
 - 🧠 **Memory and persistency**: Ensures long-term persistency of automated editing variables with TinyDB.
 
+## 🚀 Quick Start: Run ShortGPT on Google Colab (https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
-## Showcase
-
+If you prefer not to install the prerequisites on your local system, you can use the Google Colab notebook. This option is free and requires no installation setup.
 
-https://github.com/RayVentura/ShortGPT/assets/121462835/d357ba50-51d7-4c1c-a7ba-72d8353a804d
+1. Click on the link to the Google Colab notebook: [https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
+2. Once you're in the notebook, simply run the cells in order from top to bottom. You can do this by clicking on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy using ShortGPT!
 
 # Instructions for running shortGPT
-
-This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `shortgptUI.py` successfully.
+This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
 
 ## Prerequisites
-
 Before you begin, ensure that you have the following prerequisites installed on your system:
 - Python 3.x
 - Pip (Python package installer)
 
 ## Installation Steps
-
 Follow the instructions below to install ImageMagick, FFmpeg, and clone the shortGPT repository:
 
 ### Step 1: Install ImageMagick
-
 1. For `Windows` download the installer from the official ImageMagick website and follow the installation instructions.
       
       [https://imagemagick.org/script/download.php](https://imagemagick.org/script/download.php)
-      
-     
+          
 2. For Ubuntu/Debian-based systems, use the command:
      ```
      sudo apt-get install imagemagick
-     ```   
-    For macOS using Homebrew, use the command:
+     ```
+     Then run the following command to fix a moviepy Imagemagick policy.xml incompatibility problem:
+     ```
+     !sed -i '/<policy domain="path" rights="none" pattern="@\*"/d' /etc/ImageMagick-6/policy.xml
+     ```    
+4. For macOS using Homebrew, use the command:
      ```
      brew install imagemagick
      ```
-
 2. Verify the installation by running the following command:
    ```
    convert --version
    ```
-
    You should see the ImageMagick version information if the installation was successful.
 
-### Step 2: Install FFmpeg
-
-1. For `Windows`Download the FFmpeg binaries from the official website and add the executable to your system's PATH. 
+### Step 2: Install FFmpeg (REQUIRED FOR SHORTGPT TO WORK)
+1. For `Windows`Download the FFmpeg binaries from this Windows Installer (It will download ffmpeg, ffprobe and add it to your path).
       
-      [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)
+      [https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306)
       
 2. For macOS using Homebrew, use the command:
      ```
      brew install ffmpeg
      ```   
     For Ubuntu/Debian-based systems, use the command:
      ```
      sudo apt-get install ffmpeg
      ```
 2. Verify the installation by running the following command:
    ```
    ffmpeg -version
    ```
-
    You should see the FFmpeg version information if the installation was successful.
 
 ### Step 3: Clone the shortGPT Repository
 
 1. Open a terminal or command prompt.
 2. Execute the following command to clone the shortGPT repository:
    ```
    git clone https://github.com/rayventura/shortgpt.git
    ```
 
 ### Step 4: Install Python Dependencies
 
 1. Open a terminal or command prompt.
-2. Navigate to the directory where `shortgpt.py` is located (the cloned repo).
+2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to install the required Python dependencies:
    ```
    pip install -r requirements.txt
    ```
 
    This command will install the necessary packages specified in the `requirements.txt` file.
 
-## Running shortgptUI.py Web Interface
+## Running runShortGPT.py Web Interface
 
-Once you have successfully installed ImageMagick, FFmpeg, and the Python dependencies, you can run `shortgpt.py` by following these steps:
+Once you have successfully installed ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py` by following these steps:
 
 1. Open a terminal or command prompt.
-2. Navigate to the directory where `shortgptUI.py` is located (the cloned repo).
+2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to run the script:
    ```
-   python shortgptUI.py
+   python runShortGPT.py
    ```
 4. After running the script, a Gradio interface should open at your local host on port 31415 (http://localhost:31415). 
 
 ## Putting API Keys
 The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for running short automations. For video automations, you will also need to add a Pexels API.
 
 Follow these steps to add your OpenAI and ElevenLabs API keys:
@@ -152,32 +161,29 @@
 1. Open [http://localhost:31415/?__theme=light](http://localhost:31415/?__theme=light) from a web browser. 
 2. Click on the `config` tab located at the left side bar of the user interface.
 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the corresponding input fields.
 4. Click `Save` to save your API keys.
 
 That's it! You have successfully set up your API keys and can now utilize the functionality of ShortGPT in the Gradio interface.
 
-## 💁 Contributing
-
-As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
-
 ## Framework overview
 
 - 🎬 The `ContentShortEngine` is designed for creating shorts, handling tasks from script generation to final rendering, including adding YouTube metadata.
 
 - 🎥 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like generating audio, automatically sourcing background video footage, timing captions, and preparing background assets.
   
 - 🎞️ The automated `EditingEngine`, using Editing Markup Language and JSON, breaks down the editing process into manageable and customizable blocks, comprehensible to Large Language Models.
 
 💡 ShortGPT offers customization options to suit your needs, from language selection to watermark addition.
 
 🔧 As a framework, ShortGPT is adaptable and flexible, offering the potential for efficient, creative content creation.
 
 More documentation incomming, please be patient.
 
+
 ## Technologies Used
 
 ShortGPT utilizes the following technologies to power its functionality:
 
 - **Moviepy**: Moviepy is used for video editing, allowing ShortGPT to make video editing and rendering
 
 - **Openai**: Openai is used for automating the entire process, including generating scripts and prompts for LLM automated editing processes.
@@ -186,20 +192,23 @@
 
 - **Pexels**: Pexels is used for sourcing background footage, allowing ShortGPT to connect with the web and access a wide range of images and videos.
 
 - **Bing Image**: Bing Image is used for sourcing images, providing a comprehensive database for ShortGPT to retrieve relevant visuals.
 
 These technologies work together to provide a seamless and efficient experience in automating video and short content creation with AI.
 
+## 💁 Contributing
+
+As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it would be in the form of a new feature, improved infrastructure, or better documentation.
+
 ## 🔗 Get in touch on Twitter 🐦
 
 Keep up with the latest happenings, announcements, and insights about Short-GPT by checking out our Twitter accounts. Spark a conversation with our developer and the AI's own account for fascinating dialogues, latest news about the project, and more.
 
 - **Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ). Deep-dive into behind-the-scenes, project news, and related topics from the person behind ShortGPT.
 
-We're eager to interact with you and listen to your feedback, concepts, and experiences with Auto-GPT. Come on board on Twitter and let's navigate the future of AI as a team! 💡🤖
-
+We're eager to interact with you and listen to your feedback, concepts, and experiences with Short-GPT. Come on board on Twitter and let's navigate the future of AI as a team! 💡🤖
 <p align="center">
-  <a href="https://star-history.com/#ReyVentura/ShortGPT&Date">
+  <a href="https://star-history.com/#RayVentura/ShortGPT&Date">
     <img src="https://api.star-history.com/svg?repos=RayVentura/ShortGPT&type=Date" alt="Star History Chart">
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,88 +1,109 @@
-Metadata-Version: 2.1 Name: ShortGPT Version: 0.0.1 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.0.2 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
-LICENSE # ð¬ð ShortGPT [![License: MIT](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![](https://
-dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://
-discord.gg/uERx39ru3R) [![GitHub star chart](https://img.shields.io/github/
-stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
-shortgpt) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/
+LICENSE # ðð¬ ShortGPT [![](https://dcbadge.vercel.app/api/server/
+uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R) [![Twitter]
+(https://img.shields.io/twitter/url/https/twitter.com/
 rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://
-twitter.com/RayVenturaHQ)
+twitter.com/RayVenturaHQ) [![GitHub star chart](https://img.shields.io/github/
+stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
+shortgpt)
                                 [ShortGPT-logo]
                               [Join_our_Discord]
-â¡ Automating video and short content creation with AI â¡ ## ð
-Introduction to ShortGPT ShortGPT is a powerful tool for automating content
-creation. It simplifies video creation, footage sourcing, voiceover synthesis,
-and editing tasks. - ðï¸ **Automated editing framework**: Streamlines the
-video creation process with an LLM oriented video editing language. - ð
-**Scripts and Prompts**: Provides ready-to-use scripts and prompts for various
-LLM automated editing processes. - ð£ï¸ **Voiceover / Content Creation**:
-Supports multiple languages including English ðºð¸, Spanish ðªð¸,
-Arabic ð¦ðª, French ð«ð·, Polish ðµð±, German ð©ðª, Italian
-ð®ð¹, and Portuguese ðµð¹. - ð **Caption Generation**: Automates the
-generation of video captions. - ðð¥ **Asset Sourcing**: Sources images and
-video footage from the internet, connecting with the web and Pexels API as
-necessary. - ð§  **Memory and persistency**: Ensures long-term persistency of
-automated editing variables with TinyDB. ## Showcase https://github.com/
-RayVentura/ShortGPT/assets/121462835/d357ba50-51d7-4c1c-a7ba-72d8353a804d #
-Instructions for running shortGPT This guide provides step-by-step instructions
-for installing ImageMagick and FFmpeg on your system, which are both required
-to do automated editing. Once installed, you can proceed to run `shortgptUI.py`
-successfully. ## Prerequisites Before you begin, ensure that you have the
-following prerequisites installed on your system: - Python 3.x - Pip (Python
-package installer) ## Installation Steps Follow the instructions below to
-install ImageMagick, FFmpeg, and clone the shortGPT repository: ### Step 1:
-Install ImageMagick 1. For `Windows` download the installer from the official
-ImageMagick website and follow the installation instructions. [https://
-imagemagick.org/script/download.php](https://imagemagick.org/script/
-download.php) 2. For Ubuntu/Debian-based systems, use the command: ``` sudo
-apt-get install imagemagick ``` For macOS using Homebrew, use the command: ```
-brew install imagemagick ``` 2. Verify the installation by running the
-following command: ``` convert --version ``` You should see the ImageMagick
+          â¡ Automating video and short content creation with AI â¡
+## ð¥ Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U)) https:
+//github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-
+6365c27ea5fe ## ð¥ Voice Dubbing https://github.com/RayVentura/ShortGPT/
+assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef ## ð Show Your Support
+We hope you find ShortGPT helpful! If you do, let us know by giving us a star
+â­ on the repo. It's easy, just click on the 'Star' button at the top right of
+the page. Your support means a lot to us and keeps us motivated to improve and
+expand ShortGPT. Thank you and happy content creating! ð [![GitHub star
+chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)]
+(https://github.com/RayVentura/ShortGPT/stargazers) ## ð ï¸ How it works !
+[alt text](https://github.com/RayVentura/ShortGPT/assets/121462835/fcee74d4-
+f856-4481-949f-244558bf3bfa) ## ð Introduction to ShortGPT ShortGPT is a
+powerful framework for automating content creation. It simplifies video
+creation, footage sourcing, voiceover synthesis, and editing tasks. - ðï¸
+**Automated editing framework**: Streamlines the video creation process with an
+LLM oriented video editing language. - ð **Scripts and Prompts**: Provides
+ready-to-use scripts and prompts for various LLM automated editing processes. -
+ð£ï¸ **Voiceover / Content Creation**: Supports multiple languages including
+English ðºð¸, Spanish ðªð¸, Arabic ð¦ðª, French ð«ð·, Polish
+ðµð±, German ð©ðª, Italian ð®ð¹, and Portuguese ðµð¹. - ð
+**Caption Generation**: Automates the generation of video captions. - ðð¥
+**Asset Sourcing**: Sources images and video footage from the internet,
+connecting with the web and Pexels API as necessary. - ð§  **Memory and
+persistency**: Ensures long-term persistency of automated editing variables
+with TinyDB. ## ð Quick Start: Run ShortGPT on Google Colab (https://
+colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
+If you prefer not to install the prerequisites on your local system, you can
+use the Google Colab notebook. This option is free and requires no installation
+setup. 1. Click on the link to the Google Colab notebook: [https://
+colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing]
+(https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) 2. Once you're in the notebook,
+simply run the cells in order from top to bottom. You can do this by clicking
+on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy
+using ShortGPT! # Instructions for running shortGPT This guide provides step-
+by-step instructions for installing ImageMagick and FFmpeg on your system,
+which are both required to do automated editing. Once installed, you can
+proceed to run `runShortGPT.py` successfully. ## Prerequisites Before you
+begin, ensure that you have the following prerequisites installed on your
+system: - Python 3.x - Pip (Python package installer) ## Installation Steps
+Follow the instructions below to install ImageMagick, FFmpeg, and clone the
+shortGPT repository: ### Step 1: Install ImageMagick 1. For `Windows` download
+the installer from the official ImageMagick website and follow the installation
+instructions. [https://imagemagick.org/script/download.php](https://
+imagemagick.org/script/download.php) 2. For Ubuntu/Debian-based systems, use
+the command: ``` sudo apt-get install imagemagick ``` Then run the following
+command to fix a moviepy Imagemagick policy.xml incompatibility problem: ```
+!sed -i '/
+' /etc/ImageMagick-6/policy.xml ``` 4. For macOS using Homebrew, use the
+command: ``` brew install imagemagick ``` 2. Verify the installation by running
+the following command: ``` convert --version ``` You should see the ImageMagick
 version information if the installation was successful. ### Step 2: Install
-FFmpeg 1. For `Windows`Download the FFmpeg binaries from the official website
-and add the executable to your system's PATH. [https://ffmpeg.org/
-download.html](https://ffmpeg.org/download.html) 2. For macOS using Homebrew,
-use the command: ``` brew install ffmpeg ``` For Ubuntu/Debian-based systems,
-use the command: ``` sudo apt-get install ffmpeg ``` 2. Verify the installation
-by running the following command: ``` ffmpeg -version ``` You should see the
-FFmpeg version information if the installation was successful. ### Step 3:
-Clone the shortGPT Repository 1. Open a terminal or command prompt. 2. Execute
-the following command to clone the shortGPT repository: ``` git clone https://
-github.com/rayventura/shortgpt.git ``` ### Step 4: Install Python Dependencies
-1. Open a terminal or command prompt. 2. Navigate to the directory where
-`shortgpt.py` is located (the cloned repo). 3. Execute the following command to
-install the required Python dependencies: ``` pip install -r requirements.txt
-``` This command will install the necessary packages specified in the
-`requirements.txt` file. ## Running shortgptUI.py Web Interface Once you have
-successfully installed ImageMagick, FFmpeg, and the Python dependencies, you
-can run `shortgpt.py` by following these steps: 1. Open a terminal or command
-prompt. 2. Navigate to the directory where `shortgptUI.py` is located (the
-cloned repo). 3. Execute the following command to run the script: ``` python
-shortgptUI.py ``` 4. After running the script, a Gradio interface should open
-at your local host on port 31415 (http://localhost:31415). ## Putting API Keys
-The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for
-running short automations. For video automations, you will also need to add a
-Pexels API. Follow these steps to add your OpenAI and ElevenLabs API keys: 1.
-Open [http://localhost:31415/?__theme=light](http://localhost:31415/
-?__theme=light) from a web browser. 2. Click on the `config` tab located at the
-left side bar of the user interface. 3. Add your `OPENAI API KEY` and
-`ELEVENLABS API KEY` in the corresponding input fields. 4. Click `Save` to save
-your API keys. That's it! You have successfully set up your API keys and can
-now utilize the functionality of ShortGPT in the Gradio interface. ## ð
-Contributing As an open-source project in a rapidly developing field, we are
-extremely open to contributions, whether it be in the form of a new feature,
-improved infrastructure, or better documentation. ## Framework overview - ð¬
+FFmpeg (REQUIRED FOR SHORTGPT TO WORK) 1. For `Windows`Download the FFmpeg
+binaries from this Windows Installer (It will download ffmpeg, ffprobe and add
+it to your path). [https://github.com/icedterminal/ffmpeg-installer/releases/
+tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/
+tag/6.0.0.20230306) 2. For macOS using Homebrew, use the command: ``` brew
+install ffmpeg ``` For Ubuntu/Debian-based systems, use the command: ``` sudo
+apt-get install ffmpeg ``` 2. Verify the installation by running the following
+command: ``` ffmpeg -version ``` You should see the FFmpeg version information
+if the installation was successful. ### Step 3: Clone the shortGPT Repository
+1. Open a terminal or command prompt. 2. Execute the following command to clone
+the shortGPT repository: ``` git clone https://github.com/rayventura/
+shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a terminal or
+command prompt. 2. Navigate to the directory where `runShortGPT.py` is located
+(the cloned repo). 3. Execute the following command to install the required
+Python dependencies: ``` pip install -r requirements.txt ``` This command will
+install the necessary packages specified in the `requirements.txt` file. ##
+Running runShortGPT.py Web Interface Once you have successfully installed
+ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py`
+by following these steps: 1. Open a terminal or command prompt. 2. Navigate to
+the directory where `runShortGPT.py` is located (the cloned repo). 3. Execute
+the following command to run the script: ``` python runShortGPT.py ``` 4. After
+running the script, a Gradio interface should open at your local host on port
+31415 (http://localhost:31415). ## Putting API Keys The ShortGPT UI needs you
+to input at least OpenAI and ElevenLabs api keys for running short automations.
+For video automations, you will also need to add a Pexels API. Follow these
+steps to add your OpenAI and ElevenLabs API keys: 1. Open [http://localhost:
+31415/?__theme=light](http://localhost:31415/?__theme=light) from a web
+browser. 2. Click on the `config` tab located at the left side bar of the user
+interface. 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the
+corresponding input fields. 4. Click `Save` to save your API keys. That's it!
+You have successfully set up your API keys and can now utilize the
+functionality of ShortGPT in the Gradio interface. ## Framework overview - ð¬
 The `ContentShortEngine` is designed for creating shorts, handling tasks from
 script generation to final rendering, including adding YouTube metadata. - ð¥
 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like
 generating audio, automatically sourcing background video footage, timing
 captions, and preparing background assets. - ðï¸ The automated
 `EditingEngine`, using Editing Markup Language and JSON, breaks down the
 editing process into manageable and customizable blocks, comprehensible to
@@ -97,17 +118,20 @@
 automated editing processes. - **ElevenLabs**: ElevenLabs is used for voice
 synthesis, supporting multiple languages for voiceover creation. - **Pexels**:
 Pexels is used for sourcing background footage, allowing ShortGPT to connect
 with the web and access a wide range of images and videos. - **Bing Image**:
 Bing Image is used for sourcing images, providing a comprehensive database for
 ShortGPT to retrieve relevant visuals. These technologies work together to
 provide a seamless and efficient experience in automating video and short
-content creation with AI. ## ð Get in touch on Twitter ð¦ Keep up with the
-latest happenings, announcements, and insights about Short-GPT by checking out
-our Twitter accounts. Spark a conversation with our developer and the AI's own
+content creation with AI. ## ð Contributing As an open-source project in a
+rapidly developing field, we are extremely open to contributions, whether it
+would be in the form of a new feature, improved infrastructure, or better
+documentation. ## ð Get in touch on Twitter ð¦ Keep up with the latest
+happenings, announcements, and insights about Short-GPT by checking out our
+Twitter accounts. Spark a conversation with our developer and the AI's own
 account for fascinating dialogues, latest news about the project, and more. -
 **Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ).
 Deep-dive into behind-the-scenes, project news, and related topics from the
 person behind ShortGPT. We're eager to interact with you and listen to your
-feedback, concepts, and experiences with Auto-GPT. Come on board on Twitter and
-let's navigate the future of AI as a team! ð¡ð¤
+feedback, concepts, and experiences with Short-GPT. Come on board on Twitter
+and let's navigate the future of AI as a team! ð¡ð¤
                              [Star_History_Chart]
```

### Comparing `ShortGPT-0.0.1/README.md` & `shortgpt-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,133 +1,142 @@
-
-# 🎬🚀 ShortGPT
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+# 🚀🎬 ShortGPT
 [![](https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R)
+[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ)
 [![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/shortgpt)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ) 
 <div align="center">
-    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/d9f87cf2-021d-4b8d-bb86-b3a7af1d80d4" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
+    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
 </div>
-
 <div align="center">
   <a href="https://discord.gg/uERx39ru3R">
     <img src="https://img.shields.io/badge/discord-join%20chat-blue.svg" alt="Join our Discord" height="34">
   </a>
 </div>
 
+<div align="center">
 ⚡ Automating video and short content creation with AI ⚡
+</div>
+
+## 🎥 Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U))
+
+https://github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-6365c27ea5fe
+## 🎥 Voice Dubbing
+
+
+https://github.com/RayVentura/ShortGPT/assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef
 
+## 🌟 Show Your Support
+We hope you find ShortGPT helpful! If you do, let us know by giving us a star ⭐ on the repo. It's easy, just click on the 'Star' button at the top right of the page. Your support means a lot to us and keeps us motivated to improve and expand ShortGPT. Thank you and happy content creating! 🎉 
+
+[![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://github.com/RayVentura/ShortGPT/stargazers)
+## 🛠️ How it works
+![alt text](https://github.com/RayVentura/ShortGPT/assets/121462835/fcee74d4-f856-4481-949f-244558bf3bfa)
 ## 📝 Introduction to ShortGPT 
-ShortGPT is a powerful tool for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
+ShortGPT is a powerful framework for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
 
 - 🎞️ **Automated editing framework**: Streamlines the video creation process with an LLM oriented video editing language.
 
 - 📃 **Scripts and Prompts**: Provides ready-to-use scripts and prompts for various LLM automated editing processes.
 
 - 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, and Portuguese 🇵🇹.
 
 - 🔗 **Caption Generation**: Automates the generation of video captions.
 
 - 🌐🎥 **Asset Sourcing**: Sources images and video footage from the internet, connecting with the web and Pexels API as necessary.
 
 - 🧠 **Memory and persistency**: Ensures long-term persistency of automated editing variables with TinyDB.
 
+## 🚀 Quick Start: Run ShortGPT on Google Colab (https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
-## Showcase
-
+If you prefer not to install the prerequisites on your local system, you can use the Google Colab notebook. This option is free and requires no installation setup.
 
-https://github.com/RayVentura/ShortGPT/assets/121462835/d357ba50-51d7-4c1c-a7ba-72d8353a804d
+1. Click on the link to the Google Colab notebook: [https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
+2. Once you're in the notebook, simply run the cells in order from top to bottom. You can do this by clicking on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy using ShortGPT!
 
 # Instructions for running shortGPT
-
-This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `shortgptUI.py` successfully.
+This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
 
 ## Prerequisites
-
 Before you begin, ensure that you have the following prerequisites installed on your system:
 - Python 3.x
 - Pip (Python package installer)
 
 ## Installation Steps
-
 Follow the instructions below to install ImageMagick, FFmpeg, and clone the shortGPT repository:
 
 ### Step 1: Install ImageMagick
-
 1. For `Windows` download the installer from the official ImageMagick website and follow the installation instructions.
       
       [https://imagemagick.org/script/download.php](https://imagemagick.org/script/download.php)
-      
-     
+          
 2. For Ubuntu/Debian-based systems, use the command:
      ```
      sudo apt-get install imagemagick
-     ```   
-    For macOS using Homebrew, use the command:
+     ```
+     Then run the following command to fix a moviepy Imagemagick policy.xml incompatibility problem:
+     ```
+     !sed -i '/<policy domain="path" rights="none" pattern="@\*"/d' /etc/ImageMagick-6/policy.xml
+     ```    
+4. For macOS using Homebrew, use the command:
      ```
      brew install imagemagick
      ```
-
 2. Verify the installation by running the following command:
    ```
    convert --version
    ```
-
    You should see the ImageMagick version information if the installation was successful.
 
-### Step 2: Install FFmpeg
-
-1. For `Windows`Download the FFmpeg binaries from the official website and add the executable to your system's PATH. 
+### Step 2: Install FFmpeg (REQUIRED FOR SHORTGPT TO WORK)
+1. For `Windows`Download the FFmpeg binaries from this Windows Installer (It will download ffmpeg, ffprobe and add it to your path).
       
-      [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)
+      [https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306)
       
 2. For macOS using Homebrew, use the command:
      ```
      brew install ffmpeg
      ```   
     For Ubuntu/Debian-based systems, use the command:
      ```
      sudo apt-get install ffmpeg
      ```
 2. Verify the installation by running the following command:
    ```
    ffmpeg -version
    ```
-
    You should see the FFmpeg version information if the installation was successful.
 
 ### Step 3: Clone the shortGPT Repository
 
 1. Open a terminal or command prompt.
 2. Execute the following command to clone the shortGPT repository:
    ```
    git clone https://github.com/rayventura/shortgpt.git
    ```
 
 ### Step 4: Install Python Dependencies
 
 1. Open a terminal or command prompt.
-2. Navigate to the directory where `shortgpt.py` is located (the cloned repo).
+2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to install the required Python dependencies:
    ```
    pip install -r requirements.txt
    ```
 
    This command will install the necessary packages specified in the `requirements.txt` file.
 
-## Running shortgptUI.py Web Interface
+## Running runShortGPT.py Web Interface
 
-Once you have successfully installed ImageMagick, FFmpeg, and the Python dependencies, you can run `shortgpt.py` by following these steps:
+Once you have successfully installed ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py` by following these steps:
 
 1. Open a terminal or command prompt.
-2. Navigate to the directory where `shortgptUI.py` is located (the cloned repo).
+2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to run the script:
    ```
-   python shortgptUI.py
+   python runShortGPT.py
    ```
 4. After running the script, a Gradio interface should open at your local host on port 31415 (http://localhost:31415). 
 
 ## Putting API Keys
 The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for running short automations. For video automations, you will also need to add a Pexels API.
 
 Follow these steps to add your OpenAI and ElevenLabs API keys:
@@ -135,32 +144,29 @@
 1. Open [http://localhost:31415/?__theme=light](http://localhost:31415/?__theme=light) from a web browser. 
 2. Click on the `config` tab located at the left side bar of the user interface.
 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the corresponding input fields.
 4. Click `Save` to save your API keys.
 
 That's it! You have successfully set up your API keys and can now utilize the functionality of ShortGPT in the Gradio interface.
 
-## 💁 Contributing
-
-As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
-
 ## Framework overview
 
 - 🎬 The `ContentShortEngine` is designed for creating shorts, handling tasks from script generation to final rendering, including adding YouTube metadata.
 
 - 🎥 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like generating audio, automatically sourcing background video footage, timing captions, and preparing background assets.
   
 - 🎞️ The automated `EditingEngine`, using Editing Markup Language and JSON, breaks down the editing process into manageable and customizable blocks, comprehensible to Large Language Models.
 
 💡 ShortGPT offers customization options to suit your needs, from language selection to watermark addition.
 
 🔧 As a framework, ShortGPT is adaptable and flexible, offering the potential for efficient, creative content creation.
 
 More documentation incomming, please be patient.
 
+
 ## Technologies Used
 
 ShortGPT utilizes the following technologies to power its functionality:
 
 - **Moviepy**: Moviepy is used for video editing, allowing ShortGPT to make video editing and rendering
 
 - **Openai**: Openai is used for automating the entire process, including generating scripts and prompts for LLM automated editing processes.
@@ -169,20 +175,23 @@
 
 - **Pexels**: Pexels is used for sourcing background footage, allowing ShortGPT to connect with the web and access a wide range of images and videos.
 
 - **Bing Image**: Bing Image is used for sourcing images, providing a comprehensive database for ShortGPT to retrieve relevant visuals.
 
 These technologies work together to provide a seamless and efficient experience in automating video and short content creation with AI.
 
+## 💁 Contributing
+
+As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it would be in the form of a new feature, improved infrastructure, or better documentation.
+
 ## 🔗 Get in touch on Twitter 🐦
 
 Keep up with the latest happenings, announcements, and insights about Short-GPT by checking out our Twitter accounts. Spark a conversation with our developer and the AI's own account for fascinating dialogues, latest news about the project, and more.
 
 - **Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ). Deep-dive into behind-the-scenes, project news, and related topics from the person behind ShortGPT.
 
-We're eager to interact with you and listen to your feedback, concepts, and experiences with Auto-GPT. Come on board on Twitter and let's navigate the future of AI as a team! 💡🤖
-
+We're eager to interact with you and listen to your feedback, concepts, and experiences with Short-GPT. Come on board on Twitter and let's navigate the future of AI as a team! 💡🤖
 <p align="center">
-  <a href="https://star-history.com/#ReyVentura/ShortGPT&Date">
+  <a href="https://star-history.com/#RayVentura/ShortGPT&Date">
     <img src="https://api.star-history.com/svg?repos=RayVentura/ShortGPT&type=Date" alt="Star History Chart">
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,80 +1,101 @@
- # ð¬ð ShortGPT [![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT) [![](https://
-dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://
-discord.gg/uERx39ru3R) [![GitHub star chart](https://img.shields.io/github/
-stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
-shortgpt) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/
+# ðð¬ ShortGPT [![](https://dcbadge.vercel.app/api/server/
+uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R) [![Twitter]
+(https://img.shields.io/twitter/url/https/twitter.com/
 rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://
-twitter.com/RayVenturaHQ)
+twitter.com/RayVenturaHQ) [![GitHub star chart](https://img.shields.io/github/
+stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
+shortgpt)
                                 [ShortGPT-logo]
                               [Join_our_Discord]
-â¡ Automating video and short content creation with AI â¡ ## ð
-Introduction to ShortGPT ShortGPT is a powerful tool for automating content
-creation. It simplifies video creation, footage sourcing, voiceover synthesis,
-and editing tasks. - ðï¸ **Automated editing framework**: Streamlines the
-video creation process with an LLM oriented video editing language. - ð
-**Scripts and Prompts**: Provides ready-to-use scripts and prompts for various
-LLM automated editing processes. - ð£ï¸ **Voiceover / Content Creation**:
-Supports multiple languages including English ðºð¸, Spanish ðªð¸,
-Arabic ð¦ðª, French ð«ð·, Polish ðµð±, German ð©ðª, Italian
-ð®ð¹, and Portuguese ðµð¹. - ð **Caption Generation**: Automates the
-generation of video captions. - ðð¥ **Asset Sourcing**: Sources images and
-video footage from the internet, connecting with the web and Pexels API as
-necessary. - ð§  **Memory and persistency**: Ensures long-term persistency of
-automated editing variables with TinyDB. ## Showcase https://github.com/
-RayVentura/ShortGPT/assets/121462835/d357ba50-51d7-4c1c-a7ba-72d8353a804d #
-Instructions for running shortGPT This guide provides step-by-step instructions
-for installing ImageMagick and FFmpeg on your system, which are both required
-to do automated editing. Once installed, you can proceed to run `shortgptUI.py`
-successfully. ## Prerequisites Before you begin, ensure that you have the
-following prerequisites installed on your system: - Python 3.x - Pip (Python
-package installer) ## Installation Steps Follow the instructions below to
-install ImageMagick, FFmpeg, and clone the shortGPT repository: ### Step 1:
-Install ImageMagick 1. For `Windows` download the installer from the official
-ImageMagick website and follow the installation instructions. [https://
-imagemagick.org/script/download.php](https://imagemagick.org/script/
-download.php) 2. For Ubuntu/Debian-based systems, use the command: ``` sudo
-apt-get install imagemagick ``` For macOS using Homebrew, use the command: ```
-brew install imagemagick ``` 2. Verify the installation by running the
-following command: ``` convert --version ``` You should see the ImageMagick
+          â¡ Automating video and short content creation with AI â¡
+## ð¥ Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U)) https:
+//github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-
+6365c27ea5fe ## ð¥ Voice Dubbing https://github.com/RayVentura/ShortGPT/
+assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef ## ð Show Your Support
+We hope you find ShortGPT helpful! If you do, let us know by giving us a star
+â­ on the repo. It's easy, just click on the 'Star' button at the top right of
+the page. Your support means a lot to us and keeps us motivated to improve and
+expand ShortGPT. Thank you and happy content creating! ð [![GitHub star
+chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)]
+(https://github.com/RayVentura/ShortGPT/stargazers) ## ð ï¸ How it works !
+[alt text](https://github.com/RayVentura/ShortGPT/assets/121462835/fcee74d4-
+f856-4481-949f-244558bf3bfa) ## ð Introduction to ShortGPT ShortGPT is a
+powerful framework for automating content creation. It simplifies video
+creation, footage sourcing, voiceover synthesis, and editing tasks. - ðï¸
+**Automated editing framework**: Streamlines the video creation process with an
+LLM oriented video editing language. - ð **Scripts and Prompts**: Provides
+ready-to-use scripts and prompts for various LLM automated editing processes. -
+ð£ï¸ **Voiceover / Content Creation**: Supports multiple languages including
+English ðºð¸, Spanish ðªð¸, Arabic ð¦ðª, French ð«ð·, Polish
+ðµð±, German ð©ðª, Italian ð®ð¹, and Portuguese ðµð¹. - ð
+**Caption Generation**: Automates the generation of video captions. - ðð¥
+**Asset Sourcing**: Sources images and video footage from the internet,
+connecting with the web and Pexels API as necessary. - ð§  **Memory and
+persistency**: Ensures long-term persistency of automated editing variables
+with TinyDB. ## ð Quick Start: Run ShortGPT on Google Colab (https://
+colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
+If you prefer not to install the prerequisites on your local system, you can
+use the Google Colab notebook. This option is free and requires no installation
+setup. 1. Click on the link to the Google Colab notebook: [https://
+colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing]
+(https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) 2. Once you're in the notebook,
+simply run the cells in order from top to bottom. You can do this by clicking
+on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy
+using ShortGPT! # Instructions for running shortGPT This guide provides step-
+by-step instructions for installing ImageMagick and FFmpeg on your system,
+which are both required to do automated editing. Once installed, you can
+proceed to run `runShortGPT.py` successfully. ## Prerequisites Before you
+begin, ensure that you have the following prerequisites installed on your
+system: - Python 3.x - Pip (Python package installer) ## Installation Steps
+Follow the instructions below to install ImageMagick, FFmpeg, and clone the
+shortGPT repository: ### Step 1: Install ImageMagick 1. For `Windows` download
+the installer from the official ImageMagick website and follow the installation
+instructions. [https://imagemagick.org/script/download.php](https://
+imagemagick.org/script/download.php) 2. For Ubuntu/Debian-based systems, use
+the command: ``` sudo apt-get install imagemagick ``` Then run the following
+command to fix a moviepy Imagemagick policy.xml incompatibility problem: ```
+!sed -i '/
+' /etc/ImageMagick-6/policy.xml ``` 4. For macOS using Homebrew, use the
+command: ``` brew install imagemagick ``` 2. Verify the installation by running
+the following command: ``` convert --version ``` You should see the ImageMagick
 version information if the installation was successful. ### Step 2: Install
-FFmpeg 1. For `Windows`Download the FFmpeg binaries from the official website
-and add the executable to your system's PATH. [https://ffmpeg.org/
-download.html](https://ffmpeg.org/download.html) 2. For macOS using Homebrew,
-use the command: ``` brew install ffmpeg ``` For Ubuntu/Debian-based systems,
-use the command: ``` sudo apt-get install ffmpeg ``` 2. Verify the installation
-by running the following command: ``` ffmpeg -version ``` You should see the
-FFmpeg version information if the installation was successful. ### Step 3:
-Clone the shortGPT Repository 1. Open a terminal or command prompt. 2. Execute
-the following command to clone the shortGPT repository: ``` git clone https://
-github.com/rayventura/shortgpt.git ``` ### Step 4: Install Python Dependencies
-1. Open a terminal or command prompt. 2. Navigate to the directory where
-`shortgpt.py` is located (the cloned repo). 3. Execute the following command to
-install the required Python dependencies: ``` pip install -r requirements.txt
-``` This command will install the necessary packages specified in the
-`requirements.txt` file. ## Running shortgptUI.py Web Interface Once you have
-successfully installed ImageMagick, FFmpeg, and the Python dependencies, you
-can run `shortgpt.py` by following these steps: 1. Open a terminal or command
-prompt. 2. Navigate to the directory where `shortgptUI.py` is located (the
-cloned repo). 3. Execute the following command to run the script: ``` python
-shortgptUI.py ``` 4. After running the script, a Gradio interface should open
-at your local host on port 31415 (http://localhost:31415). ## Putting API Keys
-The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for
-running short automations. For video automations, you will also need to add a
-Pexels API. Follow these steps to add your OpenAI and ElevenLabs API keys: 1.
-Open [http://localhost:31415/?__theme=light](http://localhost:31415/
-?__theme=light) from a web browser. 2. Click on the `config` tab located at the
-left side bar of the user interface. 3. Add your `OPENAI API KEY` and
-`ELEVENLABS API KEY` in the corresponding input fields. 4. Click `Save` to save
-your API keys. That's it! You have successfully set up your API keys and can
-now utilize the functionality of ShortGPT in the Gradio interface. ## ð
-Contributing As an open-source project in a rapidly developing field, we are
-extremely open to contributions, whether it be in the form of a new feature,
-improved infrastructure, or better documentation. ## Framework overview - ð¬
+FFmpeg (REQUIRED FOR SHORTGPT TO WORK) 1. For `Windows`Download the FFmpeg
+binaries from this Windows Installer (It will download ffmpeg, ffprobe and add
+it to your path). [https://github.com/icedterminal/ffmpeg-installer/releases/
+tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/
+tag/6.0.0.20230306) 2. For macOS using Homebrew, use the command: ``` brew
+install ffmpeg ``` For Ubuntu/Debian-based systems, use the command: ``` sudo
+apt-get install ffmpeg ``` 2. Verify the installation by running the following
+command: ``` ffmpeg -version ``` You should see the FFmpeg version information
+if the installation was successful. ### Step 3: Clone the shortGPT Repository
+1. Open a terminal or command prompt. 2. Execute the following command to clone
+the shortGPT repository: ``` git clone https://github.com/rayventura/
+shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a terminal or
+command prompt. 2. Navigate to the directory where `runShortGPT.py` is located
+(the cloned repo). 3. Execute the following command to install the required
+Python dependencies: ``` pip install -r requirements.txt ``` This command will
+install the necessary packages specified in the `requirements.txt` file. ##
+Running runShortGPT.py Web Interface Once you have successfully installed
+ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py`
+by following these steps: 1. Open a terminal or command prompt. 2. Navigate to
+the directory where `runShortGPT.py` is located (the cloned repo). 3. Execute
+the following command to run the script: ``` python runShortGPT.py ``` 4. After
+running the script, a Gradio interface should open at your local host on port
+31415 (http://localhost:31415). ## Putting API Keys The ShortGPT UI needs you
+to input at least OpenAI and ElevenLabs api keys for running short automations.
+For video automations, you will also need to add a Pexels API. Follow these
+steps to add your OpenAI and ElevenLabs API keys: 1. Open [http://localhost:
+31415/?__theme=light](http://localhost:31415/?__theme=light) from a web
+browser. 2. Click on the `config` tab located at the left side bar of the user
+interface. 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the
+corresponding input fields. 4. Click `Save` to save your API keys. That's it!
+You have successfully set up your API keys and can now utilize the
+functionality of ShortGPT in the Gradio interface. ## Framework overview - ð¬
 The `ContentShortEngine` is designed for creating shorts, handling tasks from
 script generation to final rendering, including adding YouTube metadata. - ð¥
 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like
 generating audio, automatically sourcing background video footage, timing
 captions, and preparing background assets. - ðï¸ The automated
 `EditingEngine`, using Editing Markup Language and JSON, breaks down the
 editing process into manageable and customizable blocks, comprehensible to
@@ -89,17 +110,20 @@
 automated editing processes. - **ElevenLabs**: ElevenLabs is used for voice
 synthesis, supporting multiple languages for voiceover creation. - **Pexels**:
 Pexels is used for sourcing background footage, allowing ShortGPT to connect
 with the web and access a wide range of images and videos. - **Bing Image**:
 Bing Image is used for sourcing images, providing a comprehensive database for
 ShortGPT to retrieve relevant visuals. These technologies work together to
 provide a seamless and efficient experience in automating video and short
-content creation with AI. ## ð Get in touch on Twitter ð¦ Keep up with the
-latest happenings, announcements, and insights about Short-GPT by checking out
-our Twitter accounts. Spark a conversation with our developer and the AI's own
+content creation with AI. ## ð Contributing As an open-source project in a
+rapidly developing field, we are extremely open to contributions, whether it
+would be in the form of a new feature, improved infrastructure, or better
+documentation. ## ð Get in touch on Twitter ð¦ Keep up with the latest
+happenings, announcements, and insights about Short-GPT by checking out our
+Twitter accounts. Spark a conversation with our developer and the AI's own
 account for fascinating dialogues, latest news about the project, and more. -
 **Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ).
 Deep-dive into behind-the-scenes, project news, and related topics from the
 person behind ShortGPT. We're eager to interact with you and listen to your
-feedback, concepts, and experiences with Auto-GPT. Come on board on Twitter and
-let's navigate the future of AI as a team! ð¡ð¤
+feedback, concepts, and experiences with Short-GPT. Come on board on Twitter
+and let's navigate the future of AI as a team! ð¡ð¤
                              [Star_History_Chart]
```

### Comparing `ShortGPT-0.0.1/ShortGPT.egg-info/PKG-INFO` & `shortgpt-0.0.2/shortgpt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,150 +1,159 @@
 Metadata-Version: 2.1
-Name: ShortGPT
-Version: 0.0.1
+Name: shortgpt
+Version: 0.0.2
 Summary: Automating video and short content creation with AI
 Author: RayVentura
 Author-email: 
 Keywords: python,video,content creation,AI,automation,editing,voiceover synthesis,video captions,asset sourcing,tinyDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-
-# 🎬🚀 ShortGPT
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+# 🚀🎬 ShortGPT
 [![](https://dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R)
+[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ)
 [![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/shortgpt)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://twitter.com/RayVenturaHQ) 
 <div align="center">
-    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/d9f87cf2-021d-4b8d-bb86-b3a7af1d80d4" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
+    <img src="https://github.com/RayVentura/ShortGPT/assets/121462835/083c8dc3-bac5-42c1-a08d-3ff9686d18c5" alt="ShortGPT-logo" style="border-radius: 20px;" width="22%"/>
 </div>
-
 <div align="center">
   <a href="https://discord.gg/uERx39ru3R">
     <img src="https://img.shields.io/badge/discord-join%20chat-blue.svg" alt="Join our Discord" height="34">
   </a>
 </div>
 
+<div align="center">
 ⚡ Automating video and short content creation with AI ⚡
+</div>
+
+## 🎥 Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U))
+
+https://github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-6365c27ea5fe
+## 🎥 Voice Dubbing
+
+
+https://github.com/RayVentura/ShortGPT/assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef
 
+## 🌟 Show Your Support
+We hope you find ShortGPT helpful! If you do, let us know by giving us a star ⭐ on the repo. It's easy, just click on the 'Star' button at the top right of the page. Your support means a lot to us and keeps us motivated to improve and expand ShortGPT. Thank you and happy content creating! 🎉 
+
+[![GitHub star chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)](https://github.com/RayVentura/ShortGPT/stargazers)
+## 🛠️ How it works
+![alt text](https://github.com/RayVentura/ShortGPT/assets/121462835/fcee74d4-f856-4481-949f-244558bf3bfa)
 ## 📝 Introduction to ShortGPT 
-ShortGPT is a powerful tool for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
+ShortGPT is a powerful framework for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.
 
 - 🎞️ **Automated editing framework**: Streamlines the video creation process with an LLM oriented video editing language.
 
 - 📃 **Scripts and Prompts**: Provides ready-to-use scripts and prompts for various LLM automated editing processes.
 
 - 🗣️ **Voiceover / Content Creation**: Supports multiple languages including English 🇺🇸, Spanish 🇪🇸, Arabic 🇦🇪, French 🇫🇷, Polish 🇵🇱, German 🇩🇪, Italian 🇮🇹, and Portuguese 🇵🇹.
 
 - 🔗 **Caption Generation**: Automates the generation of video captions.
 
 - 🌐🎥 **Asset Sourcing**: Sources images and video footage from the internet, connecting with the web and Pexels API as necessary.
 
 - 🧠 **Memory and persistency**: Ensures long-term persistency of automated editing variables with TinyDB.
 
+## 🚀 Quick Start: Run ShortGPT on Google Colab (https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
-## Showcase
-
+If you prefer not to install the prerequisites on your local system, you can use the Google Colab notebook. This option is free and requires no installation setup.
 
-https://github.com/RayVentura/ShortGPT/assets/121462835/d357ba50-51d7-4c1c-a7ba-72d8353a804d
+1. Click on the link to the Google Colab notebook: [https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing](https://colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
 
+2. Once you're in the notebook, simply run the cells in order from top to bottom. You can do this by clicking on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy using ShortGPT!
 
 # Instructions for running shortGPT
-
-This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `shortgptUI.py` successfully.
+This guide provides step-by-step instructions for installing ImageMagick and FFmpeg on your system, which are both required to do automated editing. Once installed, you can proceed to run `runShortGPT.py` successfully.
 
 ## Prerequisites
-
 Before you begin, ensure that you have the following prerequisites installed on your system:
 - Python 3.x
 - Pip (Python package installer)
 
 ## Installation Steps
-
 Follow the instructions below to install ImageMagick, FFmpeg, and clone the shortGPT repository:
 
 ### Step 1: Install ImageMagick
-
 1. For `Windows` download the installer from the official ImageMagick website and follow the installation instructions.
       
       [https://imagemagick.org/script/download.php](https://imagemagick.org/script/download.php)
-      
-     
+          
 2. For Ubuntu/Debian-based systems, use the command:
      ```
      sudo apt-get install imagemagick
-     ```   
-    For macOS using Homebrew, use the command:
+     ```
+     Then run the following command to fix a moviepy Imagemagick policy.xml incompatibility problem:
+     ```
+     !sed -i '/<policy domain="path" rights="none" pattern="@\*"/d' /etc/ImageMagick-6/policy.xml
+     ```    
+4. For macOS using Homebrew, use the command:
      ```
      brew install imagemagick
      ```
-
 2. Verify the installation by running the following command:
    ```
    convert --version
    ```
-
    You should see the ImageMagick version information if the installation was successful.
 
-### Step 2: Install FFmpeg
-
-1. For `Windows`Download the FFmpeg binaries from the official website and add the executable to your system's PATH. 
+### Step 2: Install FFmpeg (REQUIRED FOR SHORTGPT TO WORK)
+1. For `Windows`Download the FFmpeg binaries from this Windows Installer (It will download ffmpeg, ffprobe and add it to your path).
       
-      [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)
+      [https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/tag/6.0.0.20230306)
       
 2. For macOS using Homebrew, use the command:
      ```
      brew install ffmpeg
      ```   
     For Ubuntu/Debian-based systems, use the command:
      ```
      sudo apt-get install ffmpeg
      ```
 2. Verify the installation by running the following command:
    ```
    ffmpeg -version
    ```
-
    You should see the FFmpeg version information if the installation was successful.
 
 ### Step 3: Clone the shortGPT Repository
 
 1. Open a terminal or command prompt.
 2. Execute the following command to clone the shortGPT repository:
    ```
    git clone https://github.com/rayventura/shortgpt.git
    ```
 
 ### Step 4: Install Python Dependencies
 
 1. Open a terminal or command prompt.
-2. Navigate to the directory where `shortgpt.py` is located (the cloned repo).
+2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to install the required Python dependencies:
    ```
    pip install -r requirements.txt
    ```
 
    This command will install the necessary packages specified in the `requirements.txt` file.
 
-## Running shortgptUI.py Web Interface
+## Running runShortGPT.py Web Interface
 
-Once you have successfully installed ImageMagick, FFmpeg, and the Python dependencies, you can run `shortgpt.py` by following these steps:
+Once you have successfully installed ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py` by following these steps:
 
 1. Open a terminal or command prompt.
-2. Navigate to the directory where `shortgptUI.py` is located (the cloned repo).
+2. Navigate to the directory where `runShortGPT.py` is located (the cloned repo).
 3. Execute the following command to run the script:
    ```
-   python shortgptUI.py
+   python runShortGPT.py
    ```
 4. After running the script, a Gradio interface should open at your local host on port 31415 (http://localhost:31415). 
 
 ## Putting API Keys
 The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for running short automations. For video automations, you will also need to add a Pexels API.
 
 Follow these steps to add your OpenAI and ElevenLabs API keys:
@@ -152,32 +161,29 @@
 1. Open [http://localhost:31415/?__theme=light](http://localhost:31415/?__theme=light) from a web browser. 
 2. Click on the `config` tab located at the left side bar of the user interface.
 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the corresponding input fields.
 4. Click `Save` to save your API keys.
 
 That's it! You have successfully set up your API keys and can now utilize the functionality of ShortGPT in the Gradio interface.
 
-## 💁 Contributing
-
-As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
-
 ## Framework overview
 
 - 🎬 The `ContentShortEngine` is designed for creating shorts, handling tasks from script generation to final rendering, including adding YouTube metadata.
 
 - 🎥 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like generating audio, automatically sourcing background video footage, timing captions, and preparing background assets.
   
 - 🎞️ The automated `EditingEngine`, using Editing Markup Language and JSON, breaks down the editing process into manageable and customizable blocks, comprehensible to Large Language Models.
 
 💡 ShortGPT offers customization options to suit your needs, from language selection to watermark addition.
 
 🔧 As a framework, ShortGPT is adaptable and flexible, offering the potential for efficient, creative content creation.
 
 More documentation incomming, please be patient.
 
+
 ## Technologies Used
 
 ShortGPT utilizes the following technologies to power its functionality:
 
 - **Moviepy**: Moviepy is used for video editing, allowing ShortGPT to make video editing and rendering
 
 - **Openai**: Openai is used for automating the entire process, including generating scripts and prompts for LLM automated editing processes.
@@ -186,20 +192,23 @@
 
 - **Pexels**: Pexels is used for sourcing background footage, allowing ShortGPT to connect with the web and access a wide range of images and videos.
 
 - **Bing Image**: Bing Image is used for sourcing images, providing a comprehensive database for ShortGPT to retrieve relevant visuals.
 
 These technologies work together to provide a seamless and efficient experience in automating video and short content creation with AI.
 
+## 💁 Contributing
+
+As an open-source project in a rapidly developing field, we are extremely open to contributions, whether it would be in the form of a new feature, improved infrastructure, or better documentation.
+
 ## 🔗 Get in touch on Twitter 🐦
 
 Keep up with the latest happenings, announcements, and insights about Short-GPT by checking out our Twitter accounts. Spark a conversation with our developer and the AI's own account for fascinating dialogues, latest news about the project, and more.
 
 - **Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ). Deep-dive into behind-the-scenes, project news, and related topics from the person behind ShortGPT.
 
-We're eager to interact with you and listen to your feedback, concepts, and experiences with Auto-GPT. Come on board on Twitter and let's navigate the future of AI as a team! 💡🤖
-
+We're eager to interact with you and listen to your feedback, concepts, and experiences with Short-GPT. Come on board on Twitter and let's navigate the future of AI as a team! 💡🤖
 <p align="center">
-  <a href="https://star-history.com/#ReyVentura/ShortGPT&Date">
+  <a href="https://star-history.com/#RayVentura/ShortGPT&Date">
     <img src="https://api.star-history.com/svg?repos=RayVentura/ShortGPT&type=Date" alt="Star History Chart">
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,88 +1,109 @@
-Metadata-Version: 2.1 Name: ShortGPT Version: 0.0.1 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.0.2 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
-LICENSE # ð¬ð ShortGPT [![License: MIT](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![](https://
-dcbadge.vercel.app/api/server/uERx39ru3R?compact=true&style=flat)](https://
-discord.gg/uERx39ru3R) [![GitHub star chart](https://img.shields.io/github/
-stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
-shortgpt) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/
+LICENSE # ðð¬ ShortGPT [![](https://dcbadge.vercel.app/api/server/
+uERx39ru3R?compact=true&style=flat)](https://discord.gg/uERx39ru3R) [![Twitter]
+(https://img.shields.io/twitter/url/https/twitter.com/
 rayventurahq.svg?style=social&label=Follow%20%40RayVentura)](https://
-twitter.com/RayVenturaHQ)
+twitter.com/RayVenturaHQ) [![GitHub star chart](https://img.shields.io/github/
+stars/rayventura/shortgpt?style=social)](https://star-history.com/#rayventura/
+shortgpt)
                                 [ShortGPT-logo]
                               [Join_our_Discord]
-â¡ Automating video and short content creation with AI â¡ ## ð
-Introduction to ShortGPT ShortGPT is a powerful tool for automating content
-creation. It simplifies video creation, footage sourcing, voiceover synthesis,
-and editing tasks. - ðï¸ **Automated editing framework**: Streamlines the
-video creation process with an LLM oriented video editing language. - ð
-**Scripts and Prompts**: Provides ready-to-use scripts and prompts for various
-LLM automated editing processes. - ð£ï¸ **Voiceover / Content Creation**:
-Supports multiple languages including English ðºð¸, Spanish ðªð¸,
-Arabic ð¦ðª, French ð«ð·, Polish ðµð±, German ð©ðª, Italian
-ð®ð¹, and Portuguese ðµð¹. - ð **Caption Generation**: Automates the
-generation of video captions. - ðð¥ **Asset Sourcing**: Sources images and
-video footage from the internet, connecting with the web and Pexels API as
-necessary. - ð§  **Memory and persistency**: Ensures long-term persistency of
-automated editing variables with TinyDB. ## Showcase https://github.com/
-RayVentura/ShortGPT/assets/121462835/d357ba50-51d7-4c1c-a7ba-72d8353a804d #
-Instructions for running shortGPT This guide provides step-by-step instructions
-for installing ImageMagick and FFmpeg on your system, which are both required
-to do automated editing. Once installed, you can proceed to run `shortgptUI.py`
-successfully. ## Prerequisites Before you begin, ensure that you have the
-following prerequisites installed on your system: - Python 3.x - Pip (Python
-package installer) ## Installation Steps Follow the instructions below to
-install ImageMagick, FFmpeg, and clone the shortGPT repository: ### Step 1:
-Install ImageMagick 1. For `Windows` download the installer from the official
-ImageMagick website and follow the installation instructions. [https://
-imagemagick.org/script/download.php](https://imagemagick.org/script/
-download.php) 2. For Ubuntu/Debian-based systems, use the command: ``` sudo
-apt-get install imagemagick ``` For macOS using Homebrew, use the command: ```
-brew install imagemagick ``` 2. Verify the installation by running the
-following command: ``` convert --version ``` You should see the ImageMagick
+          â¡ Automating video and short content creation with AI â¡
+## ð¥ Showcase ([Full video on YouTube](https://youtu.be/hpoSHq-ER8U)) https:
+//github.com/RayVentura/ShortGPT/assets/121462835/a802faad-0fd7-4fcb-aa82-
+6365c27ea5fe ## ð¥ Voice Dubbing https://github.com/RayVentura/ShortGPT/
+assets/121462835/06f51b2d-f8b1-4a23-b299-55e0e18902ef ## ð Show Your Support
+We hope you find ShortGPT helpful! If you do, let us know by giving us a star
+â­ on the repo. It's easy, just click on the 'Star' button at the top right of
+the page. Your support means a lot to us and keeps us motivated to improve and
+expand ShortGPT. Thank you and happy content creating! ð [![GitHub star
+chart](https://img.shields.io/github/stars/rayventura/shortgpt?style=social)]
+(https://github.com/RayVentura/ShortGPT/stargazers) ## ð ï¸ How it works !
+[alt text](https://github.com/RayVentura/ShortGPT/assets/121462835/fcee74d4-
+f856-4481-949f-244558bf3bfa) ## ð Introduction to ShortGPT ShortGPT is a
+powerful framework for automating content creation. It simplifies video
+creation, footage sourcing, voiceover synthesis, and editing tasks. - ðï¸
+**Automated editing framework**: Streamlines the video creation process with an
+LLM oriented video editing language. - ð **Scripts and Prompts**: Provides
+ready-to-use scripts and prompts for various LLM automated editing processes. -
+ð£ï¸ **Voiceover / Content Creation**: Supports multiple languages including
+English ðºð¸, Spanish ðªð¸, Arabic ð¦ðª, French ð«ð·, Polish
+ðµð±, German ð©ðª, Italian ð®ð¹, and Portuguese ðµð¹. - ð
+**Caption Generation**: Automates the generation of video captions. - ðð¥
+**Asset Sourcing**: Sources images and video footage from the internet,
+connecting with the web and Pexels API as necessary. - ð§  **Memory and
+persistency**: Ensures long-term persistency of automated editing variables
+with TinyDB. ## ð Quick Start: Run ShortGPT on Google Colab (https://
+colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing)
+If you prefer not to install the prerequisites on your local system, you can
+use the Google Colab notebook. This option is free and requires no installation
+setup. 1. Click on the link to the Google Colab notebook: [https://
+colab.research.google.com/drive/1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing]
+(https://colab.research.google.com/drive/
+1_2UKdpF6lqxCqWaAcZb3rwMVQqtbisdE?usp=sharing) 2. Once you're in the notebook,
+simply run the cells in order from top to bottom. You can do this by clicking
+on each cell and pressing the 'Play' button, or by using the keyboard . Enjoy
+using ShortGPT! # Instructions for running shortGPT This guide provides step-
+by-step instructions for installing ImageMagick and FFmpeg on your system,
+which are both required to do automated editing. Once installed, you can
+proceed to run `runShortGPT.py` successfully. ## Prerequisites Before you
+begin, ensure that you have the following prerequisites installed on your
+system: - Python 3.x - Pip (Python package installer) ## Installation Steps
+Follow the instructions below to install ImageMagick, FFmpeg, and clone the
+shortGPT repository: ### Step 1: Install ImageMagick 1. For `Windows` download
+the installer from the official ImageMagick website and follow the installation
+instructions. [https://imagemagick.org/script/download.php](https://
+imagemagick.org/script/download.php) 2. For Ubuntu/Debian-based systems, use
+the command: ``` sudo apt-get install imagemagick ``` Then run the following
+command to fix a moviepy Imagemagick policy.xml incompatibility problem: ```
+!sed -i '/
+' /etc/ImageMagick-6/policy.xml ``` 4. For macOS using Homebrew, use the
+command: ``` brew install imagemagick ``` 2. Verify the installation by running
+the following command: ``` convert --version ``` You should see the ImageMagick
 version information if the installation was successful. ### Step 2: Install
-FFmpeg 1. For `Windows`Download the FFmpeg binaries from the official website
-and add the executable to your system's PATH. [https://ffmpeg.org/
-download.html](https://ffmpeg.org/download.html) 2. For macOS using Homebrew,
-use the command: ``` brew install ffmpeg ``` For Ubuntu/Debian-based systems,
-use the command: ``` sudo apt-get install ffmpeg ``` 2. Verify the installation
-by running the following command: ``` ffmpeg -version ``` You should see the
-FFmpeg version information if the installation was successful. ### Step 3:
-Clone the shortGPT Repository 1. Open a terminal or command prompt. 2. Execute
-the following command to clone the shortGPT repository: ``` git clone https://
-github.com/rayventura/shortgpt.git ``` ### Step 4: Install Python Dependencies
-1. Open a terminal or command prompt. 2. Navigate to the directory where
-`shortgpt.py` is located (the cloned repo). 3. Execute the following command to
-install the required Python dependencies: ``` pip install -r requirements.txt
-``` This command will install the necessary packages specified in the
-`requirements.txt` file. ## Running shortgptUI.py Web Interface Once you have
-successfully installed ImageMagick, FFmpeg, and the Python dependencies, you
-can run `shortgpt.py` by following these steps: 1. Open a terminal or command
-prompt. 2. Navigate to the directory where `shortgptUI.py` is located (the
-cloned repo). 3. Execute the following command to run the script: ``` python
-shortgptUI.py ``` 4. After running the script, a Gradio interface should open
-at your local host on port 31415 (http://localhost:31415). ## Putting API Keys
-The ShortGPT UI needs you to input at least OpenAI and ElevenLabs api keys for
-running short automations. For video automations, you will also need to add a
-Pexels API. Follow these steps to add your OpenAI and ElevenLabs API keys: 1.
-Open [http://localhost:31415/?__theme=light](http://localhost:31415/
-?__theme=light) from a web browser. 2. Click on the `config` tab located at the
-left side bar of the user interface. 3. Add your `OPENAI API KEY` and
-`ELEVENLABS API KEY` in the corresponding input fields. 4. Click `Save` to save
-your API keys. That's it! You have successfully set up your API keys and can
-now utilize the functionality of ShortGPT in the Gradio interface. ## ð
-Contributing As an open-source project in a rapidly developing field, we are
-extremely open to contributions, whether it be in the form of a new feature,
-improved infrastructure, or better documentation. ## Framework overview - ð¬
+FFmpeg (REQUIRED FOR SHORTGPT TO WORK) 1. For `Windows`Download the FFmpeg
+binaries from this Windows Installer (It will download ffmpeg, ffprobe and add
+it to your path). [https://github.com/icedterminal/ffmpeg-installer/releases/
+tag/6.0.0.20230306](https://github.com/icedterminal/ffmpeg-installer/releases/
+tag/6.0.0.20230306) 2. For macOS using Homebrew, use the command: ``` brew
+install ffmpeg ``` For Ubuntu/Debian-based systems, use the command: ``` sudo
+apt-get install ffmpeg ``` 2. Verify the installation by running the following
+command: ``` ffmpeg -version ``` You should see the FFmpeg version information
+if the installation was successful. ### Step 3: Clone the shortGPT Repository
+1. Open a terminal or command prompt. 2. Execute the following command to clone
+the shortGPT repository: ``` git clone https://github.com/rayventura/
+shortgpt.git ``` ### Step 4: Install Python Dependencies 1. Open a terminal or
+command prompt. 2. Navigate to the directory where `runShortGPT.py` is located
+(the cloned repo). 3. Execute the following command to install the required
+Python dependencies: ``` pip install -r requirements.txt ``` This command will
+install the necessary packages specified in the `requirements.txt` file. ##
+Running runShortGPT.py Web Interface Once you have successfully installed
+ImageMagick, FFmpeg, and the Python dependencies, you can run `runShortGPT.py`
+by following these steps: 1. Open a terminal or command prompt. 2. Navigate to
+the directory where `runShortGPT.py` is located (the cloned repo). 3. Execute
+the following command to run the script: ``` python runShortGPT.py ``` 4. After
+running the script, a Gradio interface should open at your local host on port
+31415 (http://localhost:31415). ## Putting API Keys The ShortGPT UI needs you
+to input at least OpenAI and ElevenLabs api keys for running short automations.
+For video automations, you will also need to add a Pexels API. Follow these
+steps to add your OpenAI and ElevenLabs API keys: 1. Open [http://localhost:
+31415/?__theme=light](http://localhost:31415/?__theme=light) from a web
+browser. 2. Click on the `config` tab located at the left side bar of the user
+interface. 3. Add your `OPENAI API KEY` and `ELEVENLABS API KEY` in the
+corresponding input fields. 4. Click `Save` to save your API keys. That's it!
+You have successfully set up your API keys and can now utilize the
+functionality of ShortGPT in the Gradio interface. ## Framework overview - ð¬
 The `ContentShortEngine` is designed for creating shorts, handling tasks from
 script generation to final rendering, including adding YouTube metadata. - ð¥
 The `ContentVideoEngine` is ideal for longer videos, taking care of tasks like
 generating audio, automatically sourcing background video footage, timing
 captions, and preparing background assets. - ðï¸ The automated
 `EditingEngine`, using Editing Markup Language and JSON, breaks down the
 editing process into manageable and customizable blocks, comprehensible to
@@ -97,17 +118,20 @@
 automated editing processes. - **ElevenLabs**: ElevenLabs is used for voice
 synthesis, supporting multiple languages for voiceover creation. - **Pexels**:
 Pexels is used for sourcing background footage, allowing ShortGPT to connect
 with the web and access a wide range of images and videos. - **Bing Image**:
 Bing Image is used for sourcing images, providing a comprehensive database for
 ShortGPT to retrieve relevant visuals. These technologies work together to
 provide a seamless and efficient experience in automating video and short
-content creation with AI. ## ð Get in touch on Twitter ð¦ Keep up with the
-latest happenings, announcements, and insights about Short-GPT by checking out
-our Twitter accounts. Spark a conversation with our developer and the AI's own
+content creation with AI. ## ð Contributing As an open-source project in a
+rapidly developing field, we are extremely open to contributions, whether it
+would be in the form of a new feature, improved infrastructure, or better
+documentation. ## ð Get in touch on Twitter ð¦ Keep up with the latest
+happenings, announcements, and insights about Short-GPT by checking out our
+Twitter accounts. Spark a conversation with our developer and the AI's own
 account for fascinating dialogues, latest news about the project, and more. -
 **Developer**: Stay updated [@RayVentura](https://twitter.com/RayVenturaHQ).
 Deep-dive into behind-the-scenes, project news, and related topics from the
 person behind ShortGPT. We're eager to interact with you and listen to your
-feedback, concepts, and experiences with Auto-GPT. Come on board on Twitter and
-let's navigate the future of AI as a team! ð¡ð¤
+feedback, concepts, and experiences with Short-GPT. Come on board on Twitter
+and let's navigate the future of AI as a team! ð¡ð¤
                              [Star_History_Chart]
```

### Comparing `ShortGPT-0.0.1/ShortGPT.egg-info/SOURCES.txt` & `shortgpt-0.0.2/shortgpt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 LICENSE
 README.md
 setup.py
-ShortGPT.egg-info/PKG-INFO
-ShortGPT.egg-info/SOURCES.txt
-ShortGPT.egg-info/dependency_links.txt
-ShortGPT.egg-info/requires.txt
-ShortGPT.egg-info/top_level.txt
 shortGPT/__init__.py
 shortGPT/api_utils/__init__.py
 shortGPT/api_utils/eleven_api.py
 shortGPT/api_utils/image_api.py
 shortGPT/api_utils/pexels_api.py
 shortGPT/audio/__init__.py
 shortGPT/audio/audio_duration.py
 shortGPT/audio/audio_utils.py
+shortGPT/audio/edge_voice_module.py
 shortGPT/audio/eleven_voice_module.py
 shortGPT/audio/voice_module.py
 shortGPT/config/__init__.py
 shortGPT/config/api_db.py
 shortGPT/config/asset_db.py
 shortGPT/config/config.py
 shortGPT/config/languages.py
+shortGPT/config/path_utils.py
 shortGPT/database/__init__.py
 shortGPT/database/content_data_manager.py
 shortGPT/database/content_database.py
 shortGPT/database/db_document.py
 shortGPT/editing_utils/__init__.py
 shortGPT/editing_utils/captions.py
 shortGPT/editing_utils/editing_images.py
 shortGPT/editing_utils/handle_videos.py
 shortGPT/engine/__init__.py
 shortGPT/engine/abstract_content_engine.py
 shortGPT/engine/content_short_engine.py
+shortGPT/engine/content_translation_engine.py
 shortGPT/engine/content_video_engine.py
 shortGPT/engine/facts_short_engine.py
+shortGPT/engine/multi_language_translation_engine.py
 shortGPT/engine/reddit_short_engine.py
 shortGPT/gpt/__init__.py
 shortGPT/gpt/facts_gpt.py
 shortGPT/gpt/gpt_chat_video.py
 shortGPT/gpt/gpt_editing.py
 shortGPT/gpt/gpt_translate.py
 shortGPT/gpt/gpt_utils.py
 shortGPT/gpt/gpt_voice.py
 shortGPT/gpt/gpt_yt.py
 shortGPT/gpt/reddit_gpt.py
 shortGPT/tracking/__init__.py
 shortGPT/tracking/api_tracking.py
-shortGPT/tracking/cost_analytics.py
+shortGPT/tracking/cost_analytics.py
+shortgpt.egg-info/PKG-INFO
+shortgpt.egg-info/SOURCES.txt
+shortgpt.egg-info/dependency_links.txt
+shortgpt.egg-info/requires.txt
+shortgpt.egg-info/top_level.txt
```

### Comparing `ShortGPT-0.0.1/setup.py` & `shortgpt-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Automating video and short content creation with AI'
 LONG_DESCRIPTION = 'A powerful tool for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.'
 
-# Setting up
+
 setup(
-    name="ShortGPT",
+    name="shortgpt",
     version=VERSION,
     author="RayVentura",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
@@ -27,19 +27,21 @@
         'gradio',
         'openai', 
         'tiktoken',
         'tinydb',
         'tinymongo',
         'proglog',
         'yt-dlp',
-        'torch', 
+        'torch',
+        'whisper-timestamped',
         'torchaudio',
+        'pillow==9.0.0',
         'protobuf==3.20.0',
-        'langchain',
-        'moviepy',
+        'edge-tts',
+        'moviepy==1.0.3',
         'termcolor',
         'progress',
         'questionary',
     ],
     keywords=['python', 'video', 'content creation', 'AI', 'automation', 'editing', 'voiceover synthesis', 'video captions', 'asset sourcing', 'tinyDB'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `ShortGPT-0.0.1/shortGPT/__init__.py` & `shortgpt-0.0.2/shortGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/api_utils/image_api.py` & `shortgpt-0.0.2/shortGPT/api_utils/image_api.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/api_utils/pexels_api.py` & `shortgpt-0.0.2/shortGPT/api_utils/pexels_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import requests
-from shortGPT.config.api_db import get_api_key
+
+from shortGPT.config.api_db import ApiKeyManager
+
+
 def search_videos(query_string, orientation_landscape=True):
     url = "https://api.pexels.com/videos/search"
     headers = {
-        "Authorization": get_api_key("PEXELS")
+        "Authorization": ApiKeyManager.get_api_key("PEXELS")
     }
     params = {
         "query": query_string,
         "orientation": "landscape" if orientation_landscape else "portrait",
         "per_page": 15
     }
-    
+
     response = requests.get(url, headers=headers, params=params)
     json_data = response.json()
     # print(response.headers['X-Ratelimit-Limit'])
     # print(response.headers['X-Ratelimit-Remaining'])
     # print(response.headers['X-Ratelimit-Reset'])
-    
+
     return json_data
 
-def getBestVideo(query_string, orientation_landscape=True, used_vids = []):
+
+def getBestVideo(query_string, orientation_landscape=True, used_vids=[]):
     vids = search_videos(query_string, orientation_landscape)
     videos = vids['videos']  # Extract the videos list from JSON
 
     # Filter and extract videos with width and height as 1920x1080 for landscape or 1080x1920 for portrait
     if orientation_landscape:
-        filtered_videos = [video for video in videos if video['width'] >= 1920 and video['height'] >= 1080 and video['width']/video['height']==16/9]
+        filtered_videos = [video for video in videos if video['width'] >= 1920 and video['height'] >= 1080 and video['width']/video['height'] == 16/9]
     else:
-        filtered_videos = [video for video in videos if video['width'] >= 1080 and video['height'] >= 1920 and video['height']/video['width']==16/9]
+        filtered_videos = [video for video in videos if video['width'] >= 1080 and video['height'] >= 1920 and video['height']/video['width'] == 16/9]
 
     # Sort the filtered videos by duration in ascending order
     sorted_videos = sorted(filtered_videos, key=lambda x: abs(15-int(x['duration'])))
 
     # Extract the top 3 videos' URLs
     for video in sorted_videos:
         for video_file in video['video_files']:
@@ -40,8 +44,8 @@
                     if not (video_file['link'].split('.hd')[0] in used_vids):
                         return video_file['link']
             else:
                 if video_file['width'] == 1080 and video_file['height'] == 1920:
                     if not (video_file['link'].split('.hd')[0] in used_vids):
                         return video_file['link']
     print("NO LINKS found for this round of search with query :", query_string)
-    return None
+    return None
```

### Comparing `ShortGPT-0.0.1/shortGPT/audio/audio_duration.py` & `shortgpt-0.0.2/shortGPT/audio/audio_duration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-import yt_dlp
-import subprocess
 import json
+import subprocess
+
+import yt_dlp
+
+from shortGPT.editing_utils.handle_videos import getYoutubeVideoLink
 
 
 def get_duration_yt_dlp(url):
     ydl_opts = {
-    "quiet": True,
-    "no_warnings": True,
-    "no_color": True,
-    "no_call_home": True,
-    "no_check_certificate": True
-}
+        "quiet": True,
+        "no_warnings": True,
+        "no_color": True,
+        "no_call_home": True,
+        "no_check_certificate": True
+    }
     try:
         with yt_dlp.YoutubeDL(ydl_opts) as ydl:
             dictMeta = ydl.extract_info(url, download=False, )
             return dictMeta['duration'], ""
     except Exception as e:
         return None, f"Failed getting duration from the following video/audio url/path using yt_dlp. {e.args[0]}"
 
+
 def get_duration_ffprobe(signed_url):
     try:
         cmd = [
             "ffprobe",
             "-v",
             "quiet",
             "-print_format",
@@ -38,67 +42,46 @@
         metadata = json.loads(output.stdout)
         duration = float(metadata["format"]["duration"])
         return duration, ""
     except Exception as e:
         print("Failed getting the duration of the asked ressource", e.args[0])
     return None, ""
 
-def getAssetDuration(url, isVideo=True):
-    if("youtube.com" in url):
+
+def get_asset_duration(url, isVideo=True):
+    if ("youtube.com" in url):
         if not isVideo:
-            return getYoutubeAudioLink(url)
+            url, _ = getYoutubeAudioLink(url)
         else:
-            return getYoutubeVideoLink(url)
-        
-    #Audio/Video is from some cloud storage provider. Link must be public.
-    else:
-        #Trying two different method to get the duration of the video / audio
-        duration, err_ffprobe = get_duration_ffprobe(url)
-        if duration is not None:
-            return url, duration
-
-        duration, err_yt_dlp = get_duration_yt_dlp(url)
-        if duration is not None:
-            return url, duration
-        print(err_yt_dlp)
-        print(err_ffprobe)
-        print(f"The url/path {url} does not point to a video/ audio. Impossible to extract its duration")
-        return url, None
+            url, _ = getYoutubeVideoLink(url)
+    # Trying two different method to get the duration of the video / audio
+    duration, err_ffprobe = get_duration_ffprobe(url)
+    if duration is not None:
+        return url, duration
+
+    duration, err_yt_dlp = get_duration_yt_dlp(url)
+    if duration is not None:
+        return url, duration
+    print(err_yt_dlp)
+    print(err_ffprobe)
+    print(f"The url/path {url} does not point to a video/ audio. Impossible to extract its duration")
+    return url, None
 
 
 def getYoutubeAudioLink(url):
     ydl_opts = {
-    "quiet": True,
-    "no_warnings": True,
-    "no_color": True,
-    "no_call_home": True,
-    "no_check_certificate": True,
-    "format": "bestaudio/best"
-    }
-    try:
-        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-            dictMeta = ydl.extract_info(
-                url,
-                download=False)
-            return dictMeta['url'], dictMeta['duration']
-    except Exception as e:
-        print("Failed getting audio link from the following video/url", e.args[0])
-    return None
-
-def getYoutubeVideoLink(url):
-    ydl_opts = {
         "quiet": True,
         "no_warnings": True,
         "no_color": True,
         "no_call_home": True,
         "no_check_certificate": True,
-        "format": "bestvideo[height<=1080]"
+        "format": "bestaudio/best"
     }
     try:
         with yt_dlp.YoutubeDL(ydl_opts) as ydl:
             dictMeta = ydl.extract_info(
                 url,
                 download=False)
             return dictMeta['url'], dictMeta['duration']
     except Exception as e:
-        print("Failed getting video link from the following video/url", e.args[0])
-    return None, None
+        print("Failed getting audio link from the following video/url", e.args[0])
+    return None
```

### Comparing `ShortGPT-0.0.1/shortGPT/audio/audio_utils.py` & `shortgpt-0.0.2/shortGPT/audio/audio_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from shortGPT.audio.audio_duration import getAssetDuration
 import os
 import subprocess
+
 import yt_dlp
-CONST_CHARS_PER_SEC = 20.5 # Arrived to this result after whispering a ton of shorts and calculating the average number of characters per second of speech.
+
+from shortGPT.audio.audio_duration import get_asset_duration
+
+CONST_CHARS_PER_SEC = 20.5  # Arrived to this result after whispering a ton of shorts and calculating the average number of characters per second of speech.
 
 WHISPER_MODEL = None
 
+
 def downloadYoutubeAudio(url, outputFile):
     ydl_opts = {
         "quiet": True,
         "no_warnings": True,
         "no_color": True,
         "no_call_home": True,
         "no_check_certificate": True,
@@ -24,23 +28,27 @@
             if (not os.path.exists(outputFile)):
                 raise Exception("Audio Download Failed")
             return outputFile, dictMeta['duration']
     except Exception as e:
         print("Failed downloading audio from the following video/url", e.args[0])
     return None
 
-def speedUpAudio(tempAudioPath, outputFile, expected_chars_per_sec=CONST_CHARS_PER_SEC): # Speeding up the audio to make it under 60secs, otherwise the output video is not considered as a short.
-    tempAudioPath, duration = getAssetDuration(tempAudioPath, False)
-    if(duration > 57):
-        subprocess.run(['ffmpeg', '-i', tempAudioPath, '-af', f'atempo={(duration/57):.5f}', outputFile])
+
+def speedUpAudio(tempAudioPath, outputFile, expected_duration=None):  # Speeding up the audio to make it under 60secs, otherwise the output video is not considered as a short.
+    tempAudioPath, duration = get_asset_duration(tempAudioPath, False)
+    if not expected_duration:
+        if (duration > 57):
+            subprocess.run(['ffmpeg', '-i', tempAudioPath, '-af', f'atempo={(duration/57):.5f}', outputFile])
+        else:
+            subprocess.run(['ffmpeg', '-i', tempAudioPath, outputFile])
     else:
-        subprocess.run(['ffmpeg', '-i', tempAudioPath, outputFile])
-    if(os.path.exists(outputFile)):
+        subprocess.run(['ffmpeg', '-i', tempAudioPath, '-af', f'atempo={(duration/expected_duration):.5f}', outputFile])
+    if (os.path.exists(outputFile)):
         return outputFile
-    return ""
+
 
 def ChunkForAudio(alltext, chunk_size=2500):
     alltext_list = alltext.split('.')
     chunks = []
     curr_chunk = ''
     for text in alltext_list:
         if len(curr_chunk) + len(text) <= chunk_size:
@@ -48,22 +56,43 @@
         else:
             chunks.append(curr_chunk)
             curr_chunk = text + '.'
     if curr_chunk:
         chunks.append(curr_chunk)
     return chunks
 
-def audioToText(filename):
+
+def audioToText(filename, model_size="base"):
     from whisper_timestamped import load_model, transcribe_timestamped
     global WHISPER_MODEL
-    if(WHISPER_MODEL == None):
-        WHISPER_MODEL = load_model("tiny")
-    gen = transcribe_timestamped(WHISPER_MODEL, filename,verbose=False, fp16=False)
+    if (WHISPER_MODEL == None):
+        WHISPER_MODEL = load_model(model_size)
+    gen = transcribe_timestamped(WHISPER_MODEL, filename, verbose=False, fp16=False)
     return gen
 
+
 def getWordsPerSec(filename):
     a = audioToText(filename)
     return len(a['text'].split()) / a['segments'][-1]['end']
 
+
 def getCharactersPerSec(filename):
     a = audioToText(filename)
     return len(a['text']) / a['segments'][-1]['end']
+
+def run_background_audio_split(sound_file_path):
+    try:
+        # Run spleeter command
+        # Get absolute path of sound file 
+        output_dir = os.path.dirname(sound_file_path)
+        command = f"spleeter separate -p spleeter:2stems -o '{output_dir}' '{sound_file_path}'"
+
+        process = subprocess.run(command, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+
+        # If spleeter runs successfully, return the path to the background music file
+        if process.returncode == 0:
+            return os.path.join(output_dir, sound_file_path.split("/")[-1].split(".")[0], "accompaniment.wav")
+        else:
+            return None
+    except Exception:
+        # If spleeter crashes, return None
+        return None
```

### Comparing `ShortGPT-0.0.1/shortGPT/audio/eleven_voice_module.py` & `shortgpt-0.0.2/shortGPT/audio/eleven_voice_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from shortGPT.api_utils.eleven_api import generateVoice, getCharactersFromKey
+from shortGPT.api_utils.eleven_api import ElevenLabsAPI
 from shortGPT.audio.voice_module import VoiceModule
 
+
 class ElevenLabsVoiceModule(VoiceModule):
-    def __init__(self, api_key):
+    def __init__(self, api_key, voiceName, checkElevenCredits):
         self.api_key = api_key
+        self.voiceName = voiceName
         self.remaining_credits = None
+        self.eleven_labs_api = ElevenLabsAPI(self.api_key)
         self.update_usage()
-        if self.get_remaining_characters() < 1200:
+        if checkElevenCredits and self.get_remaining_characters() < 1200:
             raise Exception(f"Your ElevenLabs API KEY doesn't have enough credits ({self.remaining_credits} character remaining). Minimum required: 1200 characters (equivalent to a 45sec short)")
         super().__init__()
 
     def update_usage(self):
-        self.remaining_credits = getCharactersFromKey(self.api_key)
+        self.remaining_credits = self.eleven_labs_api.get_remaining_characters()
         return self.remaining_credits
 
     def get_remaining_characters(self):
-        return self.remaining_credits if self.remaining_credits else getCharactersFromKey(self.api_key)
+        return self.remaining_credits if self.remaining_credits else self.eleven_labs_api.get_remaining_characters()
 
-    def generate_voice(self, text, outputfile, character="Antoni"):
+    def generate_voice(self, text, outputfile):
         if self.get_remaining_characters() >= len(text):
-            file_path = generateVoice(text=text, character=character, fileName=outputfile, api_key=self.api_key)
+            file_path =self.eleven_labs_api.generate_voice(text=text, character=self.voiceName, filename=outputfile)
             self.update_usage()
             return file_path
         else:
-            raise Exception(f"You cannot generate {len(text)} characters as your ElevenLabs key has only {self.remaining_credits} characters remaining")
+            raise Exception(f"You cannot generate {len(text)} characters as your ElevenLabs key has only {self.remaining_credits} characters remaining")
```

### Comparing `ShortGPT-0.0.1/shortGPT/config/config.py` & `shortgpt-0.0.2/shortGPT/config/config.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/database/content_data_manager.py` & `shortgpt-0.0.2/shortGPT/database/content_data_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from shortGPT.database.db_document import DatabaseDocument
+from shortGPT.database.db_document import AbstractDatabaseDocument
+
+
 class ContentDataManager():
 
-    def __init__(self, db_doc: DatabaseDocument, content_type: str, new=False):
-        self.contentType= content_type
+    def __init__(self, db_doc: AbstractDatabaseDocument, content_type: str, new=False):
+        self.contentType = content_type
         self.db_doc = db_doc
         if new:
             self.db_doc._save({
                 'content_type': content_type,
                 'ready_to_upload': False,
                 'last_completed_step': 0,
             })
+
     def save(self, key, value):
         self.db_doc._save({key: value})
 
     def get(self, key):
         return self.db_doc._get(key)
-    
 
     def _getId(self):
         return self.db_doc._getId()
 
     def delete(self):
         self.db_doc.delete()
 
     def __str__(self):
-        return self.db_doc.__str__()
+        return self.db_doc.__str__()
```

### Comparing `ShortGPT-0.0.1/shortGPT/database/content_database.py` & `shortgpt-0.0.2/shortGPT/database/content_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from uuid import uuid4
 from shortGPT.database.db_document import TINY_MONGO_DATABASE, TinyMongoDocument
 
 from shortGPT.database.content_data_manager import ContentDataManager
 class ContentDatabase:
     def __init__(self, ):
-        self.shorts_collections = TINY_MONGO_DATABASE["content_db"]["content_documents"]
+        self.content_collection = TINY_MONGO_DATABASE["content_db"]["content_documents"]
 
     def instanciateContentDataManager(self, id: str, content_type: str, new=False):
         db_doc = TinyMongoDocument("content_db", "content_documents", id)
         return ContentDataManager(db_doc, content_type, new)
 
     def getContentDataManager(self, id, content_type: str):
         try:
```

### Comparing `ShortGPT-0.0.1/shortGPT/database/db_document.py` & `shortgpt-0.0.2/shortGPT/database/db_document.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,119 @@
-import tinymongo as tm
-import tinydb
+import threading
 from abc import ABC, abstractmethod
 
-class DatabaseDocument(ABC):
-    
+import tinydb
+import tinymongo as tm
+
+
+class AbstractDatabaseDocument(ABC):
+
     @abstractmethod
     def _save(self, key, data):
+        '''Save the data in the database'''
         pass
 
     @abstractmethod
     def _get(self, key):
+        '''Get the data from the database'''
         pass
 
     @abstractmethod
     def _getId(self):
+        '''Get the id of the document'''
         pass
-    
+
     @abstractmethod
     def __str__(self):
+        '''Return the string representation of the document'''
         pass
 
     @abstractmethod
     def _delete(self):
+        '''Delete the document'''
         pass
 
 
 class TinyMongoClient(tm.TinyMongoClient):
     @property
     def _storage(self):
         return tinydb.storages.JSONStorage
 
+
 TINY_MONGO_DATABASE = TinyMongoClient("./.database")
 
-class TinyMongoDocument(DatabaseDocument):
+
+class TinyMongoDocument(AbstractDatabaseDocument):
+    _lock = threading.Lock()
 
     def __init__(self, db_name: str, collection_name: str, document_id: str, create=False):
         self.collection = TINY_MONGO_DATABASE[db_name][collection_name]
         self.collection_name = collection_name
         self.document_id = document_id
-        if(not self.exists()):
+        if (not self.exists()):
             if create:
                 self.collection.insert_one({"_id": document_id})
             else:
                 raise Exception(f"The document with id {document_id} in collection {collection_name} of database {db_name} does not exist")
 
     def exists(self):
-        return self.collection.find({"_id": self.document_id}).count() == 1
+        with self._lock:
+            return self.collection.find({"_id": self.document_id}).count() == 1
 
     def _save(self, data):
-        try:    
-            update_data = {'$set': {}}
-            for key, value in data.items():
-                path_parts = key.split(".")
-                
-                if len(path_parts) > 1:
-                    root_key = ".".join(path_parts[:-1])
-                    last_key = path_parts[-1]
-                    current_value = self._get(root_key)
-                    if not isinstance(current_value, dict):
-                        current_value = {}
-                    current_value[last_key] = value
-                    update_data['$set'][root_key] = current_value
-                else:
-                    update_data['$set'][key] = value
-
-            self.collection.update_one({'_id': self.document_id}, update_data)
-        except Exception as e:
-            print(f"Error saving data: {e}")
-
+        with self._lock:
+            try:
+                update_data = {'$set': {}}
+                for key, value in data.items():
+                    path_parts = key.split(".")
+
+                    if len(path_parts) > 1:
+                        root_key = ".".join(path_parts[:-1])
+                        last_key = path_parts[-1]
+                        current_value = self._get(root_key)
+                        if not isinstance(current_value, dict):
+                            current_value = {}
+                        current_value[last_key] = value
+                        update_data['$set'][root_key] = current_value
+                    else:
+                        update_data['$set'][key] = value
+
+                self.collection.update_one({'_id': self.document_id}, update_data)
+            except Exception as e:
+                print(f"Error saving data: {e}")
 
     def _get(self, key=None):
-        try:
-            document = self.collection.find_one({'_id': self.document_id})
-            if not key:
-                del document['_id']
-                return document
-            keys = key.split(".")
-            value = document[keys[0]]
-            for k in keys[1:]:
-                value = value[k]
-            return value
-        except Exception as e:
-            return None
-            #print(f"Error getting value for key '{key}': {e}")
-            
+        with self._lock:
+            try:
+                document = self.collection.find_one({'_id': self.document_id})
+                if not key:
+                    del document['_id']
+                    return document
+                keys = key.split(".")
+                value = document[keys[0]]
+                for k in keys[1:]:
+                    value = value[k]
+                return value
+            except Exception as e:
+                #print(f"Error getting value for key '{key}': {e}")
+                return None
+
     def _delete(self, key):
-        try:
-            document = self.collection.find_one({'_id': self.document_id})
-            if key in document:
-                del document[key]
-                self.collection.remove({'_id': self.document_id})
-                self.collection.insert(document)
-            else:
-                print(f"Key '{key}' not found in the document")
-        except Exception as e:
-            print(f"Error deleting key '{key}': {e}")
+        with self._lock:
+            try:
+                document = self.collection.find_one({'_id': self.document_id})
+                if key in document:
+                    del document[key]
+                    self.collection.remove({'_id': self.document_id})
+                    self.collection.insert(document)
+                else:
+                    print(f"Key '{key}' not found in the document")
+            except Exception as e:
+                print(f"Error deleting key '{key}': {e}")
+
     def _getId(self):
         return self.document_id
 
-
     def __str__(self):
-        document = self.collection.find_one({'_id': self.document_id})
-        return str(document)
+        with self._lock:
+            document = self.collection.find_one({'_id': self.document_id})
+            return str(document)
```

### Comparing `ShortGPT-0.0.1/shortGPT/editing_utils/captions.py` & `shortgpt-0.0.2/shortGPT/editing_utils/captions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,71 @@
 import re
 
+def getSpeechBlocks(whispered, silence_time=2):
+    text_blocks, (st, et, txt) = [], (0,0,"")
+    for i, seg in enumerate(whispered['segments']):
+        if seg['start'] - et > silence_time:
+            if txt: text_blocks.append([[st, et], txt])
+            (st, et, txt) = (seg['start'], seg['end'], seg['text'])
+        else: 
+            et, txt = seg['end'], txt + seg['text']
+
+    if txt: text_blocks.append([[st, et], txt]) # For last text block
+
+    return text_blocks
+
+def cleanWord(word):
+    return re.sub(r'[^\w\s\-_"\'\']', '', word)
+
 def interpolateTimeFromDict(word_position, d):
     for key, value in d.items():
         if key[0] <= word_position <= key[1]:
             return value
     return None
 
-def cleanWord(word):
-    return re.sub(r'[^\w\s]', '', word)
-
 def getTimestampMapping(whisper_analysis):
     index = 0
     locationToTimestamp = {}
     for segment in whisper_analysis['segments']:
         for word in segment['words']:
             newIndex = index + len(word['text'])+1
             locationToTimestamp[(index, newIndex)] = word['end']
             index = newIndex
     return locationToTimestamp
 
+
 def splitWordsBySize(words, maxCaptionSize):
+    halfCaptionSize = maxCaptionSize / 2
     captions = []
-    i = 0
-    while i < len(words):
-        caption = words[i]
-        while i + 1 < len(words) and len(caption + ' ' + words[i + 1]) <= maxCaptionSize:
-            i += 1
-            caption += ' ' + words[i]
+    while words:
+        caption = words[0]
+        words = words[1:]
+        while words and len(caption + ' ' + words[0]) <= maxCaptionSize:
+            caption += ' ' + words[0]
+            words = words[1:]
+            if len(caption) >= halfCaptionSize and words:
+                break
         captions.append(caption)
-        i += 1
     return captions
-def getCaptionsWithTime(whisper_analysis, maxCaptionSize=15):
+
+def getCaptionsWithTime(whisper_analysis, maxCaptionSize=15, considerPunctuation=False):
     wordLocationToTime = getTimestampMapping(whisper_analysis)
     position = 0
     start_time = 0
     CaptionsPairs = []
-    words = whisper_analysis['text'].split()
-    split_captions = splitWordsBySize(words, maxCaptionSize)
-    for caption in split_captions:
-        position += len(caption) + 1
+    text = whisper_analysis['text']
+    
+    if considerPunctuation:
+        sentences = re.split(r'(?<=[.!?]) +', text)
+        words = [word for sentence in sentences for word in splitWordsBySize(sentence.split(), maxCaptionSize)]
+    else:
+        words = text.split()
+        words = [cleanWord(word) for word in splitWordsBySize(words, maxCaptionSize)]
+    
+    for word in words:
+        position += len(word) + 1
         end_time = interpolateTimeFromDict(position, wordLocationToTime)
-        if(end_time and caption):
-            CaptionsPairs.append(((start_time, end_time), cleanWord(caption)))
+        if end_time and word:
+            CaptionsPairs.append(((start_time, end_time), word))
             start_time = end_time
 
-    return CaptionsPairs
+    return CaptionsPairs
```

### Comparing `ShortGPT-0.0.1/shortGPT/editing_utils/editing_images.py` & `shortgpt-0.0.2/shortGPT/editing_utils/editing_images.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/editing_utils/handle_videos.py` & `shortgpt-0.0.2/shortGPT/editing_utils/handle_videos.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,33 @@
 import ffmpeg
 import os
 import random
 import yt_dlp
-def getYoutubeAudio(url):
-    ydl_opts = {
-    "quiet": True,
-    "no_warnings": True,
-    "no_color": True,
-    "no_call_home": True,
-    "no_check_certificate": True,
-    "format": "bestaudio/best"
-    }
-    try:
-        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-            dictMeta = ydl.extract_info(
-                url,
-                download=False)
-            return dictMeta['url'], dictMeta['duration']
-    except Exception as e:
-        print("Failed getting audio link from the following video/url", e.args[0])
-    return None
-
-def getYoutubeAudio(url):
-    ydl_opts = {
-    "quiet": True,
-    "no_warnings": True,
-    "no_color": True,
-    "no_call_home": True,
-    "no_check_certificate": True,
-    "format": "bestaudio/best"
-    }
-    try:
-        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-            dictMeta = ydl.extract_info(
-                url,
-                download=False)
-            return dictMeta['url'], dictMeta['duration']
-    except Exception as e:
-        print("Failed getting audio link from the following video/url", e.args[0])
-    return None
+import subprocess
+import json
 
 def getYoutubeVideoLink(url):
-    ydl_opts = {
+    if 'shorts' in url:
+        ydl_opts = {
+            "quiet": True,
+            "no_warnings": True,
+            "no_color": True,
+            "no_call_home": True,
+            "no_check_certificate": True,
+            "format": "bestvideo[height<=1920]"
+        }
+    else:
+        ydl_opts = {
         "quiet": True,
         "no_warnings": True,
         "no_color": True,
         "no_call_home": True,
         "no_check_certificate": True,
         "format": "bestvideo[height<=1080]"
-    }
+        }
     try:
         with yt_dlp.YoutubeDL(ydl_opts) as ydl:
             dictMeta = ydl.extract_info(
                 url,
                 download=False)
             return dictMeta['url'], dictMeta['duration']
     except Exception as e:
@@ -80,7 +55,34 @@
         .input(video_url, ss=start_time, t=clip_duration)
         .output(output_file, codec="libx264", preset="ultrafast")
         .run()
     )
     if not os.path.exists(output_file):
         raise Exception("Random clip failed to be written")
     return output_file
+
+
+def get_aspect_ratio(video_file):
+    cmd = 'ffprobe -i "{}" -v quiet -print_format json -show_format -show_streams'.format(video_file)
+#     jsonstr = subprocess.getoutput(cmd)
+    jsonstr = subprocess.check_output(cmd, shell=True, encoding='utf-8')
+    r = json.loads(jsonstr)
+    # look for "codec_type": "video". take the 1st one if there are mulitple
+    video_stream_info = [x for x in r['streams'] if x['codec_type']=='video'][0]
+    if 'display_aspect_ratio' in video_stream_info and video_stream_info['display_aspect_ratio']!="0:1":
+        a,b = video_stream_info['display_aspect_ratio'].split(':')
+        dar = int(a)/int(b)
+    else:
+        # some video do not have the info of 'display_aspect_ratio'
+        w,h = video_stream_info['width'], video_stream_info['height']
+        dar = int(w)/int(h)
+        ## not sure if we should use this
+        #cw,ch = video_stream_info['coded_width'], video_stream_info['coded_height']
+        #sar = int(cw)/int(ch)
+    if 'sample_aspect_ratio' in video_stream_info and video_stream_info['sample_aspect_ratio']!="0:1":
+        # some video do not have the info of 'sample_aspect_ratio'
+        a,b = video_stream_info['sample_aspect_ratio'].split(':')
+        sar = int(a)/int(b)
+    else:
+        sar = dar
+    par = dar/sar
+    return dar
```

### Comparing `ShortGPT-0.0.1/shortGPT/engine/abstract_content_engine.py` & `shortgpt-0.0.2/shortGPT/engine/abstract_content_engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,93 @@
-from shortGPT.audio.eleven_voice_module import ElevenLabsVoiceModule
-from shortGPT.config.asset_db import AssetDatabase
-from shortGPT.config.api_db import get_api_key
-from shortGPT.database.content_database import ContentDatabase
-from shortGPT.config.languages import Language
-from abc import ABC
 import os
+from abc import ABC
+
+from shortGPT.audio.voice_module import VoiceModule
+from shortGPT.config.languages import Language
+from shortGPT.config.path_utils import get_program_path
+from shortGPT.database.content_database import ContentDatabase
+
 CONTENT_DB = ContentDatabase()
 
+
 class AbstractContentEngine(ABC):
-    def __init__(self, short_id: str, content_type:str, language: Language):
+    def __init__(self, short_id: str, content_type: str, language: Language, voiceModule: VoiceModule):
         if short_id:
             self.dataManager = CONTENT_DB.getContentDataManager(
                 short_id, content_type
             )
         else:
             self.dataManager = CONTENT_DB.createContentDataManager(content_type)
         self.id = str(self.dataManager._getId())
+        self.initializeMagickAndFFMPEG()
         self.prepareEditingPaths()
         self._db_language = language.value
-        self.voiceModule = ElevenLabsVoiceModule(get_api_key("ELEVEN LABS"))
-        self.assetStore = AssetDatabase()
+        self.voiceModule = voiceModule
         self.stepDict = {}
         self.logger = lambda _: print(_)
 
     def __getattr__(self, name):
-            if name.startswith('_db_'):
-                db_path = name[4:]  # remove '_db_' prefix
-                cache_attr = '_' + name
-                if not hasattr(self, cache_attr):
-                    setattr(self, cache_attr, self.dataManager.get(db_path))
-                return getattr(self, cache_attr)
-            else:
-                return super().__getattr__(name)
+        if name.startswith('_db_'):
+            db_path = name[4:]  # remove '_db_' prefix
+            cache_attr = '_' + name
+            if not hasattr(self, cache_attr):
+                setattr(self, cache_attr, self.dataManager.get(db_path))
+            return getattr(self, cache_attr)
+        else:
+            return super().__getattr__(name)
 
     def __setattr__(self, name, value):
         if name.startswith('_db_'):
             db_path = name[4:]  # remove '_db_' prefix
             cache_attr = '_' + name
             setattr(self, cache_attr, value)
             self.dataManager.save(db_path, value)
         else:
             super().__setattr__(name, value)
-    
+
     def prepareEditingPaths(self):
         self.dynamicAssetDir = f".editing_assets/{self.dataManager.contentType}_assets/{self.id}/"
         if not os.path.exists(self.dynamicAssetDir):
             os.makedirs(self.dynamicAssetDir)
 
     def verifyParameters(*args, **kargs):
         keys = list(kargs.keys())
         for key in keys:
             if not kargs[key]:
                 print(kargs)
                 raise Exception(f"Parameter :{key} is null")
-            
+
     def isShortDone(self):
         return self._db_ready_to_upload
 
-    def makeShort(self):
+    def makeContent(self):
         while (not self.isShortDone()):
             currentStep = self._db_last_completed_step + 1
             if currentStep not in self.stepDict:
                 raise Exception(f'Incorrect step {currentStep}')
-            if  self.stepDict[currentStep].__name__ == "_editAndRenderShort":
+            if self.stepDict[currentStep].__name__ == "_editAndRenderShort":
                 yield currentStep, f'Current step ({currentStep} / {self.get_total_steps()}) : ' + "Preparing rendering assets..."
             else:
                 yield currentStep, f'Current step ({currentStep} / {self.get_total_steps()}) : ' + self.stepDict[currentStep].__name__
             print(f'Step {currentStep} {self.stepDict[currentStep].__name__}')
             self.stepDict[currentStep]()
             self._db_last_completed_step = currentStep
 
     def get_video_output_path(self):
         return self._db_video_path
-    
+
     def get_total_steps(self):
         return len(self.stepDict)
-    
-    def set_logger(self,logger):
-        self.logger = logger
+
+    def set_logger(self, logger):
+        self.logger = logger
+
+    def initializeMagickAndFFMPEG(self):
+        ffmpeg_path = get_program_path("ffmpeg")
+        if not ffmpeg_path:
+            raise Exception("FFmpeg, a program used for automated editing within ShortGPT was not found on your computer. Please go back to the README and follow the instructions to install FFMPEG")
+        ffprobe_path = get_program_path("ffprobe")
+        if not ffprobe_path:
+            raise Exception("FFProbe, a dependecy of FFmpeg was not found. Please go back to the README and follow the instructions to install FFMPEG")
+        convert_path = get_program_path("convert")
+        if not convert_path:
+            raise Exception("ImageMagick, a program required for making Captions with ShortGPT was not found on your computer. Please go back to the README and follow the instructions to install ImageMagick")
```

### Comparing `ShortGPT-0.0.1/shortGPT/engine/content_short_engine.py` & `shortgpt-0.0.2/shortGPT/engine/content_short_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from shortGPT.audio.audio_duration import getAssetDuration
-from shortGPT.gpt import  gpt_editing, gpt_translate, gpt_yt
+import datetime
+import os
+import re
+import shutil
+from abc import abstractmethod
+
 from shortGPT.audio import audio_utils
+from shortGPT.audio.audio_duration import get_asset_duration
+from shortGPT.audio.voice_module import VoiceModule
+from shortGPT.config.asset_db import AssetDatabase
+from shortGPT.config.languages import Language
+from shortGPT.editing_framework.editing_engine import (EditingEngine,
+                                                       EditingStep)
 from shortGPT.editing_utils import captions, editing_images
 from shortGPT.editing_utils.handle_videos import extract_random_clip_from_video
 from shortGPT.engine.abstract_content_engine import AbstractContentEngine
-from shortGPT.config.languages import Language
-from shortGPT.editing_framework.editing_engine import EditingEngine, EditingStep
-from abc import  abstractmethod
-import re
-import shutil
-import os
-import datetime
+from shortGPT.gpt import gpt_editing, gpt_translate, gpt_yt
+
 
 class ContentShortEngine(AbstractContentEngine):
 
-    def __init__(self, short_type: str, background_video_name: str, background_music_name: str,short_id="",
-                 num_images=None, watermark=None, language:Language = Language.ENGLISH):
-        super().__init__(short_id, short_type, language)
-        if (num_images):
-            self._db_num_images = num_images
-        if (watermark):
-            self._db_watermark = watermark
-        self._db_background_video_name = background_video_name
-        self._db_background_music_name = background_music_name
-        
+    def __init__(self, short_type: str, background_video_name: str, background_music_name: str, voiceModule: VoiceModule, short_id="",
+                 num_images=None, watermark=None, language: Language = Language.ENGLISH,):
+        super().__init__(short_id, short_type, language, voiceModule)
+        if not short_id:
+            if (num_images):
+                self._db_num_images = num_images
+            if (watermark):
+                self._db_watermark = watermark
+            self._db_background_video_name = background_video_name
+            self._db_background_music_name = background_music_name
+
         self.stepDict = {
             1:  self._generateScript,
             2:  self._generateTempAudio,
             3:  self._speedUpAudio,
             4:  self._timeCaptions,
             5:  self._generateImageSearchTerms,
             6:  self._generateImageUrls,
             7:  self._chooseBackgroundMusic,
             8:  self._chooseBackgroundVideo,
             9:  self._prepareBackgroundAssets,
             10: self._prepareCustomAssets,
             11: self._editAndRenderShort,
             12: self._addYoutubeMetadata
         }
-    
+
     @abstractmethod
     def _generateScript(self):
         self._db_script = ""
 
-
     def _generateTempAudio(self):
         if not self._db_script:
             raise NotImplementedError("generateScript method must set self._db_script.")
         if (self._db_temp_audio_path):
             return
         self.verifyParameters(text=self._db_script)
-        if not self._db_voice_character:
-            if (self._db_voice_gender == 'male'):
-                self._db_voice_character = "Antoni"
-            else:
-                self._db_voice_character = "Bella"
         script = self._db_script
         if (self._db_language != Language.ENGLISH.value):
             self._db_translated_script = gpt_translate.translateContent(script, self._db_language)
             script = self._db_translated_script
         self._db_temp_audio_path = self.voiceModule.generate_voice(
-            script, self.dynamicAssetDir + "temp_audio_path.wav", self._db_voice_character)
+            script, self.dynamicAssetDir + "temp_audio_path.wav")
 
     def _speedUpAudio(self):
         if (self._db_audio_path):
             return
         self.verifyParameters(tempAudioPath=self._db_temp_audio_path)
         self._db_audio_path = audio_utils.speedUpAudio(
             self._db_temp_audio_path, self.dynamicAssetDir+"audio_voice.wav")
@@ -83,47 +83,46 @@
 
     def _generateImageUrls(self):
         if self._db_timed_image_searches:
             self._db_timed_image_urls = editing_images.getImageUrlsTimed(
                 self._db_timed_image_searches)
 
     def _chooseBackgroundMusic(self):
-        self._db_background_music_url = self.assetStore.getAssetLink(self._db_background_music_name)
+        self._db_background_music_url = AssetDatabase.get_asset_link(self._db_background_music_name)
 
     def _chooseBackgroundVideo(self):
-        self._db_background_video_url = self.assetStore.getAssetLink(
+        self._db_background_video_url = AssetDatabase.get_asset_link(
             self._db_background_video_name)
-        self._db_background_video_duration = self.assetStore.getAssetDuration(
+        self._db_background_video_duration = AssetDatabase.get_asset_duration(
             self._db_background_video_name)
 
     def _prepareBackgroundAssets(self):
         self.verifyParameters(
-                              voiceover_audio_url=self._db_audio_path,
-                              video_duration=self._db_background_video_duration,
-                              background_video_url=self._db_background_video_url, music_url=self._db_background_music_url)
+            voiceover_audio_url=self._db_audio_path,
+            video_duration=self._db_background_video_duration,
+            background_video_url=self._db_background_video_url, music_url=self._db_background_music_url)
         if not self._db_voiceover_duration:
             self.logger("Rendering short: (1/4) preparing voice asset...")
-            self._db_audio_path, self._db_voiceover_duration = getAssetDuration(
+            self._db_audio_path, self._db_voiceover_duration = get_asset_duration(
                 self._db_audio_path, isVideo=False)
         if not self._db_background_trimmed:
             self.logger("Rendering short: (2/4) preparing background video asset...")
             self._db_background_trimmed = extract_random_clip_from_video(
                 self._db_background_video_url, self._db_background_video_duration, self._db_voiceover_duration, self.dynamicAssetDir + "clipped_background.mp4")
-      
+
     def _prepareCustomAssets(self):
         self.logger("Rendering short: (3/4) preparing custom assets...")
         pass
-    
 
     def _editAndRenderShort(self):
         self.verifyParameters(
-                              voiceover_audio_url=self._db_audio_path,
-                              video_duration=self._db_background_video_duration, 
-                              music_url=self._db_background_music_url)
-        
+            voiceover_audio_url=self._db_audio_path,
+            video_duration=self._db_background_video_duration,
+            music_url=self._db_background_music_url)
+
         outputPath = self.dynamicAssetDir+"rendered_video.mp4"
         if not (os.path.exists(outputPath)):
             self.logger("Rendering short: Starting automated editing...")
             videoEditor = EditingEngine()
             videoEditor.addEditingStep(EditingStep.ADD_VOICEOVER_AUDIO, {
                                        'url': self._db_audio_path})
             videoEditor.addEditingStep(EditingStep.ADD_BACKGROUND_MUSIC, {'url': self._db_background_music_url,
@@ -132,32 +131,32 @@
             videoEditor.addEditingStep(EditingStep.CROP_1920x1080, {
                                        'url': self._db_background_trimmed})
             videoEditor.addEditingStep(EditingStep.ADD_SUBSCRIBE_ANIMATION)
 
             if self._db_watermark:
                 videoEditor.addEditingStep(EditingStep.ADD_WATERMARK, {
                                            'text': self._db_watermark})
-            
-            caption_type = EditingStep.ADD_CAPTION_SHORT_ARABIC if self._db_language == Language.ARABIC.value else EditingStep.ADD_CAPTION_SHORT 
+
+            caption_type = EditingStep.ADD_CAPTION_SHORT_ARABIC if self._db_language == Language.ARABIC.value else EditingStep.ADD_CAPTION_SHORT
             for timing, text in self._db_timed_captions:
                 videoEditor.addEditingStep(caption_type, {'text': text.upper(),
-                                                                     'set_time_start': timing[0],
-                                                                     'set_time_end': timing[1]})
+                                                          'set_time_start': timing[0],
+                                                          'set_time_end': timing[1]})
             if self._db_num_images:
                 for timing, image_url in self._db_timed_image_urls:
                     videoEditor.addEditingStep(EditingStep.SHOW_IMAGE, {'url': image_url,
                                                                         'set_time_start': timing[0],
                                                                         'set_time_end': timing[1]})
 
             videoEditor.renderVideo(outputPath, logger=self.logger)
 
         self._db_video_path = outputPath
 
     def _addYoutubeMetadata(self):
-        
+
         self._db_yt_title, self._db_yt_description = gpt_yt.generate_title_description_dict(self._db_script)
 
         now = datetime.datetime.now()
         date_str = now.strftime("%Y-%m-%d_%H-%M-%S")
         newFileName = f"videos/{date_str} - " + \
             re.sub(r"[^a-zA-Z0-9 '\n\.]", '', self._db_yt_title)
```

### Comparing `ShortGPT-0.0.1/shortGPT/engine/content_video_engine.py` & `shortgpt-0.0.2/shortGPT/engine/content_video_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,71 @@
+import datetime
+import os
+import re
+import shutil
+
 from shortGPT.api_utils.pexels_api import getBestVideo
-from shortGPT.audio.audio_duration import getAssetDuration
-from shortGPT.gpt import  gpt_editing, gpt_translate, gpt_yt
 from shortGPT.audio import audio_utils
+from shortGPT.audio.audio_duration import get_asset_duration
+from shortGPT.audio.voice_module import VoiceModule
+from shortGPT.config.asset_db import AssetDatabase
+from shortGPT.config.languages import Language
+from shortGPT.editing_framework.editing_engine import (EditingEngine,
+                                                       EditingStep)
 from shortGPT.editing_utils import captions
 from shortGPT.engine.abstract_content_engine import AbstractContentEngine
-from shortGPT.config.languages import Language
-from shortGPT.editing_framework.editing_flow import EditingEngine, EditingStep
-import re
-import shutil
-import os
-import datetime
+from shortGPT.gpt import gpt_editing, gpt_translate, gpt_yt
+
 
 class ContentVideoEngine(AbstractContentEngine):
 
-    def __init__(self, script: str, background_music_name="",id="",
-     watermark=None,isVerticalFormat=False, language:Language = Language.ENGLISH):
-        super().__init__(id, "general_video", language)
+    def __init__(self, voiceModule: VoiceModule, script: str, background_music_name="", id="",
+                 watermark=None, isVerticalFormat=False, language: Language = Language.ENGLISH):
+        super().__init__(id, "general_video", language, voiceModule)
         if not id:
             if (watermark):
                 self._db_watermark = watermark
             if background_music_name:
                 self._db_background_music_name = background_music_name
             self._db_script = script
             self._db_format_vertical = isVerticalFormat
-        
+
         self.stepDict = {
             1:  self._generateTempAudio,
             2:  self._speedUpAudio,
             3:  self._timeCaptions,
             4:  self._generateVideoSearchTerms,
             5:  self._generateVideoUrls,
             6:  self._chooseBackgroundMusic,
             7:  self._prepareBackgroundAssets,
             8: self._prepareCustomAssets,
             9: self._editAndRenderShort,
             10: self._addMetadata
         }
-    
-
 
     def _generateTempAudio(self):
         if not self._db_script:
             raise NotImplementedError("generateScript method must set self._db_script.")
         if (self._db_temp_audio_path):
             return
         self.verifyParameters(text=self._db_script)
-        if not self._db_voice_character:
-            if (self._db_voice_gender == 'male'):
-                self._db_voice_character = "Antoni"
-            else:
-                self._db_voice_character = "Bella"
         script = self._db_script
         if (self._db_language != Language.ENGLISH.value):
             self._db_translated_script = gpt_translate.translateContent(script, self._db_language)
             script = self._db_translated_script
         self._db_temp_audio_path = self.voiceModule.generate_voice(
-            script, self.dynamicAssetDir + "temp_audio_path.wav", self._db_voice_character)
+            script, self.dynamicAssetDir + "temp_audio_path.wav")
 
     def _speedUpAudio(self):
         if (self._db_audio_path):
             return
         self.verifyParameters(tempAudioPath=self._db_temp_audio_path)
+        # Since the video is not supposed to be a short( less than 60sec), there is no reason to speed it up
+        self._db_audio_path = self._db_temp_audio_path
+        return
         self._db_audio_path = audio_utils.speedUpAudio(
             self._db_temp_audio_path, self.dynamicAssetDir+"audio_voice.wav")
 
     def _timeCaptions(self):
         self.verifyParameters(audioPath=self._db_audio_path)
         whisper_analysis = audio_utils.audioToText(self._db_audio_path)
         max_len = 15
@@ -82,72 +83,70 @@
         timed_video_searches = self._db_timed_video_searches
         self.verifyParameters(captionsTimed=timed_video_searches)
         timed_video_urls = []
         used_links = []
         for (t1, t2), search_terms in timed_video_searches:
             url = ""
             for query in reversed(search_terms):
-                url = getBestVideo(query,orientation_landscape= not self._db_format_vertical, used_vids=used_links)
+                url = getBestVideo(query, orientation_landscape=not self._db_format_vertical, used_vids=used_links)
                 if url:
                     used_links.append(url.split('.hd')[0])
                     break
-            timed_video_urls.append([[t1,t2], url])
+            timed_video_urls.append([[t1, t2], url])
         self._db_timed_video_urls = timed_video_urls
 
-
     def _chooseBackgroundMusic(self):
         if self._db_background_music_name:
-            self._db_background_music_url = self.assetStore.getAssetLink(self._db_background_music_name)
+            self._db_background_music_url = AssetDatabase.get_asset_link(self._db_background_music_name)
 
     def _prepareBackgroundAssets(self):
         self.verifyParameters(voiceover_audio_url=self._db_audio_path)
         if not self._db_voiceover_duration:
             self.logger("Rendering short: (1/4) preparing voice asset...")
-            self._db_audio_path, self._db_voiceover_duration = getAssetDuration(
+            self._db_audio_path, self._db_voiceover_duration = get_asset_duration(
                 self._db_audio_path, isVideo=False)
 
     def _prepareCustomAssets(self):
         self.logger("Rendering short: (3/4) preparing custom assets...")
         pass
-    
 
     def _editAndRenderShort(self):
         self.verifyParameters(
-                              voiceover_audio_url=self._db_audio_path)
-        
+            voiceover_audio_url=self._db_audio_path)
+
         outputPath = self.dynamicAssetDir+"rendered_video.mp4"
         if not (os.path.exists(outputPath)):
             self.logger("Rendering short: Starting automated editing...")
             videoEditor = EditingEngine()
             videoEditor.addEditingStep(EditingStep.ADD_VOICEOVER_AUDIO, {
                                        'url': self._db_audio_path})
             if (self._db_background_music_url):
                 videoEditor.addEditingStep(EditingStep.ADD_BACKGROUND_MUSIC, {'url': self._db_background_music_url,
-                                                                            'loop_background_music': self._db_voiceover_duration,
-                                                                            "volume_percentage": 0.08})
+                                                                              'loop_background_music': self._db_voiceover_duration,
+                                                                              "volume_percentage": 0.08})
             for (t1, t2), video_url in self._db_timed_video_urls:
                 videoEditor.addEditingStep(EditingStep.ADD_BACKGROUND_VIDEO, {'url': video_url,
-                                                                     'set_time_start': t1,
-                                                                     'set_time_end': t2})
+                                                                              'set_time_start': t1,
+                                                                              'set_time_end': t2})
             if (self._db_format_vertical):
-                caption_type = EditingStep.ADD_CAPTION_SHORT_ARABIC if self._db_language == Language.ARABIC.value else EditingStep.ADD_CAPTION_SHORT 
+                caption_type = EditingStep.ADD_CAPTION_SHORT_ARABIC if self._db_language == Language.ARABIC.value else EditingStep.ADD_CAPTION_SHORT
             else:
-                caption_type = EditingStep.ADD_CAPTION_LANDSCAPE_ARABIC if self._db_language == Language.ARABIC.value else EditingStep.ADD_CAPTION_LANDSCAPE 
-            
+                caption_type = EditingStep.ADD_CAPTION_LANDSCAPE_ARABIC if self._db_language == Language.ARABIC.value else EditingStep.ADD_CAPTION_LANDSCAPE
+
             for (t1, t2), text in self._db_timed_captions:
                 videoEditor.addEditingStep(caption_type, {'text': text.upper(),
-                                                                     'set_time_start': t1,
-                                                                     'set_time_end': t2})
-    
+                                                          'set_time_start': t1,
+                                                          'set_time_end': t2})
+
             videoEditor.renderVideo(outputPath, logger=self.logger)
 
         self._db_video_path = outputPath
 
     def _addMetadata(self):
-        
+
         self._db_yt_title, self._db_yt_description = gpt_yt.generate_title_description_dict(self._db_script)
 
         now = datetime.datetime.now()
         date_str = now.strftime("%Y-%m-%d_%H-%M-%S")
         newFileName = f"videos/{date_str} - " + \
             re.sub(r"[^a-zA-Z0-9 '\n\.]", '', self._db_yt_title)
```

### Comparing `ShortGPT-0.0.1/shortGPT/engine/facts_short_engine.py` & `shortgpt-0.0.2/shortGPT/engine/facts_short_engine.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from shortGPT.audio.voice_module import VoiceModule
 from shortGPT.gpt import facts_gpt
 from shortGPT.config.languages import Language
 from shortGPT.engine.content_short_engine import ContentShortEngine
 
 
 class FactsShortEngine(ContentShortEngine):
 
-    def __init__(self, facts_type: str, background_video_name: str, background_music_name: str,short_id="",
+    def __init__(self, voiceModule: VoiceModule, facts_type: str, background_video_name: str, background_music_name: str,short_id="",
                  num_images=None, watermark=None, language:Language = Language.ENGLISH):
         super().__init__(short_id=short_id, short_type="facts_shorts", background_video_name=background_video_name, background_music_name=background_music_name,
-                 num_images=num_images, watermark=watermark, language=language)
+                 num_images=num_images, watermark=watermark, language=language, voiceModule=voiceModule)
         
         self._db_facts_type = facts_type
 
     def _generateScript(self):
         """
         Implements Abstract parent method to generate the script for the Facts short.
         """
```

### Comparing `ShortGPT-0.0.1/shortGPT/engine/reddit_short_engine.py` & `shortgpt-0.0.2/shortGPT/engine/reddit_short_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from shortGPT.audio.voice_module import VoiceModule
 from shortGPT.config.languages import Language
 from shortGPT.engine.content_short_engine import ContentShortEngine
-from shortGPT.editing_framework.editing_flow import EditingEngine, EditingStep, Flow
+from shortGPT.editing_framework.editing_engine import EditingEngine, EditingStep, Flow
 from shortGPT.gpt import reddit_gpt, gpt_voice
 import os
 
 
 class RedditShortEngine(ContentShortEngine):
     # Mapping of variable names to database paths
-    def __init__(self, background_video_name: str, background_music_name: str,short_id="",
+    def __init__(self,voiceModule: VoiceModule, background_video_name: str, background_music_name: str,short_id="",
                  num_images=None, watermark=None, language:Language = Language.ENGLISH):
         super().__init__(short_id=short_id, short_type="reddit_shorts", background_video_name=background_video_name, background_music_name=background_music_name,
-                 num_images=num_images, watermark=watermark, language=language)
+                 num_images=num_images, watermark=watermark, language=language, voiceModule=voiceModule)
     
     def __generateRandomStory(self):
         question = reddit_gpt.getInterestingRedditQuestion()
         script = reddit_gpt.createRedditScript(question)
         return script
 
-    def __getRealisticStory(self, max_tries=6):
+    def __getRealisticStory(self, max_tries=3):
         current_realistic_score = 0
         current_try = 0
         current_generated_script = ""
         while (current_realistic_score < 6 and current_try < max_tries) or len(current_generated_script) > 1000:
             new_script = self.__generateRandomStory()
             new_realistic_score = reddit_gpt.getRealisticness(new_script)
             if new_realistic_score >= current_realistic_score:
@@ -31,19 +32,17 @@
         return current_generated_script, current_try
 
     def _generateScript(self):
         """
         Implements Abstract parent method to generate the script for the reddit short
         """
         self.logger("Generating reddit question & entertaining story")
-        self._db_script, _ = self.__getRealisticStory(max_tries=5)
+        self._db_script, _ = self.__getRealisticStory(max_tries=1)
         self._db_reddit_question = reddit_gpt.getQuestionFromThread(
             self._db_script)
-        self.logger("Choosing narration voice gender")
-        self._db_voice_gender = gpt_voice.getGenderFromText(self._db_script)
 
     def _prepareCustomAssets(self):
         """
         Override parent method to generate custom reddit image asset
         """
         self.logger("Rendering short: (3/4) preparing custom reddit image...")
         self.verifyParameters(question=self._db_reddit_question,)
```

### Comparing `ShortGPT-0.0.1/shortGPT/gpt/facts_gpt.py` & `shortgpt-0.0.2/shortGPT/gpt/facts_gpt.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/gpt/gpt_chat_video.py` & `shortgpt-0.0.2/shortGPT/gpt/gpt_chat_video.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/gpt/gpt_editing.py` & `shortgpt-0.0.2/shortGPT/gpt/gpt_editing.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/gpt/gpt_utils.py` & `shortgpt-0.0.2/shortGPT/gpt/gpt_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,101 @@
-import openai
-import yaml
+import json
 import os
-from time import time,sleep
 import re
+from time import sleep, time
+
+import openai
 import tiktoken
-import json
-from shortGPT.config.api_db import get_api_key
+import yaml
+
+from shortGPT.config.api_db import ApiKeyManager
+
 
 def num_tokens_from_messages(texts, model="gpt-3.5-turbo-0301"):
     """Returns the number of tokens used by a list of messages."""
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         encoding = tiktoken.get_encoding("cl100k_base")
     if model == "gpt-3.5-turbo-0301":  # note: future models may deviate from this
         if isinstance(texts, str):
             texts = [texts]
         score = 0
         for text in texts:
-            score+= 4 + len(encoding.encode(text))
+            score += 4 + len(encoding.encode(text))
         return score
     else:
         raise NotImplementedError(f"""num_tokens_from_messages() is not presently implemented for model {model}.
         See https://github.com/openai/openai-python/blob/main/chatml.md for information""")
 
+
 def extract_biggest_json(string):
     json_regex = r"\{(?:[^{}]|(?R))*\}"
     json_objects = re.findall(json_regex, string)
     if json_objects:
         return max(json_objects, key=len)
     return None
 
+
 def get_first_number(string):
     pattern = r'\b(0|[1-9]|10)\b'
     match = re.search(pattern, string)
     if match:
         return int(match.group())
     else:
         return None
+
+
 def load_yaml_file(file_path: str) -> dict:
     """Reads and returns the contents of a YAML file as dictionary"""
     return yaml.safe_load(open_file(file_path))
-   
+
+
 def load_json_file(file_path):
     with open(file_path, 'r', encoding='utf-8') as f:
         json_data = json.load(f)
     return json_data
 
+
 def load_yaml_prompt(file_path):
-    json_template= load_yaml_file(file_path)
+    json_template = load_yaml_file(file_path)
     return json_template['chat_prompt'], json_template['system_prompt']
 
+
 def open_file(filepath):
     with open(filepath, 'r', encoding='utf-8') as infile:
         return infile.read()
 
-def gpt3Turbo_completion(chat_prompt="", system="You are an AI that can give the answer to anything", temp=0.7, model="gpt-3.5-turbo", conversation=None):
-    openai.api_key = get_api_key("OPENAI")
+
+def gpt3Turbo_completion(chat_prompt="", system="You are an AI that can give the answer to anything", temp=0.7, model="gpt-3.5-turbo", max_tokens=1000, remove_nl=True, conversation=None):
+    openai.api_key = ApiKeyManager.get_api_key("OPENAI")
     max_retry = 5
     retry = 0
     while True:
         try:
             if conversation:
-                messages= conversation
+                messages = conversation
             else:
                 messages = [
-                {"role": "system", "content": system},
-                {"role": "user", "content": chat_prompt}
+                    {"role": "system", "content": system},
+                    {"role": "user", "content": chat_prompt}
                 ]
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=messages,
-                max_tokens=1000,
+                max_tokens=max_tokens,
                 temperature=temp)
             text = response['choices'][0]['message']['content'].strip()
-            text = re.sub('\s+', ' ', text)
+            if remove_nl:
+                text = re.sub('\s+', ' ', text)
             filename = '%s_gpt3.txt' % time()
             if not os.path.exists('.logs/gpt_logs'):
                 os.makedirs('.logs/gpt_logs')
             with open('.logs/gpt_logs/%s' % filename, 'w', encoding='utf-8') as outfile:
-                outfile.write(f"System prompt: ===\n{system}\n===\n"+f"Chat prompt: ===\n{chat_prompt}\n===\n"+ f'RESPONSE:\n====\n{text}\n===\n')
+                outfile.write(f"System prompt: ===\n{system}\n===\n"+f"Chat prompt: ===\n{chat_prompt}\n===\n" + f'RESPONSE:\n====\n{text}\n===\n')
             return text
         except Exception as oops:
             retry += 1
             if retry >= max_retry:
                 raise Exception("GPT3 error: %s" % oops)
             print('Error communicating with OpenAI:', oops)
             sleep(1)
-
-
```

### Comparing `ShortGPT-0.0.1/shortGPT/gpt/gpt_yt.py` & `shortgpt-0.0.2/shortGPT/gpt/gpt_yt.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     out = {"title": "", "description":""}
     chat, system = gpt_utils.load_yaml_prompt('shortGPT/prompt_templates/yt_title_description.yaml')
     chat = chat.replace("<<CONTENT>>", f"{content}")
     
     while out["title"] == "" or out["description"] == "":
         result = gpt_utils.gpt3Turbo_completion(chat_prompt=chat, system=system, temp=1)
         try:
-            response = json.loads(result.replace("'", '"'))
+            response = json.loads(result)
             if "title" in response:
                 out["title"] = response["title"]
             if "description" in response:
                 out["description"] = response["description"]
         except Exception as e:
             pass
         
-    return out['title'], out['description']
+    return out['title'], out['description']
```

### Comparing `ShortGPT-0.0.1/shortGPT/gpt/reddit_gpt.py` & `shortgpt-0.0.2/shortGPT/gpt/reddit_gpt.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/tracking/api_tracking.py` & `shortgpt-0.0.2/shortGPT/tracking/api_tracking.py`

 * *Files identical despite different names*

### Comparing `ShortGPT-0.0.1/shortGPT/tracking/cost_analytics.py` & `shortgpt-0.0.2/shortGPT/tracking/cost_analytics.py`

 * *Files identical despite different names*

