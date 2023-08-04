# Comparing `tmp/pysna-0.1.1.tar.gz` & `tmp/pysna-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysna-0.1.1.tar", last modified: Tue Jun 20 09:10:48 2023, max compression
+gzip compressed data, was "pysna-0.1.2.tar", last modified: Fri Aug  4 09:15:38 2023, max compression
```

## Comparing `pysna-0.1.1.tar` & `pysna-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.703758 pysna-0.1.1/
--rw-rw-rw-   0        0        0     1084 2022-12-21 10:40:25.000000 pysna-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4138 2023-06-20 09:10:48.703758 pysna-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.656481 pysna-0.1.1/PySNA.egg-info/
--rw-rw-rw-   0        0        0     4138 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3613 2023-03-15 14:43:39.000000 pysna-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.672098 pysna-0.1.1/pysna/
--rw-rw-rw-   0        0        0      383 2023-06-20 09:05:39.000000 pysna-0.1.1/pysna/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-02-23 14:25:50.000000 pysna-0.1.1/pysna/api.py
--rw-rw-rw-   0        0        0    14055 2023-03-15 13:49:38.000000 pysna-0.1.1/pysna/cli.py
--rw-rw-rw-   0        0        0    21580 2023-03-15 13:49:38.000000 pysna-0.1.1/pysna/fetch.py
--rw-rw-rw-   0        0        0    12947 2023-03-15 13:49:38.000000 pysna-0.1.1/pysna/process.py
--rw-rw-rw-   0        0        0    11279 2023-03-15 13:51:05.000000 pysna-0.1.1/pysna/utils.py
--rw-rw-rw-   0        0        0       42 2023-06-20 09:10:48.703758 pysna-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-03-14 20:31:07.000000 pysna-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.703758 pysna-0.1.1/tests/
--rw-rw-rw-   0        0        0     2510 2023-03-10 16:55:23.000000 pysna-0.1.1/tests/test_api.py
--rw-rw-rw-   0        0        0    18072 2023-03-10 17:02:53.000000 pysna-0.1.1/tests/test_fetch.py
--rw-rw-rw-   0        0        0     8254 2023-02-23 15:33:31.000000 pysna-0.1.1/tests/test_process.py
--rw-rw-rw-   0        0        0     1083 2023-02-19 17:05:43.000000 pysna-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:15:38.471693 pysna-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 09:15:27.000000 pysna-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-04 09:15:38.471693 pysna-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-04 09:15:27.000000 pysna-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:15:38.467692 pysna-0.1.2/pysna/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-04 09:15:27.000000 pysna-0.1.2/pysna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31735 2023-08-04 09:15:27.000000 pysna-0.1.2/pysna/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-08-04 09:15:27.000000 pysna-0.1.2/pysna/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-08-04 09:15:27.000000 pysna-0.1.2/pysna/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-08-04 09:15:27.000000 pysna-0.1.2/pysna/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-08-04 09:15:27.000000 pysna-0.1.2/pysna/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:15:38.467692 pysna-0.1.2/pysna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-04 09:15:38.000000 pysna-0.1.2/pysna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-04 09:15:38.000000 pysna-0.1.2/pysna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:15:38.000000 pysna-0.1.2/pysna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 09:15:38.000000 pysna-0.1.2/pysna.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 09:15:38.000000 pysna-0.1.2/pysna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 09:15:38.000000 pysna-0.1.2/pysna.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:15:38.471693 pysna-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-04 09:15:27.000000 pysna-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:15:38.471693 pysna-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-04 09:15:27.000000 pysna-0.1.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-08-04 09:15:27.000000 pysna-0.1.2/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-08-04 09:15:27.000000 pysna-0.1.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-04 09:15:27.000000 pysna-0.1.2/tests/test_utils.py
```

### Comparing `pysna-0.1.1/PKG-INFO` & `pysna-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-Metadata-Version: 2.1
-Name: pysna
-Version: 0.1.1
-Summary: Python Package for Social Network Analytics
-Home-page: https://github.com/mathun3003/PySNA
-Author: Mathis Hunke
-Author-email: mathun3003@gmail.com
-License: MIT License
-Project-URL: Documentation, https://mathun3003.github.io/PySNA/
-Project-URL: Issue Tracker, https://github.com/mathun3003/PySNA/issues
-Project-URL: Source Code, https://github.com/mathun3003/PySNA
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PySNA
-
-[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
-[![Twitter API v1.1](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard)](https://developer.twitter.com/en/docs/twitter-api/v1)
-[![Twitter API v2](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2)](https://developer.twitter.com/en/docs/twitter-api)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-
-
-Python Package for Social Network Analytics
-
-Installation
-------------
-
-The easiest way to install the latest version from PyPI is by using
-[pip](https://pip.pypa.io/):
-
-    pip install pysna
-
-You can also use Git to clone the repository from GitHub to install the latest
-development version:
-
-    git clone https://github.com/mathun3003/PySNA.git
-    cd PySNA
-    pip install .
-
-Alternatively, install directly from the GitHub repository:
-
-    pip install git+https://github.com/mathun3003/PySNA.git
-
-
-Quick Start
-------------
-Import the API class for the Twitter API by writing:
-
-```python
-from pysna import TwitterAPI
-```
-
-or import utility functions, too, by writing:
-
-```python
-from pysna import *
-```
-
-Then, create an API instance by running:
-
-```python
-api = TwitterAPI("BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")
-```
-
-and invoke a function:
-
-```python
-api.user_info(...)
-```
-
-Find usage and output examples in the [examples folder](https://github.com/mathun3003/PySNA/tree/main/examples).
-
-Functionalities
-------------
-This package was designed to perform data analysis on Twitter data. It extends the official Twitter API by using the open-source package [tweepy](https://github.com/tweepy/tweepy).
-
-Thus, the following functions are added to the tweepy package:
-- ``user_info``
-- ``tweet_info``
-- ``compare_users``
-- ``compare_tweets``
-
-Furthermore, some utility functions exist:
-- ``export_to_json``
-- ``append_to_json``
-- ``load_from_json``
-- ``export_to_csv``
-- ``append_to_csv``
-
-You can find further information on the [Documentation](https://mathun3003.github.io/PySNA/).
-
-
-CLI
-----------------
-The above mentioned functions are also available on the CLI.
-
-To see the usage instructions and help, run:
-
-    pysna -h
-
-If you wish to see the usage instructions for a function, run:
-
-    pysna <function> --help
-
-For example, if you want to request a comparison of two users, you can run:
-
-```bash
-pysna compare-users "WWU_Muenster" "goetheuni" -c "tweets_count" "common_followers" -o "results.json" --return-timestamp
-```
-
-This will perform a comparison on the ``"WWU_Muenster"`` and ``"goetheuni"`` Twitter Accounts based on their number of composed Tweets and common followers. The results are exported to the ``results.json`` file. Also, the timestamp of the request will be returned.
-
-**NOTE**: Every request needs valid credentials for the official Twitter API. Thus, pass in a .env file to every function call by using the ``--env`` flag or use the ``set-secrets`` function to set the API secrets for upcoming requests (recommended). See the corresponding section in the [documentation](https://mathun3003.github.io/PySNA/user-guide/overview/cli/).
-
-
-Notes
-------------
-
-- Only Python 3.10 is supported.
-- Only ``.env`` files are supported for the CLI, yet.
+Metadata-Version: 2.1
+Name: pysna
+Version: 0.1.2
+Summary: Python Package for Social Network Analytics
+Home-page: https://github.com/mathun3003/PySNA
+Author: Mathis Hunke
+Author-email: mathun3003@gmail.com
+License: MIT License
+Project-URL: Documentation, https://mathun3003.github.io/PySNA/
+Project-URL: Issue Tracker, https://github.com/mathun3003/PySNA/issues
+Project-URL: Source Code, https://github.com/mathun3003/PySNA
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PySNA
+
+[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+
+Python Package for Social Network Analytics
+
+Installation
+------------
+
+The easiest way to install the latest version from PyPI is by using
+[pip](https://pip.pypa.io/):
+
+    pip install pysna
+
+You can also use Git to clone the repository from GitHub to install the latest
+development version:
+
+    git clone https://github.com/mathun3003/PySNA.git
+    cd PySNA
+    pip install .
+
+Alternatively, install directly from the GitHub repository:
+
+    pip install git+https://github.com/mathun3003/PySNA.git
+
+
+Quick Start
+------------
+Import the API class for the Twitter API by writing:
+
+```python
+from pysna import TwitterAPI
+```
+
+or import utility functions, too, by writing:
+
+```python
+from pysna import *
+```
+
+Then, create an API instance by running:
+
+```python
+api = TwitterAPI("BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")
+```
+
+and invoke a function:
+
+```python
+api.user_info(...)
+```
+
+Find usage and output examples in the [examples folder](https://github.com/mathun3003/PySNA/tree/main/examples).
+
+Functionalities
+------------
+This package was designed to perform data analysis on Twitter data. It extends the official Twitter API by using the open-source package [tweepy](https://github.com/tweepy/tweepy).
+
+Thus, the following functions are added to the tweepy package:
+- ``user_info``
+- ``tweet_info``
+- ``compare_users``
+- ``compare_tweets``
+
+Furthermore, some utility functions exist:
+- ``export_to_json``
+- ``append_to_json``
+- ``load_from_json``
+- ``export_to_csv``
+- ``append_to_csv``
+
+You can find further information on the [Documentation](https://mathun3003.github.io/PySNA/).
+
+
+CLI
+----------------
+The above mentioned functions are also available on the CLI.
+
+To see the usage instructions and help, run:
+
+    pysna -h
+
+If you wish to see the usage instructions for a function, run:
+
+    pysna <function> --help
+
+For example, if you want to request a comparison of two users, you can run:
+
+```bash
+pysna compare-users "WWU_Muenster" "goetheuni" -c "tweets_count" "common_followers" -o "results.json" --return-timestamp
+```
+
+This will perform a comparison on the ``"WWU_Muenster"`` and ``"goetheuni"`` Twitter Accounts based on their number of composed Tweets and common followers. The results are exported to the ``results.json`` file. Also, the timestamp of the request will be returned.
+
+**NOTE**: Every request needs valid credentials for the official Twitter API. Thus, pass in a .env file to every function call by using the ``--env`` flag or use the ``set-secrets`` function to set the API secrets for upcoming requests (recommended). See the corresponding section in the [documentation](https://mathun3003.github.io/PySNA/user-guide/overview/cli/).
+
+
+Notes
+------------
+
+- Only Python >= 3.10 is supported.
+- Only ``.env`` files are supported for the CLI, yet.
+- Use the ``sample.local.env`` to ensure functionality of the CLI tool.
```

### Comparing `pysna-0.1.1/PySNA.egg-info/PKG-INFO` & `pysna-0.1.2/pysna.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-Metadata-Version: 2.1
-Name: pysna
-Version: 0.1.1
-Summary: Python Package for Social Network Analytics
-Home-page: https://github.com/mathun3003/PySNA
-Author: Mathis Hunke
-Author-email: mathun3003@gmail.com
-License: MIT License
-Project-URL: Documentation, https://mathun3003.github.io/PySNA/
-Project-URL: Issue Tracker, https://github.com/mathun3003/PySNA/issues
-Project-URL: Source Code, https://github.com/mathun3003/PySNA
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PySNA
-
-[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
-[![Twitter API v1.1](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard)](https://developer.twitter.com/en/docs/twitter-api/v1)
-[![Twitter API v2](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2)](https://developer.twitter.com/en/docs/twitter-api)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-
-
-Python Package for Social Network Analytics
-
-Installation
-------------
-
-The easiest way to install the latest version from PyPI is by using
-[pip](https://pip.pypa.io/):
-
-    pip install pysna
-
-You can also use Git to clone the repository from GitHub to install the latest
-development version:
-
-    git clone https://github.com/mathun3003/PySNA.git
-    cd PySNA
-    pip install .
-
-Alternatively, install directly from the GitHub repository:
-
-    pip install git+https://github.com/mathun3003/PySNA.git
-
-
-Quick Start
-------------
-Import the API class for the Twitter API by writing:
-
-```python
-from pysna import TwitterAPI
-```
-
-or import utility functions, too, by writing:
-
-```python
-from pysna import *
-```
-
-Then, create an API instance by running:
-
-```python
-api = TwitterAPI("BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")
-```
-
-and invoke a function:
-
-```python
-api.user_info(...)
-```
-
-Find usage and output examples in the [examples folder](https://github.com/mathun3003/PySNA/tree/main/examples).
-
-Functionalities
-------------
-This package was designed to perform data analysis on Twitter data. It extends the official Twitter API by using the open-source package [tweepy](https://github.com/tweepy/tweepy).
-
-Thus, the following functions are added to the tweepy package:
-- ``user_info``
-- ``tweet_info``
-- ``compare_users``
-- ``compare_tweets``
-
-Furthermore, some utility functions exist:
-- ``export_to_json``
-- ``append_to_json``
-- ``load_from_json``
-- ``export_to_csv``
-- ``append_to_csv``
-
-You can find further information on the [Documentation](https://mathun3003.github.io/PySNA/).
-
-
-CLI
-----------------
-The above mentioned functions are also available on the CLI.
-
-To see the usage instructions and help, run:
-
-    pysna -h
-
-If you wish to see the usage instructions for a function, run:
-
-    pysna <function> --help
-
-For example, if you want to request a comparison of two users, you can run:
-
-```bash
-pysna compare-users "WWU_Muenster" "goetheuni" -c "tweets_count" "common_followers" -o "results.json" --return-timestamp
-```
-
-This will perform a comparison on the ``"WWU_Muenster"`` and ``"goetheuni"`` Twitter Accounts based on their number of composed Tweets and common followers. The results are exported to the ``results.json`` file. Also, the timestamp of the request will be returned.
-
-**NOTE**: Every request needs valid credentials for the official Twitter API. Thus, pass in a .env file to every function call by using the ``--env`` flag or use the ``set-secrets`` function to set the API secrets for upcoming requests (recommended). See the corresponding section in the [documentation](https://mathun3003.github.io/PySNA/user-guide/overview/cli/).
-
-
-Notes
-------------
-
-- Only Python 3.10 is supported.
-- Only ``.env`` files are supported for the CLI, yet.
+Metadata-Version: 2.1
+Name: pysna
+Version: 0.1.2
+Summary: Python Package for Social Network Analytics
+Home-page: https://github.com/mathun3003/PySNA
+Author: Mathis Hunke
+Author-email: mathun3003@gmail.com
+License: MIT License
+Project-URL: Documentation, https://mathun3003.github.io/PySNA/
+Project-URL: Issue Tracker, https://github.com/mathun3003/PySNA/issues
+Project-URL: Source Code, https://github.com/mathun3003/PySNA
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PySNA
+
+[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+
+Python Package for Social Network Analytics
+
+Installation
+------------
+
+The easiest way to install the latest version from PyPI is by using
+[pip](https://pip.pypa.io/):
+
+    pip install pysna
+
+You can also use Git to clone the repository from GitHub to install the latest
+development version:
+
+    git clone https://github.com/mathun3003/PySNA.git
+    cd PySNA
+    pip install .
+
+Alternatively, install directly from the GitHub repository:
+
+    pip install git+https://github.com/mathun3003/PySNA.git
+
+
+Quick Start
+------------
+Import the API class for the Twitter API by writing:
+
+```python
+from pysna import TwitterAPI
+```
+
+or import utility functions, too, by writing:
+
+```python
+from pysna import *
+```
+
+Then, create an API instance by running:
+
+```python
+api = TwitterAPI("BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")
+```
+
+and invoke a function:
+
+```python
+api.user_info(...)
+```
+
+Find usage and output examples in the [examples folder](https://github.com/mathun3003/PySNA/tree/main/examples).
+
+Functionalities
+------------
+This package was designed to perform data analysis on Twitter data. It extends the official Twitter API by using the open-source package [tweepy](https://github.com/tweepy/tweepy).
+
+Thus, the following functions are added to the tweepy package:
+- ``user_info``
+- ``tweet_info``
+- ``compare_users``
+- ``compare_tweets``
+
+Furthermore, some utility functions exist:
+- ``export_to_json``
+- ``append_to_json``
+- ``load_from_json``
+- ``export_to_csv``
+- ``append_to_csv``
+
+You can find further information on the [Documentation](https://mathun3003.github.io/PySNA/).
+
+
+CLI
+----------------
+The above mentioned functions are also available on the CLI.
+
+To see the usage instructions and help, run:
+
+    pysna -h
+
+If you wish to see the usage instructions for a function, run:
+
+    pysna <function> --help
+
+For example, if you want to request a comparison of two users, you can run:
+
+```bash
+pysna compare-users "WWU_Muenster" "goetheuni" -c "tweets_count" "common_followers" -o "results.json" --return-timestamp
+```
+
+This will perform a comparison on the ``"WWU_Muenster"`` and ``"goetheuni"`` Twitter Accounts based on their number of composed Tweets and common followers. The results are exported to the ``results.json`` file. Also, the timestamp of the request will be returned.
+
+**NOTE**: Every request needs valid credentials for the official Twitter API. Thus, pass in a .env file to every function call by using the ``--env`` flag or use the ``set-secrets`` function to set the API secrets for upcoming requests (recommended). See the corresponding section in the [documentation](https://mathun3003.github.io/PySNA/user-guide/overview/cli/).
+
+
+Notes
+------------
+
+- Only Python >= 3.10 is supported.
+- Only ``.env`` files are supported for the CLI, yet.
+- Use the ``sample.local.env`` to ensure functionality of the CLI tool.
```

### Comparing `pysna-0.1.1/README.md` & `pysna-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,106 @@
-# PySNA
-
-[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
-[![Twitter API v1.1](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard)](https://developer.twitter.com/en/docs/twitter-api/v1)
-[![Twitter API v2](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2)](https://developer.twitter.com/en/docs/twitter-api)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-
-
-Python Package for Social Network Analytics
-
-Installation
-------------
-
-The easiest way to install the latest version from PyPI is by using
-[pip](https://pip.pypa.io/):
-
-    pip install pysna
-
-You can also use Git to clone the repository from GitHub to install the latest
-development version:
-
-    git clone https://github.com/mathun3003/PySNA.git
-    cd PySNA
-    pip install .
-
-Alternatively, install directly from the GitHub repository:
-
-    pip install git+https://github.com/mathun3003/PySNA.git
-
-
-Quick Start
-------------
-Import the API class for the Twitter API by writing:
-
-```python
-from pysna import TwitterAPI
-```
-
-or import utility functions, too, by writing:
-
-```python
-from pysna import *
-```
-
-Then, create an API instance by running:
-
-```python
-api = TwitterAPI("BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")
-```
-
-and invoke a function:
-
-```python
-api.user_info(...)
-```
-
-Find usage and output examples in the [examples folder](https://github.com/mathun3003/PySNA/tree/main/examples).
-
-Functionalities
-------------
-This package was designed to perform data analysis on Twitter data. It extends the official Twitter API by using the open-source package [tweepy](https://github.com/tweepy/tweepy).
-
-Thus, the following functions are added to the tweepy package:
-- ``user_info``
-- ``tweet_info``
-- ``compare_users``
-- ``compare_tweets``
-
-Furthermore, some utility functions exist:
-- ``export_to_json``
-- ``append_to_json``
-- ``load_from_json``
-- ``export_to_csv``
-- ``append_to_csv``
-
-You can find further information on the [Documentation](https://mathun3003.github.io/PySNA/).
-
-
-CLI
-----------------
-The above mentioned functions are also available on the CLI.
-
-To see the usage instructions and help, run:
-
-    pysna -h
-
-If you wish to see the usage instructions for a function, run:
-
-    pysna <function> --help
-
-For example, if you want to request a comparison of two users, you can run:
-
-```bash
-pysna compare-users "WWU_Muenster" "goetheuni" -c "tweets_count" "common_followers" -o "results.json" --return-timestamp
-```
-
-This will perform a comparison on the ``"WWU_Muenster"`` and ``"goetheuni"`` Twitter Accounts based on their number of composed Tweets and common followers. The results are exported to the ``results.json`` file. Also, the timestamp of the request will be returned.
-
-**NOTE**: Every request needs valid credentials for the official Twitter API. Thus, pass in a .env file to every function call by using the ``--env`` flag or use the ``set-secrets`` function to set the API secrets for upcoming requests (recommended). See the corresponding section in the [documentation](https://mathun3003.github.io/PySNA/user-guide/overview/cli/).
-
-
-Notes
-------------
-
-- Only Python 3.10 is supported.
-- Only ``.env`` files are supported for the CLI, yet.
+# PySNA
+
+[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+
+Python Package for Social Network Analytics
+
+Installation
+------------
+
+The easiest way to install the latest version from PyPI is by using
+[pip](https://pip.pypa.io/):
+
+    pip install pysna
+
+You can also use Git to clone the repository from GitHub to install the latest
+development version:
+
+    git clone https://github.com/mathun3003/PySNA.git
+    cd PySNA
+    pip install .
+
+Alternatively, install directly from the GitHub repository:
+
+    pip install git+https://github.com/mathun3003/PySNA.git
+
+
+Quick Start
+------------
+Import the API class for the Twitter API by writing:
+
+```python
+from pysna import TwitterAPI
+```
+
+or import utility functions, too, by writing:
+
+```python
+from pysna import *
+```
+
+Then, create an API instance by running:
+
+```python
+api = TwitterAPI("BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")
+```
+
+and invoke a function:
+
+```python
+api.user_info(...)
+```
+
+Find usage and output examples in the [examples folder](https://github.com/mathun3003/PySNA/tree/main/examples).
+
+Functionalities
+------------
+This package was designed to perform data analysis on Twitter data. It extends the official Twitter API by using the open-source package [tweepy](https://github.com/tweepy/tweepy).
+
+Thus, the following functions are added to the tweepy package:
+- ``user_info``
+- ``tweet_info``
+- ``compare_users``
+- ``compare_tweets``
+
+Furthermore, some utility functions exist:
+- ``export_to_json``
+- ``append_to_json``
+- ``load_from_json``
+- ``export_to_csv``
+- ``append_to_csv``
+
+You can find further information on the [Documentation](https://mathun3003.github.io/PySNA/).
+
+
+CLI
+----------------
+The above mentioned functions are also available on the CLI.
+
+To see the usage instructions and help, run:
+
+    pysna -h
+
+If you wish to see the usage instructions for a function, run:
+
+    pysna <function> --help
+
+For example, if you want to request a comparison of two users, you can run:
+
+```bash
+pysna compare-users "WWU_Muenster" "goetheuni" -c "tweets_count" "common_followers" -o "results.json" --return-timestamp
+```
+
+This will perform a comparison on the ``"WWU_Muenster"`` and ``"goetheuni"`` Twitter Accounts based on their number of composed Tweets and common followers. The results are exported to the ``results.json`` file. Also, the timestamp of the request will be returned.
+
+**NOTE**: Every request needs valid credentials for the official Twitter API. Thus, pass in a .env file to every function call by using the ``--env`` flag or use the ``set-secrets`` function to set the API secrets for upcoming requests (recommended). See the corresponding section in the [documentation](https://mathun3003.github.io/PySNA/user-guide/overview/cli/).
+
+
+Notes
+------------
+
+- Only Python >= 3.10 is supported.
+- Only ``.env`` files are supported for the CLI, yet.
+- Use the ``sample.local.env`` to ensure functionality of the CLI tool.
```

### Comparing `pysna-0.1.1/pysna/api.py` & `pysna-0.1.2/pysna/api.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,605 +1,605 @@
-# -*- coding: utf-8 -*-
-import logging
-import sys
-from datetime import datetime
-from typing import Any, List, Literal, get_args
-
-import tweepy
-
-from pysna.fetch import TwitterDataFetcher
-from pysna.process import TwitterDataProcessor
-from pysna.utils import strf_datetime
-
-# create logger instance
-log = logging.getLogger(__name__)
-# log to stdout
-handler = logging.StreamHandler(sys.stdout)
-handler.setLevel(logging.ERROR)
-formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-handler.setFormatter(formatter)
-log.addHandler(handler)
-
-
-class TwitterAPI(tweepy.Client):
-    """Twitter API interface in order to interact with the Twitter Search API v2."""
-
-    LITERALS_USER_INFO = Literal[
-        "id",
-        "id_str",
-        "name",
-        "screen_name",
-        "followers",
-        "followees",
-        "location",
-        "description",
-        "url",
-        "entities",
-        "protected",
-        "followers_count",
-        "friends_count",
-        "listed_count",
-        "created_at",
-        "latest_activity",
-        "last_active",
-        "liked_tweets",
-        "composed_tweets",
-        "favourites_count",
-        "verified",
-        "statuses_count",
-        "status",
-        "contributors_enabled",
-        "profile_image_url_https",
-        "profile_banner_url",
-        "default_profile",
-        "default_profile_image",
-        "withheld_in_countries",
-        "bot_scores",
-    ]
-
-    LITERALS_TWEET_INFO = Literal[
-        "id",
-        "id_str",
-        "full_text",
-        "display_text_range",
-        "truncated",
-        "created_at",
-        "entities",
-        "tweet_annotations",
-        "source",
-        "retweeters",
-        "in_reply_to_status_id",
-        "in_reply_to_status_id_str",
-        "in_reply_to_user_id",
-        "in_reply_to_user_id_str",
-        "in_reply_to_screen_name",
-        "user",
-        "contributors",
-        "coordinates",
-        "place",
-        "is_quote_status",
-        "public_metrics",
-        "quoting_users",
-        "liking_users",
-        "favorited",
-        "retweeted",
-        "retweeted_status",
-        "possibly_sensitive",
-        "lang",
-        "sentiment",
-    ]
-
-    LITERALS_COMPARE_USERS = Literal[
-        "relationship",
-        "followers_count",
-        "followees_count",
-        "tweets_count",
-        "favourites_count",
-        "common_followers",
-        "distinct_followers",
-        "common_followees",
-        "distinct_followees",
-        "commonly_liked_tweets",
-        "distinctly_liked_tweets",
-        "similarity",
-        "created_at",
-        "protected",
-        "verified",
-    ]
-
-    SIMILARITY_FEATURES_COMPARE_USERS = Literal["followers_count", "friends_count", "listed_count", "favourites_count", "statuses_count"]
-
-    LITERALS_COMPARE_TWEETS = Literal[
-        "view_count",
-        "like_count",
-        "retweet_count",
-        "quote_count",
-        "reply_count",
-        "common_quoting_users",
-        "distinct_quoting_users",
-        "common_liking_users",
-        "distinct_liking_users",
-        "common_retweeters",
-        "distinct_retweeters",
-        "similarity",
-        "created_at",
-    ]
-
-    SIMILARITY_FEATURES_COMPARE_TWEETS = Literal["retweet_count", "reply_count", "like_count", "quote_count", "impression_count"]
-
-    def __init__(
-        self,
-        bearer_token: Any | None = None,
-        consumer_key: Any | None = None,
-        consumer_secret: Any | None = None,
-        access_token: Any | None = None,
-        access_token_secret: Any | None = None,
-        x_rapidapi_key: Any | None = None,
-        x_rapidapi_host: Any | None = None,
-        wait_on_rate_limit: bool = True,
-    ):
-        super(self.__class__, self).__init__(bearer_token, consumer_key, consumer_secret, access_token, access_token_secret, wait_on_rate_limit=wait_on_rate_limit)
-
-        self._bearer_token = bearer_token
-        self._consumer_key = consumer_key
-        self._consumer_secret = consumer_secret
-        self._access_token = access_token
-        self._access_token_secret = access_token_secret
-        self._x_rapidapi_key = x_rapidapi_key
-        self._x_rapidapi_host = x_rapidapi_host
-        self._wait_on_rate_limit = wait_on_rate_limit
-
-        # init TwitterDataFetcher
-        self.fetcher = TwitterDataFetcher(self._bearer_token, self._consumer_key, self._consumer_secret, self._access_token, self._access_token_secret, self._x_rapidapi_key, self._x_rapidapi_host)
-
-        # init DataProcessor
-        self.data_processor = TwitterDataProcessor()
-
-    def _handle_output(self, output: dict) -> Any:
-        """Returns either the single value from one-key dictionary or the dictionary itself.
-
-        Args:
-            output (dict): Input dictionary, usually the output of a function.
-
-        Returns:
-            Any: Either the single value from one-key dictionary or the dictionary itself.
-        """
-        # if output has only one key
-        if len(output) == 1:
-            # return single value
-            return next(iter(output.values()))
-        else:
-            # else return original output
-            return output
-
-    def user_info(self, user: str | int, attributes: List[LITERALS_USER_INFO] | str, return_timestamp: bool = False) -> Any:
-        """Receive requested user information from Twitter User Object.
-
-        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
-
-        Args:
-            user (str | int): Twitter User either specified by corresponding ID or screen name.
-            attributes (List[str] | str): Attributes of the User object. These must be from: id, id_str, name, screen_name, followers, followees, location, description, url, entities, protected, followers_count, friends_count, listed_count, created_at, latest_activity, last_active, liked_tweets, composed_tweets, favourites_count, verified, statuses_count, status, contributors_enabled, profile_image_url_https, profile_banner_url, default_profile, default_profile_image, withheld_in_countries, bot_scores
-            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
-
-        Raises:
-            KeyError: If invalid attribute was provided.
-            ValueError: If Botometer secrets were not provided.
-
-        Returns:
-            dict: Requested user information.
-
-        References: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#user_info
-        """
-        # catch Botometer API secrets before iteration over attributes.
-        if "bot_scores" in attributes:
-            if (self._x_rapidapi_key is None) or (self._x_rapidapi_host is None):
-                raise ValueError("'X_RAPIDAPI_KEY' and 'X_RAPIDAPI_HOST' secrets for Botometer API need to be provided.")
-
-        # initialize empty dict to store requested attributes
-        user_info = dict()
-        # if single string was provided
-        if isinstance(attributes, str):
-            # convert to list for iteration
-            attributes = [attributes]
-        # get user object
-        user_obj = self.fetcher.get_user_object(user)
-        # loop through the list of attributes and add them to the dictionary
-        for attr in attributes:
-            # if invalid attribute was provided
-            if attr not in get_args(self.LITERALS_USER_INFO):
-                raise ValueError("Invalid attribute for '{}'".format(attr))
-            # if the desired attribute is in default user object returned by the v1 Search API
-            elif attr in user_obj._json.keys():
-                user_info[attr] = user_obj._json[attr]
-            # get information about user's followers
-            elif attr == "followers":
-                user_info[attr] = self.data_processor.extract_followers(user_obj)
-            # get information about user's followees
-            elif attr == "followees":
-                user_info[attr] = self.data_processor.extract_followees(user_obj)
-            # get all liked tweets of user
-            elif attr == "liked_tweets":
-                # get page results first
-                liked_tweets = self.fetcher.get_liked_tweets_ids(user)
-                user_info[attr] = liked_tweets
-            # get all composed tweets
-            elif attr == "composed_tweets":
-                # get page results first
-                composed_tweets = self.fetcher.get_composed_tweets_ids(user)
-                user_info[attr] = composed_tweets
-            # get user's latest activity
-            elif attr == "latest_activity":
-                user_info[attr] = self.fetcher.get_latest_activity(user)
-            # get user's latest activity date
-            elif attr == "last_active":
-                user_info[attr] = self.fetcher.get_latest_activity_date(user)
-            # get user's botometer scores
-            elif attr == "bot_scores":
-                user_info[attr] = self.fetcher.get_botometer_scores(user)
-            # if attribute was not found
-            else:
-                user_info[attr] = None
-            # if timestamp should be returned
-        if return_timestamp:
-            user_info["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
-
-        return self._handle_output(user_info)
-
-    def compare_users(self, users: List[str | int], compare: str | List[LITERALS_COMPARE_USERS], return_timestamp: bool = False, features: List[str] | None = None) -> Any:
-        """Compare two or more users with the specified comparison attribute(s).
-
-        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
-
-        Args:
-            users (List[str  |  int]): User IDs or screen names
-            compare (str): Comparison attribute. Must be from: relationship, followers_count, followees_count, tweets_count, favourites_count, common_followers, distinct_followers, common_followees, distinct_followees, commonly_liked_tweets, distinctly_liked_tweets, similarity, created_at, protected, verified.
-            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
-            features (List[str] | None, optional): Defined features of Twitter User Object on which similarity will be computed. Must be from: followers_count, friends_count, listed_count, favourites_count, statuses_count. Defaults to None.
-
-        Raises:
-            ValueError: If invalid comparison attribute was provided.
-
-        Returns:
-            dict | list: Results of requested comparison attribute(s).
-
-        Referencs: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#compare_users
-        """
-        # users list must contain at least two elements
-        assert len(users) > 1, "'users' list must contain at least two elements, {} was/were provided".format(len(users))
-
-        # catch if feature vector contains only numeric values, and contains at least two elements
-        if features:
-            assert len(features) > 1, "'features' list must have at least two elements. {} was/were given".format(len(features))
-            for feat in features:
-                if feat not in get_args(self.SIMILARITY_FEATURES_COMPARE_USERS):
-                    raise ValueError(f"Only numeric features are supported. Must be from: {', '.join(get_args(self.SIMILARITY_FEATURES_COMPARE_USERS))}. You passed in {feat}")
-
-        # if single comparison attribute was provided as string
-        if isinstance(compare, str):
-            # change to list object
-            compare = [compare]
-        # init empty dict to store results
-        results = dict()
-        # iterate over comparison attributes
-        for attr in compare:
-            # if invalid attribute was provided
-            if attr not in get_args(self.LITERALS_COMPARE_USERS):
-                raise ValueError("Invalid attribute for '{}'".format(attr))
-            # match comparison attributes
-            match attr:
-                # compare relationships between two users
-                case "relationship":
-                    results[attr] = self.fetcher.get_relationship_pairs(users)
-                # compare number of followers
-                case "followers_count":
-                    # get individual followers
-                    followers = {user: self.fetcher.get_user_object(user).followers_count for user in users}
-                    # add descriptive metrics
-                    followers_with_metrics = self.data_processor.calc_descriptive_metrics(followers)
-                    results[attr] = followers_with_metrics
-                # compare number of friends
-                case "followees_count":
-                    # get individual followees
-                    followees = {user: self.fetcher.get_user_object(user).friends_count for user in users}
-                    # add descriptive metrics
-                    followees = self.data_processor.calc_descriptive_metrics(followees)
-                    results[attr] = followees
-                # compare number of Tweets issued by each user
-                case "tweets_count":
-                    # get individual statuses counts
-                    tweets = {user: self.fetcher.get_user_object(user).statuses_count for user in users}
-                    # add descriptive metrics
-                    tweets = self.data_processor.calc_descriptive_metrics(tweets)
-                    results[attr] = tweets
-                # compare number of likes issued by each user
-                case "favourites_count":
-                    # get individual likes
-                    likes = {user: self.fetcher.get_user_object(user).favourites_count for user in users}
-                    # add descriptive metrics
-                    likes = self.data_processor.calc_descriptive_metrics(likes)
-                    results[attr] = likes
-                # compare protected attribute of users
-                case "protected":
-                    results[attr] = {user: self.fetcher.get_user_object(user).protected for user in users}
-                # compare verified attribute for users
-                case "verified":
-                    results[attr] = {user: self.fetcher.get_user_object(user).verified for user in users}
-                # get common followers
-                case "common_followers":
-                    # get individual followers first
-                    individual_followers = [self.fetcher.get_user_follower_ids(user) for user in users]
-                    # get common followers by calculating the intersection
-                    common_followers = self.data_processor.intersection(individual_followers)
-                    results[attr] = common_followers
-                # get distinct followers
-                case "distinct_followers":
-                    # get individual followers first
-                    individual_followers = {user: self.fetcher.get_user_follower_ids(user) for user in users}
-                    # get distinct followers by calculating the difference of each set
-                    distinct_followers = self.data_processor.difference(individual_followers)
-                    results[attr] = distinct_followers
-                # get common followees
-                case "common_followees":
-                    # get individual followees first
-                    individual_followees = [self.fetcher.get_user_followee_ids(user) for user in users]
-                    # get common followees by calculating the intersection
-                    common_followees = self.data_processor.intersection(individual_followees)
-                    results[attr] = common_followees
-                # get distinct followees
-                case "distinct_followees":
-                    # get individual followees first
-                    individual_followees = {user: self.fetcher.get_user_followee_ids(user) for user in users}
-                    # get distinct followees by calculating the difference of each set
-                    distinct_followees = self.data_processor.difference(individual_followees)
-                    results[attr] = distinct_followees
-                # get common liked tweets
-                case "commonly_liked_tweets":
-                    # get individual liked tweets first
-                    individual_likes = [self.fetcher.get_liked_tweets_ids(user) for user in users]
-                    # get common liked tweets by calculating the intersection
-                    common_likes = self.data_processor.intersection(individual_likes)
-                    results[attr] = common_likes
-                # get distinct liked tweets
-                case "distinctly_liked_tweets":
-                    # get individual liked tweets first
-                    individual_likes = {user: self.fetcher.get_liked_tweets_ids(user) for user in users}
-                    # get distinct liked tweets by calculating the difference for each set
-                    distinct_likes = self.data_processor.difference(individual_likes)
-                    results[attr] = distinct_likes
-                # compute similarity between two users basd on the defined features
-                case "similarity":
-                    # feature list object must be defined
-                    if features is None:
-                        raise ValueError("'features' list must be provided.")
-                    # get serialized user objects first
-                    user_objs = [self.fetcher.get_user_object(user)._json for user in users]
-                    # calculate similarity based on defined feature vector
-                    results[attr] = self.data_processor.calc_similarity(user_objs=user_objs, features=features)
-                # compare creaation dates
-                case "created_at":
-                    # get individual creation dates first
-                    creation_dates = {user: self.fetcher.get_user_object(user).created_at for user in users}
-                    # add datetime metrics
-                    creation_dates = self.data_processor.calc_datetime_metrics(creation_dates)
-                    results[attr] = creation_dates
-                # if comparison attribute was not found
-                case _:
-                    results[attr] = None
-        # if timestamp should be returned
-        if return_timestamp:
-            results["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
-
-        return self._handle_output(results)
-
-    def tweet_info(self, tweet_id: str | int, attributes: List[LITERALS_TWEET_INFO] | str, return_timestamp: bool = False) -> Any:
-        """Receive requested Tweet information from Tweet Object.
-
-        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
-
-        Args:
-            tweet_id (str | int): Tweet ID
-            attributes (List[LITERALS_TWEET_INFO] | str): Attributes of the Tweet object. These must be from: id, id_str, full_text, display_text_range, truncated, created_at, entities, tweet_annotations, source, retweeters, in_reply_to_status_id, in_reply_to_status_id_str, in_reply_to_user_id, in_reply_to_user_id_str, in_reply_to_screen_name, user, contributors, coordinates, place, is_quote_status, public_metrics, quoting_users, liking_users, favorited, retweeted, retweeted_status, possibly_sensitive, lang, sentiment.
-            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
-
-        Raises:
-            ValueError: If invalid attribute was provided.
-
-        Returns:
-            dict: Requested Tweet information.
-
-        References: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#tweet_info
-        """
-        # get tweet object
-        tweet_obj = self.fetcher.get_tweet_object(tweet_id)
-
-        # initialize empty dict to store request information
-        tweet_info = dict()
-
-        # if single string was provided
-        if isinstance(attributes, str):
-            # convert to list for iteration
-            attributes = [attributes]
-        for attr in attributes:
-            # if invalid attribute was provided
-            if attr not in get_args(self.LITERALS_TWEET_INFO):
-                raise ValueError("Invalid attribute for '{}'".format(attr))
-            # get default attributes from tweepy Status model
-            elif attr in tweet_obj._json.keys():
-                tweet_info[attr] = tweet_obj._json[attr]
-            # get all quoting users
-            elif attr == "quoting_users":
-                quoting_users = self.fetcher.get_quoting_users_ids(tweet_id)
-                tweet_info[attr] = quoting_users
-            # get all liking users
-            elif attr == "liking_users":
-                liking_users = self.fetcher.get_liking_users_ids(tweet_id)
-                tweet_info[attr] = liking_users
-            # get all retweeters
-            elif attr == "retweeters":
-                retweeters = self.fetcher.get_retweeters_ids(tweet_id)
-                tweet_info[attr] = retweeters
-            # get public metrics
-            elif attr == "public_metrics":
-                tweet_info[attr] = self.fetcher.get_public_metrics(tweet_id)
-            # get context annotations
-            elif attr == "tweet_annotations":
-                tweet_info[attr] = self.fetcher.get_context_annotations_and_entities(tweet_id)
-            # get tweet sentiment
-            elif attr == "sentiment":
-                tweet_info[attr] = self.data_processor.detect_tweet_sentiment(tweet_obj.full_text)
-            # if attribute was not found
-            else:
-                tweet_info[attr] = None
-        # if timestamp should be returned
-        if return_timestamp:
-            tweet_info["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
-
-        return self._handle_output(tweet_info)
-
-    def compare_tweets(self, tweet_ids: List[str | int], compare: str | List[LITERALS_COMPARE_TWEETS], return_timestamp: bool = False, features: List[str] | None = None) -> Any:
-        """Compare two or more Tweets with the specified comparison attribute.
-
-        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
-
-        Args:
-            tweets (List[str  |  int]): List of Tweet IDs.
-            compare (str | List[LITERALS_COMPARE_TWEETS]): Comparison attribute. Needs to be from the following: view_count, like_count, retweet_count, quote_count, reply_count, common_quoting_users, distinct_quoting_users, common_liking_users, distinct_liking_users, common_retweeters, distinct_retweeters, similarity, created_at.
-            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
-            features (List[str] | None, optional): Defined features of Twitter User Object on which similarity will be computed. Must be from: retweet_count, reply_count, like_count, quote_count, impression_count. Defaults to None.
-
-        Raises:
-            AssertionError: If a list of one Tweet ID was provided.
-            ValueError: If invalid comparison attribute was provided.
-
-        Returns:
-            dict: Requested results for comparison attribute.
-
-        References: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#compare_tweets
-        """
-        # tweets list must contain at least two IDs
-        assert len(tweet_ids) > 1, "'tweets' list object needs at least two entries, not {}".format(len(tweet_ids))
-
-        # catch if feature vector contains only numeric values, and contains at least two elements
-        if features:
-            assert len(features) > 1, "'features' list must have at least two elements. {} was/were given".format(len(features))
-            for feat in features:
-                if feat not in get_args(self.SIMILARITY_FEATURES_COMPARE_TWEETS):
-                    raise ValueError(f"Only numeric features are supported. Must be from: {', '.join(get_args(self.SIMILARITY_FEATURES_COMPARE_TWEETS))}. You passed in {feat}.")
-
-        # if single comparison attribute was provided as string
-        if isinstance(compare, str):
-            # change to list object
-            compare = [compare]
-        # init empty dict to store results
-        results = dict()
-        # iterate over every given comparison atttribute
-        for attr in compare:
-            # if invalid attribute was provided
-            if attr not in get_args(self.LITERALS_COMPARE_TWEETS):
-                raise ValueError("Invalid attribute for '{}'".format(attr))
-            # match comparison attribute
-            match attr:
-                # compare numer of views / impressions
-                case "view_count":
-                    # get individual view_counts
-                    view_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["impression_count"] for tweet_id in tweet_ids}
-                    # add descriptive metrics
-                    view_counts = self.data_processor.calc_descriptive_metrics(view_counts)
-                    results[attr] = view_counts
-                # compare number of likes
-                case "like_count":
-                    # get individual like_counts
-                    like_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["like_count"] for tweet_id in tweet_ids}
-                    # add descriptive metrics
-                    like_counts = self.data_processor.calc_descriptive_metrics(like_counts)
-                    results[attr] = like_counts
-                # compare number or retweets
-                case "retweet_count":
-                    # get individual number of retweets
-                    retweet_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["retweet_count"] for tweet_id in tweet_ids}
-                    # add descriptive metrics
-                    retweet_counts = self.data_processor.calc_descriptive_metrics(retweet_counts)
-                    results[attr] = retweet_counts
-                # compare number of quotes
-                case "quote_count":
-                    # get individual number of quotes
-                    quote_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["quote_count"] for tweet_id in tweet_ids}
-                    # add descriptive metrics
-                    quote_counts = self.data_processor.calc_descriptive_metrics(quote_counts)
-                    results[attr] = quote_counts
-                # compare number of commonts
-                case "reply_count":
-                    # get individual number of replies first
-                    reply_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["reply_count"] for tweet_id in tweet_ids}
-                    # add descriptive metrics
-                    reply_counts = self.data_processor.calc_descriptive_metrics(reply_counts)
-                    results[attr] = reply_counts
-                # get all quoting users all Tweets have in common
-                case "common_quoting_users":
-                    # get individual quoting users first
-                    quoting_users = [self.fetcher.get_quoting_users_ids(tweet_id) for tweet_id in tweet_ids]
-                    # get common quoting users by calculating the intersection
-                    common_quoting_users = self.data_processor.intersection(quoting_users)
-                    # return quoting users
-                    results[attr] = common_quoting_users
-                # get distinct quoting users for each tweet
-                case "distinct_quoting_users":
-                    # get individual quoting users first
-                    quoting_users = {tweet_id: self.fetcher.get_quoting_users_ids(tweet_id) for tweet_id in tweet_ids}
-                    # get distinct quoting users for each tweet by calculating the difference for each set
-                    distinct_quoting_users = self.data_processor.difference(quoting_users)
-                    results[attr] = distinct_quoting_users
-                # get all liking users that all tweets have in common
-                case "common_liking_users":
-                    # get individual liking users first
-                    liking_users = [self.fetcher.get_liking_users_ids(tweet_id) for tweet_id in tweet_ids]
-                    # get common liking users by calculating the intersection
-                    common_liking_users = self.data_processor.intersection(liking_users)
-                    # return common liking users
-                    results[attr] = common_liking_users
-                # get distinct liking users of all tweets
-                case "distinct_liking_users":
-                    # get individual liking users first
-                    liking_users = {tweet_id: self.fetcher.get_liking_users_ids(tweet_id) for tweet_id in tweet_ids}
-                    # get distinct liking users for each tweet by calculating the difference for each set
-                    distinct_liking_users = self.data_processor.difference(liking_users)
-                    results[attr] = distinct_liking_users
-                # get all retweeters all tweets have in common
-                case "common_retweeters":
-                    # get individual retweeters first
-                    retweeters = [self.fetcher.get_retweeters_ids(tweet_id) for tweet_id in tweet_ids]
-                    # get common retweeters by calculating the intersection
-                    common_retweeters = self.data_processor.intersection(retweeters)
-                    # return common retweeters
-                    results[attr] = common_retweeters
-                # get distinct retweeters of all tweets
-                case "distinct_retweeters":
-                    # get individual retweeters first
-                    retweeters = {tweet_id: self.fetcher.get_retweeters_ids(tweet_id) for tweet_id in tweet_ids}
-                    # get distinct retweeters by calculating the difference for each set
-                    distinct_retweeters = self.data_processor.difference(retweeters)
-                    results[attr] = distinct_retweeters
-                # compute similarity between two tweets basd on the defined features
-                case "similarity":
-                    # feature list object must be defined
-                    if features is None:
-                        raise ValueError("'features' list must be provided.")
-                    # get public metrics for Tweet objects first
-                    public_metrics = {tweet_id: self.fetcher.get_public_metrics(tweet_id) for tweet_id in tweet_ids}
-                    # calculate similarity based on defined feature vector
-                    results[attr] = self.data_processor.calc_similarity(tweet_metrics=public_metrics, features=features)
-                # compare creation dates of tweets
-                case "created_at":
-                    # get individual creation dates first
-                    creation_dates = {tweet_id: self.fetcher.get_tweet_object(tweet_id).created_at for tweet_id in tweet_ids}
-                    # add datetime metrics
-                    creation_dates = self.data_processor.calc_datetime_metrics(creation_dates)
-                    results[attr] = creation_dates
-                # if attribute was not found
-                case _:
-                    results[attr] = None
-        # if UTC timestamp should be returned
-        if return_timestamp:
-            results["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
-
-        return self._handle_output(results)
+# -*- coding: utf-8 -*-
+import logging
+import sys
+from datetime import datetime
+from typing import Any, List, Literal, get_args
+
+import tweepy
+
+from pysna.fetch import TwitterDataFetcher
+from pysna.process import TwitterDataProcessor
+from pysna.utils import strf_datetime
+
+# create logger instance
+log = logging.getLogger(__name__)
+# log to stdout
+handler = logging.StreamHandler(sys.stdout)
+handler.setLevel(logging.ERROR)
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+handler.setFormatter(formatter)
+log.addHandler(handler)
+
+
+class TwitterAPI(tweepy.Client):
+    """Twitter API interface in order to interact with the Twitter Search API v2."""
+
+    LITERALS_USER_INFO = Literal[
+        "id",
+        "id_str",
+        "name",
+        "screen_name",
+        "followers",
+        "followees",
+        "location",
+        "description",
+        "url",
+        "entities",
+        "protected",
+        "followers_count",
+        "friends_count",
+        "listed_count",
+        "created_at",
+        "latest_activity",
+        "last_active",
+        "liked_tweets",
+        "composed_tweets",
+        "favourites_count",
+        "verified",
+        "statuses_count",
+        "status",
+        "contributors_enabled",
+        "profile_image_url_https",
+        "profile_banner_url",
+        "default_profile",
+        "default_profile_image",
+        "withheld_in_countries",
+        "bot_scores",
+    ]
+
+    LITERALS_TWEET_INFO = Literal[
+        "id",
+        "id_str",
+        "full_text",
+        "display_text_range",
+        "truncated",
+        "created_at",
+        "entities",
+        "tweet_annotations",
+        "source",
+        "retweeters",
+        "in_reply_to_status_id",
+        "in_reply_to_status_id_str",
+        "in_reply_to_user_id",
+        "in_reply_to_user_id_str",
+        "in_reply_to_screen_name",
+        "user",
+        "contributors",
+        "coordinates",
+        "place",
+        "is_quote_status",
+        "public_metrics",
+        "quoting_users",
+        "liking_users",
+        "favorited",
+        "retweeted",
+        "retweeted_status",
+        "possibly_sensitive",
+        "lang",
+        "sentiment",
+    ]
+
+    LITERALS_COMPARE_USERS = Literal[
+        "relationship",
+        "followers_count",
+        "followees_count",
+        "tweets_count",
+        "favourites_count",
+        "common_followers",
+        "distinct_followers",
+        "common_followees",
+        "distinct_followees",
+        "commonly_liked_tweets",
+        "distinctly_liked_tweets",
+        "similarity",
+        "created_at",
+        "protected",
+        "verified",
+    ]
+
+    SIMILARITY_FEATURES_COMPARE_USERS = Literal["followers_count", "friends_count", "listed_count", "favourites_count", "statuses_count"]
+
+    LITERALS_COMPARE_TWEETS = Literal[
+        "view_count",
+        "like_count",
+        "retweet_count",
+        "quote_count",
+        "reply_count",
+        "common_quoting_users",
+        "distinct_quoting_users",
+        "common_liking_users",
+        "distinct_liking_users",
+        "common_retweeters",
+        "distinct_retweeters",
+        "similarity",
+        "created_at",
+    ]
+
+    SIMILARITY_FEATURES_COMPARE_TWEETS = Literal["retweet_count", "reply_count", "like_count", "quote_count", "impression_count"]
+
+    def __init__(
+        self,
+        bearer_token: Any | None = None,
+        consumer_key: Any | None = None,
+        consumer_secret: Any | None = None,
+        access_token: Any | None = None,
+        access_token_secret: Any | None = None,
+        x_rapidapi_key: Any | None = None,
+        x_rapidapi_host: Any | None = None,
+        wait_on_rate_limit: bool = True,
+    ):
+        super(self.__class__, self).__init__(bearer_token, consumer_key, consumer_secret, access_token, access_token_secret, wait_on_rate_limit=wait_on_rate_limit)
+
+        self._bearer_token = bearer_token
+        self._consumer_key = consumer_key
+        self._consumer_secret = consumer_secret
+        self._access_token = access_token
+        self._access_token_secret = access_token_secret
+        self._x_rapidapi_key = x_rapidapi_key
+        self._x_rapidapi_host = x_rapidapi_host
+        self._wait_on_rate_limit = wait_on_rate_limit
+
+        # init TwitterDataFetcher
+        self.fetcher = TwitterDataFetcher(self._bearer_token, self._consumer_key, self._consumer_secret, self._access_token, self._access_token_secret, self._x_rapidapi_key, self._x_rapidapi_host)
+
+        # init DataProcessor
+        self.data_processor = TwitterDataProcessor()
+
+    def _handle_output(self, output: dict) -> Any:
+        """Returns either the single value from one-key dictionary or the dictionary itself.
+
+        Args:
+            output (dict): Input dictionary, usually the output of a function.
+
+        Returns:
+            Any: Either the single value from one-key dictionary or the dictionary itself.
+        """
+        # if output has only one key
+        if len(output) == 1:
+            # return single value
+            return next(iter(output.values()))
+        else:
+            # else return original output
+            return output
+
+    def user_info(self, user: str | int, attributes: List[LITERALS_USER_INFO] | str, return_timestamp: bool = False) -> Any:
+        """Receive requested user information from Twitter User Object.
+
+        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
+
+        Args:
+            user (str | int): Twitter User either specified by corresponding ID or screen name.
+            attributes (List[str] | str): Attributes of the User object. These must be from: id, id_str, name, screen_name, followers, followees, location, description, url, entities, protected, followers_count, friends_count, listed_count, created_at, latest_activity, last_active, liked_tweets, composed_tweets, favourites_count, verified, statuses_count, status, contributors_enabled, profile_image_url_https, profile_banner_url, default_profile, default_profile_image, withheld_in_countries, bot_scores
+            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
+
+        Raises:
+            KeyError: If invalid attribute was provided.
+            ValueError: If Botometer secrets were not provided.
+
+        Returns:
+            dict: Requested user information.
+
+        References: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#user_info
+        """
+        # catch Botometer API secrets before iteration over attributes.
+        if "bot_scores" in attributes:
+            if (self._x_rapidapi_key is None) or (self._x_rapidapi_host is None):
+                raise ValueError("'X_RAPIDAPI_KEY' and 'X_RAPIDAPI_HOST' secrets for Botometer API need to be provided.")
+
+        # initialize empty dict to store requested attributes
+        user_info = dict()
+        # if single string was provided
+        if isinstance(attributes, str):
+            # convert to list for iteration
+            attributes = [attributes]
+        # get user object
+        user_obj = self.fetcher.get_user_object(user)
+        # loop through the list of attributes and add them to the dictionary
+        for attr in attributes:
+            # if invalid attribute was provided
+            if attr not in get_args(self.LITERALS_USER_INFO):
+                raise ValueError("Invalid attribute for '{}'".format(attr))
+            # if the desired attribute is in default user object returned by the v1 Search API
+            elif attr in user_obj._json.keys():
+                user_info[attr] = user_obj._json[attr]
+            # get information about user's followers
+            elif attr == "followers":
+                user_info[attr] = self.data_processor.extract_followers(user_obj)
+            # get information about user's followees
+            elif attr == "followees":
+                user_info[attr] = self.data_processor.extract_followees(user_obj)
+            # get all liked tweets of user
+            elif attr == "liked_tweets":
+                # get page results first
+                liked_tweets = self.fetcher.get_liked_tweets_ids(user)
+                user_info[attr] = liked_tweets
+            # get all composed tweets
+            elif attr == "composed_tweets":
+                # get page results first
+                composed_tweets = self.fetcher.get_composed_tweets_ids(user)
+                user_info[attr] = composed_tweets
+            # get user's latest activity
+            elif attr == "latest_activity":
+                user_info[attr] = self.fetcher.get_latest_activity(user)
+            # get user's latest activity date
+            elif attr == "last_active":
+                user_info[attr] = self.fetcher.get_latest_activity_date(user)
+            # get user's botometer scores
+            elif attr == "bot_scores":
+                user_info[attr] = self.fetcher.get_botometer_scores(user)
+            # if attribute was not found
+            else:
+                user_info[attr] = None
+            # if timestamp should be returned
+        if return_timestamp:
+            user_info["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
+
+        return self._handle_output(user_info)
+
+    def compare_users(self, users: List[str | int], compare: str | List[LITERALS_COMPARE_USERS], return_timestamp: bool = False, features: List[str] | None = None) -> Any:
+        """Compare two or more users with the specified comparison attribute(s).
+
+        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
+
+        Args:
+            users (List[str  |  int]): User IDs or screen names
+            compare (str): Comparison attribute. Must be from: relationship, followers_count, followees_count, tweets_count, favourites_count, common_followers, distinct_followers, common_followees, distinct_followees, commonly_liked_tweets, distinctly_liked_tweets, similarity, created_at, protected, verified.
+            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
+            features (List[str] | None, optional): Defined features of Twitter User Object on which similarity will be computed. Must be from: followers_count, friends_count, listed_count, favourites_count, statuses_count. Defaults to None.
+
+        Raises:
+            ValueError: If invalid comparison attribute was provided.
+
+        Returns:
+            dict | list: Results of requested comparison attribute(s).
+
+        Referencs: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#compare_users
+        """
+        # users list must contain at least two elements
+        assert len(users) > 1, "'users' list must contain at least two elements, {} was/were provided".format(len(users))
+
+        # catch if feature vector contains only numeric values, and contains at least two elements
+        if features:
+            assert len(features) > 1, "'features' list must have at least two elements. {} was/were given".format(len(features))
+            for feat in features:
+                if feat not in get_args(self.SIMILARITY_FEATURES_COMPARE_USERS):
+                    raise ValueError(f"Only numeric features are supported. Must be from: {', '.join(get_args(self.SIMILARITY_FEATURES_COMPARE_USERS))}. You passed in {feat}")
+
+        # if single comparison attribute was provided as string
+        if isinstance(compare, str):
+            # change to list object
+            compare = [compare]
+        # init empty dict to store results
+        results = dict()
+        # iterate over comparison attributes
+        for attr in compare:
+            # if invalid attribute was provided
+            if attr not in get_args(self.LITERALS_COMPARE_USERS):
+                raise ValueError("Invalid attribute for '{}'".format(attr))
+            # match comparison attributes
+            match attr:
+                # compare relationships between two users
+                case "relationship":
+                    results[attr] = self.fetcher.get_relationship_pairs(users)
+                # compare number of followers
+                case "followers_count":
+                    # get individual followers
+                    followers = {user: self.fetcher.get_user_object(user).followers_count for user in users}
+                    # add descriptive metrics
+                    followers_with_metrics = self.data_processor.calc_descriptive_metrics(followers)
+                    results[attr] = followers_with_metrics
+                # compare number of friends
+                case "followees_count":
+                    # get individual followees
+                    followees = {user: self.fetcher.get_user_object(user).friends_count for user in users}
+                    # add descriptive metrics
+                    followees = self.data_processor.calc_descriptive_metrics(followees)
+                    results[attr] = followees
+                # compare number of Tweets issued by each user
+                case "tweets_count":
+                    # get individual statuses counts
+                    tweets = {user: self.fetcher.get_user_object(user).statuses_count for user in users}
+                    # add descriptive metrics
+                    tweets = self.data_processor.calc_descriptive_metrics(tweets)
+                    results[attr] = tweets
+                # compare number of likes issued by each user
+                case "favourites_count":
+                    # get individual likes
+                    likes = {user: self.fetcher.get_user_object(user).favourites_count for user in users}
+                    # add descriptive metrics
+                    likes = self.data_processor.calc_descriptive_metrics(likes)
+                    results[attr] = likes
+                # compare protected attribute of users
+                case "protected":
+                    results[attr] = {user: self.fetcher.get_user_object(user).protected for user in users}
+                # compare verified attribute for users
+                case "verified":
+                    results[attr] = {user: self.fetcher.get_user_object(user).verified for user in users}
+                # get common followers
+                case "common_followers":
+                    # get individual followers first
+                    individual_followers = [self.fetcher.get_user_follower_ids(user) for user in users]
+                    # get common followers by calculating the intersection
+                    common_followers = self.data_processor.intersection(individual_followers)
+                    results[attr] = common_followers
+                # get distinct followers
+                case "distinct_followers":
+                    # get individual followers first
+                    individual_followers = {user: self.fetcher.get_user_follower_ids(user) for user in users}
+                    # get distinct followers by calculating the difference of each set
+                    distinct_followers = self.data_processor.difference(individual_followers)
+                    results[attr] = distinct_followers
+                # get common followees
+                case "common_followees":
+                    # get individual followees first
+                    individual_followees = [self.fetcher.get_user_followee_ids(user) for user in users]
+                    # get common followees by calculating the intersection
+                    common_followees = self.data_processor.intersection(individual_followees)
+                    results[attr] = common_followees
+                # get distinct followees
+                case "distinct_followees":
+                    # get individual followees first
+                    individual_followees = {user: self.fetcher.get_user_followee_ids(user) for user in users}
+                    # get distinct followees by calculating the difference of each set
+                    distinct_followees = self.data_processor.difference(individual_followees)
+                    results[attr] = distinct_followees
+                # get common liked tweets
+                case "commonly_liked_tweets":
+                    # get individual liked tweets first
+                    individual_likes = [self.fetcher.get_liked_tweets_ids(user) for user in users]
+                    # get common liked tweets by calculating the intersection
+                    common_likes = self.data_processor.intersection(individual_likes)
+                    results[attr] = common_likes
+                # get distinct liked tweets
+                case "distinctly_liked_tweets":
+                    # get individual liked tweets first
+                    individual_likes = {user: self.fetcher.get_liked_tweets_ids(user) for user in users}
+                    # get distinct liked tweets by calculating the difference for each set
+                    distinct_likes = self.data_processor.difference(individual_likes)
+                    results[attr] = distinct_likes
+                # compute similarity between two users basd on the defined features
+                case "similarity":
+                    # feature list object must be defined
+                    if features is None:
+                        raise ValueError("'features' list must be provided.")
+                    # get serialized user objects first
+                    user_objs = [self.fetcher.get_user_object(user)._json for user in users]
+                    # calculate similarity based on defined feature vector
+                    results[attr] = self.data_processor.calc_similarity(user_objs=user_objs, features=features)
+                # compare creaation dates
+                case "created_at":
+                    # get individual creation dates first
+                    creation_dates = {user: self.fetcher.get_user_object(user).created_at for user in users}
+                    # add datetime metrics
+                    creation_dates = self.data_processor.calc_datetime_metrics(creation_dates)
+                    results[attr] = creation_dates
+                # if comparison attribute was not found
+                case _:
+                    results[attr] = None
+        # if timestamp should be returned
+        if return_timestamp:
+            results["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
+
+        return self._handle_output(results)
+
+    def tweet_info(self, tweet_id: str | int, attributes: List[LITERALS_TWEET_INFO] | str, return_timestamp: bool = False) -> Any:
+        """Receive requested Tweet information from Tweet Object.
+
+        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
+
+        Args:
+            tweet_id (str | int): Tweet ID
+            attributes (List[LITERALS_TWEET_INFO] | str): Attributes of the Tweet object. These must be from: id, id_str, full_text, display_text_range, truncated, created_at, entities, tweet_annotations, source, retweeters, in_reply_to_status_id, in_reply_to_status_id_str, in_reply_to_user_id, in_reply_to_user_id_str, in_reply_to_screen_name, user, contributors, coordinates, place, is_quote_status, public_metrics, quoting_users, liking_users, favorited, retweeted, retweeted_status, possibly_sensitive, lang, sentiment.
+            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
+
+        Raises:
+            ValueError: If invalid attribute was provided.
+
+        Returns:
+            dict: Requested Tweet information.
+
+        References: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#tweet_info
+        """
+        # get tweet object
+        tweet_obj = self.fetcher.get_tweet_object(tweet_id)
+
+        # initialize empty dict to store request information
+        tweet_info = dict()
+
+        # if single string was provided
+        if isinstance(attributes, str):
+            # convert to list for iteration
+            attributes = [attributes]
+        for attr in attributes:
+            # if invalid attribute was provided
+            if attr not in get_args(self.LITERALS_TWEET_INFO):
+                raise ValueError("Invalid attribute for '{}'".format(attr))
+            # get default attributes from tweepy Status model
+            elif attr in tweet_obj._json.keys():
+                tweet_info[attr] = tweet_obj._json[attr]
+            # get all quoting users
+            elif attr == "quoting_users":
+                quoting_users = self.fetcher.get_quoting_users_ids(tweet_id)
+                tweet_info[attr] = quoting_users
+            # get all liking users
+            elif attr == "liking_users":
+                liking_users = self.fetcher.get_liking_users_ids(tweet_id)
+                tweet_info[attr] = liking_users
+            # get all retweeters
+            elif attr == "retweeters":
+                retweeters = self.fetcher.get_retweeters_ids(tweet_id)
+                tweet_info[attr] = retweeters
+            # get public metrics
+            elif attr == "public_metrics":
+                tweet_info[attr] = self.fetcher.get_public_metrics(tweet_id)
+            # get context annotations
+            elif attr == "tweet_annotations":
+                tweet_info[attr] = self.fetcher.get_context_annotations_and_entities(tweet_id)
+            # get tweet sentiment
+            elif attr == "sentiment":
+                tweet_info[attr] = self.data_processor.detect_tweet_sentiment(tweet_obj.full_text)
+            # if attribute was not found
+            else:
+                tweet_info[attr] = None
+        # if timestamp should be returned
+        if return_timestamp:
+            tweet_info["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
+
+        return self._handle_output(tweet_info)
+
+    def compare_tweets(self, tweet_ids: List[str | int], compare: str | List[LITERALS_COMPARE_TWEETS], return_timestamp: bool = False, features: List[str] | None = None) -> Any:
+        """Compare two or more Tweets with the specified comparison attribute.
+
+        For one attribute, only the corresponding value is returned. For multiple attributes, a dictionary with the key-value pairs of the requested attributes is returned.
+
+        Args:
+            tweets (List[str  |  int]): List of Tweet IDs.
+            compare (str | List[LITERALS_COMPARE_TWEETS]): Comparison attribute. Needs to be from the following: view_count, like_count, retweet_count, quote_count, reply_count, common_quoting_users, distinct_quoting_users, common_liking_users, distinct_liking_users, common_retweeters, distinct_retweeters, similarity, created_at.
+            return_timestamp (bool, optional): Add UTC Timestamp to results. Defaults to False.
+            features (List[str] | None, optional): Defined features of Twitter User Object on which similarity will be computed. Must be from: retweet_count, reply_count, like_count, quote_count, impression_count. Defaults to None.
+
+        Raises:
+            AssertionError: If a list of one Tweet ID was provided.
+            ValueError: If invalid comparison attribute was provided.
+
+        Returns:
+            dict: Requested results for comparison attribute.
+
+        References: https://mathun3003.github.io/PySNA/user-guide/overview/TwitterAPI/#compare_tweets
+        """
+        # tweets list must contain at least two IDs
+        assert len(tweet_ids) > 1, "'tweets' list object needs at least two entries, not {}".format(len(tweet_ids))
+
+        # catch if feature vector contains only numeric values, and contains at least two elements
+        if features:
+            assert len(features) > 1, "'features' list must have at least two elements. {} was/were given".format(len(features))
+            for feat in features:
+                if feat not in get_args(self.SIMILARITY_FEATURES_COMPARE_TWEETS):
+                    raise ValueError(f"Only numeric features are supported. Must be from: {', '.join(get_args(self.SIMILARITY_FEATURES_COMPARE_TWEETS))}. You passed in {feat}.")
+
+        # if single comparison attribute was provided as string
+        if isinstance(compare, str):
+            # change to list object
+            compare = [compare]
+        # init empty dict to store results
+        results = dict()
+        # iterate over every given comparison atttribute
+        for attr in compare:
+            # if invalid attribute was provided
+            if attr not in get_args(self.LITERALS_COMPARE_TWEETS):
+                raise ValueError("Invalid attribute for '{}'".format(attr))
+            # match comparison attribute
+            match attr:
+                # compare numer of views / impressions
+                case "view_count":
+                    # get individual view_counts
+                    view_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["impression_count"] for tweet_id in tweet_ids}
+                    # add descriptive metrics
+                    view_counts = self.data_processor.calc_descriptive_metrics(view_counts)
+                    results[attr] = view_counts
+                # compare number of likes
+                case "like_count":
+                    # get individual like_counts
+                    like_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["like_count"] for tweet_id in tweet_ids}
+                    # add descriptive metrics
+                    like_counts = self.data_processor.calc_descriptive_metrics(like_counts)
+                    results[attr] = like_counts
+                # compare number or retweets
+                case "retweet_count":
+                    # get individual number of retweets
+                    retweet_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["retweet_count"] for tweet_id in tweet_ids}
+                    # add descriptive metrics
+                    retweet_counts = self.data_processor.calc_descriptive_metrics(retweet_counts)
+                    results[attr] = retweet_counts
+                # compare number of quotes
+                case "quote_count":
+                    # get individual number of quotes
+                    quote_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["quote_count"] for tweet_id in tweet_ids}
+                    # add descriptive metrics
+                    quote_counts = self.data_processor.calc_descriptive_metrics(quote_counts)
+                    results[attr] = quote_counts
+                # compare number of commonts
+                case "reply_count":
+                    # get individual number of replies first
+                    reply_counts = {tweet_id: self.fetcher.get_public_metrics(tweet_id)["reply_count"] for tweet_id in tweet_ids}
+                    # add descriptive metrics
+                    reply_counts = self.data_processor.calc_descriptive_metrics(reply_counts)
+                    results[attr] = reply_counts
+                # get all quoting users all Tweets have in common
+                case "common_quoting_users":
+                    # get individual quoting users first
+                    quoting_users = [self.fetcher.get_quoting_users_ids(tweet_id) for tweet_id in tweet_ids]
+                    # get common quoting users by calculating the intersection
+                    common_quoting_users = self.data_processor.intersection(quoting_users)
+                    # return quoting users
+                    results[attr] = common_quoting_users
+                # get distinct quoting users for each tweet
+                case "distinct_quoting_users":
+                    # get individual quoting users first
+                    quoting_users = {tweet_id: self.fetcher.get_quoting_users_ids(tweet_id) for tweet_id in tweet_ids}
+                    # get distinct quoting users for each tweet by calculating the difference for each set
+                    distinct_quoting_users = self.data_processor.difference(quoting_users)
+                    results[attr] = distinct_quoting_users
+                # get all liking users that all tweets have in common
+                case "common_liking_users":
+                    # get individual liking users first
+                    liking_users = [self.fetcher.get_liking_users_ids(tweet_id) for tweet_id in tweet_ids]
+                    # get common liking users by calculating the intersection
+                    common_liking_users = self.data_processor.intersection(liking_users)
+                    # return common liking users
+                    results[attr] = common_liking_users
+                # get distinct liking users of all tweets
+                case "distinct_liking_users":
+                    # get individual liking users first
+                    liking_users = {tweet_id: self.fetcher.get_liking_users_ids(tweet_id) for tweet_id in tweet_ids}
+                    # get distinct liking users for each tweet by calculating the difference for each set
+                    distinct_liking_users = self.data_processor.difference(liking_users)
+                    results[attr] = distinct_liking_users
+                # get all retweeters all tweets have in common
+                case "common_retweeters":
+                    # get individual retweeters first
+                    retweeters = [self.fetcher.get_retweeters_ids(tweet_id) for tweet_id in tweet_ids]
+                    # get common retweeters by calculating the intersection
+                    common_retweeters = self.data_processor.intersection(retweeters)
+                    # return common retweeters
+                    results[attr] = common_retweeters
+                # get distinct retweeters of all tweets
+                case "distinct_retweeters":
+                    # get individual retweeters first
+                    retweeters = {tweet_id: self.fetcher.get_retweeters_ids(tweet_id) for tweet_id in tweet_ids}
+                    # get distinct retweeters by calculating the difference for each set
+                    distinct_retweeters = self.data_processor.difference(retweeters)
+                    results[attr] = distinct_retweeters
+                # compute similarity between two tweets basd on the defined features
+                case "similarity":
+                    # feature list object must be defined
+                    if features is None:
+                        raise ValueError("'features' list must be provided.")
+                    # get public metrics for Tweet objects first
+                    public_metrics = {tweet_id: self.fetcher.get_public_metrics(tweet_id) for tweet_id in tweet_ids}
+                    # calculate similarity based on defined feature vector
+                    results[attr] = self.data_processor.calc_similarity(tweet_metrics=public_metrics, features=features)
+                # compare creation dates of tweets
+                case "created_at":
+                    # get individual creation dates first
+                    creation_dates = {tweet_id: self.fetcher.get_tweet_object(tweet_id).created_at for tweet_id in tweet_ids}
+                    # add datetime metrics
+                    creation_dates = self.data_processor.calc_datetime_metrics(creation_dates)
+                    results[attr] = creation_dates
+                # if attribute was not found
+                case _:
+                    results[attr] = None
+        # if UTC timestamp should be returned
+        if return_timestamp:
+            results["utc_timestamp"] = strf_datetime(datetime.utcnow(), format="%Y-%m-%d %H:%M:%S.%f")
+
+        return self._handle_output(results)
```

### Comparing `pysna-0.1.1/pysna/cli.py` & `pysna-0.1.2/pysna/cli.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,288 +1,288 @@
-# -*- coding: utf-8 -*-
-import argparse
-import json
-import os
-import pathlib
-import re
-import shutil
-from typing import get_args
-
-from dotenv import load_dotenv
-
-from pysna.api import TwitterAPI
-from pysna.utils import append_to_csv, append_to_json, export_to_csv, export_to_json
-
-msg = """
-The command-line interface for the PySNA package
-
-Reference: https://mathun3003.github.io/PySNA/user-guide/overview/cli/
-
-Usage:
-  pysna set-secrets <path>
-  pysna user-info <user> <attributes> [--return-timestamp] [--output] [--append] [--encoding] [--env]
-  pysna compare-users <users> -c <compare> [--features] [--return-timestamp] [--output] [--append] [--encoding] [--env]
-  pysna tweet-info <tweet> <attributes> [--return-timestamp] [--output] [--append] [--encoding] [--env]
-  pysna compare-tweets <tweets> -c <compare> [--features] [--return-timestamp] [--output] [--append] [--encoding] [--env]
-
-Options:
-  -h --help        Show this screen.
-  --version        Show version.
-"""
-
-# get version from __init__.py
-HERE = pathlib.Path(__file__).parent
-VERSION_FILE = f"{HERE}/__init__.py"
-with open(VERSION_FILE) as version_file:
-    match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file.read(), re.MULTILINE)
-
-if match:
-    version = match.group(1)
-else:
-    raise RuntimeError(f"Unable to find version string in {VERSION_FILE}.")
-
-# set constant for required and optional secrets
-REQUIRED_SECRETS = ["BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET"]
-OPTIONAL_SECRETS = ["X_RAPIDAPI_KEY", "X_RAPIDAPI_HOST"]
-# set config file path under "~/.pysna/config/secrets.env"
-config_file_path = os.path.join(os.path.expanduser("~"), ".pysna", "config", "secrets.env")
-
-# set main parser
-parser = argparse.ArgumentParser(prog="pysna", usage=msg)
-# set subparser
-subparsers = parser.add_subparsers(dest="subcommand")
-# add version argument
-parser.add_argument("--version", action="version", version="%(prog)s {version}".format(version=version))
-
-
-def read_secrets(env_path: str) -> dict:
-    if not os.path.exists(env_path):
-        raise Exception("No config file found for secrets. Use the 'set-secrets' function to create a config file or provide a .env file using the '--env' flag.")
-    else:
-        load_dotenv(env_path)
-        # catch environmental variables
-        for secret in REQUIRED_SECRETS:
-            if secret not in os.environ:
-                raise KeyError(f"{secret} must be provided in the environment variables.")
-        # collect secrets
-        secrets = {secret.lower(): os.getenv(secret) for secret in REQUIRED_SECRETS + OPTIONAL_SECRETS}
-        return secrets
-
-
-def output(data: dict, encoding: str, path: str | None = None, append: bool = False):
-    # either print results if '--output' arg was provided
-    if (path is not None) and (append is False):
-        if path.endswith(".json"):
-            export_to_json(data, path, encoding)
-        elif path.endswith(".csv"):
-            export_to_csv(data, path, encoding)
-    # or append to existing file
-    elif (path is not None) and (append is True):
-        if path.endswith(".json"):
-            append_to_json(data, path, encoding)
-        elif path.endswith(".csv"):
-            append_to_csv(data, path, encoding)
-    # or print them to the CLI in JSON format
-    else:
-        print(json.dumps(data, ensure_ascii=False))
-    pass
-
-
-def argument(*name_or_flags, **kwargs):
-    """Convenience function to properly format arguments to pass to the subcommand decorator."""
-    return (list(name_or_flags), kwargs)
-
-
-def subcommand(function_name: str, args=[], parent=subparsers):
-    """Decorator to define a new subcommand in a sanity-preserving way.
-    The function will be stored in the ``func`` variable when the parser
-    parses arguments so that it can be called directly like so::
-        args = cli.parse_args()
-        args.func(args)
-    Usage example::
-        @subcommand([argument("-d", help="Enable debug mode", action="store_true")])
-        def subcommand(args):
-            print(args)
-    Then on the command line::
-        $ python cli.py subcommand -d
-    """
-
-    def decorator(func):
-        parser = parent.add_parser(function_name, description=func.__doc__)
-        for arg in args:
-            parser.add_argument(*arg[0], **arg[1])
-        parser.set_defaults(func=func)
-
-    return decorator
-
-
-@subcommand("set-secrets", args=[argument("secrets_file", type=str, help="Path to the secrets file. Only .env files are supported.")])
-def set_secrets(args):
-    """CLI function to set or overwrite a config file for storing API secrets. Config file will be set to '~/.pysna/config/secrets.env'."""
-    if not args.secrets_file.endswith(".env"):
-        raise Exception("Only .env files are supported. Please pass in a .env file.")
-    # check .env file format
-    load_dotenv(args.secrets_file)
-    for secret in REQUIRED_SECRETS:
-        if secret not in os.environ:
-            raise Exception(
-                f"{secret} must be provided in the {args.secrets_file} file."
-                f"\nMake sure that your {args.secrets_file} has the following format:"
-                f"\nBEARER_TOKEN=...\nCONSUMER_KEY=...\nCONSUMER_SECRET=...\nACCESS_TOKEN=...\nACCESS_TOKEN_SECRET=..."
-                f"\nIf you wish to use the Botometer API, also provide the {', '.join(OPTIONAL_SECRETS)} keys in the {args.secrets_file} file."
-            )
-    # create folders if it does not exist yet
-    os.makedirs(os.path.dirname(config_file_path), exist_ok=True)
-    # copy file content from args.secrets_file to config file path
-    shutil.copy2(args.secrets_file, config_file_path)
-    print(f"Secrets from {args.secrets_file} file were set.")
-
-
-@subcommand(
-    "user-info",
-    args=[
-        argument("user", help="Twitter User ID or screen name"),
-        argument("attributes", nargs="+", default=[], help=f"List or string of desired User attributes. Must be from {', '.join(get_args(TwitterAPI.LITERALS_USER_INFO))}"),
-        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
-        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
-        argument(
-            "--output",
-            "-o",
-            type=str,
-            default=None,
-            required=False,
-            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
-        ),
-        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
-        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
-    ],
-)
-def user_info_cli(args):
-    """CLI function to request information from the specified Twitter user."""
-    # read secrets
-    secrets = read_secrets(args.env)
-    # establish connection to the API
-    api = TwitterAPI(**secrets)
-    # get results
-    result = api.user_info(user=args.user, attributes=args.attributes, return_timestamp=args.return_timestamp)
-    # handle output
-    output(result, path=args.output, encoding=args.encoding, append=args.append)
-    pass
-
-
-@subcommand(
-    "tweet-info",
-    args=[
-        argument("tweet_id", help="Tweet ID"),
-        argument("attributes", nargs="+", default=[], help=f"List or string of desired Tweet attribute. Must be from {', '.join(get_args(TwitterAPI.LITERALS_TWEET_INFO))}"),
-        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
-        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
-        argument(
-            "--output",
-            "-o",
-            type=str,
-            default=None,
-            required=False,
-            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
-        ),
-        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
-        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
-    ],
-)
-def tweet_info_cli(args):
-    """CLI function to request information from the specified Tweet."""
-    # read secrets
-    secrets = read_secrets(args.env)
-    # establish connection to the API
-    api = TwitterAPI(**secrets)
-    # get results
-    result = api.tweet_info(tweet_id=args.tweet_id, attributes=args.attributes, return_timestamp=args.return_timestamp)
-    # handle output
-    output(result, path=args.output, encoding=args.encoding, append=args.append)
-    pass
-
-
-@subcommand(
-    "compare-users",
-    args=[
-        argument("users", nargs="+", default=[], help="The IDs or screen names of the users."),
-        argument("--compare", "-c", nargs="+", default=[], required=True, help=f"The comparison attribute(s). Must be from following: {', '.join(get_args(TwitterAPI.LITERALS_COMPARE_USERS))}."),
-        argument(
-            "--features",
-            "-f",
-            nargs="+",
-            default=[],
-            required=False,
-            help=f"Features that should be contained in the feature vector for similarity comparison. Must be from: {', '.join(get_args(TwitterAPI.SIMILARITY_FEATURES_COMPARE_USERS))}",
-        ),
-        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
-        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
-        argument(
-            "--output",
-            "-o",
-            type=str,
-            default=None,
-            required=False,
-            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
-        ),
-        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
-        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
-    ],
-)
-def compare_users_cli(args):
-    """CLI function to compare multiple Twitter users with the specified comparision attribute(s)."""
-    # read secrets
-    secrets = read_secrets(args.env)
-    # establish connection to the API
-    api = TwitterAPI(**secrets)
-    # get results
-    result = api.compare_users(users=args.users, compare=args.compare, return_timestamp=args.return_timestamp, features=args.features)
-    # handle output
-    output(result, path=args.output, encoding=args.encoding, append=args.append)
-    pass
-
-
-@subcommand(
-    "compare-tweets",
-    args=[
-        argument("tweets", nargs="+", default=[], help="The IDs of the Tweets."),
-        argument("--compare", "-c", nargs="+", default=[], required=True, help=f"The comparison attribute(s). Must be the following: {', '.join(get_args(TwitterAPI.LITERALS_COMPARE_TWEETS))}."),
-        argument(
-            "--features", "-f", nargs="+", default=[], required=False, help=f"Features that should be contained in the feature vector for similarity comparison. Must be from: {', '.join(get_args(TwitterAPI.SIMILARITY_FEATURES_COMPARE_TWEETS))}"
-        ),
-        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
-        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
-        argument(
-            "--output",
-            "-o",
-            type=str,
-            default=None,
-            required=False,
-            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
-        ),
-        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
-        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
-    ],
-)
-def compare_tweets_cli(args):
-    """CLI function to compare multiple Tweets with the specified comparision attribute(s)."""
-    # read secrets
-    secrets = read_secrets(args.env)
-    # establish connection to the API
-    api = TwitterAPI(**secrets)
-    # get results
-    result = api.compare_tweets(tweet_ids=args.tweets, compare=args.compare, return_timestamp=args.return_timestamp, features=args.features)
-    # handle output
-    output(result, path=args.output, encoding=args.encoding, append=args.append)
-    pass
-
-
-def main():
-    args = parser.parse_args()
-    if args.subcommand is None:
-        parser.print_help()
-    else:
-        args.func(args)
-
-
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+import argparse
+import json
+import os
+import pathlib
+import re
+import shutil
+from typing import get_args
+
+from dotenv import load_dotenv
+
+from pysna.api import TwitterAPI
+from pysna.utils import append_to_csv, append_to_json, export_to_csv, export_to_json
+
+msg = """
+The command-line interface for the PySNA package
+
+Reference: https://mathun3003.github.io/PySNA/user-guide/overview/cli/
+
+Usage:
+  pysna set-secrets <path>
+  pysna user-info <user> <attributes> [--return-timestamp] [--output] [--append] [--encoding] [--env]
+  pysna compare-users <users> -c <compare> [--features] [--return-timestamp] [--output] [--append] [--encoding] [--env]
+  pysna tweet-info <tweet> <attributes> [--return-timestamp] [--output] [--append] [--encoding] [--env]
+  pysna compare-tweets <tweets> -c <compare> [--features] [--return-timestamp] [--output] [--append] [--encoding] [--env]
+
+Options:
+  -h --help        Show this screen.
+  --version        Show version.
+"""
+
+# get version from __init__.py
+HERE = pathlib.Path(__file__).parent
+VERSION_FILE = f"{HERE}/__init__.py"
+with open(VERSION_FILE) as version_file:
+    match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file.read(), re.MULTILINE)
+
+if match:
+    version = match.group(1)
+else:
+    raise RuntimeError(f"Unable to find version string in {VERSION_FILE}.")
+
+# set constant for required and optional secrets
+REQUIRED_SECRETS = ["BEARER_TOKEN", "CONSUMER_KEY", "CONSUMER_SECRET", "ACCESS_TOKEN", "ACCESS_TOKEN_SECRET"]
+OPTIONAL_SECRETS = ["X_RAPIDAPI_KEY", "X_RAPIDAPI_HOST"]
+# set config file path under "~/.pysna/config/secrets.env"
+config_file_path = os.path.join(os.path.expanduser("~"), ".pysna", "config", "secrets.env")
+
+# set main parser
+parser = argparse.ArgumentParser(prog="pysna", usage=msg)
+# set subparser
+subparsers = parser.add_subparsers(dest="subcommand")
+# add version argument
+parser.add_argument("--version", action="version", version="%(prog)s {version}".format(version=version))
+
+
+def read_secrets(env_path: str) -> dict:
+    if not os.path.exists(env_path):
+        raise Exception("No config file found for secrets. Use the 'set-secrets' function to create a config file or provide a .env file using the '--env' flag.")
+    else:
+        load_dotenv(env_path)
+        # catch environmental variables
+        for secret in REQUIRED_SECRETS:
+            if secret not in os.environ:
+                raise KeyError(f"{secret} must be provided in the environment variables.")
+        # collect secrets
+        secrets = {secret.lower(): os.getenv(secret) for secret in REQUIRED_SECRETS + OPTIONAL_SECRETS}
+        return secrets
+
+
+def output(data: dict, encoding: str, path: str | None = None, append: bool = False):
+    # either print results if '--output' arg was provided
+    if (path is not None) and (append is False):
+        if path.endswith(".json"):
+            export_to_json(data, path, encoding)
+        elif path.endswith(".csv"):
+            export_to_csv(data, path, encoding)
+    # or append to existing file
+    elif (path is not None) and (append is True):
+        if path.endswith(".json"):
+            append_to_json(data, path, encoding)
+        elif path.endswith(".csv"):
+            append_to_csv(data, path, encoding)
+    # or print them to the CLI in JSON format
+    else:
+        print(json.dumps(data, ensure_ascii=False))
+    pass
+
+
+def argument(*name_or_flags, **kwargs):
+    """Convenience function to properly format arguments to pass to the subcommand decorator."""
+    return (list(name_or_flags), kwargs)
+
+
+def subcommand(function_name: str, args=[], parent=subparsers):
+    """Decorator to define a new subcommand in a sanity-preserving way.
+    The function will be stored in the ``func`` variable when the parser
+    parses arguments so that it can be called directly like so::
+        args = cli.parse_args()
+        args.func(args)
+    Usage example::
+        @subcommand([argument("-d", help="Enable debug mode", action="store_true")])
+        def subcommand(args):
+            print(args)
+    Then on the command line::
+        $ python cli.py subcommand -d
+    """
+
+    def decorator(func):
+        parser = parent.add_parser(function_name, description=func.__doc__)
+        for arg in args:
+            parser.add_argument(*arg[0], **arg[1])
+        parser.set_defaults(func=func)
+
+    return decorator
+
+
+@subcommand("set-secrets", args=[argument("secrets_file", type=str, help="Path to the secrets file. Only .env files are supported.")])
+def set_secrets(args):
+    """CLI function to set or overwrite a config file for storing API secrets. Config file will be set to '~/.pysna/config/secrets.env'."""
+    if not args.secrets_file.endswith(".env"):
+        raise Exception("Only .env files are supported. Please pass in a .env file.")
+    # check .env file format
+    load_dotenv(args.secrets_file)
+    for secret in REQUIRED_SECRETS:
+        if secret not in os.environ:
+            raise Exception(
+                f"{secret} must be provided in the {args.secrets_file} file."
+                f"\nMake sure that your {args.secrets_file} has the following format:"
+                f"\nBEARER_TOKEN=...\nCONSUMER_KEY=...\nCONSUMER_SECRET=...\nACCESS_TOKEN=...\nACCESS_TOKEN_SECRET=..."
+                f"\nIf you wish to use the Botometer API, also provide the {', '.join(OPTIONAL_SECRETS)} keys in the {args.secrets_file} file."
+            )
+    # create folders if it does not exist yet
+    os.makedirs(os.path.dirname(config_file_path), exist_ok=True)
+    # copy file content from args.secrets_file to config file path
+    shutil.copy2(args.secrets_file, config_file_path)
+    print(f"Secrets from {args.secrets_file} file were set.")
+
+
+@subcommand(
+    "user-info",
+    args=[
+        argument("user", help="Twitter User ID or screen name"),
+        argument("attributes", nargs="+", default=[], help=f"List or string of desired User attributes. Must be from {', '.join(get_args(TwitterAPI.LITERALS_USER_INFO))}"),
+        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
+        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
+        argument(
+            "--output",
+            "-o",
+            type=str,
+            default=None,
+            required=False,
+            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
+        ),
+        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
+        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
+    ],
+)
+def user_info_cli(args):
+    """CLI function to request information from the specified Twitter user."""
+    # read secrets
+    secrets = read_secrets(args.env)
+    # establish connection to the API
+    api = TwitterAPI(**secrets)
+    # get results
+    result = api.user_info(user=args.user, attributes=args.attributes, return_timestamp=args.return_timestamp)
+    # handle output
+    output(result, path=args.output, encoding=args.encoding, append=args.append)
+    pass
+
+
+@subcommand(
+    "tweet-info",
+    args=[
+        argument("tweet_id", help="Tweet ID"),
+        argument("attributes", nargs="+", default=[], help=f"List or string of desired Tweet attribute. Must be from {', '.join(get_args(TwitterAPI.LITERALS_TWEET_INFO))}"),
+        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
+        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
+        argument(
+            "--output",
+            "-o",
+            type=str,
+            default=None,
+            required=False,
+            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
+        ),
+        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
+        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
+    ],
+)
+def tweet_info_cli(args):
+    """CLI function to request information from the specified Tweet."""
+    # read secrets
+    secrets = read_secrets(args.env)
+    # establish connection to the API
+    api = TwitterAPI(**secrets)
+    # get results
+    result = api.tweet_info(tweet_id=args.tweet_id, attributes=args.attributes, return_timestamp=args.return_timestamp)
+    # handle output
+    output(result, path=args.output, encoding=args.encoding, append=args.append)
+    pass
+
+
+@subcommand(
+    "compare-users",
+    args=[
+        argument("users", nargs="+", default=[], help="The IDs or screen names of the users."),
+        argument("--compare", "-c", nargs="+", default=[], required=True, help=f"The comparison attribute(s). Must be from following: {', '.join(get_args(TwitterAPI.LITERALS_COMPARE_USERS))}."),
+        argument(
+            "--features",
+            "-f",
+            nargs="+",
+            default=[],
+            required=False,
+            help=f"Features that should be contained in the feature vector for similarity comparison. Must be from: {', '.join(get_args(TwitterAPI.SIMILARITY_FEATURES_COMPARE_USERS))}",
+        ),
+        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
+        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
+        argument(
+            "--output",
+            "-o",
+            type=str,
+            default=None,
+            required=False,
+            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
+        ),
+        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
+        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
+    ],
+)
+def compare_users_cli(args):
+    """CLI function to compare multiple Twitter users with the specified comparision attribute(s)."""
+    # read secrets
+    secrets = read_secrets(args.env)
+    # establish connection to the API
+    api = TwitterAPI(**secrets)
+    # get results
+    result = api.compare_users(users=args.users, compare=args.compare, return_timestamp=args.return_timestamp, features=args.features)
+    # handle output
+    output(result, path=args.output, encoding=args.encoding, append=args.append)
+    pass
+
+
+@subcommand(
+    "compare-tweets",
+    args=[
+        argument("tweets", nargs="+", default=[], help="The IDs of the Tweets."),
+        argument("--compare", "-c", nargs="+", default=[], required=True, help=f"The comparison attribute(s). Must be the following: {', '.join(get_args(TwitterAPI.LITERALS_COMPARE_TWEETS))}."),
+        argument(
+            "--features", "-f", nargs="+", default=[], required=False, help=f"Features that should be contained in the feature vector for similarity comparison. Must be from: {', '.join(get_args(TwitterAPI.SIMILARITY_FEATURES_COMPARE_TWEETS))}"
+        ),
+        argument("--env", "-e", type=str, default=config_file_path, required=False, help=f"Path to .env file. Defaults to {config_file_path}."),
+        argument("--return-timestamp", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Returns the UTC timestamp of the request."),
+        argument(
+            "--output",
+            "-o",
+            type=str,
+            default=None,
+            required=False,
+            help="Store results in a JSON or CSV file. Specify output file path (including file name). File extension specifies file export (e.g., '.csv' for CSV file export and '.json' for JSON file export)",
+        ),
+        argument("--encoding", type=str, default="utf-8", required=False, help="Encoding of the output file. Defaults to UTF-8."),
+        argument("--append", "-a", type=bool, default=False, required=False, action=argparse.BooleanOptionalAction, help="Add results to an existing JSON file. File needs to be specified in the --output flag."),
+    ],
+)
+def compare_tweets_cli(args):
+    """CLI function to compare multiple Tweets with the specified comparision attribute(s)."""
+    # read secrets
+    secrets = read_secrets(args.env)
+    # establish connection to the API
+    api = TwitterAPI(**secrets)
+    # get results
+    result = api.compare_tweets(tweet_ids=args.tweets, compare=args.compare, return_timestamp=args.return_timestamp, features=args.features)
+    # handle output
+    output(result, path=args.output, encoding=args.encoding, append=args.append)
+    pass
+
+
+def main():
+    args = parser.parse_args()
+    if args.subcommand is None:
+        parser.print_help()
+    else:
+        args.func(args)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pysna-0.1.1/pysna/fetch.py` & `pysna-0.1.2/pysna/fetch.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,489 +1,489 @@
-# -*- coding: utf-8 -*-
-import logging
-import sys
-from typing import Any, Dict, List, Set
-
-import requests
-import tweepy
-
-# create logger instance
-log = logging.getLogger(__name__)
-# log to stdout
-handler = logging.StreamHandler(sys.stdout)
-handler.setLevel(logging.ERROR)
-formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-handler.setFormatter(formatter)
-log.addHandler(handler)
-
-
-class TwitterDataFetcher:
-    """Composition class in order to fetch data from the Twitter Search API v1 and v2."""
-
-    def __init__(
-        self,
-        bearer_token: Any | None = None,
-        consumer_key: Any | None = None,
-        consumer_secret: Any | None = None,
-        access_token: Any | None = None,
-        access_token_secret: Any | None = None,
-        x_rapidapi_key: Any | None = None,
-        x_rapidapi_host: Any | None = None,
-        wait_on_rate_limit: bool = True,
-    ):
-        self._bearer_token = bearer_token
-        self._consumer_key = consumer_key
-        self._consumer_secret = consumer_secret
-        self._access_token = access_token
-        self._access_token_secret = access_token_secret
-        self._x_rapidapi_key = x_rapidapi_key
-        self._x_rapidapi_host = x_rapidapi_host
-        self._wait_on_rate_limit = wait_on_rate_limit
-
-        self.api = tweepy.API(tweepy.AppAuthHandler(consumer_key=self._consumer_key, consumer_secret=self._consumer_secret), wait_on_rate_limit=self._wait_on_rate_limit)
-
-        self.client = tweepy.Client(
-            bearer_token=self._bearer_token, consumer_key=self._consumer_key, consumer_secret=self._consumer_secret, access_token=self._access_token, access_token_secret=self._access_token_secret, wait_on_rate_limit=self._wait_on_rate_limit
-        )
-
-    def _manual_request(self, url: str, method: str = "GET", header: dict | None = None, payload: dict | None = None, additional_fields: Dict[str, List[str]] | None = None) -> dict:
-        """Perform a manual request to the Twitter API.
-
-        Args:
-            url (str): API URL (without specified fields)
-            method (str): Request method according to REST. Defaults to "GET".
-            header (dict | None): Custom HTTP Header. Defaults to None.
-            payload (dict | None): JSON data for HTTP requests. Defaults to None.
-            additional_fields (Dict[str, List[str]] | None, optional): Fields can be specified (e.g., tweet.fields) according to the official API reference. Defaults to None.
-
-        Raises:
-            Exception: If status code != 200.
-
-        Returns:
-            dict: JSON formatted response of API request.
-        """
-        # if additional_fields were provided
-        if additional_fields:
-            # init empty string
-            fields = "?"
-            # create fields string dynamically for every field in additional_fields
-            for field in additional_fields.keys():
-                # e.g., in format "tweet.fields=lang,author_id"
-                fields += f"{field}={','.join(additional_fields[field])}&"
-            # append fields to url
-            url += fields[:-1]
-        if header is None:
-            # set header
-            header = {"Authorization": f"Bearer {self._bearer_token}"}
-        response = requests.request(method=method, url=url, headers=header, json=payload)
-        if response.status_code != 200:
-            raise Exception("Request returned an error: {} {}".format(response.status_code, response.text))
-        return response.json()
-
-    def _paginate(self, func, params: Dict[str, str | int], limit: int | None = None, response_attribute: str = "data", page_attribute: str | None = None) -> list:
-        """Pagination function
-
-        Args:
-            func: Function used for pagination
-            params (Dict[str, str  |  int]): Dict containing request parameters. Should be of the form {'id': ..., 'max_results': ..., 'pagination_token': ...}
-            limit (int | None, optional): Maximum number of results. Defaults to None, thus, no limit.
-            response_attribute (str, optional): Attribute of the Response object. Defaults to "data". Options: ["data", "includes"]
-            page_attribute (str, optional): The attribute that should be extracted for every entry of a page. Defaults to None.
-
-        Raises:
-            KeyError: 'id', 'max_results', and 'pagination_token' should be provided in the params dict.
-
-        Returns:
-            set: Results
-        """
-        # init counter
-        counter = 0
-        # init empty results set
-        results = list()
-        # set break out var
-        break_out = False
-        while not break_out:
-            # make request
-            response = func(**params)
-            # if any data exists
-            if response.__getattribute__(response_attribute) is not None:
-                # iterate over response results
-                for item in response.__getattribute__(response_attribute):
-                    # add result
-                    if page_attribute is None:
-                        results.append(item)
-                    else:
-                        results.append(item.__getattribute__(page_attribute))
-                    # increment counter
-                    counter += 1
-                    # if limit was reached, break
-                    if (limit is not None) and (counter == limit):
-                        # set break_out var to true
-                        break_out = True
-                        break
-                # if last page was reached
-                if "next_token" not in response.meta:
-                    break
-                # else, set new pagination token for next iteration
-                else:
-                    params["pagination_token"] = response.meta["next_token"]
-            # if no data exists, break
-            else:
-                break
-        return results
-
-    """ User Object data methods """
-
-    def get_user_object(self, user: str | int) -> tweepy.models.User:
-        """Request Twitter User Object via tweepy
-
-        Args:
-            user (str): Either User ID or screen name
-
-        Returns:
-            tweepy.User: Twitter User object from tweepy
-        """
-        try:
-            # check if string for user1 is convertible to int in order to check for user ID or screen name
-            if (isinstance(user, int)) or (user.isdigit()):
-                # get profile for user by user ID
-                user_obj = self.api.get_user(user_id=user)
-            else:
-                # get profile for user by screen name
-                user_obj = self.api.get_user(screen_name=user)
-        except tweepy.errors.Forbidden as e:
-            # log to stdout
-            log.error("403 Forbidden: access refused or access is not allowed.")
-            # if user ID was provided
-            if user.isdigit() or isinstance(user, int):
-                url = f"https://api.twitter.com/2/users/{user}"
-            else:
-                # if screen name was provided
-                url = f"https://api.twitter.com/2/users/by/username/{user}"
-            response = self._manual_request(url)
-            # if an error occured that says the user has been suspended
-            if any("User has been suspended" in error["detail"] for error in response["errors"]):
-                log.error("User has been suspended from Twitter. Requested user: {}".format(user))
-                raise e
-            else:
-                raise e
-        return user_obj
-
-    def get_user_follower_ids(self, user: str | int) -> Set[int]:
-        """Request Twitter follower IDs from user
-
-        Args:
-            user (str | int): Either User ID or screen name.
-
-        Returns:
-            Set[int]: Array containing follower IDs
-        """
-        # check if string for user1 is convertible to int in order to check for user ID or screen name
-        if (isinstance(user, int)) or (user.isdigit()):
-            params = {"user_id": user}
-        else:
-            params = {"screen_name": user}
-
-        follower_ids = list()
-        for page in tweepy.Cursor(self.api.get_follower_ids, **params).pages():
-            follower_ids.extend(page)
-        return set(follower_ids)
-
-    def get_user_followee_ids(self, user: str | int) -> Set[int]:
-        """Request Twitter followee IDs from user
-
-        Args:
-            user (str): Either User ID or screen name.
-
-        Returns:
-            Set[int]: Array containing follow IDs
-        """
-        # check if string for user1 is convertible to int in order to check for user ID or screen name
-        if (isinstance(user, int)) or (user.isdigit()):
-            params = {"user_id": user}
-        else:
-            params = {"screen_name": user}
-
-        followee_ids = list()
-        for page in tweepy.Cursor(self.api.get_friend_ids, **params).pages():
-            followee_ids.extend(page)
-        return set(followee_ids)
-
-    def get_latest_activity(self, user: str | int) -> dict:
-        """Returns latest user's activity by fetching the top element from its timeline.
-
-        Args:
-            user (str | int): User ID or screen name.
-
-        Returns:
-            dict: Latest activity.
-        """
-        # if screen name was provided
-        if (isinstance(user, str)) and (user.isdigit() is False):
-            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={user}&include_rts=true&trim_user=true&tweet_mode=extended"
-        # else go with user ID
-        else:
-            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?user_id={user}&include_rts=true&trim_user=true&tweet_mode=extended"
-        response_json = self._manual_request(url)
-        # return the first item since timeline is sorted descending
-        return response_json[0]
-
-    def get_latest_activity_date(self, user: str | int) -> str:
-        """Get latest activity date from specified user by fetching the top element from its timeline.
-
-        Args:
-            user (str | int): User ID or screen name.
-
-        Returns:
-            str: Activity date of latest activity.
-        """
-        # if screen name was provided
-        if (isinstance(user, str)) and (user.isdigit() is False):
-            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={user}&include_rts=true&trim_user=true"
-        # else go with user ID
-        else:
-            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?user_id={user}&include_rts=true&trim_user=true"
-        response_json = self._manual_request(url)
-        # return the first item since timeline is sorted descending
-        return response_json[0]["created_at"]
-
-    def get_relationship(self, source_user: str | int, target_user: str | int) -> dict:
-        """Get relationship between two users.
-
-        Args:
-            user1 (str | int): Source user ID or screen name.
-            user2 (str | int): Target user ID or screen name.
-
-        Returns:
-            dict: Unpacked tuple of JSON from tweepy Friendship model.
-
-        Reference: https://developer.twitter.com/en/docs/twitter-api/v1/accounts-and-users/follow-search-get-users/api-reference/get-friendships-show#example-response
-        """
-
-        params = {"source_id": None, "source_screen_name": None, "target_id": None, "target_screen_name": None}
-        # if source_user is int or a digit
-        if (isinstance(source_user, int)) or (isinstance(source_user, str) and (source_user.isdigit())):
-            params["source_id"] = source_user
-        # else if screen name was provided
-        elif (isinstance(source_user, str)) and (not source_user.isdigit()):
-            params["source_screen_name"] = source_user
-        else:
-            log.error("No ID or username provided for {}".format(source_user))
-
-        # if target_user is int or a digit
-        if (isinstance(target_user, int)) or (isinstance(target_user, str) and (target_user.isdigit())):
-            params["target_id"] = target_user
-        # else if screen name was provided
-        elif (isinstance(target_user, str)) and (not target_user.isdigit()):
-            params["target_screen_name"] = target_user
-        else:
-            log.error("No ID or username provided for {}".format(target_user))
-
-        relationship = self.api.get_friendship(**params)
-        return {"source": relationship[0]._json, "target": relationship[1]._json}
-
-    def get_relationship_pairs(self, users: List[str | int]) -> dict:
-        """Creates pairs for each unique combination of provided users based on their relationship.
-
-        Args:
-            users (List[str  |  int]): List of user IDs or screen names.
-
-        Returns:
-            dict: Pairs of users containing their relationship to each other.
-        """
-        # init emtpy relationships dict
-        relationships = dict()
-        # iterate over every pair combination of provided users
-        for user in users:
-            for other_user in users:
-                if user != other_user:
-                    relationships[(user, other_user)] = self.get_relationship(source_user=user, target_user=other_user)
-        return relationships
-
-    def get_liked_tweets_ids(self, user: str | int, limit: int | None = None) -> list():
-        """Get (all) liked Tweets of provided user.
-
-        Args:
-            user (str | int): User ID or screen name.
-            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
-
-        Returns:
-            Set[int]: Tweet Objects of liked Tweets.
-        """
-        # if user ID was provided
-        if (isinstance(user, int)) or (user.isdigit()):
-            params = {"id": user, "max_results": 100, "pagination_token": None}
-        else:
-            user_obj = self.get_user_object(user)
-            params = {"id": user_obj.id, "max_results": 100, "pagination_token": None}
-
-        page_results = self._paginate(self.client.get_liked_tweets, params, limit=limit, page_attribute="id")
-        return page_results
-
-    def get_composed_tweets_ids(self, user: str | int, limit: int | None = None) -> list:
-        """Get (all) composed Tweets of provided user by pagination.
-
-        Args:
-            user (str | int): User ID or screen name.
-            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
-
-        Returns:
-            list: Tweet Objects of composed Tweets.
-        """
-
-        # user ID is required, if screen name was provided
-        if (isinstance(user, str)) and (not user.isdigit()):
-            user = self.get_user_object(user).id
-        # set params
-        params = {"id": user, "max_results": 100, "pagination_token": None}
-        # get page results
-        page_results = self._paginate(self.client.get_users_tweets, params, limit=limit, page_attribute="id")
-        return page_results
-
-    def get_botometer_scores(self, user: str | int) -> dict:
-        """Returns bot scores from the Botometer API for the specified Twitter user.
-
-        Args:
-            user (str | int): User ID or screen name.
-
-        Returns:
-            dict: The raw Botometer scores for the specified user.
-
-        Reference: https://rapidapi.com/OSoMe/api/botometer-pro/details
-        """
-        if (self._x_rapidapi_key is None) or (self._x_rapidapi_host is None):
-            raise ValueError("'X_RAPIDAPI_KEY' and 'X_RAPIDAPI_HOST' secrets for Botometer API need to be provided.")
-        # get user object
-        user_obj = self.get_user_object(user)
-        # get user timeline
-        timeline = list(map(lambda x: x._json, self.api.user_timeline(user_id=user_obj.id, count=200)))
-        # get user data
-        if timeline:
-            user_data = timeline[0]["user"]
-        else:
-            user_data = user_obj._json
-        screen_name = "@" + user_data["screen_name"]
-        # get latest 100 Tweets
-        tweets = list(map(lambda x: x._json, self.api.search_tweets(screen_name, count=100)))
-        # set payload
-        payload = {"mentions": tweets, "timeline": timeline, "user": user_data}
-        # set header
-        headers = {"content-type": "application/json", "X-RapidAPI-Key": self._x_rapidapi_key, "X-RapidAPI-Host": self._x_rapidapi_host}
-        # set url
-        url = "https://botometer-pro.p.rapidapi.com/4/check_account"
-        # get results
-        response = self._manual_request(url, "POST", headers, payload)
-        return response
-
-    """ Tweet Object data methods """
-
-    def get_tweet_object(self, tweet: str | int) -> tweepy.models.Status:
-        """Request Twitter Tweet Object via tweepy
-
-        Args:
-            tweet (int | str): Tweet ID
-
-        Returns:
-            tweepy.models.Status: tweepy Status Model
-
-        Reference: https://developer.twitter.com/en/docs/twitter-api/v1/data-dictionary/object-model/tweet
-        """
-        try:
-            tweet_obj = self.api.get_status(tweet, include_entities=True, tweet_mode="extended")
-        except tweepy.errors.NotFound as e:
-            log.error("404 Not Found: Resource not found.")
-            raise e
-        except tweepy.errors.Forbidden as e:
-            log.error("403 Forbidden: access refused or access is not allowed.")
-            raise e
-        return tweet_obj
-
-    def get_liking_users_ids(self, tweet_id: str | int, limit: int | None = None) -> list:
-        """Get (all) liking users of provided Tweet by pagination.
-
-        Args:
-            tweet (str | int): Tweet ID.
-            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
-
-        Returns:
-            list: User Objects as list.
-        """
-        # set params
-        params = {"id": tweet_id, "max_results": 100, "pagination_token": None}
-        # get page results
-        page_results = self._paginate(self.client.get_liking_users, params, limit=limit, page_attribute="id")
-        return page_results
-
-    def get_retweeters_ids(self, tweet_id: str | int, limit: int | None = None) -> list:
-        """Get (all) retweeting users of provided Tweet by pagination.
-
-        Args:
-            tweet (str | int): Tweet ID.
-            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
-
-        Returns:
-            list: User Objects of retweeting users.
-        """
-        params = {"id": tweet_id, "max_results": 100, "pagination_token": None}
-        # get page results
-        page_results = self._paginate(self.client.get_retweeters, params, limit=limit, page_attribute="id")
-        return page_results
-
-    def get_quoting_users_ids(self, tweet_id: str | int, limit: int | None = None) -> list:
-        """Get (all) quoting users of provided Tweet by pagination.
-
-        Args:
-            tweet_id (str | int): Tweet ID.
-            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
-
-        Returns:
-            list: User Objects of quoting users.
-        """
-        params = {"id": tweet_id, "max_results": 100, "pagination_token": None}
-        # get page results
-        page_results = self._paginate(self.client.get_quote_tweets, params, limit=limit, response_attribute="includes", page_attribute="id")
-        return page_results
-
-    def get_context_annotations_and_entities(self, tweet_id: str | int) -> dict | None:
-        """Get context annotations and entities from a Tweet.
-
-        Args:
-            tweet_id (str | int): Tweet ID
-
-        Returns:
-            dict | None: context annotations and entities if available, else None.
-
-        Reference: https://developer.twitter.com/en/docs/twitter-api/annotations/overview
-        """
-        url = f"https://api.twitter.com/2/tweets/{tweet_id}"
-        response_json = self._manual_request(url, additional_fields={"tweet.fields": ["context_annotations", "entities"]})
-        # if key is not awailable, return None
-        if "context_annotations" or "entities" in response_json["data"]:
-            return response_json["data"]
-        else:
-            return None
-
-    def get_public_metrics(self, tweet_id: str | int) -> dict:
-        """Get public metrics from Tweet Object
-
-        Args:
-            tweet_id (str | int): Tweet ID
-
-        Returns:
-            dict: Available public metrics for specified Tweet.
-
-        Metrics:
-            - impressions_count (=views)
-            - quote_count
-            - reply_count
-            - retweet_count
-            - favorite_count (=likes)
-
-        Reference: https://developer.twitter.com/en/docs/twitter-api/metrics
-        """
-        # set URL
-        url = f"https://api.twitter.com/2/tweets/{tweet_id}"
-        # make request
-        response_json = self._manual_request(url, additional_fields={"tweet.fields": ["public_metrics"]})
-        # get public metrics from JSON response
-        public_metrics = response_json["data"]["public_metrics"]
-        return public_metrics
+# -*- coding: utf-8 -*-
+import logging
+import sys
+from typing import Any, Dict, List, Set
+
+import requests
+import tweepy
+
+# create logger instance
+log = logging.getLogger(__name__)
+# log to stdout
+handler = logging.StreamHandler(sys.stdout)
+handler.setLevel(logging.ERROR)
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+handler.setFormatter(formatter)
+log.addHandler(handler)
+
+
+class TwitterDataFetcher:
+    """Composition class in order to fetch data from the Twitter Search API v1 and v2."""
+
+    def __init__(
+        self,
+        bearer_token: Any | None = None,
+        consumer_key: Any | None = None,
+        consumer_secret: Any | None = None,
+        access_token: Any | None = None,
+        access_token_secret: Any | None = None,
+        x_rapidapi_key: Any | None = None,
+        x_rapidapi_host: Any | None = None,
+        wait_on_rate_limit: bool = True,
+    ):
+        self._bearer_token = bearer_token
+        self._consumer_key = consumer_key
+        self._consumer_secret = consumer_secret
+        self._access_token = access_token
+        self._access_token_secret = access_token_secret
+        self._x_rapidapi_key = x_rapidapi_key
+        self._x_rapidapi_host = x_rapidapi_host
+        self._wait_on_rate_limit = wait_on_rate_limit
+
+        self.api = tweepy.API(tweepy.AppAuthHandler(consumer_key=self._consumer_key, consumer_secret=self._consumer_secret), wait_on_rate_limit=self._wait_on_rate_limit)
+
+        self.client = tweepy.Client(
+            bearer_token=self._bearer_token, consumer_key=self._consumer_key, consumer_secret=self._consumer_secret, access_token=self._access_token, access_token_secret=self._access_token_secret, wait_on_rate_limit=self._wait_on_rate_limit
+        )
+
+    def _manual_request(self, url: str, method: str = "GET", header: dict | None = None, payload: dict | None = None, additional_fields: Dict[str, List[str]] | None = None) -> dict:
+        """Perform a manual request to the Twitter API.
+
+        Args:
+            url (str): API URL (without specified fields)
+            method (str): Request method according to REST. Defaults to "GET".
+            header (dict | None): Custom HTTP Header. Defaults to None.
+            payload (dict | None): JSON data for HTTP requests. Defaults to None.
+            additional_fields (Dict[str, List[str]] | None, optional): Fields can be specified (e.g., tweet.fields) according to the official API reference. Defaults to None.
+
+        Raises:
+            Exception: If status code != 200.
+
+        Returns:
+            dict: JSON formatted response of API request.
+        """
+        # if additional_fields were provided
+        if additional_fields:
+            # init empty string
+            fields = "?"
+            # create fields string dynamically for every field in additional_fields
+            for field in additional_fields.keys():
+                # e.g., in format "tweet.fields=lang,author_id"
+                fields += f"{field}={','.join(additional_fields[field])}&"
+            # append fields to url
+            url += fields[:-1]
+        if header is None:
+            # set header
+            header = {"Authorization": f"Bearer {self._bearer_token}"}
+        response = requests.request(method=method, url=url, headers=header, json=payload)
+        if response.status_code != 200:
+            raise Exception("Request returned an error: {} {}".format(response.status_code, response.text))
+        return response.json()
+
+    def _paginate(self, func, params: Dict[str, str | int], limit: int | None = None, response_attribute: str = "data", page_attribute: str | None = None) -> list:
+        """Pagination function
+
+        Args:
+            func: Function used for pagination
+            params (Dict[str, str  |  int]): Dict containing request parameters. Should be of the form {'id': ..., 'max_results': ..., 'pagination_token': ...}
+            limit (int | None, optional): Maximum number of results. Defaults to None, thus, no limit.
+            response_attribute (str, optional): Attribute of the Response object. Defaults to "data". Options: ["data", "includes"]
+            page_attribute (str, optional): The attribute that should be extracted for every entry of a page. Defaults to None.
+
+        Raises:
+            KeyError: 'id', 'max_results', and 'pagination_token' should be provided in the params dict.
+
+        Returns:
+            set: Results
+        """
+        # init counter
+        counter = 0
+        # init empty results set
+        results = list()
+        # set break out var
+        break_out = False
+        while not break_out:
+            # make request
+            response = func(**params)
+            # if any data exists
+            if response.__getattribute__(response_attribute) is not None:
+                # iterate over response results
+                for item in response.__getattribute__(response_attribute):
+                    # add result
+                    if page_attribute is None:
+                        results.append(item)
+                    else:
+                        results.append(item.__getattribute__(page_attribute))
+                    # increment counter
+                    counter += 1
+                    # if limit was reached, break
+                    if (limit is not None) and (counter == limit):
+                        # set break_out var to true
+                        break_out = True
+                        break
+                # if last page was reached
+                if "next_token" not in response.meta:
+                    break
+                # else, set new pagination token for next iteration
+                else:
+                    params["pagination_token"] = response.meta["next_token"]
+            # if no data exists, break
+            else:
+                break
+        return results
+
+    """ User Object data methods """
+
+    def get_user_object(self, user: str | int) -> tweepy.models.User:
+        """Request Twitter User Object via tweepy
+
+        Args:
+            user (str): Either User ID or screen name
+
+        Returns:
+            tweepy.User: Twitter User object from tweepy
+        """
+        try:
+            # check if string for user1 is convertible to int in order to check for user ID or screen name
+            if (isinstance(user, int)) or (user.isdigit()):
+                # get profile for user by user ID
+                user_obj = self.api.get_user(user_id=user)
+            else:
+                # get profile for user by screen name
+                user_obj = self.api.get_user(screen_name=user)
+        except tweepy.errors.Forbidden as e:
+            # log to stdout
+            log.error("403 Forbidden: access refused or access is not allowed.")
+            # if user ID was provided
+            if user.isdigit() or isinstance(user, int):
+                url = f"https://api.twitter.com/2/users/{user}"
+            else:
+                # if screen name was provided
+                url = f"https://api.twitter.com/2/users/by/username/{user}"
+            response = self._manual_request(url)
+            # if an error occured that says the user has been suspended
+            if any("User has been suspended" in error["detail"] for error in response["errors"]):
+                log.error("User has been suspended from Twitter. Requested user: {}".format(user))
+                raise e
+            else:
+                raise e
+        return user_obj
+
+    def get_user_follower_ids(self, user: str | int) -> Set[int]:
+        """Request Twitter follower IDs from user
+
+        Args:
+            user (str | int): Either User ID or screen name.
+
+        Returns:
+            Set[int]: Array containing follower IDs
+        """
+        # check if string for user1 is convertible to int in order to check for user ID or screen name
+        if (isinstance(user, int)) or (user.isdigit()):
+            params = {"user_id": user}
+        else:
+            params = {"screen_name": user}
+
+        follower_ids = list()
+        for page in tweepy.Cursor(self.api.get_follower_ids, **params).pages():
+            follower_ids.extend(page)
+        return set(follower_ids)
+
+    def get_user_followee_ids(self, user: str | int) -> Set[int]:
+        """Request Twitter followee IDs from user
+
+        Args:
+            user (str): Either User ID or screen name.
+
+        Returns:
+            Set[int]: Array containing follow IDs
+        """
+        # check if string for user1 is convertible to int in order to check for user ID or screen name
+        if (isinstance(user, int)) or (user.isdigit()):
+            params = {"user_id": user}
+        else:
+            params = {"screen_name": user}
+
+        followee_ids = list()
+        for page in tweepy.Cursor(self.api.get_friend_ids, **params).pages():
+            followee_ids.extend(page)
+        return set(followee_ids)
+
+    def get_latest_activity(self, user: str | int) -> dict:
+        """Returns latest user's activity by fetching the top element from its timeline.
+
+        Args:
+            user (str | int): User ID or screen name.
+
+        Returns:
+            dict: Latest activity.
+        """
+        # if screen name was provided
+        if (isinstance(user, str)) and (user.isdigit() is False):
+            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={user}&include_rts=true&trim_user=true&tweet_mode=extended"
+        # else go with user ID
+        else:
+            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?user_id={user}&include_rts=true&trim_user=true&tweet_mode=extended"
+        response_json = self._manual_request(url)
+        # return the first item since timeline is sorted descending
+        return response_json[0]
+
+    def get_latest_activity_date(self, user: str | int) -> str:
+        """Get latest activity date from specified user by fetching the top element from its timeline.
+
+        Args:
+            user (str | int): User ID or screen name.
+
+        Returns:
+            str: Activity date of latest activity.
+        """
+        # if screen name was provided
+        if (isinstance(user, str)) and (user.isdigit() is False):
+            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={user}&include_rts=true&trim_user=true"
+        # else go with user ID
+        else:
+            url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?user_id={user}&include_rts=true&trim_user=true"
+        response_json = self._manual_request(url)
+        # return the first item since timeline is sorted descending
+        return response_json[0]["created_at"]
+
+    def get_relationship(self, source_user: str | int, target_user: str | int) -> dict:
+        """Get relationship between two users.
+
+        Args:
+            user1 (str | int): Source user ID or screen name.
+            user2 (str | int): Target user ID or screen name.
+
+        Returns:
+            dict: Unpacked tuple of JSON from tweepy Friendship model.
+
+        Reference: https://developer.twitter.com/en/docs/twitter-api/v1/accounts-and-users/follow-search-get-users/api-reference/get-friendships-show#example-response
+        """
+
+        params = {"source_id": None, "source_screen_name": None, "target_id": None, "target_screen_name": None}
+        # if source_user is int or a digit
+        if (isinstance(source_user, int)) or (isinstance(source_user, str) and (source_user.isdigit())):
+            params["source_id"] = source_user
+        # else if screen name was provided
+        elif (isinstance(source_user, str)) and (not source_user.isdigit()):
+            params["source_screen_name"] = source_user
+        else:
+            log.error("No ID or username provided for {}".format(source_user))
+
+        # if target_user is int or a digit
+        if (isinstance(target_user, int)) or (isinstance(target_user, str) and (target_user.isdigit())):
+            params["target_id"] = target_user
+        # else if screen name was provided
+        elif (isinstance(target_user, str)) and (not target_user.isdigit()):
+            params["target_screen_name"] = target_user
+        else:
+            log.error("No ID or username provided for {}".format(target_user))
+
+        relationship = self.api.get_friendship(**params)
+        return {"source": relationship[0]._json, "target": relationship[1]._json}
+
+    def get_relationship_pairs(self, users: List[str | int]) -> dict:
+        """Creates pairs for each unique combination of provided users based on their relationship.
+
+        Args:
+            users (List[str  |  int]): List of user IDs or screen names.
+
+        Returns:
+            dict: Pairs of users containing their relationship to each other.
+        """
+        # init emtpy relationships dict
+        relationships = dict()
+        # iterate over every pair combination of provided users
+        for user in users:
+            for other_user in users:
+                if user != other_user:
+                    relationships[(user, other_user)] = self.get_relationship(source_user=user, target_user=other_user)
+        return relationships
+
+    def get_liked_tweets_ids(self, user: str | int, limit: int | None = None) -> list():
+        """Get (all) liked Tweets of provided user.
+
+        Args:
+            user (str | int): User ID or screen name.
+            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
+
+        Returns:
+            Set[int]: Tweet Objects of liked Tweets.
+        """
+        # if user ID was provided
+        if (isinstance(user, int)) or (user.isdigit()):
+            params = {"id": user, "max_results": 100, "pagination_token": None}
+        else:
+            user_obj = self.get_user_object(user)
+            params = {"id": user_obj.id, "max_results": 100, "pagination_token": None}
+
+        page_results = self._paginate(self.client.get_liked_tweets, params, limit=limit, page_attribute="id")
+        return page_results
+
+    def get_composed_tweets_ids(self, user: str | int, limit: int | None = None) -> list:
+        """Get (all) composed Tweets of provided user by pagination.
+
+        Args:
+            user (str | int): User ID or screen name.
+            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
+
+        Returns:
+            list: Tweet Objects of composed Tweets.
+        """
+
+        # user ID is required, if screen name was provided
+        if (isinstance(user, str)) and (not user.isdigit()):
+            user = self.get_user_object(user).id
+        # set params
+        params = {"id": user, "max_results": 100, "pagination_token": None}
+        # get page results
+        page_results = self._paginate(self.client.get_users_tweets, params, limit=limit, page_attribute="id")
+        return page_results
+
+    def get_botometer_scores(self, user: str | int) -> dict:
+        """Returns bot scores from the Botometer API for the specified Twitter user.
+
+        Args:
+            user (str | int): User ID or screen name.
+
+        Returns:
+            dict: The raw Botometer scores for the specified user.
+
+        Reference: https://rapidapi.com/OSoMe/api/botometer-pro/details
+        """
+        if (self._x_rapidapi_key is None) or (self._x_rapidapi_host is None):
+            raise ValueError("'X_RAPIDAPI_KEY' and 'X_RAPIDAPI_HOST' secrets for Botometer API need to be provided.")
+        # get user object
+        user_obj = self.get_user_object(user)
+        # get user timeline
+        timeline = list(map(lambda x: x._json, self.api.user_timeline(user_id=user_obj.id, count=200)))
+        # get user data
+        if timeline:
+            user_data = timeline[0]["user"]
+        else:
+            user_data = user_obj._json
+        screen_name = "@" + user_data["screen_name"]
+        # get latest 100 Tweets
+        tweets = list(map(lambda x: x._json, self.api.search_tweets(screen_name, count=100)))
+        # set payload
+        payload = {"mentions": tweets, "timeline": timeline, "user": user_data}
+        # set header
+        headers = {"content-type": "application/json", "X-RapidAPI-Key": self._x_rapidapi_key, "X-RapidAPI-Host": self._x_rapidapi_host}
+        # set url
+        url = "https://botometer-pro.p.rapidapi.com/4/check_account"
+        # get results
+        response = self._manual_request(url, "POST", headers, payload)
+        return response
+
+    """ Tweet Object data methods """
+
+    def get_tweet_object(self, tweet: str | int) -> tweepy.models.Status:
+        """Request Twitter Tweet Object via tweepy
+
+        Args:
+            tweet (int | str): Tweet ID
+
+        Returns:
+            tweepy.models.Status: tweepy Status Model
+
+        Reference: https://developer.twitter.com/en/docs/twitter-api/v1/data-dictionary/object-model/tweet
+        """
+        try:
+            tweet_obj = self.api.get_status(tweet, include_entities=True, tweet_mode="extended")
+        except tweepy.errors.NotFound as e:
+            log.error("404 Not Found: Resource not found.")
+            raise e
+        except tweepy.errors.Forbidden as e:
+            log.error("403 Forbidden: access refused or access is not allowed.")
+            raise e
+        return tweet_obj
+
+    def get_liking_users_ids(self, tweet_id: str | int, limit: int | None = None) -> list:
+        """Get (all) liking users of provided Tweet by pagination.
+
+        Args:
+            tweet (str | int): Tweet ID.
+            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
+
+        Returns:
+            list: User Objects as list.
+        """
+        # set params
+        params = {"id": tweet_id, "max_results": 100, "pagination_token": None}
+        # get page results
+        page_results = self._paginate(self.client.get_liking_users, params, limit=limit, page_attribute="id")
+        return page_results
+
+    def get_retweeters_ids(self, tweet_id: str | int, limit: int | None = None) -> list:
+        """Get (all) retweeting users of provided Tweet by pagination.
+
+        Args:
+            tweet (str | int): Tweet ID.
+            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
+
+        Returns:
+            list: User Objects of retweeting users.
+        """
+        params = {"id": tweet_id, "max_results": 100, "pagination_token": None}
+        # get page results
+        page_results = self._paginate(self.client.get_retweeters, params, limit=limit, page_attribute="id")
+        return page_results
+
+    def get_quoting_users_ids(self, tweet_id: str | int, limit: int | None = None) -> list:
+        """Get (all) quoting users of provided Tweet by pagination.
+
+        Args:
+            tweet_id (str | int): Tweet ID.
+            limit (int | None): The maximum number of results to be returned. By default, each page will return the maximum number of results available.
+
+        Returns:
+            list: User Objects of quoting users.
+        """
+        params = {"id": tweet_id, "max_results": 100, "pagination_token": None}
+        # get page results
+        page_results = self._paginate(self.client.get_quote_tweets, params, limit=limit, response_attribute="includes", page_attribute="id")
+        return page_results
+
+    def get_context_annotations_and_entities(self, tweet_id: str | int) -> dict | None:
+        """Get context annotations and entities from a Tweet.
+
+        Args:
+            tweet_id (str | int): Tweet ID
+
+        Returns:
+            dict | None: context annotations and entities if available, else None.
+
+        Reference: https://developer.twitter.com/en/docs/twitter-api/annotations/overview
+        """
+        url = f"https://api.twitter.com/2/tweets/{tweet_id}"
+        response_json = self._manual_request(url, additional_fields={"tweet.fields": ["context_annotations", "entities"]})
+        # if key is not awailable, return None
+        if "context_annotations" or "entities" in response_json["data"]:
+            return response_json["data"]
+        else:
+            return None
+
+    def get_public_metrics(self, tweet_id: str | int) -> dict:
+        """Get public metrics from Tweet Object
+
+        Args:
+            tweet_id (str | int): Tweet ID
+
+        Returns:
+            dict: Available public metrics for specified Tweet.
+
+        Metrics:
+            - impressions_count (=views)
+            - quote_count
+            - reply_count
+            - retweet_count
+            - favorite_count (=likes)
+
+        Reference: https://developer.twitter.com/en/docs/twitter-api/metrics
+        """
+        # set URL
+        url = f"https://api.twitter.com/2/tweets/{tweet_id}"
+        # make request
+        response_json = self._manual_request(url, additional_fields={"tweet.fields": ["public_metrics"]})
+        # get public metrics from JSON response
+        public_metrics = response_json["data"]["public_metrics"]
+        return public_metrics
```

### Comparing `pysna-0.1.1/pysna/process.py` & `pysna-0.1.2/pysna/process.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-# -*- coding: utf-8 -*-
-import operator
-import re
-from datetime import datetime, timezone
-from numbers import Number
-from typing import Dict, List
-
-import numpy as np
-import tweepy
-from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
-
-
-class BaseDataProcessor:
-    """Base component class in order to process social data."""
-
-    def calc_descriptive_metrics(self, data: Dict[str | int, Number]) -> dict:
-        """Calculates descriptive metrics of a given data set.
-
-        Args:
-            data (Dict[str  |  int, Number]): Data dictionary containing numeric values.
-
-        Raises:
-            ValueError: If non-numeric values are contained in the data dictionary.
-
-        Returns:
-            dict: Input data dictionary containing descriptive metrics.
-
-        Metrics:
-            - Max Value
-            - Min Value
-            - Mean Value
-            - Median
-            - Standard Deviation
-            - Sample Variance
-            - Range (Max - Min)
-            - Interquartiles Range
-            - Mean Absolute Deviation
-        """
-        if not any(isinstance(value, Number) for value in data.values()):
-            raise ValueError("Only numeric values are allowed.")
-        # extract numeric values by iterating over data dict with iterable items
-        numerics = list(data.values())
-        # init empty dict to store descriptive metrics
-        metrics = dict()
-        # calc max
-        metrics["max"] = max(numerics)
-        # calc min
-        metrics["min"] = min(numerics)
-        # calc mean
-        metrics["mean"] = np.array(numerics).mean()
-        # calc median
-        metrics["median"] = np.median(numerics)
-        # calc standard deviation
-        metrics["std"] = np.std(numerics)
-        # calc variance
-        metrics["var"] = np.var(numerics)
-        # calc range
-        metrics["range"] = max(numerics) - min(numerics)
-        # calc interquarile range
-        metrics["IQR"] = np.subtract(*np.percentile(numerics, [75, 25]))
-        # calc absolute mean deviation
-        metrics["mad"] = np.mean(np.absolute(numerics - np.mean(numerics)))
-        # add metrics
-        data["metrics"] = metrics
-        return data
-
-    def calc_datetime_metrics(self, dates: Dict[str, datetime]) -> dict():
-        """Calculates descriptive metrics on datetime objects.
-
-        Args:
-            dates (Dict[str, datetime]): Dictionary containing identifiers as keys and datetime objects as values.
-
-        Returns:
-            dict: Input dates with added datetime metrics.
-
-        Metrics:
-            - Mean
-            - Median
-            - Max
-            - Min
-            - Time Span (in days, seconds, and microseconds)
-            - Deviation from mean (in days and seconds). Negative values indicate below average, positive ones above average.
-            - Deviation from median (in days and seconds). Negative values indicate below median, positive ones above average.
-        """
-        # use the datetime's timestamp to make them comparable
-        timestamps = [dt.timestamp() for dt in dates.values()]
-        # calc mean of creation dates
-        total_time = sum(timestamps)
-        mean_timestamp = total_time / len(timestamps)
-        # convert mean timestamp back to datetime object with timezone information
-        mean_datetime = datetime.fromtimestamp(mean_timestamp, tz=timezone.utc)
-
-        # calculate time differences to mean datetime of every creation date
-        time_diffs_mean = {key: {"days": (dt - mean_datetime).days, "seconds": (dt - mean_datetime).seconds} for key, dt in dates.items()}
-
-        # find the median of the timestamps
-        median_timestamp = np.median(timestamps)
-        # Convert median timestamp back to datetime object
-        median_datetime = datetime.fromtimestamp(median_timestamp, tz=timezone.utc)
-
-        # calculate time differences to median timestamp of every creation date
-        time_diffs_median = {key: {"days": (dt - median_datetime).days, "seconds": (dt - median_datetime).seconds} for key, dt in dates.items()}
-
-        # calc range of creation dates
-        max_date, min_date = max(dates.values()), min(dates.values())
-        time_span = max_date - min_date
-
-        # convert creation dates to isoformat for readability
-        dates = {key: dt.isoformat() for key, dt in dates.items()}
-
-        # add metrics to output
-        dates["metrics"] = dict()
-        dates["metrics"]["deviation_from_mean"] = time_diffs_mean
-        dates["metrics"]["deviation_from_median"] = time_diffs_median
-        dates["metrics"]["time_span"] = {"days": time_span.days, "seconds": time_span.seconds, "microseconds": time_span.microseconds}
-        dates["metrics"]["mean"] = mean_datetime.isoformat()
-        dates["metrics"]["median"] = median_datetime.isoformat()
-        dates["metrics"]["max"] = max_date.isoformat()
-        dates["metrics"]["min"] = min_date.isoformat()
-        return dates
-
-    def intersection(self, iterable: List[set]) -> list:
-        """Calculates the intersection of multiple sets.
-
-        Args:
-            iterable (List[set]): List containing sets.
-
-        Returns:
-            list: intersection set casted to list.
-        """
-        intersection = set.intersection(*map(set, iterable))
-        return list(intersection)
-
-    def difference(self, sets: Dict[int | str, set]) -> dict:
-        """Calculates the difference of multiple sets.
-
-        Args:
-            sets (Dict[set]): Dictionary containing sets where keys are identifiers.
-
-        Returns:
-            dict: Individual difference of each set that was provided.
-        """
-        # init empty dict to store individual differences for each set
-        differences = dict()
-        for key, values in sets.items():
-            differences[key] = list(set(values))
-            for other_key, other_values in sets.items():
-                if key != other_key:
-                    differences[key] = list(set(differences[key]) - set(other_values))
-        return differences
-
-
-class TwitterDataProcessor(BaseDataProcessor):
-    """Component class in order to process Twitter data."""
-
-    def extract_followers(self, user_object: tweepy.User) -> Dict[str, str | int]:
-        """Extract IDs, names, and screen names from a user's followers.
-
-        Args:
-            user_object (tweepy.User): Tweepy User Object.
-
-        Returns:
-            Dict[str, str | int]: Dictionary containing IDs, names, and screen names.
-        """
-        info = {"followers_ids": list(), "followers_names": list(), "followers_screen_names": list()}
-        # extract follower IDs
-        info["followers_ids"] = user_object.follower_ids()
-        # extract names and screen names
-        for follower in user_object.followers():
-            info["followers_names"].append(follower.name)
-            info["followers_screen_names"].append(follower.screen_name)
-        return info
-
-    def extract_followees(self, user_object: tweepy.User) -> Dict[str, str | int]:
-        """Extract IDs, names, and screen names from a user's followees.
-
-        Args:
-            user_object (tweepy.User): Tweepy User Object.
-
-        Returns:
-            Dict[str, str | int]: Dictionary containing IDs, names, and screen names.
-        """
-        info = {"followees_ids": list(), "followees_names": list(), "followees_screen_names": list()}
-        # extract IDs, names and screen names
-        for followee in user_object.friends():
-            info["followees_ids"].append(followee.id)
-            info["followees_names"].append(followee.name)
-            info["followees_screen_names"].append(followee.screen_name)
-        return info
-
-    def clean_tweet(self, tweet: str) -> str:
-        """Utility function to clean tweet text by removing links, special characters using simple regex statements.
-
-        Args:
-            tweet (str): Raw text of the Tweet.
-
-        Returns:
-            str: Cleaned Tweet
-        """
-        return " ".join(re.sub(r"(@[A-Za-z0-9]+)|([^0-9A-Za-z \t])|(\w+:\/\/\S+)", " ", tweet).split())
-
-    def detect_tweet_sentiment(self, tweet: str) -> dict:
-        """Utility function to classify sentiment of passed tweet using vader sentiment analyzer. English Tweets only.
-
-        Args:
-            tweet (str): The raw text of the Tweet.
-
-        Returns:
-            str: the sentiment of the Tweet (either positive, neutral, or negative) and the polarity scores.
-        """
-        # create VADER instance
-        analyser = SentimentIntensityAnalyzer()
-        # get polarity scores from cleaned tweet
-        polarity_scores = analyser.polarity_scores(self.clean_tweet(tweet))
-        # define label
-        if polarity_scores["compound"] >= 0.05:
-            label = "positive"
-        elif polarity_scores["compound"] <= -0.05:
-            label = "negative"
-        else:
-            label = "neutral"
-        # return label and polarity scores
-        return {"label": label, "polarity_scores": polarity_scores}
-
-    def calc_similarity(self, user_objs: List[dict] | None = None, tweet_metrics: List[Dict[int, dict]] | None = None, *, features: List[str]) -> dict:
-        """Calculates the euclidean distance of users/tweets based on a feature vector. Either user objects or Tweet objects must be specified, not both.
-
-        Args:
-            user_objs (List[dict] | None, optional): List of serialized Twitter user objects from Twitter Search API v1. Defaults to None.
-            tweet_metrics (List[Dict[int | dict]] | None, optional): List of public Tweet metrics as dictionaries with Tweet IDs as keys. Defaults to None.
-            features (List[str]): Features that should be contained in the feature vector. Features have to be numeric and must belong to the respective object (i.e., user or tweet.)
-
-        Raises:
-            ValueError: If either 'user_objs' and 'tweet_objs' or none of them were provided.
-            AssertionError: If non-numeric feature was provided in the 'features' list.
-
-        Returns:
-            dict: Unique pair of users/tweets containing the respective euclidean distance. Sorted in ascending order.
-        """
-        # init empty dict to store distances
-        distances = dict()
-        # if users and tweets were provided
-        if user_objs and tweet_metrics:
-            raise ValueError("Either 'user_objs' or 'tweet_metrics' must be specified, not both.")
-        # if only user_objs were provided
-        elif user_objs:
-            # iterate over every uniqe pair
-            for i in range(len(user_objs)):
-                for j in range(i + 1, len(user_objs)):
-                    # get user objects for each pair
-                    user_i = user_objs[i]
-                    user_j = user_objs[j]
-                    # build feature vector
-                    vec_i = np.array([user_i[feature] for feature in features])
-                    vec_j = np.array([user_j[feature] for feature in features])
-                    # feature vectors have to contain numeric values
-                    assert all(isinstance(feat, Number) for feat in vec_i), "only numeric features are allowed"
-                    assert all(isinstance(feat, Number) for feat in vec_j), "only numeric features are allowed"
-                    # calc euclidean distance
-                    distances[(user_i["id"], user_j["id"])] = np.linalg.norm(vec_i - vec_j, ord=2)
-        elif tweet_metrics:
-            # iterate over every uniqe pair
-            for i in range(len(tweet_metrics)):
-                for j in range(i + 1, len(tweet_metrics)):
-                    # get Tweet objects for each pair
-                    tweet_i = list(tweet_metrics.values())[i]
-                    tweet_j = list(tweet_metrics.values())[j]
-                    # build feature vector
-                    vec_i = np.array([tweet_i[feature] for feature in features])
-                    vec_j = np.array([tweet_j[feature] for feature in features])
-                    # feature vectors have to contain numeric values
-                    assert all(isinstance(feat, Number) for feat in vec_i), "only numeric features are allowed"
-                    assert all(isinstance(feat, Number) for feat in vec_j), "only numeric features are allowed"
-                    # calc euclidean distance
-                    distances[(list(tweet_metrics.keys())[i], list(tweet_metrics.keys())[j])] = np.linalg.norm(vec_i - vec_j, ord=2)
-        # if none was provided
-        else:
-            raise ValueError("Either 'user_objs' or 'tweet_metrics' must be provided.")
-        # sort dict in ascendin order
-        sorted_values = dict(sorted(distances.items(), key=operator.itemgetter(1)))
-        return sorted_values
+# -*- coding: utf-8 -*-
+import operator
+import re
+from datetime import datetime, timezone
+from numbers import Number
+from typing import Dict, List
+
+import numpy as np
+import tweepy
+from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
+
+
+class BaseDataProcessor:
+    """Base component class in order to process social data."""
+
+    def calc_descriptive_metrics(self, data: Dict[str | int, Number]) -> dict:
+        """Calculates descriptive metrics of a given data set.
+
+        Args:
+            data (Dict[str  |  int, Number]): Data dictionary containing numeric values.
+
+        Raises:
+            ValueError: If non-numeric values are contained in the data dictionary.
+
+        Returns:
+            dict: Input data dictionary containing descriptive metrics.
+
+        Metrics:
+            - Max Value
+            - Min Value
+            - Mean Value
+            - Median
+            - Standard Deviation
+            - Sample Variance
+            - Range (Max - Min)
+            - Interquartiles Range
+            - Mean Absolute Deviation
+        """
+        if not any(isinstance(value, Number) for value in data.values()):
+            raise ValueError("Only numeric values are allowed.")
+        # extract numeric values by iterating over data dict with iterable items
+        numerics = list(data.values())
+        # init empty dict to store descriptive metrics
+        metrics = dict()
+        # calc max
+        metrics["max"] = max(numerics)
+        # calc min
+        metrics["min"] = min(numerics)
+        # calc mean
+        metrics["mean"] = np.array(numerics).mean()
+        # calc median
+        metrics["median"] = np.median(numerics)
+        # calc standard deviation
+        metrics["std"] = np.std(numerics)
+        # calc variance
+        metrics["var"] = np.var(numerics)
+        # calc range
+        metrics["range"] = max(numerics) - min(numerics)
+        # calc interquarile range
+        metrics["IQR"] = np.subtract(*np.percentile(numerics, [75, 25]))
+        # calc absolute mean deviation
+        metrics["mad"] = np.mean(np.absolute(numerics - np.mean(numerics)))
+        # add metrics
+        data["metrics"] = metrics
+        return data
+
+    def calc_datetime_metrics(self, dates: Dict[str, datetime]) -> dict():
+        """Calculates descriptive metrics on datetime objects.
+
+        Args:
+            dates (Dict[str, datetime]): Dictionary containing identifiers as keys and datetime objects as values.
+
+        Returns:
+            dict: Input dates with added datetime metrics.
+
+        Metrics:
+            - Mean
+            - Median
+            - Max
+            - Min
+            - Time Span (in days, seconds, and microseconds)
+            - Deviation from mean (in days and seconds). Negative values indicate below average, positive ones above average.
+            - Deviation from median (in days and seconds). Negative values indicate below median, positive ones above average.
+        """
+        # use the datetime's timestamp to make them comparable
+        timestamps = [dt.timestamp() for dt in dates.values()]
+        # calc mean of creation dates
+        total_time = sum(timestamps)
+        mean_timestamp = total_time / len(timestamps)
+        # convert mean timestamp back to datetime object with timezone information
+        mean_datetime = datetime.fromtimestamp(mean_timestamp, tz=timezone.utc)
+
+        # calculate time differences to mean datetime of every creation date
+        time_diffs_mean = {key: {"days": (dt - mean_datetime).days, "seconds": (dt - mean_datetime).seconds} for key, dt in dates.items()}
+
+        # find the median of the timestamps
+        median_timestamp = np.median(timestamps)
+        # Convert median timestamp back to datetime object
+        median_datetime = datetime.fromtimestamp(median_timestamp, tz=timezone.utc)
+
+        # calculate time differences to median timestamp of every creation date
+        time_diffs_median = {key: {"days": (dt - median_datetime).days, "seconds": (dt - median_datetime).seconds} for key, dt in dates.items()}
+
+        # calc range of creation dates
+        max_date, min_date = max(dates.values()), min(dates.values())
+        time_span = max_date - min_date
+
+        # convert creation dates to isoformat for readability
+        dates = {key: dt.isoformat() for key, dt in dates.items()}
+
+        # add metrics to output
+        dates["metrics"] = dict()
+        dates["metrics"]["deviation_from_mean"] = time_diffs_mean
+        dates["metrics"]["deviation_from_median"] = time_diffs_median
+        dates["metrics"]["time_span"] = {"days": time_span.days, "seconds": time_span.seconds, "microseconds": time_span.microseconds}
+        dates["metrics"]["mean"] = mean_datetime.isoformat()
+        dates["metrics"]["median"] = median_datetime.isoformat()
+        dates["metrics"]["max"] = max_date.isoformat()
+        dates["metrics"]["min"] = min_date.isoformat()
+        return dates
+
+    def intersection(self, iterable: List[set]) -> list:
+        """Calculates the intersection of multiple sets.
+
+        Args:
+            iterable (List[set]): List containing sets.
+
+        Returns:
+            list: intersection set casted to list.
+        """
+        intersection = set.intersection(*map(set, iterable))
+        return list(intersection)
+
+    def difference(self, sets: Dict[int | str, set]) -> dict:
+        """Calculates the difference of multiple sets.
+
+        Args:
+            sets (Dict[set]): Dictionary containing sets where keys are identifiers.
+
+        Returns:
+            dict: Individual difference of each set that was provided.
+        """
+        # init empty dict to store individual differences for each set
+        differences = dict()
+        for key, values in sets.items():
+            differences[key] = list(set(values))
+            for other_key, other_values in sets.items():
+                if key != other_key:
+                    differences[key] = list(set(differences[key]) - set(other_values))
+        return differences
+
+
+class TwitterDataProcessor(BaseDataProcessor):
+    """Component class in order to process Twitter data."""
+
+    def extract_followers(self, user_object: tweepy.User) -> Dict[str, str | int]:
+        """Extract IDs, names, and screen names from a user's followers.
+
+        Args:
+            user_object (tweepy.User): Tweepy User Object.
+
+        Returns:
+            Dict[str, str | int]: Dictionary containing IDs, names, and screen names.
+        """
+        info = {"followers_ids": list(), "followers_names": list(), "followers_screen_names": list()}
+        # extract follower IDs
+        info["followers_ids"] = user_object.follower_ids()
+        # extract names and screen names
+        for follower in user_object.followers():
+            info["followers_names"].append(follower.name)
+            info["followers_screen_names"].append(follower.screen_name)
+        return info
+
+    def extract_followees(self, user_object: tweepy.User) -> Dict[str, str | int]:
+        """Extract IDs, names, and screen names from a user's followees.
+
+        Args:
+            user_object (tweepy.User): Tweepy User Object.
+
+        Returns:
+            Dict[str, str | int]: Dictionary containing IDs, names, and screen names.
+        """
+        info = {"followees_ids": list(), "followees_names": list(), "followees_screen_names": list()}
+        # extract IDs, names and screen names
+        for followee in user_object.friends():
+            info["followees_ids"].append(followee.id)
+            info["followees_names"].append(followee.name)
+            info["followees_screen_names"].append(followee.screen_name)
+        return info
+
+    def clean_tweet(self, tweet: str) -> str:
+        """Utility function to clean tweet text by removing links, special characters using simple regex statements.
+
+        Args:
+            tweet (str): Raw text of the Tweet.
+
+        Returns:
+            str: Cleaned Tweet
+        """
+        return " ".join(re.sub(r"(@[A-Za-z0-9]+)|([^0-9A-Za-z \t])|(\w+:\/\/\S+)", " ", tweet).split())
+
+    def detect_tweet_sentiment(self, tweet: str) -> dict:
+        """Utility function to classify sentiment of passed tweet using vader sentiment analyzer. English Tweets only.
+
+        Args:
+            tweet (str): The raw text of the Tweet.
+
+        Returns:
+            str: the sentiment of the Tweet (either positive, neutral, or negative) and the polarity scores.
+        """
+        # create VADER instance
+        analyser = SentimentIntensityAnalyzer()
+        # get polarity scores from cleaned tweet
+        polarity_scores = analyser.polarity_scores(self.clean_tweet(tweet))
+        # define label
+        if polarity_scores["compound"] >= 0.05:
+            label = "positive"
+        elif polarity_scores["compound"] <= -0.05:
+            label = "negative"
+        else:
+            label = "neutral"
+        # return label and polarity scores
+        return {"label": label, "polarity_scores": polarity_scores}
+
+    def calc_similarity(self, user_objs: List[dict] | None = None, tweet_metrics: List[Dict[int, dict]] | None = None, *, features: List[str]) -> dict:
+        """Calculates the euclidean distance of users/tweets based on a feature vector. Either user objects or Tweet objects must be specified, not both.
+
+        Args:
+            user_objs (List[dict] | None, optional): List of serialized Twitter user objects from Twitter Search API v1. Defaults to None.
+            tweet_metrics (List[Dict[int | dict]] | None, optional): List of public Tweet metrics as dictionaries with Tweet IDs as keys. Defaults to None.
+            features (List[str]): Features that should be contained in the feature vector. Features have to be numeric and must belong to the respective object (i.e., user or tweet.)
+
+        Raises:
+            ValueError: If either 'user_objs' and 'tweet_objs' or none of them were provided.
+            AssertionError: If non-numeric feature was provided in the 'features' list.
+
+        Returns:
+            dict: Unique pair of users/tweets containing the respective euclidean distance. Sorted in ascending order.
+        """
+        # init empty dict to store distances
+        distances = dict()
+        # if users and tweets were provided
+        if user_objs and tweet_metrics:
+            raise ValueError("Either 'user_objs' or 'tweet_metrics' must be specified, not both.")
+        # if only user_objs were provided
+        elif user_objs:
+            # iterate over every uniqe pair
+            for i in range(len(user_objs)):
+                for j in range(i + 1, len(user_objs)):
+                    # get user objects for each pair
+                    user_i = user_objs[i]
+                    user_j = user_objs[j]
+                    # build feature vector
+                    vec_i = np.array([user_i[feature] for feature in features])
+                    vec_j = np.array([user_j[feature] for feature in features])
+                    # feature vectors have to contain numeric values
+                    assert all(isinstance(feat, Number) for feat in vec_i), "only numeric features are allowed"
+                    assert all(isinstance(feat, Number) for feat in vec_j), "only numeric features are allowed"
+                    # calc euclidean distance
+                    distances[(user_i["id"], user_j["id"])] = np.linalg.norm(vec_i - vec_j, ord=2)
+        elif tweet_metrics:
+            # iterate over every uniqe pair
+            for i in range(len(tweet_metrics)):
+                for j in range(i + 1, len(tweet_metrics)):
+                    # get Tweet objects for each pair
+                    tweet_i = list(tweet_metrics.values())[i]
+                    tweet_j = list(tweet_metrics.values())[j]
+                    # build feature vector
+                    vec_i = np.array([tweet_i[feature] for feature in features])
+                    vec_j = np.array([tweet_j[feature] for feature in features])
+                    # feature vectors have to contain numeric values
+                    assert all(isinstance(feat, Number) for feat in vec_i), "only numeric features are allowed"
+                    assert all(isinstance(feat, Number) for feat in vec_j), "only numeric features are allowed"
+                    # calc euclidean distance
+                    distances[(list(tweet_metrics.keys())[i], list(tweet_metrics.keys())[j])] = np.linalg.norm(vec_i - vec_j, ord=2)
+        # if none was provided
+        else:
+            raise ValueError("Either 'user_objs' or 'tweet_metrics' must be provided.")
+        # sort dict in ascendin order
+        sorted_values = dict(sorted(distances.items(), key=operator.itemgetter(1)))
+        return sorted_values
```

### Comparing `pysna-0.1.1/pysna/utils.py` & `pysna-0.1.2/pysna/utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-# -*- coding: utf-8 -*-
-import copy
-import json
-import warnings
-from datetime import datetime
-from typing import Any, Dict
-
-import pandas as pd
-
-warnings.simplefilter(action="ignore", category=FutureWarning)
-
-
-def export_to_csv(data: dict, export_path: str, encoding: str = "utf-8", sep: str = ",", **kwargs):
-    """Export dictionary data to CSV file.
-
-    Args:
-        data (dict): Data dictionary (nested dictionaries are not allowed)
-        export_path (str): Export path including file name and extension.
-        encoding (str, optional): Encoding of CSV file. Defaults to 'utf-8'.
-        sep (str, optional): Value separator for CSV file. Defaults to ",".
-        kwargs: Keyword arguments for pd.DataFrame.to_csv. See references below for further details.
-
-    Raises:
-        ValueError: If nested dictionary was provided.
-        IOError: If export fails due to bad input.
-
-    References:
-        - https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#export-to-csv
-        - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_csv.html
-    """
-    # catch nested dict
-    if any(isinstance(data[key], dict) for key in data.keys()):
-        raise ValueError("'data' dictionary must not contain nested dictionaries. Use JSON export instead.")
-    try:
-        # convert to pandas dataframe from dict
-        f = pd.DataFrame(data, index=[0])
-        # export data frame
-        f.to_csv(export_path, encoding=encoding, sep=sep, index=False, **kwargs)
-    except IOError as e:
-        raise e
-
-
-def append_to_csv(data: dict, filepath: str, encoding: str = "utf-8", sep: str = ","):
-    """Append a dictionary to an existing CSV file.
-
-    Args:
-        data (dict): Dictionary containing new data that should be added to file.
-        filepath (str): Absolute or relative filepath including the file extension. Depending on the current working directory.
-        encoding (str, optional): Encoding of CSV file.. Defaults to 'utf-8'.
-        sep (str, optional): Value separator for CSV file. Defaults to ",".
-        args: Keyword Arguments for reading and writing from/to CSV file from pandas. Pass in: *[read_kwargs, write_kwargs]. See references below for further details on possible read/write arguments.
-
-    Raises:
-        ValueError: If nested dictionary was provided.
-        ValueError: If 'args' does not contain a dictionaries for read and write.
-        IOError: If export fails due to bad input.
-
-    References:
-        - https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#append-to-csv
-        - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_csv.html
-        - https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html
-    """
-    # catch nested dict
-    if any(isinstance(data[key], dict) for key in data.keys()):
-        raise ValueError("'data' dictionary must not contain nested dictionaries. Use JSON export instead.")
-    try:
-        # read existing file
-        f = pd.read_csv(filepath, sep=sep, encoding=encoding)
-        # convert data dict to df
-        input_df = pd.DataFrame(data, index=[0])
-        # concat dfs
-        f = pd.concat([f, input_df], axis=0)
-        # export to CSV
-        f.to_csv(filepath, sep=sep, encoding=encoding, index=False)
-    except IOError as e:
-        raise e
-
-
-def export_to_json(data: dict, export_path: str, encoding: str = "utf-8", ensure_ascii: bool = False, *args):
-    """Export dictionary data to JSON file. Tuple-keys are encoded to strings.
-
-    Args:
-        data (dict): Data dictionary
-        export_path (str): Export path including file name and extension.
-        encoding (str, optional): Encoding of JSON file. Defaults to "utf-8".
-        ensure_ascii (bool): Wheather to convert characters to ASCII. Defaults to False.
-
-    References: https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#export-to-json
-    """
-
-    try:
-        with open(export_path, "w", encoding=encoding) as jsonfile:
-            # add 'data' key in order to append additional dicts to same file, if not already exist
-            if "data" not in data:
-                serialized_data = {"data": [data]}
-            # dump to json
-            json.dump(serialized_data, jsonfile, indent=4, ensure_ascii=ensure_ascii, *args)
-    except IOError as e:
-        raise e
-    # usually when tuple cannot be serialized
-    except TypeError or json.JSONDecodeError:
-        # serialize tuples
-        data = _tuple_to_string(data)
-        # retry
-        export_to_json(data=data, export_path=export_path, encoding=encoding, ensure_ascii=ensure_ascii)
-    pass
-
-
-def append_to_json(input_dict: Dict[str, Any], filepath: str, encoding: str = "utf-8", **kwargs):
-    """Append a dictionary to an existing JSON file. Tuple-keys are encoded to strings.
-
-    Args:
-        input_dict (Dict[str, Any]): Dictionary containing new data that should be added to file.
-        filepath (str): Absolute or relative filepath including the file extension. Depending on the current working directory.
-        encoding (str, optional): The encoding of the file. Defaults to "utf-8".
-
-    NOTE: Existing JSON file needs a 'data' key.
-
-    Raises:
-        ValueError: If input dict and file do not have the same keys or columns, respectively.
-
-    References: https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#append-to-json
-    """
-
-    # load file from path
-    with open(filepath, "r", encoding=encoding) as input_file:
-        f = json.load(input_file, **kwargs)
-    # existing file should have a "data"-key and a list to append to
-    if "data" not in f.keys():
-        raise KeyError("The file to be extended must contain the key 'data'.")
-    else:
-        try:
-            # serialize tuples if any exist
-            input_dict = _tuple_to_string(input_dict)
-            # append new dict to file
-            f["data"].append(input_dict)
-            with open(filepath, "w", encoding=encoding) as jsonfile:
-                json.dump(f, jsonfile, indent=4, **kwargs)
-        except IOError as e:
-            raise e
-        # usually when tuple cannot be serialized
-        except TypeError or json.JSONDecodeError:
-            # serialize tuples
-            input_dict = _tuple_to_string(input_dict)
-            # retry
-            append_to_json(input_dict=input_dict, filepath=filepath, encoding=encoding, **kwargs)
-    pass
-
-
-def load_from_json(filepath: str, encoding: str = "utf-8", **kwargs) -> dict:
-    """Load Python Dictionary from JSON file. Tuples are recovered.
-
-    Args:
-        filepath (str): Path to JSON file.
-        encoding (str, optional): Encoding of file. Defaults to "utf-8".
-
-    Returns:
-        dict: Python Dictionary containing (deserialized) data from JSON file.
-
-    References: https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#load-from-json
-    """
-    # read from filepath
-    with open(filepath, "r", encoding=encoding) as jsonfile:
-        f = json.load(jsonfile, **kwargs)
-
-    if "data" in f:
-        entries = [_string_to_tuple(entry) for entry in f["data"]]
-        f = {"data": entries}
-    else:
-        # try to deserialize if any tuples were found in the file
-        f = _string_to_tuple(f)
-    return f
-
-
-def strf_datetime(date: datetime, format: str = "%Y-%m-%d %H:%M:%S") -> str:
-    """Convert datetime object to string representation.
-
-    Args:
-        date (datetime): Input datetime object
-        format (str, optional): Datetime string format. Defaults to "%Y-%m-%d %H:%M:%S".
-
-    Returns:
-        str: string representation of input datetime in given format.
-    """
-    return date.strftime(format)
-
-
-def _tuple_to_string(obj: Any) -> Any:
-    """Serialize tuple-keys to string representation. A tuple wil obtain a leading '__tuple__' string and decomposed in list representation.
-
-    Args:
-        obj (Any): Typically a dict, tuple, list, int, or string.
-
-    Returns:
-        Any: Input object with serialized tuples.
-
-    Example:
-        A tuple ("WWU_Muenster", "goetheuni") will be encoded to "__tuple__["WWU_Muenster", "goetheuni"].
-    """
-    # deep copy object to avoid manipulation during iteration
-    obj_copy = copy.deepcopy(obj)
-    # if the object is a dictionary
-    if isinstance(obj, dict):
-        # iterate over every key
-        for key in obj:
-            # set for later to avoid modification in later iterations when this var does not get overwritten
-            serialized_key = None
-            # if key is tuple
-            if isinstance(key, tuple):
-                # stringify the key
-                serialized_key = f"__tuple__{list(key)}"
-                # replace old key with encoded key
-                obj_copy[serialized_key] = obj_copy.pop(key)
-            # if the key was modified
-            if serialized_key is not None:
-                # do it again for the next nested dictionary
-                obj_copy[serialized_key] = _tuple_to_string(obj[key])
-            # else, just do it for the next dictionary
-            else:
-                obj_copy[key] = _tuple_to_string(obj[key])
-    return obj_copy
-
-
-def _string_to_tuple(obj: Any) -> Any:
-    """Convert serialized tuples back to original representation. Tuples need to have a leading "__tuple__" string.
-
-    Args:
-        obj (Any): Typically a dict, tuple, list, int, or string.
-
-    Returns:
-        Any: Input object with recovered tuples.
-
-    Example:
-        A encoded tuple "__tuple__["WWU_Muenster", "goetheuni"] will be decoded to ("WWU_Muenster", "goetheuni").
-    """
-    # deep copy object to avoid manipulation during iteration
-    obj_copy = copy.deepcopy(obj)
-    # if the object is a dictionary
-    if isinstance(obj, dict):
-        # iterate over every key
-        for key in obj:
-            # set for later to avoid modification in later iterations when this var does not get overwritten
-            serialized_key = None
-            # if key is a serialized tuple starting with the "__tuple__" affix
-            if isinstance(key, str) and key.startswith("__tuple__"):
-                # decode it so tuple
-                serialized_key = tuple(key.split("__tuple__")[1].strip("[]").replace("'", "").split(", "))
-                # if key is number in string representation
-                if all(entry.isdigit() for entry in serialized_key):
-                    # convert to integer, recover ID
-                    serialized_key = tuple(map(int, serialized_key))
-                # replace old key with encoded key
-                obj_copy[serialized_key] = obj_copy.pop(key)
-            # if the key was modified
-            if serialized_key is not None:
-                # do it again for the next nested dictionary
-                obj_copy[serialized_key] = _string_to_tuple(obj[key])
-            # else, just do it for the next dictionary
-            else:
-                obj_copy[key] = _string_to_tuple(obj[key])
-    # if another instance was found
-    elif isinstance(obj, list):
-        for item in obj:
-            _string_to_tuple(item)
-    return obj_copy
+# -*- coding: utf-8 -*-
+import copy
+import json
+import warnings
+from datetime import datetime
+from typing import Any, Dict
+
+import pandas as pd
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
+
+
+def export_to_csv(data: dict, export_path: str, encoding: str = "utf-8", sep: str = ",", **kwargs):
+    """Export dictionary data to CSV file.
+
+    Args:
+        data (dict): Data dictionary (nested dictionaries are not allowed)
+        export_path (str): Export path including file name and extension.
+        encoding (str, optional): Encoding of CSV file. Defaults to 'utf-8'.
+        sep (str, optional): Value separator for CSV file. Defaults to ",".
+        kwargs: Keyword arguments for pd.DataFrame.to_csv. See references below for further details.
+
+    Raises:
+        ValueError: If nested dictionary was provided.
+        IOError: If export fails due to bad input.
+
+    References:
+        - https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#export-to-csv
+        - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_csv.html
+    """
+    # catch nested dict
+    if any(isinstance(data[key], dict) for key in data.keys()):
+        raise ValueError("'data' dictionary must not contain nested dictionaries. Use JSON export instead.")
+    try:
+        # convert to pandas dataframe from dict
+        f = pd.DataFrame(data, index=[0])
+        # export data frame
+        f.to_csv(export_path, encoding=encoding, sep=sep, index=False, **kwargs)
+    except IOError as e:
+        raise e
+
+
+def append_to_csv(data: dict, filepath: str, encoding: str = "utf-8", sep: str = ","):
+    """Append a dictionary to an existing CSV file.
+
+    Args:
+        data (dict): Dictionary containing new data that should be added to file.
+        filepath (str): Absolute or relative filepath including the file extension. Depending on the current working directory.
+        encoding (str, optional): Encoding of CSV file.. Defaults to 'utf-8'.
+        sep (str, optional): Value separator for CSV file. Defaults to ",".
+        args: Keyword Arguments for reading and writing from/to CSV file from pandas. Pass in: *[read_kwargs, write_kwargs]. See references below for further details on possible read/write arguments.
+
+    Raises:
+        ValueError: If nested dictionary was provided.
+        ValueError: If 'args' does not contain a dictionaries for read and write.
+        IOError: If export fails due to bad input.
+
+    References:
+        - https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#append-to-csv
+        - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_csv.html
+        - https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html
+    """
+    # catch nested dict
+    if any(isinstance(data[key], dict) for key in data.keys()):
+        raise ValueError("'data' dictionary must not contain nested dictionaries. Use JSON export instead.")
+    try:
+        # read existing file
+        f = pd.read_csv(filepath, sep=sep, encoding=encoding)
+        # convert data dict to df
+        input_df = pd.DataFrame(data, index=[0])
+        # concat dfs
+        f = pd.concat([f, input_df], axis=0)
+        # export to CSV
+        f.to_csv(filepath, sep=sep, encoding=encoding, index=False)
+    except IOError as e:
+        raise e
+
+
+def export_to_json(data: dict, export_path: str, encoding: str = "utf-8", ensure_ascii: bool = False, *args):
+    """Export dictionary data to JSON file. Tuple-keys are encoded to strings.
+
+    Args:
+        data (dict): Data dictionary
+        export_path (str): Export path including file name and extension.
+        encoding (str, optional): Encoding of JSON file. Defaults to "utf-8".
+        ensure_ascii (bool): Wheather to convert characters to ASCII. Defaults to False.
+
+    References: https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#export-to-json
+    """
+
+    try:
+        with open(export_path, "w", encoding=encoding) as jsonfile:
+            # add 'data' key in order to append additional dicts to same file, if not already exist
+            if "data" not in data:
+                serialized_data = {"data": [data]}
+            # dump to json
+            json.dump(serialized_data, jsonfile, indent=4, ensure_ascii=ensure_ascii, *args)
+    except IOError as e:
+        raise e
+    # usually when tuple cannot be serialized
+    except TypeError or json.JSONDecodeError:
+        # serialize tuples
+        data = _tuple_to_string(data)
+        # retry
+        export_to_json(data=data, export_path=export_path, encoding=encoding, ensure_ascii=ensure_ascii)
+    pass
+
+
+def append_to_json(input_dict: Dict[str, Any], filepath: str, encoding: str = "utf-8", **kwargs):
+    """Append a dictionary to an existing JSON file. Tuple-keys are encoded to strings.
+
+    Args:
+        input_dict (Dict[str, Any]): Dictionary containing new data that should be added to file.
+        filepath (str): Absolute or relative filepath including the file extension. Depending on the current working directory.
+        encoding (str, optional): The encoding of the file. Defaults to "utf-8".
+
+    NOTE: Existing JSON file needs a 'data' key.
+
+    Raises:
+        ValueError: If input dict and file do not have the same keys or columns, respectively.
+
+    References: https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#append-to-json
+    """
+
+    # load file from path
+    with open(filepath, "r", encoding=encoding) as input_file:
+        f = json.load(input_file, **kwargs)
+    # existing file should have a "data"-key and a list to append to
+    if "data" not in f.keys():
+        raise KeyError("The file to be extended must contain the key 'data'.")
+    else:
+        try:
+            # serialize tuples if any exist
+            input_dict = _tuple_to_string(input_dict)
+            # append new dict to file
+            f["data"].append(input_dict)
+            with open(filepath, "w", encoding=encoding) as jsonfile:
+                json.dump(f, jsonfile, indent=4, **kwargs)
+        except IOError as e:
+            raise e
+        # usually when tuple cannot be serialized
+        except TypeError or json.JSONDecodeError:
+            # serialize tuples
+            input_dict = _tuple_to_string(input_dict)
+            # retry
+            append_to_json(input_dict=input_dict, filepath=filepath, encoding=encoding, **kwargs)
+    pass
+
+
+def load_from_json(filepath: str, encoding: str = "utf-8", **kwargs) -> dict:
+    """Load Python Dictionary from JSON file. Tuples are recovered.
+
+    Args:
+        filepath (str): Path to JSON file.
+        encoding (str, optional): Encoding of file. Defaults to "utf-8".
+
+    Returns:
+        dict: Python Dictionary containing (deserialized) data from JSON file.
+
+    References: https://mathun3003.github.io/PySNA/user-guide/overview/Utilities/#load-from-json
+    """
+    # read from filepath
+    with open(filepath, "r", encoding=encoding) as jsonfile:
+        f = json.load(jsonfile, **kwargs)
+
+    if "data" in f:
+        entries = [_string_to_tuple(entry) for entry in f["data"]]
+        f = {"data": entries}
+    else:
+        # try to deserialize if any tuples were found in the file
+        f = _string_to_tuple(f)
+    return f
+
+
+def strf_datetime(date: datetime, format: str = "%Y-%m-%d %H:%M:%S") -> str:
+    """Convert datetime object to string representation.
+
+    Args:
+        date (datetime): Input datetime object
+        format (str, optional): Datetime string format. Defaults to "%Y-%m-%d %H:%M:%S".
+
+    Returns:
+        str: string representation of input datetime in given format.
+    """
+    return date.strftime(format)
+
+
+def _tuple_to_string(obj: Any) -> Any:
+    """Serialize tuple-keys to string representation. A tuple wil obtain a leading '__tuple__' string and decomposed in list representation.
+
+    Args:
+        obj (Any): Typically a dict, tuple, list, int, or string.
+
+    Returns:
+        Any: Input object with serialized tuples.
+
+    Example:
+        A tuple ("WWU_Muenster", "goetheuni") will be encoded to "__tuple__["WWU_Muenster", "goetheuni"].
+    """
+    # deep copy object to avoid manipulation during iteration
+    obj_copy = copy.deepcopy(obj)
+    # if the object is a dictionary
+    if isinstance(obj, dict):
+        # iterate over every key
+        for key in obj:
+            # set for later to avoid modification in later iterations when this var does not get overwritten
+            serialized_key = None
+            # if key is tuple
+            if isinstance(key, tuple):
+                # stringify the key
+                serialized_key = f"__tuple__{list(key)}"
+                # replace old key with encoded key
+                obj_copy[serialized_key] = obj_copy.pop(key)
+            # if the key was modified
+            if serialized_key is not None:
+                # do it again for the next nested dictionary
+                obj_copy[serialized_key] = _tuple_to_string(obj[key])
+            # else, just do it for the next dictionary
+            else:
+                obj_copy[key] = _tuple_to_string(obj[key])
+    return obj_copy
+
+
+def _string_to_tuple(obj: Any) -> Any:
+    """Convert serialized tuples back to original representation. Tuples need to have a leading "__tuple__" string.
+
+    Args:
+        obj (Any): Typically a dict, tuple, list, int, or string.
+
+    Returns:
+        Any: Input object with recovered tuples.
+
+    Example:
+        A encoded tuple "__tuple__["WWU_Muenster", "goetheuni"] will be decoded to ("WWU_Muenster", "goetheuni").
+    """
+    # deep copy object to avoid manipulation during iteration
+    obj_copy = copy.deepcopy(obj)
+    # if the object is a dictionary
+    if isinstance(obj, dict):
+        # iterate over every key
+        for key in obj:
+            # set for later to avoid modification in later iterations when this var does not get overwritten
+            serialized_key = None
+            # if key is a serialized tuple starting with the "__tuple__" affix
+            if isinstance(key, str) and key.startswith("__tuple__"):
+                # decode it so tuple
+                serialized_key = tuple(key.split("__tuple__")[1].strip("[]").replace("'", "").split(", "))
+                # if key is number in string representation
+                if all(entry.isdigit() for entry in serialized_key):
+                    # convert to integer, recover ID
+                    serialized_key = tuple(map(int, serialized_key))
+                # replace old key with encoded key
+                obj_copy[serialized_key] = obj_copy.pop(key)
+            # if the key was modified
+            if serialized_key is not None:
+                # do it again for the next nested dictionary
+                obj_copy[serialized_key] = _string_to_tuple(obj[key])
+            # else, just do it for the next dictionary
+            else:
+                obj_copy[key] = _string_to_tuple(obj[key])
+    # if another instance was found
+    elif isinstance(obj, list):
+        for item in obj:
+            _string_to_tuple(item)
+    return obj_copy
```

### Comparing `pysna-0.1.1/setup.py` & `pysna-0.1.2/setup.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# -*- coding: utf-8 -*-
-import pathlib
-import re
-
-from setuptools import find_packages, setup
-
-VERSION_FILE = "pysna/__init__.py"
-with open(VERSION_FILE) as version_file:
-    match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file.read(), re.MULTILINE)
-
-if match:
-    version = match.group(1)
-else:
-    raise RuntimeError(f"Unable to find version string in {VERSION_FILE}.")
-
-HERE = pathlib.Path(__file__).parent
-
-VERSION = version
-PACKAGE_NAME = "pysna"
-AUTHOR = "Mathis Hunke"
-AUTHOR_EMAIL = "mathun3003@gmail.com"
-URL = "https://github.com/mathun3003/PySNA"
-
-LICENSE = "MIT License"
-DESCRIPTION = "Python Package for Social Network Analytics"
-LONG_DESCRIPTION = (HERE / "README.md").read_text()
-LONG_DESC_TYPE = "text/markdown"
-
-INSTALL_REQUIRES = ["tweepy~=4.12.1", "argparse~=1.4.0", "numpy~=1.24.0", "python-dotenv~=0.21.0", "vaderSentiment~=3.3.2", "pandas~=1.5.3"]
-
-
-setup(
-    name=PACKAGE_NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type=LONG_DESC_TYPE,
-    author=AUTHOR,
-    license=LICENSE,
-    author_email=AUTHOR_EMAIL,
-    url=URL,
-    install_requires=INSTALL_REQUIRES,
-    packages=find_packages(),
-    python_requires=">=3.10",
-    entry_points={"console_scripts": ["pysna = pysna.cli:main"]},
-    project_urls={
-        "Documentation": "https://mathun3003.github.io/PySNA/",
-        "Issue Tracker": "https://github.com/mathun3003/PySNA/issues",
-        "Source Code": "https://github.com/mathun3003/PySNA",
-    },
-)
+# -*- coding: utf-8 -*-
+import pathlib
+import re
+
+from setuptools import find_packages, setup
+
+VERSION_FILE = "pysna/__init__.py"
+with open(VERSION_FILE) as version_file:
+    match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file.read(), re.MULTILINE)
+
+if match:
+    version = match.group(1)
+else:
+    raise RuntimeError(f"Unable to find version string in {VERSION_FILE}.")
+
+HERE = pathlib.Path(__file__).parent
+
+VERSION = version
+PACKAGE_NAME = "pysna"
+AUTHOR = "Mathis Hunke"
+AUTHOR_EMAIL = "mathun3003@gmail.com"
+URL = "https://github.com/mathun3003/PySNA"
+
+LICENSE = "MIT License"
+DESCRIPTION = "Python Package for Social Network Analytics"
+LONG_DESCRIPTION = (HERE / "README.md").read_text()
+LONG_DESC_TYPE = "text/markdown"
+
+INSTALL_REQUIRES = ["tweepy~=4.12.1", "argparse~=1.4.0", "numpy~=1.24.0", "python-dotenv~=0.21.0", "vaderSentiment~=3.3.2", "pandas~=1.5.3"]
+
+
+setup(
+    name=PACKAGE_NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type=LONG_DESC_TYPE,
+    author=AUTHOR,
+    license=LICENSE,
+    author_email=AUTHOR_EMAIL,
+    url=URL,
+    install_requires=INSTALL_REQUIRES,
+    packages=find_packages(),
+    python_requires=">=3.10",
+    entry_points={"console_scripts": ["pysna = pysna.cli:main"]},
+    project_urls={
+        "Documentation": "https://mathun3003.github.io/PySNA/",
+        "Issue Tracker": "https://github.com/mathun3003/PySNA/issues",
+        "Source Code": "https://github.com/mathun3003/PySNA",
+    },
+)
```

### Comparing `pysna-0.1.1/tests/test_api.py` & `pysna-0.1.2/tests/test_api.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# -*- coding: utf-8 -*-
-import pickle
-from typing import get_args
-
-from config import PySNATestCase, tape
-
-test_user_id_1 = 24677217
-test_username_1 = "WWU_Muenster"
-
-test_user_id_2 = 38180826
-test_username_2 = "goetheuni"
-
-test_user_id_3 = 160286320
-test_username_3 = "UniKonstanz"
-
-test_tweet_id_1 = 1612443577447026689
-test_tweet_id_2 = 1611301422364082180
-test_tweet_id_3 = 1612823288723476480
-
-test_tweet = "Next I'm buying Coca-Cola to put the cocaine back in."
-
-
-class TestTwitterAPI(PySNATestCase):
-
-    maxDiff = None
-
-    @tape.use_cassette("tests/cassettes/user_info.yaml")
-    def test_user_info(self):
-        user_info = self.api.user_info(test_username_1, get_args(self.api.LITERALS_USER_INFO))
-        # Assert that the response matches the saved cassette
-        cassette_response = user_info
-        with open("tests/fixtures/user_info.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        self.assertDictEqual(cassette_response, expected_response)
-
-    @tape.use_cassette("tests/cassettes/tweet_info.yaml")
-    def test_tweet_info(self):
-        cassette_response = self.api.tweet_info(test_tweet_id_1, get_args(self.api.LITERALS_TWEET_INFO))
-        with open("tests/fixtures/tweet_info.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        self.assertDictEqual(cassette_response, expected_response)
-
-    @tape.use_cassette("tests/cassettes/compare_users.yaml")
-    def test_compare_users(self):
-        cassette_response = self.api.compare_users([test_username_1, test_username_2, test_username_3], get_args(self.api.LITERALS_COMPARE_USERS), features=["followers_count", "friends_count", "listed_count", "favourites_count", "statuses_count"])
-        with open("tests/fixtures/compare_users.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        self.assertDictEqual(cassette_response, expected_response)
-
-    @tape.use_cassette("tests/cassettes/compare_tweets.yaml")
-    def test_compare_tweets(self):
-        cassette_response = self.api.compare_tweets(
-            [test_tweet_id_1, test_tweet_id_2, test_tweet_id_3],
-            get_args(self.api.LITERALS_COMPARE_TWEETS),
-            features=["retweet_count", "like_count"],
-        )
-        with open("tests/fixtures/compare_tweets.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        self.assertDictEqual(cassette_response, expected_response)
+# -*- coding: utf-8 -*-
+import pickle
+from typing import get_args
+
+from config import PySNATestCase, tape
+
+test_user_id_1 = 24677217
+test_username_1 = "WWU_Muenster"
+
+test_user_id_2 = 38180826
+test_username_2 = "goetheuni"
+
+test_user_id_3 = 160286320
+test_username_3 = "UniKonstanz"
+
+test_tweet_id_1 = 1612443577447026689
+test_tweet_id_2 = 1611301422364082180
+test_tweet_id_3 = 1612823288723476480
+
+test_tweet = "Next I'm buying Coca-Cola to put the cocaine back in."
+
+
+class TestTwitterAPI(PySNATestCase):
+
+    maxDiff = None
+
+    @tape.use_cassette("tests/cassettes/user_info.yaml")
+    def test_user_info(self):
+        user_info = self.api.user_info(test_username_1, get_args(self.api.LITERALS_USER_INFO))
+        # Assert that the response matches the saved cassette
+        cassette_response = user_info
+        with open("tests/fixtures/user_info.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        self.assertDictEqual(cassette_response, expected_response)
+
+    @tape.use_cassette("tests/cassettes/tweet_info.yaml")
+    def test_tweet_info(self):
+        cassette_response = self.api.tweet_info(test_tweet_id_1, get_args(self.api.LITERALS_TWEET_INFO))
+        with open("tests/fixtures/tweet_info.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        self.assertDictEqual(cassette_response, expected_response)
+
+    @tape.use_cassette("tests/cassettes/compare_users.yaml")
+    def test_compare_users(self):
+        cassette_response = self.api.compare_users([test_username_1, test_username_2, test_username_3], get_args(self.api.LITERALS_COMPARE_USERS), features=["followers_count", "friends_count", "listed_count", "favourites_count", "statuses_count"])
+        with open("tests/fixtures/compare_users.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        self.assertDictEqual(cassette_response, expected_response)
+
+    @tape.use_cassette("tests/cassettes/compare_tweets.yaml")
+    def test_compare_tweets(self):
+        cassette_response = self.api.compare_tweets(
+            [test_tweet_id_1, test_tweet_id_2, test_tweet_id_3],
+            get_args(self.api.LITERALS_COMPARE_TWEETS),
+            features=["retweet_count", "like_count"],
+        )
+        with open("tests/fixtures/compare_tweets.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        self.assertDictEqual(cassette_response, expected_response)
```

### Comparing `pysna-0.1.1/tests/test_fetch.py` & `pysna-0.1.2/tests/test_fetch.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,335 +1,335 @@
-# -*- coding: utf-8 -*-
-import pickle
-
-import tweepy
-from config import PySNATestCase, tape
-
-test_user_id_1 = 24677217
-test_username_1 = "WWU_Muenster"
-
-test_user_id_2 = 38180826
-test_username_2 = "goetheuni"
-
-test_user_id_3 = 160286320
-test_username_3 = "UniKonstanz"
-
-test_tweet_id_1 = 1612443577447026689
-test_tweet_id_2 = 1611301422364082180
-test_tweet_id_3 = 1612823288723476480
-
-test_tweet = "Next I'm buying Coca-Cola to put the cocaine back in."
-
-
-class TestTwitterDataFetcher(PySNATestCase):
-
-    maxDiff = None
-
-    @tape.use_cassette("tests/cassettes/manual_request.yaml")
-    def test_manual_request(self):
-        url = f"https://api.twitter.com/2/users/{test_user_id_1}"
-        cassette_response = self.fetcher._manual_request(url, "GET", additional_fields={"user.fields": ["username"]})
-        self.assertIsInstance(cassette_response, dict)
-        self.assertEqual(cassette_response["data"]["username"], test_username_1)
-        with open("tests/fixtures/manual_request.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        self.assertDictEqual(cassette_response, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_user_object.yaml")
-    def test_get_user_object(self):
-        # by screen name
-        cassette_response_1 = self.fetcher.get_user_object(test_username_1)
-        # by ID
-        cassette_response_2 = self.fetcher.get_user_object(test_user_id_1)
-        # ensure tweepy.models.User instance
-        self.assertIsInstance(cassette_response_1, tweepy.models.User)
-        self.assertIsInstance(cassette_response_2, tweepy.models.User)
-        # ensure same User
-        self.assertEqual(cassette_response_1._json["id"], test_user_id_1)
-        self.assertEqual(cassette_response_2._json["screen_name"], test_username_1)
-        # ensure same user object
-        self.assertEqual(cassette_response_1, cassette_response_2)
-        with open("tests/fixtures/get_user_object.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertDictEqual(cassette_response_1._json, expected_response)
-        self.assertDictEqual(cassette_response_2._json, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_user_follower_ids.yaml")
-    def test_get_user_follower_ids(self):
-        # by screen name
-        cassette_response_1 = self.fetcher.get_user_follower_ids(test_username_1)
-        # by ID
-        cassette_response_2 = self.fetcher.get_user_follower_ids(test_user_id_1)
-        # by string ID
-        cassette_response_3 = self.fetcher.get_user_follower_ids(str(test_user_id_1))
-        # ensure Set instance
-        self.assertIsInstance(cassette_response_1, set)
-        self.assertIsInstance(cassette_response_2, set)
-        self.assertIsInstance(cassette_response_3, set)
-        with open("tests/fixtures/get_user_follower_ids.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertSetEqual(cassette_response_1, expected_response)
-        self.assertSetEqual(cassette_response_2, expected_response)
-        self.assertSetEqual(cassette_response_3, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_user_followee_ids.yaml")
-    def test_get_user_followee_ids(self):
-        # by screen name
-        cassette_response_1 = self.fetcher.get_user_followee_ids(test_username_1)
-        # by ID
-        cassette_response_2 = self.fetcher.get_user_followee_ids(test_user_id_1)
-        # by string ID
-        cassette_response_3 = self.fetcher.get_user_followee_ids(str(test_user_id_1))
-        # ensure Set instance
-        self.assertIsInstance(cassette_response_1, set)
-        self.assertIsInstance(cassette_response_2, set)
-        self.assertIsInstance(cassette_response_3, set)
-        with open("tests/fixtures/get_user_followee_ids.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertSetEqual(cassette_response_1, expected_response)
-        self.assertSetEqual(cassette_response_2, expected_response)
-        self.assertSetEqual(cassette_response_3, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_latest_activity.yaml")
-    def test_get_latest_activity(self):
-        # by screen name
-        cassette_response_1 = self.fetcher.get_latest_activity(test_username_1)
-        # by ID
-        cassette_response_2 = self.fetcher.get_latest_activity(test_user_id_1)
-        # ensure dict instance
-        self.assertIsInstance(cassette_response_1, dict)
-        self.assertIsInstance(cassette_response_2, dict)
-        # ensure that both cassettes are equal
-        self.assertDictEqual(cassette_response_1, cassette_response_2)
-        with open("tests/fixtures/get_latest_activity.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertDictEqual(cassette_response_1, expected_response)
-        self.assertDictEqual(cassette_response_2, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_lastest_activity_date.yaml")
-    def test_get_latest_activity_date(self):
-        # by screen name
-        cassette_response_1 = self.fetcher.get_latest_activity_date(test_username_1)
-        # by ID
-        cassette_response_2 = self.fetcher.get_latest_activity_date(test_user_id_1)
-        # ensure dict instance
-        self.assertIsInstance(cassette_response_1, str)
-        self.assertIsInstance(cassette_response_2, str)
-        # ensure that both cassettes are equal
-        self.assertEqual(cassette_response_1, cassette_response_2)
-        with open("tests/fixtures/get_latest_activity_date.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertEqual(cassette_response_1, expected_response)
-        self.assertEqual(cassette_response_2, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_relationship.yaml")
-    def test_get_relationship(self):
-        # by screen name
-        cassette_response_1 = self.fetcher.get_relationship(test_username_1, test_username_2)
-        # by ID
-        cassette_response_2 = self.fetcher.get_relationship(test_user_id_1, test_user_id_2)
-        # by string ID
-        cassette_response_3 = self.fetcher.get_relationship(str(test_user_id_1), str(test_user_id_2))
-        # by ID and string ID
-        cassette_response_4 = self.fetcher.get_relationship(str(test_user_id_1), test_user_id_2)
-        cassette_response_5 = self.fetcher.get_relationship(test_user_id_1, str(test_user_id_2))
-        # ensure Set instance
-        self.assertIsInstance(cassette_response_1, dict)
-        self.assertIsInstance(cassette_response_2, dict)
-        self.assertIsInstance(cassette_response_3, dict)
-        self.assertIsInstance(cassette_response_4, dict)
-        self.assertIsInstance(cassette_response_5, dict)
-        with open("tests/fixtures/get_relationship.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertDictEqual(cassette_response_1, expected_response)
-        self.assertDictEqual(cassette_response_2, expected_response)
-        self.assertDictEqual(cassette_response_3, expected_response)
-        self.assertDictEqual(cassette_response_4, expected_response)
-        self.assertDictEqual(cassette_response_5, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_relationship_pairs.yaml")
-    def test_get_relationship_pairs(self):
-        # generate results
-        results = self.fetcher.get_relationship_pairs([test_user_id_1, test_user_id_2, test_user_id_3])
-        # assert instances
-        self.assertIsInstance(results, dict)
-        assert all(isinstance(key, tuple) for key in results.keys())
-        assert all(isinstance(value, dict) for value in results.values())
-        # compare with fixture
-        with open("tests/fixtures/get_relationship_pairs.pickle", "rb") as handle:
-            test_results = pickle.load(handle)
-        self.assertDictEqual(results, test_results)
-
-    @tape.use_cassette("tests/cassettes/get_tweet_object.yaml")
-    def test_get_tweet_object(self):
-        # by int
-        cassette_response_1 = self.fetcher.get_tweet_object(test_tweet_id_1)
-        # by str
-        cassette_response_2 = self.fetcher.get_tweet_object(str(test_tweet_id_1))
-        # ensure tweepy.models.Status instance
-        self.assertIsInstance(cassette_response_1, tweepy.models.Status)
-        self.assertIsInstance(cassette_response_2, tweepy.models.Status)
-        # ensure same status object
-        self.assertEqual(cassette_response_1, cassette_response_2)
-        with open("tests/fixtures/get_tweet_object.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertDictEqual(cassette_response_1._json, expected_response)
-        self.assertDictEqual(cassette_response_2._json, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_liking_users_ids.yaml")
-    def test_get_liking_users_ids(self):
-        cassette_response_1 = self.fetcher.get_liking_users_ids(test_tweet_id_1)
-        cassette_response_2 = self.fetcher.get_liking_users_ids(str(test_tweet_id_1))
-        # ensure set instances
-        self.assertIsInstance(cassette_response_1, list)
-        self.assertIsInstance(cassette_response_2, list)
-        # ensure same responses
-        self.assertListEqual(cassette_response_1, cassette_response_2)
-        # ensure all items are IDs
-        assert all(isinstance(item, int) for item in cassette_response_1)
-        assert all(isinstance(item, int) for item in cassette_response_2)
-        with open("tests/fixtures/get_liking_users_ids.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertListEqual(cassette_response_1, expected_response)
-        self.assertListEqual(cassette_response_2, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_retweeters_ids.yaml")
-    def test_get_retweeters_ids(self):
-        cassette_response_1 = self.fetcher.get_retweeters_ids(test_tweet_id_1)
-        cassette_response_2 = self.fetcher.get_retweeters_ids(str(test_tweet_id_1))
-        # ensure set instances
-        self.assertIsInstance(cassette_response_1, list)
-        self.assertIsInstance(cassette_response_2, list)
-        # ensure same responses
-        self.assertListEqual(cassette_response_1, cassette_response_2)
-        # ensure all items are IDs
-        assert all(isinstance(item, int) for item in cassette_response_1)
-        assert all(isinstance(item, int) for item in cassette_response_2)
-        with open("tests/fixtures/get_retweeters_ids.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertListEqual(cassette_response_1, expected_response)
-        self.assertListEqual(cassette_response_2, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_quoting_users_ids.yaml")
-    def test_get_quoting_users_ids(self):
-        cassette_response_1 = self.fetcher.get_quoting_users_ids(test_tweet_id_1)
-        cassette_response_2 = self.fetcher.get_quoting_users_ids(str(test_tweet_id_1))
-        # ensure set instances
-        self.assertIsInstance(cassette_response_1, list)
-        self.assertIsInstance(cassette_response_2, list)
-        # ensure same responses
-        self.assertListEqual(cassette_response_1, cassette_response_2)
-        # ensure all items are IDs
-        assert all(isinstance(item, int) for item in cassette_response_1)
-        assert all(isinstance(item, int) for item in cassette_response_2)
-        with open("tests/fixtures/get_quoting_users_ids.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertListEqual(cassette_response_1, expected_response)
-        self.assertListEqual(cassette_response_2, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_liked_tweets_ids.yaml")
-    def test_get_liked_tweets_ids(self):
-        cassette_response_1 = self.fetcher.get_liked_tweets_ids(test_user_id_1, limit=10)
-        cassette_response_2 = self.fetcher.get_liked_tweets_ids(str(test_user_id_1), limit=10)
-        cassette_response_3 = self.fetcher.get_liked_tweets_ids(test_username_1, limit=10)
-        # ensure set instances
-        self.assertIsInstance(cassette_response_1, list)
-        self.assertIsInstance(cassette_response_2, list)
-        self.assertIsInstance(cassette_response_3, list)
-        # ensure same responses
-        self.assertListEqual(cassette_response_1, cassette_response_2)
-        self.assertListEqual(cassette_response_1, cassette_response_3)
-        self.assertListEqual(cassette_response_2, cassette_response_3)
-        with open("tests/fixtures/get_liked_tweets_ids.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertListEqual(cassette_response_1, expected_response)
-        self.assertListEqual(cassette_response_2, expected_response)
-        self.assertListEqual(cassette_response_3, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_composed_tweets_ids.yaml")
-    def test_get_composed_tweets_ids(self):
-        cassette_response_1 = self.fetcher.get_composed_tweets_ids(test_user_id_1, limit=100)
-        cassette_response_2 = self.fetcher.get_composed_tweets_ids(str(test_user_id_1), limit=100)
-        cassette_response_3 = self.fetcher.get_composed_tweets_ids(test_username_1, limit=100)
-        # ensure set instances
-        self.assertIsInstance(cassette_response_1, list)
-        self.assertIsInstance(cassette_response_2, list)
-        self.assertIsInstance(cassette_response_3, list)
-        # ensure all items are IDs
-        assert all(isinstance(item, int) for item in cassette_response_1)
-        assert all(isinstance(item, int) for item in cassette_response_2)
-        assert all(isinstance(item, int) for item in cassette_response_3)
-        # ensure same responses
-        self.assertListEqual(cassette_response_1, cassette_response_2)
-        self.assertListEqual(cassette_response_1, cassette_response_3)
-        self.assertListEqual(cassette_response_2, cassette_response_3)
-        with open("tests/fixtures/get_composed_tweets_ids.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertListEqual(cassette_response_1, expected_response)
-        self.assertListEqual(cassette_response_2, expected_response)
-        self.assertListEqual(cassette_response_3, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_botometer_scores.yaml")
-    def test_get_botometer_scores(self):
-        cassette_response_1 = self.fetcher.get_botometer_scores(test_user_id_1)
-        cassette_response_2 = self.fetcher.get_botometer_scores(str(test_user_id_1))
-        cassette_response_3 = self.fetcher.get_botometer_scores(test_username_1)
-        # ensure dict instances
-        self.assertIsInstance(cassette_response_1, dict)
-        self.assertIsInstance(cassette_response_2, dict)
-        self.assertIsInstance(cassette_response_3, dict)
-        # ensure same responses
-        self.assertDictEqual(cassette_response_1, cassette_response_2)
-        self.assertDictEqual(cassette_response_1, cassette_response_3)
-        self.assertDictEqual(cassette_response_2, cassette_response_3)
-        with open("tests/fixtures/get_botometer_scores.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertDictEqual(cassette_response_1, expected_response)
-        self.assertDictEqual(cassette_response_2, expected_response)
-        self.assertDictEqual(cassette_response_3, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_context_annotations.yaml")
-    def test_get_context_annotations(self):
-        # by string
-        cassette_response_1 = self.fetcher.get_context_annotations_and_entities(str(test_tweet_id_1))
-        # by int
-        cassette_response_2 = self.fetcher.get_context_annotations_and_entities(test_tweet_id_1)
-        # ensure dict instance
-        self.assertIsInstance(cassette_response_1, dict)
-        self.assertIsInstance(cassette_response_2, dict)
-        # ensure same responses
-        self.assertDictEqual(cassette_response_1, cassette_response_2)
-        with open("tests/fixtures/get_context_annotations_and_entities.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertDictEqual(cassette_response_1, expected_response)
-        self.assertDictEqual(cassette_response_2, expected_response)
-
-    @tape.use_cassette("tests/cassettes/get_public_metrics.yaml")
-    def test_get_public_metrics(self):
-        # by string
-        cassette_response_1 = self.fetcher.get_public_metrics(str(test_tweet_id_1))
-        # by int
-        cassette_response_2 = self.fetcher.get_public_metrics(test_tweet_id_1)
-        # ensure dict instance
-        self.assertIsInstance(cassette_response_1, dict)
-        self.assertIsInstance(cassette_response_2, dict)
-        # ensure same responses
-        self.assertDictEqual(cassette_response_1, cassette_response_2)
-        with open("tests/fixtures/get_public_metrics.pickle", "rb") as handle:
-            expected_response = pickle.load(handle)
-        # ensure expected response
-        self.assertDictEqual(cassette_response_1, expected_response)
-        self.assertDictEqual(cassette_response_2, expected_response)
+# -*- coding: utf-8 -*-
+import pickle
+
+import tweepy
+from config import PySNATestCase, tape
+
+test_user_id_1 = 24677217
+test_username_1 = "WWU_Muenster"
+
+test_user_id_2 = 38180826
+test_username_2 = "goetheuni"
+
+test_user_id_3 = 160286320
+test_username_3 = "UniKonstanz"
+
+test_tweet_id_1 = 1612443577447026689
+test_tweet_id_2 = 1611301422364082180
+test_tweet_id_3 = 1612823288723476480
+
+test_tweet = "Next I'm buying Coca-Cola to put the cocaine back in."
+
+
+class TestTwitterDataFetcher(PySNATestCase):
+
+    maxDiff = None
+
+    @tape.use_cassette("tests/cassettes/manual_request.yaml")
+    def test_manual_request(self):
+        url = f"https://api.twitter.com/2/users/{test_user_id_1}"
+        cassette_response = self.fetcher._manual_request(url, "GET", additional_fields={"user.fields": ["username"]})
+        self.assertIsInstance(cassette_response, dict)
+        self.assertEqual(cassette_response["data"]["username"], test_username_1)
+        with open("tests/fixtures/manual_request.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        self.assertDictEqual(cassette_response, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_user_object.yaml")
+    def test_get_user_object(self):
+        # by screen name
+        cassette_response_1 = self.fetcher.get_user_object(test_username_1)
+        # by ID
+        cassette_response_2 = self.fetcher.get_user_object(test_user_id_1)
+        # ensure tweepy.models.User instance
+        self.assertIsInstance(cassette_response_1, tweepy.models.User)
+        self.assertIsInstance(cassette_response_2, tweepy.models.User)
+        # ensure same User
+        self.assertEqual(cassette_response_1._json["id"], test_user_id_1)
+        self.assertEqual(cassette_response_2._json["screen_name"], test_username_1)
+        # ensure same user object
+        self.assertEqual(cassette_response_1, cassette_response_2)
+        with open("tests/fixtures/get_user_object.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertDictEqual(cassette_response_1._json, expected_response)
+        self.assertDictEqual(cassette_response_2._json, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_user_follower_ids.yaml")
+    def test_get_user_follower_ids(self):
+        # by screen name
+        cassette_response_1 = self.fetcher.get_user_follower_ids(test_username_1)
+        # by ID
+        cassette_response_2 = self.fetcher.get_user_follower_ids(test_user_id_1)
+        # by string ID
+        cassette_response_3 = self.fetcher.get_user_follower_ids(str(test_user_id_1))
+        # ensure Set instance
+        self.assertIsInstance(cassette_response_1, set)
+        self.assertIsInstance(cassette_response_2, set)
+        self.assertIsInstance(cassette_response_3, set)
+        with open("tests/fixtures/get_user_follower_ids.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertSetEqual(cassette_response_1, expected_response)
+        self.assertSetEqual(cassette_response_2, expected_response)
+        self.assertSetEqual(cassette_response_3, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_user_followee_ids.yaml")
+    def test_get_user_followee_ids(self):
+        # by screen name
+        cassette_response_1 = self.fetcher.get_user_followee_ids(test_username_1)
+        # by ID
+        cassette_response_2 = self.fetcher.get_user_followee_ids(test_user_id_1)
+        # by string ID
+        cassette_response_3 = self.fetcher.get_user_followee_ids(str(test_user_id_1))
+        # ensure Set instance
+        self.assertIsInstance(cassette_response_1, set)
+        self.assertIsInstance(cassette_response_2, set)
+        self.assertIsInstance(cassette_response_3, set)
+        with open("tests/fixtures/get_user_followee_ids.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertSetEqual(cassette_response_1, expected_response)
+        self.assertSetEqual(cassette_response_2, expected_response)
+        self.assertSetEqual(cassette_response_3, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_latest_activity.yaml")
+    def test_get_latest_activity(self):
+        # by screen name
+        cassette_response_1 = self.fetcher.get_latest_activity(test_username_1)
+        # by ID
+        cassette_response_2 = self.fetcher.get_latest_activity(test_user_id_1)
+        # ensure dict instance
+        self.assertIsInstance(cassette_response_1, dict)
+        self.assertIsInstance(cassette_response_2, dict)
+        # ensure that both cassettes are equal
+        self.assertDictEqual(cassette_response_1, cassette_response_2)
+        with open("tests/fixtures/get_latest_activity.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertDictEqual(cassette_response_1, expected_response)
+        self.assertDictEqual(cassette_response_2, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_lastest_activity_date.yaml")
+    def test_get_latest_activity_date(self):
+        # by screen name
+        cassette_response_1 = self.fetcher.get_latest_activity_date(test_username_1)
+        # by ID
+        cassette_response_2 = self.fetcher.get_latest_activity_date(test_user_id_1)
+        # ensure dict instance
+        self.assertIsInstance(cassette_response_1, str)
+        self.assertIsInstance(cassette_response_2, str)
+        # ensure that both cassettes are equal
+        self.assertEqual(cassette_response_1, cassette_response_2)
+        with open("tests/fixtures/get_latest_activity_date.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertEqual(cassette_response_1, expected_response)
+        self.assertEqual(cassette_response_2, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_relationship.yaml")
+    def test_get_relationship(self):
+        # by screen name
+        cassette_response_1 = self.fetcher.get_relationship(test_username_1, test_username_2)
+        # by ID
+        cassette_response_2 = self.fetcher.get_relationship(test_user_id_1, test_user_id_2)
+        # by string ID
+        cassette_response_3 = self.fetcher.get_relationship(str(test_user_id_1), str(test_user_id_2))
+        # by ID and string ID
+        cassette_response_4 = self.fetcher.get_relationship(str(test_user_id_1), test_user_id_2)
+        cassette_response_5 = self.fetcher.get_relationship(test_user_id_1, str(test_user_id_2))
+        # ensure Set instance
+        self.assertIsInstance(cassette_response_1, dict)
+        self.assertIsInstance(cassette_response_2, dict)
+        self.assertIsInstance(cassette_response_3, dict)
+        self.assertIsInstance(cassette_response_4, dict)
+        self.assertIsInstance(cassette_response_5, dict)
+        with open("tests/fixtures/get_relationship.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertDictEqual(cassette_response_1, expected_response)
+        self.assertDictEqual(cassette_response_2, expected_response)
+        self.assertDictEqual(cassette_response_3, expected_response)
+        self.assertDictEqual(cassette_response_4, expected_response)
+        self.assertDictEqual(cassette_response_5, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_relationship_pairs.yaml")
+    def test_get_relationship_pairs(self):
+        # generate results
+        results = self.fetcher.get_relationship_pairs([test_user_id_1, test_user_id_2, test_user_id_3])
+        # assert instances
+        self.assertIsInstance(results, dict)
+        assert all(isinstance(key, tuple) for key in results.keys())
+        assert all(isinstance(value, dict) for value in results.values())
+        # compare with fixture
+        with open("tests/fixtures/get_relationship_pairs.pickle", "rb") as handle:
+            test_results = pickle.load(handle)
+        self.assertDictEqual(results, test_results)
+
+    @tape.use_cassette("tests/cassettes/get_tweet_object.yaml")
+    def test_get_tweet_object(self):
+        # by int
+        cassette_response_1 = self.fetcher.get_tweet_object(test_tweet_id_1)
+        # by str
+        cassette_response_2 = self.fetcher.get_tweet_object(str(test_tweet_id_1))
+        # ensure tweepy.models.Status instance
+        self.assertIsInstance(cassette_response_1, tweepy.models.Status)
+        self.assertIsInstance(cassette_response_2, tweepy.models.Status)
+        # ensure same status object
+        self.assertEqual(cassette_response_1, cassette_response_2)
+        with open("tests/fixtures/get_tweet_object.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertDictEqual(cassette_response_1._json, expected_response)
+        self.assertDictEqual(cassette_response_2._json, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_liking_users_ids.yaml")
+    def test_get_liking_users_ids(self):
+        cassette_response_1 = self.fetcher.get_liking_users_ids(test_tweet_id_1)
+        cassette_response_2 = self.fetcher.get_liking_users_ids(str(test_tweet_id_1))
+        # ensure set instances
+        self.assertIsInstance(cassette_response_1, list)
+        self.assertIsInstance(cassette_response_2, list)
+        # ensure same responses
+        self.assertListEqual(cassette_response_1, cassette_response_2)
+        # ensure all items are IDs
+        assert all(isinstance(item, int) for item in cassette_response_1)
+        assert all(isinstance(item, int) for item in cassette_response_2)
+        with open("tests/fixtures/get_liking_users_ids.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertListEqual(cassette_response_1, expected_response)
+        self.assertListEqual(cassette_response_2, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_retweeters_ids.yaml")
+    def test_get_retweeters_ids(self):
+        cassette_response_1 = self.fetcher.get_retweeters_ids(test_tweet_id_1)
+        cassette_response_2 = self.fetcher.get_retweeters_ids(str(test_tweet_id_1))
+        # ensure set instances
+        self.assertIsInstance(cassette_response_1, list)
+        self.assertIsInstance(cassette_response_2, list)
+        # ensure same responses
+        self.assertListEqual(cassette_response_1, cassette_response_2)
+        # ensure all items are IDs
+        assert all(isinstance(item, int) for item in cassette_response_1)
+        assert all(isinstance(item, int) for item in cassette_response_2)
+        with open("tests/fixtures/get_retweeters_ids.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertListEqual(cassette_response_1, expected_response)
+        self.assertListEqual(cassette_response_2, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_quoting_users_ids.yaml")
+    def test_get_quoting_users_ids(self):
+        cassette_response_1 = self.fetcher.get_quoting_users_ids(test_tweet_id_1)
+        cassette_response_2 = self.fetcher.get_quoting_users_ids(str(test_tweet_id_1))
+        # ensure set instances
+        self.assertIsInstance(cassette_response_1, list)
+        self.assertIsInstance(cassette_response_2, list)
+        # ensure same responses
+        self.assertListEqual(cassette_response_1, cassette_response_2)
+        # ensure all items are IDs
+        assert all(isinstance(item, int) for item in cassette_response_1)
+        assert all(isinstance(item, int) for item in cassette_response_2)
+        with open("tests/fixtures/get_quoting_users_ids.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertListEqual(cassette_response_1, expected_response)
+        self.assertListEqual(cassette_response_2, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_liked_tweets_ids.yaml")
+    def test_get_liked_tweets_ids(self):
+        cassette_response_1 = self.fetcher.get_liked_tweets_ids(test_user_id_1, limit=10)
+        cassette_response_2 = self.fetcher.get_liked_tweets_ids(str(test_user_id_1), limit=10)
+        cassette_response_3 = self.fetcher.get_liked_tweets_ids(test_username_1, limit=10)
+        # ensure set instances
+        self.assertIsInstance(cassette_response_1, list)
+        self.assertIsInstance(cassette_response_2, list)
+        self.assertIsInstance(cassette_response_3, list)
+        # ensure same responses
+        self.assertListEqual(cassette_response_1, cassette_response_2)
+        self.assertListEqual(cassette_response_1, cassette_response_3)
+        self.assertListEqual(cassette_response_2, cassette_response_3)
+        with open("tests/fixtures/get_liked_tweets_ids.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertListEqual(cassette_response_1, expected_response)
+        self.assertListEqual(cassette_response_2, expected_response)
+        self.assertListEqual(cassette_response_3, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_composed_tweets_ids.yaml")
+    def test_get_composed_tweets_ids(self):
+        cassette_response_1 = self.fetcher.get_composed_tweets_ids(test_user_id_1, limit=100)
+        cassette_response_2 = self.fetcher.get_composed_tweets_ids(str(test_user_id_1), limit=100)
+        cassette_response_3 = self.fetcher.get_composed_tweets_ids(test_username_1, limit=100)
+        # ensure set instances
+        self.assertIsInstance(cassette_response_1, list)
+        self.assertIsInstance(cassette_response_2, list)
+        self.assertIsInstance(cassette_response_3, list)
+        # ensure all items are IDs
+        assert all(isinstance(item, int) for item in cassette_response_1)
+        assert all(isinstance(item, int) for item in cassette_response_2)
+        assert all(isinstance(item, int) for item in cassette_response_3)
+        # ensure same responses
+        self.assertListEqual(cassette_response_1, cassette_response_2)
+        self.assertListEqual(cassette_response_1, cassette_response_3)
+        self.assertListEqual(cassette_response_2, cassette_response_3)
+        with open("tests/fixtures/get_composed_tweets_ids.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertListEqual(cassette_response_1, expected_response)
+        self.assertListEqual(cassette_response_2, expected_response)
+        self.assertListEqual(cassette_response_3, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_botometer_scores.yaml")
+    def test_get_botometer_scores(self):
+        cassette_response_1 = self.fetcher.get_botometer_scores(test_user_id_1)
+        cassette_response_2 = self.fetcher.get_botometer_scores(str(test_user_id_1))
+        cassette_response_3 = self.fetcher.get_botometer_scores(test_username_1)
+        # ensure dict instances
+        self.assertIsInstance(cassette_response_1, dict)
+        self.assertIsInstance(cassette_response_2, dict)
+        self.assertIsInstance(cassette_response_3, dict)
+        # ensure same responses
+        self.assertDictEqual(cassette_response_1, cassette_response_2)
+        self.assertDictEqual(cassette_response_1, cassette_response_3)
+        self.assertDictEqual(cassette_response_2, cassette_response_3)
+        with open("tests/fixtures/get_botometer_scores.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertDictEqual(cassette_response_1, expected_response)
+        self.assertDictEqual(cassette_response_2, expected_response)
+        self.assertDictEqual(cassette_response_3, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_context_annotations.yaml")
+    def test_get_context_annotations(self):
+        # by string
+        cassette_response_1 = self.fetcher.get_context_annotations_and_entities(str(test_tweet_id_1))
+        # by int
+        cassette_response_2 = self.fetcher.get_context_annotations_and_entities(test_tweet_id_1)
+        # ensure dict instance
+        self.assertIsInstance(cassette_response_1, dict)
+        self.assertIsInstance(cassette_response_2, dict)
+        # ensure same responses
+        self.assertDictEqual(cassette_response_1, cassette_response_2)
+        with open("tests/fixtures/get_context_annotations_and_entities.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertDictEqual(cassette_response_1, expected_response)
+        self.assertDictEqual(cassette_response_2, expected_response)
+
+    @tape.use_cassette("tests/cassettes/get_public_metrics.yaml")
+    def test_get_public_metrics(self):
+        # by string
+        cassette_response_1 = self.fetcher.get_public_metrics(str(test_tweet_id_1))
+        # by int
+        cassette_response_2 = self.fetcher.get_public_metrics(test_tweet_id_1)
+        # ensure dict instance
+        self.assertIsInstance(cassette_response_1, dict)
+        self.assertIsInstance(cassette_response_2, dict)
+        # ensure same responses
+        self.assertDictEqual(cassette_response_1, cassette_response_2)
+        with open("tests/fixtures/get_public_metrics.pickle", "rb") as handle:
+            expected_response = pickle.load(handle)
+        # ensure expected response
+        self.assertDictEqual(cassette_response_1, expected_response)
+        self.assertDictEqual(cassette_response_2, expected_response)
```

### Comparing `pysna-0.1.1/tests/test_process.py` & `pysna-0.1.2/tests/test_process.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-# -*- coding: utf-8 -*-
-import copy
-import pickle
-from datetime import datetime
-from numbers import Number
-
-import numpy as np
-from config import PySNATestCase, tape
-
-test_user_id_1 = 24677217
-test_username_1 = "WWU_Muenster"
-
-test_user_id_2 = 38180826
-test_username_2 = "goetheuni"
-
-test_user_id_3 = 160286320
-test_username_3 = "UniKonstanz"
-
-test_tweet_id_1 = 1612443577447026689
-test_tweet_id_2 = 1611301422364082180
-test_tweet_id_3 = 1612823288723476480
-
-test_tweet = "Savage Love 🎶 #SavageLoveRemix"
-
-test_sets = {test_user_id_1: set([1, 3, 5, 7]), test_user_id_2: set([3, 6, 7, 9]), test_user_id_3: set([0, 3, 7])}
-
-test_dict = {test_tweet_id_1: 150, test_tweet_id_2: 23, test_tweet_id_3: 78}
-
-dateformat = "%a %b %d %H:%M:%S %z %Y"
-
-test_dates = {
-    test_user_id_1: datetime.strptime("Mon Mar 16 11:19:30 +0000 2009", dateformat),
-    test_user_id_2: datetime.strptime("Wed May 06 13:49:31 +0000 2009", dateformat),
-    test_user_id_3: datetime.strptime("Sun Jun 27 19:10:20 +0000 2010", dateformat),
-}
-
-
-class TestBaseDataProcessor(PySNATestCase):
-
-    maxDiff = None
-
-    def test_calc_descriptive_metrics(self):
-        # calc metrics
-        results = self.data_processor.calc_descriptive_metrics(copy.deepcopy(test_dict))
-        # assert instances
-        self.assertIsInstance(results, dict)
-        assert any(isinstance(item, dict) for item in results.values())
-        # reconstruct test results
-        test_results = copy.deepcopy(test_dict)
-        test_dict_values = list(test_dict.values())
-        test_results["metrics"] = dict()
-        test_results["metrics"]["max"] = max(test_dict_values)
-        test_results["metrics"]["min"] = min(test_dict_values)
-        test_results["metrics"]["mean"] = np.array(test_dict_values).mean()
-        test_results["metrics"]["median"] = np.median(test_dict_values)
-        test_results["metrics"]["std"] = np.std(test_dict_values)
-        test_results["metrics"]["var"] = np.var(test_dict_values)
-        test_results["metrics"]["range"] = max(test_dict_values) - min(test_dict_values)
-        test_results["metrics"]["IQR"] = np.subtract(*np.percentile(test_dict_values, [75, 25]))
-        test_results["metrics"]["mad"] = np.mean(np.absolute(test_dict_values - np.mean(test_dict_values)))
-        # assert results to be equal
-        self.assertDictEqual(results, test_results)
-        pass
-
-    def test_calc_datetime_metrics(self):
-        # calc metrics
-        results = self.data_processor.calc_datetime_metrics(copy.deepcopy(test_dates))
-        # assert instances
-        self.assertIsInstance(results, dict)
-        assert any(isinstance(item, dict) for item in results.values())
-        # reconstruct test results
-        test_results = copy.deepcopy(test_dates)
-        # convert datetime to string
-        test_results = {k: dt.isoformat() for k, dt in test_results.items()}
-        metrics = {
-            "deviation_from_mean": {test_user_id_1: {"days": -174, "seconds": 73983}, test_user_id_2: {"days": -123, "seconds": 82984}, test_user_id_3: {"days": 295, "seconds": 15833}},
-            "deviation_from_median": {test_user_id_1: {"days": -52, "seconds": 77399}, test_user_id_2: {"days": 0, "seconds": 0}, test_user_id_3: {"days": 417, "seconds": 19249}},
-            "time_span": {"days": 468, "seconds": 28250, "microseconds": 0},
-            "mean": "2009-09-05T14:46:27+00:00",
-            "median": "2009-05-06T13:49:31+00:00",
-            "max": "2010-06-27T19:10:20+00:00",
-            "min": "2009-03-16T11:19:30+00:00",
-        }
-        test_results["metrics"] = metrics
-        # ensure response
-        self.assertDictEqual(results, test_results)
-
-    def test_intersection(self):
-        # calc intersection
-        results = self.data_processor.intersection(test_sets.values())
-        # assert instances
-        self.assertIsInstance(results, list)
-        assert all(isinstance(item, Number) for item in results)
-        # assert results to be equal
-        self.assertListEqual(results, [3, 7])
-
-    def test_difference(self):
-        # calc difference
-        results = self.data_processor.difference(test_sets)
-        # assert instances
-        # assert dict
-        self.assertIsInstance(results, dict)
-        # assert list as dict values
-        assert all(isinstance(item, list) for item in results.values())
-        # assert numbers as list entries
-        assert all(isinstance(entry, Number) for item in results.values() for entry in item)
-        # assert results to be equal
-        self.assertDictEqual(results, {test_user_id_1: [1, 5], test_user_id_2: [9, 6], test_user_id_3: [0]})
-
-
-class TestTwitterDataProcessor(PySNATestCase):
-
-    maxDiff = None
-
-    @tape.use_cassette("tests/cassettes/user_obj.yaml")
-    def test_extract_followers(self):
-        cassette_user = self.api.fetcher.get_user_object(test_user_id_1)
-        results = self.data_processor.extract_followers(cassette_user)
-        # ensure instances
-        self.assertIsInstance(results, dict)
-        # compare with fixture
-        with open("tests/fixtures/extract_followers.pickle", "rb") as handle:
-            test_results = pickle.load(handle)
-        self.assertDictEqual(results, test_results)
-
-    @tape.use_cassette("tests/cassettes/user_obj2.yaml")
-    def test_extract_followees(self):
-        cassette_user = self.api.fetcher.get_user_object(test_user_id_1)
-        results = self.data_processor.extract_followees(cassette_user)
-        # ensure instances
-        self.assertIsInstance(results, dict)
-        # compare with fixture
-        with open("tests/fixtures/extract_followees.pickle", "rb") as handle:
-            test_results = pickle.load(handle)
-        self.assertDictEqual(results, test_results)
-
-    def test_clean_tweet(self):
-        # generate test result
-        result = self.data_processor.clean_tweet(test_tweet)
-        # ensure instances
-        self.assertIsInstance(result, str)
-        # compare with expected result
-        self.assertEqual(result, "Savage Love SavageLoveRemix")
-
-    def test_detect_tweet_sentiment(self):
-        function_response = self.data_processor.detect_tweet_sentiment(test_tweet)
-        self.assertIsInstance(function_response, dict)
-        self.assertEqual(function_response["label"], "positive")
-
-    @tape.use_cassette("tests/cassettes/calc_similarity_users.yaml")
-    def test_calc_similarity_users(self):
-        # get serialized user objects first
-        user_objs = [self.fetcher.get_user_object(user)._json for user in [test_user_id_1, test_user_id_2, test_user_id_3]]
-        # generate results
-        results = self.data_processor.calc_similarity(user_objs=user_objs, features=["followers_count", "friends_count", "listed_count", "favourites_count", "statuses_count"])
-        # assert instances
-        self.assertIsInstance(results, dict)
-        assert all(isinstance(key, tuple) for key in results.keys())
-        assert all(isinstance(value, Number) for value in results.values())
-        # compare with fixture
-        with open("tests/fixtures/calc_similarity_users.pickle", "rb") as handle:
-            test_results = pickle.load(handle)
-        self.assertDictEqual(results, test_results)
-
-    @tape.use_cassette("tests/cassettes/calc_similarity_tweets.yaml")
-    def test_calc_similarity_tweet(self):
-        # get public metrics from Tweet objects first
-        public_metrics = {tweet_id: self.fetcher.get_public_metrics(tweet_id) for tweet_id in [test_tweet_id_1, test_tweet_id_2, test_tweet_id_3]}
-        # generate results
-        results = self.data_processor.calc_similarity(tweet_metrics=public_metrics, features=["retweet_count", "reply_count", "like_count"])
-        # assert instances
-        self.assertIsInstance(results, dict)
-        assert all(isinstance(key, tuple) for key in results.keys())
-        assert all(isinstance(value, Number) for value in results.values())
-        # compare with fixture
-        with open("tests/fixtures/calc_similarity_tweets.pickle", "rb") as handle:
-            test_results = pickle.load(handle)
-        self.assertDictEqual(results, test_results)
+# -*- coding: utf-8 -*-
+import copy
+import pickle
+from datetime import datetime
+from numbers import Number
+
+import numpy as np
+from config import PySNATestCase, tape
+
+test_user_id_1 = 24677217
+test_username_1 = "WWU_Muenster"
+
+test_user_id_2 = 38180826
+test_username_2 = "goetheuni"
+
+test_user_id_3 = 160286320
+test_username_3 = "UniKonstanz"
+
+test_tweet_id_1 = 1612443577447026689
+test_tweet_id_2 = 1611301422364082180
+test_tweet_id_3 = 1612823288723476480
+
+test_tweet = "Savage Love 🎶 #SavageLoveRemix"
+
+test_sets = {test_user_id_1: set([1, 3, 5, 7]), test_user_id_2: set([3, 6, 7, 9]), test_user_id_3: set([0, 3, 7])}
+
+test_dict = {test_tweet_id_1: 150, test_tweet_id_2: 23, test_tweet_id_3: 78}
+
+dateformat = "%a %b %d %H:%M:%S %z %Y"
+
+test_dates = {
+    test_user_id_1: datetime.strptime("Mon Mar 16 11:19:30 +0000 2009", dateformat),
+    test_user_id_2: datetime.strptime("Wed May 06 13:49:31 +0000 2009", dateformat),
+    test_user_id_3: datetime.strptime("Sun Jun 27 19:10:20 +0000 2010", dateformat),
+}
+
+
+class TestBaseDataProcessor(PySNATestCase):
+
+    maxDiff = None
+
+    def test_calc_descriptive_metrics(self):
+        # calc metrics
+        results = self.data_processor.calc_descriptive_metrics(copy.deepcopy(test_dict))
+        # assert instances
+        self.assertIsInstance(results, dict)
+        assert any(isinstance(item, dict) for item in results.values())
+        # reconstruct test results
+        test_results = copy.deepcopy(test_dict)
+        test_dict_values = list(test_dict.values())
+        test_results["metrics"] = dict()
+        test_results["metrics"]["max"] = max(test_dict_values)
+        test_results["metrics"]["min"] = min(test_dict_values)
+        test_results["metrics"]["mean"] = np.array(test_dict_values).mean()
+        test_results["metrics"]["median"] = np.median(test_dict_values)
+        test_results["metrics"]["std"] = np.std(test_dict_values)
+        test_results["metrics"]["var"] = np.var(test_dict_values)
+        test_results["metrics"]["range"] = max(test_dict_values) - min(test_dict_values)
+        test_results["metrics"]["IQR"] = np.subtract(*np.percentile(test_dict_values, [75, 25]))
+        test_results["metrics"]["mad"] = np.mean(np.absolute(test_dict_values - np.mean(test_dict_values)))
+        # assert results to be equal
+        self.assertDictEqual(results, test_results)
+        pass
+
+    def test_calc_datetime_metrics(self):
+        # calc metrics
+        results = self.data_processor.calc_datetime_metrics(copy.deepcopy(test_dates))
+        # assert instances
+        self.assertIsInstance(results, dict)
+        assert any(isinstance(item, dict) for item in results.values())
+        # reconstruct test results
+        test_results = copy.deepcopy(test_dates)
+        # convert datetime to string
+        test_results = {k: dt.isoformat() for k, dt in test_results.items()}
+        metrics = {
+            "deviation_from_mean": {test_user_id_1: {"days": -174, "seconds": 73983}, test_user_id_2: {"days": -123, "seconds": 82984}, test_user_id_3: {"days": 295, "seconds": 15833}},
+            "deviation_from_median": {test_user_id_1: {"days": -52, "seconds": 77399}, test_user_id_2: {"days": 0, "seconds": 0}, test_user_id_3: {"days": 417, "seconds": 19249}},
+            "time_span": {"days": 468, "seconds": 28250, "microseconds": 0},
+            "mean": "2009-09-05T14:46:27+00:00",
+            "median": "2009-05-06T13:49:31+00:00",
+            "max": "2010-06-27T19:10:20+00:00",
+            "min": "2009-03-16T11:19:30+00:00",
+        }
+        test_results["metrics"] = metrics
+        # ensure response
+        self.assertDictEqual(results, test_results)
+
+    def test_intersection(self):
+        # calc intersection
+        results = self.data_processor.intersection(test_sets.values())
+        # assert instances
+        self.assertIsInstance(results, list)
+        assert all(isinstance(item, Number) for item in results)
+        # assert results to be equal
+        self.assertListEqual(results, [3, 7])
+
+    def test_difference(self):
+        # calc difference
+        results = self.data_processor.difference(test_sets)
+        # assert instances
+        # assert dict
+        self.assertIsInstance(results, dict)
+        # assert list as dict values
+        assert all(isinstance(item, list) for item in results.values())
+        # assert numbers as list entries
+        assert all(isinstance(entry, Number) for item in results.values() for entry in item)
+        # assert results to be equal
+        self.assertDictEqual(results, {test_user_id_1: [1, 5], test_user_id_2: [9, 6], test_user_id_3: [0]})
+
+
+class TestTwitterDataProcessor(PySNATestCase):
+
+    maxDiff = None
+
+    @tape.use_cassette("tests/cassettes/user_obj.yaml")
+    def test_extract_followers(self):
+        cassette_user = self.api.fetcher.get_user_object(test_user_id_1)
+        results = self.data_processor.extract_followers(cassette_user)
+        # ensure instances
+        self.assertIsInstance(results, dict)
+        # compare with fixture
+        with open("tests/fixtures/extract_followers.pickle", "rb") as handle:
+            test_results = pickle.load(handle)
+        self.assertDictEqual(results, test_results)
+
+    @tape.use_cassette("tests/cassettes/user_obj2.yaml")
+    def test_extract_followees(self):
+        cassette_user = self.api.fetcher.get_user_object(test_user_id_1)
+        results = self.data_processor.extract_followees(cassette_user)
+        # ensure instances
+        self.assertIsInstance(results, dict)
+        # compare with fixture
+        with open("tests/fixtures/extract_followees.pickle", "rb") as handle:
+            test_results = pickle.load(handle)
+        self.assertDictEqual(results, test_results)
+
+    def test_clean_tweet(self):
+        # generate test result
+        result = self.data_processor.clean_tweet(test_tweet)
+        # ensure instances
+        self.assertIsInstance(result, str)
+        # compare with expected result
+        self.assertEqual(result, "Savage Love SavageLoveRemix")
+
+    def test_detect_tweet_sentiment(self):
+        function_response = self.data_processor.detect_tweet_sentiment(test_tweet)
+        self.assertIsInstance(function_response, dict)
+        self.assertEqual(function_response["label"], "positive")
+
+    @tape.use_cassette("tests/cassettes/calc_similarity_users.yaml")
+    def test_calc_similarity_users(self):
+        # get serialized user objects first
+        user_objs = [self.fetcher.get_user_object(user)._json for user in [test_user_id_1, test_user_id_2, test_user_id_3]]
+        # generate results
+        results = self.data_processor.calc_similarity(user_objs=user_objs, features=["followers_count", "friends_count", "listed_count", "favourites_count", "statuses_count"])
+        # assert instances
+        self.assertIsInstance(results, dict)
+        assert all(isinstance(key, tuple) for key in results.keys())
+        assert all(isinstance(value, Number) for value in results.values())
+        # compare with fixture
+        with open("tests/fixtures/calc_similarity_users.pickle", "rb") as handle:
+            test_results = pickle.load(handle)
+        self.assertDictEqual(results, test_results)
+
+    @tape.use_cassette("tests/cassettes/calc_similarity_tweets.yaml")
+    def test_calc_similarity_tweet(self):
+        # get public metrics from Tweet objects first
+        public_metrics = {tweet_id: self.fetcher.get_public_metrics(tweet_id) for tweet_id in [test_tweet_id_1, test_tweet_id_2, test_tweet_id_3]}
+        # generate results
+        results = self.data_processor.calc_similarity(tweet_metrics=public_metrics, features=["retweet_count", "reply_count", "like_count"])
+        # assert instances
+        self.assertIsInstance(results, dict)
+        assert all(isinstance(key, tuple) for key in results.keys())
+        assert all(isinstance(value, Number) for value in results.values())
+        # compare with fixture
+        with open("tests/fixtures/calc_similarity_tweets.pickle", "rb") as handle:
+            test_results = pickle.load(handle)
+        self.assertDictEqual(results, test_results)
```

### Comparing `pysna-0.1.1/tests/test_utils.py` & `pysna-0.1.2/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# -*- coding: utf-8 -*-
-from config import PySNATestCase
-
-from pysna.utils import _string_to_tuple, _tuple_to_string
-
-test_tuple = ("WWU_Muenster", "goetheuni")
-test_dict_decoded = {test_tuple: {test_tuple: 0.5, "id": 123}, (123, 456): 0.6}
-test_dict_encoded = {"__tuple__['WWU_Muenster', 'goetheuni']": {"id": 123, "__tuple__['WWU_Muenster', 'goetheuni']": 0.5}, "__tuple__[123, 456]": 0.6}
-
-
-class TestPrivateUtils(PySNATestCase):
-
-    maxDiff = None
-
-    def test_tuples_to_string(self):
-        # create results
-        dict_results = _tuple_to_string(test_dict_decoded)
-        # assert instances
-        self.assertIsInstance(dict_results, dict)
-        # compare with expected results
-        self.assertDictEqual(dict_results, test_dict_encoded)
-
-    def test_string_to_tuple(self):
-        # create results
-        dict_results = _string_to_tuple(test_dict_encoded)
-        # assert instances
-        self.assertIsInstance(dict_results, dict)
-        # compare with expected results
-        self.assertDictEqual(dict_results, test_dict_decoded)
+# -*- coding: utf-8 -*-
+from config import PySNATestCase
+
+from pysna.utils import _string_to_tuple, _tuple_to_string
+
+test_tuple = ("WWU_Muenster", "goetheuni")
+test_dict_decoded = {test_tuple: {test_tuple: 0.5, "id": 123}, (123, 456): 0.6}
+test_dict_encoded = {"__tuple__['WWU_Muenster', 'goetheuni']": {"id": 123, "__tuple__['WWU_Muenster', 'goetheuni']": 0.5}, "__tuple__[123, 456]": 0.6}
+
+
+class TestPrivateUtils(PySNATestCase):
+
+    maxDiff = None
+
+    def test_tuples_to_string(self):
+        # create results
+        dict_results = _tuple_to_string(test_dict_decoded)
+        # assert instances
+        self.assertIsInstance(dict_results, dict)
+        # compare with expected results
+        self.assertDictEqual(dict_results, test_dict_encoded)
+
+    def test_string_to_tuple(self):
+        # create results
+        dict_results = _string_to_tuple(test_dict_encoded)
+        # assert instances
+        self.assertIsInstance(dict_results, dict)
+        # compare with expected results
+        self.assertDictEqual(dict_results, test_dict_decoded)
```

