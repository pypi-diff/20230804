# Comparing `tmp/cds-python-sdk-0.13.tar.gz` & `tmp/cds-python-sdk-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cds-python-sdk-0.13.tar", last modified: Wed Jun 14 06:07:16 2023, max compression
+gzip compressed data, was "cds-python-sdk-0.14.tar", last modified: Fri Aug  4 05:06:42 2023, max compression
```

## Comparing `cds-python-sdk-0.13.tar` & `cds-python-sdk-0.14.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.676268 cds-python-sdk-0.13/
--rw-rw-rw-   0        0        0    10313 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/LICENSE
--rw-rw-rw-   0        0        0      221 2023-06-14 06:07:16.674252 cds-python-sdk-0.13/PKG-INFO
--rw-rw-rw-   0        0        0     4807 2023-06-14 05:59:06.000000 cds-python-sdk-0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.632641 cds-python-sdk-0.13/capitalonline/
--rw-rw-rw-   0        0        0       17 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.640258 cds-python-sdk-0.13/capitalonline/common/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/__init__.py
--rw-rw-rw-   0        0        0    18497 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/abstract_client.py
--rw-rw-rw-   0        0        0     1127 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/client.py
--rw-rw-rw-   0        0        0     1761 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/credential.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.643611 cds-python-sdk-0.13/capitalonline/common/exception/
--rw-rw-rw-   0        0        0      122 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/exception/__init__.py
--rw-rw-rw-   0        0        0      706 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/exception/cds_sdk_exception.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.646518 cds-python-sdk-0.13/capitalonline/common/http/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/http/__init__.py
--rw-rw-rw-   0        0        0     5211 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/http/request.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.649683 cds-python-sdk-0.13/capitalonline/common/profile/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/profile/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/profile/client_profile.py
--rw-rw-rw-   0        0        0     1300 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/profile/http_profile.py
--rw-rw-rw-   0        0        0     2782 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/sign.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.654652 cds-python-sdk-0.13/capitalonline/haproxy/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/__init__.py
--rw-rw-rw-   0        0        0    12947 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/client.py
--rw-rw-rw-   0        0        0     9175 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/client_test.py
--rw-rw-rw-   0        0        0     7938 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/models.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.662485 cds-python-sdk-0.13/capitalonline/instance/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/instance/__init__.py
--rw-rw-rw-   0        0        0    12078 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/instance/client.py
--rw-rw-rw-   0        0        0    11860 2023-06-14 05:59:06.000000 cds-python-sdk-0.13/capitalonline/instance/client_test.py
--rw-rw-rw-   0        0        0     6247 2023-06-14 03:18:20.000000 cds-python-sdk-0.13/capitalonline/instance/models.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.666920 cds-python-sdk-0.13/capitalonline/vdc/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/__init__.py
--rw-rw-rw-   0        0        0     5518 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/client.py
--rw-rw-rw-   0        0        0     6335 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/client_test.py
--rw-rw-rw-   0        0        0     6908 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/model.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.672855 cds-python-sdk-0.13/cds_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      221 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:07:16.676268 cds-python-sdk-0.13/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-06-14 06:07:11.000000 cds-python-sdk-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.438434 cds-python-sdk-0.14/
+-rw-rw-rw-   0        0        0    10313 2023-05-23 06:32:39.000000 cds-python-sdk-0.14/LICENSE
+-rw-rw-rw-   0        0        0      171 2023-08-04 05:06:42.437432 cds-python-sdk-0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     4807 2023-08-04 04:35:16.000000 cds-python-sdk-0.14/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.395182 cds-python-sdk-0.14/capitalonline/
+-rw-rw-rw-   0        0        0       17 2023-05-10 08:44:21.000000 cds-python-sdk-0.14/capitalonline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.403760 cds-python-sdk-0.14/capitalonline/common/
+-rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.14/capitalonline/common/__init__.py
+-rw-rw-rw-   0        0        0    18497 2023-05-29 07:01:55.000000 cds-python-sdk-0.14/capitalonline/common/abstract_client.py
+-rw-rw-rw-   0        0        0     1127 2023-05-11 07:27:33.000000 cds-python-sdk-0.14/capitalonline/common/client.py
+-rw-rw-rw-   0        0        0     1761 2023-05-29 07:01:55.000000 cds-python-sdk-0.14/capitalonline/common/credential.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.406829 cds-python-sdk-0.14/capitalonline/common/exception/
+-rw-rw-rw-   0        0        0      122 2023-05-29 07:01:55.000000 cds-python-sdk-0.14/capitalonline/common/exception/__init__.py
+-rw-rw-rw-   0        0        0      706 2023-05-10 08:44:21.000000 cds-python-sdk-0.14/capitalonline/common/exception/cds_sdk_exception.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.408829 cds-python-sdk-0.14/capitalonline/common/http/
+-rw-rw-rw-   0        0        0        0 2023-05-10 08:44:21.000000 cds-python-sdk-0.14/capitalonline/common/http/__init__.py
+-rw-rw-rw-   0        0        0     5211 2023-05-10 08:44:21.000000 cds-python-sdk-0.14/capitalonline/common/http/request.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.411894 cds-python-sdk-0.14/capitalonline/common/profile/
+-rw-rw-rw-   0        0        0        0 2023-05-10 08:44:21.000000 cds-python-sdk-0.14/capitalonline/common/profile/__init__.py
+-rw-rw-rw-   0        0        0     1048 2023-05-29 07:01:55.000000 cds-python-sdk-0.14/capitalonline/common/profile/client_profile.py
+-rw-rw-rw-   0        0        0     1300 2023-05-30 06:44:49.000000 cds-python-sdk-0.14/capitalonline/common/profile/http_profile.py
+-rw-rw-rw-   0        0        0     2782 2023-05-10 08:44:21.000000 cds-python-sdk-0.14/capitalonline/common/sign.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.416616 cds-python-sdk-0.14/capitalonline/haproxy/
+-rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.14/capitalonline/haproxy/__init__.py
+-rw-rw-rw-   0        0        0    12947 2023-05-30 06:43:43.000000 cds-python-sdk-0.14/capitalonline/haproxy/client.py
+-rw-rw-rw-   0        0        0     9175 2023-05-31 08:59:17.000000 cds-python-sdk-0.14/capitalonline/haproxy/client_test.py
+-rw-rw-rw-   0        0        0     7938 2023-05-29 07:01:55.000000 cds-python-sdk-0.14/capitalonline/haproxy/models.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.423997 cds-python-sdk-0.14/capitalonline/instance/
+-rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.14/capitalonline/instance/__init__.py
+-rw-rw-rw-   0        0        0    12730 2023-08-04 04:35:16.000000 cds-python-sdk-0.14/capitalonline/instance/client.py
+-rw-rw-rw-   0        0        0    12871 2023-08-04 04:35:16.000000 cds-python-sdk-0.14/capitalonline/instance/client_test.py
+-rw-rw-rw-   0        0        0     6439 2023-08-04 04:35:16.000000 cds-python-sdk-0.14/capitalonline/instance/models.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.427996 cds-python-sdk-0.14/capitalonline/vdc/
+-rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.14/capitalonline/vdc/__init__.py
+-rw-rw-rw-   0        0        0     5518 2023-05-30 06:43:43.000000 cds-python-sdk-0.14/capitalonline/vdc/client.py
+-rw-rw-rw-   0        0        0     6335 2023-05-31 08:48:52.000000 cds-python-sdk-0.14/capitalonline/vdc/client_test.py
+-rw-rw-rw-   0        0        0     6908 2023-05-29 07:01:55.000000 cds-python-sdk-0.14/capitalonline/vdc/model.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.432275 cds-python-sdk-0.14/cds_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-08-04 05:06:42.000000 cds-python-sdk-0.14/cds_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-08-04 05:06:42.000000 cds-python-sdk-0.14/cds_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 05:06:42.000000 cds-python-sdk-0.14/cds_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-04 05:06:42.000000 cds-python-sdk-0.14/cds_python_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 05:06:42.438434 cds-python-sdk-0.14/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-08-04 05:06:24.000000 cds-python-sdk-0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:06:42.435528 cds-python-sdk-0.14/tests/
+-rw-rw-rw-   0        0        0      676 2023-05-10 08:44:21.000000 cds-python-sdk-0.14/tests/test.py
```

### Comparing `cds-python-sdk-0.13/LICENSE` & `cds-python-sdk-0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/README.md` & `cds-python-sdk-0.14/README.md`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/abstract_client.py` & `cds-python-sdk-0.14/capitalonline/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/client.py` & `cds-python-sdk-0.14/capitalonline/common/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/credential.py` & `cds-python-sdk-0.14/capitalonline/common/credential.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/exception/cds_sdk_exception.py` & `cds-python-sdk-0.14/capitalonline/common/exception/cds_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/http/request.py` & `cds-python-sdk-0.14/capitalonline/common/http/request.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/profile/client_profile.py` & `cds-python-sdk-0.14/capitalonline/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/profile/http_profile.py` & `cds-python-sdk-0.14/capitalonline/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/common/sign.py` & `cds-python-sdk-0.14/capitalonline/common/sign.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/haproxy/client.py` & `cds-python-sdk-0.14/capitalonline/haproxy/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/haproxy/client_test.py` & `cds-python-sdk-0.14/capitalonline/haproxy/client_test.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/haproxy/models.py` & `cds-python-sdk-0.14/capitalonline/haproxy/models.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/instance/client.py` & `cds-python-sdk-0.14/capitalonline/instance/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from capitalonline.common.client import Client
 from .models import AddInstanceRequest, DescribeInstanceRequest, DeleteInstanceRequest, ModifyInstanceNameRequest, \
     ModifyInstanceSpecRequest, CreateDiskRequest, ResizeDiskRequest, DeleteDiskRequest, ModifyIpRequest, \
     ExtendSystemDiskRequest, ResetInstancesPasswordRequest, ResetImageRequest, ModifyInstanceChargeTypeRequest, \
     StopInstanceRequest, RebootInstanceRequest, StartInstanceRequest, StartInstancesRequest, StopInstancesRequest, \
-    RebootInstancesRequest
+    RebootInstancesRequest,DescribeInstanceMonitorRequest
 import json
 from capitalonline.common.profile import http_profile, client_profile
 from capitalonline.common.credential import Credential
 
 ApiVersion = "2019-08-08"
 SERVICE = 'ccs'
 
@@ -156,14 +156,20 @@
 
 def NewRebootInstancesRequest():
     request = RebootInstancesRequest(service=SERVICE, version=ApiVersion,
                                      action='RebootInstances')
     return request
 
 
+def NewDescribeInstanceMonitorRequest():
+    request = DescribeInstanceMonitorRequest(service=SERVICE, version=ApiVersion,
+                                             action='DescribeInstanceMonitor')
+    return request
+
+
 class InstanceClient(Client):
     def __init__(self, service, version, credential, region, profile=None):
         super().__init__(service=service, version=version, credential=credential,
                          region=region, profile=profile)
 
     def CreateInstance(self, request):
         """
@@ -345,7 +351,17 @@
             if request is None:
                 request = NewRebootInstancesRequest()
             self.profile.httpProfile.reqMethod = 'GET'
             response = self.call(request.action, request.to_params())
             return json.loads(response), ''
         except Exception as e:
             return '', e
+
+    def DescribeInstanceMonitor(self, request):
+        try:
+            if request is None:
+                request = NewDescribeInstanceMonitorRequest()
+            self.profile.httpProfile.reqMethod = 'POST'
+            response = self.call(request.action, request.to_params())
+            return json.loads(response), ''
+        except Exception as e:
+            return '', e
```

