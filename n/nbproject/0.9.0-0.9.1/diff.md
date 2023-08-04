# Comparing `tmp/nbproject-0.9.0.tar.gz` & `tmp/nbproject-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbproject-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nbproject-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nbproject-0.9.0.tar` & `nbproject-0.9.1.tar`

### file list

```diff
@@ -1,74 +1,73 @@
--rw-r--r--   0        0        0     2475 2023-06-15 19:08:05.360108 nbproject-0.9.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-06-10 19:50:58.313927 nbproject-0.9.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-06-10 19:50:58.314964 nbproject-0.9.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1880 2022-07-10 12:10:29.382368 nbproject-0.9.0/.gitignore
--rw-r--r--   0        0        0     1645 2022-08-29 09:33:05.135542 nbproject-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      740 2022-10-24 12:29:45.346974 nbproject-0.9.0/CITATION.cff
--rw-r--r--   0        0        0    11357 2022-04-18 20:46:44.681265 nbproject-0.9.0/LICENSE
--rw-r--r--   0        0        0     1782 2023-06-15 19:08:05.360700 nbproject-0.9.0/README.md
--rw-r--r--   0        0        0    20762 2023-06-15 19:08:47.637622 nbproject-0.9.0/docs/changelog.md
--rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.213819 nbproject-0.9.0/docs/faq/example-after-init-set-filename.ipynb
--rw-r--r--   0        0        0     1481 2022-10-07 21:00:12.845099 nbproject-0.9.0/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
--rw-r--r--   0        0        0      123 2022-09-06 11:40:41.171382 nbproject-0.9.0/docs/faq/example-project-uninitialized/index.md
--rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.214012 nbproject-0.9.0/docs/faq/example-project/2022-05-13-my-task-x.ipynb
--rw-r--r--   0        0        0     1661 2022-11-12 18:33:53.214173 nbproject-0.9.0/docs/faq/example-project/2022-07-18-my-task-y.ipynb
--rw-r--r--   0        0        0      101 2022-09-06 11:40:41.171829 nbproject-0.9.0/docs/faq/example-project/index.md
--rw-r--r--   0        0        0      364 2022-11-12 18:33:53.214429 nbproject-0.9.0/docs/faq/example-project/nbproject_metadata.yml
--rw-r--r--   0        0        0     1873 2022-11-12 18:33:53.214599 nbproject-0.9.0/docs/faq/header-author-field.ipynb
--rw-r--r--   0        0        0     1520 2022-11-12 18:33:53.214757 nbproject-0.9.0/docs/faq/inconsistent-packages-parents-no-store.ipynb
--rw-r--r--   0        0        0     2330 2022-11-12 18:33:53.214908 nbproject-0.9.0/docs/faq/inconsistent-packages-parents-store.ipynb
--rw-r--r--   0        0        0     1096 2022-10-10 12:03:49.454347 nbproject-0.9.0/docs/faq/index.md
--rw-r--r--   0        0        0     1311 2022-09-06 11:40:41.172354 nbproject-0.9.0/docs/faq/initialize-set-env.ipynb
--rw-r--r--   0        0        0     2049 2022-09-06 11:40:41.172505 nbproject-0.9.0/docs/faq/initialize.ipynb
--rw-r--r--   0        0        0     4086 2022-11-12 18:33:53.215053 nbproject-0.9.0/docs/faq/internal-functions.ipynb
--rw-r--r--   0        0        0     2708 2022-09-06 11:40:41.172679 nbproject-0.9.0/docs/faq/not-initialized.ipynb
--rw-r--r--   0        0        0     1803 2022-11-12 18:33:53.215192 nbproject-0.9.0/docs/faq/publish-not-last-cell.ipynb
--rw-r--r--   0        0        0     1399 2022-11-12 18:33:53.215339 nbproject-0.9.0/docs/faq/publish-set-version.ipynb
--rw-r--r--   0        0        0     1818 2022-11-12 18:33:53.215489 nbproject-0.9.0/docs/faq/publish-without-saving.ipynb
--rw-r--r--   0        0        0     1787 2022-11-12 18:33:53.215632 nbproject-0.9.0/docs/faq/publish-without-title.ipynb
--rw-r--r--   0        0        0     1653 2022-11-12 18:33:53.215765 nbproject-0.9.0/docs/faq/publish-wrapper.ipynb
--rw-r--r--   0        0        0     1577 2022-10-07 21:00:16.804143 nbproject-0.9.0/docs/faq/set-env-via-environment-var.ipynb
--rw-r--r--   0        0        0      679 2022-10-10 14:54:28.366976 nbproject-0.9.0/docs/faq/setup.md
--rw-r--r--   0        0        0     1357 2022-09-06 11:40:41.173529 nbproject-0.9.0/docs/faq/trigger-exit-upon-init.ipynb
--rw-r--r--   0        0        0     2694 2022-11-12 18:33:53.215926 nbproject-0.9.0/docs/guide/basic-metadata.ipynb
--rw-r--r--   0        0        0     2675 2022-09-06 11:40:41.173736 nbproject-0.9.0/docs/guide/cli.md
--rw-r--r--   0        0        0      328 2022-09-06 11:40:41.173880 nbproject-0.9.0/docs/guide/index.md
--rw-r--r--   0        0        0     4639 2023-04-17 07:11:01.412769 nbproject-0.9.0/docs/guide/meta.ipynb
--rw-r--r--   0        0        0     1637 2022-11-12 18:33:53.216221 nbproject-0.9.0/docs/guide/received.ipynb
--rw-r--r--   0        0        0     2964 2022-11-12 18:33:53.216369 nbproject-0.9.0/docs/guide/update-metadata.ipynb
--rw-r--r--   0        0        0      142 2023-04-17 07:11:01.413339 nbproject-0.9.0/docs/index.md
--rw-r--r--   0        0        0     2755 2022-11-12 18:33:53.216521 nbproject-0.9.0/docs/quickstart.ipynb
--rw-r--r--   0        0        0       57 2023-04-17 07:11:01.413670 nbproject-0.9.0/docs/reference.md
--rw-r--r--   0        0        0      137 2022-06-01 14:27:38.468097 nbproject-0.9.0/lamin-project.yaml
--rw-r--r--   0        0        0      763 2023-06-15 19:08:43.059386 nbproject-0.9.0/nbproject/__init__.py
--rw-r--r--   0        0        0     1631 2022-08-17 11:48:35.494040 nbproject-0.9.0/nbproject/__main__.py
--rw-r--r--   0        0        0     5121 2022-11-12 18:33:53.216715 nbproject-0.9.0/nbproject/_cli.py
--rw-r--r--   0        0        0     5742 2023-06-15 19:08:05.361081 nbproject-0.9.0/nbproject/_header.py
--rw-r--r--   0        0        0      285 2022-11-13 23:00:04.437788 nbproject-0.9.0/nbproject/_is_run_from_ipython.py
--rw-r--r--   0        0        0       48 2022-07-23 18:45:14.093130 nbproject-0.9.0/nbproject/_logger.py
--rw-r--r--   0        0        0     3080 2022-10-10 12:03:49.455892 nbproject-0.9.0/nbproject/_meta.py
--rw-r--r--   0        0        0     3943 2022-11-12 18:52:44.680900 nbproject-0.9.0/nbproject/_publish.py
--rw-r--r--   0        0        0     4007 2022-11-12 18:33:53.217134 nbproject-0.9.0/nbproject/_schemas.py
--rw-r--r--   0        0        0      836 2023-06-04 20:57:48.693471 nbproject-0.9.0/nbproject/dev/__init__.py
--rw-r--r--   0        0        0      590 2022-10-07 21:00:16.805272 nbproject-0.9.0/nbproject/dev/_check_last_cell.py
--rw-r--r--   0        0        0      681 2022-08-17 11:48:35.496655 nbproject-0.9.0/nbproject/dev/_classic_nb_commands.py
--rw-r--r--   0        0        0     1473 2023-06-04 20:57:48.693977 nbproject-0.9.0/nbproject/dev/_consecutiveness.py
--rw-r--r--   0        0        0      525 2022-08-17 11:48:35.496751 nbproject-0.9.0/nbproject/dev/_frontend_commands.py
--rw-r--r--   0        0        0     1843 2023-06-04 20:57:48.694457 nbproject-0.9.0/nbproject/dev/_initialize.py
--rw-r--r--   0        0        0     5137 2023-06-13 15:37:27.141838 nbproject-0.9.0/nbproject/dev/_jupyter_communicate.py
--rw-r--r--   0        0        0      822 2023-04-17 07:11:01.415333 nbproject-0.9.0/nbproject/dev/_jupyter_lab_commands.py
--rw-r--r--   0        0        0      343 2023-04-17 07:11:01.415771 nbproject-0.9.0/nbproject/dev/_lamin_communicate.py
--rw-r--r--   0        0        0     3642 2022-10-10 18:44:26.046429 nbproject-0.9.0/nbproject/dev/_meta_live.py
--rw-r--r--   0        0        0     4541 2022-11-12 18:33:53.217570 nbproject-0.9.0/nbproject/dev/_meta_store.py
--rw-r--r--   0        0        0     5242 2023-06-15 19:08:05.361229 nbproject-0.9.0/nbproject/dev/_metadata_display.py
--rw-r--r--   0        0        0      922 2022-07-15 19:53:53.061564 nbproject-0.9.0/nbproject/dev/_notebook.py
--rw-r--r--   0        0        0     3900 2022-07-23 14:31:43.204220 nbproject-0.9.0/nbproject/dev/_pypackage.py
--rw-r--r--   0        0        0      575 2022-11-12 18:52:44.681103 nbproject-0.9.0/nbproject/dev/_set_version.py
--rw-r--r--   0        0        0      532 2023-06-15 19:08:05.361346 nbproject-0.9.0/noxfile.py
--rw-r--r--   0        0        0     1071 2023-06-15 19:08:05.361460 nbproject-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      920 2022-09-06 11:40:41.175303 nbproject-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0     2428 2022-09-06 11:40:41.175526 nbproject-0.9.0/tests/test_cli.py
--rw-r--r--   0        0        0     1472 2023-04-17 07:11:01.416978 nbproject-0.9.0/tests/test_jupyter.py
--rw-r--r--   0        0        0      322 2023-06-04 20:57:48.695931 nbproject-0.9.0/tests/test_notebooks.py
--rw-r--r--   0        0        0      303 2022-11-12 18:52:44.681259 nbproject-0.9.0/tests/test_set_version.py
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 nbproject-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2475 2023-06-15 19:08:05.360108 nbproject-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-06-10 19:50:58.313927 nbproject-0.9.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-06-10 19:50:58.314964 nbproject-0.9.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1880 2022-07-10 12:10:29.382368 nbproject-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1645 2022-08-29 09:33:05.135542 nbproject-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      740 2022-10-24 12:29:45.346974 nbproject-0.9.1/CITATION.cff
+-rw-r--r--   0        0        0    11357 2022-04-18 20:46:44.681265 nbproject-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1374 2023-08-04 20:32:42.822118 nbproject-0.9.1/README.md
+-rw-r--r--   0        0        0    20948 2023-08-04 20:33:09.651587 nbproject-0.9.1/docs/changelog.md
+-rw-r--r--   0        0        0     1216 2023-08-04 20:32:42.822676 nbproject-0.9.1/docs/faq.md
+-rw-r--r--   0        0        0     1874 2023-08-04 20:19:19.961650 nbproject-0.9.1/docs/faq/example-after-init-set-filename.ipynb
+-rw-r--r--   0        0        0      153 2023-08-04 20:32:42.823012 nbproject-0.9.1/docs/faq/example-project-uninitialized.md
+-rw-r--r--   0        0        0     1481 2023-08-04 20:19:19.962250 nbproject-0.9.1/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
+-rw-r--r--   0        0        0      117 2023-08-04 20:32:42.823159 nbproject-0.9.1/docs/faq/example-project.md
+-rw-r--r--   0        0        0     1874 2023-08-04 20:19:19.963880 nbproject-0.9.1/docs/faq/example-project/2022-05-13-my-task-x.ipynb
+-rw-r--r--   0        0        0     1661 2023-08-04 20:19:19.964730 nbproject-0.9.1/docs/faq/example-project/2022-07-18-my-task-y.ipynb
+-rw-r--r--   0        0        0      364 2023-08-04 20:19:19.965113 nbproject-0.9.1/docs/faq/example-project/nbproject_metadata.yml
+-rw-r--r--   0        0        0     1873 2023-08-04 20:19:19.965699 nbproject-0.9.1/docs/faq/header-author-field.ipynb
+-rw-r--r--   0        0        0     1520 2023-08-04 20:19:19.966010 nbproject-0.9.1/docs/faq/inconsistent-packages-parents-no-store.ipynb
+-rw-r--r--   0        0        0     2330 2023-08-04 20:19:19.966373 nbproject-0.9.1/docs/faq/inconsistent-packages-parents-store.ipynb
+-rw-r--r--   0        0        0     1311 2023-08-04 20:19:19.967100 nbproject-0.9.1/docs/faq/initialize-set-env.ipynb
+-rw-r--r--   0        0        0     2049 2023-08-04 20:19:19.967641 nbproject-0.9.1/docs/faq/initialize.ipynb
+-rw-r--r--   0        0        0     4086 2023-08-04 20:19:19.967960 nbproject-0.9.1/docs/faq/internal-functions.ipynb
+-rw-r--r--   0        0        0     2708 2023-08-04 20:19:19.968582 nbproject-0.9.1/docs/faq/not-initialized.ipynb
+-rw-r--r--   0        0        0     1803 2023-08-04 20:19:19.968950 nbproject-0.9.1/docs/faq/publish-not-last-cell.ipynb
+-rw-r--r--   0        0        0     1399 2023-08-04 20:19:19.969256 nbproject-0.9.1/docs/faq/publish-set-version.ipynb
+-rw-r--r--   0        0        0     1818 2023-08-04 20:19:19.969587 nbproject-0.9.1/docs/faq/publish-without-saving.ipynb
+-rw-r--r--   0        0        0     1787 2023-08-04 20:19:19.969884 nbproject-0.9.1/docs/faq/publish-without-title.ipynb
+-rw-r--r--   0        0        0     1653 2023-08-04 20:19:19.970180 nbproject-0.9.1/docs/faq/publish-wrapper.ipynb
+-rw-r--r--   0        0        0     1577 2023-08-04 20:19:19.970709 nbproject-0.9.1/docs/faq/set-env-via-environment-var.ipynb
+-rw-r--r--   0        0        0      679 2022-10-10 14:54:28.366976 nbproject-0.9.1/docs/faq/setup.md
+-rw-r--r--   0        0        0     1357 2023-08-04 20:19:19.971363 nbproject-0.9.1/docs/faq/trigger-exit-upon-init.ipynb
+-rw-r--r--   0        0        0      317 2023-08-04 20:32:42.823391 nbproject-0.9.1/docs/guide.md
+-rw-r--r--   0        0        0     2694 2023-08-04 20:19:19.971912 nbproject-0.9.1/docs/guide/basic-metadata.ipynb
+-rw-r--r--   0        0        0     4639 2023-08-04 20:19:19.972453 nbproject-0.9.1/docs/guide/meta.ipynb
+-rw-r--r--   0        0        0     1637 2023-08-04 20:19:19.972875 nbproject-0.9.1/docs/guide/received.ipynb
+-rw-r--r--   0        0        0     2964 2023-08-04 20:19:19.973146 nbproject-0.9.1/docs/guide/update-metadata.ipynb
+-rw-r--r--   0        0        0      130 2023-08-04 20:32:42.823650 nbproject-0.9.1/docs/index.md
+-rw-r--r--   0        0        0     2755 2023-08-04 20:19:19.973501 nbproject-0.9.1/docs/quickstart.ipynb
+-rw-r--r--   0        0        0       57 2023-04-17 07:11:01.413670 nbproject-0.9.1/docs/reference.md
+-rw-r--r--   0        0        0      137 2022-06-01 14:27:38.468097 nbproject-0.9.1/lamin-project.yaml
+-rw-r--r--   0        0        0      763 2023-08-04 20:33:32.020959 nbproject-0.9.1/nbproject/__init__.py
+-rw-r--r--   0        0        0     1631 2022-08-17 11:48:35.494040 nbproject-0.9.1/nbproject/__main__.py
+-rw-r--r--   0        0        0     5121 2022-11-12 18:33:53.216715 nbproject-0.9.1/nbproject/_cli.py
+-rw-r--r--   0        0        0     5756 2023-07-02 08:17:43.608229 nbproject-0.9.1/nbproject/_header.py
+-rw-r--r--   0        0        0      285 2022-11-13 23:00:04.437788 nbproject-0.9.1/nbproject/_is_run_from_ipython.py
+-rw-r--r--   0        0        0       47 2023-08-04 20:32:42.823933 nbproject-0.9.1/nbproject/_logger.py
+-rw-r--r--   0        0        0     3080 2022-10-10 12:03:49.455892 nbproject-0.9.1/nbproject/_meta.py
+-rw-r--r--   0        0        0     3943 2022-11-12 18:52:44.680900 nbproject-0.9.1/nbproject/_publish.py
+-rw-r--r--   0        0        0     4007 2022-11-12 18:33:53.217134 nbproject-0.9.1/nbproject/_schemas.py
+-rw-r--r--   0        0        0      836 2023-06-04 20:57:48.693471 nbproject-0.9.1/nbproject/dev/__init__.py
+-rw-r--r--   0        0        0      590 2022-10-07 21:00:16.805272 nbproject-0.9.1/nbproject/dev/_check_last_cell.py
+-rw-r--r--   0        0        0      681 2022-08-17 11:48:35.496655 nbproject-0.9.1/nbproject/dev/_classic_nb_commands.py
+-rw-r--r--   0        0        0     1473 2023-06-04 20:57:48.693977 nbproject-0.9.1/nbproject/dev/_consecutiveness.py
+-rw-r--r--   0        0        0      525 2022-08-17 11:48:35.496751 nbproject-0.9.1/nbproject/dev/_frontend_commands.py
+-rw-r--r--   0        0        0     1843 2023-06-04 20:57:48.694457 nbproject-0.9.1/nbproject/dev/_initialize.py
+-rw-r--r--   0        0        0     5137 2023-06-13 15:37:27.141838 nbproject-0.9.1/nbproject/dev/_jupyter_communicate.py
+-rw-r--r--   0        0        0      822 2023-04-17 07:11:01.415333 nbproject-0.9.1/nbproject/dev/_jupyter_lab_commands.py
+-rw-r--r--   0        0        0      343 2023-04-17 07:11:01.415771 nbproject-0.9.1/nbproject/dev/_lamin_communicate.py
+-rw-r--r--   0        0        0     3642 2022-10-10 18:44:26.046429 nbproject-0.9.1/nbproject/dev/_meta_live.py
+-rw-r--r--   0        0        0     4541 2022-11-12 18:33:53.217570 nbproject-0.9.1/nbproject/dev/_meta_store.py
+-rw-r--r--   0        0        0     5242 2023-06-15 19:08:05.361229 nbproject-0.9.1/nbproject/dev/_metadata_display.py
+-rw-r--r--   0        0        0      922 2022-07-15 19:53:53.061564 nbproject-0.9.1/nbproject/dev/_notebook.py
+-rw-r--r--   0        0        0     3900 2022-07-23 14:31:43.204220 nbproject-0.9.1/nbproject/dev/_pypackage.py
+-rw-r--r--   0        0        0      575 2022-11-12 18:52:44.681103 nbproject-0.9.1/nbproject/dev/_set_version.py
+-rw-r--r--   0        0        0      483 2023-08-04 19:43:05.490269 nbproject-0.9.1/noxfile.py
+-rw-r--r--   0        0        0     1076 2023-08-04 20:32:42.824213 nbproject-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      920 2022-09-06 11:40:41.175303 nbproject-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     2428 2022-09-06 11:40:41.175526 nbproject-0.9.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1472 2023-04-17 07:11:01.416978 nbproject-0.9.1/tests/test_jupyter.py
+-rw-r--r--   0        0        0      322 2023-06-04 20:57:48.695931 nbproject-0.9.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0      303 2022-11-12 18:52:44.681259 nbproject-0.9.1/tests/test_set_version.py
+-rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 nbproject-0.9.1/PKG-INFO
```

