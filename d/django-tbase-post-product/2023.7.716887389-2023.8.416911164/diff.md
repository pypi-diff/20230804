# Comparing `tmp/django_tbase_post_product-2023.7.716887389.tar.gz` & `tmp/django_tbase_post_product-2023.8.416911164.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.7.716887389.tar", last modified: Fri Jul  7 14:09:26 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.8.416911164.tar", last modified: Fri Aug  4 02:33:25 2023, max compression
```

## Comparing `django_tbase_post_product-2023.7.716887389.tar` & `django_tbase_post_product-2023.8.416911164.tar`

### file list

```diff
@@ -1,52 +1,48 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.7.716887389/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.7.716887389/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.781842 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.7.716887389/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887389/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-07-07 14:04:14.000000 django_tbase_post_product-2023.7.716887389/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887389/tbase_post/apps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     4230 2023-07-07 14:00:03.000000 django_tbase_post_product-2023.7.716887389/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.7.716887389/tbase_post/sitemaps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.781842 django_tbase_post_product-2023.7.716887389/tbase_post/static/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/static/images/
--rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887389/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887389/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templates/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/
--rw-r--r--   0 terry     (1000) terry     (1000)     3667 2023-07-02 16:58:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/article_list_by_tag.html
--rw-r--r--   0 terry     (1000) terry     (1000)     2127 2023-07-02 15:36:36.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/blog_index.html
--rw-r--r--   0 terry     (1000) terry     (1000)     5170 2023-07-02 16:55:04.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/detail.html
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/
--rw-r--r--   0 terry     (1000) terry     (1000)      583 2023-07-02 15:28:54.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/amazon_link.html
--rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-07-02 14:56:34.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/last_update.html
--rw-r--r--   0 terry     (1000) terry     (1000)      366 2023-07-02 15:28:37.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      569 2023-07-02 16:41:58.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/sitemap.xml
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)      176 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3444 2023-07-02 16:53:59.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     6241 2023-07-07 14:08:47.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/post_extras.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887389/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      841 2023-07-02 14:42:11.000000 django_tbase_post_product-2023.7.716887389/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     4262 2023-07-02 17:03:03.000000 django_tbase_post_product-2023.7.716887389/tbase_post/views.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/MANIFEST.in
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1285 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/README.md
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/django_tbase_post_product.egg-info/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1607 2023-08-04 02:33:25.000000 django_tbase_post_product-2023.8.416911164/django_tbase_post_product.egg-info/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1399 2023-08-04 02:33:25.000000 django_tbase_post_product-2023.8.416911164/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)        1 2023-08-04 02:33:25.000000 django_tbase_post_product-2023.8.416911164/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       83 2023-08-04 02:33:25.000000 django_tbase_post_product-2023.8.416911164/django_tbase_post_product.egg-info/requires.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       11 2023-08-04 02:33:25.000000 django_tbase_post_product-2023.8.416911164/django_tbase_post_product.egg-info/top_level.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       38 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/setup.cfg
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/setup.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2672 2023-07-22 10:24:32.000000 django_tbase_post_product-2023.8.416911164/tbase_post/admin.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      146 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/apps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/migrations/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/migrations/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4531 2023-07-22 10:14:30.000000 django_tbase_post_product-2023.8.416911164/tbase_post/models.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      479 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/sitemaps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/static/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/static/images/
+-rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-rw-r--   0 terry     (1000) terry     (1000)       94 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/templates/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4988 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/article_list_by_tag.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3448 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/blog_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)    13175 2023-08-04 01:42:13.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/detail.html
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      591 2023-08-04 02:30:14.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/amazon_link.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2023-08-04 01:44:01.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/last_update.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1797 2023-08-04 01:43:29.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      569 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      576 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/youtube_player.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2023-07-26 17:48:32.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/last_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      391 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templates/sitemap.xml
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2023-08-04 02:33:25.394665 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      176 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      190 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3444 2023-07-21 12:28:28.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3907 2023-07-22 08:36:55.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7115 2023-08-04 02:27:14.000000 django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/post_extras.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)       60 2023-07-21 12:01:45.000000 django_tbase_post_product-2023.8.416911164/tbase_post/tests.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      989 2023-08-04 01:55:06.000000 django_tbase_post_product-2023.8.416911164/tbase_post/urls.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5515 2023-08-04 02:20:15.000000 django_tbase_post_product-2023.8.416911164/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.7.716887389/PKG-INFO` & `django_tbase_post_product-2023.8.416911164/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.7.716887389
+Version: 2023.8.416911164
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -32,14 +32,16 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
+- 2023/07/07
+加入更新时间,排序默认使用更新时间
 
 - 2023/06/05
 优化相关内容查询,模板文件,针对tags内容数目低于10的链接添加nofollow。
 
 
 - 2023/06/02
 加入seo优化，对tags内容过少（小于10）的页面添加noindex
