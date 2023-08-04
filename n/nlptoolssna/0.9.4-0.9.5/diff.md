# Comparing `tmp/nlptoolssna-0.9.4.tar.gz` & `tmp/nlptoolssna-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.9.4.tar", last modified: Mon Jun 19 12:49:39 2023, max compression
+gzip compressed data, was "nlptoolssna-0.9.5.tar", last modified: Fri Aug  4 14:55:09 2023, max compression
```

## Comparing `nlptoolssna-0.9.4.tar` & `nlptoolssna-0.9.5.tar`

### file list

```diff
@@ -1,105 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.672648 nlptoolssna-0.9.4/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-06-19 12:49:39.672648 nlptoolssna-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.537895 nlptoolssna-0.9.4/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.9.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.499403 nlptoolssna-0.9.4/docs/build/
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.499403 nlptoolssna-0.9.4/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.545879 nlptoolssna-0.9.4/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.4/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.547283 nlptoolssna-0.9.4/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.4/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.9.4/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.4/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.4/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.9.4/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.567382 nlptoolssna-0.9.4/docs/source/
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.567382 nlptoolssna-0.9.4/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.4/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.575654 nlptoolssna-0.9.4/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.577815 nlptoolssna-0.9.4/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.9.4/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.9.4/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.577815 nlptoolssna-0.9.4/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.9.4/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.9.4/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.585475 nlptoolssna-0.9.4/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.9.4/docs/source/api/utils/implication.rst
--rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.9.4/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.9.4/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.9.4/docs/source/api/utils/text_transliteration.rst
--rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.9.4/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.9.4/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.9.4/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.9.4/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.9.4/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.9.4/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.585475 nlptoolssna-0.9.4/nlptools/
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.595937 nlptoolssna-0.9.4/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.9.4/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     9187 2023-05-17 17:03:21.000000 nlptoolssna-0.9.4/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.9.4/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.595937 nlptoolssna-0.9.4/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.9.4/nlptools/arabiner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.604890 nlptoolssna-0.9.4/nlptools/arabiner/bin/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.4/nlptools/arabiner/bin/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-05-29 19:50:55.000000 nlptoolssna-0.9.4/nlptools/arabiner/bin/eval.py
--rw-rw-rw-   0        0        0     1549 2023-05-31 06:10:10.000000 nlptoolssna-0.9.4/nlptools/arabiner/bin/infer.py
--rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.9.4/nlptools/arabiner/bin/process.py
--rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.9.4/nlptools/arabiner/bin/train.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.612928 nlptoolssna-0.9.4/nlptools/arabiner/data/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.4/nlptools/arabiner/data/__init__.py
--rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.9.4/nlptools/arabiner/data/datasets.py
--rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.9.4/nlptools/arabiner/data/transforms.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.614448 nlptoolssna-0.9.4/nlptools/arabiner/nn/
--rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.9.4/nlptools/arabiner/nn/BaseModel.py
--rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.9.4/nlptools/arabiner/nn/BertNestedTagger.py
--rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.9.4/nlptools/arabiner/nn/BertSeqTagger.py
--rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.9.4/nlptools/arabiner/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.622844 nlptoolssna-0.9.4/nlptools/arabiner/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.4/nlptools/arabiner/utils/__init__.py
--rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.9.4/nlptools/arabiner/utils/data.py
--rw-rw-rw-   0        0        0     3720 2023-05-17 17:35:38.000000 nlptoolssna-0.9.4/nlptools/arabiner/utils/helpers.py
--rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.9.4/nlptools/arabiner/utils/metrics.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.622844 nlptoolssna-0.9.4/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.9.4/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.639059 nlptoolssna-0.9.4/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.9.4/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.9.4/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.9.4/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.9.4/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.9.4/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.643995 nlptoolssna-0.9.4/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.9.4/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    17930 2023-05-20 20:02:01.000000 nlptoolssna-0.9.4/nlptools/salma/views.py
--rw-rw-rw-   0        0        0     7719 2023-05-20 20:02:29.000000 nlptoolssna-0.9.4/nlptools/salma/wsd.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.653929 nlptoolssna-0.9.4/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.9.4/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0     4706 2023-05-29 19:21:39.000000 nlptoolssna-0.9.4/nlptools/utils/corpus.py
--rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.9.4/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0    10161 2023-06-05 13:27:15.000000 nlptoolssna-0.9.4/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     6144 2023-05-22 14:15:55.000000 nlptoolssna-0.9.4/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.9.4/nlptools/utils/text_transliteration.py
--rw-rw-rw-   0        0        0     1201 2023-05-29 19:17:26.000000 nlptoolssna-0.9.4/nlptools/utils/tokenizer.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.9.4/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.672648 nlptoolssna-0.9.4/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-06-19 12:49:39.000000 nlptoolssna-0.9.4/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2023-06-19 12:49:39.000000 nlptoolssna-0.9.4/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 12:49:39.000000 nlptoolssna-0.9.4/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-19 12:49:39.000000 nlptoolssna-0.9.4/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 12:49:39.000000 nlptoolssna-0.9.4/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       56 2023-06-19 12:49:39.000000 nlptoolssna-0.9.4/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 12:49:39.000000 nlptoolssna-0.9.4/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-06-19 12:49:39.681497 nlptoolssna-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     2105 2023-06-19 12:49:35.000000 nlptoolssna-0.9.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:39.672648 nlptoolssna-0.9.4/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.9.4/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.690560 nlptoolssna-0.9.5/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-08-04 14:55:09.691559 nlptoolssna-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.460745 nlptoolssna-0.9.5/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.9.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.389492 nlptoolssna-0.9.5/docs/build/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.390495 nlptoolssna-0.9.5/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.466768 nlptoolssna-0.9.5/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.5/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.481063 nlptoolssna-0.9.5/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.5/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.9.5/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.5/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.5/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.9.5/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.511996 nlptoolssna-0.9.5/docs/source/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.514987 nlptoolssna-0.9.5/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.5/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.532342 nlptoolssna-0.9.5/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.533662 nlptoolssna-0.9.5/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.9.5/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.9.5/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.397652 nlptoolssna-0.9.5/docs/source/api/arabiner/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.535667 nlptoolssna-0.9.5/docs/source/api/arabiner/bin/
+-rw-rw-rw-   0        0        0      217 2023-08-04 14:16:09.000000 nlptoolssna-0.9.5/docs/source/api/arabiner/bin/infer.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.536661 nlptoolssna-0.9.5/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.9.5/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.9.5/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.543665 nlptoolssna-0.9.5/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.9.5/docs/source/api/utils/implication.rst
+-rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.9.5/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.9.5/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.9.5/docs/source/api/utils/text_transliteration.rst
+-rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.9.5/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      199 2023-08-04 14:16:26.000000 nlptoolssna-0.9.5/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.9.5/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.9.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.9.5/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.9.5/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.557645 nlptoolssna-0.9.5/nlptools/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.566223 nlptoolssna-0.9.5/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.9.5/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     9253 2023-07-03 19:59:42.000000 nlptoolssna-0.9.5/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.9.5/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.571730 nlptoolssna-0.9.5/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.9.5/nlptools/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.587080 nlptoolssna-0.9.5/nlptools/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.5/nlptools/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-05-29 19:50:55.000000 nlptoolssna-0.9.5/nlptools/arabiner/bin/eval.py
+-rw-rw-rw-   0        0        0     1549 2023-05-31 06:10:10.000000 nlptoolssna-0.9.5/nlptools/arabiner/bin/infer.py
+-rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.9.5/nlptools/arabiner/bin/process.py
+-rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.9.5/nlptools/arabiner/bin/train.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.591080 nlptoolssna-0.9.5/nlptools/arabiner/data/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.5/nlptools/arabiner/data/__init__.py
+-rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.9.5/nlptools/arabiner/data/datasets.py
+-rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.9.5/nlptools/arabiner/data/transforms.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.606084 nlptoolssna-0.9.5/nlptools/arabiner/nn/
+-rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.9.5/nlptools/arabiner/nn/BaseModel.py
+-rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.9.5/nlptools/arabiner/nn/BertNestedTagger.py
+-rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.9.5/nlptools/arabiner/nn/BertSeqTagger.py
+-rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.9.5/nlptools/arabiner/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.616408 nlptoolssna-0.9.5/nlptools/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.5/nlptools/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.9.5/nlptools/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3720 2023-05-17 17:35:38.000000 nlptoolssna-0.9.5/nlptools/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.9.5/nlptools/arabiner/utils/metrics.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.617407 nlptoolssna-0.9.5/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.9.5/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.626522 nlptoolssna-0.9.5/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.9.5/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.9.5/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.9.5/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.9.5/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.9.5/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.639021 nlptoolssna-0.9.5/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.9.5/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 19:54:46.000000 nlptoolssna-0.9.5/nlptools/salma/settings.py
+-rw-rw-rw-   0        0        0    17631 2023-07-03 19:48:59.000000 nlptoolssna-0.9.5/nlptools/salma/views.py
+-rw-rw-rw-   0        0        0     7895 2023-07-03 20:03:19.000000 nlptoolssna-0.9.5/nlptools/salma/wsd.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.666904 nlptoolssna-0.9.5/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.9.5/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.9.5/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0    10161 2023-06-05 13:27:15.000000 nlptoolssna-0.9.5/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     6144 2023-05-22 14:15:55.000000 nlptoolssna-0.9.5/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.9.5/nlptools/utils/text_transliteration.py
+-rw-rw-rw-   0        0        0     1201 2023-05-29 19:17:26.000000 nlptoolssna-0.9.5/nlptools/utils/tokenizer.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.9.5/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.685455 nlptoolssna-0.9.5/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-08-04 14:55:08.000000 nlptoolssna-0.9.5/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2331 2023-08-04 14:55:09.000000 nlptoolssna-0.9.5/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:55:08.000000 nlptoolssna-0.9.5/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-08-04 14:55:08.000000 nlptoolssna-0.9.5/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 12:49:39.000000 nlptoolssna-0.9.5/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      144 2023-08-04 14:55:08.000000 nlptoolssna-0.9.5/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-04 14:55:08.000000 nlptoolssna-0.9.5/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-08-04 14:55:09.697651 nlptoolssna-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2023-08-04 14:52:51.000000 nlptoolssna-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:55:09.689557 nlptoolssna-0.9.5/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.9.5/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.9.4/CONTRIBUTING.rst` & `nlptoolssna-0.9.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/LICENSE` & `nlptoolssna-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/PKG-INFO` & `nlptoolssna-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.9.4/README.rst` & `nlptoolssna-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/docs/Makefile` & `nlptoolssna-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/docs/build/html/_images/download.png` & `nlptoolssna-0.9.5/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/docs/build/html/_static/download.png` & `nlptoolssna-0.9.5/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/docs/make.bat` & `nlptoolssna-0.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/docs/source/_static/download.png` & `nlptoolssna-0.9.5/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/docs/source/conf.py` & `nlptoolssna-0.9.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/docs/source/installation.rst` & `nlptoolssna-0.9.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.9.5/nlptools/DataDownload/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 import requests  
 import zipfile
 from tqdm import tqdm
 import tarfile
 urls = {
     'morph': 'https://portal.sina.birzeit.edu/ALMA27012000.pickle',
-    'ner': 'https://portal.sina.birzeit.edu/Wj27012000.tar.gz'
+    'ner': 'https://portal.sina.birzeit.edu/Wj27012000.tar.gz',
+    'salma' : 'http://portal.sina.birzeit.edu/SALMA27012000.zip'
 }
 
 #     'salma': 'http://portal.sina.birzeit.edu/SALMA27012000.zip',
 #     'salma2021': 'http://portal.sina.birzeit.edu/SALMA_v2.zip'
 #