### Comparing `nbproject-0.9.0/.github/workflows/build.yml` & `nbproject-0.9.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/.github/workflows/latest-changes.yml` & `nbproject-0.9.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/.gitignore` & `nbproject-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/.pre-commit-config.yaml` & `nbproject-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/CITATION.cff` & `nbproject-0.9.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/LICENSE` & `nbproject-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/changelog.md` & `nbproject-0.9.1/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+📝 Simplify docs, adopt new lamin.ai static site architecture | [269](https://github.com/laminlabs/nbproject/pull/269) | [falexwolf](https://github.com/falexwolf) | 2023-08-04 | 0.9.1
 ♻️ Remove loguru-dependent call, expand `metadata_only` return signature | [268](https://github.com/laminlabs/nbproject/pull/268) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.9.0
 📝 Position nbproject | [264](https://github.com/laminlabs/nbproject/pull/264) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 |
 🩹 Try to get vs code path first | [267](https://github.com/laminlabs/nbproject/pull/267) | [Koncopd](https://github.com/Koncopd) | 2023-06-10 |
 🦺 Safer parsing during initialization | [266](https://github.com/laminlabs/nbproject/pull/266) | [Koncopd](https://github.com/Koncopd) | 2023-06-03 | 0.8.7
 ➖ Remove nbproject-test from dependencies | [262](https://github.com/laminlabs/nbproject/pull/262) | [Koncopd](https://github.com/Koncopd) | 2023-05-30 |
 🐛 Safer ipylab initialization | [263](https://github.com/laminlabs/nbproject/pull/263) | [Koncopd](https://github.com/Koncopd) | 2023-04-18 | 0.8.6
 🐛 Fix VS Code integration for recent VS Code versions | [260](https://github.com/laminlabs/nbproject/pull/260) | [Koncopd](https://github.com/Koncopd) | 2023-04-17 | 0.8.5
```

### Comparing `nbproject-0.9.0/docs/faq/example-after-init-set-filename.ipynb` & `nbproject-0.9.1/docs/faq/example-after-init-set-filename.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb` & `nbproject-0.9.1/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/example-project/2022-05-13-my-task-x.ipynb` & `nbproject-0.9.1/docs/faq/example-project/2022-05-13-my-task-x.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/example-project/2022-07-18-my-task-y.ipynb` & `nbproject-0.9.1/docs/faq/example-project/2022-07-18-my-task-y.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/header-author-field.ipynb` & `nbproject-0.9.1/docs/faq/header-author-field.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/inconsistent-packages-parents-no-store.ipynb` & `nbproject-0.9.1/docs/faq/inconsistent-packages-parents-no-store.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/inconsistent-packages-parents-store.ipynb` & `nbproject-0.9.1/docs/faq/inconsistent-packages-parents-store.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/initialize-set-env.ipynb` & `nbproject-0.9.1/docs/faq/initialize-set-env.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/initialize.ipynb` & `nbproject-0.9.1/docs/faq/initialize.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/internal-functions.ipynb` & `nbproject-0.9.1/docs/faq/internal-functions.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/not-initialized.ipynb` & `nbproject-0.9.1/docs/faq/not-initialized.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/publish-not-last-cell.ipynb` & `nbproject-0.9.1/docs/faq/publish-not-last-cell.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/publish-set-version.ipynb` & `nbproject-0.9.1/docs/faq/publish-set-version.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/publish-without-saving.ipynb` & `nbproject-0.9.1/docs/faq/publish-without-saving.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/publish-without-title.ipynb` & `nbproject-0.9.1/docs/faq/publish-without-title.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/publish-wrapper.ipynb` & `nbproject-0.9.1/docs/faq/publish-wrapper.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/set-env-via-environment-var.ipynb` & `nbproject-0.9.1/docs/faq/set-env-via-environment-var.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/setup.md` & `nbproject-0.9.1/docs/faq/setup.md`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/faq/trigger-exit-upon-init.ipynb` & `nbproject-0.9.1/docs/faq/trigger-exit-upon-init.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/guide/basic-metadata.ipynb` & `nbproject-0.9.1/docs/guide/basic-metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/guide/meta.ipynb` & `nbproject-0.9.1/docs/guide/meta.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/guide/received.ipynb` & `nbproject-0.9.1/docs/guide/received.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/guide/update-metadata.ipynb` & `nbproject-0.9.1/docs/guide/update-metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/docs/quickstart.ipynb` & `nbproject-0.9.1/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/__init__.py` & `nbproject-0.9.1/nbproject/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 .. autosummary::
    :toctree:
 
    meta
    dev
 
 """
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 # init jupyter lab frontend immediately on import
 # nothing happens if this is not jupyter lab
 from .dev._jupyter_lab_commands import _init_frontend
 
 # trying to init ipylab JupyterFrontEnd can lead to errors on jupyter notebook
 try:
```

### Comparing `nbproject-0.9.0/nbproject/__main__.py` & `nbproject-0.9.1/nbproject/__main__.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/_cli.py` & `nbproject-0.9.1/nbproject/_cli.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/_header.py` & `nbproject-0.9.1/nbproject/_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     # make time_run available through API
     time_run = datetime.now(timezone.utc)
     global _time_run, _filepath, _env
     _time_run, _filepath, _env = time_run, filepath, env
 
     # initialize
     if "nbproject" not in nb.metadata:
-        logger.info("Initializing.")
+        logger.info("Attaching notebook metadata")
 
         if env in ("lab", "notebook"):
             _save_notebook(env)
             nb = read_notebook(filepath)  # type: ignore
 
         metadata = initialize_metadata(nb, parent=parent, pypackage=pypackage).dict()
```

### Comparing `nbproject-0.9.0/nbproject/_meta.py` & `nbproject-0.9.1/nbproject/_meta.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/_publish.py` & `nbproject-0.9.1/nbproject/_publish.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/_schemas.py` & `nbproject-0.9.1/nbproject/_schemas.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/__init__.py` & `nbproject-0.9.1/nbproject/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_check_last_cell.py` & `nbproject-0.9.1/nbproject/dev/_check_last_cell.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_classic_nb_commands.py` & `nbproject-0.9.1/nbproject/dev/_classic_nb_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_consecutiveness.py` & `nbproject-0.9.1/nbproject/dev/_consecutiveness.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_frontend_commands.py` & `nbproject-0.9.1/nbproject/dev/_frontend_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_initialize.py` & `nbproject-0.9.1/nbproject/dev/_initialize.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_jupyter_communicate.py` & `nbproject-0.9.1/nbproject/dev/_jupyter_communicate.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_jupyter_lab_commands.py` & `nbproject-0.9.1/nbproject/dev/_jupyter_lab_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_meta_live.py` & `nbproject-0.9.1/nbproject/dev/_meta_live.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_meta_store.py` & `nbproject-0.9.1/nbproject/dev/_meta_store.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_metadata_display.py` & `nbproject-0.9.1/nbproject/dev/_metadata_display.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_notebook.py` & `nbproject-0.9.1/nbproject/dev/_notebook.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_pypackage.py` & `nbproject-0.9.1/nbproject/dev/_pypackage.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/nbproject/dev/_set_version.py` & `nbproject-0.9.1/nbproject/dev/_set_version.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/pyproject.toml` & `nbproject-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "pydantic",
+    "pydantic<2.0.0",
     "pyyaml",
     "packaging",
     "orjson",
     "ipylab",
     "importlib-metadata",
     "stdlib_list; python_version < '3.10'",
-    "lamin_logger>=0.5.0",
+    "lamin_utils>=0.5.0",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/nbproject"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "black",
     "pytest>=6.0",
     "pytest-cov",
     "pandas",
     "nbformat",
-    "nbproject_test >= 0.2.0",
+    "nbproject_test >= 0.4.5",
 ]
 
 [project.scripts]
 nbproject = "nbproject.__main__:main"
 
 [tool.black]
 preview = true
```

### Comparing `nbproject-0.9.0/tests/conftest.py` & `nbproject-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/tests/test_cli.py` & `nbproject-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.9.0/tests/test_jupyter.py` & `nbproject-0.9.1/tests/test_jupyter.py`

 * *Files identical despite different names*

