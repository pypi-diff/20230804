# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.949.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.949.tar", last modified: Thu Aug  3 00:22:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.950.tar", last modified: Fri Aug  4 00:23:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.949.tar` & `tencentcloud-sdk-python-clb-3.0.950.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    90730 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)   507968 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud_sdk_python_clb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-03 00:22:52.000000 tencentcloud-sdk-python-clb-3.0.949/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    90730 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)   508027 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-clb-3.0.949/setup.py` & `tencentcloud-sdk-python-clb-3.0.950/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-clb',
-    install_requires=["tencentcloud-sdk-python-common==3.0.949"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Clb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.949/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1883,15 +1883,15 @@
         :param _SlaveZoneId: 仅适用于公网负载均衡。设置跨可用区容灾时的备可用区ID，例如 100001 或 ap-guangzhou-1
 注：备可用区是主可用区故障后，需要承载流量的可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主/备可用区的列表。
         :type SlaveZoneId: str
         :param _ZoneId: 仅适用于公网负载均衡。可用区ID，指定可用区以创建负载均衡实例。如：ap-guangzhou-1。
         :type ZoneId: str
         :param _InternetAccessible: 仅适用于公网负载均衡。负载均衡的网络计费模式。
         :type InternetAccessible: :class:`tencentcloud.clb.v20180317.models.InternetAccessible`
-        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213)  接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
+        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213)  接口查询一个地域所支持的Isp。如果指定运营商，则网络计费模式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
         :type VipIsp: str
         :param _Vip: 指定Vip申请负载均衡。
         :type Vip: str
         :param _Tags: 购买负载均衡同时，给负载均衡打上标签。
         :type Tags: list of TagInfo
         :param _ExclusiveCluster: 独占集群信息。
         :type ExclusiveCluster: :class:`tencentcloud.clb.v20180317.models.ExclusiveCluster`
@@ -3178,15 +3178,15 @@
         :param _ProjectId: 负载均衡实例所属的项目 ID，可以通过 [DescribeProject](https://cloud.tencent.com/document/api/651/78725) 接口获取。不填此参数则视为默认项目。
         :type ProjectId: int
         :param _AddressIPVersion: 仅适用于公网负载均衡。IP版本，可取值：IPV4、IPV6、IPv6FullChain，不区分大小写，默认值 IPV4。说明：取值为IPV6表示为IPV6 NAT64版本；取值为IPv6FullChain，表示为IPv6版本。
         :type AddressIPVersion: str
         :param _Number: 创建负载均衡的个数，默认值 1。
         :type Number: int
         :param _MasterZoneId: 仅适用于公网负载均衡。设置跨可用区容灾时的主可用区ID，例如 100001 或 ap-guangzhou-1
-注：主可用区是需要承载流量的可用区，备可用区默认不承载流量，主可用区不可用时才使用备可用区，平台将为您自动选择最佳备可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主可用区的列表。
+注：主可用区是需要承载流量的可用区，备可用区默认不承载流量，主可用区不可用时才使用备可用区。目前仅广州、上海、南京、北京、中国香港、首尔地域的 IPv4 版本的 CLB 支持主备可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主可用区的列表。
         :type MasterZoneId: str
         :param _ZoneId: 仅适用于公网负载均衡。可用区ID，指定可用区以创建负载均衡实例。如：ap-guangzhou-1。
         :type ZoneId: str
         :param _InternetAccessible: 仅对内网属性的性能容量型实例和公网属性的所有实例生效。
         :type InternetAccessible: :class:`tencentcloud.clb.v20180317.models.InternetAccessible`
         :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213)  接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
         :type VipIsp: str
@@ -8610,15 +8610,15 @@
         :param _HttpCode: 健康检查状态码（仅适用于HTTP/HTTPS转发规则、TCP监听器的HTTP健康检查方式）。可选值：1~31，默认 31。
 1 表示探测后返回值 1xx 代表健康，2 表示返回 2xx 代表健康，4 表示返回 3xx 代表健康，8 表示返回 4xx 代表健康，16 表示返回 5xx 代表健康。若希望多种返回码都可代表健康，则将相应的值相加。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCode: int
         :param _HttpCheckPath: 健康检查路径（仅适用于HTTP/HTTPS转发规则、TCP监听器的HTTP健康检查方式）。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCheckPath: str
-        :param _HttpCheckDomain: 健康检查域名（仅适用于HTTP/HTTPS监听器和TCP监听器的HTTP健康检查方式。针对TCP监听器，当使用HTTP健康检查方式时，建议该参数配置为必填项）。
+        :param _HttpCheckDomain: 健康检查域名（仅适用于HTTP/HTTPS监听器和TCP监听器的HTTP健康检查方式。针对TCP监听器，当使用HTTP健康检查方式时，该参数为必填项）。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCheckDomain: str
         :param _HttpCheckMethod: 健康检查方法（仅适用于HTTP/HTTPS转发规则、TCP监听器的HTTP健康检查方式），默认值：HEAD，可选值HEAD或GET。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCheckMethod: str
         :param _CheckPort: 自定义探测相关参数。健康检查端口，默认为后端服务的端口，除非您希望指定特定端口，否则建议留空。（仅适用于TCP/UDP监听器）。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -13953,15 +13953,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _SourceLocationId: 源转发规则ID
         :type SourceLocationId: str
-        :param _TargetLocationId: 重定向至的目标转发规则ID
+        :param _TargetLocationId: 重定向目标转发规则的ID
         :type TargetLocationId: str
         :param _RewriteCode: 重定向状态码，可取值301,302,307
         :type RewriteCode: int
         :param _TakeUrl: 重定向是否携带匹配的url，配置RewriteCode时必填
         :type TakeUrl: bool
         :param _SourceDomain: 源转发的域名，必须是SourceLocationId对应的域名，配置RewriteCode时必填
         :type SourceDomain: str
```

### Comparing `tencentcloud-sdk-python-clb-3.0.949/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.949/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.950/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.949/README.rst` & `tencentcloud-sdk-python-clb-3.0.950/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.949/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.949
+Version: 3.0.950
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