### Comparing `cds-python-sdk-0.13/capitalonline/instance/client_test.py` & `cds-python-sdk-0.14/capitalonline/instance/client_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from capitalonline.instance.client import NewClient, NewAddInstanceRequest, NewModifyInstanceNameRequest, \
     NewDescribeInstanceRequest, NewDeleteInstanceRequest, NewModifyInstanceSpecRequest, NewCreateDiskRequest, \
     NewResizeDiskRequest, NewDeleteDiskRequest, NewStartInstancesRequest, NewStopInstancesRequest, \
     NewRebootInstancesRequest, NewModifyIpRequest, NewExtendSystemDiskRequest, NewResetInstancesPasswordRequest, \
-    NewResetImageRequest, NewModifyInstanceChargeTypeRequest
+    NewResetImageRequest, NewModifyInstanceChargeTypeRequest, NewDescribeInstanceMonitorRequest
 from capitalonline.instance.models import DataDisk, PrivateIp, SystemDisk, OrderedIP
 
 ak = ''
 sk = ''
 Beijing_region = 'Beijing'
 
 
@@ -334,14 +334,37 @@
     request = NewModifyInstanceChargeTypeRequest()
     request.InstanceId = "instance id"                                           #Instance id must be set.
     request.InstanceChargeType = 'PrePaid'                                       #Charge type must be set
     response, err = client.ModifyInstanceChargeType(request)
     print(f"Modify Instance Charge Type response:{response}, err:{err}")
 
 