```

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/bin/eval.py` & `nlptoolssna-0.9.5/nlptools/arabiner/bin/eval.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/bin/infer.py` & `nlptoolssna-0.9.5/nlptools/arabiner/bin/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/bin/process.py` & `nlptoolssna-0.9.5/nlptools/arabiner/bin/process.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/bin/train.py` & `nlptoolssna-0.9.5/nlptools/arabiner/bin/train.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/data/datasets.py` & `nlptoolssna-0.9.5/nlptools/arabiner/data/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/data/transforms.py` & `nlptoolssna-0.9.5/nlptools/arabiner/data/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/nn/BaseModel.py` & `nlptoolssna-0.9.5/nlptools/arabiner/nn/BaseModel.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/nn/BertNestedTagger.py` & `nlptoolssna-0.9.5/nlptools/arabiner/nn/BertNestedTagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/utils/data.py` & `nlptoolssna-0.9.5/nlptools/arabiner/utils/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/utils/helpers.py` & `nlptoolssna-0.9.5/nlptools/arabiner/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/arabiner/utils/metrics.py` & `nlptoolssna-0.9.5/nlptools/arabiner/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/data/my_data.pickle` & `nlptoolssna-0.9.5/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/morphology/charsets.py` & `nlptoolssna-0.9.5/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.9.5/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.9.5/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/salma/views.py` & `nlptoolssna-0.9.5/nlptools/salma/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 # ./bookstore_app/api/views.py
-import django
-django.setup()
-import requests
-import json
-from django.http import JsonResponse
-from rest_framework.decorators import api_view
-from salma import settings 
+
 # Comented by tymaa to Run service via GPU
 #from salma.word_sense_disambiguation import word_sense
 from salma.word_sense_disambiguation import normalizearabert
 from salma.word_sense_disambiguation import load_data_model
 from salma.word_sense_disambiguation import GlossPredictor
-from salma.parser import arStrip
-from salma.parser import removePunctuation
-from salma.parser import removeEnglish
-from salma.tokenizers_words import simple_word_tokenize
+from nlptools.utils.parser import arStrip
+from nlptools.utils.parser  import remove_punctuation
+from nlptools.utils.parser  import remove_latin
+from nlptools.utils.tokenizer import simple_word_tokenize
 from ALMA_multi_word_service.views import ALMA_multi_word
-import re
 import numpy as np
 from arabiner.bin import infer
-from api_clients_counter_month.ApikeyValidation import checkApikey
-from ApiTrackingService.InsertApiLog import insertLog
-import multiprocessing
+
 from functools import partial
 from lemmatizer_v2_DB.views import lemmatize_sentence
 from arabiner.views import NER
 
 # Added By Tymaa: 2023-02-05 to call GlossPredictor as a web service from GPU machine 
 #from urllib.request import Request, urlopen
```

