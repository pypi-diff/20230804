# Comparing `tmp/craft-archives-1.1.2.tar.gz` & `tmp/craft-archives-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-archives-1.1.2.tar", last modified: Tue Jul 11 20:48:18 2023, max compression
+gzip compressed data, was "craft-archives-1.1.3.tar", last modified: Fri Aug  4 16:52:51 2023, max compression
```

## Comparing `craft-archives-1.1.2.tar` & `craft-archives-1.1.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.595326 craft-archives-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.codespell_ignore_lines
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/bug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/ISSUE_TEMPLATE/task.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/renovate.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/cla-check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/issues.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/release-drafter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/release-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.yamlignore
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-11 20:48:02.000000 craft-archives-1.1.2/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-11 20:48:02.000000 craft-archives-1.1.2/HACKING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-11 20:48:02.000000 craft-archives-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-11 20:48:18.595326 craft-archives-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 20:48:02.000000 craft-archives-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/craft_archives/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/craft_archives/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/apt_uca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/package_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/repo/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-11 20:48:02.000000 craft-archives-1.1.2/craft_archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.587326 craft-archives-1.1.2/craft_archives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 20:48:18.000000 craft-archives-1.1.2/craft_archives.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.583326 craft-archives-1.1.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/explanation/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/explanation/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/howto/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/howto/add_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/howto/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/reference/repo_properties.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 20:48:02.000000 craft-archives-1.1.2/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-11 20:48:02.000000 craft-archives-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:48:18.595326 craft-archives-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/integration/repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/repo/test_apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/integration/repo/test_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/FC42E99D.asc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/empty.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/expected.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/many_blank_lines.preferences
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/test_data/multi-keys/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/multi-keys/0264B26D.asc
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/multi-keys/9E61EF26.asc
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/no_header.preferences
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/only_comment.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/test_data/with_header.preferences
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.591326 craft-archives-1.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:18.595326 craft-archives-1.1.2/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_apt_uca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_package_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tests/unit/repo/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-11 20:48:02.000000 craft-archives-1.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.283678 craft-archives-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.codespell_ignore_lines
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.271678 craft-archives-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.271678 craft-archives-1.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/ISSUE_TEMPLATE/task.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.271678 craft-archives-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/workflows/cla-check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/workflows/issues.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/workflows/release-drafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/workflows/release-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.yamlignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-04 16:52:30.000000 craft-archives-1.1.3/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-04 16:52:30.000000 craft-archives-1.1.3/HACKING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-04 16:52:30.000000 craft-archives-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-04 16:52:51.283678 craft-archives-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-04 16:52:30.000000 craft-archives-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.275678 craft-archives-1.1.3/craft_archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 16:52:51.000000 craft-archives-1.1.3/craft_archives/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.275678 craft-archives-1.1.3/craft_archives/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/repo/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-08-04 16:52:30.000000 craft-archives-1.1.3/craft_archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.275678 craft-archives-1.1.3/craft_archives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-04 16:52:51.000000 craft-archives-1.1.3/craft_archives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-04 16:52:51.000000 craft-archives-1.1.3/craft_archives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:52:51.000000 craft-archives-1.1.3/craft_archives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-04 16:52:51.000000 craft-archives-1.1.3/craft_archives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 16:52:51.000000 craft-archives-1.1.3/craft_archives.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.275678 craft-archives-1.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.267678 craft-archives-1.1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.275678 craft-archives-1.1.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.275678 craft-archives-1.1.3/docs/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/explanation/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.275678 craft-archives-1.1.3/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/howto/add_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/howto/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.279678 craft-archives-1.1.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/reference/repo_properties.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.279678 craft-archives-1.1.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-04 16:52:30.000000 craft-archives-1.1.3/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-08-04 16:52:30.000000 craft-archives-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:52:51.283678 craft-archives-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.279678 craft-archives-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.279678 craft-archives-1.1.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.279678 craft-archives-1.1.3/tests/integration/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/integration/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/integration/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/integration/repo/test_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.279678 craft-archives-1.1.3/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/FC42E99D.asc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/empty.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/expected.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/many_blank_lines.preferences
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.283678 craft-archives-1.1.3/tests/test_data/multi-keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/multi-keys/0264B26D.asc
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/multi-keys/9E61EF26.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/no_header.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/only_comment.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/test_data/with_header.preferences
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.283678 craft-archives-1.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:51.283678 craft-archives-1.1.3/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tests/unit/repo/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-04 16:52:30.000000 craft-archives-1.1.3/tox.ini
```

### Comparing `craft-archives-1.1.2/.editorconfig` & `craft-archives-1.1.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/ISSUE_TEMPLATE/bug.yaml` & `craft-archives-1.1.3/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/ISSUE_TEMPLATE/task.yaml` & `craft-archives-1.1.3/.github/ISSUE_TEMPLATE/task.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/renovate.json5` & `craft-archives-1.1.3/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/workflows/docs.yaml` & `craft-archives-1.1.3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/workflows/issues.yaml` & `craft-archives-1.1.3/.github/workflows/issues.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/workflows/release-drafter.yaml` & `craft-archives-1.1.3/.github/workflows/release-drafter.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/workflows/release-publish.yaml` & `craft-archives-1.1.3/.github/workflows/release-publish.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.github/workflows/tests.yaml` & `craft-archives-1.1.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.gitignore` & `craft-archives-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/.pre-commit-config.yaml` & `craft-archives-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/HACKING.rst` & `craft-archives-1.1.3/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/LICENSE` & `craft-archives-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/PKG-INFO` & `craft-archives-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.1.2
+Version: 1.1.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.1.2/README.rst` & `craft-archives-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/__init__.py` & `craft-archives-1.1.3/craft_archives/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/errors.py` & `craft-archives-1.1.3/craft_archives/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/__init__.py` & `craft-archives-1.1.3/craft_archives/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/apt_key_manager.py` & `craft-archives-1.1.3/craft_archives/repo/apt_key_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/apt_ppa.py` & `craft-archives-1.1.3/craft_archives/repo/apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/apt_preferences_manager.py` & `craft-archives-1.1.3/craft_archives/repo/apt_preferences_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/apt_sources_manager.py` & `craft-archives-1.1.3/craft_archives/repo/apt_sources_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -295,13 +295,29 @@
             return changed
 
         raise RuntimeError(f"unhandled package repository: {package_repository!r}")
 
 
 def _add_architecture(architectures: List[str], root: Path) -> None:
     """Add package repository architecture."""
