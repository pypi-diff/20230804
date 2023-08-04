# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.949.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.949.tar", last modified: Thu Aug  3 00:19:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.950.tar", last modified: Fri Aug  4 00:19:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.949.tar` & `tencentcloud-sdk-python-autoscaling-3.0.950.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19989 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60726 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)   392015 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      583 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-08-03 00:19:26.000000 tencentcloud-sdk-python-autoscaling-3.0.949/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19989 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60726 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)   391964 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-08-04 00:19:31.000000 tencentcloud-sdk-python-autoscaling-3.0.950/README.rst
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.950/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-autoscaling',
-    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Autoscaling SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud/autoscaling/v20180419/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10215,15 +10215,15 @@
 <br><li> ANY，存在任何一个实例类型（InstanceType）可用则通过校验，否则校验报错。
 
 实例类型不可用的常见原因包括该实例类型售罄、对应云盘售罄等。
 如果 InstanceTypes 中一款机型不存在或者已下线，则无论 InstanceTypesCheckPolicy 采用何种取值，都会校验报错。
         :type InstanceTypesCheckPolicy: str
         :param _InternetAccessible: 公网带宽相关信息设置。若不指定该参数，则默认公网带宽为0Mbps。
         :type InternetAccessible: :class:`tencentcloud.autoscaling.v20180419.models.InternetAccessible`
-        :param _LoginSettings: 实例登录设置。通过该参数可以设置实例的登录方式密码、密钥或保持镜像的原始登录设置。默认情况下会随机生成密码，并以站内信方式知会到用户。
+        :param _LoginSettings: 该参数已失效，请勿使用。升级启动配置接口无法修改或覆盖 LoginSettings 参数，升级后 LoginSettings 不会发生变化。
         :type LoginSettings: :class:`tencentcloud.autoscaling.v20180419.models.LoginSettings`
         :param _ProjectId: 实例所属项目ID。不填为默认项目。
         :type ProjectId: int
         :param _SecurityGroupIds: 实例所属安全组。该参数可以通过调用 [DescribeSecurityGroups](https://cloud.tencent.com/document/api/215/15808) 的返回值中的`SecurityGroupId`字段来获取。若不指定该参数，则默认不绑定安全组。
         :type SecurityGroupIds: list of str
         :param _SystemDisk: 实例系统盘配置信息。若不指定该参数，则按照系统默认值进行分配。
         :type SystemDisk: :class:`tencentcloud.autoscaling.v20180419.models.SystemDisk`
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.950/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.950/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.949/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.950/README.rst`

 * *Files identical despite different names*

