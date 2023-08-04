# Comparing `tmp/pytest-reana-0.9.0a7.tar.gz` & `tmp/pytest-reana-0.9.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reana-0.9.0a7.tar", last modified: Fri Nov 25 12:43:50 2022, max compression
+gzip compressed data, was "pytest-reana-0.9.1a1.tar", last modified: Fri Aug  4 09:45:33 2023, max compression
```

## Comparing `pytest-reana-0.9.0a7.tar` & `pytest-reana-0.9.1a1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.247019 pytest-reana-0.9.0a7/
--rw-r--r--   0 madonado   (501) staff       (20)      272 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/.flake8
--rw-r--r--   0 madonado   (501) staff       (20)      600 2022-05-17 13:12:56.000000 pytest-reana-0.9.0a7/AUTHORS.rst
--rw-r--r--   0 madonado   (501) staff       (20)     2501 2022-11-14 14:24:28.000000 pytest-reana-0.9.0a7/CHANGES.rst
--rw-r--r--   0 madonado   (501) staff       (20)      675 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/CONTRIBUTING.rst
--rw-r--r--   0 madonado   (501) staff       (20)     1086 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/LICENSE
--rw-r--r--   0 madonado   (501) staff       (20)      649 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/MANIFEST.in
--rw-r--r--   0 madonado   (501) staff       (20)     5766 2022-11-25 12:43:50.247133 pytest-reana-0.9.0a7/PKG-INFO
--rw-r--r--   0 madonado   (501) staff       (20)     2134 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/README.rst
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.242454 pytest-reana-0.9.0a7/docs/
--rw-r--r--   0 madonado   (501) staff       (20)     6175 2022-06-14 12:37:19.000000 pytest-reana-0.9.0a7/docs/conf.py
--rw-r--r--   0 madonado   (501) staff       (20)      687 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/docs/index.rst
--rw-r--r--   0 madonado   (501) staff       (20)      210 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/docs/requirements.txt
--rw-r--r--   0 madonado   (501) staff       (20)      333 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/pytest.ini
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.243871 pytest-reana-0.9.0a7/pytest_reana/
--rw-r--r--   0 madonado   (501) staff       (20)      376 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/pytest_reana/__init__.py
--rw-r--r--   0 madonado   (501) staff       (20)    29651 2022-05-17 13:12:56.000000 pytest-reana-0.9.0a7/pytest_reana/fixtures.py
--rw-r--r--   0 madonado   (501) staff       (20)      989 2022-05-17 13:12:56.000000 pytest-reana-0.9.0a7/pytest_reana/plugin.py
--rw-r--r--   0 madonado   (501) staff       (20)     1023 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/pytest_reana/test_utils.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.238116 pytest-reana-0.9.0a7/pytest_reana/test_workspace/
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.245874 pytest-reana-0.9.0a7/pytest_reana/test_workspace/code/
--rw-r--r--   0 madonado   (501) staff       (20)    19221 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/pytest_reana/test_workspace/code/worldpopulation.ipynb
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.246151 pytest-reana-0.9.0a7/pytest_reana/test_workspace/data/
--rw-r--r--   0 madonado   (501) staff       (20)      574 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/pytest_reana/test_workspace/data/World_historical_and_predicted_populations_in_percentage.csv
--rwxr-xr-x   0 madonado   (501) staff       (20)      456 2022-11-25 12:41:57.000000 pytest-reana-0.9.0a7/pytest_reana/version.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.245575 pytest-reana-0.9.0a7/pytest_reana.egg-info/
--rw-r--r--   0 madonado   (501) staff       (20)     5766 2022-11-25 12:43:50.000000 pytest-reana-0.9.0a7/pytest_reana.egg-info/PKG-INFO
--rw-r--r--   0 madonado   (501) staff       (20)      769 2022-11-25 12:43:50.000000 pytest-reana-0.9.0a7/pytest_reana.egg-info/SOURCES.txt
--rw-r--r--   0 madonado   (501) staff       (20)        1 2022-11-25 12:43:50.000000 pytest-reana-0.9.0a7/pytest_reana.egg-info/dependency_links.txt
--rw-r--r--   0 madonado   (501) staff       (20)       39 2022-11-25 12:43:50.000000 pytest-reana-0.9.0a7/pytest_reana.egg-info/entry_points.txt
--rw-r--r--   0 madonado   (501) staff       (20)        1 2022-11-25 12:43:50.000000 pytest-reana-0.9.0a7/pytest_reana.egg-info/not-zip-safe
--rw-r--r--   0 madonado   (501) staff       (20)      485 2022-11-25 12:43:50.000000 pytest-reana-0.9.0a7/pytest_reana.egg-info/requires.txt
--rw-r--r--   0 madonado   (501) staff       (20)       13 2022-11-25 12:43:50.000000 pytest-reana-0.9.0a7/pytest_reana.egg-info/top_level.txt
--rwxr-xr-x   0 madonado   (501) staff       (20)     1173 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/run-tests.sh
--rw-r--r--   0 madonado   (501) staff       (20)      136 2022-11-25 12:43:50.247579 pytest-reana-0.9.0a7/setup.cfg
--rwxr-xr-x   0 madonado   (501) staff       (20)     2959 2022-11-14 14:24:28.000000 pytest-reana-0.9.0a7/setup.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-11-25 12:43:50.246821 pytest-reana-0.9.0a7/tests/
--rw-r--r--   0 madonado   (501) staff       (20)      358 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/tests/conftest.py
--rw-r--r--   0 madonado   (501) staff       (20)      803 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/tests/test_fixtures.py
--rw-r--r--   0 madonado   (501) staff       (20)      447 2022-03-25 14:10:35.000000 pytest-reana-0.9.0a7/tests/test_version.py
--rw-r--r--   0 madonado   (501) staff       (20)      333 2022-11-14 14:24:28.000000 pytest-reana-0.9.0a7/tox.ini
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.742490 pytest-reana-0.9.1a1/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      272 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/.flake8
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      600 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/AUTHORS.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2663 2023-08-04 09:44:10.000000 pytest-reana-0.9.1a1/CHANGES.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      675 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/CONTRIBUTING.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1086 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/LICENSE
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      675 2023-06-29 13:00:05.000000 pytest-reana-0.9.1a1/MANIFEST.in
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     5928 2023-08-04 09:45:33.742490 pytest-reana-0.9.1a1/PKG-INFO
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     2134 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/README.rst
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.738490 pytest-reana-0.9.1a1/docs/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     6175 2023-06-29 13:00:05.000000 pytest-reana-0.9.1a1/docs/conf.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      687 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/docs/index.rst
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      210 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/docs/requirements.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      333 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/pytest.ini
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.739490 pytest-reana-0.9.1a1/pytest_reana/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      376 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/pytest_reana/__init__.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    29643 2023-06-29 13:00:05.000000 pytest-reana-0.9.1a1/pytest_reana/fixtures.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      989 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/pytest_reana/plugin.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     1022 2023-06-29 13:00:05.000000 pytest-reana-0.9.1a1/pytest_reana/test_utils.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.736490 pytest-reana-0.9.1a1/pytest_reana/test_workspace/
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.740491 pytest-reana-0.9.1a1/pytest_reana/test_workspace/code/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)    19221 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/pytest_reana/test_workspace/code/worldpopulation.ipynb
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.741490 pytest-reana-0.9.1a1/pytest_reana/test_workspace/data/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      574 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/pytest_reana/test_workspace/data/World_historical_and_predicted_populations_in_percentage.csv
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)      456 2023-08-04 09:44:10.000000 pytest-reana-0.9.1a1/pytest_reana/version.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.740491 pytest-reana-0.9.1a1/pytest_reana.egg-info/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)     5928 2023-08-04 09:45:33.000000 pytest-reana-0.9.1a1/pytest_reana.egg-info/PKG-INFO
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      769 2023-08-04 09:45:33.000000 pytest-reana-0.9.1a1/pytest_reana.egg-info/SOURCES.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-08-04 09:45:33.000000 pytest-reana-0.9.1a1/pytest_reana.egg-info/dependency_links.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)       39 2023-08-04 09:45:33.000000 pytest-reana-0.9.1a1/pytest_reana.egg-info/entry_points.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)        1 2023-08-04 09:45:33.000000 pytest-reana-0.9.1a1/pytest_reana.egg-info/not-zip-safe
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      509 2023-08-04 09:45:33.000000 pytest-reana-0.9.1a1/pytest_reana.egg-info/requires.txt
+-rw-r--r--   0 madonado  (1000) madonado  (1000)       13 2023-08-04 09:45:33.000000 pytest-reana-0.9.1a1/pytest_reana.egg-info/top_level.txt
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)     1173 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/run-tests.sh
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      136 2023-08-04 09:45:33.742490 pytest-reana-0.9.1a1/setup.cfg
+-rwxr-xr-x   0 madonado  (1000) madonado  (1000)     3047 2023-08-04 09:44:10.000000 pytest-reana-0.9.1a1/setup.py
+drwxr-xr-x   0 madonado  (1000) madonado  (1000)        0 2023-08-04 09:45:33.741490 pytest-reana-0.9.1a1/tests/
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      358 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/tests/conftest.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      803 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/tests/test_fixtures.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      447 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/tests/test_version.py
+-rw-r--r--   0 madonado  (1000) madonado  (1000)      333 2023-06-22 07:53:52.000000 pytest-reana-0.9.1a1/tox.ini
```

### Comparing `pytest-reana-0.9.0a7/AUTHORS.rst` & `pytest-reana-0.9.1a1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/CHANGES.rst` & `pytest-reana-0.9.1a1/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Changes
 =======
 
