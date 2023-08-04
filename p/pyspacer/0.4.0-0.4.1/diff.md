# Comparing `tmp/pyspacer-0.4.0.tar.gz` & `tmp/pyspacer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspacer-0.4.0.tar", last modified: Fri May  5 06:55:27 2023, max compression
+gzip compressed data, was "pyspacer-0.4.1.tar", last modified: Fri Aug  4 09:16:17 2023, max compression
```

## Comparing `pyspacer-0.4.0.tar` & `pyspacer-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.765171 pyspacer-0.4.0/
--rw-rw-rw-   0        0        0      320 2023-05-05 06:55:07.000000 pyspacer-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5595 2023-05-05 06:55:27.762179 pyspacer-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3764 2023-03-22 02:10:27.000000 pyspacer-0.4.0/README.md
--rw-rw-rw-   0        0        0     1073 2023-01-18 22:46:34.000000 pyspacer-0.4.0/license.txt
--rw-rw-rw-   0        0        0      754 2023-05-05 06:35:48.000000 pyspacer-0.4.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.727298 pyspacer-0.4.0/pyspacer.egg-info/
--rw-rw-rw-   0        0        0     5595 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 06:55:27.765171 pyspacer-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.755202 pyspacer-0.4.0/spacer/
--rw-rw-rw-   0        0        0       21 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/__init__.py
--rw-rw-rw-   0        0        0     4570 2023-01-23 20:13:32.000000 pyspacer-0.4.0/spacer/caffe_utils.py
--rw-rw-rw-   0        0        0     5274 2023-04-27 05:43:33.000000 pyspacer-0.4.0/spacer/config.py
--rw-rw-rw-   0        0        0    10871 2023-01-23 20:13:32.000000 pyspacer-0.4.0/spacer/data_classes.py
--rw-rw-rw-   0        0        0      271 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/exceptions.py
--rw-rw-rw-   0        0        0     5931 2023-04-25 04:49:47.000000 pyspacer-0.4.0/spacer/extract_features.py
--rw-rw-rw-   0        0        0     1573 2023-01-25 01:02:22.000000 pyspacer-0.4.0/spacer/extract_features_utils.py
--rw-rw-rw-   0        0        0     2718 2023-04-20 05:31:47.000000 pyspacer-0.4.0/spacer/mailman.py
--rw-rw-rw-   0        0        0    17105 2023-04-25 04:49:47.000000 pyspacer-0.4.0/spacer/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.760210 pyspacer-0.4.0/spacer/models/
--rw-rw-rw-   0        0        0      405 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/models/__init__.py
--rw-rw-rw-   0        0        0    10959 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/models/effcientnet_utils.py
--rw-rw-rw-   0        0        0     9854 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/models/efficientnet.py
--rw-rw-rw-   0        0        0    10695 2023-04-15 21:20:49.000000 pyspacer-0.4.0/spacer/storage.py
--rw-rw-rw-   0        0        0      840 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/task_utils.py
--rw-rw-rw-   0        0        0     4547 2023-01-19 01:13:55.000000 pyspacer-0.4.0/spacer/tasks.py
--rw-rw-rw-   0        0        0     2809 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/torch_utils.py
--rw-rw-rw-   0        0        0     2690 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/train_classifier.py
--rw-rw-rw-   0        0        0     8837 2023-01-24 22:36:53.000000 pyspacer-0.4.0/spacer/train_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:16:17.772266 pyspacer-0.4.1/
+-rw-rw-rw-   0        0        0      320 2023-06-08 08:12:51.000000 pyspacer-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6387 2023-08-04 09:16:17.772266 pyspacer-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4643 2023-08-04 08:39:40.000000 pyspacer-0.4.1/README.md
+-rw-rw-rw-   0        0        0     1073 2023-01-18 22:46:34.000000 pyspacer-0.4.1/license.txt
+-rw-rw-rw-   0        0        0      755 2023-08-04 08:36:18.000000 pyspacer-0.4.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-04 09:16:17.722147 pyspacer-0.4.1/pyspacer.egg-info/
+-rw-rw-rw-   0        0        0     6387 2023-08-04 09:16:17.000000 pyspacer-0.4.1/pyspacer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-08-04 09:16:17.000000 pyspacer-0.4.1/pyspacer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 09:16:17.000000 pyspacer-0.4.1/pyspacer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-08-04 09:16:17.000000 pyspacer-0.4.1/pyspacer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 09:16:17.000000 pyspacer-0.4.1/pyspacer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 09:16:17.772266 pyspacer-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 09:16:17.767207 pyspacer-0.4.1/spacer/
+-rw-rw-rw-   0        0        0       21 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-06-08 08:12:51.000000 pyspacer-0.4.1/spacer/caffe_utils.py
+-rw-rw-rw-   0        0        0     7445 2023-08-04 08:35:41.000000 pyspacer-0.4.1/spacer/config.py
+-rw-rw-rw-   0        0        0    11178 2023-06-08 08:12:51.000000 pyspacer-0.4.1/spacer/data_classes.py
+-rw-rw-rw-   0        0        0      271 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/exceptions.py
+-rw-rw-rw-   0        0        0     6107 2023-06-08 08:12:51.000000 pyspacer-0.4.1/spacer/extract_features.py
+-rw-rw-rw-   0        0        0     1633 2023-06-08 08:12:51.000000 pyspacer-0.4.1/spacer/extract_features_utils.py
+-rw-rw-rw-   0        0        0     2798 2023-06-08 08:12:51.000000 pyspacer-0.4.1/spacer/mailman.py
+-rw-rw-rw-   0        0        0    17573 2023-06-08 08:12:51.000000 pyspacer-0.4.1/spacer/messages.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:16:17.772266 pyspacer-0.4.1/spacer/models/
+-rw-rw-rw-   0        0        0      405 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/models/__init__.py
+-rw-rw-rw-   0        0        0    10959 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/models/effcientnet_utils.py
+-rw-rw-rw-   0        0        0     9854 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/models/efficientnet.py
+-rw-rw-rw-   0        0        0    11461 2023-06-08 08:12:51.000000 pyspacer-0.4.1/spacer/storage.py
+-rw-rw-rw-   0        0        0      840 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/task_utils.py
+-rw-rw-rw-   0        0        0     4547 2023-05-14 01:45:58.000000 pyspacer-0.4.1/spacer/tasks.py
+-rw-rw-rw-   0        0        0     2809 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/torch_utils.py
+-rw-rw-rw-   0        0        0     2690 2023-01-18 22:46:34.000000 pyspacer-0.4.1/spacer/train_classifier.py
+-rw-rw-rw-   0        0        0     9075 2023-06-08 08:12:52.000000 pyspacer-0.4.1/spacer/train_utils.py
```

### Comparing `pyspacer-0.4.0/PKG-INFO` & `pyspacer-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspacer
-Version: 0.4.0
+Version: 0.4.1
 Summary: Spatial image analysis with pytorch and caffe backends.
 Author-email: Oscar Beijbom <oscar.beijbom@gmail.com>
 License: MIT License
         
         Copyright (c) [2020] [Oscar Beijbom]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,30 +20,30 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/beijbom/pyspacer
+Project-URL: Homepage, https://github.com/coralnet/pyspacer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # PySpacer
 
