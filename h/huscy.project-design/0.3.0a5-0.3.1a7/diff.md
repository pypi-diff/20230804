# Comparing `tmp/huscy.project_design-0.3.0a5.tar.gz` & `tmp/huscy.project_design-0.3.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_design-0.3.0a5.tar", last modified: Mon Apr 17 10:53:51 2023, max compression
+gzip compressed data, was "huscy.project_design-0.3.1a7.tar", last modified: Fri Aug  4 12:40:48 2023, max compression
```

## Comparing `huscy.project_design-0.3.0a5.tar` & `huscy.project_design-0.3.1a7.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.397515 huscy.project_design-0.3.0a5/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2021-10-25 14:36:31.000000 huscy.project_design-0.3.0a5/LICENSE
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1020 2023-04-17 10:53:51.397515 huscy.project_design-0.3.0a5/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.3.0a5/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy/project_design/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-04-14 09:00:23.000000 huscy.project_design-0.3.0a5/huscy/project_design/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      466 2022-12-05 13:36:14.000000 huscy.project_design-0.3.0a5/huscy/project_design/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.3.0a5/huscy/project_design/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy/project_design/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     8576 2023-04-17 10:53:50.000000 huscy.project_design-0.3.0a5/huscy/project_design/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.3.0a5/huscy/project_design/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4677 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2017 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1669 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1393 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1020 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      591 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:53:51.397515 huscy.project_design-0.3.0a5/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1548 2023-04-17 10:46:38.000000 huscy.project_design-0.3.0a5/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-04 12:40:48.786615 huscy.project_design-0.3.1a7/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1054 2023-08-04 12:40:48.786615 huscy.project_design-0.3.1a7/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.3.1a7/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-04 12:40:48.782616 huscy.project_design-0.3.1a7/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-04 12:40:48.786615 huscy.project_design-0.3.1a7/huscy/project_design/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-08-04 12:15:52.000000 huscy.project_design-0.3.1a7/huscy/project_design/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.3.1a7/huscy/project_design/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      769 2023-08-03 12:41:53.000000 huscy.project_design-0.3.1a7/huscy/project_design/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.3.1a7/huscy/project_design/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-04 12:40:48.786615 huscy.project_design-0.3.1a7/huscy/project_design/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3802 2023-08-04 12:40:48.000000 huscy.project_design-0.3.1a7/huscy/project_design/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.3.1a7/huscy/project_design/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2569 2023-08-04 12:15:52.000000 huscy.project_design-0.3.1a7/huscy/project_design/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2277 2023-08-03 12:41:53.000000 huscy.project_design-0.3.1a7/huscy/project_design/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2214 2023-08-03 12:41:53.000000 huscy.project_design-0.3.1a7/huscy/project_design/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2302 2023-08-03 12:41:53.000000 huscy.project_design-0.3.1a7/huscy/project_design/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-04 12:40:48.786615 huscy.project_design-0.3.1a7/huscy.project_design.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1054 2023-08-04 12:40:48.000000 huscy.project_design-0.3.1a7/huscy.project_design.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      583 2023-08-04 12:40:48.000000 huscy.project_design-0.3.1a7/huscy.project_design.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-08-04 12:40:48.000000 huscy.project_design-0.3.1a7/huscy.project_design.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2023-08-04 12:40:48.000000 huscy.project_design-0.3.1a7/huscy.project_design.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-08-04 12:40:48.000000 huscy.project_design-0.3.1a7/huscy.project_design.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-08-04 12:40:48.786615 huscy.project_design-0.3.1a7/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1548 2023-04-17 10:46:38.000000 huscy.project_design-0.3.1a7/setup.py
```

### Comparing `huscy.project_design-0.3.0a5/PKG-INFO` & `huscy.project_design-0.3.1a7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: huscy.project_design
-Version: 0.3.0a5
+Version: 0.3.1a7
+Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # huscy.project_design
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -18,10 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-License-File: LICENSE
-
-# huscy.project_design
```

### Comparing `huscy.project_design-0.3.0a5/huscy/project_design/serializer.py` & `huscy.project_design-0.3.1a7/huscy/project_design/serializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 from rest_framework import serializers
 
-from huscy.project_design.models import DataAcquisitionMethod, Experiment, Session
-from huscy.project_design.services import (
-    add_data_acquisition_method,
-    create_experiment,
-    create_session,
-)
+from huscy.project_design import models, services
 
 
 class DataAcquisitionMethodSerializer(serializers.ModelSerializer):
     class Meta:
-        model = DataAcquisitionMethod
+        model = models.DataAcquisitionMethod
         fields = (
             'id',
             'location',
             'order',
             'session',
+            'stimulus',
             'type',
         )
+        read_only_fields = 'id', 'order', 'session'
+
+    def get_fields(self):
+        fields = super().get_fields()
+        request = self.context.get('request')
+        if request and request.method == 'PUT':
+            fields['type'].read_only = True
+        return fields
 
     def create(self, validated_data):
-        return add_data_acquisition_method(**validated_data)
+        return services.create_data_acquisition_method(**validated_data)
+
+    def update(self, data_acquisition_method, validated_data):
+        return services.update_data_acquisition_method(data_acquisition_method, **validated_data)
 
 
 class SessionSerializer(serializers.ModelSerializer):
-    order = serializers.IntegerField(required=False)
+    data_acquisition_methods = DataAcquisitionMethodSerializer(many=True, read_only=True)
     title = serializers.CharField(required=False)
 
     class Meta:
