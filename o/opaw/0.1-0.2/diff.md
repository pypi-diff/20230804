# Comparing `tmp/opaw-0.1.tar.gz` & `tmp/opaw-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opaw-0.1.tar", last modified: Fri Aug  4 16:25:36 2023, max compression
+gzip compressed data, was "opaw-0.2.tar", last modified: Fri Aug  4 16:54:29 2023, max compression
```

## Comparing `opaw-0.1.tar` & `opaw-0.2.tar`

### file list

```diff
@@ -1,14 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:25:36.819760 opaw-0.1/
--rw-rw-rw-   0        0        0      405 2023-08-04 16:25:36.819760 opaw-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-08-04 14:53:26.000000 opaw-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 16:25:36.768845 opaw-0.1/opaw/
--rw-rw-rw-   0        0        0        0 2023-08-04 15:52:21.000000 opaw-0.1/opaw/__init__.py
--rw-rw-rw-   0        0        0       29 2023-08-03 17:18:41.000000 opaw-0.1/opaw/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:25:36.817475 opaw-0.1/opaw.egg-info/
--rw-rw-rw-   0        0        0      405 2023-08-04 16:25:36.000000 opaw-0.1/opaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-08-04 16:25:36.000000 opaw-0.1/opaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:25:36.000000 opaw-0.1/opaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 16:25:36.000000 opaw-0.1/opaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-04 16:25:36.000000 opaw-0.1/opaw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-08-04 16:25:36.822306 opaw-0.1/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-08-04 16:03:00.000000 opaw-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:54:29.940593 opaw-0.2/
+-rw-rw-rw-   0        0        0      405 2023-08-04 16:54:29.940593 opaw-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-08-04 14:53:26.000000 opaw-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 16:54:29.873618 opaw-0.2/opaw/
+-rw-rw-rw-   0        0        0        0 2023-08-04 15:52:21.000000 opaw-0.2/opaw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:54:29.914162 opaw-0.2/opaw/examples/
+-rw-rw-rw-   0        0        0        0 2023-08-04 16:15:43.000000 opaw-0.2/opaw/examples/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-08-04 16:11:30.000000 opaw-0.2/opaw/examples/audio.py
+-rw-rw-rw-   0        0        0      217 2023-08-04 16:11:30.000000 opaw-0.2/opaw/examples/basic.py
+-rw-rw-rw-   0        0        0      392 2023-08-04 16:11:30.000000 opaw-0.2/opaw/examples/chat.py
+-rw-rw-rw-   0        0        0      334 2023-08-04 16:20:25.000000 opaw-0.2/opaw/examples/completion.py
+-rw-rw-rw-   0        0        0      384 2023-08-04 16:20:25.000000 opaw-0.2/opaw/examples/edit.py
+-rw-rw-rw-   0        0        0      368 2023-08-04 16:20:25.000000 opaw-0.2/opaw/examples/embedding.py
+-rw-rw-rw-   0        0        0      588 2023-08-04 16:20:25.000000 opaw-0.2/opaw/examples/file.py
+-rw-rw-rw-   0        0        0      461 2023-08-04 16:20:25.000000 opaw-0.2/opaw/examples/finetune.py
+-rw-rw-rw-   0        0        0      625 2023-08-04 16:11:30.000000 opaw-0.2/opaw/examples/function_call.py
+-rw-rw-rw-   0        0        0      353 2023-08-04 16:20:25.000000 opaw-0.2/opaw/examples/image.py
+-rw-rw-rw-   0        0        0      569 2023-08-04 16:20:25.000000 opaw-0.2/opaw/examples/moderation.py
+-rw-rw-rw-   0        0        0       29 2023-08-03 17:18:41.000000 opaw-0.2/opaw/main.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:54:29.931607 opaw-0.2/opaw/model/
+-rw-rw-rw-   0        0        0        0 2023-07-31 12:07:48.000000 opaw-0.2/opaw/model/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/audio.py
+-rw-rw-rw-   0        0        0     1320 2023-08-03 11:13:00.000000 opaw-0.2/opaw/model/bot.py
+-rw-rw-rw-   0        0        0     2310 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/chat.py
+-rw-rw-rw-   0        0        0      635 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/completion.py
+-rw-rw-rw-   0        0        0      638 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/edit.py
+-rw-rw-rw-   0        0        0      634 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/embedding.py
+-rw-rw-rw-   0        0        0     1040 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/file.py
+-rw-rw-rw-   0        0        0     1107 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/finetune.py
+-rw-rw-rw-   0        0        0     1287 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/image.py
+-rw-rw-rw-   0        0        0      663 2023-08-04 16:20:25.000000 opaw-0.2/opaw/model/moderation.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:54:29.935045 opaw-0.2/opaw/tool/
+-rw-rw-rw-   0        0        0      553 2023-08-04 16:20:25.000000 opaw-0.2/opaw/tool/__init__.py
+-rw-rw-rw-   0        0        0      226 2023-07-30 07:02:06.000000 opaw-0.2/opaw/tool/stock.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:54:29.938937 opaw-0.2/opaw/util/
+-rw-rw-rw-   0        0        0     1631 2023-08-04 16:23:34.000000 opaw-0.2/opaw/util/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-08-04 16:03:00.000000 opaw-0.2/opaw/util/log.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:54:29.892765 opaw-0.2/opaw.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-08-04 16:54:29.000000 opaw-0.2/opaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-08-04 16:54:29.000000 opaw-0.2/opaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 16:54:29.000000 opaw-0.2/opaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 16:54:29.000000 opaw-0.2/opaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 16:54:29.000000 opaw-0.2/opaw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-08-04 16:54:29.943331 opaw-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      604 2023-08-04 16:52:28.000000 opaw-0.2/setup.py
```

### Comparing `opaw-0.1/setup.py` & `opaw-0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup
+from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='opaw',
-    packages=['opaw'],
-    version='0.1',
+    packages=find_packages(),
+    version='0.2',
     license='MIT',
     description='Unofficial python wrapper of OpenAI API.',
     author='hiimanget',
     author_email='hiimanget@gmail.com',
     url='https://github.com/hiimanget/openai-pw',
     keywords=['openai', 'python', 'api', 'wrapper'],
     install_requires=['openai'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent"]
+        "Operating System :: OS Independent"],
 )
```