+def TestClient_DescribeInstanceMonitor():
+    """
+    get instance monitor.
+    :return:
+    """
+
+    client, err = NewClient(ak, sk, Beijing_region)
+    if err:
+        print(f'err:{err}')
+        return
+    request = NewDescribeInstanceMonitorRequest()
+    request.InstanceId = "instance_id"  # Instance id must be set.
+    request.MetricName = 'CPUUtilization'  # MetricName  must be set
+    request.Period = 60  # Period  must be set  60/900
+    request.StartTime = '2023-08-01 16:15:00'  # StartTime must be set
+    request.EndTime = '2023-08-01 16:25:00'  # EndTime must be set
+    request.InterfaceId = ''  # This parameter is required if you need to query network information
+    request.DiskId = ''  # This parameter is required if you need to query disk information
+    response, err = client.DescribeInstanceMonitor(request)
+    print(f"Describe  Instance Monitor response:{response}, err:{err}")
+
+
+
 if __name__ == '__main__':
     # TestClient_CreateInstance()
     # TestClient_DescribeInstance()
     # TestClient_ModifyInstanceName()
     # TestClient_ModifyInstanceSpec()
     # TestClient_CreateDisk()
     # TestClient_ResizeDisk()
@@ -350,12 +373,12 @@
     # TestClient_StartInstances()
     # TestClient_RebootInstances()
     # TestClient_DeleteInstance()
     # TestClient_ModifyIpAddress()
     # TestClient_ExtendSystemDisk()
     # TestClient_ResetInstancesPassword()
     # TestClient_ResetImage()
