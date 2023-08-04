# Comparing `tmp/django_tbase_post_product-2023.8.416911572.tar.gz` & `tmp/django_tbase_post_product-2023.8.416911573.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.8.416911572.tar", last modified: Fri Aug  4 13:54:03 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.8.416911573.tar", last modified: Fri Aug  4 13:56:00 2023, max compression
```

## Comparing `django_tbase_post_product-2023.8.416911572.tar` & `django_tbase_post_product-2023.8.416911573.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.585408 django_tbase_post_product-2023.8.416911572/
--rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/MANIFEST.in
--rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 13:54:03.585408 django_tbase_post_product-2023.8.416911572/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1285 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/README.md
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.581408 django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/
--rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 13:54:03.000000 django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1399 2023-08-04 13:54:03.000000 django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/SOURCES.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)        1 2023-08-04 13:54:03.000000 django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/dependency_links.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       83 2023-08-04 13:54:03.000000 django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/requires.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       11 2023-08-04 13:54:03.000000 django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/top_level.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2023-08-04 13:54:03.585408 django_tbase_post_product-2023.8.416911572/setup.cfg
--rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/setup.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.581408 django_tbase_post_product-2023.8.416911572/tbase_post/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     2672 2023-07-22 10:24:32.000000 django_tbase_post_product-2023.8.416911572/tbase_post/admin.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      146 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/apps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.581408 django_tbase_post_product-2023.8.416911572/tbase_post/migrations/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/migrations/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     5845 2023-08-04 13:50:20.000000 django_tbase_post_product-2023.8.416911572/tbase_post/models.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      479 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/sitemaps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.581408 django_tbase_post_product-2023.8.416911572/tbase_post/static/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.581408 django_tbase_post_product-2023.8.416911572/tbase_post/static/images/
--rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-rw-r--   0 terry     (1000) terry     (1000)       94 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.581408 django_tbase_post_product-2023.8.416911572/tbase_post/templates/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.585408 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     5352 2023-08-04 13:52:40.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/article_list_by_tag.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     3448 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/blog_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)    13517 2023-08-04 13:51:51.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/detail.html
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.585408 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/
--rw-rw-r--   0 terry     (1000) terry     (1000)      591 2023-08-04 02:30:14.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/amazon_link.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2023-08-04 01:44:01.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/last_update.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1797 2023-08-04 01:43:29.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      569 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      576 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/youtube_player.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/last_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      391 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templates/sitemap.xml
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.585408 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:54:03.585408 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)      176 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      190 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     3444 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     3907 2023-07-22 08:36:55.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     7115 2023-08-04 02:27:14.000000 django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/post_extras.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       60 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911572/tbase_post/tests.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      989 2023-08-04 01:55:06.000000 django_tbase_post_product-2023.8.416911572/tbase_post/urls.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     5515 2023-08-04 02:20:15.000000 django_tbase_post_product-2023.8.416911572/tbase_post/views.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/MANIFEST.in
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1285 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/README.md
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.377760 django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 13:56:00.000000 django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1399 2023-08-04 13:56:00.000000 django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)        1 2023-08-04 13:56:00.000000 django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       83 2023-08-04 13:56:00.000000 django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/requires.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       11 2023-08-04 13:56:00.000000 django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/top_level.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       38 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/setup.cfg
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/setup.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2672 2023-07-22 10:24:32.000000 django_tbase_post_product-2023.8.416911573/tbase_post/admin.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      146 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/apps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/migrations/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/migrations/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5845 2023-08-04 13:55:54.000000 django_tbase_post_product-2023.8.416911573/tbase_post/models.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      479 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/sitemaps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.377760 django_tbase_post_product-2023.8.416911573/tbase_post/static/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/static/images/
+-rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-rw-r--   0 terry     (1000) terry     (1000)       94 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/templates/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5352 2023-08-04 13:52:40.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/article_list_by_tag.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3448 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/blog_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)    13517 2023-08-04 13:51:51.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/detail.html
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      591 2023-08-04 02:30:14.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/amazon_link.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2023-08-04 01:44:01.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/last_update.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1797 2023-08-04 01:43:29.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      569 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      576 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/youtube_player.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/last_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      391 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templates/sitemap.xml
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:00.381760 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      176 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      190 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3444 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3907 2023-07-22 08:36:55.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7115 2023-08-04 02:27:14.000000 django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/post_extras.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)       60 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911573/tbase_post/tests.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      989 2023-08-04 01:55:06.000000 django_tbase_post_product-2023.8.416911573/tbase_post/urls.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5515 2023-08-04 02:20:15.000000 django_tbase_post_product-2023.8.416911573/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.8.416911572/PKG-INFO` & `django_tbase_post_product-2023.8.416911573/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.8.416911572
+Version: 2023.8.416911573
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.8.416911572/README.md` & `django_tbase_post_product-2023.8.416911573/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.8.416911572
+Version: 2023.8.416911573
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.8.416911572/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.8.416911573/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/setup.py` & `django_tbase_post_product-2023.8.416911573/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/admin.py` & `django_tbase_post_product-2023.8.416911573/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/models.py` & `django_tbase_post_product-2023.8.416911573/tbase_post/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,37 +109,37 @@
                                     default=None,
                                     help_text="""
                                     亚马逊的推广id，用于生成推广链接，可以通过https://affiliate-program.amazon.com/home 注册。
                                     
                                     """)
 
 
-    ads_sidebar = models.CharField("ads_sidebar",
+    ads_sidebar = models.TextField("ads_sidebar",
                                     # max_length=32,
                                     null=True,
                                     blank=True,
                                     default=None,
                                     help_text="""
                                     广告1: 右侧边栏
                                     
                                     """)
 
-    ads_content1 = models.CharField("ads_content1",
+    ads_content1 = models.TextField("ads_content1",
                                     # max_length=32,
                                     null=True,
                                     blank=True,
                                     default=None,
                                     help_text="""
                                     广告2: 主要内容之后
                                     
                                     """)
 
 
 
-    ads_list1 = models.CharField("ads_list1",
+    ads_list1 = models.TextField("ads_list1",
                                     # max_length=32,
                                     null=True,
                                     blank=True,
                                     default=None,
                                     help_text="""
                                     广告3:  列表广告
```

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.8.416911573/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/article_list_by_tag.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/amazon_link.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/last_update.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/last_update.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/related_post_by_tags.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/related_post_by_tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/tags.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/extras/youtube_player.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/extras/youtube_player.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templates/post/last_index.html` & `django_tbase_post_product-2023.8.416911573/tbase_post/templates/post/last_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc` & `django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.8.416911573/tbase_post/templatetags/post_extras.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/urls.py` & `django_tbase_post_product-2023.8.416911573/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911572/tbase_post/views.py` & `django_tbase_post_product-2023.8.416911573/tbase_post/views.py`

 * *Files identical despite different names*