+    current_arch = _get_current_architecture()
+    compatible_pairs = {"amd64": "i386", "arm64": "armhf"}
     for arch in architectures:
-        logger.info(f"Add repository architecture: {arch}")
-        subprocess.run(
-            ["dpkg", "--add-architecture", arch, "--root", str(root)],
-            check=True,
-        )
+        # We can only add architectures if they are compatible with the running host,
+        # because of the way the default repositories are typically setup.
+        if compatible_pairs.get(current_arch) == arch:
+            logger.info(f"Add repository architecture: {arch}")
+            subprocess.run(
+                # Note: the order of parameters matters here, as "--add-architecture"
+                # must come last because of the way dpkg parses the command.
+                ["dpkg", "--root", str(root), "--add-architecture", arch],
+                check=True,
+            )
+
+
+def _get_current_architecture() -> str:
+    """Get the "main" architecture of the running system, as reported by dpkg."""
+    return (
+        subprocess.check_output(["dpkg", "--print-architecture"])
+        .decode("utf-8")
+        .strip()
+    )
```

### Comparing `craft-archives-1.1.2/craft_archives/repo/apt_uca.py` & `craft-archives-1.1.3/craft_archives/repo/apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/errors.py` & `craft-archives-1.1.3/craft_archives/repo/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/installer.py` & `craft-archives-1.1.3/craft_archives/repo/installer.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/package_repository.py` & `craft-archives-1.1.3/craft_archives/repo/package_repository.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/repo/projects.py` & `craft-archives-1.1.3/craft_archives/repo/projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives/utils.py` & `craft-archives-1.1.3/craft_archives/utils.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/craft_archives.egg-info/PKG-INFO` & `craft-archives-1.1.3/craft_archives.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.1.2
+Version: 1.1.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.1.2/craft_archives.egg-info/SOURCES.txt` & `craft-archives-1.1.3/craft_archives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/docs/conf.py` & `craft-archives-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/docs/howto/add_repo.rst` & `craft-archives-1.1.3/docs/howto/add_repo.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/docs/index.rst` & `craft-archives-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/docs/reference/repo_properties.rst` & `craft-archives-1.1.3/docs/reference/repo_properties.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/pyproject.toml` & `craft-archives-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/conftest.py` & `craft-archives-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/integration/repo/test_apt_key_manager.py` & `craft-archives-1.1.3/tests/integration/repo/test_apt_key_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/integration/repo/test_installer.py` & `craft-archives-1.1.3/tests/integration/repo/test_installer.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/test_data/FC42E99D.asc` & `craft-archives-1.1.3/tests/test_data/FC42E99D.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/test_data/multi-keys/0264B26D.asc` & `craft-archives-1.1.3/tests/test_data/multi-keys/0264B26D.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/test_data/multi-keys/9E61EF26.asc` & `craft-archives-1.1.3/tests/test_data/multi-keys/9E61EF26.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_apt_key_manager.py` & `craft-archives-1.1.3/tests/unit/repo/test_apt_key_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_apt_ppa.py` & `craft-archives-1.1.3/tests/unit/repo/test_apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_apt_preferences_manager.py` & `craft-archives-1.1.3/tests/unit/repo/test_apt_preferences_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_apt_sources_manager.py` & `craft-archives-1.1.3/tests/unit/repo/test_apt_sources_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 import distro
 import pytest
 from craft_archives.repo import apt_ppa, apt_sources_manager, errors
 from craft_archives.repo.apt_sources_manager import (
     _DEFAULT_SOURCES_DIRECTORY,
     AptSourcesManager,
+    _add_architecture,
 )
 from craft_archives.repo.package_repository import (
     PackageRepositoryApt,
     PackageRepositoryAptPPA,
     PackageRepositoryAptUCA,
 )
 