```

### Comparing `django_tbase_post_product-2023.7.716887389/README.md` & `django_tbase_post_product-2023.8.416911164/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
+- 2023/07/07
+加入更新时间,排序默认使用更新时间
 
 - 2023/06/05
 优化相关内容查询,模板文件,针对tags内容数目低于10的链接添加nofollow。
 
 
 - 2023/06/02
 加入seo优化，对tags内容过少（小于10）的页面添加noindex
```

### Comparing `django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.8.416911164/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.7.716887389
+Version: 2023.8.416911164
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -32,14 +32,16 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
+- 2023/07/07
+加入更新时间,排序默认使用更新时间
 
 - 2023/06/05
 优化相关内容查询,模板文件,针对tags内容数目低于10的链接添加nofollow。
 
 
 - 2023/06/02
 加入seo优化，对tags内容过少（小于10）的页面添加noindex
```

### Comparing `django_tbase_post_product-2023.7.716887389/setup.py` & `django_tbase_post_product-2023.8.416911164/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/admin.py` & `django_tbase_post_product-2023.8.416911164/tbase_post/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,35 +3,59 @@
 # Register your models here.
 from .models import Post,AmazonSettings
 # from markdownx.admin import MarkdownxModelAdmin
 # from markdownx.widgets import AdminMarkdownxWidget
 from martor.widgets import AdminMartorWidget
 from solo.admin import SingletonModelAdmin
 from django.utils.safestring import mark_safe
-
+from django.utils.safestring import SafeText
 class PostAdmin(admin.ModelAdmin):
-    list_display = ('title','image_data', 'updated_on','product_name','product_id')
+    save_on_top = True
+    list_display = ('title','image_data', 'updated_on','product_name','product_id','youtube_id')
     list_filter = (['updated_on']) # 过滤字段
     search_fields =('title', 'product_name','product_id')  # 设置搜索字段
     ordering = ('-updated_on','product_name','product_id' )
     # formfield_overrides = {
     #     models.TextField: {'widget': AdminMarkdownxWidget},
     # }
-    readonly_fields=('image_data',)
+    fieldsets = (
+            ('产品信息', {
+                'fields': ('product_name', 'product_id', 'article_img','image_data',
+                            'youtube_id','youtube_player'
+                            ),
+            }),
+            ('seo优化', {
+                'fields': ('tags', 'meta_keywords', 'meta_description'),
+            }),
+            ('内容', {
+                'fields': ['content'],
+            }),
+            ('资料', {
+                'fields': ['data'],
+            }),
+        )
+
+    readonly_fields=('image_data','youtube_player',)
 
     def image_data(self, obj):
         return mark_safe(f'<img width="100px" class="list_img_article_img" src="{obj.article_img}">')
+
+
+    def youtube_player(self, obj):
+        return SafeText(f'<iframe width="560" height="315" src="https://www.youtube.com/embed/{obj.youtube_id}" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>')
+ 
+
+
+ 
     formfield_overrides = {
         models.TextField: {
             'widget': AdminMartorWidget
         },
     }
 
-    # pass
-
 
 admin.site.register(Post, PostAdmin)
 
 class AmazonSettingsAdmin(SingletonModelAdmin):
     # form = ConfigurationForm):
     # form = ConfigurationForm
     # list_display = ('site_title', 'maintenance_mode')
