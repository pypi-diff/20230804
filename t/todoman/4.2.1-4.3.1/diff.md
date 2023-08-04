# Comparing `tmp/todoman-4.2.1.tar.gz` & `tmp/todoman-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todoman-4.2.1.tar", last modified: Sat Mar 25 14:49:31 2023, max compression
+gzip compressed data, was "todoman-4.3.1.tar", last modified: Fri Aug  4 09:27:28 2023, max compression
```

## Comparing `todoman-4.2.1.tar` & `todoman-4.3.1.tar`

### file list

```diff
@@ -1,75 +1,73 @@
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.313775 todoman-4.2.1/
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.303775 todoman-4.2.1/.builds/
--rw-r--r--   0 build     (1000) build     (1001)      570 2023-03-25 14:45:16.000000 todoman-4.2.1/.builds/alpine.yml
--rw-r--r--   0 build     (1000) build     (1001)      860 2023-03-25 14:45:16.000000 todoman-4.2.1/.builds/archlinux.yml
--rw-r--r--   0 build     (1000) build     (1001)      137 2023-03-25 14:45:16.000000 todoman-4.2.1/.gitignore
--rw-r--r--   0 build     (1000) build     (1001)      753 2023-03-25 14:45:16.000000 todoman-4.2.1/.pre-commit-config.yaml
--rw-r--r--   0 build     (1000) build     (1001)     1341 2023-03-25 14:45:16.000000 todoman-4.2.1/AUTHORS.rst
--rw-r--r--   0 build     (1000) build     (1001)     8358 2023-03-25 14:45:16.000000 todoman-4.2.1/CHANGELOG.rst
--rw-r--r--   0 build     (1000) build     (1001)       51 2023-03-25 14:45:16.000000 todoman-4.2.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 build     (1000) build     (1001)      762 2023-03-25 14:45:16.000000 todoman-4.2.1/LICENCE
--rw-r--r--   0 build     (1000) build     (1001)     3175 2023-03-25 14:49:31.310442 todoman-4.2.1/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)     2284 2023-03-25 14:45:16.000000 todoman-4.2.1/README.rst
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.303775 todoman-4.2.1/bin/
--rwxr-xr-x   0 build     (1000) build     (1001)       88 2023-03-25 14:45:16.000000 todoman-4.2.1/bin/todo
--rw-r--r--   0 build     (1000) build     (1001)       13 2023-03-25 14:45:16.000000 todoman-4.2.1/codecov.yml
--rw-r--r--   0 build     (1000) build     (1001)      186 2023-03-25 14:45:16.000000 todoman-4.2.1/config.py.sample
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.300442 todoman-4.2.1/contrib/
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.300442 todoman-4.2.1/contrib/completion/
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.303775 todoman-4.2.1/contrib/completion/bash/
--rw-r--r--   0 build     (1000) build     (1001)     2472 2023-03-25 14:45:16.000000 todoman-4.2.1/contrib/completion/bash/_todo
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.303775 todoman-4.2.1/contrib/completion/zsh/
--rw-r--r--   0 build     (1000) build     (1001)     9503 2023-03-25 14:45:16.000000 todoman-4.2.1/contrib/completion/zsh/_todo
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.303775 todoman-4.2.1/docs/
--rw-r--r--   0 build     (1000) build     (1001)     7422 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/Makefile
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.303775 todoman-4.2.1/docs/examples/
--rw-r--r--   0 build     (1000) build     (1001)     2423 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/examples/conky.conf
--rw-r--r--   0 build     (1000) build     (1001)      434 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/pull_request_template.md
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.307108 todoman-4.2.1/docs/source/
--rw-r--r--   0 build     (1000) build     (1001)       33 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/changelog.rst
--rw-r--r--   0 build     (1000) build     (1001)     2282 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/conf.py
--rw-r--r--   0 build     (1000) build     (1001)     1510 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/configure.rst
--rw-r--r--   0 build     (1000) build     (1001)     5055 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/contributing.rst
--rw-r--r--   0 build     (1000) build     (1001)     1515 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/index.rst
--rw-r--r--   0 build     (1000) build     (1001)     3590 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/install.rst
--rw-r--r--   0 build     (1000) build     (1001)      101 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/licence.rst
--rw-r--r--   0 build     (1000) build     (1001)      808 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/man.rst
--rw-r--r--   0 build     (1000) build     (1001)     3526 2023-03-25 14:45:16.000000 todoman-4.2.1/docs/source/usage.rst
--rw-r--r--   0 build     (1000) build     (1001)      552 2023-03-25 14:45:16.000000 todoman-4.2.1/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1001)       58 2023-03-25 14:45:16.000000 todoman-4.2.1/requirements-dev.txt
--rw-r--r--   0 build     (1000) build     (1001)       45 2023-03-25 14:45:16.000000 todoman-4.2.1/requirements-docs.txt
--rw-r--r--   0 build     (1000) build     (1001)       38 2023-03-25 14:49:31.313775 todoman-4.2.1/setup.cfg
--rw-r--r--   0 build     (1000) build     (1001)     1641 2023-03-25 14:45:16.000000 todoman-4.2.1/setup.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.310442 todoman-4.2.1/tests/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     4588 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/conftest.py
--rw-r--r--   0 build     (1000) build     (1001)      861 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/helpers.py
--rw-r--r--   0 build     (1000) build     (1001)     3364 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_backend.py
--rw-r--r--   0 build     (1000) build     (1001)    31426 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_cli.py
--rw-r--r--   0 build     (1000) build     (1001)     4604 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_config.py
--rw-r--r--   0 build     (1000) build     (1001)     8998 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_filtering.py
--rw-r--r--   0 build     (1000) build     (1001)     6218 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_formatter.py
--rw-r--r--   0 build     (1000) build     (1001)      536 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_main.py
--rw-r--r--   0 build     (1000) build     (1001)    14775 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_model.py
--rw-r--r--   0 build     (1000) build     (1001)     7269 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_porcelain.py
--rw-r--r--   0 build     (1000) build     (1001)     4822 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_ui.py
--rw-r--r--   0 build     (1000) build     (1001)     6437 2023-03-25 14:45:16.000000 todoman-4.2.1/tests/test_widgets.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.310442 todoman-4.2.1/todoman/
--rw-r--r--   0 build     (1000) build     (1001)      133 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)       94 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/__main__.py
--rw-r--r--   0 build     (1000) build     (1001)    17396 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/cli.py
--rw-r--r--   0 build     (1000) build     (1001)     6799 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/configuration.py
--rw-r--r--   0 build     (1000) build     (1001)     1042 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/exceptions.py
--rw-r--r--   0 build     (1000) build     (1001)     9894 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/formatters.py
--rw-r--r--   0 build     (1000) build     (1001)     6488 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/interactive.py
--rw-r--r--   0 build     (1000) build     (1001)    34893 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/model.py
--rw-r--r--   0 build     (1000) build     (1001)      160 2023-03-25 14:49:31.000000 todoman-4.2.1/todoman/version.py
--rw-r--r--   0 build     (1000) build     (1001)     5359 2023-03-25 14:45:16.000000 todoman-4.2.1/todoman/widgets.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-03-25 14:49:31.310442 todoman-4.2.1/todoman.egg-info/
--rw-r--r--   0 build     (1000) build     (1001)     3175 2023-03-25 14:49:31.000000 todoman-4.2.1/todoman.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)     1248 2023-03-25 14:49:31.000000 todoman-4.2.1/todoman.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1001)        1 2023-03-25 14:49:31.000000 todoman-4.2.1/todoman.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1001)       41 2023-03-25 14:49:31.000000 todoman-4.2.1/todoman.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1001)      193 2023-03-25 14:49:31.000000 todoman-4.2.1/todoman.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1001)        8 2023-03-25 14:49:31.000000 todoman-4.2.1/todoman.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1001)      314 2023-03-25 14:45:16.000000 todoman-4.2.1/tox.ini
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.194489 todoman-4.3.1/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.187822 todoman-4.3.1/.builds/
+-rw-r--r--   0 build     (1000) build     (1001)      467 2023-08-04 09:22:58.000000 todoman-4.3.1/.builds/alpine.yml
+-rw-r--r--   0 build     (1000) build     (1001)      848 2023-08-04 09:22:58.000000 todoman-4.3.1/.builds/archlinux.yml
+-rw-r--r--   0 build     (1000) build     (1001)      137 2023-08-04 09:22:58.000000 todoman-4.3.1/.gitignore
+-rw-r--r--   0 build     (1000) build     (1001)      795 2023-08-04 09:22:58.000000 todoman-4.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 build     (1000) build     (1001)      160 2023-08-04 09:22:58.000000 todoman-4.3.1/.readthedocs.yaml
+-rw-r--r--   0 build     (1000) build     (1001)     1341 2023-08-04 09:22:58.000000 todoman-4.3.1/AUTHORS.rst
+-rw-r--r--   0 build     (1000) build     (1001)     8620 2023-08-04 09:22:58.000000 todoman-4.3.1/CHANGELOG.rst
+-rw-r--r--   0 build     (1000) build     (1001)       51 2023-08-04 09:22:58.000000 todoman-4.3.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 build     (1000) build     (1001)      762 2023-08-04 09:22:58.000000 todoman-4.3.1/LICENCE
+-rw-r--r--   0 build     (1000) build     (1001)     3521 2023-08-04 09:27:28.194489 todoman-4.3.1/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)     2284 2023-08-04 09:22:58.000000 todoman-4.3.1/README.rst
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.187822 todoman-4.3.1/bin/
+-rwxr-xr-x   0 build     (1000) build     (1001)       88 2023-08-04 09:22:58.000000 todoman-4.3.1/bin/todo
+-rw-r--r--   0 build     (1000) build     (1001)       13 2023-08-04 09:22:58.000000 todoman-4.3.1/codecov.yml
+-rw-r--r--   0 build     (1000) build     (1001)      186 2023-08-04 09:22:58.000000 todoman-4.3.1/config.py.sample
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.184489 todoman-4.3.1/contrib/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.184489 todoman-4.3.1/contrib/completion/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.187822 todoman-4.3.1/contrib/completion/bash/
+-rw-r--r--   0 build     (1000) build     (1001)     2472 2023-08-04 09:22:58.000000 todoman-4.3.1/contrib/completion/bash/_todo
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.187822 todoman-4.3.1/contrib/completion/zsh/
+-rw-r--r--   0 build     (1000) build     (1001)    10052 2023-08-04 09:22:58.000000 todoman-4.3.1/contrib/completion/zsh/_todo
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.187822 todoman-4.3.1/docs/
+-rw-r--r--   0 build     (1000) build     (1001)     7422 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/Makefile
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.187822 todoman-4.3.1/docs/examples/
+-rw-r--r--   0 build     (1000) build     (1001)     2423 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/examples/conky.conf
+-rw-r--r--   0 build     (1000) build     (1001)      434 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/pull_request_template.md
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.187822 todoman-4.3.1/docs/source/
+-rw-r--r--   0 build     (1000) build     (1001)       33 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/changelog.rst
+-rw-r--r--   0 build     (1000) build     (1001)     2282 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/conf.py
+-rw-r--r--   0 build     (1000) build     (1001)     1510 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/configure.rst
+-rw-r--r--   0 build     (1000) build     (1001)     5055 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/contributing.rst
+-rw-r--r--   0 build     (1000) build     (1001)     1515 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/index.rst
+-rw-r--r--   0 build     (1000) build     (1001)     3590 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/install.rst
+-rw-r--r--   0 build     (1000) build     (1001)      101 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/licence.rst
+-rw-r--r--   0 build     (1000) build     (1001)      808 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/man.rst
+-rw-r--r--   0 build     (1000) build     (1001)     3526 2023-08-04 09:22:58.000000 todoman-4.3.1/docs/source/usage.rst
+-rw-r--r--   0 build     (1000) build     (1001)     2198 2023-08-04 09:22:58.000000 todoman-4.3.1/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1001)       38 2023-08-04 09:27:28.194489 todoman-4.3.1/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.191156 todoman-4.3.1/tests/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     4588 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/conftest.py
+-rw-r--r--   0 build     (1000) build     (1001)      861 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/helpers.py
+-rw-r--r--   0 build     (1000) build     (1001)     3364 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_backend.py
+-rw-r--r--   0 build     (1000) build     (1001)    31402 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_cli.py
+-rw-r--r--   0 build     (1000) build     (1001)     4604 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_config.py
+-rw-r--r--   0 build     (1000) build     (1001)     8998 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_filtering.py
+-rw-r--r--   0 build     (1000) build     (1001)     6218 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_formatter.py
+-rw-r--r--   0 build     (1000) build     (1001)      536 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_main.py
+-rw-r--r--   0 build     (1000) build     (1001)    14737 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_model.py
+-rw-r--r--   0 build     (1000) build     (1001)     7269 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_porcelain.py
+-rw-r--r--   0 build     (1000) build     (1001)     4822 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_ui.py
+-rw-r--r--   0 build     (1000) build     (1001)     6437 2023-08-04 09:22:58.000000 todoman-4.3.1/tests/test_widgets.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.194489 todoman-4.3.1/todoman/
+-rw-r--r--   0 build     (1000) build     (1001)      133 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)       94 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/__main__.py
+-rw-r--r--   0 build     (1000) build     (1001)    17484 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/cli.py
+-rw-r--r--   0 build     (1000) build     (1001)     6799 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/configuration.py
+-rw-r--r--   0 build     (1000) build     (1001)     1042 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/exceptions.py
+-rw-r--r--   0 build     (1000) build     (1001)     9734 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/formatters.py
+-rw-r--r--   0 build     (1000) build     (1001)     6488 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/interactive.py
+-rw-r--r--   0 build     (1000) build     (1001)    34788 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/model.py
+-rw-r--r--   0 build     (1000) build     (1001)      160 2023-08-04 09:27:27.000000 todoman-4.3.1/todoman/version.py
+-rw-r--r--   0 build     (1000) build     (1001)     5359 2023-08-04 09:22:58.000000 todoman-4.3.1/todoman/widgets.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-08-04 09:27:28.194489 todoman-4.3.1/todoman.egg-info/
+-rw-r--r--   0 build     (1000) build     (1001)     3521 2023-08-04 09:27:28.000000 todoman-4.3.1/todoman.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)     1214 2023-08-04 09:27:28.000000 todoman-4.3.1/todoman.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1001)        1 2023-08-04 09:27:28.000000 todoman-4.3.1/todoman.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1001)       41 2023-08-04 09:27:28.000000 todoman-4.3.1/todoman.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1001)      259 2023-08-04 09:27:28.000000 todoman-4.3.1/todoman.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1001)        8 2023-08-04 09:27:28.000000 todoman-4.3.1/todoman.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1001)      264 2023-08-04 09:22:58.000000 todoman-4.3.1/tox.ini
```

### Comparing `todoman-4.2.1/.builds/alpine.yml` & `todoman-4.3.1/.builds/archlinux.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,40 @@
-image: alpine/3.13
+image: archlinux
 packages:
