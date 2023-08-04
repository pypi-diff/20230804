# Comparing `tmp/click-default-group-1.2.2.tar.gz` & `tmp/click_default_group-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/click-default-group-1.2.2.tar", last modified: Thu Sep  5 02:49:08 2019, max compression
+gzip compressed data, was "click_default_group-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `click-default-group-1.2.2.tar` & `click_default_group-1.2.3.tar`

### file list

```diff
@@ -1,12 +1,5 @@
-drwxrwxr-x   0 sub       (1006) sub       (1006)        0 2019-09-05 02:49:08.000000 click-default-group-1.2.2/
--rw-rw-r--   0 sub       (1006) sub       (1006)     3113 2019-09-05 02:49:08.000000 click-default-group-1.2.2/PKG-INFO
--rw-rw-r--   0 sub       (1006) sub       (1006)     1573 2019-06-14 07:42:16.000000 click-default-group-1.2.2/README.md
-drwxrwxr-x   0 sub       (1006) sub       (1006)        0 2019-09-05 02:49:08.000000 click-default-group-1.2.2/click_default_group.egg-info/
--rw-rw-r--   0 sub       (1006) sub       (1006)     3113 2019-09-05 02:49:08.000000 click-default-group-1.2.2/click_default_group.egg-info/PKG-INFO
--rw-rw-r--   0 sub       (1006) sub       (1006)      265 2019-09-05 02:49:08.000000 click-default-group-1.2.2/click_default_group.egg-info/SOURCES.txt
--rw-rw-r--   0 sub       (1006) sub       (1006)        1 2019-09-05 02:49:08.000000 click-default-group-1.2.2/click_default_group.egg-info/dependency_links.txt
--rw-rw-r--   0 sub       (1006) sub       (1006)        6 2019-09-05 02:49:08.000000 click-default-group-1.2.2/click_default_group.egg-info/requires.txt
--rw-rw-r--   0 sub       (1006) sub       (1006)       20 2019-09-05 02:49:08.000000 click-default-group-1.2.2/click_default_group.egg-info/top_level.txt
--rw-rw-r--   0 sub       (1006) sub       (1006)     3926 2019-09-05 02:48:38.000000 click-default-group-1.2.2/click_default_group.py
--rw-rw-r--   0 sub       (1006) sub       (1006)      175 2019-09-05 02:49:08.000000 click-default-group-1.2.2/setup.cfg
--rw-rw-r--   0 sub       (1006) sub       (1006)     1661 2019-09-05 02:46:21.000000 click-default-group-1.2.2/setup.py
+-rw-r--r--   0        0        0     1495 2023-08-04 07:26:25.351242 click_default_group-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1576 2023-08-04 07:16:48.738963 click_default_group-1.2.3/README.md
+-rw-r--r--   0        0        0     3902 2023-08-04 07:14:31.106893 click_default_group-1.2.3/click_default_group.py
+-rw-r--r--   0        0        0     1219 2023-08-04 07:30:20.863321 click_default_group-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 click_default_group-1.2.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `click-default-group-1.2.2/PKG-INFO` & `click_default_group-1.2.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,102 @@
 Metadata-Version: 2.1
 Name: click-default-group