### Comparing `nlptoolssna-0.9.4/nlptools/salma/wsd.py` & `nlptoolssna-0.9.5/nlptools/salma/wsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Comented by tymaa to Run service via GPU
 from nlptools.utils.implication import Implication
 from salma import settings 
 from pandas import read_excel, concat
 import re
 from transformers import BertTokenizer,BertForSequenceClassification
 from transformers import BertTokenizer,BertForSequenceClassification
-
+from nlptools.DataDownload import downloader
 import warnings
 warnings.filterwarnings("ignore")
 import torch
-
+import os
 import numpy as np
 
 import pandas as pd
 
 from arabert.preprocess import ArabertPreprocessor
 
 def word_sense(word, sentence):
@@ -25,14 +25,15 @@
 def normalizearabert(s):
   model_name = 'aubmindlab/bert-base-arabertv02'
   arabert_prep = ArabertPreprocessor(model_name.split("/")[-1])
   return arabert_prep.preprocess(str(s))
 
 
 def load_data_model():
+  
   file = './modern_examples4bert_true_v4_newcorrectData_BZUthes.xlsx'
   df = read_excel("{}".format(file))
   df['Example'] = df['Example'].apply(lambda x: str(x).upper())
   df['Example'] = df['Example'].apply(lambda x: re.sub(r'^((.?\[UNUSED0\].?){1})\[UNUSED0\]', r'\1[UNUSED1]', str(x)) )
 
   dftrain = df[df['Is_training'] == 1]
 