```

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/models.py` & `django_tbase_post_product-2023.8.416911164/tbase_post/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,15 +45,21 @@
                            blank=True,
                            help_text="""填写亚马逊的产品id，用于产生产品链接,
                            比如：https://www.amazon.com/Audio-Wireless-Bluetooth-Earbuds-Charging/dp/B07R7DT3JV/
                            id则为B07R7DT3JV
                            
                            """
                            )
-    
+    youtube_id = models.CharField("Youtube id",
+                           max_length=64,
+                           blank=True,
+                           help_text="""youtube视频id
+                           
+                           """
+                           )
     # author = models.TextField()
     # text = MarkdownField(rendered_field='text_rendered', use_editor=False, use_admin_editor=True,validator=VALIDATOR_STANDARD)
     # text_rendered = RenderedMarkdownField(default='')
     tags = TaggableManager("标签")
     meta_keywords = models.CharField("meta keywords",
                            max_length=128,
                            blank=True,
@@ -80,14 +86,16 @@
         # if not self.slug:
         #     self.slug = slugify(self.title)
         # self.updated_on = django.timezone.now()
         super(Post, self).save(*args, **kwargs)
 
     class Meta:
         ordering = ['-updated_on']
+        # fields=['product_id']
+
 
         def __unicode__(self):
             return self.title
         
 
 
 class AmazonSettings(SingletonModel):
```

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.8.416911164/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/article_list_by_tag.html`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,63 @@
 {% block head %}
 {% if meta.noindex %} 
 <meta name="robots" content="noindex">
 {% endif %} 
 
 {% endblock %}
 
+
 {% block body_class_expand %}tag{% endblock %}
+
+
+
+
+
+{% block top_toolbar %}
+    {% comment %} top_toolbar start {% endcomment %}
+
+     <nav class="w-full py-2 bg-zinc-800 shadow">
+        <div class="w-full container mx-auto flex flex-wrap items-center justify-between">
+
+            <nav>
+                <ul class="flex items-center justify-between font-bold text-sm text-white uppercase no-underline">
+                    <li><a class="hover:text-gray-200 hover:underline px-4" href="{% url 'home'%}">Home</a></li>
+                    <li><a class="hover:text-gray-200 hover:underline px-4"  rel="nofollow" href="{% url  'last_index' %}">Update</a></li>
+                </ul>
+            </nav>
+
+            <div class="flex items-center text-lg no-underline text-white pr-6">
+                <!-- <a class="" href="#">
+                    <i class="fab fa-facebook"></i>
+                </a>
+                <a class="pl-6" href="#">
+                    <i class="fab fa-instagram"></i>
+                </a>
+                <a class="pl-6" href="#">
+                    <i class="fab fa-twitter"></i>
+                </a>
+                <a class="pl-6" href="#">
+                    <i class="fab fa-linkedin"></i>
+                </a> -->
+            </div>
+        </div>
+
+    </nav>
+    {% comment %} top_toolbar end {% endcomment %}
+{% endblock %}
+
+
+
+
+
+
+
+
+
+
  {% block article_list %}
 
  {% for detail in object_list %}
             <article class="w-full flex flex-col shadow my-4">
                 <!-- Article Image -->
                 {%if detail.article_img%}
                 <div class="flex items-center justify-center bg-gray-100">
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
 {% extends 'blog/blog.html' %} {% load static %} {% comment %} {% extends
 'base.html' %} {% endcomment %} {% load cache %} {% load post_extras %} {%
 block title %}
 {% endblock %} {% block top_nav %} {% endblock %} {% block head %} {% if
 meta.noindex %}
  {% endif %} {% endblock %} {% block body_class_expand %}tag{% endblock %} {%
-block article_list %} {% for detail in object_list %}   {%if
-detail.article_img%}
+block top_toolbar %} {% comment %} top_toolbar start {% endcomment %}
+    * Home
+    * Update
+ {% comment %} top_toolbar end {% endcomment %} {% endblock %} {% block
+article_list %} {% for detail in object_list %}   {%if detail.article_img%}
 [{{detail.product_name}}]
 {%endif%}
 {{detail.title}}
 Published on {{detail.created_on}}
 {% cache 36000 content_truncatechars_128 detail.pk %} {
 {detail.content|truncatechars:128}} {% endcache %}
 {% cache 36000 tags detail.pk %} {% tags detail.tags 5 detail.pk %} {% endcache
```

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/amazon_link.html`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 load post_extras
 
 使用示例：
 tags object.tags.all
 
 -->
 {% load cache %}
-{% cache 36000 amazon_link_block pk %}
+{% cache 36000 amazon_link_block product_id %}
 
 <div class="amazon_link">
     
     <div class="flex flex-wrap">
      
         {%if product_id and store_id %}
```

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/tags.html` & `django_tbase_post_product-2023.8.416911164/tbase_post/templates/post/extras/tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.8.416911164/tbase_post/templatetags/post_extras.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,18 +32,28 @@
 
 
     """
     return {
         "product_id":product_id,
         "store_id":store_id,
         "product_name":product_name,
-        "link":f"https://www.amazon.com/dp/{product_id}/?tag={store_id}",
+        "link": f"/post/amz/{product_id}/" 
     }
 
+# 生成亚马逊推广的banner链接
+@register.simple_tag(takes_context=False)
+# @register.inclusion_tag("post/extras/amazon_link.html", takes_context=False)
+def amazon_base_link(product_id=None,product_name=None,store_id=None, *args, **kwargs):
+    """
+     生成亚马逊推广的banner链接
 
