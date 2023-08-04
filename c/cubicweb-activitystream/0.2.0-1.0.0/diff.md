# Comparing `tmp/cubicweb-activitystream-0.2.0.tar.gz` & `tmp/cubicweb-activitystream-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-activitystream-0.2.0.tar", last modified: Thu Jul 18 10:14:54 2019, max compression
+gzip compressed data, was "cubicweb-activitystream-1.0.0.tar", last modified: Fri Aug  4 13:27:19 2023, max compression
```

## Comparing `cubicweb-activitystream-0.2.0.tar` & `cubicweb-activitystream-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      342 2019-06-12 14:54:26.000000 cubicweb-activitystream-0.2.0/MANIFEST.in
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2666 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/setup.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     3677 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/entities.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      649 2019-07-18 10:13:52.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/__pkginfo__.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1437 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/views.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/i18n/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      246 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/i18n/fr.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      236 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/i18n/es.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      251 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/i18n/en.po
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/migration/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1069 2019-06-12 14:55:09.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/migration/postcreate.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       69 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/__init__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/data/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      271 2019-06-12 14:44:48.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream/data/cubes.activitystream.css
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      446 2019-06-12 14:54:48.000000 cubicweb-activitystream-0.2.0/tox.ini
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/setup.cfg
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       85 2019-06-04 23:36:21.000000 cubicweb-activitystream-0.2.0/README
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      581 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/PKG-INFO
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/test/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      239 2019-06-13 07:01:34.000000 cubicweb-activitystream-0.2.0/test/test_activitystream.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       59 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       24 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/top_level.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      744 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       15 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      581 2019-07-18 10:14:54.000000 cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/PKG-INFO
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      407 2023-08-04 12:35:34.000000 cubicweb-activitystream-1.0.0/MANIFEST.in
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      502 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       85 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/README.rst
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:27:19.066744 cubicweb-activitystream-1.0.0/cubicweb_activitystream/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       69 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/__init__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      705 2023-08-04 12:35:34.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/__pkginfo__.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/cubicweb_activitystream/data/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      271 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/data/cubes.activitystream.css
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     3679 2023-05-04 09:19:16.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/entities.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/cubicweb_activitystream/i18n/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      251 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/i18n/en.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      236 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/i18n/es.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      246 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/i18n/fr.po
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/cubicweb_activitystream/migration/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1069 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/migration/postcreate.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1441 2023-05-04 09:19:29.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream/views.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      502 2023-08-04 13:27:18.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      748 2023-08-04 13:27:18.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/SOURCES.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-08-04 13:27:18.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/dependency_links.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       58 2023-08-04 13:27:18.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/entry_points.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-05-04 09:17:30.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/not-zip-safe
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       50 2023-08-04 13:27:18.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/requires.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       24 2023-08-04 13:27:18.000000 cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/top_level.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       38 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/setup.cfg
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2670 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/setup.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-08-04 13:27:19.070744 cubicweb-activitystream-1.0.0/test/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      239 2023-05-04 09:15:53.000000 cubicweb-activitystream-1.0.0/test/test_activitystream.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1116 2023-08-04 13:26:26.000000 cubicweb-activitystream-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-activitystream-0.2.0/setup.py` & `cubicweb-activitystream-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 license = __pkginfo__['license']
 description = __pkginfo__['description']
 web = __pkginfo__['web']
 author = __pkginfo__['author']
 author_email = __pkginfo__['author_email']
 classifiers = __pkginfo__['classifiers']
 
-with open(join(here, 'README')) as f:
+with open(join(here, 'README.rst')) as f:
     long_description = f.read()
 
 # get optional metadatas
 data_files = __pkginfo__.get('data_files', None)
 dependency_links = __pkginfo__.get('dependency_links', ())
 
 requires = {}
```

### Comparing `cubicweb-activitystream-0.2.0/cubicweb_activitystream/entities.py` & `cubicweb-activitystream-1.0.0/cubicweb_activitystream/entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 """cubicweb-activitystream adapters"""
 
 from cubicweb.predicates import is_instance, adaptable
-from cubicweb.view import EntityAdapter
 from cubicweb.appobject import AppObject
+from cubicweb.entity import EntityAdapter
 
 
 class IActivityStreamAdapter(EntityAdapter):
     __regid__ = 'IActivityStream'
     __abstract__ = True
 
     @property
```

### Comparing `cubicweb-activitystream-0.2.0/cubicweb_activitystream/__pkginfo__.py` & `cubicweb-activitystream-1.0.0/cubicweb_activitystream/__pkginfo__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # pylint: disable=W0622
 """cubicweb-activitystream application packaging information"""
 
 
 modname = 'cubicweb_activitystream'
 distname = 'cubicweb-activitystream'
 
-numversion = (0, 2, 0)
+numversion = (1, 0, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 author = 'LOGILAB S.A. (Paris, FRANCE)'
 author_email = 'contact@logilab.fr'
 description = 'activity streams'
 web = 'http://www.cubicweb.org/project/%s' % distname
 
-__depends__ = {'cubicweb': '>= 3.24'}
+__depends__ = {
+    'cubicweb': '>= 4.0.0,< 5.0.0',
+    'cubicweb_web': '>= 1.0.0,< 2.0.0',
+}
 __recommends__ = {}
 
 classifiers = [
     'Environment :: Web Environment',
     'Framework :: CubicWeb',
     'Programming Language :: Python :: 3',
     'Programming Language :: JavaScript',
```

### Comparing `cubicweb-activitystream-0.2.0/cubicweb_activitystream/views.py` & `cubicweb-activitystream-1.0.0/cubicweb_activitystream/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from logilab.mtconverter import xml_escape
 from cubicweb.predicates import adaptable
-from cubicweb.view import EntityView
 from cubicweb import _
+from cubicweb_web.view import EntityView
 
 
 class AStreamView(EntityView):
     __regid__ = 'activitystream'
     __select__ = EntityView.__select__ & adaptable('IActivityStream')
     title = _('activitystream')
```

### Comparing `cubicweb-activitystream-0.2.0/cubicweb_activitystream/migration/postcreate.py` & `cubicweb-activitystream-1.0.0/cubicweb_activitystream/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-activitystream-0.2.0/cubicweb_activitystream.egg-info/SOURCES.txt` & `cubicweb-activitystream-1.0.0/cubicweb_activitystream.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MANIFEST.in
-README
+README.rst
 setup.py
 tox.ini
 cubicweb_activitystream/__init__.py
 cubicweb_activitystream/__pkginfo__.py
 cubicweb_activitystream/entities.py
 cubicweb_activitystream/views.py
 cubicweb_activitystream.egg-info/PKG-INFO
```

