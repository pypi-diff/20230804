# Comparing `tmp/Jakit-0.3.tar.gz` & `tmp/Jakit-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jakit-0.3.tar", last modified: Thu Aug  3 14:29:07 2023, max compression
+gzip compressed data, was "Jakit-0.4.tar", last modified: Fri Aug  4 10:38:31 2023, max compression
```

## Comparing `Jakit-0.3.tar` & `Jakit-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 14:29:07.263231 Jakit-0.3/
-drwxrwxrwx   0        0        0        0 2023-08-03 14:29:07.220229 Jakit-0.3/Jakit/
--rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.3/Jakit/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-08-03 13:26:48.000000 Jakit-0.3/Jakit/jakit_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:29:07.259230 Jakit-0.3/Jakit.egg-info/
--rw-rw-rw-   0        0        0      523 2023-08-03 14:29:06.000000 Jakit-0.3/Jakit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-08-03 14:29:07.000000 Jakit-0.3/Jakit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 14:29:06.000000 Jakit-0.3/Jakit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-03 14:29:06.000000 Jakit-0.3/Jakit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.3/LICENSE
--rw-rw-rw-   0        0        0      523 2023-08-03 14:29:07.262229 Jakit-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 14:29:07.263231 Jakit-0.3/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-08-03 14:28:59.000000 Jakit-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:38:31.876247 Jakit-0.4/
+drwxrwxrwx   0        0        0        0 2023-08-04 10:38:31.863246 Jakit-0.4/Jakit/
+-rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.4/Jakit/__init__.py
+-rw-rw-rw-   0        0        0     2875 2023-08-04 10:21:48.000000 Jakit-0.4/Jakit/jakit_jobs.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:38:31.873244 Jakit-0.4/Jakit.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-08-04 10:38:31.000000 Jakit-0.4/Jakit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-08-04 10:38:31.000000 Jakit-0.4/Jakit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 10:38:31.000000 Jakit-0.4/Jakit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 10:38:31.000000 Jakit-0.4/Jakit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.4/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-08-04 10:38:31.876247 Jakit-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 10:38:31.877242 Jakit-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-08-04 10:37:20.000000 Jakit-0.4/setup.py
```

### Comparing `Jakit-0.3/Jakit/jakit_jobs.py` & `Jakit-0.4/Jakit/jakit_jobs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+# designed by: Idriss Animashaun
 import pymongo
 from bson.objectid import ObjectId
 from Dager.dager_data import Database
 import requests
 
 Dager_client = "mongodb://DaggerData_rw:eEsQcKvMgKfH5Di@p1ir1mon019.ger.corp.intel.com:7174,p2ir1mon019.ger.corp.intel.com:7174,p3ir1mon019.ger.corp.intel.com:7174/DaggerData?ssl=true&replicaSet=mongo7174"
 Dager_conn = 'DaggerData'
 Jobs_status_coll = 'Jobs'
 
 ConnectionStringDager = pymongo.MongoClient(Dager_client)
 DatabaseDager = ConnectionStringDager[Dager_conn]
 CollectionJobs = DatabaseDager[Jobs_status_coll]
 
+Jakit_client = "mongodb://JakitDB_rw:6MiQ2Bf5kByS23c@p1ir1mon019.ger.corp.intel.com:7174,p2ir1mon019.ger.corp.intel.com:7174,p3ir1mon019.ger.corp.intel.com:7174/JakitDB?ssl=true&replicaSet=mongo7174"
+Jakit_conn = 'JakitDB'
+Reports_coll = 'Reports'
+
+ConnectionStringJakit = pymongo.MongoClient(Jakit_client)
+DatabaseJakit = ConnectionStringJakit[Jakit_conn]
+CollectionReports = DatabaseJakit[Reports_coll]
+
 class JakitJobs:
     """Jobs class"""
 
     def __init__(self):
         '''Initialize jobids'''
-        # Convert jobids to ObjectIds
-        # self.jobids = [ObjectId(jobid) for jobid in jobids]
 
     def get_jobs(self,jobids):
         """ Read from Mongo and Store into DataFrame """
 
         jobs = CollectionJobs.find({"_id": {"$in": jobids}})
         list_jobs = list(jobs)
 
         return list_jobs
     
     def report_info(self,reportid,toolid):
         """call jakit api"""
-        # get request to jakit api
         report_info = requests.get(f'https://JakitAPI.apps1-ir-int.icloud.intel.com/args?reportID={reportid}&toolID={toolid}')
         
         return report_info.json()
 
 
     def job_info(self,jobids,indicator_names):
         jobids = [ObjectId(jobid) for jobid in jobids]
@@ -60,10 +66,16 @@
                     # Store dataframe in 'Data' field under corresponding wafer
                     if wfr not in job['Data']:
                         job['Data'][wfr] = {}
                     job['Data'][wfr][indicator_name] = df_data
 
         return jobs_info
     
-# jobids = ['64c8b660737dbc28fa09c61a','64c8b66a737dbc28fa09c61b','64c8b677737dbc28fa09c61c']
-# jobs_info = JakitJobs(jobids).get_jobs()
-# print(jobs_info)
+    def report_info(self, reportid):
+
+        info = CollectionReports.find_one({"_id": ObjectId(reportid)})
+
+        if info is not None:
+            return info
+        else:
+            return None
+
```

### Comparing `Jakit-0.3/Jakit.egg-info/PKG-INFO` & `Jakit-0.4/Jakit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.3
+Version: 0.4
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Jakit-0.3/LICENSE` & `Jakit-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Jakit-0.3/PKG-INFO` & `Jakit-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.3
+Version: 0.4
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Jakit-0.3/setup.py` & `Jakit-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Jakit",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     author="Idriss Animashaun",
     author_email="idriss.animashaun@intel.com",
     description="Just Another Kappa Information Tool",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/iddy-ani/Jakit",
```