+
+    """
+    # return f"https://www.amazon.com/dp/{product_id}/?tag={store_id}" 
+    return f"/post/amz/{product_id}/" 
 def tags_with_count(tags):
     """
     将标签数量添加到每个标签对象中
     """
     key = "-".join(list(tags.slugs()))
     key=f'tags_with_count_{key}'
     # print("key",key)
@@ -119,15 +129,15 @@
         if i>limit:
             break
         # if items_with_count[item.pk]<10:
             
         items.append({
             'name':item.name,
             'pk':item.pk,
-            'count':items_with_count[item.pk],
+            'count':items_with_count.get(item.pk),
             'object':item
 
         })
         i=i+1
 
     # print("tags", context)
     key = "-".join(list(tags.slugs()))
@@ -217,8 +227,26 @@
         return {
             'state': False,
             'link': "context['home_link']",
             'title': "Last Update",
             "page_obj": [],
             "pk":"last_update"
             # "content": context
-        }
+        }
+    
+
+
+# 生成亚马逊推广的banner链接
+@register.filter
+@register.inclusion_tag("post/extras/youtube_player.html", takes_context=False)
+def youtube_player(youtube_id=None,product_name=None,store_id=None, *args, **kwargs):
+    """
+     生成亚马逊推广的banner链接
+
+
+    """
+    return {
+        "youtube_id":youtube_id,
+        # "store_id":store_id,
+        # "product_name":product_name,
+        "link":f"https://www.youtube-nocookie.com/embed/{youtube_id}",
+    }
```

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/urls.py` & `django_tbase_post_product-2023.8.416911164/tbase_post/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from .sitemaps import PostSitemap
 from . import views
 sitemaps = {
     'posts': PostSitemap,
 }
 urlpatterns = [
     path('', cache_page(60 * 15)(views.IndexView.as_view()), name='detail_index'),
+    path('last', cache_page(10 * 1)(views.LastUpdateView.as_view()), name='last_index'),
     path('detail/<int:pk>/', cache_page(60 * 15)(views.DetailView.as_view()), name='detail_view'),
     path('tag/<int:pk>/',
          cache_page(60 * 60)(views.TagListView.as_view()),
          name='article_list_by_tag'),
+    path('amz/<str:id>/', views.amazon_go, name='amz_go'),
     path('sitemap.xml', 
          sitemap, 
          {'sitemaps': sitemaps}, 
          name='django.contrib.sitemaps.views.sitemap'),  # 网站地图 
     # path('detail/<int:pk>', views.DetailView.as_view(), name='post_view'),
     # path('<int:pk>/', views.PostView.as_view(), name='post'),
 ]
```

### Comparing `django_tbase_post_product-2023.7.716887389/tbase_post/views.py` & `django_tbase_post_product-2023.8.416911164/tbase_post/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from django.shortcuts import render
 from django.views import View
 
 # Create your views here.
 from django.http import HttpResponse, Http404
+from django.http import HttpResponseRedirect
 
+from urllib.parse import urlencode
 from taggit.models import TaggedItem
 from taggit.models import Tag
 from django.views.generic.base import TemplateView
 from django.views import generic
 from django.views.decorators.cache import cache_page
 # from django.core.cache import caches
 from django.core.cache import cache
@@ -28,15 +30,15 @@
     template_name = 'post/detail.html'
     # context_object_name = 'post'
     # def get(request, pk):
     #     """Return the last five published questions."""
     #     return Post.objects.get(id=pk)
     model = models.Post
     context_object_name = 'detail'
-    ordering = ['-created_on']
+    ordering = ['-updated_on']
     # # 控制访问权限
     # @method_decorator(login_required)
     # @method_decorator(permission_required('dashboard.view_server'))
     # def get(self, request, *args, **kwargs):
     #     print("kwargs", kwargs)
     #     # context = self.model.objects.get(id=pk)
     #     context = super().get_context_data(**kwargs)
@@ -57,37 +59,63 @@
 
     # def get(self, request, *args, **kwargs):
     #     return HttpResponse('Hello, World! index')
 
     template_name = 'post/blog_index.html'
     model = models.Post
     paginate_by = 10
-    ordering = ['-created_on']
+    ordering = ['-updated_on']
 
 
     # context_object_name = 'model_list'
     # def get(self, request, *args, **kwargs):
     #     return HttpResponse('Hello, World! index')
     #     # return {}
     def get_context_data(self, *args, **kwargs):
         # print("kwargs",kwargs)
         # context = Post.objects.get(id=pk)
         context = super().get_context_data(**kwargs)
         # context['now'] = timezone.now()
         # context['title'] = "Post Details"
         # print(context)
         return context
+# @cache_page(60*2)
+class LastUpdateView(generic.ListView):
+    """
+    最后更新页面
+    """
+
+    # def get(self, request, *args, **kwargs):
+    #     return HttpResponse('Hello, World! index')
+
+    template_name = 'post/last_index.html'
+    model = models.Post
+    paginate_by = 200
+    ordering = ['-updated_on']
+
 
+    # context_object_name = 'model_list'
+    # def get(self, request, *args, **kwargs):
+    #     return HttpResponse('Hello, World! index')
+    #     # return {}
+    def get_context_data(self, *args, **kwargs):
+        # print("kwargs",kwargs)
+        # context = Post.objects.get(id=pk)
+        context = super().get_context_data(**kwargs)
+        # context['now'] = timezone.now()
+        # context['title'] = "Post Details"
+        # print(context)
+        return context
 # @cache_page(60*60)
 class TagListView(generic.ListView):
     model = models.Post
     template_name = 'post/article_list_by_tag.html'
     context_object_name = 'posts'
     paginate_by = 20
-    ordering = ['-created_on']
+    ordering = ['-updated_on']
     def get_queryset(self):
         # retrieve the tag from the URL
         tag_slug = self.kwargs['pk']
 
         key=f'article_tag_{tag_slug}'
         articles=cache.get(key)
         if articles is not None: 
@@ -124,8 +152,29 @@
             # return Http404('project list dose not exist')
             # return View.defaults.page_not_found()
             # raise Http404("Poll does not exist")
         else:
             context['meta'] = {
             'noindex':False
              }
-        return context
+        return context
+    
+
+def amazon_go(request,id):
+    """
+    
+    跳转到亚马逊
+    
+    """
+ 
+    response = HttpResponse("", status=302)
+    querydict={}
+
+    amazon=models.AmazonSettings()
+    a=amazon.get_solo()
+
+    querydict['tag']=a.store_id
+
+    # print(querydict)
+    q=urlencode(querydict)
+    response['Location'] = f"https://www.amazon.com/dp/{id}/?{q}"
+    return response
```

