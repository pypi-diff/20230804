# Comparing `tmp/strongmind_deployment-1.1.0-py3-none-any.whl.zip` & `tmp/strongmind_deployment-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 11121 bytes, number of entries: 10
+Zip file size: 11934 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
 -rw-r--r--  2.0 unx    11707 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
 -rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 strongmind_deployment/dynamo.py
--rw-r--r--  2.0 unx    10429 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+-rw-r--r--  2.0 unx    11019 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
 -rw-r--r--  2.0 unx     2918 b- defN 20-Feb-02 00:00 strongmind_deployment/redis.py
 -rw-r--r--  2.0 unx     2097 b- defN 20-Feb-02 00:00 strongmind_deployment/secrets.py
-?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      889 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/RECORD
-10 files, 34612 bytes uncompressed, 9585 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx     2093 b- defN 20-Feb-02 00:00 strongmind_deployment/storage.py
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      978 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.1.dist-info/RECORD
+11 files, 37384 bytes uncompressed, 10258 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -12,20 +12,23 @@
 
 Filename: strongmind_deployment/redis.py
 Comment: 
 
 Filename: strongmind_deployment/secrets.py
 Comment: 
 
-Filename: strongmind_deployment-1.1.0.dist-info/METADATA
+Filename: strongmind_deployment/storage.py
 Comment: 
 
-Filename: strongmind_deployment-1.1.0.dist-info/WHEEL
+Filename: strongmind_deployment-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-1.1.0.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-1.1.0.dist-info/RECORD
+Filename: strongmind_deployment-1.1.1.dist-info/licenses/LICENSE
+Comment: 
+
+Filename: strongmind_deployment-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/rails.py

```diff
@@ -4,14 +4,15 @@
 import pulumi
 import pulumi_random as random
 import pulumi_aws as aws
 from pulumi import export, Output
 
 from strongmind_deployment.container import ContainerComponent
 from strongmind_deployment.redis import RedisComponent, QueueComponent, CacheComponent
+from strongmind_deployment.storage import StorageComponent
 from strongmind_deployment.secrets import SecretsComponent
 
 
 def sidekiq_present():  # pragma: no cover
     return os.path.exists('../Gemfile') and 'sidekiq' in open('../Gemfile').read()
 
 
@@ -35,16 +36,18 @@
         :key cpu: The number of CPU units to reserve for the web container. Defaults to 256.
         :key memory: The amount of memory (in MiB) to allow the web container to use. Defaults to 512.
         :key app_path: The path to the Rails application for the web. Defaults to `./`.
         :key worker_cpu: The number of CPU units to reserve for the worker container. Defaults to 256.
         :key worker_memory: The amount of memory (in MiB) to allow the worker container to use. Defaults to 512.
         :key worker_app_path: The path to the Rails application for the worker. Defaults to `./`.
         :key dynamo_tables: A list of DynamoDB tables to create. Defaults to `[]`. Each table is a DynamoComponent.
+        :key storage: Whether to create an S3 bucket for the Rails application. Defaults to False.
         """
         super().__init__('strongmind:global_build:commons:rails', name, None, opts)
+        self.storage = None
         self.need_worker = None
         self.cname_record = None
         self.firewall_rule = None
         self.db_password = None
         self.web_container = None
         self.worker_container = None
         self.secret = None
@@ -151,14 +154,17 @@
         if self.need_worker is None:  # pragma: no cover
             # If we don't know if we need a worker, check for sidekiq in the Gemfile
             self.need_worker = sidekiq_present()
 
         if self.need_worker:
             self.setup_worker()
 
+        if self.kwargs.get('storage', False):
+            self.setup_storage()
+
     def setup_worker(self):
         worker_entry_point = self.kwargs.get('worker_entry_point', ["sh", "-c", "bundle exec sidekiq"])
         self.kwargs['entry_point'] = worker_entry_point
         self.kwargs['cpu'] = self.kwargs.get('worker_cpu')
         self.kwargs['memory'] = self.kwargs.get('worker_memory')
         self.kwargs['app_path'] = self.kwargs.get('worker_app_path')
         self.kwargs['need_load_balancer'] = False
@@ -222,7 +228,15 @@
                              self.rds_serverless_cluster.endpoint,
                              ':5432/app')
 
     def setup_dynamo(self):
         for table_component in self.dynamo_tables:
             env_var_name = table_component._name.upper() + '_DYNAMO_TABLE_NAME'
             self.env_vars[env_var_name] = table_component.table.name
+
+    def setup_storage(self):
+        self.storage = StorageComponent("storage",
+                                        pulumi.ResourceOptions(parent=self),
+                                        **self.kwargs
+                                        )
+        self.env_vars['S3_BUCKET_NAME'] = self.storage.bucket.bucket
+
```

## Comparing `strongmind_deployment-1.1.0.dist-info/METADATA` & `strongmind_deployment-1.1.1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 1.1.0
+Version: 1.1.1
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-1.1.0.dist-info/licenses/LICENSE` & `strongmind_deployment-1.1.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-1.1.0.dist-info/RECORD` & `strongmind_deployment-1.1.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 strongmind_deployment/container.py,sha256=8Ke-4oZScnN6dr1eoyp1LvE-pPHt4ZcrS4RBWUBnHY4,11707
 strongmind_deployment/dynamo.py,sha256=ppTNvIMdj9tr85thLlciCoszdZAa6ehgeIIm9pwu1Es,4757
-strongmind_deployment/rails.py,sha256=dHMilL9Red9FbnHizsnL8C-ZnfmmdgYVl0Xe7xCo7Bc,10429
+strongmind_deployment/rails.py,sha256=StD30BisgNpq30vCkTvFfhYfZbsztOd3l7ruIdNhWDQ,11019
 strongmind_deployment/redis.py,sha256=Cl7avjc0PNiqJ3E4IgG9_2js8tcG3FeSNpGbpGmCAeE,2918
 strongmind_deployment/secrets.py,sha256=YbsgCd1Uz94ZAu9VrtNjc0f5nc1xNEHEdhb150mOnzU,2097
-strongmind_deployment-1.1.0.dist-info/METADATA,sha256=9KEACxjhC2fzYQGkEZbK5nTbnzdd9V8J3LITYNXXC6c,675
-strongmind_deployment-1.1.0.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-strongmind_deployment-1.1.0.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-1.1.0.dist-info/RECORD,,
+strongmind_deployment/storage.py,sha256=-C09-MBKoHyCb9n6lvyETa14ZuFz030HNpai-4zFpC4,2093
+strongmind_deployment-1.1.1.dist-info/METADATA,sha256=Arr9m_Rt-RQzeSaV-lYTHIv2nc3Xw4C0WYLqwI8GBBU,675
+strongmind_deployment-1.1.1.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+strongmind_deployment-1.1.1.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-1.1.1.dist-info/RECORD,,
```