-Version 0.9.0 (UNRELEASED)
+Version 0.9.1 (UNRELEASED)
 --------------------------
 
-- Adds fixture providing the secrets needed by Kerberos.
+- Changes ``apispec`` dependency version in order to be compatible with ``PyYAML`` v6.
+
+Version 0.9.0 (2022-12-13)
+--------------------------
+
+- Adds fixture providing example of user secrets needed for Kerberos tests.
 - Adds support for Python 3.11.
 - Fixes location of Celery docs for ReadTheDocs pages.
 - Removes hard-dependency on `black` code formatter version.
 
 Version 0.8.1 (2022-01-05)
 --------------------------
```

### Comparing `pytest-reana-0.9.0a7/CONTRIBUTING.rst` & `pytest-reana-0.9.1a1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/LICENSE` & `pytest-reana-0.9.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/MANIFEST.in` & `pytest-reana-0.9.1a1/MANIFEST.in`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 include *.sh
 include *.yaml
 include .dockerignore
 include .flake8
 include LICENSE
 include pytest.ini
 include tox.ini
+exclude .readthedocs.yaml
 prune docs/_build
 recursive-include docs *.png
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include pytest_reana *.csv
 recursive-include pytest_reana *.ipynb
```

### Comparing `pytest-reana-0.9.0a7/PKG-INFO` & `pytest-reana-0.9.1a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reana
-Version: 0.9.0a7
+Version: 0.9.1a1
 Summary: Pytest fixtures for REANA.
 Home-page: https://github.com/reanahub/pytest-reana
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -88,18 +88,23 @@
 - `pytest-REANA known issues <https://github.com/reanahub/pytest-reana/issues>`_
 - `pytest-REANA source code <https://github.com/reanahub/pytest-reana>`_
 
 
 Changes
 =======
 
