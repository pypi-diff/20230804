# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.949.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.949.tar", last modified: Thu Aug  3 00:24:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.950.tar", last modified: Fri Aug  4 00:25:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.949.tar` & `tencentcloud-sdk-python-dlc-3.0.950.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud_sdk_python_dlc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82705 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   562911 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:24:52.000000 tencentcloud-sdk-python-dlc-3.0.949/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82705 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   562911 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/README.rst
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/setup.py` & `tencentcloud-sdk-python-dlc-3.0.950/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-dlc',
-    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Dlc SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.949'
+__version__ = '3.0.950'
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.950/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.949/README.rst` & `tencentcloud-sdk-python-dlc-3.0.950/README.rst`

 * *Files identical despite different names*