-        model = Session
+        model = models.Session
         fields = (
+            'id',
+            'data_acquisition_methods',
             'duration',
             'experiment',
-            'id',
-            'operator',
             'order',
             'title',
         )
+        read_only_fields = 'id', 'experiment', 'order'
 
     def create(self, validated_data):
-        return create_session(**validated_data)
+        return services.create_session(**validated_data)
 
-    def to_representation(self, session):
-        response = super().to_representation(session)
-        response['data_acquisition_methods'] = \
-            DataAcquisitionMethodSerializer(session.dataacquisitionmethod_set.all(), many=True).data
-        return response
+    def update(self, session, validated_data):
+        return services.update_session(session, **validated_data)
 
 
 class ExperimentSerializer(serializers.ModelSerializer):
-    order = serializers.IntegerField(required=False)
+    sessions = SessionSerializer(many=True, read_only=True)
     title = serializers.CharField(required=False)
 
     class Meta:
-        model = Experiment
+        model = models.Experiment
         fields = (
-            'description',
             'id',
+            'description',
             'order',
             'project',
+            'sessions',
             'title',
         )
-        read_only_fields = 'project',
+        read_only_fields = 'id', 'order', 'project',
 
     def create(self, validated_data):
-        return create_experiment(**validated_data)
+        return services.create_experiment(**validated_data)
 
-    def to_representation(self, experiment):
-        response = super().to_representation(experiment)
-        response['sessions'] = SessionSerializer(experiment.sessions.all(), many=True).data
-        return response
+    def update(self, experiment, validated_data):
+        return services.update_experiment(experiment, **validated_data)
```

### Comparing `huscy.project_design-0.3.0a5/huscy/project_design/views.py` & `huscy.project_design-0.3.1a7/huscy/project_design/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 from django.shortcuts import get_object_or_404
 from rest_framework import mixins, viewsets
 from rest_framework.permissions import IsAuthenticated
 
-from huscy.project_design import serializer, services
+from huscy.project_design import models, serializer, services
 from huscy.projects.models import Project
 
 
-class DataAcquisitionMethodViewSet(mixins.CreateModelMixin, mixins.DestroyModelMixin,
-                                   mixins.UpdateModelMixin, viewsets.GenericViewSet):
-    queryset = services.get_data_acquisition_methods()
-    serializer_class = serializer.DataAcquisitionMethodSerializer
-    permission_classes = (IsAuthenticated, )
-
-
 class ExperimentViewSet(mixins.CreateModelMixin, mixins.DestroyModelMixin, mixins.ListModelMixin,
                         mixins.UpdateModelMixin, viewsets.GenericViewSet):
     serializer_class = serializer.ExperimentSerializer
     permission_classes = (IsAuthenticated, )
 
     def initial(self, request, *args, **kwargs):
         self.project = get_object_or_404(Project, pk=self.kwargs['project_pk'])
@@ -25,11 +18,42 @@
     def get_queryset(self):
         return services.get_experiments(self.project)
 
     def perform_create(self, serializer):
         serializer.save(project=self.project)
 
 
-class SessionViewSet(viewsets.ModelViewSet):
-    queryset = services.get_sessions()
+class SessionViewSet(mixins.CreateModelMixin, mixins.DestroyModelMixin, mixins.UpdateModelMixin,
+                     viewsets.GenericViewSet):
+    queryset = models.Session.objects.all()
+    permission_classes = (IsAuthenticated, )
     serializer_class = serializer.SessionSerializer
+
+    def initial(self, request, *args, **kwargs):
+        self.experiment = get_object_or_404(
+            models.Experiment,
+            pk=self.kwargs['experiment_pk'],
+            project=self.kwargs['project_pk']
+        )
+        super().initial(request, *args, **kwargs)
+
+    def perform_create(self, serializer):
+        serializer.save(experiment=self.experiment)
+
+
+class DataAcquisitionMethodViewSet(mixins.CreateModelMixin, mixins.DestroyModelMixin,
+                                   mixins.UpdateModelMixin, viewsets.GenericViewSet):
+    queryset = models.DataAcquisitionMethod.objects.all()
+    serializer_class = serializer.DataAcquisitionMethodSerializer
     permission_classes = (IsAuthenticated, )
+
+    def initial(self, request, *args, **kwargs):
+        self.session = get_object_or_404(
+            models.Session,
+            experiment=self.kwargs['experiment_pk'],
+            pk=self.kwargs['session_pk'],
+            experiment__project=self.kwargs['project_pk']
+        )
+        super().initial(request, *args, **kwargs)
+
+    def perform_create(self, serializer):
+        serializer.save(session=self.session)
```

### Comparing `huscy.project_design-0.3.0a5/huscy.project_design.egg-info/PKG-INFO` & `huscy.project_design-0.3.1a7/huscy.project_design.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: huscy.project-design
-Version: 0.3.0a5
+Version: 0.3.1a7
+Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # huscy.project_design
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -18,10 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-License-File: LICENSE
-
-# huscy.project_design
```

### Comparing `huscy.project_design-0.3.0a5/huscy.project_design.egg-info/SOURCES.txt` & `huscy.project_design-0.3.1a7/huscy.project_design.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 huscy.project_design.egg-info/PKG-INFO
 huscy.project_design.egg-info/SOURCES.txt
 huscy.project_design.egg-info/dependency_links.txt
 huscy.project_design.egg-info/requires.txt
 huscy.project_design.egg-info/top_level.txt
```

### Comparing `huscy.project_design-0.3.0a5/setup.py` & `huscy.project_design-0.3.1a7/setup.py`

 * *Files identical despite different names*