@@ -47,16 +48,19 @@
   # l.append("Target")
   # l.append("Example")
   # dftrue = "{}".format(l)
   # print("df :  \n ",dftrue)
 
 
 #   dftrue['Lemma'] = dftrue['Lemma'].apply(normalizearabert)
-  name = './bert-base-arabertv02_22_May_2021_00h_allglosses_unused01'
-  model = BertForSequenceClassification.from_pretrained('{}'.format(name),
+  filename = 'SALMA27012000'
+  path =downloader.get_appdatadir()
+  model_path = os.path.join(path, filename)
+  #name = './bert-base-arabertv02_22_May_2021_00h_allglosses_unused01'
+  model = BertForSequenceClassification.from_pretrained('{}'.format(model_path),
                                                         output_hidden_states = True,
                                                         num_labels=2
                                                         )
   tokenizer = BertTokenizer.from_pretrained('{}'.format('./bert-base-arabertv02'))
   tokenizer.add_special_tokens({ "additional_special_tokens": [ "[UNUSED0]" ] })
   tokenizer.add_special_tokens({ "additional_special_tokens": [ "[UNUSED1]" ] })
```

### Comparing `nlptoolssna-0.9.4/nlptools/utils/implication.py` & `nlptoolssna-0.9.5/nlptools/utils/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/utils/jaccard.py` & `nlptoolssna-0.9.5/nlptools/utils/jaccard.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/utils/parser.py` & `nlptoolssna-0.9.5/nlptools/utils/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/utils/text_transliteration.py` & `nlptoolssna-0.9.5/nlptools/utils/text_transliteration.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptools/utils/tokenizer.py` & `nlptoolssna-0.9.5/nlptools/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.9.5/nlptoolssna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.9.4/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.9.5/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/source/installation.rst
 docs/source/readme.rst
 docs/source/_static/download.png
 docs/source/api/DataDownload.rst
 docs/source/api/morphology.rst
 docs/source/api/utils.rst
 docs/source/api/DataDownload/downloader.rst
+docs/source/api/arabiner/bin/infer.rst
 docs/source/api/morphology/morph_analyzer.rst
 docs/source/api/utils/implication.rst
 docs/source/api/utils/jaccard.rst
 docs/source/api/utils/parser.rst
 docs/source/api/utils/text_transliteration.rst
 nlptools/__init__.py
 nlptools/cli.py
@@ -54,18 +55,18 @@
 nlptools/data/my_data.pickle
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
 nlptools/salma/__init__.py
+nlptools/salma/settings.py
 nlptools/salma/views.py
 nlptools/salma/wsd.py
 nlptools/utils/__init__.py
-nlptools/utils/corpus.py
 nlptools/utils/implication.py
 nlptools/utils/jaccard.py
 nlptools/utils/parser.py
 nlptools/utils/text_transliteration.py
 nlptools/utils/tokenizer.py
 nlptools/utils/utils.py
 nlptoolssna.egg-info/PKG-INFO
```

### Comparing `nlptoolssna-0.9.4/setup.cfg` & `nlptoolssna-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.4/setup.py` & `nlptoolssna-0.9.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 requirements = [
     'six',
     'farasapy',
     'tqdm',
     'requests',
     'regex',
     'pathlib',
-    # 'torch==1.13.0',
-    # 'transformers==4.24.0',
-    # 'torchtext==0.14.0',
-    # 'torchvision==0.14.0',
-    # 'seqeval==1.2.2',
+    'torch==1.13.0',
+    'transformers==4.24.0',
+    'torchtext==0.14.0',
+    'torchvision==0.14.0',
+    'seqeval==1.2.2',
     'natsort==7.1.1'
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Alaa' Omar",
```