-[![CI Status](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml/badge.svg)](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml)
+[![CI Status](https://github.com/coralnet/pyspacer/actions/workflows/python-app.yml/badge.svg)](https://github.com/coralnet/pyspacer/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/pyspacer.svg)](https://badge.fury.io/py/pyspacer)
 
 This repository provide utilities to extract features from random point 
 locations in images and then training classifiers over those features.
-It is used in the vision backend of `https://github.com/beijbom/coralnet`.
+It is used in the vision backend of `https://github.com/coralnet/coralnet`.
 
 Spacer currently supports python >=3.8.
 
 ### Overview
 Spacer executes tasks as defined in messages. The messages types are defined
 in `messages.py` and the tasks in `tasks.py`. We also define several data-types
 in `data_classes.py` which define input and output types. 
@@ -64,28 +64,40 @@
 
 The spacer repo can be installed in three ways.
 * Using Docker -- the only option that supports Caffe.
 * Local clone -- ideal for testing and development.
 * Using pip install -- for integration in other code-bases.
 
 #### Config
-Spacer needs three variables. They can either be set
-as environmental variables (recommended if you `pip install` the package), 
-or in a `secrets.json` file in the same directory as this README 
-(recommended for Docker builds and local clones). 
-The `secrets.json` should look like this.
-```json
-{
-  "SPACER_AWS_ACCESS_KEY_ID": "YOUR_AWS_KEY_ID",
-  "SPACER_AWS_SECRET_ACCESS_KEY": "YOUR_AWS_SECRET_KEY",
-  "SPACER_LOCAL_MODEL_PATH": "/path/to/your/local/models"
-}
-```
+Spacer's config variables can be set in any of the following ways:
 
-There is also an optional `TMP_PATH` setting: a filesystem directory to use for temporary files from unit tests and downloads. It defaults to the relative path `tmp`.
+1. As environment variables; recommended if you `pip install` the package. Each variable name must be prefixed with `SPACER_`:
+   - `export SPACER_AWS_ACCESS_KEY_ID='YOUR_AWS_KEY_ID'`
+   - `export SPACER_AWS_SECRET_ACCESS_KEY='YOUR_AWS_SECRET_KEY'`
+   - `export SPACER_LOCAL_MODEL_PATH='/path/to/your/local/models'`
+2. As a Django setting; recommended for a Django project that uses spacer. Example code in a Django settings module:
+   ```python
+   SPACER = {
+       'AWS_ACCESS_KEY_ID': 'YOUR_AWS_KEY_ID',
+       'AWS_SECRET_ACCESS_KEY': 'YOUR_AWS_SECRET_KEY',
+       'LOCAL_MODEL_PATH': '/path/to/your/local/models',
+   }
+   ```
+3. In a `secrets.json` file in the same directory as this README; recommended for Docker builds and local clones. Example `secrets.json` contents:
+   ```json
+   {
+     "AWS_ACCESS_KEY_ID": "YOUR_AWS_KEY_ID",
+     "AWS_SECRET_ACCESS_KEY": "YOUR_AWS_SECRET_KEY",
+     "LOCAL_MODEL_PATH": "/path/to/your/local/models"
+   }
+   ```
+   
+LOCAL_MODEL_PATH is required. The two AWS access variables are required unless spacer is running on an AWS instance which has been set up with `aws configure`. The rest of the config variables are optional; see `CONFIGURABLE_VARS` in `config.py` for a full list.
+
+To debug your configuration, try opening a Python shell and run `from spacer import config`, then `config.check()`.
 
 #### Docker build
 The docker build is the preferred build and the one used in deployment.
 * Install docker on your system
 * Create `secrets.json` as detailed above.
 * Create folder `/path/to/your/local/models` for caching model files.
 * Build image: `docker build -t spacer:test .`
@@ -99,15 +111,15 @@
 `secrets.json` so that the container has the right permissions.
 
 The last step will run the default CMD command specified in the dockerfile 
 (unit-test with coverage). If you want to enter the docker container 
 run the same command but append `bash` in the end.
 
 #### Pip install
-* `pip install spacer`
+* `pip install pyspacer`
 * Set environmental variables.
 
 #### Local clone
 * Clone this repo
 * `pip install -r requirements.txt`
 
 If using Windows: turn Git's `autocrlf` setting off before your initial checkout. Otherwise, pickled classifiers in `spacer/tests/fixtures` will get checked out with `\r\n` newlines, and the pickle module will fail to load them, leading to test failures. However, autocrlf should be left on when adding any new non-pickle files.
```

### Comparing `pyspacer-0.4.0/README.md` & `pyspacer-0.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,100 @@
-# PySpacer
-
-[![CI Status](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml/badge.svg)](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml)
-[![PyPI version](https://badge.fury.io/py/pyspacer.svg)](https://badge.fury.io/py/pyspacer)
-
-This repository provide utilities to extract features from random point 
-locations in images and then training classifiers over those features.
-It is used in the vision backend of `https://github.com/beijbom/coralnet`.
-
-Spacer currently supports python >=3.8.
-
-### Overview
-Spacer executes tasks as defined in messages. The messages types are defined
-in `messages.py` and the tasks in `tasks.py`. We also define several data-types
-in `data_classes.py` which define input and output types. 
-
-Refer to the unit-test in `test_tasks.py` for examples on how to create tasks.
-
-Tasks can be executed directly by calling the methods in tasks.py. 
-However, spacer also supports an interface with AWS Batch 
-handled by `env_job()` in `mailman.py`. 
-
-Spacer supports four storage types: `s3`, `filesystem`, `memory` and `url`.
- Refer to `storage.py` for details. The Memory storage is mostly used for 
- testing, and the `url` storage is read only.
-
-Also take a look at `config.py` for settings and configuration. 
-
-### Installation
-
-The spacer repo can be installed in three ways.
-* Using Docker -- the only option that supports Caffe.
-* Local clone -- ideal for testing and development.
-* Using pip install -- for integration in other code-bases.
-
-#### Config
-Spacer needs three variables. They can either be set
-as environmental variables (recommended if you `pip install` the package), 
-or in a `secrets.json` file in the same directory as this README 
-(recommended for Docker builds and local clones). 
-The `secrets.json` should look like this.
-```json
-{
-  "SPACER_AWS_ACCESS_KEY_ID": "YOUR_AWS_KEY_ID",
-  "SPACER_AWS_SECRET_ACCESS_KEY": "YOUR_AWS_SECRET_KEY",
-  "SPACER_LOCAL_MODEL_PATH": "/path/to/your/local/models"
-}
-```
-
-There is also an optional `TMP_PATH` setting: a filesystem directory to use for temporary files from unit tests and downloads. It defaults to the relative path `tmp`.
-
-#### Docker build
-The docker build is the preferred build and the one used in deployment.
-* Install docker on your system
-* Create `secrets.json` as detailed above.
-* Create folder `/path/to/your/local/models` for caching model files.
-* Build image: `docker build -t spacer:test .`
-* Run: `docker run -v /path/to/your/local/models:/workspace/models -v ${PWD}:/workspace/spacer/ -it spacer:test`
-
-The `-v /path/to/your/local/models:/workspace/models` part will make sure 
-the downloaded models are cached to your host storage. 
-which makes rerunning stuff much faster.
-
-The `-v ${PWD}:/workspace/spacer/` mounts your current folder including 
-`secrets.json` so that the container has the right permissions.
-
-The last step will run the default CMD command specified in the dockerfile 
-(unit-test with coverage). If you want to enter the docker container 
-run the same command but append `bash` in the end.
-
-#### Pip install
-* `pip install spacer`
-* Set environmental variables.
-
-#### Local clone
-* Clone this repo
-* `pip install -r requirements.txt`
-
-If using Windows: turn Git's `autocrlf` setting off before your initial checkout. Otherwise, pickled classifiers in `spacer/tests/fixtures` will get checked out with `\r\n` newlines, and the pickle module will fail to load them, leading to test failures. However, autocrlf should be left on when adding any new non-pickle files.
-
-### Code coverage
-If you are using the docker build or local install, 
-you can check code coverage like so:
-```
-    coverage run --source=spacer --omit=spacer/tests/* -m unittest    
-    coverage report -m
-    coverage html
-```
+# PySpacer
+
+[![CI Status](https://github.com/coralnet/pyspacer/actions/workflows/python-app.yml/badge.svg)](https://github.com/coralnet/pyspacer/actions/workflows/python-app.yml)
+[![PyPI version](https://badge.fury.io/py/pyspacer.svg)](https://badge.fury.io/py/pyspacer)
+
+This repository provide utilities to extract features from random point 
+locations in images and then training classifiers over those features.
+It is used in the vision backend of `https://github.com/coralnet/coralnet`.
+
+Spacer currently supports python >=3.8.
+
+### Overview
+Spacer executes tasks as defined in messages. The messages types are defined
+in `messages.py` and the tasks in `tasks.py`. We also define several data-types
+in `data_classes.py` which define input and output types. 
+
+Refer to the unit-test in `test_tasks.py` for examples on how to create tasks.
+
+Tasks can be executed directly by calling the methods in tasks.py. 
+However, spacer also supports an interface with AWS Batch 
+handled by `env_job()` in `mailman.py`. 
+
+Spacer supports four storage types: `s3`, `filesystem`, `memory` and `url`.
+ Refer to `storage.py` for details. The Memory storage is mostly used for 
+ testing, and the `url` storage is read only.
+
+Also take a look at `config.py` for settings and configuration. 
+
+### Installation
+
+The spacer repo can be installed in three ways.
+* Using Docker -- the only option that supports Caffe.
+* Local clone -- ideal for testing and development.
+* Using pip install -- for integration in other code-bases.
+
+#### Config
+Spacer's config variables can be set in any of the following ways:
+
+1. As environment variables; recommended if you `pip install` the package. Each variable name must be prefixed with `SPACER_`:
+   - `export SPACER_AWS_ACCESS_KEY_ID='YOUR_AWS_KEY_ID'`
+   - `export SPACER_AWS_SECRET_ACCESS_KEY='YOUR_AWS_SECRET_KEY'`
+   - `export SPACER_LOCAL_MODEL_PATH='/path/to/your/local/models'`
+2. As a Django setting; recommended for a Django project that uses spacer. Example code in a Django settings module:
+   ```python
+   SPACER = {
+       'AWS_ACCESS_KEY_ID': 'YOUR_AWS_KEY_ID',
+       'AWS_SECRET_ACCESS_KEY': 'YOUR_AWS_SECRET_KEY',
+       'LOCAL_MODEL_PATH': '/path/to/your/local/models',
+   }
+   ```
+3. In a `secrets.json` file in the same directory as this README; recommended for Docker builds and local clones. Example `secrets.json` contents:
+   ```json
+   {
+     "AWS_ACCESS_KEY_ID": "YOUR_AWS_KEY_ID",
+     "AWS_SECRET_ACCESS_KEY": "YOUR_AWS_SECRET_KEY",
+     "LOCAL_MODEL_PATH": "/path/to/your/local/models"
+   }
+   ```
+   
+LOCAL_MODEL_PATH is required. The two AWS access variables are required unless spacer is running on an AWS instance which has been set up with `aws configure`. The rest of the config variables are optional; see `CONFIGURABLE_VARS` in `config.py` for a full list.
+
+To debug your configuration, try opening a Python shell and run `from spacer import config`, then `config.check()`.
+
+#### Docker build
+The docker build is the preferred build and the one used in deployment.
+* Install docker on your system
+* Create `secrets.json` as detailed above.
+* Create folder `/path/to/your/local/models` for caching model files.
+* Build image: `docker build -t spacer:test .`
+* Run: `docker run -v /path/to/your/local/models:/workspace/models -v ${PWD}:/workspace/spacer/ -it spacer:test`
+
+The `-v /path/to/your/local/models:/workspace/models` part will make sure 
+the downloaded models are cached to your host storage. 
+which makes rerunning stuff much faster.
+
+The `-v ${PWD}:/workspace/spacer/` mounts your current folder including 
+`secrets.json` so that the container has the right permissions.
+
+The last step will run the default CMD command specified in the dockerfile 
+(unit-test with coverage). If you want to enter the docker container 
+run the same command but append `bash` in the end.
+
+#### Pip install
+* `pip install pyspacer`
+* Set environmental variables.
+
+#### Local clone
+* Clone this repo
+* `pip install -r requirements.txt`
+
+If using Windows: turn Git's `autocrlf` setting off before your initial checkout. Otherwise, pickled classifiers in `spacer/tests/fixtures` will get checked out with `\r\n` newlines, and the pickle module will fail to load them, leading to test failures. However, autocrlf should be left on when adding any new non-pickle files.
+
+### Code coverage
+If you are using the docker build or local install, 
+you can check code coverage like so:
+```
+    coverage run --source=spacer --omit=spacer/tests/* -m unittest    
+    coverage report -m
+    coverage html
+```
```

### Comparing `pyspacer-0.4.0/license.txt` & `pyspacer-0.4.1/license.txt`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/pyproject.toml` & `pyspacer-0.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyspacer"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Oscar Beijbom", email="oscar.beijbom@gmail.com" },
 ]
 description = "Spatial image analysis with pytorch and caffe backends."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -23,8 +23,8 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/beijbom/pyspacer"
+"Homepage" = "https://github.com/coralnet/pyspacer"
```

### Comparing `pyspacer-0.4.0/pyspacer.egg-info/PKG-INFO` & `pyspacer-0.4.1/pyspacer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspacer
-Version: 0.4.0
+Version: 0.4.1
 Summary: Spatial image analysis with pytorch and caffe backends.
 Author-email: Oscar Beijbom <oscar.beijbom@gmail.com>
 License: MIT License
         
         Copyright (c) [2020] [Oscar Beijbom]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,30 +20,30 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/beijbom/pyspacer
+Project-URL: Homepage, https://github.com/coralnet/pyspacer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # PySpacer
 
-[![CI Status](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml/badge.svg)](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml)
+[![CI Status](https://github.com/coralnet/pyspacer/actions/workflows/python-app.yml/badge.svg)](https://github.com/coralnet/pyspacer/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/pyspacer.svg)](https://badge.fury.io/py/pyspacer)
 
 This repository provide utilities to extract features from random point 
 locations in images and then training classifiers over those features.
-It is used in the vision backend of `https://github.com/beijbom/coralnet`.
+It is used in the vision backend of `https://github.com/coralnet/coralnet`.
 
 Spacer currently supports python >=3.8.
 
 ### Overview
 Spacer executes tasks as defined in messages. The messages types are defined
 in `messages.py` and the tasks in `tasks.py`. We also define several data-types
 in `data_classes.py` which define input and output types. 
@@ -64,28 +64,40 @@
 
 The spacer repo can be installed in three ways.
 * Using Docker -- the only option that supports Caffe.
 * Local clone -- ideal for testing and development.
 * Using pip install -- for integration in other code-bases.
 
 #### Config
-Spacer needs three variables. They can either be set
-as environmental variables (recommended if you `pip install` the package), 
-or in a `secrets.json` file in the same directory as this README 
-(recommended for Docker builds and local clones). 
-The `secrets.json` should look like this.
-```json
-{
-  "SPACER_AWS_ACCESS_KEY_ID": "YOUR_AWS_KEY_ID",
-  "SPACER_AWS_SECRET_ACCESS_KEY": "YOUR_AWS_SECRET_KEY",
-  "SPACER_LOCAL_MODEL_PATH": "/path/to/your/local/models"
-}
-```
+Spacer's config variables can be set in any of the following ways:
 
-There is also an optional `TMP_PATH` setting: a filesystem directory to use for temporary files from unit tests and downloads. It defaults to the relative path `tmp`.
+1. As environment variables; recommended if you `pip install` the package. Each variable name must be prefixed with `SPACER_`:
+   - `export SPACER_AWS_ACCESS_KEY_ID='YOUR_AWS_KEY_ID'`
+   - `export SPACER_AWS_SECRET_ACCESS_KEY='YOUR_AWS_SECRET_KEY'`
+   - `export SPACER_LOCAL_MODEL_PATH='/path/to/your/local/models'`
+2. As a Django setting; recommended for a Django project that uses spacer. Example code in a Django settings module:
+   ```python
+   SPACER = {
+       'AWS_ACCESS_KEY_ID': 'YOUR_AWS_KEY_ID',
+       'AWS_SECRET_ACCESS_KEY': 'YOUR_AWS_SECRET_KEY',
+       'LOCAL_MODEL_PATH': '/path/to/your/local/models',
+   }
+   ```
+3. In a `secrets.json` file in the same directory as this README; recommended for Docker builds and local clones. Example `secrets.json` contents:
+   ```json
+   {
+     "AWS_ACCESS_KEY_ID": "YOUR_AWS_KEY_ID",
+     "AWS_SECRET_ACCESS_KEY": "YOUR_AWS_SECRET_KEY",
+     "LOCAL_MODEL_PATH": "/path/to/your/local/models"
+   }
+   ```
+   
+LOCAL_MODEL_PATH is required. The two AWS access variables are required unless spacer is running on an AWS instance which has been set up with `aws configure`. The rest of the config variables are optional; see `CONFIGURABLE_VARS` in `config.py` for a full list.
+
+To debug your configuration, try opening a Python shell and run `from spacer import config`, then `config.check()`.
 
 #### Docker build
 The docker build is the preferred build and the one used in deployment.
 * Install docker on your system
 * Create `secrets.json` as detailed above.
 * Create folder `/path/to/your/local/models` for caching model files.
 * Build image: `docker build -t spacer:test .`
@@ -99,15 +111,15 @@
 `secrets.json` so that the container has the right permissions.
 
 The last step will run the default CMD command specified in the dockerfile 
 (unit-test with coverage). If you want to enter the docker container 
 run the same command but append `bash` in the end.
 
 #### Pip install
-* `pip install spacer`
+* `pip install pyspacer`
 * Set environmental variables.
 
 #### Local clone
 * Clone this repo
 * `pip install -r requirements.txt`
 
 If using Windows: turn Git's `autocrlf` setting off before your initial checkout. Otherwise, pickled classifiers in `spacer/tests/fixtures` will get checked out with `\r\n` newlines, and the pickle module will fail to load them, leading to test failures. However, autocrlf should be left on when adding any new non-pickle files.
```

### Comparing `pyspacer-0.4.0/pyspacer.egg-info/SOURCES.txt` & `pyspacer-0.4.1/pyspacer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/spacer/caffe_utils.py` & `pyspacer-0.4.1/spacer/caffe_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-"""
-This file contains a set of caffe utility functions copied into this repo for
-simplicity. Since support for Caffe will be deprecate,
-these are only lightly cleaned up from their original state.
-"""
-
-from copy import copy
-from functools import lru_cache
-from typing import List, Any, Tuple
-
-import caffe
-import hashlib
-import numpy as np
-
-from spacer import config
-
-
-class Transformer:
-    """
-    Transformer is a class for preprocessing and deprocessing images
-    according to the vgg16 pre-processing paradigm.
-    (scaling and mean subtraction.).
-    """
-
-    def __init__(self, mean: Tuple = (0, 0, 0)) -> None:
-        self.mean = np.array(mean, dtype=np.float32)
-        self.scale = 1.0
-
-    def preprocess(self, im: np.ndarray) -> np.ndarray:
-        """
-        preprocess() emulate the pre-processing occurring
-        in the vgg16 caffe prototxt.
-        :param im: numpy array.
-        :return: normalized numpy array.
-        """
-        im = np.float32(im)
-        im = im[:, :, ::-1]  # change to BGR
-        im -= self.mean
-        im *= self.scale
-        im = im.transpose((2, 0, 1))
-
-        return im
-
-    def deprocess(self, im: np.ndarray) -> np.ndarray:
-        """
-        inverse of preprocess().
-        :param im: normalized numpy array.
-        :return: original image.
-        """
-        im = im.transpose((1, 2, 0))
-        im /= self.scale
-        im += self.mean
-        im = im[:, :, ::-1]  # change to RGB
-
-        return np.uint8(im)
-
-
-def classify_from_imlist(im_list: List,
-                         net: Any,
-                         transformer: Transformer,
-                         batch_size: int,
-                         scorelayer: str = 'score',
-                         startlayer: str = 'conv1_1') -> List:
-    """
-    classify_from_imlist classifies a list of images and returns
-    estimated labels and scores.
-    Only support classification nets (not FCNs).
-    :param im_list: list of images to classify (each stored as a numpy array).
-    :param net: caffe net object.
-    :param transformer: transformer object as defined above.
-    :param batch_size: batch size for the net.
-    :param scorelayer: name of the score (the last conv) layer.
-    :param startlayer: name of first convolutional layer.
-    :return: features list.
-    """
-    with config.log_entry_and_exit('forward pass through net'):
-        scorelist = []
-        for b in range(len(im_list) // batch_size + 1):
-            for i in range(batch_size):
-                pos = b * batch_size + i
-                if pos < len(im_list):
-                    net.blobs['data'].data[i, :, :, :] = \
-                        transformer.preprocess(im_list[pos])
-            net.forward(start=startlayer)
-            scorelist.extend(list(copy(net.blobs[scorelayer].data).
-                                  astype(float)))
-
-        scorelist = scorelist[:len(im_list)]
-
-    return scorelist
-
-
-@lru_cache(maxsize=1)
-def load_net(modeldef_path: str,
-             modelweighs_path: str) -> Any:
-    """
-    load pretrained net.
-    :param modeldef_path: model path.
-    :param modelweighs_path: pretrained weights path.
-    :return: pretrained model.
-    """
-    # To verify that the correct weight is loaded
-    with config.log_entry_and_exit("load net, check SHA"):
-        with open(modelweighs_path, 'rb') as fp:
-            sha256 = hashlib.sha256(fp.read()).hexdigest()
-        assert sha256 == config.MODEL_WEIGHTS_SHA['vgg16']
-
-    return caffe.Net(modeldef_path, modelweighs_path, caffe.TEST)
-
-
-def classify_from_patchlist(patchlist: List,
-                            pyparams: dict,
-                            modeldef_path: str,
-                            modelweighs_path: str,
-                            scorelayer: str = 'score',
-                            startlayer: str = 'conv1_1') -> List:
-    """
-    extract features of a list of patches
-    :param patchlist: a list of patches (cropped images).
-    :param pyparams: a set of parameters.
-    :param modeldef_path: model path.
-    :param modelweighs_path: pretrained weights path.
-    :param scorelayer: name of the score (the last conv) layer.
-    :param startlayer: name of first convolutional layer.
-    :return: a list of features
-    """
-    # Setup caffe
-    caffe.set_mode_cpu()
-    net = load_net(modeldef_path, modelweighs_path)
-
-    # Classify
-    transformer = Transformer(pyparams['im_mean'])
-    scorelist = classify_from_imlist(
-        patchlist, net, transformer, pyparams['batch_size'],
-        scorelayer=scorelayer, startlayer=startlayer
-    )
-
-    return scorelist
+"""
+This file contains a set of caffe utility functions copied into this repo for
+simplicity. Since support for Caffe will be deprecate,
+these are only lightly cleaned up from their original state.
+"""
+
+from copy import copy
+from functools import lru_cache
+from typing import List, Any, Tuple
+
+import caffe
+import hashlib
+import numpy as np
+
+from spacer import config
+
+
+class Transformer:
+    """
+    Transformer is a class for preprocessing and deprocessing images
+    according to the vgg16 pre-processing paradigm.
+    (scaling and mean subtraction.).
+    """
+
+    def __init__(self, mean: Tuple = (0, 0, 0)) -> None:
+        self.mean = np.array(mean, dtype=np.float32)
+        self.scale = 1.0
+
+    def preprocess(self, im: np.ndarray) -> np.ndarray:
+        """
+        preprocess() emulate the pre-processing occurring
+        in the vgg16 caffe prototxt.
+        :param im: numpy array.
+        :return: normalized numpy array.
+        """
+        im = np.float32(im)
+        im = im[:, :, ::-1]  # change to BGR
+        im -= self.mean
+        im *= self.scale
+        im = im.transpose((2, 0, 1))
+
+        return im
+
+    def deprocess(self, im: np.ndarray) -> np.ndarray:
+        """
+        inverse of preprocess().
+        :param im: normalized numpy array.
+        :return: original image.
+        """
+        im = im.transpose((1, 2, 0))
+        im /= self.scale
+        im += self.mean
+        im = im[:, :, ::-1]  # change to RGB
+
+        return np.uint8(im)
+
+
+def classify_from_imlist(im_list: List,
+                         net: Any,
+                         transformer: Transformer,
+                         batch_size: int,
+                         scorelayer: str = 'score',
+                         startlayer: str = 'conv1_1') -> List:
+    """
+    classify_from_imlist classifies a list of images and returns
+    estimated labels and scores.
+    Only support classification nets (not FCNs).
+    :param im_list: list of images to classify (each stored as a numpy array).
+    :param net: caffe net object.
+    :param transformer: transformer object as defined above.
+    :param batch_size: batch size for the net.
+    :param scorelayer: name of the score (the last conv) layer.
+    :param startlayer: name of first convolutional layer.
+    :return: features list.
+    """
+    with config.log_entry_and_exit('forward pass through net'):
+        scorelist = []
+        for b in range(len(im_list) // batch_size + 1):
+            for i in range(batch_size):
+                pos = b * batch_size + i
+                if pos < len(im_list):
+                    net.blobs['data'].data[i, :, :, :] = \
+                        transformer.preprocess(im_list[pos])
+            net.forward(start=startlayer)
+            scorelist.extend(list(copy(net.blobs[scorelayer].data).
+                                  astype(float)))
+
+        scorelist = scorelist[:len(im_list)]
+
+    return scorelist
+
+
+@lru_cache(maxsize=1)
+def load_net(modeldef_path: str,
+             modelweighs_path: str) -> Any:
+    """
+    load pretrained net.
+    :param modeldef_path: model path.
+    :param modelweighs_path: pretrained weights path.
+    :return: pretrained model.
+    """
+    # To verify that the correct weight is loaded
+    with config.log_entry_and_exit("load net, check SHA"):
+        with open(modelweighs_path, 'rb') as fp:
+            sha256 = hashlib.sha256(fp.read()).hexdigest()
+        assert sha256 == config.MODEL_WEIGHTS_SHA['vgg16']
+
+    return caffe.Net(modeldef_path, modelweighs_path, caffe.TEST)
+
+
+def classify_from_patchlist(patchlist: List,
+                            pyparams: dict,
+                            modeldef_path: str,
+                            modelweighs_path: str,
+                            scorelayer: str = 'score',
+                            startlayer: str = 'conv1_1') -> List:
+    """
+    extract features of a list of patches
+    :param patchlist: a list of patches (cropped images).
+    :param pyparams: a set of parameters.
+    :param modeldef_path: model path.
+    :param modelweighs_path: pretrained weights path.
+    :param scorelayer: name of the score (the last conv) layer.
+    :param startlayer: name of first convolutional layer.
+    :return: a list of features
+    """
+    # Setup caffe
+    caffe.set_mode_cpu()
+    net = load_net(modeldef_path, modelweighs_path)
+
+    # Classify
+    transformer = Transformer(pyparams['im_mean'])
+    scorelist = classify_from_imlist(
+        patchlist, net, transformer, pyparams['batch_size'],
+        scorelayer=scorelayer, startlayer=startlayer
+    )
+
+    return scorelist
```

### Comparing `pyspacer-0.4.0/spacer/data_classes.py` & `pyspacer-0.4.1/spacer/data_classes.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-"""
-Defines data-classes for input and output types.
-Each data-class can serialize itself to a structure of JSON-friendly
-python-native data-structures such that it can be stored.
-"""
-import json
-from abc import ABC, abstractmethod
-from io import BytesIO
-from pprint import pformat
-from typing import Dict, List, Tuple, Set, Optional, Union
-
-import numpy as np
-
-from spacer.storage import storage_factory
-
-
-class DataClass(ABC):  # pragma: no cover
-
-    @classmethod
-    def load(cls, loc: 'DataLocation'):
-        storage = storage_factory(loc.storage_type, loc.bucket_name)
-        return cls.deserialize(json.loads(
-            storage.load(loc.key).getvalue().decode('utf-8')))
-
-    def store(self, loc: 'DataLocation'):
-        storage = storage_factory(loc.storage_type, loc.bucket_name)
-        storage.store(loc.key, BytesIO(
-            json.dumps(self.serialize()).encode('utf-8')))
-
-    @classmethod
-    @abstractmethod
-    def example(cls):
-        """
-        Instantiate an example member of the class.
-        Useful for testing, tutorials, etc.
-        """
-
-    @classmethod
-    def deserialize(cls, data: Dict) -> 'DataClass':
-        """
-        Initializes a class instance from input data.
-        Input should be a dictionary containing native python data structures.
-        """
-        return cls(**data)
-
-    def serialize(self) -> Dict:
-        """
-        Serialized the class content to native data-types, dicts, lists, etc,
-        such that it it compatible with json.dumps and json.loads.
-        """
-        return self.__dict__
-
-    def __repr__(self):
-        """ Give a (sort of) nicely formatted string repr. of class. """
-        return pformat(vars(self))
-
-    def __eq__(self, other):
-        """
-        This only works for the simple classes, more complicated
-        need to overwrite this method
-        """
-        sd = self.__dict__
-        od = other.__dict__
-        return sd.keys() == od.keys() and all([sd[key] == od[key]
-                                               for key in sd])
-
-
-class ImageLabels(DataClass):
-    """ Contains row, col, label information for an image. """
-
-    def __init__(self,
-                 # Data maps a feature key (or file path) to a List of
-                 # (row, col, label).
-                 data: Dict[str, List[Tuple[int, int, int]]]):
-        self.data = data
-
-    @classmethod
-    def example(cls):
-        return ImageLabels({
-            'img1.features': [(100, 200, 3), (101, 200, 2)],
-            'img2.features': [(100, 202, 3), (101, 200, 3)],
-            'img3.features': [(100, 202, 3), (101, 200, 3)],
-            'img4.features': [(100, 202, 3), (101, 200, 3)],
-        })
-
-    @classmethod
-    def deserialize(cls, data: Dict) -> 'ImageLabels':
-        """ Custom deserializer required to convert back to tuples. """
-        return ImageLabels(
-            data={key: [tuple(entry) for entry in value] for
-                  key, value in data['data'].items()})
-
-    @property
-    def image_keys(self):
-        return list(self.data.keys())
-
-    @property
-    def samples_per_image(self):
-        return len(next(iter(self.data.values())))
-
-    def unique_classes(self, key_list: List[str]) -> Set[int]:
-        """ Returns the set of all unique classes in the key_list subset. """
-        labels = set()
-        for im_key in key_list:
-            labels |= {label for (row, col, label) in self.data[im_key]}
-        return labels
-
-    def __len__(self):
-        return len(self.data)
-
-
-class PointFeatures(DataClass):
-    """ Contains row, col, feature-vector for a single point. """
-
-    def __init__(self,
-                 row: Optional[int],  # Row where feature was extracted
-                 col: Optional[int],  # Column where feature was extracted
-                 data: np.array,  # Feature vector with 32 bit precision.
-                 ):
-        self.row = row
-        self.col = col
-        self.data = np.array(data, dtype=float)
-
-    @classmethod
-    def example(cls):
-        return cls(
-            row=100,
-            col=100,
-            data=np.array([1.1, 1.3, 1.12], dtype=float)
-        )
-
-    def __eq__(self, other):
-        return self.row == other.row and self.col == other.col and \
-               np.allclose(self.data, other.data)
-
-
-class ImageFeatures(DataClass):
-    """ Contains row, col, feature-vectors for an image. """
-
-    def __init__(self,
-                 # List of features for all points in image
-                 point_features: List[PointFeatures],
-                 # Legacy feature did not store row and column locations.
-                 valid_rowcol: bool,
-                 # Dimensionality of the feature vectors.
-                 feature_dim: int,
-                 # Number of points in this image.
-                 npoints: int,
-                 ):
-
-        assert len(point_features) == npoints
-        assert len(point_features) > 0
-        assert len(point_features[0].data) == feature_dim
-
-        self.point_features = point_features
-        self.valid_rowcol = valid_rowcol
-        self.feature_dim = feature_dim
-        self.npoints = npoints
-
-        if self.valid_rowcol:
-            # Store a row_col hash for quick retrieval based on (row, col)
-            self._rchash = {(pf.row, pf.col): enum for
-                            enum, pf in enumerate(self.point_features)}
-
-    def __getitem__(self, rowcol: Tuple[int, int]) -> List[float]:
-        """ Returns features at (row, col) location. """
-        if not self.valid_rowcol:
-            raise ValueError('Method not supported for legacy features')
-        return self.point_features[self._rchash[rowcol]].data
-
-    def get_array(self, rowcol: Tuple[int, int]) -> np.array:
-        """
-        Similar to __getitem__ but returns a numpy array formatted
-        correctly for classification by a classifier of type
-        sklearn.calibration.CalibratedClassifierCV
-        """
-        return np.array(self[rowcol]).reshape(1, -1)
-
-    @classmethod
-    def example(cls):
-        pf1 = PointFeatures(row=100, col=100, data=[1.1, 1.3, 1.12])
-        pf2 = PointFeatures(row=120, col=110, data=[1.9, 1.3, 1.12])
-        return cls(
-            point_features=[pf1, pf2],
-            valid_rowcol=True,
-            feature_dim=len(pf1.data),
-            npoints=2
-        )
-
-    @classmethod
-    def deserialize(cls, data: Union[Dict, List]) -> 'ImageFeatures':
-
-        assert isinstance(data, List), \
-            "Deserialize only supported for legacy format"
-        # Legacy feature were stored as a list of list
-        # without row and column information.
-        assert len(data) > 0, "Empty features file."
-        return ImageFeatures(
-            point_features=[PointFeatures(row=None,
-                                          col=None,
-                                          data=entry) for entry in data],
-            valid_rowcol=False,
-            feature_dim=len(data[0]),
-            npoints=len(data)
-        )
-
-    def serialize(self):
-        raise NotImplementedError('Use .store() and .load() methods instead.')
-
-    def __eq__(self, other):
-        return all([a == b for a, b in zip(self.point_features,
-                                           other.point_features)]) and \
-               self.valid_rowcol == other.valid_rowcol and \
-               self.feature_dim == other.feature_dim and \
-               self.npoints == other.npoints
-
-    @classmethod
-    def make_random(cls,
-                    point_labels: List[int],
-                    feature_dim: int):
-        pfs = [PointFeatures(row=itt,
-                             col=itt,
-                             data=list(label + np.random.randn(feature_dim)))
-               for itt, label in enumerate(point_labels)]
-
-        return ImageFeatures(point_features=pfs,
-                             valid_rowcol=True,
-                             feature_dim=feature_dim,
-                             npoints=len(point_labels))
-
-    @classmethod
-    def load(cls, loc: 'DataLocation'):
-
-        storage = storage_factory(loc.storage_type, loc.bucket_name)
-        stream = storage.load(loc.key)
-        stream.seek(0)
-        try:
-            data = np.load(stream)
-            valid_rowcol = data['meta'][0]
-            if valid_rowcol:
-                return ImageFeatures(
-                    point_features=[PointFeatures(
-                        row=int(row),
-                        col=int(col),
-                        data=feat) for row, col, feat in zip(data['rows'],
-                                                             data['cols'],
-                                                             data['feat'])],
-                    valid_rowcol=bool(data['meta'][0]),
-                    npoints=data['meta'][1],
-                    feature_dim=data['meta'][2])
-            else:
-                return cls.deserialize(data['feat'].tolist())
-
-        except ValueError:
-            "We used to store these as a JSON file with a list of features."
-            data = json.loads(stream.getvalue().decode('utf-8'))
-            return cls.deserialize(data)
-
-    def store(self, loc: 'DataLocation'):
-        storage = storage_factory(loc.storage_type, loc.bucket_name)
-        if self.valid_rowcol:
-            rows = np.array([p.row for p in self.point_features], dtype=np.uint16)
-            cols = np.array([p.col for p in self.point_features], dtype=np.uint16)
-        else:
-            rows = np.array([])
-            cols = np.array([])
-        feat = np.array([p.data for p in self.point_features], dtype=float)
-        meta = np.array([self.valid_rowcol, self.npoints, self.feature_dim])
-        output = BytesIO()
-        np.savez_compressed(output, meta=meta, rows=rows, cols=cols, feat=feat)
-        output.seek(0)
-        storage.store(loc.key, output)
-
-
-class ValResults(DataClass):
-    """ Defines the validation results data class. Note that the gt and est
-    lists points to the index into the classes list."""
-
-    def __init__(self,
-                 scores: List[float],
-                 gt: List[int],  # Using singular for backwards compatibility.
-                 est: List[int],  # Using singular for backwards compatibility.
-                 classes: List[int]):
-
-        assert len(gt) == len(est)
-        assert len(gt) == len(scores)
-        assert max(gt) < len(classes)
-        assert max(est) < len(classes)
-        assert min(gt) >= 0
-        assert min(est) >= 0
-
-        self.scores = scores
-        self.gt = gt
-        self.est = est
-        self.classes = classes
-
-    @classmethod
-    def example(cls):
-        return cls(scores=[.9, .8, .7],
-                   gt=[0, 1, 0],
-                   est=[0, 1, 1],
-                   classes=[121, 1222])
-
-    @classmethod
-    def deserialize(cls, data: Dict) -> 'ValResults':
-        """ Redefined here to help the Typing module. """
-        return ValResults(**data)
+"""
+Defines data-classes for input and output types.
+Each data-class can serialize itself to a structure of JSON-friendly
+python-native data-structures such that it can be stored.
+"""
+import json
+from abc import ABC, abstractmethod
+from io import BytesIO
+from pprint import pformat
+from typing import Dict, List, Tuple, Set, Optional, Union
+
+import numpy as np
+
+from spacer.storage import storage_factory
+
+
+class DataClass(ABC):  # pragma: no cover
+
+    @classmethod
+    def load(cls, loc: 'DataLocation'):
+        storage = storage_factory(loc.storage_type, loc.bucket_name)
+        return cls.deserialize(json.loads(
+            storage.load(loc.key).getvalue().decode('utf-8')))
+
+    def store(self, loc: 'DataLocation'):
+        storage = storage_factory(loc.storage_type, loc.bucket_name)
+        storage.store(loc.key, BytesIO(
+            json.dumps(self.serialize()).encode('utf-8')))
+
+    @classmethod
+    @abstractmethod
+    def example(cls):
+        """
+        Instantiate an example member of the class.
+        Useful for testing, tutorials, etc.
+        """
+
+    @classmethod
+    def deserialize(cls, data: Dict) -> 'DataClass':
+        """
+        Initializes a class instance from input data.
+        Input should be a dictionary containing native python data structures.
+        """
+        return cls(**data)
+
+    def serialize(self) -> Dict:
+        """
+        Serialized the class content to native data-types, dicts, lists, etc,
+        such that it it compatible with json.dumps and json.loads.
+        """
+        return self.__dict__
+
+    def __repr__(self):
+        """ Give a (sort of) nicely formatted string repr. of class. """
+        return pformat(vars(self))
+
+    def __eq__(self, other):
+        """
+        This only works for the simple classes, more complicated
+        need to overwrite this method
+        """
+        sd = self.__dict__
+        od = other.__dict__
+        return sd.keys() == od.keys() and all([sd[key] == od[key]
+                                               for key in sd])
+
+
+class ImageLabels(DataClass):
+    """ Contains row, col, label information for an image. """
+
+    def __init__(self,
+                 # Data maps a feature key (or file path) to a List of
+                 # (row, col, label).
+                 data: Dict[str, List[Tuple[int, int, int]]]):
+        self.data = data
+
+    @classmethod
+    def example(cls):
+        return ImageLabels({
+            'img1.features': [(100, 200, 3), (101, 200, 2)],
+            'img2.features': [(100, 202, 3), (101, 200, 3)],
+            'img3.features': [(100, 202, 3), (101, 200, 3)],
+            'img4.features': [(100, 202, 3), (101, 200, 3)],
+        })
+
+    @classmethod
+    def deserialize(cls, data: Dict) -> 'ImageLabels':
+        """ Custom deserializer required to convert back to tuples. """
+        return ImageLabels(
+            data={key: [tuple(entry) for entry in value] for
+                  key, value in data['data'].items()})
+
+    @property
+    def image_keys(self):
+        return list(self.data.keys())
+
+    @property
+    def samples_per_image(self):
+        return len(next(iter(self.data.values())))
+
+    def unique_classes(self, key_list: List[str]) -> Set[int]:
+        """ Returns the set of all unique classes in the key_list subset. """
+        labels = set()
+        for im_key in key_list:
+            labels |= {label for (row, col, label) in self.data[im_key]}
+        return labels
+
+    def __len__(self):
+        return len(self.data)
+
+
+class PointFeatures(DataClass):
+    """ Contains row, col, feature-vector for a single point. """
+
+    def __init__(self,
+                 row: Optional[int],  # Row where feature was extracted
+                 col: Optional[int],  # Column where feature was extracted
+                 data: np.array,  # Feature vector with 32 bit precision.
+                 ):
+        self.row = row
+        self.col = col
+        self.data = np.array(data, dtype=float)
+
+    @classmethod
+    def example(cls):
+        return cls(
+            row=100,
+            col=100,
+            data=np.array([1.1, 1.3, 1.12], dtype=float)
+        )
+
+    def __eq__(self, other):
+        return self.row == other.row and self.col == other.col and \
+               np.allclose(self.data, other.data)
+
+
+class ImageFeatures(DataClass):
+    """ Contains row, col, feature-vectors for an image. """
+
+    def __init__(self,
+                 # List of features for all points in image
+                 point_features: List[PointFeatures],
+                 # Legacy feature did not store row and column locations.
+                 valid_rowcol: bool,
+                 # Dimensionality of the feature vectors.
+                 feature_dim: int,
+                 # Number of points in this image.
+                 npoints: int,
+                 ):
+
+        assert len(point_features) == npoints
+        assert len(point_features) > 0
+        assert len(point_features[0].data) == feature_dim
+
+        self.point_features = point_features
+        self.valid_rowcol = valid_rowcol
+        self.feature_dim = feature_dim
+        self.npoints = npoints
+
+        if self.valid_rowcol:
+            # Store a row_col hash for quick retrieval based on (row, col)
+            self._rchash = {(pf.row, pf.col): enum for
+                            enum, pf in enumerate(self.point_features)}
+
+    def __getitem__(self, rowcol: Tuple[int, int]) -> List[float]:
+        """ Returns features at (row, col) location. """
+        if not self.valid_rowcol:
+            raise ValueError('Method not supported for legacy features')
+        return self.point_features[self._rchash[rowcol]].data
+
+    def get_array(self, rowcol: Tuple[int, int]) -> np.array:
+        """
+        Similar to __getitem__ but returns a numpy array formatted
+        correctly for classification by a classifier of type
+        sklearn.calibration.CalibratedClassifierCV
+        """
+        return np.array(self[rowcol]).reshape(1, -1)
+
+    @classmethod
+    def example(cls):
+        pf1 = PointFeatures(row=100, col=100, data=[1.1, 1.3, 1.12])
+        pf2 = PointFeatures(row=120, col=110, data=[1.9, 1.3, 1.12])
+        return cls(
+            point_features=[pf1, pf2],
+            valid_rowcol=True,
+            feature_dim=len(pf1.data),
+            npoints=2
+        )
+
+    @classmethod
+    def deserialize(cls, data: Union[Dict, List]) -> 'ImageFeatures':
+
+        assert isinstance(data, List), \
+            "Deserialize only supported for legacy format"
+        # Legacy feature were stored as a list of list
+        # without row and column information.
+        assert len(data) > 0, "Empty features file."
+        return ImageFeatures(
+            point_features=[PointFeatures(row=None,
+                                          col=None,
+                                          data=entry) for entry in data],
+            valid_rowcol=False,
+            feature_dim=len(data[0]),
+            npoints=len(data)
+        )
+
+    def serialize(self):
+        raise NotImplementedError('Use .store() and .load() methods instead.')
+
+    def __eq__(self, other):
+        return all([a == b for a, b in zip(self.point_features,
+                                           other.point_features)]) and \
+               self.valid_rowcol == other.valid_rowcol and \
+               self.feature_dim == other.feature_dim and \
+               self.npoints == other.npoints
+
+    @classmethod
+    def make_random(cls,
+                    point_labels: List[int],
+                    feature_dim: int):
+        pfs = [PointFeatures(row=itt,
+                             col=itt,
+                             data=list(label + np.random.randn(feature_dim)))
+               for itt, label in enumerate(point_labels)]
+
+        return ImageFeatures(point_features=pfs,
+                             valid_rowcol=True,
+                             feature_dim=feature_dim,
+                             npoints=len(point_labels))
+
+    @classmethod
+    def load(cls, loc: 'DataLocation'):
+
+        storage = storage_factory(loc.storage_type, loc.bucket_name)
+        stream = storage.load(loc.key)
+        stream.seek(0)
+        try:
+            data = np.load(stream)
+            valid_rowcol = data['meta'][0]
+            if valid_rowcol:
+                return ImageFeatures(
+                    point_features=[PointFeatures(
+                        row=int(row),
+                        col=int(col),
+                        data=feat) for row, col, feat in zip(data['rows'],
+                                                             data['cols'],
+                                                             data['feat'])],
+                    valid_rowcol=bool(data['meta'][0]),
+                    npoints=data['meta'][1],
+                    feature_dim=data['meta'][2])
+            else:
+                return cls.deserialize(data['feat'].tolist())
+
+        except ValueError:
+            "We used to store these as a JSON file with a list of features."
+            data = json.loads(stream.getvalue().decode('utf-8'))
+            return cls.deserialize(data)
+
+    def store(self, loc: 'DataLocation'):
+        storage = storage_factory(loc.storage_type, loc.bucket_name)
+        if self.valid_rowcol:
+            rows = np.array([p.row for p in self.point_features], dtype=np.uint16)
+            cols = np.array([p.col for p in self.point_features], dtype=np.uint16)
+        else:
+            rows = np.array([])
+            cols = np.array([])
+        feat = np.array([p.data for p in self.point_features], dtype=float)
+        meta = np.array([self.valid_rowcol, self.npoints, self.feature_dim])
+        output = BytesIO()
+        np.savez_compressed(output, meta=meta, rows=rows, cols=cols, feat=feat)
+        output.seek(0)
+        storage.store(loc.key, output)
+
+
+class ValResults(DataClass):
+    """ Defines the validation results data class. Note that the gt and est
+    lists points to the index into the classes list."""
+
+    def __init__(self,
+                 scores: List[float],
+                 gt: List[int],  # Using singular for backwards compatibility.
+                 est: List[int],  # Using singular for backwards compatibility.
+                 classes: List[int]):
+
+        assert len(gt) == len(est)
+        assert len(gt) == len(scores)
+        assert max(gt) < len(classes)
+        assert max(est) < len(classes)
+        assert min(gt) >= 0
+        assert min(est) >= 0
+
+        self.scores = scores
+        self.gt = gt
+        self.est = est
+        self.classes = classes
+
+    @classmethod
+    def example(cls):
+        return cls(scores=[.9, .8, .7],
+                   gt=[0, 1, 0],
+                   est=[0, 1, 1],
+                   classes=[121, 1222])
+
+    @classmethod
+    def deserialize(cls, data: Dict) -> 'ValResults':
+        """ Redefined here to help the Typing module. """
+        return ValResults(**data)
```

### Comparing `pyspacer-0.4.0/spacer/extract_features.py` & `pyspacer-0.4.1/spacer/extract_features.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-"""
-Defines feature-extractor ABC; implementations; and factory.
-"""
-
-import abc
-import random
-import time
-from typing import List
-from typing import Tuple
-
-from PIL import Image
-
-from spacer import config
-from spacer.data_classes import PointFeatures, ImageFeatures
-from spacer.extract_features_utils import crop_patches
-from spacer.messages import ExtractFeaturesReturnMsg
-from spacer.storage import download_model
-from spacer.torch_utils import extract_feature
-
-
-class FeatureExtractor(abc.ABC):  # pragma: no cover
-
-    @abc.abstractmethod
-    def __call__(self,
-                 im: Image,
-                 rowcols: List[Tuple[int, int]]) \
-            -> Tuple[ImageFeatures, ExtractFeaturesReturnMsg]:
-        """ Runs the feature extraction """
-
-    @property
-    @abc.abstractmethod
-    def feature_dim(self) -> int:
-        """ Returns the feature dimension of extractor. """
-
-
-class DummyExtractor(FeatureExtractor):
-    """
-    This doesn't actually extract any features from the image,
-    it just returns dummy information.
-    Note that feature dimension is compatible with the VGG16CaffeExtractor.
-    """
-    def __init__(self, feature_dim):
-        self._feature_dim = feature_dim
-
-    def __call__(self, im, rowcols):
-        return ImageFeatures(
-            point_features=[PointFeatures(row=rc[0],
-                                          col=rc[1],
-                                          data=[random.random() for _ in
-                                                range(self.feature_dim)])
-                            for rc in rowcols],
-            valid_rowcol=True,
-            npoints=len(rowcols),
-            feature_dim=self.feature_dim
-        ), ExtractFeaturesReturnMsg.example()
-
-    @property
-    def feature_dim(self):
-        return self._feature_dim
-
-
-class VGG16CaffeExtractor(FeatureExtractor):
-
-    def __init__(self):
-
-        # Cache models and prototxt locally.
-        self.modeldef_path, _ = download_model(
-            'vgg16_coralnet_ver1.deploy.prototxt')
-        self.modelweighs_path, self.model_was_cached = download_model(
-            'vgg16_coralnet_ver1.caffemodel')
-
-    def __call__(self, im, rowcols):
-
-        # We should only reach this line if it is confirmed caffe is available
-        from spacer.caffe_utils import classify_from_patchlist
-
-        start_time = time.time()
-
-        # Set caffe parameters
-        caffe_params = {'im_mean': [128, 128, 128],
-                        'scaling_method': 'scale',
-                        'crop_size': 224,
-                        'batch_size': 10}
-
-        # Crop patches
-        with config.log_entry_and_exit('cropping of {} patches'.format(
-                len(rowcols))):
-            patch_list = crop_patches(im, rowcols, caffe_params['crop_size'])
-        del im
-
-        # Extract features
-        feats = classify_from_patchlist(patch_list,
-                                        caffe_params,
-                                        self.modeldef_path,
-                                        self.modelweighs_path,
-                                        scorelayer='fc7')
-
-        return \
-            ImageFeatures(
-                point_features=[PointFeatures(row=rc[0],
-                                              col=rc[1],
-                                              data=ft.tolist())
-                                for rc, ft in zip(rowcols, feats)],
-                valid_rowcol=True,
-                feature_dim=len(feats[0]),
-                npoints=len(feats)
-            ), ExtractFeaturesReturnMsg(
-                model_was_cached=self.model_was_cached,
-                runtime=time.time() - start_time
-            )
-
-    @property
-    def feature_dim(self):
-        return 4096
-
-
-class EfficientNetExtractor(FeatureExtractor):
-
-    def __init__(self):
-
-        # Cache models locally.
-        self.modelweighs_path, self.model_was_cached = download_model(
-           'efficientnet_b0_ver1.pt')
-
-    def __call__(self, im, rowcols):
-
-        start_time = time.time()
-
-        # Set torch parameters
-        torch_params = {'model_type': 'efficientnet',
-                        'model_name': 'efficientnet-b0',
-                        'weights_path': self.modelweighs_path,
-                        'num_class': 1275,
-                        'crop_size': 224,
-                        'batch_size': 10}
-
-        # Crop patches
-        with config.log_entry_and_exit('cropping %s patches' % len(rowcols)):
-            patch_list = crop_patches(im, rowcols, torch_params['crop_size'])
-        del im
-
-        # Extract features
-        feats = extract_feature(patch_list, torch_params)
-
-        return ImageFeatures(
-            point_features=[PointFeatures(row=rc[0], col=rc[1], data=ft)
-                            for rc, ft in zip(rowcols, feats)],
-            valid_rowcol=True, feature_dim=len(feats[0]), npoints=len(feats)
-        ), ExtractFeaturesReturnMsg(
-            model_was_cached=self.model_was_cached,
-            runtime=time.time() - start_time
-        )
-
-    @property
-    def feature_dim(self):
-        return 1280
-
-
-def feature_extractor_factory(modelname,
-                              dummy_featuredim=4096) -> FeatureExtractor:
-
-    assert modelname in config.FEATURE_EXTRACTOR_NAMES, \
-        "Model name {} not registered".format(modelname)
-
-    if modelname == 'vgg16_coralnet_ver1':
-        assert config.HAS_CAFFE, \
-            "Need Caffe installed to instantiate {}".format(modelname)
-        with config.log_entry_and_exit("initializing VGG16CaffeExtractor"):
-            extractor = VGG16CaffeExtractor()
-    if modelname == 'efficientnet_b0_ver1':
-        with config.log_entry_and_exit("initializing EfficientNetExtractor"):
-            extractor = EfficientNetExtractor()
-    if modelname == 'dummy':
-        with config.log_entry_and_exit("initializing DummyExtractor"):
-            extractor = DummyExtractor(dummy_featuredim)
-    return extractor
+"""
+Defines feature-extractor ABC; implementations; and factory.
+"""
+
+import abc
+import random
+import time
+from typing import List
+from typing import Tuple
+
+from PIL import Image
+
+from spacer import config
+from spacer.data_classes import PointFeatures, ImageFeatures
+from spacer.extract_features_utils import crop_patches
+from spacer.messages import ExtractFeaturesReturnMsg
+from spacer.storage import download_model
+from spacer.torch_utils import extract_feature
+
+
+class FeatureExtractor(abc.ABC):  # pragma: no cover
+
+    @abc.abstractmethod
+    def __call__(self,
+                 im: Image,
+                 rowcols: List[Tuple[int, int]]) \
+            -> Tuple[ImageFeatures, ExtractFeaturesReturnMsg]:
+        """ Runs the feature extraction """
+
+    @property
+    @abc.abstractmethod
+    def feature_dim(self) -> int:
+        """ Returns the feature dimension of extractor. """
+
+
+class DummyExtractor(FeatureExtractor):
+    """
+    This doesn't actually extract any features from the image,
+    it just returns dummy information.
+    Note that feature dimension is compatible with the VGG16CaffeExtractor.
+    """
+    def __init__(self, feature_dim):
+        self._feature_dim = feature_dim
+
+    def __call__(self, im, rowcols):
+        return ImageFeatures(
+            point_features=[PointFeatures(row=rc[0],
+                                          col=rc[1],
+                                          data=[random.random() for _ in
+                                                range(self.feature_dim)])
+                            for rc in rowcols],
+            valid_rowcol=True,
+            npoints=len(rowcols),
+            feature_dim=self.feature_dim
+        ), ExtractFeaturesReturnMsg.example()
+
+    @property
+    def feature_dim(self):
+        return self._feature_dim
+
+
+class VGG16CaffeExtractor(FeatureExtractor):
+
+    def __init__(self):
+
+        # Cache models and prototxt locally.
+        self.modeldef_path, _ = download_model(
+            'vgg16_coralnet_ver1.deploy.prototxt')
+        self.modelweighs_path, self.model_was_cached = download_model(
+            'vgg16_coralnet_ver1.caffemodel')
+
+    def __call__(self, im, rowcols):
+
+        # We should only reach this line if it is confirmed caffe is available
+        from spacer.caffe_utils import classify_from_patchlist
+
+        start_time = time.time()
+
+        # Set caffe parameters
+        caffe_params = {'im_mean': [128, 128, 128],
+                        'scaling_method': 'scale',
+                        'crop_size': 224,
+                        'batch_size': 10}
+
+        # Crop patches
+        with config.log_entry_and_exit('cropping of {} patches'.format(
+                len(rowcols))):
+            patch_list = crop_patches(im, rowcols, caffe_params['crop_size'])
+        del im
+
+        # Extract features
+        feats = classify_from_patchlist(patch_list,
+                                        caffe_params,
+                                        self.modeldef_path,
+                                        self.modelweighs_path,
+                                        scorelayer='fc7')
+
+        return \
+            ImageFeatures(
+                point_features=[PointFeatures(row=rc[0],
+                                              col=rc[1],
+                                              data=ft.tolist())
+                                for rc, ft in zip(rowcols, feats)],
+                valid_rowcol=True,
+                feature_dim=len(feats[0]),
+                npoints=len(feats)
+            ), ExtractFeaturesReturnMsg(
+                model_was_cached=self.model_was_cached,
+                runtime=time.time() - start_time
+            )
+
+    @property
+    def feature_dim(self):
+        return 4096
+
+
+class EfficientNetExtractor(FeatureExtractor):
+
+    def __init__(self):
+
+        # Cache models locally.
+        self.modelweighs_path, self.model_was_cached = download_model(
+           'efficientnet_b0_ver1.pt')
+
+    def __call__(self, im, rowcols):
+
+        start_time = time.time()
+
+        # Set torch parameters
+        torch_params = {'model_type': 'efficientnet',
+                        'model_name': 'efficientnet-b0',
+                        'weights_path': self.modelweighs_path,
+                        'num_class': 1275,
+                        'crop_size': 224,
+                        'batch_size': 10}
+
+        # Crop patches
+        with config.log_entry_and_exit('cropping %s patches' % len(rowcols)):
+            patch_list = crop_patches(im, rowcols, torch_params['crop_size'])
+        del im
+
+        # Extract features
+        feats = extract_feature(patch_list, torch_params)
+
+        return ImageFeatures(
+            point_features=[PointFeatures(row=rc[0], col=rc[1], data=ft)
+                            for rc, ft in zip(rowcols, feats)],
+            valid_rowcol=True, feature_dim=len(feats[0]), npoints=len(feats)
+        ), ExtractFeaturesReturnMsg(
+            model_was_cached=self.model_was_cached,
+            runtime=time.time() - start_time
+        )
+
+    @property
+    def feature_dim(self):
+        return 1280
+
+
+def feature_extractor_factory(modelname,
+                              dummy_featuredim=4096) -> FeatureExtractor:
+
+    assert modelname in config.FEATURE_EXTRACTOR_NAMES, \
+        "Model name {} not registered".format(modelname)
+
+    if modelname == 'vgg16_coralnet_ver1':
+        assert config.HAS_CAFFE, \
+            "Need Caffe installed to instantiate {}".format(modelname)
+        with config.log_entry_and_exit("initializing VGG16CaffeExtractor"):
+            extractor = VGG16CaffeExtractor()
+    if modelname == 'efficientnet_b0_ver1':
+        with config.log_entry_and_exit("initializing EfficientNetExtractor"):
+            extractor = EfficientNetExtractor()
+    if modelname == 'dummy':
+        with config.log_entry_and_exit("initializing DummyExtractor"):
+            extractor = DummyExtractor(dummy_featuredim)
+    return extractor
```

### Comparing `pyspacer-0.4.0/spacer/extract_features_utils.py` & `pyspacer-0.4.1/spacer/extract_features_utils.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from typing import List, Tuple
-
-import numpy as np
-from PIL import Image
-
-
-def gray2rgb(im: np.ndarray) -> np.ndarray:
-    """
-    Convert gray image to RGB image
-    :param im: gray image to be converted
-    :return: RGB image
-    """
-    w, h = im.shape
-    ret = np.empty((w, h, 3), dtype=np.uint8)
-    ret[:, :, 0] = im
-    ret[:, :, 1] = im
-    ret[:, :, 2] = im
-
-    return ret
-
-
-def crop_patches(im: Image,
-                 rowcols: List[Tuple[int, int]],
-                 crop_size: int) -> List[np.ndarray]:
-    """
-    Crop patches from an image
-    :param im: image for cropping
-    :param rowcols: [(row1, col1), (row2, col2), ...]
-    :param crop_size: patch size
-    :return: patch list
-    """
-    im = np.array(im)
-
-    if len(im.shape) == 2 or im.shape[2] == 1:
-        im = gray2rgb(im)
-    im = im[:, :, :3]  # only keep the first three color channels
-
-    pad = crop_size
-    im = np.pad(im, ((pad, pad), (pad, pad), (0, 0)), mode='reflect')
-
-    patches = [crop_simple(im, (row + pad, col + pad), crop_size)
-               for row, col in rowcols]
-
-    return patches
-
-
-def crop_simple(im: np.ndarray,
-                center: Tuple[int, int],
-                crop_size: int) -> np.ndarray:
-    """
-    Crops an image around the given center
-    :param im: image to be cropped
-    :param center: offset (row, col)
-    :param crop_size: cropping size
-    :return: cropped image in numpy array
-    """
-    upper = int(center[0] - crop_size / 2)
-    left = int(center[1] - crop_size / 2)
-
-    return im[upper: upper + crop_size, left: left + crop_size, :]
+from typing import List, Tuple
+
+import numpy as np
+from PIL import Image
+
+
+def gray2rgb(im: np.ndarray) -> np.ndarray:
+    """
+    Convert gray image to RGB image
+    :param im: gray image to be converted
+    :return: RGB image
+    """
+    w, h = im.shape
+    ret = np.empty((w, h, 3), dtype=np.uint8)
+    ret[:, :, 0] = im
+    ret[:, :, 1] = im
+    ret[:, :, 2] = im
+
+    return ret
+
+
+def crop_patches(im: Image,
+                 rowcols: List[Tuple[int, int]],
+                 crop_size: int) -> List[np.ndarray]:
+    """
+    Crop patches from an image
+    :param im: image for cropping
+    :param rowcols: [(row1, col1), (row2, col2), ...]
+    :param crop_size: patch size
+    :return: patch list
+    """
+    im = np.array(im)
+
+    if len(im.shape) == 2 or im.shape[2] == 1:
+        im = gray2rgb(im)
+    im = im[:, :, :3]  # only keep the first three color channels
+
+    pad = crop_size
+    im = np.pad(im, ((pad, pad), (pad, pad), (0, 0)), mode='reflect')
+
+    patches = [crop_simple(im, (row + pad, col + pad), crop_size)
+               for row, col in rowcols]
+
+    return patches
+
+
+def crop_simple(im: np.ndarray,
+                center: Tuple[int, int],
+                crop_size: int) -> np.ndarray:
+    """
+    Crops an image around the given center
+    :param im: image to be cropped
+    :param center: offset (row, col)
+    :param crop_size: cropping size
+    :return: cropped image in numpy array
+    """
+    upper = int(center[0] - crop_size / 2)
+    left = int(center[1] - crop_size / 2)
+
+    return im[upper: upper + crop_size, left: left + crop_size, :]
```

### Comparing `pyspacer-0.4.0/spacer/mailman.py` & `pyspacer-0.4.1/spacer/mailman.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-"""
-Defines the highest-level method for task handling through AWS Batch.
-"""
-
-import json
-import logging
-import os
-
-import fire
-
-from spacer import config
-from spacer.messages import JobMsg, DataLocation
-from spacer.tasks import process_job
-
-
-# Configure a simple logger that works with AWS CloudWatch.
-if len(logging.getLogger().handlers) > 0:
-    # The Lambda environment pre-configures a handler logging to stderr.
-    # If a handler is already configured,
-    # `.basicConfig` does not execute. Thus we set the level directly.
-    logging.getLogger().setLevel(logging.INFO)
-else:
-    logging.basicConfig(level=logging.INFO, format='%(asctime)s %(message)s')
-
-
-def env_job(): # pragma: no cover
-    """
-    Runs a job defined in environment variables.
-    This is set up to be used in AWS Batch, using a job definition with
-    a command such as: ["python3","spacer/mailman.py","env_job"]
-
-    Expects JOB_MSG_LOC to contain the json-serialized DataLocation of the
-    job msg.
-    Expects RES_MSG_LOC to contain the json-serialized DataLocation of the
-    job return msg.
-    """
-
-    job_msg_loc = os.getenv('JOB_MSG_LOC')
-    if job_msg_loc is None:
-        raise ValueError('JOB_MSG_LOC env. variable not set. '
-                         'Can not process job.')
-
-    logging.info(" Received job for ENV {}.".format(job_msg_loc))
-
-    with config.log_entry_and_exit('job message location deserialization'):
-        job_msg_loc = DataLocation.deserialize(json.loads(job_msg_loc))
-
-    with config.log_entry_and_exit('job message initialization'):
-        job_msg = JobMsg.load(job_msg_loc)
-
-    try:
-        job_return_msg = process_job(job_msg)
-        job_return_msg_dict = job_return_msg.serialize()
-    except Exception as e:
-        # Handle deserialization errors directly in mailman.
-        # All other errors are handled in "handle_message" function.
-        job_return_msg_dict = {
-            'original_job': job_msg.serialize(),
-            'ok': False,
-            'results': None,
-            'error_message': 'Error deserializing message: ' + repr(e)
-        }
-
-    # Return
-    out_msg_loc = os.getenv('RES_MSG_LOC')
-    if out_msg_loc is not None:
-        with config.log_entry_and_exit('out message location deserialization'):
-            out_msg_loc = DataLocation.deserialize(json.loads(out_msg_loc))
-
-        with config.log_entry_and_exit('writing res to {}'.format(
-                out_msg_loc.key)):
-            s3 = config.get_s3_conn()
-            s3.Bucket(out_msg_loc.bucket_name).put_object(
-                Key=out_msg_loc.key,
-                Body=bytes(json.dumps(job_return_msg_dict).encode('UTF-8')))
-    return 1
-
-
-if __name__ == '__main__':
-    fire.Fire()  # pragma: no cover
+"""
+Defines the highest-level method for task handling through AWS Batch.
+"""
+
+import json
+import logging
+import os
+
+import fire
+
+from spacer import config
+from spacer.messages import JobMsg, DataLocation
+from spacer.tasks import process_job
+
+
+# Configure a simple logger that works with AWS CloudWatch.
+if len(logging.getLogger().handlers) > 0:
+    # The Lambda environment pre-configures a handler logging to stderr.
+    # If a handler is already configured,
+    # `.basicConfig` does not execute. Thus we set the level directly.
+    logging.getLogger().setLevel(logging.INFO)
+else:
+    logging.basicConfig(level=logging.INFO, format='%(asctime)s %(message)s')
+
+
+def env_job(): # pragma: no cover
+    """
+    Runs a job defined in environment variables.
+    This is set up to be used in AWS Batch, using a job definition with
+    a command such as: ["python3","spacer/mailman.py","env_job"]
+
+    Expects JOB_MSG_LOC to contain the json-serialized DataLocation of the
+    job msg.
+    Expects RES_MSG_LOC to contain the json-serialized DataLocation of the
+    job return msg.
+    """
+
+    job_msg_loc = os.getenv('JOB_MSG_LOC')
+    if job_msg_loc is None:
+        raise ValueError('JOB_MSG_LOC env. variable not set. '
+                         'Can not process job.')
+
+    logging.info(" Received job for ENV {}.".format(job_msg_loc))
+
+    with config.log_entry_and_exit('job message location deserialization'):
+        job_msg_loc = DataLocation.deserialize(json.loads(job_msg_loc))
+
+    with config.log_entry_and_exit('job message initialization'):
+        job_msg = JobMsg.load(job_msg_loc)
+
+    try:
+        job_return_msg = process_job(job_msg)
+        job_return_msg_dict = job_return_msg.serialize()
+    except Exception as e:
+        # Handle deserialization errors directly in mailman.
+        # All other errors are handled in "handle_message" function.
+        job_return_msg_dict = {
+            'original_job': job_msg.serialize(),
+            'ok': False,
+            'results': None,
+            'error_message': 'Error deserializing message: ' + repr(e)
+        }
+
+    # Return
+    out_msg_loc = os.getenv('RES_MSG_LOC')
+    if out_msg_loc is not None:
+        with config.log_entry_and_exit('out message location deserialization'):
+            out_msg_loc = DataLocation.deserialize(json.loads(out_msg_loc))
+
+        with config.log_entry_and_exit('writing res to {}'.format(
+                out_msg_loc.key)):
+            s3 = config.get_s3_conn()
+            s3.Bucket(out_msg_loc.bucket_name).put_object(
+                Key=out_msg_loc.key,
+                Body=bytes(json.dumps(job_return_msg_dict).encode('UTF-8')))
+    return 1
+
+
+if __name__ == '__main__':
+    fire.Fire()  # pragma: no cover
```

### Comparing `pyspacer-0.4.0/spacer/models/effcientnet_utils.py` & `pyspacer-0.4.1/spacer/models/effcientnet_utils.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/spacer/models/efficientnet.py` & `pyspacer-0.4.1/spacer/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/spacer/task_utils.py` & `pyspacer-0.4.1/spacer/task_utils.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/spacer/tasks.py` & `pyspacer-0.4.1/spacer/tasks.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/spacer/torch_utils.py` & `pyspacer-0.4.1/spacer/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/spacer/train_classifier.py` & `pyspacer-0.4.1/spacer/train_classifier.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.4.0/spacer/train_utils.py` & `pyspacer-0.4.1/spacer/train_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-"""
-Utility methods for training classifiers.
-"""
-
-import logging
-import random
-import string
-from typing import Tuple, List
-
-import numpy as np
-from sklearn.calibration import CalibratedClassifierCV
-from sklearn.linear_model import SGDClassifier
-from sklearn.neural_network import MLPClassifier
-
-from spacer import config
-from spacer.data_classes import ImageLabels, ImageFeatures
-from spacer.messages import DataLocation
-
-
-def train(labels: ImageLabels,
-          feature_loc: DataLocation,
-          nbr_epochs: int,
-          clf_type: str) -> Tuple[CalibratedClassifierCV, List[float]]:
-
-    if len(labels) < config.MIN_TRAINIMAGES:
-        raise ValueError('Not enough training samples.')
-
-    # Calculate max nbr images to keep in memory (for 5000 samples total).
-    max_imgs_in_memory = 5000 // labels.samples_per_image
-
-    # Make train and ref split.
-    # Reference set is here a hold-out part of the train-data portion.
-    # Purpose of reference set is to
-    # 1) know accuracy per epoch
-    # 2) calibrate classifier output scores.
-    # We call it "reference" to disambiguate from the validation set.
-    ref_set = labels.image_keys[::10]
-    np.random.shuffle(ref_set)
-    ref_set = ref_set[:max_imgs_in_memory]  # Enforce memory limit.
-    train_set = list(set(labels.image_keys) - set(ref_set))
-    logging.info("Trainset: {}, valset: {} images".
-                 format(len(train_set), len(ref_set)))
-
-    # Figure out # images per batch and batches per epoch.
-    images_per_batch, batches_per_epoch = \
-        calc_batch_size(max_imgs_in_memory, len(train_set))
-    logging.info("Using {} images per mini-batch and {} mini-batches per "
-                 "epoch".format(images_per_batch, batches_per_epoch))
-
-    # Identify classes common to both train and val.
-    # This will be our labelset for the training.
-    trainclasses = labels.unique_classes(train_set)
-    refclasses = labels.unique_classes(ref_set)
-    classes = list(trainclasses.intersection(refclasses))
-    logging.info("Trainset: {}, valset: {}, common: {} labels".format(
-        len(trainclasses), len(refclasses), len(classes)))
-    if len(classes) == 1:
-        raise ValueError('Not enough classes to do training (only 1)')
-
-    # Load reference data (must hold in memory for the calibration)
-    with config.log_entry_and_exit("loading of reference data"):
-        refx, refy = load_batch_data(labels, ref_set, classes, feature_loc)
-
-    # Initialize classifier and ref set accuracy list
-    with config.log_entry_and_exit("training using " + clf_type):
-        if clf_type == 'MLP':
-            if len(train_set) * labels.samples_per_image >= 50000:
-                hls, lr = (200, 100), 1e-4
-            else:
-                hls, lr = (100,), 1e-3
-            clf = MLPClassifier(hidden_layer_sizes=hls, learning_rate_init=lr)
-        else:
-            clf = SGDClassifier(loss='log_loss', average=True, random_state=0)
-        ref_acc = []
-        for epoch in range(nbr_epochs):
-            np.random.shuffle(train_set)
-            mini_batches = chunkify(train_set, batches_per_epoch)
-            for mb in mini_batches:
-                x, y = load_batch_data(labels, mb, classes, feature_loc)
-                clf.partial_fit(x, y, classes=classes)
-            ref_acc.append(calc_acc(refy, clf.predict(refx)))
-            logging.info("Epoch {}, acc: {}".format(epoch, ref_acc[-1]))
-
-    with config.log_entry_and_exit("calibration"):
-        clf_calibrated = CalibratedClassifierCV(clf, cv="prefit")
-        clf_calibrated.fit(refx, refy)
-
-    return clf_calibrated, ref_acc
-
-
-def evaluate_classifier(clf: CalibratedClassifierCV,
-                        labels: ImageLabels,
-                        classes: List[int],
-                        feature_loc: DataLocation) -> Tuple[List, List, List]:
-    """ Evaluates classifier on data """
-    scores, gts, ests = [], [], []
-    for imkey in labels.image_keys:
-        x, y = load_image_data(labels, imkey, classes, feature_loc)
-        if len(x) > 0:
-            scores.extend(clf.predict_proba(x).max(axis=1).tolist())
-            ests.extend(clf.predict(x))
-            gts.extend(y)
-
-    if len(gts) == 0:
-        raise ValueError('Not enough data in validation set.')
-
-    return gts, ests, scores
-
-
-def chunkify(lst: List,
-             nbr_chunks: int) -> List:
-    return [lst[i::nbr_chunks] for i in range(nbr_chunks)]
-
-
-def calc_batch_size(max_imgs_in_memory: int,
-                    train_set_size: int) -> Tuple[int, int]:
-    images_per_batch = min(max_imgs_in_memory, train_set_size)
-    batches_per_epoch = int(np.ceil(train_set_size / images_per_batch))
-    return images_per_batch, batches_per_epoch
-
-
-def load_image_data(labels: ImageLabels,
-                    imkey: str,
-                    classes: List[int],
-                    feature_loc: DataLocation) \
-        -> Tuple[List[List[float]], List[int]]:
-    """
-    Loads features and labels for image and matches feature with labels.
-    """
-
-    # Load features for this image.
-    feature_loc.key = imkey  # Set the relevant key here.
-    image_features = ImageFeatures.load(feature_loc)
-
-    # Load row, col, labels for this image.
-    image_labels = labels.data[imkey]
-
-    # Sanity check
-    if image_features.valid_rowcol:
-        # With new data structure just check that the sets of row, col
-        # given by the labels is available in the features.
-        rc_features_set = set([(pf.row, pf.col) for pf in
-                               image_features.point_features])
-        rc_labels_set = set([(row, col) for (row, col, _) in image_labels])
-        assert rc_labels_set.issubset(rc_features_set)
-    else:
-        # With legacy data structure check that length is the same.
-        assert len(image_labels) == len(image_features.point_features), \
-            "number of extracted features doesn't match the number of labels!"
-
-    x, y = [], []
-    if image_features.valid_rowcol:
-        for row, col, label in image_labels:
-            if label not in classes:
-                # Remove samples for which the label is not in classes.
-                continue
-            x.append(image_features[(row, col)])
-            y.append(label)
-
-    else:
-        # For legacy features, we didn't store the row, col information.
-        # Instead rely on ordering.
-        for (_, _, label), point_feature in zip(image_labels,
-                                                image_features.point_features):
-            if label not in classes:
-                continue
-            x.append(point_feature.data)
-            y.append(label)
-
-    return x, y
-
-
-def load_batch_data(labels: ImageLabels,
-                    imkeylist: List[str],
-                    classes: List[int],
-                    feature_loc: DataLocation) \
-        -> Tuple[List[List[float]], List[int]]:
-    """ Loads features and labels and match them together. """
-    x, y = [], []
-    for imkey in imkeylist:
-        x_, y_ = load_image_data(labels, imkey, classes, feature_loc)
-        x.extend(x_)
-        y.extend(y_)
-    return x, y
-
-
-def calc_acc(gt: List[int], est: List[int]) -> float:
-    """
-    Calculate the accuracy of (agreement between) two integer valued list.
-    """
-    if len(gt) == 0 or len(est) == 0:
-        raise TypeError('Inputs can not be empty')
-
-    if not len(gt) == len(est):
-        raise ValueError('Input gt and est must have the same length')
-
-    for g in gt:
-        if not int(g) == g:
-            raise TypeError('Input gt must be an array of ints')
-
-    for e in est:
-        if not int(e) == e:
-            raise TypeError('Input est must be an array of ints')
-
-    return float(sum([(g == e) for (g, e) in zip(gt, est)])) / len(gt)
-
-
-def make_random_data(im_count: int,
-                     class_list: List[int],
-                     points_per_image: int,
-                     feature_dim: int,
-                     feature_loc: DataLocation) -> ImageLabels:
-    """
-    Utility method for testing that generates an ImageLabels instance
-    complete with stored ImageFeatures.
-    """
-    labels = ImageLabels(data={})
-    for _ in range(im_count):
-
-        # Generate random features (using labels to draw from a Gaussian).
-        point_labels = np.random.choice(class_list, points_per_image).tolist()
-
-        # Make sure all classes are present
-        point_labels[:len(class_list)] = class_list
-        feats = ImageFeatures.make_random(point_labels, feature_dim)
-
-        # Generate a random string as imkey.
-        imkey = ''.join(random.choice(string.ascii_uppercase + string.digits)
-                        for _ in range(20))
-
-        # Store
-        feature_loc.key = imkey
-        feats.store(feature_loc)
-        labels.data[imkey] = [
-            (pf.row, pf.col, pl) for pf, pl in
-            zip(feats.point_features, point_labels)
-        ]
-    return labels
+"""
+Utility methods for training classifiers.
+"""
+
+import logging
+import random
+import string
+from typing import Tuple, List
+
+import numpy as np
+from sklearn.calibration import CalibratedClassifierCV
+from sklearn.linear_model import SGDClassifier
+from sklearn.neural_network import MLPClassifier
+
+from spacer import config
+from spacer.data_classes import ImageLabels, ImageFeatures
+from spacer.messages import DataLocation
+
+
+def train(labels: ImageLabels,
+          feature_loc: DataLocation,
+          nbr_epochs: int,
+          clf_type: str) -> Tuple[CalibratedClassifierCV, List[float]]:
+
+    if len(labels) < config.MIN_TRAINIMAGES:
+        raise ValueError('Not enough training samples.')
+
+    # Calculate max nbr images to keep in memory (for 5000 samples total).
+    max_imgs_in_memory = 5000 // labels.samples_per_image
+
+    # Make train and ref split.
+    # Reference set is here a hold-out part of the train-data portion.
+    # Purpose of reference set is to
+    # 1) know accuracy per epoch
+    # 2) calibrate classifier output scores.
+    # We call it "reference" to disambiguate from the validation set.
+    ref_set = labels.image_keys[::10]
+    np.random.shuffle(ref_set)
+    ref_set = ref_set[:max_imgs_in_memory]  # Enforce memory limit.
+    train_set = list(set(labels.image_keys) - set(ref_set))
+    logging.info("Trainset: {}, valset: {} images".
+                 format(len(train_set), len(ref_set)))
+
+    # Figure out # images per batch and batches per epoch.
+    images_per_batch, batches_per_epoch = \
+        calc_batch_size(max_imgs_in_memory, len(train_set))
+    logging.info("Using {} images per mini-batch and {} mini-batches per "
+                 "epoch".format(images_per_batch, batches_per_epoch))
+
+    # Identify classes common to both train and val.
+    # This will be our labelset for the training.
+    trainclasses = labels.unique_classes(train_set)
+    refclasses = labels.unique_classes(ref_set)
+    classes = list(trainclasses.intersection(refclasses))
+    logging.info("Trainset: {}, valset: {}, common: {} labels".format(
+        len(trainclasses), len(refclasses), len(classes)))
+    if len(classes) == 1:
+        raise ValueError('Not enough classes to do training (only 1)')
+
+    # Load reference data (must hold in memory for the calibration)
+    with config.log_entry_and_exit("loading of reference data"):
+        refx, refy = load_batch_data(labels, ref_set, classes, feature_loc)
+
+    # Initialize classifier and ref set accuracy list
+    with config.log_entry_and_exit("training using " + clf_type):
+        if clf_type == 'MLP':
+            if len(train_set) * labels.samples_per_image >= 50000:
+                hls, lr = (200, 100), 1e-4
+            else:
+                hls, lr = (100,), 1e-3
+            clf = MLPClassifier(hidden_layer_sizes=hls, learning_rate_init=lr)
+        else:
+            clf = SGDClassifier(loss='log_loss', average=True, random_state=0)
+        ref_acc = []
+        for epoch in range(nbr_epochs):
+            np.random.shuffle(train_set)
+            mini_batches = chunkify(train_set, batches_per_epoch)
+            for mb in mini_batches:
+                x, y = load_batch_data(labels, mb, classes, feature_loc)
+                clf.partial_fit(x, y, classes=classes)
+            ref_acc.append(calc_acc(refy, clf.predict(refx)))
+            logging.info("Epoch {}, acc: {}".format(epoch, ref_acc[-1]))
+
+    with config.log_entry_and_exit("calibration"):
+        clf_calibrated = CalibratedClassifierCV(clf, cv="prefit")
+        clf_calibrated.fit(refx, refy)
+
+    return clf_calibrated, ref_acc
+
+
+def evaluate_classifier(clf: CalibratedClassifierCV,
+                        labels: ImageLabels,
+                        classes: List[int],
+                        feature_loc: DataLocation) -> Tuple[List, List, List]:
+    """ Evaluates classifier on data """
+    scores, gts, ests = [], [], []
+    for imkey in labels.image_keys:
+        x, y = load_image_data(labels, imkey, classes, feature_loc)
+        if len(x) > 0:
+            scores.extend(clf.predict_proba(x).max(axis=1).tolist())
+            ests.extend(clf.predict(x))
+            gts.extend(y)
+
+    if len(gts) == 0:
+        raise ValueError('Not enough data in validation set.')
+
+    return gts, ests, scores
+
+
+def chunkify(lst: List,
+             nbr_chunks: int) -> List:
+    return [lst[i::nbr_chunks] for i in range(nbr_chunks)]
+
+
+def calc_batch_size(max_imgs_in_memory: int,
+                    train_set_size: int) -> Tuple[int, int]:
+    images_per_batch = min(max_imgs_in_memory, train_set_size)
+    batches_per_epoch = int(np.ceil(train_set_size / images_per_batch))
+    return images_per_batch, batches_per_epoch
+
+
+def load_image_data(labels: ImageLabels,
+                    imkey: str,
+                    classes: List[int],
+                    feature_loc: DataLocation) \
+        -> Tuple[List[List[float]], List[int]]:
+    """
+    Loads features and labels for image and matches feature with labels.
+    """
+
+    # Load features for this image.
+    feature_loc.key = imkey  # Set the relevant key here.
+    image_features = ImageFeatures.load(feature_loc)
+
+    # Load row, col, labels for this image.
+    image_labels = labels.data[imkey]
+
+    # Sanity check
+    if image_features.valid_rowcol:
+        # With new data structure just check that the sets of row, col
+        # given by the labels is available in the features.
+        rc_features_set = set([(pf.row, pf.col) for pf in
+                               image_features.point_features])
+        rc_labels_set = set([(row, col) for (row, col, _) in image_labels])
+        assert rc_labels_set.issubset(rc_features_set)
+    else:
+        # With legacy data structure check that length is the same.
+        assert len(image_labels) == len(image_features.point_features), \
+            "number of extracted features doesn't match the number of labels!"
+
+    x, y = [], []
+    if image_features.valid_rowcol:
+        for row, col, label in image_labels:
+            if label not in classes:
+                # Remove samples for which the label is not in classes.
+                continue
+            x.append(image_features[(row, col)])
+            y.append(label)
+
+    else:
+        # For legacy features, we didn't store the row, col information.
+        # Instead rely on ordering.
+        for (_, _, label), point_feature in zip(image_labels,
+                                                image_features.point_features):
+            if label not in classes:
+                continue
+            x.append(point_feature.data)
+            y.append(label)
+
+    return x, y
+
+
+def load_batch_data(labels: ImageLabels,
+                    imkeylist: List[str],
+                    classes: List[int],
+                    feature_loc: DataLocation) \
+        -> Tuple[List[List[float]], List[int]]:
+    """ Loads features and labels and match them together. """
+    x, y = [], []
+    for imkey in imkeylist:
+        x_, y_ = load_image_data(labels, imkey, classes, feature_loc)
+        x.extend(x_)
+        y.extend(y_)
+    return x, y
+
+
+def calc_acc(gt: List[int], est: List[int]) -> float:
+    """
+    Calculate the accuracy of (agreement between) two integer valued list.
+    """
+    if len(gt) == 0 or len(est) == 0:
+        raise TypeError('Inputs can not be empty')
+
+    if not len(gt) == len(est):
+        raise ValueError('Input gt and est must have the same length')
+
+    for g in gt:
+        if not int(g) == g:
+            raise TypeError('Input gt must be an array of ints')
+
+    for e in est:
+        if not int(e) == e:
+            raise TypeError('Input est must be an array of ints')
+
+    return float(sum([(g == e) for (g, e) in zip(gt, est)])) / len(gt)
+
+
+def make_random_data(im_count: int,
+                     class_list: List[int],
+                     points_per_image: int,
+                     feature_dim: int,
+                     feature_loc: DataLocation) -> ImageLabels:
+    """
+    Utility method for testing that generates an ImageLabels instance
+    complete with stored ImageFeatures.
+    """
+    labels = ImageLabels(data={})
+    for _ in range(im_count):
+
+        # Generate random features (using labels to draw from a Gaussian).
+        point_labels = np.random.choice(class_list, points_per_image).tolist()
+
+        # Make sure all classes are present
+        point_labels[:len(class_list)] = class_list
+        feats = ImageFeatures.make_random(point_labels, feature_dim)
+
+        # Generate a random string as imkey.
+        imkey = ''.join(random.choice(string.ascii_uppercase + string.digits)
+                        for _ in range(20))
+
+        # Store
+        feature_loc.key = imkey
+        feats.store(feature_loc)
+        labels.data[imkey] = [
+            (pf.row, pf.col, pl) for pf, pl in
+            zip(feats.point_features, point_labels)
+        ]
+    return labels
```