-Version 0.9.0 (UNRELEASED)
+Version 0.9.1 (UNRELEASED)
 --------------------------
 
-- Adds fixture providing the secrets needed by Kerberos.
+- Changes ``apispec`` dependency version in order to be compatible with ``PyYAML`` v6.
+
+Version 0.9.0 (2022-12-13)
+--------------------------
+
+- Adds fixture providing example of user secrets needed for Kerberos tests.
 - Adds support for Python 3.11.
 - Fixes location of Celery docs for ReadTheDocs pages.
 - Removes hard-dependency on `black` code formatter version.
 
 Version 0.8.1 (2022-01-05)
 --------------------------
```

### Comparing `pytest-reana-0.9.0a7/README.rst` & `pytest-reana-0.9.1a1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/docs/conf.py` & `pytest-reana-0.9.1a1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,9 +193,9 @@
         "One line description of project.",
         "Miscellaneous",
     ),
 ]
 
 # Intersphinx configuration
 intersphinx_mapping = {
-    "kombu": ("https://docs.celeryq.dev/projects/kombu/en/latest/", None),
+    "kombu": ("https://docs.celeryq.dev/projects/kombu/en/stable/", None),
 }
```

#### html2text {}

```diff
@@ -70,8 +70,8 @@
 manual section). man_pages = [(master_doc, "reana", "reana Documentation",
 [author], 1)] # -- Options for Texinfo output ---------------------------------
 ---------- # Grouping the document tree into Texinfo files. List of tuples #
 (source start file, target name, title, author, # dir menu entry, description,
 category) texinfo_documents = [ ( master_doc, "reana", "reana Documentation",
 author, "reana", "One line description of project.", "Miscellaneous", ), ] #
 Intersphinx configuration intersphinx_mapping = { "kombu": ("https://
-docs.celeryq.dev/projects/kombu/en/latest/", None), }
+docs.celeryq.dev/projects/kombu/en/stable/", None), }
```

### Comparing `pytest-reana-0.9.0a7/docs/index.rst` & `pytest-reana-0.9.1a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/pytest_reana/fixtures.py` & `pytest-reana-0.9.1a1/pytest_reana/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,15 +603,15 @@
             consume_queue(consumer, limit=1)
 
     """
 
     def _consume_queue(consumer, limit=None):
         """Consume AMQP queue.
 
-        :param consumer: A :class:`kombu.Consumer` to consume from.
+        :param consumer: A class:`kombu.Consumer` to consume from.
         :param limit: Integer which represents how many items to consume
             from the queue, if not specified, the consume method will run
             uninterruptedly.
         """
         consumer_generator = consumer.consume(limit=limit)
         while True:
             try:
@@ -625,15 +625,15 @@
 
 @pytest.fixture(scope="session")
 def in_memory_queue_connection():
     """In memory message queue.
 
     Scope: session
 
-    This fixture offers an in memory :class:`kombu.Connection` scoped to the
+    This fixture offers an in memory class:`kombu.Connection` scoped to the
     testing session.
 
     .. code-block:: python
 
         def test_something(ConsumerBase, in_memory_queue_connection):
             consumer = ConsumerBase(connection=in_memory_queue_connection)
             # Now you have a consumer connected to an in memory queue
@@ -641,43 +641,43 @@
 
     """
     return Connection("memory:///")
 
 
 @pytest.fixture
 def default_exchange():
-    """Return a default :class:`kombu.Exchange` created from configuration.
+    """Return a default class:`kombu.Exchange` created from configuration.
 
     Scope: function
 
-    This fixture offers a default :class:`kombu.Exchange`.
+    This fixture offers a default class:`kombu.Exchange`.
     """
     return Exchange("test-exchange", type="direct")
 
 
 @pytest.fixture
 def default_queue(default_exchange):
-    """Return a default :class:`kombu.Queue` created from configuration.
+    """Return a default class:`kombu.Queue` created from configuration.
 
     Scope: function
 
-    This fixture offers a default :class:`kombu.Queue`.
+    This fixture offers a default class:`kombu.Queue`.
     """
     return Queue(
         "test-queue", exchange=default_exchange, routing_key="test-routing-key"
     )
 
 
 @pytest.fixture
 def default_in_memory_producer(in_memory_queue_connection, default_exchange):
-    """Rerturn a :class:`kombu.Producer` connected to in memory queue.
+    """Rerturn a class:`kombu.Producer` connected to in memory queue.
 
     Scope: function
 
-    This fixture offers a default :class:`kombu.Producer` instantiated using
+    This fixture offers a default class:`kombu.Producer` instantiated using
     the ``in_memory_queue_connection``.
 
     .. code-block:: python
 
         def test_publish_hello(default_in_memory_producer, default_queue):
             msg = {'hello': 'ninja turtle'}
             default_in_memory_producer.publish(msg,
```

### Comparing `pytest-reana-0.9.0a7/pytest_reana/plugin.py` & `pytest-reana-0.9.1a1/pytest_reana/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/pytest_reana/test_utils.py` & `pytest-reana-0.9.1a1/pytest_reana/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 """REANA Pytest Commons test utilities."""
 
 from mock import Mock
 from reana_commons.api_client import BaseAPIClient
 
 
 def make_mock_api_client(component):
-
     mock_response, mock_http_response = Mock(), Mock()
     mock_response = {}
     mock_http_response.status_code = 200
     mock_http_response.raw_bytes = b"Sample downloaded data"
 
     def mock_api_client(
         mock_response=mock_response, mock_http_response=mock_http_response
```

### Comparing `pytest-reana-0.9.0a7/pytest_reana/test_workspace/code/worldpopulation.ipynb` & `pytest-reana-0.9.1a1/pytest_reana/test_workspace/code/worldpopulation.ipynb`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/pytest_reana/test_workspace/data/World_historical_and_predicted_populations_in_percentage.csv` & `pytest-reana-0.9.1a1/pytest_reana/test_workspace/data/World_historical_and_predicted_populations_in_percentage.csv`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/pytest_reana.egg-info/PKG-INFO` & `pytest-reana-0.9.1a1/pytest_reana.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reana
-Version: 0.9.0a7
+Version: 0.9.1a1
 Summary: Pytest fixtures for REANA.
 Home-page: https://github.com/reanahub/pytest-reana
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -88,18 +88,23 @@
 - `pytest-REANA known issues <https://github.com/reanahub/pytest-reana/issues>`_
 - `pytest-REANA source code <https://github.com/reanahub/pytest-reana>`_
 
 
 Changes
 =======
 
-Version 0.9.0 (UNRELEASED)
+Version 0.9.1 (UNRELEASED)
 --------------------------
 
-- Adds fixture providing the secrets needed by Kerberos.
+- Changes ``apispec`` dependency version in order to be compatible with ``PyYAML`` v6.
+
+Version 0.9.0 (2022-12-13)
+--------------------------
+
+- Adds fixture providing example of user secrets needed for Kerberos tests.
 - Adds support for Python 3.11.
 - Fixes location of Celery docs for ReadTheDocs pages.
 - Removes hard-dependency on `black` code formatter version.
 
 Version 0.8.1 (2022-01-05)
 --------------------------
```

### Comparing `pytest-reana-0.9.0a7/pytest_reana.egg-info/SOURCES.txt` & `pytest-reana-0.9.1a1/pytest_reana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/run-tests.sh` & `pytest-reana-0.9.1a1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `pytest-reana-0.9.0a7/setup.py` & `pytest-reana-0.9.1a1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of REANA.
-# Copyright (C) 2018, 2019, 2020, 2021, 2022 CERN.
+# Copyright (C) 2018, 2019, 2020, 2021, 2022, 2023 CERN.
 #
 # REANA is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Pytest fixtures for REANA."""
 
 from __future__ import absolute_import, print_function
@@ -32,15 +32,17 @@
     extras_require["all"].extend(reqs)
 
 setup_requires = [
     "pytest-runner>=2.7",
 ]
 
 install_requires = [
-    "apispec>=0.21.0,<0.40",
+    # apispec>=4.0 drops support for marshmallow<3
+    "apispec[yaml]>=3.0,<4.0",
+    "apispec-webframeworks",
     "check-manifest>=0.25,<1",
     "checksumdir>=1.1.4,<1.2",
     "coverage>=5.0,<6.0",
     "jsonschema>=3.2.0,<4.0",
     "mock>=3.0,<4.0",
     "pika>=0.12.0,<0.13",
     "pydocstyle>=5.0.0,<6.0.0",
```

### Comparing `pytest-reana-0.9.0a7/tests/test_fixtures.py` & `pytest-reana-0.9.1a1/tests/test_fixtures.py`

 * *Files identical despite different names*

