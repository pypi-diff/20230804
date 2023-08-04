# Comparing `tmp/robocorp_browser-2.0.1.tar.gz` & `tmp/robocorp_browser-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-2.0.1.tar", max compression
+gzip compressed data, was "robocorp_browser-2.1.0.tar", max compression
```

## Comparing `robocorp_browser-2.0.1.tar` & `robocorp_browser-2.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1786 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/README.md
--rw-r--r--   0        0        0      712 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6318 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0       81 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/src/robocorp/browser/__main__.py
--rw-r--r--   0        0        0     7104 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0     1890 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/src/robocorp/browser/_browser_engines.py
--rw-r--r--   0        0        0      825 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/src/robocorp/browser/cli.py
--rw-r--r--   0        0        0        0 2023-07-14 13:26:27.585406 robocorp_browser-2.0.1/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 robocorp_browser-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2210 2023-08-04 11:14:45.219672 robocorp_browser-2.1.0/docs/README.md
+-rw-r--r--   0        0        0      712 2023-08-04 11:14:45.219672 robocorp_browser-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8079 2023-08-04 11:14:45.219672 robocorp_browser-2.1.0/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0       81 2023-08-04 11:14:45.219672 robocorp_browser-2.1.0/src/robocorp/browser/__main__.py
+-rw-r--r--   0        0        0     7545 2023-08-04 11:14:45.219672 robocorp_browser-2.1.0/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0     1890 2023-08-04 11:14:45.223670 robocorp_browser-2.1.0/src/robocorp/browser/_browser_engines.py
+-rw-r--r--   0        0        0      825 2023-08-04 11:14:45.223670 robocorp_browser-2.1.0/src/robocorp/browser/cli.py
+-rw-r--r--   0        0        0        0 2023-08-04 11:14:45.223670 robocorp_browser-2.1.0/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 robocorp_browser-2.1.0/PKG-INFO
```

### Comparing `robocorp_browser-2.0.1/README.md` & `robocorp_browser-2.1.0/docs/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# Robocorp browser library
+# robocorp-browser
 