-  - py-pip
-  - py-tox
-  - icu-dev
-  - alpine-sdk
-  - python3-dev
+  - python-build
+  - python-pipx
+  - python-pre-commit
+  - python-setuptools-scm
+  - python-tox
+  - python-wheel
+  - twine
 sources:
   - https://github.com/pimutils/todoman
+secrets:
+  - 9a8d4d44-96f9-4365-beaa-aaa759c4f1c4
 environment:
   CODECOV_TOKEN: a4471483-7f55-411a-bf2f-f65a91013dc4
   CI: true
 tasks:
   - setup: |
-      sudo pip install codecov
+      pipx install codecov
+      echo "export PATH=/home/build/.local/bin:$PATH" >> $HOME/.buildenv
   - test: |
-      # Test without pyicu installed:
       cd todoman
       tox -e py
       codecov
   - test-pyicu: |
-      # Test with pyicu installed:
       cd todoman
-      TOXENV=pyicu tox
+      tox -e pyicu
       codecov
   - test-repl: |
-      # Test repl repl:
       cd todoman
-      TOXENV=repl tox
+      tox -e repl
       codecov
+  - package: |
+      cd todoman
+      git fetch --tags
+      python -m build --no-isolation
+      git describe --exact-match --tags || complete-build
+  - publish: |
+      cd todoman
+      twine upload dist/*
```

### Comparing `todoman-4.2.1/.pre-commit-config.yaml` & `todoman-4.3.1/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,24 +5,25 @@
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
       - id: end-of-file-fixer
       - id: check-toml
       - id: check-added-large-files
       - id: debug-statements
   - repo: https://github.com/psf/black
-    rev: "23.1.0"
+    rev: "23.7.0"
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.0.0"
+    rev: "v1.4.1"
     hooks:
       - id: mypy
         additional_dependencies:
           - types-atomicwrites
           - types-tabulate
           - types-freezegun
           - types-pytz
           - types-python-dateutil
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.246'
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: 'v0.0.280'
     hooks:
       - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `todoman-4.2.1/AUTHORS.rst` & `todoman-4.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/CHANGELOG.rst` & `todoman-4.3.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Changelog
 =========
 
 This file contains a brief summary of new features and dependency changes or
 releases, in reverse chronological order.
 
+v4.3.0
+------
+
+* Add support for Python 3.11. Todoman already worked with Python 3.11, but is
+  now tested with this Python version in CI and has the relevant classifiers.
+* Improved zsh shell completion.
+* Dropped ``setup.py`` in favour of ``pyproject.toml``.
+
 v4.2.0
 ------
 
 * Added full support for categories.
 
 v4.1.0
 ------
```

### Comparing `todoman-4.2.1/LICENCE` & `todoman-4.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/PKG-INFO` & `todoman-4.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: todoman
-Version: 4.2.1
+Version: 4.3.1
 Summary: A simple icalendar-based todo manager.
-Home-page: https://github.com/pimutils/todoman
-Author: Hugo Osvaldo Barrera
-Author-email: hugo@barrera.io
+Author-email: Hugo Osvaldo Barrera <hugo@barrera.io>
 License: ISC
+Project-URL: homepage, https://github.com/pimutils/todoman
+Project-URL: documentation, https://todoman.readthedocs.io/
+Project-URL: changelog, https://github.com/pimutils/todoman/blob/main/CHANGELOG.rst
+Project-URL: issues, https://github.com/pimutils/todoman/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business :: Scheduling
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: repl
 License-File: LICENCE
 License-File: AUTHORS.rst
 
 Todoman
 =======
```

### Comparing `todoman-4.2.1/README.rst` & `todoman-4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/contrib/completion/bash/_todo` & `todoman-4.3.1/contrib/completion/bash/_todo`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/contrib/completion/zsh/_todo` & `todoman-4.3.1/contrib/completion/zsh/_todo`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,30 @@
 )
 local common_options_interactive=(
 	{-i,--interactive}'[Go into interactive mode before saving the task]'
 )
 local common_options_location=(
 	'--location=[The location where this todo takes place]:LOCATION:'
 )
+local common_options_category=(
+    \*{-c,--category=}'[Task categories. Can be used multiple times]:TEXT:__todo_existing_categories'
+)
+# }}}
+# {{{ general helper: check if jq is installed
+__todo_check_jq(){
+	# checking if the command jq exists and it's version
+	# credit: http://stackoverflow.com/a/592649/4935114
+	jq_version=$(jq --version 2>/dev/null)
+	if [ ${${jq_version#jq\-}//./} -lt 15 ]; then
+		_message "we can't complete tasks unless you'll install the latest version of jq: https://stedolan.github.io/jq/"
+		return 1
+    else
+        return 0
+	fi
+}
 # }}}
 # {{{ option helper: color mode
 __color_mode(){
 	local modes=(
 		"always:enable regardless of stdout"
 		"auto:enable only when not on tty (default)"
 		"never:disable colored output entirely"
@@ -40,15 +56,15 @@
 	fi
 }
 # }}}
 # {{{ general helper: set variable main.path from configuration file
 __todo_set_conf_path(){
 	if __todo_set_conf; then
 		tasks_lists_path="$(sed -n -e "s/^\\s*path\\s*=\\s*['\"]\\(.*\\)['\"]$/\\1/p" $todoman_configuration_file 2>/dev/null)"
-		# the eval echo is needed since the path may contain ~ which should be evalueated to $HOME
+		# the eval echo is needed since the path may contain ~ which should be evaluated to $HOME
 		tasks_lists_dir="$(eval echo ${tasks_lists_path%/\**})"
 		if [[ -z "${tasks_lists_path}" || ! -d "${tasks_lists_dir}" ]]; then
 			return 1
 		else
 			return 0
 		fi
 	else
@@ -100,24 +116,29 @@
 		'move:Move tasks to another list'
 		'new:Create a new task with SUMMARY'
 		'show:Show details about a task'
 	)
 	_describe "command" commands
 }
 # }}}
+# {{{ argument helper: available categories
+__todo_existing_categories(){
+    __todo_check_jq || return 1
+    local -a categories
+    IFS=$'\n'
+    for category in $(todo --porcelain list | jq --raw-output '[ .[] | .categories[] ] | unique[]'); do
+        categories+="$category"
+    done
+    _describe categories categories
+}
+# }}}
 # {{{ argument helper: available tasks choice
 __todo_tasks(){
-	# checking if the command jq exists and it's version
-	# credit: http://stackoverflow.com/a/592649/4935114
-	jq_version=$(jq --version 2>/dev/null)
-	if [ ${${jq_version#jq\-}//./} -lt 15 ]; then
-		_message "we can't complete tasks unless you'll install the latest version of jq: https://stedolan.github.io/jq/"
-		return
-	fi
-	# $1 is a comma-seperated list of statuses to show when trying to complete this
+    __todo_check_jq || return 1
+	# $1 is a comma-separated list of statuses to show when trying to complete this
 	local status_search_query="$1"
 	local -a tasks
 	IFS=$'\n'
 	for task_and_description in $(todo --porcelain list --status "${status_search_query}" | jq --raw-output '.[] | .id,":\"@",.list," ",.summary,"\"\\0"' | sed -e ':a' -e 'N' -e '$!ba' -e 's/\n//g' -e 's/\\0/\n/g'); do
 		tasks+="$(eval echo ${task_and_description})"
 	done
 	_describe tasks tasks
@@ -216,14 +237,15 @@
 # {{{ command `edit`
 local _command_edit_options=(
 	"${common_options_help[@]}"
 	"${common_options_start[@]}"
 	"${common_options_due[@]}"
 	"${common_options_priority[@]}"
 	"${common_options_location[@]}"
+	"${common_options_category[@]}"
 	"${common_options_interactive[@]}"
 )
 _todo_edit(){
 	_arguments \
 		"${_command_edit_options[@]}" \
 		'*: :{__todo_tasks "IN-PROCESS,NEEDS-ACTION"}'
 }
@@ -231,22 +253,22 @@
 # {{{ command `flush`
 _todo_flush(){
 }
 # }}}
 # {{{ command `list`
 _command_list_options=(
 	"${common_options_location[@]}"
-	'--category=[Only show tasks with category containg TEXT]:TEXT:__todo_existing_categories'
-	'--grep=[Only show tasks with message containg TEXT]:TEXT:'
+	"${common_options_category[@]}"
+	'--grep=[Only show tasks with message containing TEXT]:TEXT:'
 	'--sort=[Sort tasks using these fields]:TEXT:(description location status summary uid rrule percent_complete priority sequence categories completed_at created_at dtstamp start due last_modified)'
 	'(--reverse --no-reverse)'{--reverse,--no-reverse}'[sort tasks in reverse order (see --sort)]'
 	"${common_options_start[@]}"
 	"${common_options_due[@]}"
 	'--priority=[Only show tasks with priority at least as high as TEXT]:TEXT:("low" "medium" "high")'
-	'--startable[Show only todos which should can be started today]'
+	'--startable[Show only todos which can be started today]'
 	{-s,--status=}'[Show only todos with the provided comma-separated statuses]:STATUS:{_values -s , "status" "NEEDS-ACTION" "CANCELLED" "COMPLETED" "IN-PROCESS" "ANY"}'
 	"${common_options_help[@]}"
 )
 _todo_list(){
 	_arguments \
 		"${_command_list_options[@]}" \
 		'1: :__todo_lists' \
@@ -259,15 +281,16 @@
 # }}}
 # {{{ command `new`
 local _command_new_options=(
 	"${common_options_start[@]}"
 	"${common_options_due[@]}"
 	"${common_options_help[@]}"
 	{-l,--list=}'[The list to move the tasks to]:TEXT:__todo_lists'
-	'--location[The location where this todo takes place.]:TEXT:__todo_existing_locations'
+	"${common_options_location[@]}"
+	"${common_options_category[@]}"
 	"${common_options_priority[@]}"
 	"${common_options_interactive[@]}"
 )
 _todo_new(){
 	_arguments \
 		"${_command_new_options[@]}" \
 		'*: :{_message "summary"}'
```

### Comparing `todoman-4.2.1/docs/Makefile` & `todoman-4.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/examples/conky.conf` & `todoman-4.3.1/docs/examples/conky.conf`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/source/conf.py` & `todoman-4.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/source/configure.rst` & `todoman-4.3.1/docs/source/configure.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/source/contributing.rst` & `todoman-4.3.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/source/index.rst` & `todoman-4.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/source/install.rst` & `todoman-4.3.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/source/man.rst` & `todoman-4.3.1/docs/source/man.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/docs/source/usage.rst` & `todoman-4.3.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/setup.py` & `todoman-4.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,102 @@
-#!/usr/bin/env python3
-from setuptools import setup
+[project]
+name = "todoman"
+authors = [
+    {name = "Hugo Osvaldo Barrera", email = "hugo@barrera.io"},
+]
+description = "A simple icalendar-based todo manager."
+readme = "README.rst"
+requires-python = ">=3.7"
+# keywords = ["TODO"]
+license = {text = "ISC"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Environment :: Console :: Curses",
+    "License :: OSI Approved :: ISC License (ISCL)",
+    "Operating System :: POSIX",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Topic :: Office/Business :: Scheduling",
+    "Topic :: Utilities",
+]
+dependencies = [
+    "atomicwrites",
+    "click>=7.1,<9.0",
+    "click-log>=0.2.1",
+    "humanize",
+    "icalendar>=4.0.3",
+    "parsedatetime",
+    "python-dateutil",
+    "pyxdg",
+    "urwid",
+]
+dynamic = ["version"]
 
-with open("README.rst") as r:
-    long_description = r.read()
-with open("requirements-dev.txt") as r:
-    tests_require = r.readlines()
-with open("requirements-docs.txt") as r:
-    docs = r.readlines()
-
-setup(
-    name="todoman",
-    description="A simple icalendar-based todo manager.",
-    author="Hugo Osvaldo Barrera",
-    author_email="hugo@barrera.io",
-    url="https://github.com/pimutils/todoman",
-    license="ISC",
-    packages=["todoman"],
-    include_package_data=True,
-    entry_points={"console_scripts": ["todo = todoman.cli:cli"]},
-    install_requires=[
-        "atomicwrites",
-        "click>=7.1,<9.0",
-        "click-log>=0.2.1",
-        "humanize",
-        "icalendar>=4.0.3",
-        "parsedatetime",
-        "python-dateutil",
-        "pyxdg",
-        "urwid",
-    ],
-    long_description=long_description,
-    setup_requires=["setuptools_scm"],
-    tests_require=tests_require,
-    extras_require={
-        "docs": docs,
-        "repl": ["click-repl>=0.1.6"],
-    },
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Console",
-        "Environment :: Console :: Curses",
-        "License :: OSI Approved :: ISC License (ISCL)",
-        "Operating System :: POSIX",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: Implementation :: PyPy",
-        "Topic :: Office/Business :: Scheduling",
-        "Topic :: Utilities",
-    ],
-)
+[project.optional-dependencies]
+test = [
+    "freezegun",
+    "hypothesis",
+    "pytest",
+    "pytest-cov",
+    "pytest-runner",
+    "ruff",
+]
+docs = [
+    "sphinx_autorun",
+    "sphinx-click",
+    "sphinx_rtd_theme",
+]
+repl = [
+    "click-repl>=0.1.6",
+]
+
+[project.urls]
+homepage = "https://github.com/pimutils/todoman"
+documentation = "https://todoman.readthedocs.io/"
+changelog = "https://github.com/pimutils/todoman/blob/main/CHANGELOG.rst"
+issues = "https://github.com/pimutils/todoman/issues"
+
+[project.scripts]
+todo = "todoman.cli:cli"
+
+[tool.setuptools]
+packages = ["todoman"]
+
+[tool.ruff]
+select = [
+    "E",
+    "F",
+    "W",
+    "B",
+    "I",
+    "UP",
+    "N",
+    # "ANN",
+    # "A",
+    "C4",
+    "PT",
+    "SIM",
+    "TID",
+]
+target-version = "py38"
+
+[tool.ruff.isort]
+force-single-line = true
+
+[build-system]
+requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
+
+[tool.setuptools_scm]
+write_to = "todoman/version.py"
+version_scheme = "post-release"
+
+[tool.mypy]
+ignore_missing_imports = true
+
+[tool.pytest.ini_options]
+testpaths = "tests"
+addopts = "--cov=todoman --cov-report=term-missing --color=yes --verbose"
```

### Comparing `todoman-4.2.1/tests/conftest.py` & `todoman-4.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/helpers.py` & `todoman-4.3.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_backend.py` & `todoman-4.3.1/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_cli.py` & `todoman-4.3.1/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,17 +531,15 @@
 
 def test_empty_list(tmpdir, runner, create):
     for item in tmpdir.listdir():
         if item.isdir():
             item.remove()
 
     result = runner.invoke(cli)
-    expected = (
-        "No lists found matching {}/*, create a directory for a new list"
-    ).format(tmpdir)
+    expected = f"No lists found matching {tmpdir}/*, create a directory for a new list"
 
     assert expected in result.output
 
 
 def test_show_location(tmpdir, runner, create):
     create("test.ics", f"UID:{uuid4()}\nSUMMARY:harhar\nLOCATION:Boston\n")
```

### Comparing `todoman-4.2.1/tests/test_config.py` & `todoman-4.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_filtering.py` & `todoman-4.3.1/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_formatter.py` & `todoman-4.3.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_main.py` & `todoman-4.3.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_model.py` & `todoman-4.3.1/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 
 
 def test_querying(create, tmpdir):
     for list in "abc":
         for i, location in enumerate("abc"):
             create(
                 f"test{i}.ics",
-                ("UID:{}\nSUMMARY:test_querying\r\nLOCATION:{}\r\n").format(
-                    uuid4(), location
-                ),
+                f"UID:{uuid4()}\nSUMMARY:test_querying\r\nLOCATION:{location}\r\n",
                 list_name=list,
             )
 
     db = Database(
         [str(tmpdir.ensure_dir(list_)) for list_ in "abc"], str(tmpdir.join("cache"))
     )
 
@@ -193,21 +191,19 @@
     default_database.save(todo)
 
     assert default_database.todos().__next__().uid == uid
 
     default_database.delete(todo)
     default_database.update_cache()
 
-    query = """
+    query = f"""
         SELECT distinct category
         FROM categories
-        WHERE categories.todos_id = '{}'
-        """.format(
-        todo.id,
-    )
+        WHERE categories.todos_id = '{todo.id}'
+        """
 
     categories = default_database.cache._conn.execute(query).fetchall()
     assert categories == []
 
 
 def test_todo_setters(todo_factory):
     todo = todo_factory()
@@ -534,8 +530,8 @@
         db.save(todo)
 
 
 def test_todo_path_without_list(tmpdir):
     todo = Todo()
 
     with pytest.raises(ValueError, match="A todo without a list does not have a path."):
-        todo.path
+        todo.path  # noqa: B018  # expression raises
```

### Comparing `todoman-4.2.1/tests/test_porcelain.py` & `todoman-4.3.1/tests/test_porcelain.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_ui.py` & `todoman-4.3.1/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/tests/test_widgets.py` & `todoman-4.3.1/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/todoman/cli.py` & `todoman-4.3.1/todoman/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import contextlib
 import functools
 import glob
 import locale
 import sys
 from contextlib import contextmanager
+from datetime import datetime
 from datetime import timedelta
 from os.path import isdir
+from typing import Tuple
 
 import click
 import click_log
 
 from todoman import exceptions
 from todoman import formatters
 from todoman.configuration import ConfigurationError
@@ -91,18 +93,18 @@
     ctx = ctx.find_object(AppContext)
     try:
         return ctx.formatter.parse_priority(val)
     except ValueError as e:
         raise click.BadParameter(e) from None
 
 
-def _validate_start_date_param(ctx, param, val):
+def _validate_start_date_param(ctx, param, val) -> Tuple[bool, datetime] | None:
     ctx = ctx.find_object(AppContext)
     if not val:
-        return val
+        return None
 
     if len(val) != 2 or val[0] not in ["before", "after"]:
         raise click.BadParameter("Format should be '[before|after] [DATE]'")
 
     is_before = val[0] == "before"
 
     try:
```

### Comparing `todoman-4.2.1/todoman/configuration.py` & `todoman-4.3.1/todoman/configuration.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/todoman/exceptions.py` & `todoman-4.3.1/todoman/exceptions.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/todoman/formatters.py` & `todoman-4.3.1/todoman/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,27 +86,20 @@
             due_colour = self._due_colour(todo)
             if due_colour:
                 due = click.style(str(due), fg=due_colour)
 
             recurring = "⟳" if todo.is_recurring else ""
 
             if hide_list:
-                summary = "{} {}".format(
-                    todo.summary,
-                    percent,
-                )
+                summary = f"{todo.summary} {percent}"
             else:
                 if not todo.list:
                     raise ValueError("Cannot format todo without a list")
 
-                summary = "{} {}{}".format(
-                    todo.summary,
-                    self.format_database(todo.list),
-                    percent,
-                )
+                summary = f"{todo.summary} {self.format_database(todo.list)}{percent}"
 
             # TODO: add spaces on the left based on max todos"
 
             # FIXME: double space when no priority
             # split into parts to satisfy linter line too long
             table.append(
                 f"[{completed}] {todo.id} {priority} {due} "
```

### Comparing `todoman-4.2.1/todoman/interactive.py` & `todoman-4.3.1/todoman/interactive.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/todoman/model.py` & `todoman-4.3.1/todoman/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -764,19 +764,15 @@
                 list_.name if isinstance(list_, TodoList) else list_ for list_ in lists
             ]
             q = ", ".join(["?"] * len(lists))
             extra_where.append(f"AND files.list_name IN ({q})")
             params.extend(lists)
         if categories:
             category_slots = ", ".join(["?"] * len(categories))
-            extra_where.append(
-                "AND upper(categories.category) IN ({category_slots})".format(
-                    category_slots=category_slots
-                )
-            )
+            extra_where.append(f"AND upper(categories.category) IN ({category_slots})")
             params = params + [category.upper() for category in categories]
         if priority:
             extra_where.append("AND PRIORITY > 0 AND PRIORITY <= ?")
             params.append(f"{priority}")
         if location:
             extra_where.append("AND location LIKE ?")
             params.append(f"%{location}%")
```

### Comparing `todoman-4.2.1/todoman/widgets.py` & `todoman-4.3.1/todoman/widgets.py`

 * *Files identical despite different names*

### Comparing `todoman-4.2.1/todoman.egg-info/PKG-INFO` & `todoman-4.3.1/todoman.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: todoman
-Version: 4.2.1
+Version: 4.3.1
 Summary: A simple icalendar-based todo manager.
-Home-page: https://github.com/pimutils/todoman
-Author: Hugo Osvaldo Barrera
-Author-email: hugo@barrera.io
+Author-email: Hugo Osvaldo Barrera <hugo@barrera.io>
 License: ISC
+Project-URL: homepage, https://github.com/pimutils/todoman
+Project-URL: documentation, https://todoman.readthedocs.io/
+Project-URL: changelog, https://github.com/pimutils/todoman/blob/main/CHANGELOG.rst
+Project-URL: issues, https://github.com/pimutils/todoman/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business :: Scheduling
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: repl
 License-File: LICENCE
 License-File: AUTHORS.rst
 
 Todoman
 =======
```

### Comparing `todoman-4.2.1/todoman.egg-info/SOURCES.txt` & `todoman-4.3.1/todoman.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 LICENCE
 README.rst
 codecov.yml
 config.py.sample
 pyproject.toml
-requirements-dev.txt
-requirements-docs.txt
-setup.py
 tox.ini
 .builds/alpine.yml
 .builds/archlinux.yml
 bin/todo
 contrib/completion/bash/_todo
 contrib/completion/zsh/_todo
 docs/Makefile
```