-    TestClient_ModifyInstanceChargeType()
-
+    # TestClient_ModifyInstanceChargeType()
+    TestClient_DescribeInstanceMonitor()
```

### Comparing `cds-python-sdk-0.13/capitalonline/instance/models.py` & `cds-python-sdk-0.14/capitalonline/instance/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -283,7 +283,17 @@
 
 class StopInstancesRequest(BaseRequest):
     InstanceIds: str
 
 
 class RebootInstancesRequest(BaseRequest):
     InstanceIds: str
+
+
+class DescribeInstanceMonitorRequest(BaseRequest):
+    InstanceId: str
+    MetricName: str
+    Period: int
+    StartTime: str
+    EndTime: str
+    InterfaceId: str
+    DiskId: str
```

### Comparing `cds-python-sdk-0.13/capitalonline/vdc/client.py` & `cds-python-sdk-0.14/capitalonline/vdc/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/vdc/client_test.py` & `cds-python-sdk-0.14/capitalonline/vdc/client_test.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/capitalonline/vdc/model.py` & `cds-python-sdk-0.14/capitalonline/vdc/model.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.13/cds_python_sdk.egg-info/SOURCES.txt` & `cds-python-sdk-0.14/cds_python_sdk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 capitalonline/vdc/__init__.py
 capitalonline/vdc/client.py
 capitalonline/vdc/client_test.py
 capitalonline/vdc/model.py
 cds_python_sdk.egg-info/PKG-INFO
 cds_python_sdk.egg-info/SOURCES.txt
 cds_python_sdk.egg-info/dependency_links.txt
-cds_python_sdk.egg-info/top_level.txt
+cds_python_sdk.egg-info/top_level.txt
+tests/test.py
```

