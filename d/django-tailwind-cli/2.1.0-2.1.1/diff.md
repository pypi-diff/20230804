# Comparing `tmp/django_tailwind_cli-2.1.0.tar.gz` & `tmp/django_tailwind_cli-2.1.1.tar.gz`

## Comparing `django_tailwind_cli-2.1.0.tar` & `django_tailwind_cli-2.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/mkdocs.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/base_template.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/changelog.md
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/development.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/index.md
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/installation.md
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/settings.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/template_tags.md
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/__version__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/settings.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/test_management_commands.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/test_tailwind_css_tag.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/LICENSE
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/README.md
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/base_template.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/changelog.md
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/development.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/index.md
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/installation.md
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/settings.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/template_tags.md
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/__version__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/settings.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/test_management_commands.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/test_tailwind_css_tag.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/README.md
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/PKG-INFO
```

### Comparing `django_tailwind_cli-2.1.0/.pre-commit-config.yaml` & `django_tailwind_cli-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/CHANGELOG.md` & `django_tailwind_cli-2.1.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changelog
 
-## 2.1.0
+## 2.1.1
 
 - Switched from poetry to hatch for package management.
 
 ## 2.0.6
 
 - Bugfix for default tailwind.config.js.
```

### Comparing `django_tailwind_cli-2.1.0/mkdocs.yml` & `django_tailwind_cli-2.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/.github/workflows/publish.yml` & `django_tailwind_cli-2.1.1/.github/workflows/publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
       - name: Built
         run: hatch build
 
       - name: Publish
         env:
           HATCH_INDEX_USER: "__token__"
-          HATCH_INDEX_AUTH: "pypi-${{ secrets.PYPI_TOKEN }}"
+          HATCH_INDEX_AUTH: "${{ secrets.PYPI_TOKEN }}"
         run: hatch publish
 
       - name: Deploy docs
         uses: mhausenblas/mkdocs-deploy-gh-pages@master
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           CUSTOM_DOMAIN: django-tailwind-cli.andrich.me
```

### Comparing `django_tailwind_cli-2.1.0/.github/workflows/test.yml` & `django_tailwind_cli-2.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/docs/base_template.md` & `django_tailwind_cli-2.1.1/docs/base_template.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/docs/development.md` & `django_tailwind_cli-2.1.1/docs/development.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/docs/installation.md` & `django_tailwind_cli-2.1.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/docs/settings.md` & `django_tailwind_cli-2.1.1/docs/settings.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/docs/template_tags.md` & `django_tailwind_cli-2.1.1/docs/template_tags.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/docs/usage.md` & `django_tailwind_cli-2.1.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.1.1/src/django_tailwind_cli/utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.1.1/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/tests/settings.py` & `django_tailwind_cli-2.1.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/tests/test_management_commands.py` & `django_tailwind_cli-2.1.1/tests/test_management_commands.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/tests/test_tailwind_css_tag.py` & `django_tailwind_cli-2.1.1/tests/test_tailwind_css_tag.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/tests/test_utils.py` & `django_tailwind_cli-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/.gitignore` & `django_tailwind_cli-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/LICENSE` & `django_tailwind_cli-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/README.md` & `django_tailwind_cli-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/pyproject.toml` & `django_tailwind_cli-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.0/PKG-INFO` & `django_tailwind_cli-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.1.0
+Version: 2.1.1
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Project-URL: Documentation, https://django-tailwind-cli.andrich.me/
 Project-URL: Issues, https://github.com/oliverandrich/django-tailwind-cli/issues
 Project-URL: Source, https://github.com/oliverandrich/django-tailwind-cli
 Author-email: Oliver Andrich <oliver@andrich.me>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.1.0 Summary: Django
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.1.1 Summary: Django
 and Tailwind integration based on the prebuilt Tailwind CSS CLI. Project-URL:
 Documentation, https://django-tailwind-cli.andrich.me/ Project-URL: Issues,
 https://github.com/oliverandrich/django-tailwind-cli/issues Project-URL:
 Source, https://github.com/oliverandrich/django-tailwind-cli Author-email:
 Oliver Andrich
 andrich.me> License-Expression: MIT License-File: LICENSE Keywords:
 css,django,tailwind Classifier: Development Status :: 5 - Production/Stable
```