-Version: 1.2.2
-Summary: Extends click.Group to invoke a command without explicit subcommand name
-Home-page: https://github.com/sublee/click-default-group/
-Author: Heungsub Lee
-Author-email: sub@subl.ee
-License: BSD
-Description: Click Default Group
-        ===================
-        
-        `DefaultGroup` is a sub class of [`click.Group`](http://click.pocoo.org/6/api/#click.Group).  But it invokes a default
-        subcommand instead of showing a help message when a subcommand is not passed.
-        
-        [![Build Status](https://img.shields.io/travis/click-contrib/click-default-group.svg)](https://travis-ci.org/click-contrib/click-default-group)
-        [![Coverage Status](https://img.shields.io/coveralls/click-contrib/click-default-group.svg)](https://coveralls.io/r/click-contrib/click-default-group)
-        
-        Usage
-        -----
-        
-        Define a default subcommand by `default=NAME`:
-        
-        ```python
-        import click
-        from click_default_group import DefaultGroup
-        
-        @click.group(cls=DefaultGroup, default='foo', default_if_no_args=True)
-        def cli():
-            pass
-        
-        @cli.command()
-        def foo():
-            click.echo('foo')
-        
-        @cli.command()
-        def bar():
-            click.echo('bar')
-        ```
-        
-        Then you can invoke that without explicit subcommand name:
-        
-        ```console
-        $ cli.py --help
-        Usage: cli.py [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          --help    Show this message and exit.
-        
-        Command:
-          foo*
-          bar
-        
-        $ cli.py
-        foo
-        $ cli.py foo
-        foo
-        $ cli.py bar
-        bar
-        ```
-        
-        Compatibility
-        -------------
-        
-        `click-default-group` is compatible with these Click versions:
-        
-        - Click-7.0
-        - Click-6.x
-        - Click-5.1
-        - Click-5.0
-        - Click-4.1
-        - Click-4.0
-        
-        See the [latest build status](https://travis-ci.org/click-contrib/click-default-group)
-        at Travis CI.
-        
-        Licensing
-        ---------
-        
-        Written by [Heungsub Lee], and distributed under the [BSD 3-Clause] license.
-        
-        [Heungsub Lee]: http://subl.ee/
-        [BSD 3-Clause]: http://opensource.org/licenses/BSD-3-Clause
-        
-Platform: any
+Version: 1.2.3
+Summary: click_default_group
+Author-email: Heungsub Lee <heungsub@subl.ee>
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
+Requires-Dist: pytest ; extra == "test"
+Project-URL: Source, https://github.com/click-contrib/click-default-group
+Provides-Extra: test
+
+Click Default Group
+===================
+
+`DefaultGroup` is a sub class of [`click.Group`](https://click.pocoo.org/6/api/#click.Group).  But it invokes a default
+subcommand instead of showing a help message when a subcommand is not passed.
+
+[![Build Status](https://img.shields.io/travis/click-contrib/click-default-group.svg)](https://travis-ci.org/click-contrib/click-default-group)
+[![Coverage Status](https://img.shields.io/coveralls/click-contrib/click-default-group.svg)](https://coveralls.io/r/click-contrib/click-default-group)
+
+Usage
+-----
+
+Define a default subcommand by `default=NAME`:
+
+```python
+import click
+from click_default_group import DefaultGroup
+
+@click.group(cls=DefaultGroup, default='foo', default_if_no_args=True)
+def cli():
+    pass
+
+@cli.command()
+def foo():
+    click.echo('foo')
+
+@cli.command()
+def bar():
+    click.echo('bar')
+```
+
+Then you can invoke that without explicit subcommand name:
+
+```console
+$ cli.py --help
+Usage: cli.py [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help    Show this message and exit.
+
+Command:
+  foo*
+  bar
+
+$ cli.py
+foo
+$ cli.py foo
+foo
+$ cli.py bar
+bar
+```
+
+Compatibility
+-------------
+
+`click-default-group` is compatible with these Click versions:
+
+- Click-7.0
+- Click-6.x
+- Click-5.1
+- Click-5.0
+- Click-4.1
+- Click-4.0
+
+See the [latest build status](https://travis-ci.org/click-contrib/click-default-group)
+at Travis CI.
+
+Licensing
+---------
+
+Written by [Heungsub Lee], and distributed under the [BSD 3-Clause] license.
+
+[Heungsub Lee]: https://subl.ee/
+[BSD 3-Clause]: https://opensource.org/licenses/BSD-3-Clause
+
```

### Comparing `click-default-group-1.2.2/README.md` & `click_default_group-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Click Default Group
 ===================
 
-`DefaultGroup` is a sub class of [`click.Group`](http://click.pocoo.org/6/api/#click.Group).  But it invokes a default
+`DefaultGroup` is a sub class of [`click.Group`](https://click.pocoo.org/6/api/#click.Group).  But it invokes a default
 subcommand instead of showing a help message when a subcommand is not passed.
 
 [![Build Status](https://img.shields.io/travis/click-contrib/click-default-group.svg)](https://travis-ci.org/click-contrib/click-default-group)
 [![Coverage Status](https://img.shields.io/coveralls/click-contrib/click-default-group.svg)](https://coveralls.io/r/click-contrib/click-default-group)
 
 Usage
 -----
@@ -66,9 +66,9 @@
 at Travis CI.
 
 Licensing
 ---------
 
 Written by [Heungsub Lee], and distributed under the [BSD 3-Clause] license.
 
-[Heungsub Lee]: http://subl.ee/
-[BSD 3-Clause]: http://opensource.org/licenses/BSD-3-Clause
+[Heungsub Lee]: https://subl.ee/
+[BSD 3-Clause]: https://opensource.org/licenses/BSD-3-Clause
```

### Comparing `click-default-group-1.2.2/click_default_group.py` & `click_default_group-1.2.3/click_default_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
    click_default_group
    ~~~~~~~~~~~~~~~~~~~
 
    Define a default subcommand by `default=True`:
 
    .. sourcecode:: python
@@ -46,15 +45,15 @@
 """
 import warnings
 
 import click
 
 
 __all__ = ['DefaultGroup']
-__version__ = '1.2.2'
+__version__ = '1.2.3'
 
 
 class DefaultGroup(click.Group):
     """Invokes a subcommand marked with `default=True` if any subcommand not
     chosen.
 
     :param default_if_no_args: resolves to the default command if no arguments
```

