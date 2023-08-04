# Comparing `tmp/django_tbase_post_product-2023.8.416911605.tar.gz` & `tmp/django_tbase_post_product-2023.8.416911617.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.8.416911605.tar", last modified: Fri Aug  4 14:49:30 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.8.416911617.tar", last modified: Fri Aug  4 15:08:50 2023, max compression
```

## Comparing `django_tbase_post_product-2023.8.416911605.tar` & `django_tbase_post_product-2023.8.416911617.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/
--rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/MANIFEST.in
--rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1285 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/README.md
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/
--rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 14:49:30.000000 django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1448 2023-08-04 14:49:30.000000 django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/SOURCES.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)        1 2023-08-04 14:49:30.000000 django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/dependency_links.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       83 2023-08-04 14:49:30.000000 django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/requires.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       11 2023-08-04 14:49:30.000000 django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/top_level.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/setup.cfg
--rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/setup.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/tbase_post/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     2761 2023-08-04 14:02:14.000000 django_tbase_post_product-2023.8.416911605/tbase_post/admin.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      146 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/tbase_post/apps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/migrations/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/tbase_post/migrations/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     5845 2023-08-04 14:01:34.000000 django_tbase_post_product-2023.8.416911605/tbase_post/models.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      479 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/tbase_post/sitemaps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/static/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/static/images/
--rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-rw-r--   0 terry     (1000) terry     (1000)       94 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/templates/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     5352 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/article_list_by_tag.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     3448 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/blog_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)    13927 2023-08-04 14:39:03.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/detail.html
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/
--rw-rw-r--   0 terry     (1000) terry     (1000)      732 2023-08-04 14:44:59.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/amazon_ads.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      591 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/amazon_link.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/last_update.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1797 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      569 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      576 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/youtube_player.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/last_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      391 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templates/sitemap.xml
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 14:49:30.823673 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)      176 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      190 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     3444 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2023-08-04 14:28:25.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     7717 2023-08-04 14:28:24.000000 django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/post_extras.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       60 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911605/tbase_post/tests.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      989 2023-08-04 01:55:06.000000 django_tbase_post_product-2023.8.416911605/tbase_post/urls.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     5515 2023-08-04 02:20:15.000000 django_tbase_post_product-2023.8.416911605/tbase_post/views.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/MANIFEST.in
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1285 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/README.md
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 15:08:50.000000 django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1448 2023-08-04 15:08:50.000000 django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)        1 2023-08-04 15:08:50.000000 django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       83 2023-08-04 15:08:50.000000 django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/requires.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       11 2023-08-04 15:08:50.000000 django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/top_level.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       38 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/setup.cfg
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/setup.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/tbase_post/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2761 2023-08-04 14:02:14.000000 django_tbase_post_product-2023.8.416911617/tbase_post/admin.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      146 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/tbase_post/apps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/migrations/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/tbase_post/migrations/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5845 2023-08-04 14:01:34.000000 django_tbase_post_product-2023.8.416911617/tbase_post/models.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      479 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/tbase_post/sitemaps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/static/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/static/images/
+-rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-rw-r--   0 terry     (1000) terry     (1000)       94 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/templates/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5394 2023-08-04 15:07:46.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/article_list_by_tag.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3448 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/blog_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)    14019 2023-08-04 15:06:23.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/detail.html
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      732 2023-08-04 14:44:59.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/amazon_ads.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      591 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/amazon_link.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/last_update.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1797 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      569 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      576 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/youtube_player.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/last_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      391 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templates/sitemap.xml
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 15:08:50.090973 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      176 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      190 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3444 2023-08-04 13:56:42.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2023-08-04 14:28:25.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7717 2023-08-04 14:28:24.000000 django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/post_extras.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)       60 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911617/tbase_post/tests.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      989 2023-08-04 01:55:06.000000 django_tbase_post_product-2023.8.416911617/tbase_post/urls.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5515 2023-08-04 02:20:15.000000 django_tbase_post_product-2023.8.416911617/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.8.416911605/PKG-INFO` & `django_tbase_post_product-2023.8.416911617/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.8.416911605
+Version: 2023.8.416911617
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.8.416911605/README.md` & `django_tbase_post_product-2023.8.416911617/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.8.416911605
+Version: 2023.8.416911617
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.8.416911605/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.8.416911617/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/setup.py` & `django_tbase_post_product-2023.8.416911617/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/admin.py` & `django_tbase_post_product-2023.8.416911617/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/models.py` & `django_tbase_post_product-2023.8.416911617/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.8.416911617/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/article_list_by_tag.html`

 * *Files 2% similar despite different names*

```diff
@@ -163,13 +163,20 @@
    {% endblock %}
     <div class="w-full bg-white shadow flex flex-col my-4 p-6">
 
     </div>
 
 <!-- 广告代码  ads_sidebar-->
 {% autoescape off %}
-{% get_solo 'tbase_post.AmazonSettings' as amz %}{{amz.ads_sidebar}}
+{% get_solo 'tbase_post.AmazonSettings' as amz %}
+
+
+{% if amz.ads_sidebar %}
+{{amz.ads_sidebar}}
+
+{% endif %}
+
 {% endautoescape %}
 <!-- 广告代码结束 -->
 
     <!-- sidebar_section endblock -->
    {% endblock %}