@@ -183,14 +184,22 @@
     package_repo,
     name,
     content_template,
     use_signed_by_root,
     mocker,
 ):
     run_mock = mocker.patch("subprocess.run")
+    get_architecture_mock = mocker.patch(
+        "subprocess.check_output", return_value=b"fake"
+    )
+    add_architecture_mock = mocker.spy(
+        apt_sources_manager,
+        "_add_architecture",
+    )
+
     mocker.patch("urllib.request.urlopen")
 
     apt_sources_mgr = create_apt_sources_mgr(
         tmp_path, use_signed_by_root=use_signed_by_root
     )
     sources_path = apt_sources_mgr._sources_list_d / name
 
@@ -212,31 +221,27 @@
         package_repo=package_repo
     )
 
     assert changed is True
     assert sources_path.read_bytes() == content
 
     if use_signed_by_root:
-        expected_root = str(tmp_path)
+        expected_root = tmp_path
     else:
-        expected_root = "/"
+        expected_root = Path("/")
 
     if isinstance(package_repo, PackageRepositoryApt) and package_repo.architectures:
-        assert run_mock.mock_calls == [
-            call(
-                ["dpkg", "--add-architecture", "amd64", "--root", expected_root],
-                check=True,
-            ),
-            call(
-                ["dpkg", "--add-architecture", "arm64", "--root", expected_root],
-                check=True,
-            ),
+        assert add_architecture_mock.mock_calls == [
+            call(package_repo.architectures, root=expected_root)
         ]
-    else:
-        assert run_mock.mock_calls == []
+        assert get_architecture_mock.called
+
+    # Regardless of host architecture, "dpkg --add-architecture" must _not_ be called,
+    # because the fantasy archs in the test repos are not compatible.
+    assert run_mock.mock_calls == []
 
     run_mock.reset_mock()
 
     # Verify a second-run does not incur any changes.
     changed = apt_sources_mgr.install_package_repository_sources(
         package_repo=package_repo
     )
@@ -290,7 +295,48 @@
 
 
 def test_preferences_path_for_root():
     assert AptSourcesManager.sources_path_for_root() == _DEFAULT_SOURCES_DIRECTORY
     assert AptSourcesManager.sources_path_for_root(Path("/my/root")) == Path(
         "/my/root/etc/apt/sources.list.d"
     )
+
+
+@pytest.mark.parametrize(
+    ("host_arch, repo_arch"),
+    [
+        (b"amd64\n", "i386"),
+        (b"arm64\n", "armhf"),
+    ],
+)
+def test_add_architecture_compatible(mocker, host_arch, repo_arch):
+    """Test calling _add_architecture() with compatible pairs of (host, repo)."""
+    check_output_mock = mocker.patch("subprocess.check_output", return_value=host_arch)
+    run_mock = mocker.patch("subprocess.run")
+
+    _add_architecture([repo_arch], root=Path("/"))
+
+    check_output_mock.assert_called_once_with(["dpkg", "--print-architecture"])
+    assert run_mock.mock_calls == [
+        call(
+            ["dpkg", "--root", "/", "--add-architecture", repo_arch],
+            check=True,
+        ),
+    ]
+
+
+@pytest.mark.parametrize(
+    ("host_arch, repo_arch"),
+    [
+        (b"amd64\n", "arm64"),
+        (b"arm64\n", "i386"),
+    ],
+)
+def test_add_architecture_incompatible(mocker, host_arch, repo_arch):
+    """Test calling _add_architecture() with incompatible pairs of (host, repo)."""
+    check_output_mock = mocker.patch("subprocess.check_output", return_value=host_arch)
+    run_mock = mocker.patch("subprocess.run")
+
+    _add_architecture([repo_arch], root=Path("/"))
+
+    check_output_mock.assert_called_once_with(["dpkg", "--print-architecture"])
+    assert not run_mock.called
```

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_apt_uca.py` & `craft-archives-1.1.3/tests/unit/repo/test_apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_installer.py` & `craft-archives-1.1.3/tests/unit/repo/test_installer.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_package_repository.py` & `craft-archives-1.1.3/tests/unit/repo/test_package_repository.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tests/unit/repo/test_projects.py` & `craft-archives-1.1.3/tests/unit/repo/test_projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.1.2/tox.ini` & `craft-archives-1.1.3/tox.ini`

 * *Files identical despite different names*