-The `robocorp-browser` library helps in automating browsers by providing 
-convenient APIs to manage the lifecycle of playwright objects using `robocorp-tasks`.
-
-
-The code below reflects the basic usage of the library:
+The `robocorp-browser` is a wrapper for the [Playwright](https://playwright.dev/python/)
+project, with quality-of-life improvements such as automatic lifecycle management
+for Playwright objects.
 
+## Getting started
 
 ```python
-from robocorp import browser
 from robocorp.tasks import task
+from robocorp import browser
 from robocorp import vault
 
 
 @task
 def browser_automate():
     # Configure may be used to set the basic robocorp.browser settings.
     # It must be called prior to calling APIs which create playwright objects.
@@ -22,32 +21,44 @@
         # If the browser_automate() function finishes with an exception it will
         # make a screenshot and embed it into the logs.
         screenshot="only-on-failure",
         
         # By default headless is False unless running in a Linux container
         # without a DISPLAY/WAYLAND_DISPLAY environment variable, but it
         # can also be manually specified.
-        # headless=True|False,
+        headless=True,
         
         # Interactions may be run in slow-motion (given in milliseconds).
-        # slowmo=100,
+        slowmo=100,
     )
 
     # browser.goto() may be used as a shortcut to get the current page and
     # go to some url (it may create the browser if still not created).
-    browser.goto("https://<target-page.com>")
+    browser.goto("https://example.com>")
 
     login()
 
 
 def login():
     # APIs in robocorp.browser return the same browser instance, which is
     # automatically closed when the task finishes.
     page = browser.page()
 
     # robocorp.vault is recommended for managing secrets.
-    password = vault.get_secret("default-account")["password"]
+    account = vault.get_secret("default-account")
 
     # Use the playwright Browser api as usual.
-    page.fill('//input[@ng-reflect-name="password"]', password)
+    page.fill('//input[@ng-reflect-name="password"]', account["password"])
     page.click("input:text('Submit')")
 ```
+
+## Guides
+
+- [Browser configuration](https://github.com/robocorp/robo/blob/master/browser/docs/guides/configuration.md)
+
+## API Reference
+
+Information on specific functions or classes: [robocorp.browser](https://github.com/robocorp/robo/blob/master/browser/docs/api/robocorp.browser.md)
+
+## Changelog
+
+A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robo/blob/master/browser/docs/CHANGELOG.md).
```

### Comparing `robocorp_browser-2.0.1/pyproject.toml` & `robocorp_browser-2.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "2.0.1"
+version = "2.1.0"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
```

### Comparing `robocorp_browser-2.0.1/src/robocorp/browser/__init__.py` & `robocorp_browser-2.1.0/src/robocorp/browser/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,67 +7,111 @@
     Locator,
     Page,
     Playwright,
 )
 
 from ._browser_engines import BrowserEngine
 
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
 
     Calling this method is optional (if not called a default configuration will
     be used -- note that calling this method after the browser is already
     initialized will have no effect).
 
     Args:
         browser_engine:
-            help="Browser engine which should be used",
-            choices=[chromium", "chrome", "chrome-beta", "msedge", "msedge-beta", "msedge-dev", "firefox", "webkit"]
+            Browser engine which should be used
+            default="chromium"
+            choices=["chromium", "chrome", "chrome-beta", "msedge",
+                     "msedge-beta", "msedge-dev", "firefox", "webkit"]
 
         headless: If set to False the browser UI will be shown. If set to True
             the browser UI will be kept hidden. If unset or set to None it'll
             show the browser UI only if a debugger is detected.
 
         slowmo:
             Run interactions in slow motion.
 
         screenshot:
-            default="only-on-failure",
-            choices=["on", "off", "only-on-failure"],
-            help="Whether to automatically capture a screenshot after each task.",
+            Whether to automatically capture a screenshot after each task.
+            default="only-on-failure"
+            choices=["on", "off", "only-on-failure"]
+
+        viewport_size:
+            Size to be set for the viewport. Specified as tuple(width, height).
+
+    Note:
+        See also: `robocorp.browser.configure_context` to change other
+        arguments related to the browser context creation.
     """  # noqa
     from ._browser_context import _browser_config
 
     config = _browser_config()
 
     for key, value in kwargs.items():
+        if key == "viewport_size":
+            width, height = value
+            configure_context(viewport={"width": width, "height": height})
+            continue
+
         if not hasattr(config, key):
             raise ValueError(f"Invalid configuration: {key}.")
         setattr(config, key, value)
 
 
+def configure_context(**kwargs) -> None:
+    """
+    While the most common configurations may be configured through `configure`,
+    not all arguments passed to `playwright.Browser.new_context` are covered.
+
+    For cases where different context keyword arguments are needed it's possible
+    to use this method to customize the keyword arguments passed to
+    `playwright.Browser.new_context`.
+
+    Example:
+        ```python
+        from robocorp import browser
+        browser.configure_context(ignore_https_errors = True)
+        ```
+
+    Note:
+        The changes done persist through the full session, so, new tasks which
+        create a browser context will also get the configuration changes.
+        If the change should not be used across tasks it's possible
+        to call `robocorp.browser.context(...)` with the required arguments
+        directly.
+    """
+    from . import _browser_context
+
+    browser_context_kwargs = _browser_context.browser_context_kwargs()
+    browser_context_kwargs.update(kwargs)
+
+
 def page() -> Page:
     """
     Provides a managed instance of the browser page to interact with.
 
     Returns:
         The browser page to interact with.
 
         Note that after a page is created, the same page is returned until the
         current task finishes or the page is closed.
 
         If a new page is required without closing the current page use:
 
+        ```python
         from robocorp import browser
         page = browser.context.new_page()
+        ```
     """
     from . import _browser_context
 
     return _browser_context.page()
 
 
 def browser() -> Browser:
@@ -108,33 +152,38 @@
         automatically closed when the task run session finishes.
     """
     from . import _browser_context
 
     return _browser_context.playwright()
 
 
-def context() -> BrowserContext:
+def context(**kwargs) -> BrowserContext:
     """
     Provides a managed instance of the browser context to interact with.
 
     Returns:
         The browser context instance to interact with.
 
         If no browser context instance is created yet one is created and the
         same one is returned on new invocations.
 
-        To customize it use the `configure` method (prior
-        to calling this method).
-
         Note that the returned instance must not be closed. It will be
         automatically closed when the task run session finishes.
+
+    Note:
+        If the context is not created it's possible to customize the context
+        arguments through the kwargs provided, by using the `configure(...)`
+        method or by editing the `configure_context(...)` returned dict.
+
+        If the context was already previously created the **kwargs passed will
+        be ignored.
     """
     from . import _browser_context
 
-    return _browser_context.context()
+    return _browser_context.context(**kwargs)
 
 
 def goto(url: str) -> Page:
     """
     Changes the url of the current page (creating a page if needed).
 
     Args:
```

### Comparing `robocorp_browser-2.0.1/src/robocorp/browser/_browser_context.py` & `robocorp_browser-2.1.0/src/robocorp/browser/_browser_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,31 +38,33 @@
         headless: Optional[bool] = None,
         slowmo: int = 0,
         screenshot: str = "only-on-failure",
     ):
         """
         Args:
             browser_engine:
-                help="Browser engine which should be used",
-                choices=[chromium", "chrome", "chrome-beta", "msedge", "msedge-beta", "msedge-dev", "firefox", "webkit"]
+                Browser engine which should be used
+                default="chromium"
+                choices=["chromium", "chrome", "chrome-beta", "msedge",
+                         "msedge-beta", "msedge-dev", "firefox", "webkit"]
 
             install:
                 Install browser or not. If not defined, download is only
                 attempted if the browser fails to launch.
 
             headless:
                 Run headless or not.
 
             slowmo:
                 Run interactions in slow motion (number in millis).
 
             screenshot:
-                default="only-on-failure",
-                choices=["on", "off", "only-on-failure"],
-                help="Whether to automatically capture a screenshot after each task.",
+                Whether to automatically capture a screenshot after each task.
+                default="only-on-failure"
+                choices=["on", "off", "only-on-failure"]
         """  # noqa
         self.browser_engine = browser_engine
         self.install = install
         self.headless = headless
         self.slowmo = slowmo
         self.screenshot = screenshot
 
@@ -214,20 +216,36 @@
         else:
             raise
 
     yield browser
     browser.close()
 
 
+@session_cache
+def browser_context_kwargs() -> dict:
+    """
+    The returned dict may be edited to change the arguments passed to
+    `playwright.Browser.new_context`.
+
+    Note:
+        This is a (robocorp.tasks) session cache, so, the same dict will be
+        returned over and over again.
+    """
+    return {}
+
+
 @task_cache
-def context(**browser_context_kwargs) -> Iterator[BrowserContext]:
+def context(**kwargs) -> Iterator[BrowserContext]:
     from robocorp.tasks import get_current_task
 
     pages: List[Page] = []
-    ctx = browser().new_context(**browser_context_kwargs)
+    all_kwargs: dict = {}
+    all_kwargs.update(**browser_context_kwargs())
+    all_kwargs.update(**kwargs)
+    ctx = browser().new_context(**all_kwargs)
     ctx.on("page", lambda page: pages.append(page))
 
     yield ctx
 
     task = get_current_task()
     failed = False
     if task is not None:
```

### Comparing `robocorp_browser-2.0.1/src/robocorp/browser/_browser_engines.py` & `robocorp_browser-2.1.0/src/robocorp/browser/_browser_engines.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-2.0.1/src/robocorp/browser/cli.py` & `robocorp_browser-2.1.0/src/robocorp/browser/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-2.0.1/PKG-INFO` & `robocorp_browser-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 2.0.1
+Version: 2.1.0
 Summary: Robocorp browser automation library
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,26 +13,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: playwright (>=1.32.1,<2.0.0)
 Requires-Dist: robocorp-tasks (>=1,<3)
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
-# Robocorp browser library
+# robocorp-browser
 
-The `robocorp-browser` library helps in automating browsers by providing 
-convenient APIs to manage the lifecycle of playwright objects using `robocorp-tasks`.
-
-
-The code below reflects the basic usage of the library:
+The `robocorp-browser` is a wrapper for the [Playwright](https://playwright.dev/python/)
+project, with quality-of-life improvements such as automatic lifecycle management
+for Playwright objects.
 
+## Getting started
 
 ```python
-from robocorp import browser
 from robocorp.tasks import task
+from robocorp import browser
 from robocorp import vault
 
 
 @task
 def browser_automate():
     # Configure may be used to set the basic robocorp.browser settings.
     # It must be called prior to calling APIs which create playwright objects.
@@ -41,33 +40,45 @@
         # If the browser_automate() function finishes with an exception it will
         # make a screenshot and embed it into the logs.
         screenshot="only-on-failure",
         
         # By default headless is False unless running in a Linux container
         # without a DISPLAY/WAYLAND_DISPLAY environment variable, but it
         # can also be manually specified.
-        # headless=True|False,
+        headless=True,
         
         # Interactions may be run in slow-motion (given in milliseconds).
-        # slowmo=100,
+        slowmo=100,
     )
 
     # browser.goto() may be used as a shortcut to get the current page and
     # go to some url (it may create the browser if still not created).
-    browser.goto("https://<target-page.com>")
+    browser.goto("https://example.com>")
 
     login()
 
 
 def login():
     # APIs in robocorp.browser return the same browser instance, which is
     # automatically closed when the task finishes.
     page = browser.page()
 
     # robocorp.vault is recommended for managing secrets.
-    password = vault.get_secret("default-account")["password"]
+    account = vault.get_secret("default-account")
 
     # Use the playwright Browser api as usual.
-    page.fill('//input[@ng-reflect-name="password"]', password)
+    page.fill('//input[@ng-reflect-name="password"]', account["password"])
     page.click("input:text('Submit')")
 ```
 
+## Guides
+
+- [Browser configuration](https://github.com/robocorp/robo/blob/master/browser/docs/guides/configuration.md)
+
+## API Reference
+
+Information on specific functions or classes: [robocorp.browser](https://github.com/robocorp/robo/blob/master/browser/docs/api/robocorp.browser.md)
+
+## Changelog
+
+A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robo/blob/master/browser/docs/CHANGELOG.md).
+
```