```

#### html2text {}

```diff
@@ -24,9 +24,10 @@
  {% if page_obj.has_previous %} «_first previous {% endif %}  Page {
 { page_obj.number }} of {{ page_obj.paginator.num_pages }}.  {% if
 page_obj.has_next %} next last_» {% endif %}
 {% endcomment %} {% endblock %} {% block sidebar_section %}  {% block about_us
 %}
  {% last_update 10 %}
 {% endblock %}
- {% autoescape off %} {% get_solo 'tbase_post.AmazonSettings' as amz %}{
-{amz.ads_sidebar}} {% endautoescape %}   {% endblock %}
+ {% autoescape off %} {% get_solo 'tbase_post.AmazonSettings' as amz %} {% if
+amz.ads_sidebar %} {{amz.ads_sidebar}} {% endif %} {% endautoescape %}   {%
+endblock %}
```

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/detail.html`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,19 @@
 
 
 
 
 
 <!-- 广告代码 ads_content1 -->
     {% autoescape off %}
-    {% get_solo 'tbase_post.AmazonSettings' as amz %}{{amz.ads_content1}}
+    {% get_solo 'tbase_post.AmazonSettings' as amz %}
+    {% if amz.ads_content1 %}
+    {{amz.ads_content1}}
+
+    {% endif %}
     {% endautoescape %}
 <!-- 广告代码结束 -->
 
         <div class="fixed bottom-0 left-0 w-full bg-gray-800 text-white py-4 px-6">
                <!-- 这里放置固定顶端内容 -->
                 <div class="container mx-auto flex flex-wrap py-1 px-3 ">
                      
@@ -384,16 +388,20 @@
 
 <!--亚马逊推广链接-->
 {% get_solo 'tbase_post.AmazonSettings' as amazon %}
 {% amazon_ads object.product_id detail.product_name amazon.store_id %}
 <!--亚马逊推广链接结束-->
 
  
-{% get_solo 'tbase_post.AmazonSettings' as amz %}{{amz.ads_sidebar}}
+{% get_solo 'tbase_post.AmazonSettings' as amz %} 
+
 
+{% if amz.ads_sidebar %}
+{{amz.ads_sidebar}}
 
+{% endif %}
 
 {% endautoescape %}
 <!-- 广告代码结束 -->
 
     <!-- sidebar_section endblock -->
    {% endblock %}
```

#### html2text {}

```diff
@@ -26,16 +26,16 @@
 {% comment %} By David_Grzyb, {% endcomment %} Published on {
 {detail.created_on}}
  {% youtube_player object.youtube_id %}
     {{ detail.content|safe_markdown }}   {% get_solo
 'tbase_post.AmazonSettings' as amazon %}
 **_{{detail.product_name}}_**
  Buy_on_Amazon
-   {% autoescape off %} {% get_solo 'tbase_post.AmazonSettings' as amz %}{
-{amz.ads_content1}} {% endautoescape %}
+   {% autoescape off %} {% get_solo 'tbase_post.AmazonSettings' as amz %} {% if
+amz.ads_content1 %} {{amz.ads_content1}} {% endif %} {% endautoescape %}
 [{{detail.product_name}}]
  {% get_solo 'tbase_post.AmazonSettings' as amazon %} {% amazon_link
 object.product_id detail.product_name amazon.store_id %}
 {% cache 36000 tags object.pk %}  {% tags object.tags 5 object.pk %}  {%
 endcache %}
 {% cache 36000 related_post_by_tags object.pk %} {% related_post_by_tags
 object.tags 10 object.pk %} {% endcache %}
@@ -45,9 +45,9 @@
  {{detail.get_previous_by_created_on.title}}
  {%endif%} {% if detail.get_next_by_created_on %}
 {{detail.get_next_by_created_on.title}}
  {%endif%} {% endblock %}   {% block article_author %} {% endblock %}  {% block
 sidebar_section %}
  {% autoescape off %}  {% get_solo 'tbase_post.AmazonSettings' as amazon %} {%
 amazon_ads object.product_id detail.product_name amazon.store_id %}  {%
-get_solo 'tbase_post.AmazonSettings' as amz %}{{amz.ads_sidebar}} {%
-endautoescape %}   {% endblock %}
+get_solo 'tbase_post.AmazonSettings' as amz %} {% if amz.ads_sidebar %} {
+{amz.ads_sidebar}} {% endif %} {% endautoescape %}   {% endblock %}
```

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/amazon_ads.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/amazon_ads.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/amazon_link.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/last_update.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/last_update.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/related_post_by_tags.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/related_post_by_tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/tags.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/extras/youtube_player.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/extras/youtube_player.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templates/post/last_index.html` & `django_tbase_post_product-2023.8.416911617/tbase_post/templates/post/last_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc` & `django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.8.416911617/tbase_post/templatetags/post_extras.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/urls.py` & `django_tbase_post_product-2023.8.416911617/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.8.416911605/tbase_post/views.py` & `django_tbase_post_product-2023.8.416911617/tbase_post/views.py`

 * *Files identical despite different names*

