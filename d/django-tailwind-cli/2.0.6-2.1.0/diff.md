# Comparing `tmp/django_tailwind_cli-2.0.6.tar.gz` & `tmp/django_tailwind_cli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-2.0.6.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django_tailwind_cli-2.0.6.tar` & `django_tailwind_cli-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,36 @@
--rw-r--r--   0        0        0     1071 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/LICENSE
--rw-r--r--   0        0        0     2776 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/README.md
--rw-r--r--   0        0        0     2432 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     7645 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0       79 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/styles.css
--rw-r--r--   0        0        0      436 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/tailwind.config.js
--rw-r--r--   0        0        0      518 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      420 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     3034 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/base_template.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/development.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/index.md
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/installation.md
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/settings.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/template_tags.md
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/docs/usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/__version__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/settings.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/test_management_commands.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/test_tailwind_css_tag.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/README.md
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.0/PKG-INFO
```

### Comparing `django_tailwind_cli-2.0.6/LICENSE` & `django_tailwind_cli-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.6/README.md` & `django_tailwind_cli-2.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # django-tailwind-cli
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oliverandrich/django-tailwind-cli/test.yml?style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/django-tailwind-cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-cli/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 ![GitHub](https://img.shields.io/github/license/oliverandrich/django-tailwind-cli?style=flat-square)
-[![poetry-managed](https://img.shields.io/badge/poetry-managed-blue?style=flat-square)](https://python-poetry.org)
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg?style=flat-square)](https://github.com/pypa/hatch)
 
 This library provides an integration of [Tailwind CSS](https://tailwindcss.com) for Django that is using on the precompiled versions of the [Tailwind CSS CLI](https://tailwindcss.com/blog/standalone-cli).
 
 The goal of this library is to provided the simplest possible Tailwind integration for your Django project. It took its inspiration from the [Tailwind integration for Phoenix](https://github.com/phoenixframework/tailwind) which completely skips the neccesity of a node installation.
 
 ## Installation
 
 1. Install the library.
 
-    ```shell
-    python -m pip install django-tailwind-cli
-    ```
+   ```shell
+   python -m pip install django-tailwind-cli
+   ```
 
 2. Add `django_tailwind_cli` to `INSTALLED_APPS` in `settings.py`.
 
-    ```python
-    INSTALLED_APPS = [
-        # other Django apps
-        "django_tailwind_cli",
-    ]
-    ```
+   ```python
+   INSTALLED_APPS = [
+       # other Django apps
+       "django_tailwind_cli",
+   ]
+   ```
 
 3. Configure the `STATICFILES_DIRS` parameter in your `settings.py` if not already configured.
 
-    ```python
-    STATICFILES_DIRS = [BASE_DIR / "assets"]
-    ```
+   ```python
+   STATICFILES_DIRS = [BASE_DIR / "assets"]
+   ```
 
 4. Add template code.
 
-    ```htmldjango
-    {% load tailwind_cli %}
-    ...
-    <head>
-      ...
-      {% tailwind_css %}
-      ...
-    </head>
-    ```
+   ```htmldjango
+   {% load tailwind_cli %}
+   ...
+   <head>
+     ...
+     {% tailwind_css %}
+     ...
+   </head>
+   ```
 
 5. Start the debug server.
 
-    ```shell
-    python manage.py tailwind runserver
-    ```
+   ```shell
+   python manage.py tailwind runserver
+   ```
 
 Enjoy!
 
 ## Features
 
--   Simplest possible integration.
--   Management commands:
-    -   To start the Tailwind CLI in watch mode during development.
-    -   To build the production grade CSS file for your project.
-    -   To start a debug server along with the Tailwind CLI in watch mode in a single session.
--   Necessary configuration to adapt the library to your project, when the defaults don't fit you.
--   A template tag to include the Tailwind CSS file in your project.
--   A base template for your project.
--   A sane tailwind.config.js that activates all the official plugins and includes a simple HTMX plugin.
+- Simplest possible integration.
+- Management commands:
+  - To start the Tailwind CLI in watch mode during development.
+  - To build the production grade CSS file for your project.
+  - To start a debug server along with the Tailwind CLI in watch mode in a single session.
+- Necessary configuration to adapt the library to your project, when the defaults don't fit you.
+- A template tag to include the Tailwind CSS file in your project.
+- A base template for your project.
+- A sane tailwind.config.js that activates all the official plugins and includes a simple HTMX plugin.
+
+## Requirements
+
+Python 3.8 or newer with Django >= 3.2.
 
 ## Documentation
 
 The documentation can be found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-cli.andrich.me/)
 
-## Requirements
+## Contributing
 
-Python 3.8 or newer with Django >= 3.2.
+If you want to contribute to this project, checkout the [development guide](https://django-tailwind-cli.andrich.me/development/) for details to get your dev environment up and running.
 
 ## License
 
 This software is licensed under [MIT license](https://github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 # django-tailwind-cli ![GitHub Workflow Status](https://img.shields.io/github/
 actions/workflow/status/oliverandrich/django-tailwind-cli/test.yml?style=flat-
 square) [![PyPI](https://img.shields.io/pypi/v/django-tailwind-
 cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-cli/) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/psf/black) ![GitHub](https://
 img.shields.io/github/license/oliverandrich/django-tailwind-cli?style=flat-
-square) [![poetry-managed](https://img.shields.io/badge/poetry-managed-
-blue?style=flat-square)](https://python-poetry.org) This library provides an
-integration of [Tailwind CSS](https://tailwindcss.com) for Django that is using
-on the precompiled versions of the [Tailwind CSS CLI](https://tailwindcss.com/
-blog/standalone-cli). The goal of this library is to provided the simplest
-possible Tailwind integration for your Django project. It took its inspiration
-from the [Tailwind integration for Phoenix](https://github.com/
+square) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-
+4051b5.svg?style=flat-square)](https://github.com/pypa/hatch) This library
+provides an integration of [Tailwind CSS](https://tailwindcss.com) for Django
+that is using on the precompiled versions of the [Tailwind CSS CLI](https://
+tailwindcss.com/blog/standalone-cli). The goal of this library is to provided
+the simplest possible Tailwind integration for your Django project. It took its
+inspiration from the [Tailwind integration for Phoenix](https://github.com/
 phoenixframework/tailwind) which completely skips the neccesity of a node
 installation. ## Installation 1. Install the library. ```shell python -m pip
 install django-tailwind-cli ``` 2. Add `django_tailwind_cli` to
 `INSTALLED_APPS` in `settings.py`. ```python INSTALLED_APPS = [ # other Django
 apps "django_tailwind_cli", ] ``` 3. Configure the `STATICFILES_DIRS` parameter
 in your `settings.py` if not already configured. ```python STATICFILES_DIRS =
 [BASE_DIR / "assets"] ``` 4. Add template code. ```htmldjango {% load
@@ -25,12 +25,15 @@
 Enjoy! ## Features - Simplest possible integration. - Management commands: - To
 start the Tailwind CLI in watch mode during development. - To build the
 production grade CSS file for your project. - To start a debug server along
 with the Tailwind CLI in watch mode in a single session. - Necessary
 configuration to adapt the library to your project, when the defaults don't fit
 you. - A template tag to include the Tailwind CSS file in your project. - A
 base template for your project. - A sane tailwind.config.js that activates all
-the official plugins and includes a simple HTMX plugin. ## Documentation The
-documentation can be found at [https://django-tailwind-cli.andrich.me/](https:/
-/django-tailwind-cli.andrich.me/) ## Requirements Python 3.8 or newer with
-Django >= 3.2. ## License This software is licensed under [MIT license](https:/
-/github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
+the official plugins and includes a simple HTMX plugin. ## Requirements Python
+3.8 or newer with Django >= 3.2. ## Documentation The documentation can be
+found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-
+cli.andrich.me/) ## Contributing If you want to contribute to this project,
+checkout the [development guide](https://django-tailwind-cli.andrich.me/
+development/) for details to get your dev environment up and running. ##
+License This software is licensed under [MIT license](https://github.com/
+oliverandrich/django-tailwind-cli/blob/main/LICENSE).
```

### Comparing `django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-2.1.0/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,78 +14,79 @@
 
 from django_tailwind_cli.utils import Config
 
 
 class Command(BaseCommand):
     """Create and manage a Tailwind CSS theme."""
 
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
+    def __init__(self, *args: Any, **kwargs: Any):
         """Initialize the command."""
 
         super().__init__(*args, **kwargs)
 
         # Get the config from the settings and validate it.
         self.config = Config()
         try:
             self.config.validate_settings()
         except Exception as e:
-            raise CommandError("Configuration error") from e
+            msg = "Configuration error"
+            raise CommandError(msg) from e
 
     def add_arguments(self, parser: Any) -> None:
         """Add arguments to the command."""
         subparsers = parser.add_subparsers(dest="tailwind", required=True)
 
         subparsers.add_parser("build", help="Build a minified production ready CSS file.")
 
         subparsers.add_parser("watch", help="Start Tailwind CLI in watch mode during development.")
 
         runserver_parser = subparsers.add_parser(
             "runserver", help="Start the Django development server and the Tailwind CLI in watch mode."
         )
         runserver_parser.add_argument("addrport", nargs="?", help="Optional port number, or ipaddr:port")
 
-    def handle(self, *args: Any, **kwargs: Any) -> None:
+    def handle(self, *_args: Any, **kwargs: Any) -> None:
         """Perform the command's actions."""
 
         # Get the subcommand from the kwargs.
         label = kwargs.get("tailwind")
         del kwargs["tailwind"]
 
         # Before running the actual subcommand, we need to make sure that the CLI is installed and
         # the config file exists.
         self._download_cli_if_not_exists()
         self._create_tailwind_config_if_not_exists()
 
         # Start the subcommand.
         if label == "build":
-            self.build(*args[1:], **kwargs)
+            self.build()
         elif label == "watch":
-            self.watch(*args[1:], **kwargs)
+            self.watch()
         elif label == "runserver":  # pragma: no cover
-            self.runserver(*args[1:], **kwargs)
+            self.runserver(**kwargs)
 
-    def build(self, *args: Any, **kwargs: Any) -> None:
+    def build(self) -> None:
         """Build a minified production ready CSS file."""
         try:
-            subprocess.run(self.get_build_cmd(), cwd=settings.BASE_DIR, check=True)
+            subprocess.run(self.get_build_cmd(), cwd=settings.BASE_DIR, check=True)  # noqa: S603
         except KeyboardInterrupt:
             self.stdout.write(self.style.ERROR("Canceled building production stylesheet."))
         else:
             self.stdout.write(
                 self.style.SUCCESS(f"Built production stylesheet '{self.config.get_full_dist_css_path()}'.")
             )
 
-    def watch(self, *args: Any, **kwargs: Any) -> None:
+    def watch(self) -> None:
         """Start Tailwind CLI in watch mode during development."""
         try:
-            subprocess.run(self.get_watch_cmd(), cwd=settings.BASE_DIR, check=True)
+            subprocess.run(self.get_watch_cmd(), cwd=settings.BASE_DIR, check=True)  # noqa: S603
         except KeyboardInterrupt:
             self.stdout.write(self.style.SUCCESS("Stopped watching for changes."))
 
-    def runserver(self, *args: Any, **kwargs: Any) -> None:  # pragma: no cover
+    def runserver(self, **kwargs: Any) -> None:  # pragma: no cover
         """Start the Django development server and the Tailwind CLI in watch mode."""
 
         # Start the watch process in a separate process.
         watch_cmd = [sys.executable, "manage.py", "tailwind", "watch"]
         watch_process = Process(
             target=subprocess.run,
             args=(watch_cmd,),
@@ -160,15 +161,15 @@
         download_url = self.config.get_download_url()
 
         if not dest_file.exists():
             self.stdout.write(self.style.ERROR("Tailwind CSS CLI not found."))
             self.stdout.write(self.style.WARNING(f"Downloading Tailwind CSS CLI from '{download_url}'"))
             dest_file.parent.mkdir(parents=True, exist_ok=True)
             certifi_context = ssl.create_default_context(cafile=certifi.where())
-            with urllib.request.urlopen(download_url, context=certifi_context) as source, dest_file.open(
+            with urllib.request.urlopen(download_url, context=certifi_context) as source, dest_file.open(  # noqa: S310
                 mode="wb"
             ) as dest:
                 shutil.copyfileobj(source, dest)
             # make cli executable
             dest_file.chmod(0o755)
             self.stdout.write(self.style.SUCCESS(f"Downloaded Tailwind CSS CLI to '{dest_file}'"))
```

### Comparing `django_tailwind_cli-2.0.6/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.1.0/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% load tailwind_cli %}
 <!DOCTYPE html>
 <html lang="{{ LANGUAGE_CODE }}">
-  <head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>{% block title %}Home{% endblock title %}</title>
-    {% tailwind_css%}
-    {% block extra_head %}{% endblock extra_head %}
-  </head>
-  <body>
-    {% block content %}
-    {% endblock content %}
-    {% block extra_body %}{% endblock extra_body %}
-  </body>
+    <head>
+        <meta charset="UTF-8">
+        <meta http-equiv="X-UA-Compatible" content="IE=edge">
+        <meta name="viewport" content="width=device-width, initial-scale=1.0">
+        <title>{% block title %}Home{% endblock title %}</title>
+        {% tailwind_css%}
+        {% block extra_head %}{% endblock extra_head %}
+    </head>
+    <body>
+        {% block content %}
+        {% endblock content %}
+        {% block extra_body %}{% endblock extra_body %}
+    </body>
 </html>
```

### Comparing `django_tailwind_cli-2.0.6/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.1.0/src/django_tailwind_cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 from django.conf import settings
 
 
 class Config:
     """Configuration for the Tailwind CSS CLI."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the configuration."""
         self.tailwind_version: str = getattr(settings, "TAILWIND_CLI_VERSION", "3.3.3")
         self.cli_path: Union[str, None] = getattr(settings, "TAILWIND_CLI_PATH", "~/.local/bin/")
         self.src_css: Union[str, None] = getattr(settings, "TAILWIND_CLI_SRC_CSS", None)
         self.dist_css: str = getattr(settings, "TAILWIND_CLI_DIST_CSS", "css/tailwind.css")
         self.config_file: str = getattr(settings, "TAILWIND_CLI_CONFIG_FILE", "tailwind.config.js")
 
     def validate_settings(self) -> None:
         """Validate the settings."""
         if settings.STATICFILES_DIRS is None or len(settings.STATICFILES_DIRS) == 0:
-            raise ValueError("STATICFILES_DIRS is empty. Please add a path to your static files.")
+            msg = "STATICFILES_DIRS is empty. Please add a path to your static files."
+            raise ValueError(msg)
 
     def get_system_and_machine(self) -> Tuple[str, str]:
         """Get the system and machine name."""
         system = platform.system().lower()
         if system == "darwin":  # pragma: no cover
             system = "macos"
 
@@ -56,20 +57,22 @@
             return Path(settings.BASE_DIR) / executable_name
         else:
             return Path(self.cli_path).expanduser() / executable_name
 
     def get_full_src_css_path(self) -> Path:
         """Get path to the source css."""
         if self.src_css is None:
-            raise ValueError("No source CSS file specified. Please set TAILWIND_SRC_CSS in your settings.")
+            msg = "No source CSS file specified. Please set TAILWIND_SRC_CSS in your settings."
+            raise ValueError(msg)
         return Path(settings.BASE_DIR) / self.src_css
 
     def get_full_dist_css_path(self) -> Path:
         """Get path to the compiled css."""
         if settings.STATICFILES_DIRS is None or len(settings.STATICFILES_DIRS) == 0:
-            raise ValueError("STATICFILES_DIRS is empty. Please add a path to your static files.")
+            msg = "STATICFILES_DIRS is empty. Please add a path to your static files."
+            raise ValueError(msg)
 
         return Path(settings.STATICFILES_DIRS[0]) / self.dist_css
 
     def get_full_config_file_path(self) -> Path:
         """Get path to the tailwind.config.js file."""
         return Path(settings.BASE_DIR) / self.config_file
```

### Comparing `django_tailwind_cli-2.0.6/PKG-INFO` & `django_tailwind_cli-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,113 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.0.6
+Version: 2.1.0
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
-Home-page: https://oliverandrich.github.io/django-tailwind-cli/
-License: MIT
-Keywords: django,tailwind,css
-Author: Oliver Andrich
-Author-email: oliver@andrich.me
-Requires-Python: >=3.8,<4
+Project-URL: Documentation, https://django-tailwind-cli.andrich.me/
+Project-URL: Issues, https://github.com/oliverandrich/django-tailwind-cli/issues
+Project-URL: Source, https://github.com/oliverandrich/django-tailwind-cli
+Author-email: Oliver Andrich <oliver@andrich.me>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: css,django,tailwind
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
+Requires-Python: >=3.8
 Requires-Dist: certifi
-Requires-Dist: django (>=3.2,<4.3)
-Project-URL: Mastodon, https://2pxnl.de/@oliver
-Project-URL: Repository, https://github.com/oliverandrich/django-tailwind-cli
+Requires-Dist: django<5.0,>=3.2
 Description-Content-Type: text/markdown
 
 # django-tailwind-cli
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oliverandrich/django-tailwind-cli/test.yml?style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/django-tailwind-cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-cli/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 ![GitHub](https://img.shields.io/github/license/oliverandrich/django-tailwind-cli?style=flat-square)
-[![poetry-managed](https://img.shields.io/badge/poetry-managed-blue?style=flat-square)](https://python-poetry.org)
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg?style=flat-square)](https://github.com/pypa/hatch)
 
 This library provides an integration of [Tailwind CSS](https://tailwindcss.com) for Django that is using on the precompiled versions of the [Tailwind CSS CLI](https://tailwindcss.com/blog/standalone-cli).
 
 The goal of this library is to provided the simplest possible Tailwind integration for your Django project. It took its inspiration from the [Tailwind integration for Phoenix](https://github.com/phoenixframework/tailwind) which completely skips the neccesity of a node installation.
 
 ## Installation
 
 1. Install the library.
 
-    ```shell
-    python -m pip install django-tailwind-cli
-    ```
+   ```shell
+   python -m pip install django-tailwind-cli
+   ```
 
 2. Add `django_tailwind_cli` to `INSTALLED_APPS` in `settings.py`.
 
-    ```python
-    INSTALLED_APPS = [
-        # other Django apps
-        "django_tailwind_cli",
-    ]
-    ```
+   ```python
+   INSTALLED_APPS = [
+       # other Django apps
+       "django_tailwind_cli",
+   ]
+   ```
 
 3. Configure the `STATICFILES_DIRS` parameter in your `settings.py` if not already configured.
 
-    ```python
-    STATICFILES_DIRS = [BASE_DIR / "assets"]
-    ```
+   ```python
+   STATICFILES_DIRS = [BASE_DIR / "assets"]
+   ```
 
 4. Add template code.
 
-    ```htmldjango
-    {% load tailwind_cli %}
-    ...
-    <head>
-      ...
-      {% tailwind_css %}
-      ...
-    </head>
-    ```
+   ```htmldjango
+   {% load tailwind_cli %}
+   ...
+   <head>
+     ...
+     {% tailwind_css %}
+     ...
+   </head>
+   ```
 
 5. Start the debug server.
 
-    ```shell
-    python manage.py tailwind runserver
-    ```
+   ```shell
+   python manage.py tailwind runserver
+   ```
 
 Enjoy!
 
 ## Features
 
--   Simplest possible integration.
--   Management commands:
-    -   To start the Tailwind CLI in watch mode during development.
-    -   To build the production grade CSS file for your project.
-    -   To start a debug server along with the Tailwind CLI in watch mode in a single session.
--   Necessary configuration to adapt the library to your project, when the defaults don't fit you.
--   A template tag to include the Tailwind CSS file in your project.
--   A base template for your project.
--   A sane tailwind.config.js that activates all the official plugins and includes a simple HTMX plugin.
+- Simplest possible integration.
+- Management commands:
+  - To start the Tailwind CLI in watch mode during development.
+  - To build the production grade CSS file for your project.
+  - To start a debug server along with the Tailwind CLI in watch mode in a single session.
+- Necessary configuration to adapt the library to your project, when the defaults don't fit you.
+- A template tag to include the Tailwind CSS file in your project.
+- A base template for your project.
+- A sane tailwind.config.js that activates all the official plugins and includes a simple HTMX plugin.
+
+## Requirements
+
+Python 3.8 or newer with Django >= 3.2.
 
 ## Documentation
 
 The documentation can be found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-cli.andrich.me/)
 
-## Requirements
+## Contributing
 
-Python 3.8 or newer with Django >= 3.2.
+If you want to contribute to this project, checkout the [development guide](https://django-tailwind-cli.andrich.me/development/) for details to get your dev environment up and running.
 
 ## License
 
 This software is licensed under [MIT license](https://github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
-
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.0.6 Summary: Django
-and Tailwind integration based on the prebuilt Tailwind CSS CLI. Home-page:
-https://oliverandrich.github.io/django-tailwind-cli/ License: MIT Keywords:
-django,tailwind,css Author: Oliver Andrich Author-email: oliver@andrich.me
-Requires-Python: >=3.8,<4 Classifier: Development Status :: 5 - Production/
-Stable Classifier: Environment :: Web Environment Classifier: Framework ::
-Django :: 3.2 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
-Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: License
-:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Utilities Requires-Dist: certifi Requires-Dist: django (>=3.2,<4.3) Project-
-URL: Mastodon, https://2pxnl.de/@oliver Project-URL: Repository, https://
-github.com/oliverandrich/django-tailwind-cli Description-Content-Type: text/
-markdown # django-tailwind-cli ![GitHub Workflow Status](https://
-img.shields.io/github/actions/workflow/status/oliverandrich/django-tailwind-
-cli/test.yml?style=flat-square) [![PyPI](https://img.shields.io/pypi/v/django-
-tailwind-cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-
-cli/) [![Code style: black](https://img.shields.io/badge/code%20style-black-
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.1.0 Summary: Django
+and Tailwind integration based on the prebuilt Tailwind CSS CLI. Project-URL:
+Documentation, https://django-tailwind-cli.andrich.me/ Project-URL: Issues,
+https://github.com/oliverandrich/django-tailwind-cli/issues Project-URL:
+Source, https://github.com/oliverandrich/django-tailwind-cli Author-email:
+Oliver Andrich
+andrich.me> License-Expression: MIT License-File: LICENSE Keywords:
+css,django,tailwind Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment Classifier: Framework :: Django ::
+3.2 Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django ::
+4.2 Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Utilities Requires-Python: >=3.8 Requires-Dist:
+certifi Requires-Dist: django<5.0,>=3.2 Description-Content-Type: text/markdown
+# django-tailwind-cli ![GitHub Workflow Status](https://img.shields.io/github/
+actions/workflow/status/oliverandrich/django-tailwind-cli/test.yml?style=flat-
+square) [![PyPI](https://img.shields.io/pypi/v/django-tailwind-
+cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-cli/) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/psf/black) ![GitHub](https://
 img.shields.io/github/license/oliverandrich/django-tailwind-cli?style=flat-
-square) [![poetry-managed](https://img.shields.io/badge/poetry-managed-
-blue?style=flat-square)](https://python-poetry.org) This library provides an
-integration of [Tailwind CSS](https://tailwindcss.com) for Django that is using
-on the precompiled versions of the [Tailwind CSS CLI](https://tailwindcss.com/
-blog/standalone-cli). The goal of this library is to provided the simplest
-possible Tailwind integration for your Django project. It took its inspiration
-from the [Tailwind integration for Phoenix](https://github.com/
+square) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-
+4051b5.svg?style=flat-square)](https://github.com/pypa/hatch) This library
+provides an integration of [Tailwind CSS](https://tailwindcss.com) for Django
+that is using on the precompiled versions of the [Tailwind CSS CLI](https://
+tailwindcss.com/blog/standalone-cli). The goal of this library is to provided
+the simplest possible Tailwind integration for your Django project. It took its
+inspiration from the [Tailwind integration for Phoenix](https://github.com/
 phoenixframework/tailwind) which completely skips the neccesity of a node
 installation. ## Installation 1. Install the library. ```shell python -m pip
 install django-tailwind-cli ``` 2. Add `django_tailwind_cli` to
 `INSTALLED_APPS` in `settings.py`. ```python INSTALLED_APPS = [ # other Django
 apps "django_tailwind_cli", ] ``` 3. Configure the `STATICFILES_DIRS` parameter
 in your `settings.py` if not already configured. ```python STATICFILES_DIRS =
 [BASE_DIR / "assets"] ``` 4. Add template code. ```htmldjango {% load
@@ -42,12 +43,15 @@
 Enjoy! ## Features - Simplest possible integration. - Management commands: - To
 start the Tailwind CLI in watch mode during development. - To build the
 production grade CSS file for your project. - To start a debug server along
 with the Tailwind CLI in watch mode in a single session. - Necessary
 configuration to adapt the library to your project, when the defaults don't fit
 you. - A template tag to include the Tailwind CSS file in your project. - A
 base template for your project. - A sane tailwind.config.js that activates all
-the official plugins and includes a simple HTMX plugin. ## Documentation The
-documentation can be found at [https://django-tailwind-cli.andrich.me/](https:/
-/django-tailwind-cli.andrich.me/) ## Requirements Python 3.8 or newer with
-Django >= 3.2. ## License This software is licensed under [MIT license](https:/
-/github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
+the official plugins and includes a simple HTMX plugin. ## Requirements Python
+3.8 or newer with Django >= 3.2. ## Documentation The documentation can be
+found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-
+cli.andrich.me/) ## Contributing If you want to contribute to this project,
+checkout the [development guide](https://django-tailwind-cli.andrich.me/
+development/) for details to get your dev environment up and running. ##
+License This software is licensed under [MIT license](https://github.com/
+oliverandrich/django-tailwind-cli/blob/main/LICENSE).
```

