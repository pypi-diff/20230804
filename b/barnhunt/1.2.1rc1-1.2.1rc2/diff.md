# Comparing `tmp/barnhunt-1.2.1rc1.tar.gz` & `tmp/barnhunt-1.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barnhunt-1.2.1rc1.tar", last modified: Tue May 23 03:12:11 2023, max compression
+gzip compressed data, was "barnhunt-1.2.1rc2.tar", last modified: Tue Jun  6 17:49:44 2023, max compression
```

## Comparing `barnhunt-1.2.1rc1.tar` & `barnhunt-1.2.1rc2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    15578 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/CHANGES.md
--rw-r--r--   0        0        0    32528 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/LICENSE
--rw-r--r--   0        0        0     4615 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/README.md
--rw-r--r--   0        0        0       61 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/__init__.py
--rw-r--r--   0        0        0      269 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/__main__.py
--rw-r--r--   0        0        0      585 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/_compat.py
--rw-r--r--   0        0        0       22 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/_version.py
--rw-r--r--   0        0        0    18454 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/cli.py
--rw-r--r--   0        0        0     8946 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/coursemaps.py
--rw-r--r--   0        0        0        0 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/__init__.py
--rw-r--r--   0        0        0     3022 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/css.py
--rw-r--r--   0        0        0    12227 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/runner.py
--rw-r--r--   0        0        0    11100 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/svg.py
--rw-r--r--   0        0        0     3699 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/utils.py
--rw-r--r--   0        0        0     8378 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/installer/__init__.py
--rw-r--r--   0        0        0     2101 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/installer/github.py
--rw-r--r--   0        0        0     4612 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/installer/metadata.py
--rw-r--r--   0        0        0     4717 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/layerinfo.py
--rw-r--r--   0        0        0     4252 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/pager.py
--rw-r--r--   0        0        0     3843 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/pdfutil.py
--rw-r--r--   0        0        0     7769 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/templating.py
--rw-r--r--   0        0        0     3882 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/pdm_build.py
--rw-r--r--   0        0        0     9885 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/pyoxidizer/pyoxidizer.bzl
--rw-r--r--   0        0        0    24251 2023-05-23 03:12:11.768145 barnhunt-1.2.1rc1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/__init__.pyi
--rw-r--r--   0        0        0      205 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/exceptions.pyi
--rw-r--r--   0        0        0     1774 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/popen_spawn.pyi
--rw-r--r--   0        0        0     5501 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/spawnbase.pyi
--rw-r--r--   0        0        0     1053 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/conftest.py
--rw-r--r--   0        0        0     4089 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/drawing.svg
--rw-r--r--   0        0        0      558 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/dummy_inkscape.py
--rw-r--r--   0        0        0     2221 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_css.py
--rw-r--r--   0        0        0     8129 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_runner.py
--rw-r--r--   0        0        0     1899 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_shell_mode_integration.py
--rw-r--r--   0        0        0    10830 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_svg.py
--rw-r--r--   0        0        0     5702 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_utils.py
--rw-r--r--   0        0        0      887 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/ratelimit.py
--rw-r--r--   0        0        0      627 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/test_github.py
--rw-r--r--   0        0        0    11880 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/test_installer.py
--rw-r--r--   0        0        0     3457 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/test_metadata.py
--rw-r--r--   0        0        0     4052 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test1.pdf
--rw-r--r--   0        0        0     4098 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test2.pdf
--rw-r--r--   0        0        0     6695 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_cli.py
--rw-r--r--   0        0        0     8719 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_coursemaps.py
--rw-r--r--   0        0        0     3366 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_functional.py
--rw-r--r--   0        0        0     5833 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_layerinfo.py
--rw-r--r--   0        0        0      350 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_main.py
--rw-r--r--   0        0        0     3616 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_pager.py
--rw-r--r--   0        0        0     3998 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_pdfutil.py
--rw-r--r--   0        0        0     9120 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_templating.py
--rw-r--r--   0        0        0     2780 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/testlib.py
--rw-r--r--   0        0        0     1544 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tox.ini
--rw-r--r--   0        0        0    21367 1970-01-01 00:00:00.000000 barnhunt-1.2.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    15894 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/CHANGES.md
+-rw-r--r--   0        0        0    32528 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/LICENSE
+-rw-r--r--   0        0        0     4615 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/README.md
+-rw-r--r--   0        0        0       61 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/__main__.py
+-rw-r--r--   0        0        0      585 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/_compat.py
+-rw-r--r--   0        0        0       22 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/_version.py
+-rw-r--r--   0        0        0    18454 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/cli.py
+-rw-r--r--   0        0        0     8946 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/coursemaps.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/inkscape/__init__.py
+-rw-r--r--   0        0        0     3022 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/inkscape/css.py
+-rw-r--r--   0        0        0    12275 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/inkscape/runner.py
+-rw-r--r--   0        0        0    11100 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/inkscape/svg.py
+-rw-r--r--   0        0        0     3699 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/inkscape/utils.py
+-rw-r--r--   0        0        0     8378 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/installer/__init__.py
+-rw-r--r--   0        0        0     2101 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/installer/github.py
+-rw-r--r--   0        0        0     4612 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/installer/metadata.py
+-rw-r--r--   0        0        0     4717 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/layerinfo.py
+-rw-r--r--   0        0        0     4252 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/pager.py
+-rw-r--r--   0        0        0     3843 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/pdfutil.py
+-rw-r--r--   0        0        0    14020 2023-06-06 17:49:30.752495 barnhunt-1.2.1rc2/barnhunt/templating.py
+-rw-r--r--   0        0        0     3882 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/pdm_build.py
+-rw-r--r--   0        0        0     9885 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/pyoxidizer/pyoxidizer.bzl
+-rw-r--r--   0        0        0    24599 2023-06-06 17:49:44.236666 barnhunt-1.2.1rc2/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/stubs/pexpect/__init__.pyi
+-rw-r--r--   0        0        0      205 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/stubs/pexpect/exceptions.pyi
+-rw-r--r--   0        0        0     1774 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/stubs/pexpect/popen_spawn.pyi
+-rw-r--r--   0        0        0     5501 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/stubs/pexpect/spawnbase.pyi
+-rw-r--r--   0        0        0     1053 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/conftest.py
+-rw-r--r--   0        0        0     5673 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/drawing.svg
+-rw-r--r--   0        0        0      558 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/inkscape/dummy_inkscape.py
+-rw-r--r--   0        0        0     2221 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/inkscape/test_css.py
+-rw-r--r--   0        0        0     8129 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/inkscape/test_runner.py
+-rw-r--r--   0        0        0     1899 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/inkscape/test_shell_mode_integration.py
+-rw-r--r--   0        0        0    10830 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/inkscape/test_svg.py
+-rw-r--r--   0        0        0     5702 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/inkscape/test_utils.py
+-rw-r--r--   0        0        0      887 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/installer/ratelimit.py
+-rw-r--r--   0        0        0      627 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/installer/test_github.py
+-rw-r--r--   0        0        0    11880 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/installer/test_installer.py
+-rw-r--r--   0        0        0     3457 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/installer/test_metadata.py
+-rw-r--r--   0        0        0     4052 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test1.pdf
+-rw-r--r--   0        0        0     4098 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test2.pdf
+-rw-r--r--   0        0        0     6695 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_cli.py
+-rw-r--r--   0        0        0     8719 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_coursemaps.py
+-rw-r--r--   0        0        0     3366 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_functional.py
+-rw-r--r--   0        0        0     5833 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_layerinfo.py
+-rw-r--r--   0        0        0      350 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_main.py
+-rw-r--r--   0        0        0     3616 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_pager.py
+-rw-r--r--   0        0        0     3998 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_pdfutil.py
+-rw-r--r--   0        0        0    14215 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/test_templating.py
+-rw-r--r--   0        0        0     2780 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tests/testlib.py
+-rw-r--r--   0        0        0     1427 2023-06-06 17:49:30.756495 barnhunt-1.2.1rc2/tox.ini
+-rw-r--r--   0        0        0    21710 1970-01-01 00:00:00.000000 barnhunt-1.2.1rc2/PKG-INFO
```

### Comparing `barnhunt-1.2.1rc1/CHANGES.md` & `barnhunt-1.2.1rc2/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 ## Changes
 
+### Release 1.2.1rc2 (2023-06-06)
+
+#### New Features
+
+- Provide access to RDF metadata in the SVG source in string
+  templates.  E.g. the document description may be interpolated via
+  `{{ rdf['dc:description'] }}`.
+
+#### Bugs Fixed
+
+- Fix parsing of version strings reported by pre-release versions of
+  Inkscape.
+
 ### Release 1.2.1rc1 (2023-05-22)
 
 (There was no final release of 1.2.0. It is a long story. I mistakenly
 committed a couple of files to LFS. To clear out LFS storage for a
 GitHub repo, one has to [delete the whole repo](😬). As a result, the
 workflow `$GITHUB_RUN_NUMBER` has reset. Thus a micro-version bump
 is required to keep those PyOxidizer windows build version numbers —
```

### Comparing `barnhunt-1.2.1rc1/LICENSE` & `barnhunt-1.2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/README.md` & `barnhunt-1.2.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/_compat.py` & `barnhunt-1.2.1rc2/barnhunt/_compat.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/cli.py` & `barnhunt-1.2.1rc2/barnhunt/cli.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/coursemaps.py` & `barnhunt-1.2.1rc2/barnhunt/coursemaps.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/inkscape/css.py` & `barnhunt-1.2.1rc2/barnhunt/inkscape/css.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/inkscape/runner.py` & `barnhunt-1.2.1rc2/barnhunt/inkscape/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,13 +373,15 @@
     runner: type[Runner] = ShellModeRunner if shell_mode else CliRunner
     return runner(api, executable)
 
 
 def dwim_old_inkscape(executable: str) -> bool:
     """Determine whether we're running an old Inkscape."""
     proc = run([executable, "--version"], capture_output=True, text=True, check=True)
-    m = re.search(r"(?m)^Inkscape (\d+)\.(\d+)\.(\d+) ", proc.stdout)
+    m = re.search(
+        r"(?m)^Inkscape (\d+)\.(\d+)(?:\.(\d+))?(?:-(dev|alpha|beta))? ", proc.stdout
+    )
     if m is None:
         log.warning("Can not determine Inkscape version.")
         return False
-    version = tuple(map(int, m.groups()))
+    version = tuple(map(int, m.groups("0")[:3]))
     return version < (1, 0)
```

### Comparing `barnhunt-1.2.1rc1/barnhunt/inkscape/svg.py` & `barnhunt-1.2.1rc2/barnhunt/inkscape/svg.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/inkscape/utils.py` & `barnhunt-1.2.1rc2/barnhunt/inkscape/utils.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/installer/__init__.py` & `barnhunt-1.2.1rc2/barnhunt/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/installer/github.py` & `barnhunt-1.2.1rc2/barnhunt/installer/github.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/installer/metadata.py` & `barnhunt-1.2.1rc2/barnhunt/installer/metadata.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/layerinfo.py` & `barnhunt-1.2.1rc2/barnhunt/layerinfo.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/pager.py` & `barnhunt-1.2.1rc2/barnhunt/pager.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/barnhunt/pdfutil.py` & `barnhunt-1.2.1rc2/barnhunt/pdfutil.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/pdm_build.py` & `barnhunt-1.2.1rc2/pdm_build.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/pyoxidizer/pyoxidizer.bzl` & `barnhunt-1.2.1rc2/pyoxidizer/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/pyproject.toml` & `barnhunt-1.2.1rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,31 +35,32 @@
     "jinja2~=3.1",
     "lxml~=4.9",
     "marshmallow~=3.19",
     "marshmallow-dataclass~=8.5.13",
     "packaging~=23.1",
     "pexpect~=4.8",
     "pikepdf~=6.2",
+    "rdflib~=6.3",
     "requests~=2.29",
     "tinycss2~=1.2",
     "typing-extensions~=4.5; python_version < \"3.10\"",
 ]
-version = "1.2.1rc1"
+version = "1.2.1rc2"
 
 [project.license]
 text = "GPL-3.0-only"
 
 [project.urls]
 Homepage = "https://github.com/barnhunt/barnhunt"
 
 [project.entry-points.console_scripts]
 barnhunt = "barnhunt.cli:main"
 
 [project.readme]
-text = "# Barn Hunt Map Helper\n\n[![Test status badge](https://img.shields.io/github/actions/workflow/status/barnhunt/barnhunt/ci.yml?label=tests)](https://github.com/barnhunt/barnhunt/actions/workflows/ci.yml)\n[![Latest version badge](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Supported Python versions badge](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Supported Inkscape versions badge](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2.2-blue.svg?logo=inkscape)](https://inkscape.org/)\n[![Development status badge](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Trackgit-views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhapwefdbvler7yp5dsl)](https://trackgit.com)\n\nThis is a helper script Jeff uses for drafting [Barn Hunt][] course\nmaps.\n\nIt does a bunch of stuff, but the important bit is that it exports PDF\nversions of maps from [Inkscape][] SVG files.\n\nI draw all the maps for a given ring (for a day or weekend) in a\nsingle Inkscape drawing.  Various maps (for different trials/classes,\nbuild map, rat-maps, base maps, etc.) are generated by hiding and\nunhiding appropriate layers in the drawing and exporting to PDF.\n\nThis program automates that process.\n\n## Requirements\n\nThis program requires Python, version 3.7 or higher to run.\n\nIt \"should\" work with all versions of Inkscape, 0.9x through 1.2.1.\n\nI use this program on Linux, however the package now includes a GitHub\nCI workflow that performs rudimentary testing on Windows and macOS, so\nthere’s a moderate chance it might \"just work\" on those platforms.\n(Due to a dependency on the [pikepdf][] package, it should work on\nx86_64-based Macs, but may not work on Macs that use Apple silicon. If\npikepdf compatibility is an issue for you, let me know — it’s probably\nfixable.)\n\n## Installation\n\n### Windows\n\nWe now publish a compiled version of the program for Windows (which may\neven work.) Using this version has the advantage that Python is not required\nto be installed. (And even if Python is installed, this version may work-around\nsome bugs having to do with the various different ways that Python can be\ninstalled on on Windows computer.)\n\n1. Browse to our [releases](https://github.com/barnhunt/barnhunt/releases/)\n   page. Select a release, and look down in the *Assets* section of the\n   release page. (You may have to click the triangle to expand the\n   *Assets* section.)\n\n2. Download the MSI installer (the filename should end with `.msi` —\n   e.g. `Barnhunt-1.2.0.49-x86_64-pc-windows-msvc.msi`). The file\n   is not signed, so you may have to click through some nasty warnings\n   about \"unrecognized, potentially dangerous\" files.\n\n3. Once downloaded, open (double-click) the file you just\n   downloaded. Hopefully and installer dialog should open.  Accept the\n   default choices.\n\n4. Now open a terminal command-line window. Type `barnhunt\n   --version`. If all is good, barnhunt should report its version. Run\n   `barnhunt --help` for the help screen.\n\n\n### Linux (or Windows with Python installed)\n\nAs this package is published to\n[PyPI](https://pypi.org/project/barnhunt/) it may be installed into a\n[_virtualenv_][venv] using [`pip`][pip]. It is suggested that you use\n[`pipx`][pipx] to combine those two steps.\n\nA basic outline of how to proceed:\n\n1. Install [python][] if it is not already installed.  (Version 3.7 or\n   greater is required.)\n\n2. Install [pipx][].  This might look like:\n\n   ```sh\n   python3 -m pip install --user pipx\n   python3 -m pipx ensurepath\n   ```\n\n3. Install `barnhunt`.\n\n   ```sh\n   pipx install barnhunt\n   ```\n\n## How to Use\n\nSadly, this program is currently quite under-documented.\n\nThe functions of the basic sub-commands and command-line options are\ntersely documented via the `--help` option.  Try:\n\n```sh\nbarnhunt --help\n```\n\nand\n\n```sh\nbarnhunt pdfs --help\n```\n\nfor starters.\n\nIf you get stuck, kick me!\n\n## Author\n\nThis package was written by Jeff Dairiki, BHAJ-221A, <dairiki@dairiki.org>.\n\n----\n\n[Inkscape]: https://inkscape.org/ (The Inkscape home page)\n[Barn Hunt]: https://www.barnhunt.com/ (Barn Hunt — a fabulous sport for dogs)\n[python]: https://www.python.org/ (The Python home page)\n[venv]: https://docs.python.org/3/library/venv.html\n(Python venv module documentation)\n[pipx]: https://pypa.github.io/pipx/ (The pipx home page)\n[pip]: https://pip.pypa.io/en/stable/ (Documentation for pip)\n[pikepdf]: https://pikepdf.readthedocs.io/en/latest/installation.html\n(The Installation section of the pikepdf documentation)\n\n## Changes\n\n### Release 1.2.1rc1 (2023-05-22)\n\n(There was no final release of 1.2.0. It is a long story. I mistakenly\ncommitted a couple of files to LFS. To clear out LFS storage for a\nGitHub repo, one has to [delete the whole repo](😬). As a result, the\nworkflow `$GITHUB_RUN_NUMBER` has reset. Thus a micro-version bump\nis required to keep those PyOxidizer windows build version numbers —\n`<major>.<minor>.<micro>.<run-number>` — monotonic.)\n\n[delete the whole repo]: https://docs.github.com/en/repositories/working-with-files/managing-large-files/removing-files-from-git-large-file-storage#git-lfs-objects-in-your-repository\n\n#### CLI Changes\n\n- The `--inkscape-command`, `--processes` and `--shell-mode-inkscape`\n  options have been moved from the `barnhunt pdfs` subcommand to the\n  man `barnhunt` command group.\n\n- And new `debug-info` subcommand has been added to display various\n  information about the installed version of the `barnhunt` command\n  and its execution environment.\n\n- The `--dump-loaded-modules` option has been removed.  The\n  functionality is still available by setting the\n  `$BARNHUNT_DUMP_LOADED_MODULES` environment variable to a non-empty\n  value.\n\n#### Bugs Fixed\n\n- Fixed exception in `barnhunt.cli.default_2up_output_file` during\n  shell-completion for `barnhunt 2up`.\n\n### Release 1.2.0rc6 (2023-04-27)\n\n- Build an Windows executable and installer using [PyOxidizer].  The\n  .msi installer should be downloadable from the\n  [Releases](https://github.com/barnhunt/barnhunt/releases) page.\n\n- Added a `--dump-loaded-modules` option which causes `barnhunt` to\n  write a list of all loaded modules the current working directory.\n  (This is a development tool, not generally useful to most users.)\n\n- Hardwire the distribution version into `barnhunt.__version__` rather\n  than deducing it via `importlib.metadata`.  This allows us to monkey\n  with the version we report from the PyOxidizer-built Windows\n  executable so that it indicates the MSI build version as well as\n  the distribution version.\n\n- Convert package from setuptools to PDM.\n\n[PyOxidizer]: https://pyoxidizer.readthedocs.io/en/stable/pyoxidizer.html\n\n### Release 1.2.0rc5 (2023-03-05)\n\n#### Bugs Fixed\n\n- When there was a visible “clone” (`<svg:use>` element) that\n  referenced a source on a hidden layer were being pruned from the SVG\n  before conversion to PDF.  (When exporting an SVG, hidden layers are\n  omitted from the SVG — this speeds Inkscape up considerably when\n  there is a large amount of hidden content.) Now we detect hidden\n  layers that contain source material for clones, and retain them in\n  the SVG file.\n\n- Add a cruft pattern to ignore “`Gtk-WARNING\"`” messages that have\n  started appearing since I installed Inkscape from [Inkscape’s ppa][ppa].\n\n- Fix tests to workaround segfault from pikepdf 7.0.0, 7.1.0, and 7.1.1.\n  (See [pikepdf/pikepdf#452].)\n\n[ppa]: https://inkscape.org/release/inkscape-1.2.2/gnulinux/ubuntu/ppa/dl/\n[pikepdf/pikepdf#452]: https://github.com/pikepdf/pikepdf/issues/452).\n\n### Release 1.2.0rc4 (2023-01-09)\n\nSupport python 3.11.\n\n#### Bugs\n\n- Shell-mode runner: fix readline/pexpect disagreement with respect to\n  horizontal scrolling of long lines.  In some cases, when Inkscape is\n  compiled to use GNU readline, long input lines will be scrolled\n  horizontally (even when stdin is not a tty). This messes with\n  pexpect's head. We've now added some basic tests for this, and set\n  some environment variables to try to convince readline not to do the\n  scrolling.\n\n#### Testing\n\n- Test under python 3.11\n- Fix tests for Windows environments where $APPDATA is not set\n- Fix tests for error message changes in packaging>=22\n\n### Release 1.2.0rc3 (2022-10-19)\n\n#### Extension/Symbols Installer\n\n- Make code for deducing Inkscape profile directory more robust.\n  (There's now a beter chance this will actually work on Windows.)\n- Support setting Inkscape profile directory via `$INKSCAPE_PROFILE_DIR`.\n\n### Release 1.2.0rc2 (2022-10-17)\n\n### Extension and Symbol Set Installation\n\n- This release add a `barnhunt install` (and `uninstall`) sub-command\n  to simplify installation of the\n  [inkex-bh](https://github.com/barnhunt/inkex-bh) Inkscape extensions\n  and [bh-symbols](https://github.com/barnhunt/bh-symbols) symbol\n  sets.\n\n#### Testing\n\n- Update to `mypy==0.982` for testing. Fix spurious mypy errors.\n\n### Release 1.2.0rc1 (2022-08-31)\n\nFirst public release to PyPI. Moved project to\n[GitHub](https://github.com/barnhunt/barnhunt).\n\n- Dropped support for python 3.6\n- Changed license to GPL version 3\n- We now do rudimentary testing under Windows and macOS.\n\n#### Dependencies\n\n- Use [pikepdf](https://pypi.org/project/pikepdf/) instead of\n  [pdfrw](https://pypi.org/project/pdfrw/) to manipulate PDFs.  (Pdfrw\n  seems not to be very actively maintained.) The only possible\n  downside of this is that `pikepdf` is not pure-python. It claims to\n  be easily installable on Windows and _x86_64_ Macs, but is not\n  (easily) installable on Macs with Apple silicon.\n\n- Generated PDFs are now [linearized][qpdf-linearize] and\n  [compressed][qpdf-object-streams].\n\n- Add test dependency on\n  [pdfminer.six](https://pypi.org/project/pdfminer.six/) (but drop\n  dependency on [PyPDF2](https://pypi.org/project/PyPDF2/)).\n\n\n#### Compatibility\n\n- Refactor `barnhunt.inkscape.runner` to support running\n  Inkscape >= 1.0 (as well as continuing to support Inkscape 0.9x).\n\n- Add `--inkscape-command` parameter to the `barnhunt pdfs` command\n  to specify the name/path of the Inkscape binary to run to export PDFs.\n  This also supports setting the Inkscape executable via the `$INKSCAPE_COMMAND`\n  environment variable.  Default executable is not `inkscape.exe` on Windows\n  (and `inkscape` everywhere else).\n\n- Use `pexpect.popen_spawn.PopenSpawn` instead of `pexpect.spawn` to\n  run Inkscape in shell-mode. Due to `pexpect.spawn`'s use of ptys, it\n  [will not work][pexpect-windows] on Windows.\n\n- **MacOS**: our code for running Inkscape in shell-mode appears to be broken.\n  For now, on _macOS_ we default to not using shell-mode.\n\n#### Packaging\n\n- Added a stub `barnhunt.__main__` module to allow running via `python\n  -m barnhunt`.\n\n#### Testing\n\n- Add type annotations.\n\n#### Bit Rot\n\n- Fix up tests to address deprecations in PyPDF2.\n\n[qpdf-linearize]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=linearize#option-linearize\n[qpdf-object-streams]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=object-streams#option-object-streams\n[pexpect-windows]: https://pexpect.readthedocs.io/en/stable/overview.html#windows\n\n### Release 1.1.0a1 (2022-03-08)\n\n#### \"Base Map\" support\n\nAdd ability to mark layers for exclusion from particular output files.\n\nThis adds the ability to list multiple comma-separated output base\nfilenames for a given overlay.\nE.g. A layer with label `\"[o|build_notes,base] Build Notes\"`\nwill define an overlay which will generate maps in two separate\noutput files.\n\nTagging a layer with `[!`_output-basename_`]` will exclude that\nlayer from any maps which are directed to the specified output\nfilename.\n\nTagging a layer with `[=`_output-basename_`]` will include that layer\nfrom any maps which are directed to the specified output filename, while\nexcluding all other sibling layers not explicitly tagged to be included\nin that output file.\n\n\n### Release 1.0.1 (2021-11-10)\n\n#### Diagnostics\n\n`Barnhunt pdfs` now issues a warning when generating PDFs from an SVG\nfile which does not have an explicit random-seed set.\n\n#### Bugs Fixed\n\nOpen SVG files in binary mode in order to let the XML parser figure\nout the encoding from the XML declaration.\n\n### Release 1.0 (2021-11-10)\n\nSupport python 3.10.\n\n#### Random Seed\n\nThe way the random seed (used for generating random rat numbers) for\neach SVG layer is computed has been changed in a\n**backward-incompatible** way.  This was done so that rat numbers can\nbe kept from changing when an SVG source file is copied or edited in\nsuch a way that the device and/or inode of the file changes.\n\nNow, the file-level random seed (an integer) is read from the\n`bh:random-seed` attribute of the root `svg` element of the SVG\nfile. If no `bh:random-seed` attribute is set, the file-level seed is\ncomputed by hashing the device and inode numbers of the SVG file.\n\nThe layer-level seed is formed by hashing the file-level random seed\nwith the XML *id* of the layer.\n\n(Formerly, the layer-level seed was form by hashing a triple of the\nfile-level seed (which was always zero), the hash of the SVG files\ndevice and inode, and the id of the layer.)\n\nA new `barnhunt random-seed` sub-command has been implemented to help\nwith setting the random seed for SVG source files.\n\n#### Bit-rot\n\nAddress `DeprecationWarning: 'contextfunction' is renamed to\n'pass_context'` from Jinja2. Require `Jinja2>3`.\n\n#### OCDisms\n\nRun `pyupgrade --py36-plus` on source.\n\n\n### Release 0.5 (2021-05-04)\n\nMake `-o` option to `2up` sub-command optional.\n\nRemove support for python < 3.6.\n\n### Release 0.4 (2019-02-25)\n\n#### New Sub-Command: 2up\n\nNew `2up` sub-command to format PDFs for 2-up printing.  Pages are\npre-shuffled so that the 2-up pages do not need to be shuffled after\ncutting.\n\n\n### Release 0.3 (2019-02-20)\n\n#### `barnhunt pdfs`\n\n- Multi-page output support.\n\n  There is a new syntax to specify the output file basename for an overlay.\n  Multiple overlays which specify the same output file will all be saved to\n  the same file.\n\n- It is now possible to render course maps from multiple SVG files in a\n  single invocation.  (Just list all the files to be rendered on the\n  command line.)\n\n#### Tests\n\n- `test_layerinfo.test_layerflags_str`: Fix test to deal with\n  arbitrary ordering of `enum.Flag` flags.\n\n### Release 0.2 (2018-11-07)\n\n#### Templating\n\n- Do not expand text within hidden layers.  This avoids generating\n  error messages (e.g. \"'overlay' is undefined\") due to template\n  expansion of unused text.\n\n- Add optional `skip` argument to the `random_rats` function.\n  This allows the generation of more than one set of stable random rat\n  numbers per layer.  E.g. `random_rats(skip=5)` will generate a set\n  of random number totally uncorrelated to that generated by\n  `random_rats()`.  Using `skip` has the advantage over using\n  `seed=None` that the results are stable and do not vary from\n  render to render.\n\n### Release 0.1 (2018-11-07)\n\n- Python 3.7 is now supported.\n\n- The template for the output filename has been generalized to work\n  sensibly in the case where overlays are nested more than two deep.\n\n#### Templating\n\n- Added new attributes to layers:\n\n  `layer.is_overlay`\n      Boolean.  True if layer is an overlay.\n\n  `layer.lineage`\n      Sequence starting with layer and including each parent layer in\n      turn.\n\n  `layer.overlay`\n      Returns the nearest overlay layer.  If the layer is an overlay,\n      `layer.overlay` returns `layer`, otherwise it returns the\n      nearest parent layer which is an overlay.  If the layer is not\n      contained within an overlay, returns `None`.\n\n- Added new values to context when expanding text in SVG:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the text\n      element, in order from outermost to innermost.\n\n  `course`\n      The outermost overlay layer.  (Equivalent to `overlays[0]`.)\n      This value already existed in the context used for filename expansion.\n\n  `overlay`\n      If the element is at least two overlays deep, this is the\n      innermost overlay.  Otherwise it is unset.  This value already\n      existed in the context used for filename expansion.\n\n- Added new values to context when expanding output filenames:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the overlay\n      being expanded.\n\n#### Bugs\n\n- Templating: the `safepath` filter would fail with a `TypeError`\n  if applied to anything but a string.  Now it coerces its argument to\n  text.\n\n- Templating: (New style) layer flags in parent layers were not being\n  removed from the layer labels.  (E.g. `\"{{ layer.parent.label }}\"`\n  was expanding to `\"[o] Some Overlay\"`, when it should expand to\n  `\"Some Overlay\"`.)\n\n- Pexpect==4.4.0 appears to have a subtle brokenness when\n  `searchwindowsize` is set to something other than `None`.  The\n  problem seems to be in [pexpect.expect.py][], and is triggered when\n  multiple chunks of output are read before a match is found.\n\n[pexpect.expect.py]: <https://github.com/pexpect/pexpect/blob/606f368b4a0dc442e2523d439d722a389b6e54c6/pexpect/expect.py#L22>\n\n#### Bit-Rot\n\n- Use `log.warning`, rather than the deprecated `log.warn`.\n\n### Release 0.1a12 (2017-02-09)\n\n- Remove tags from layer.label when expanding templated text in SVG file.\n\n### Release 0.1a11 (2017-02-01)\n\n- Add `--version` command line option\n\n#### Pager for `coords`\n\n- A fancy pager (poor man's `less`) has been added for viewing the\n  output of the `barnhunt coords` sub-command.  If any of `sys.stdin`\n  or `sys.stdout` is not a tty, then the pager will be disabled.\n\n- Since there is now a fancy pager, the default for `--number-of-rows`\n  has been increased to 1000.\n\n### Release 0.1a10 (2017-01-30)\n\n#### Things still to be fixed\n\nThings still to be fixed: I'm pretty sure things are direly broken if\na drawing contains no overlays, and somewhat broken if a drawing\ncontains more than two layers of overlays.  The problems have to do\nwith how the output PDF filenames are determined...\n\n#### New layer flag scheme\n\nNew scheme for marking overlay and hidden layers.  One can now set\nbit-flags on layers by including the flags in square brackets at the\nbeginning of the layer label.  I.e. a label like `\"[o] Master Trial\n1\"` marks the layer as an overlay layer, while `\"[h] Prototypes\"`\nmarks a hidden layer.\n\nIf no layers have any flags, `barnhunt pdfs` will fall back to the\nold name-based heuristics for determining hidden and overlay layers.\n\n\n### Release 0.1a9 (2017-01-03)\n\n* When exporting PDFs, run `inkscape` with `--export-area-page`.\n\n#### Packaging\n\n* Fix MANIFEST.in. Tests were not being included in sdist.\n\n* Add `url` to package metadata.\n\n### Release 0.1a8 (2018-01-03)\n\n* Ignore *ring* layers when identifying *course* layers.  (Now a layer\n  labeled “C8 Ring” will not be treated as a course layer.)\n\n* `pdfs`: default `--output-directory` to `.` (avoiding exception when no\n  explicit output directory is specified.)\n\n### Release 0.1a7 (2017-11-18)\n\n* Change `barnhunt coords` so that it omits duplicate coordinates in its output.\n  Also increase the default for `--number-of-rows` to 50 and\n  add the `--group-size` parameter to separate output into groups.\n\n### Release 0.1a6 (2017-11-15)\n\n* Templating: `LabelAdapter` now stringifies to the layer label, and\n  `FileAdapter` now stringifies to the file name.\n* More refactoring, more tests\n* Run several inkscapes in parallel.  This results in a major speedup.\n\n### Release 0.1a5 (2017-11-13)\n\n* Expand text in SVG file.\n* Add tests.\n* Major code refactor.\n\n### Release 0.1a4 (2017-11-10)\n\n#### PDFS\n\n* Log unexpected output from inkscape.\n\n* Add `--no-shell-mode-inkscape` option to control whether shell-mode inkscape\n  optimization is used.\n\n### Release 0.1a3.post1 (2017-11-10)\n\n#### PDFS\n\n* Reverse order that layers are considered.  (Layers are listed from\n  bottom to top in the SVG file.)\n\n### Release 0.1a3 (2017-11-10)\n\n#### PDFS\n\nReplace spaces and other shell-unfriendly characters with underscores\nin output file names.\n\n### Release 0.1a2 (2017-11-09)\n\nAdd sub-commands for generating random numbers.\n\n### Release 0.1a1 (2017-11-07)\n\nInitial release.\n"
+text = "# Barn Hunt Map Helper\n\n[![Test status badge](https://img.shields.io/github/actions/workflow/status/barnhunt/barnhunt/ci.yml?label=tests)](https://github.com/barnhunt/barnhunt/actions/workflows/ci.yml)\n[![Latest version badge](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Supported Python versions badge](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Supported Inkscape versions badge](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2.2-blue.svg?logo=inkscape)](https://inkscape.org/)\n[![Development status badge](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Trackgit-views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhapwefdbvler7yp5dsl)](https://trackgit.com)\n\nThis is a helper script Jeff uses for drafting [Barn Hunt][] course\nmaps.\n\nIt does a bunch of stuff, but the important bit is that it exports PDF\nversions of maps from [Inkscape][] SVG files.\n\nI draw all the maps for a given ring (for a day or weekend) in a\nsingle Inkscape drawing.  Various maps (for different trials/classes,\nbuild map, rat-maps, base maps, etc.) are generated by hiding and\nunhiding appropriate layers in the drawing and exporting to PDF.\n\nThis program automates that process.\n\n## Requirements\n\nThis program requires Python, version 3.7 or higher to run.\n\nIt \"should\" work with all versions of Inkscape, 0.9x through 1.2.1.\n\nI use this program on Linux, however the package now includes a GitHub\nCI workflow that performs rudimentary testing on Windows and macOS, so\nthere’s a moderate chance it might \"just work\" on those platforms.\n(Due to a dependency on the [pikepdf][] package, it should work on\nx86_64-based Macs, but may not work on Macs that use Apple silicon. If\npikepdf compatibility is an issue for you, let me know — it’s probably\nfixable.)\n\n## Installation\n\n### Windows\n\nWe now publish a compiled version of the program for Windows (which may\neven work.) Using this version has the advantage that Python is not required\nto be installed. (And even if Python is installed, this version may work-around\nsome bugs having to do with the various different ways that Python can be\ninstalled on on Windows computer.)\n\n1. Browse to our [releases](https://github.com/barnhunt/barnhunt/releases/)\n   page. Select a release, and look down in the *Assets* section of the\n   release page. (You may have to click the triangle to expand the\n   *Assets* section.)\n\n2. Download the MSI installer (the filename should end with `.msi` —\n   e.g. `Barnhunt-1.2.0.49-x86_64-pc-windows-msvc.msi`). The file\n   is not signed, so you may have to click through some nasty warnings\n   about \"unrecognized, potentially dangerous\" files.\n\n3. Once downloaded, open (double-click) the file you just\n   downloaded. Hopefully and installer dialog should open.  Accept the\n   default choices.\n\n4. Now open a terminal command-line window. Type `barnhunt\n   --version`. If all is good, barnhunt should report its version. Run\n   `barnhunt --help` for the help screen.\n\n\n### Linux (or Windows with Python installed)\n\nAs this package is published to\n[PyPI](https://pypi.org/project/barnhunt/) it may be installed into a\n[_virtualenv_][venv] using [`pip`][pip]. It is suggested that you use\n[`pipx`][pipx] to combine those two steps.\n\nA basic outline of how to proceed:\n\n1. Install [python][] if it is not already installed.  (Version 3.7 or\n   greater is required.)\n\n2. Install [pipx][].  This might look like:\n\n   ```sh\n   python3 -m pip install --user pipx\n   python3 -m pipx ensurepath\n   ```\n\n3. Install `barnhunt`.\n\n   ```sh\n   pipx install barnhunt\n   ```\n\n## How to Use\n\nSadly, this program is currently quite under-documented.\n\nThe functions of the basic sub-commands and command-line options are\ntersely documented via the `--help` option.  Try:\n\n```sh\nbarnhunt --help\n```\n\nand\n\n```sh\nbarnhunt pdfs --help\n```\n\nfor starters.\n\nIf you get stuck, kick me!\n\n## Author\n\nThis package was written by Jeff Dairiki, BHAJ-221A, <dairiki@dairiki.org>.\n\n----\n\n[Inkscape]: https://inkscape.org/ (The Inkscape home page)\n[Barn Hunt]: https://www.barnhunt.com/ (Barn Hunt — a fabulous sport for dogs)\n[python]: https://www.python.org/ (The Python home page)\n[venv]: https://docs.python.org/3/library/venv.html\n(Python venv module documentation)\n[pipx]: https://pypa.github.io/pipx/ (The pipx home page)\n[pip]: https://pip.pypa.io/en/stable/ (Documentation for pip)\n[pikepdf]: https://pikepdf.readthedocs.io/en/latest/installation.html\n(The Installation section of the pikepdf documentation)\n\n## Changes\n\n### Release 1.2.1rc2 (2023-06-06)\n\n#### New Features\n\n- Provide access to RDF metadata in the SVG source in string\n  templates.  E.g. the document description may be interpolated via\n  `{{ rdf['dc:description'] }}`.\n\n#### Bugs Fixed\n\n- Fix parsing of version strings reported by pre-release versions of\n  Inkscape.\n\n### Release 1.2.1rc1 (2023-05-22)\n\n(There was no final release of 1.2.0. It is a long story. I mistakenly\ncommitted a couple of files to LFS. To clear out LFS storage for a\nGitHub repo, one has to [delete the whole repo](😬). As a result, the\nworkflow `$GITHUB_RUN_NUMBER` has reset. Thus a micro-version bump\nis required to keep those PyOxidizer windows build version numbers —\n`<major>.<minor>.<micro>.<run-number>` — monotonic.)\n\n[delete the whole repo]: https://docs.github.com/en/repositories/working-with-files/managing-large-files/removing-files-from-git-large-file-storage#git-lfs-objects-in-your-repository\n\n#### CLI Changes\n\n- The `--inkscape-command`, `--processes` and `--shell-mode-inkscape`\n  options have been moved from the `barnhunt pdfs` subcommand to the\n  man `barnhunt` command group.\n\n- And new `debug-info` subcommand has been added to display various\n  information about the installed version of the `barnhunt` command\n  and its execution environment.\n\n- The `--dump-loaded-modules` option has been removed.  The\n  functionality is still available by setting the\n  `$BARNHUNT_DUMP_LOADED_MODULES` environment variable to a non-empty\n  value.\n\n#### Bugs Fixed\n\n- Fixed exception in `barnhunt.cli.default_2up_output_file` during\n  shell-completion for `barnhunt 2up`.\n\n### Release 1.2.0rc6 (2023-04-27)\n\n- Build an Windows executable and installer using [PyOxidizer].  The\n  .msi installer should be downloadable from the\n  [Releases](https://github.com/barnhunt/barnhunt/releases) page.\n\n- Added a `--dump-loaded-modules` option which causes `barnhunt` to\n  write a list of all loaded modules the current working directory.\n  (This is a development tool, not generally useful to most users.)\n\n- Hardwire the distribution version into `barnhunt.__version__` rather\n  than deducing it via `importlib.metadata`.  This allows us to monkey\n  with the version we report from the PyOxidizer-built Windows\n  executable so that it indicates the MSI build version as well as\n  the distribution version.\n\n- Convert package from setuptools to PDM.\n\n[PyOxidizer]: https://pyoxidizer.readthedocs.io/en/stable/pyoxidizer.html\n\n### Release 1.2.0rc5 (2023-03-05)\n\n#### Bugs Fixed\n\n- When there was a visible “clone” (`<svg:use>` element) that\n  referenced a source on a hidden layer were being pruned from the SVG\n  before conversion to PDF.  (When exporting an SVG, hidden layers are\n  omitted from the SVG — this speeds Inkscape up considerably when\n  there is a large amount of hidden content.) Now we detect hidden\n  layers that contain source material for clones, and retain them in\n  the SVG file.\n\n- Add a cruft pattern to ignore “`Gtk-WARNING\"`” messages that have\n  started appearing since I installed Inkscape from [Inkscape’s ppa][ppa].\n\n- Fix tests to workaround segfault from pikepdf 7.0.0, 7.1.0, and 7.1.1.\n  (See [pikepdf/pikepdf#452].)\n\n[ppa]: https://inkscape.org/release/inkscape-1.2.2/gnulinux/ubuntu/ppa/dl/\n[pikepdf/pikepdf#452]: https://github.com/pikepdf/pikepdf/issues/452).\n\n### Release 1.2.0rc4 (2023-01-09)\n\nSupport python 3.11.\n\n#### Bugs\n\n- Shell-mode runner: fix readline/pexpect disagreement with respect to\n  horizontal scrolling of long lines.  In some cases, when Inkscape is\n  compiled to use GNU readline, long input lines will be scrolled\n  horizontally (even when stdin is not a tty). This messes with\n  pexpect's head. We've now added some basic tests for this, and set\n  some environment variables to try to convince readline not to do the\n  scrolling.\n\n#### Testing\n\n- Test under python 3.11\n- Fix tests for Windows environments where $APPDATA is not set\n- Fix tests for error message changes in packaging>=22\n\n### Release 1.2.0rc3 (2022-10-19)\n\n#### Extension/Symbols Installer\n\n- Make code for deducing Inkscape profile directory more robust.\n  (There's now a beter chance this will actually work on Windows.)\n- Support setting Inkscape profile directory via `$INKSCAPE_PROFILE_DIR`.\n\n### Release 1.2.0rc2 (2022-10-17)\n\n### Extension and Symbol Set Installation\n\n- This release add a `barnhunt install` (and `uninstall`) sub-command\n  to simplify installation of the\n  [inkex-bh](https://github.com/barnhunt/inkex-bh) Inkscape extensions\n  and [bh-symbols](https://github.com/barnhunt/bh-symbols) symbol\n  sets.\n\n#### Testing\n\n- Update to `mypy==0.982` for testing. Fix spurious mypy errors.\n\n### Release 1.2.0rc1 (2022-08-31)\n\nFirst public release to PyPI. Moved project to\n[GitHub](https://github.com/barnhunt/barnhunt).\n\n- Dropped support for python 3.6\n- Changed license to GPL version 3\n- We now do rudimentary testing under Windows and macOS.\n\n#### Dependencies\n\n- Use [pikepdf](https://pypi.org/project/pikepdf/) instead of\n  [pdfrw](https://pypi.org/project/pdfrw/) to manipulate PDFs.  (Pdfrw\n  seems not to be very actively maintained.) The only possible\n  downside of this is that `pikepdf` is not pure-python. It claims to\n  be easily installable on Windows and _x86_64_ Macs, but is not\n  (easily) installable on Macs with Apple silicon.\n\n- Generated PDFs are now [linearized][qpdf-linearize] and\n  [compressed][qpdf-object-streams].\n\n- Add test dependency on\n  [pdfminer.six](https://pypi.org/project/pdfminer.six/) (but drop\n  dependency on [PyPDF2](https://pypi.org/project/PyPDF2/)).\n\n\n#### Compatibility\n\n- Refactor `barnhunt.inkscape.runner` to support running\n  Inkscape >= 1.0 (as well as continuing to support Inkscape 0.9x).\n\n- Add `--inkscape-command` parameter to the `barnhunt pdfs` command\n  to specify the name/path of the Inkscape binary to run to export PDFs.\n  This also supports setting the Inkscape executable via the `$INKSCAPE_COMMAND`\n  environment variable.  Default executable is not `inkscape.exe` on Windows\n  (and `inkscape` everywhere else).\n\n- Use `pexpect.popen_spawn.PopenSpawn` instead of `pexpect.spawn` to\n  run Inkscape in shell-mode. Due to `pexpect.spawn`'s use of ptys, it\n  [will not work][pexpect-windows] on Windows.\n\n- **MacOS**: our code for running Inkscape in shell-mode appears to be broken.\n  For now, on _macOS_ we default to not using shell-mode.\n\n#### Packaging\n\n- Added a stub `barnhunt.__main__` module to allow running via `python\n  -m barnhunt`.\n\n#### Testing\n\n- Add type annotations.\n\n#### Bit Rot\n\n- Fix up tests to address deprecations in PyPDF2.\n\n[qpdf-linearize]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=linearize#option-linearize\n[qpdf-object-streams]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=object-streams#option-object-streams\n[pexpect-windows]: https://pexpect.readthedocs.io/en/stable/overview.html#windows\n\n### Release 1.1.0a1 (2022-03-08)\n\n#### \"Base Map\" support\n\nAdd ability to mark layers for exclusion from particular output files.\n\nThis adds the ability to list multiple comma-separated output base\nfilenames for a given overlay.\nE.g. A layer with label `\"[o|build_notes,base] Build Notes\"`\nwill define an overlay which will generate maps in two separate\noutput files.\n\nTagging a layer with `[!`_output-basename_`]` will exclude that\nlayer from any maps which are directed to the specified output\nfilename.\n\nTagging a layer with `[=`_output-basename_`]` will include that layer\nfrom any maps which are directed to the specified output filename, while\nexcluding all other sibling layers not explicitly tagged to be included\nin that output file.\n\n\n### Release 1.0.1 (2021-11-10)\n\n#### Diagnostics\n\n`Barnhunt pdfs` now issues a warning when generating PDFs from an SVG\nfile which does not have an explicit random-seed set.\n\n#### Bugs Fixed\n\nOpen SVG files in binary mode in order to let the XML parser figure\nout the encoding from the XML declaration.\n\n### Release 1.0 (2021-11-10)\n\nSupport python 3.10.\n\n#### Random Seed\n\nThe way the random seed (used for generating random rat numbers) for\neach SVG layer is computed has been changed in a\n**backward-incompatible** way.  This was done so that rat numbers can\nbe kept from changing when an SVG source file is copied or edited in\nsuch a way that the device and/or inode of the file changes.\n\nNow, the file-level random seed (an integer) is read from the\n`bh:random-seed` attribute of the root `svg` element of the SVG\nfile. If no `bh:random-seed` attribute is set, the file-level seed is\ncomputed by hashing the device and inode numbers of the SVG file.\n\nThe layer-level seed is formed by hashing the file-level random seed\nwith the XML *id* of the layer.\n\n(Formerly, the layer-level seed was form by hashing a triple of the\nfile-level seed (which was always zero), the hash of the SVG files\ndevice and inode, and the id of the layer.)\n\nA new `barnhunt random-seed` sub-command has been implemented to help\nwith setting the random seed for SVG source files.\n\n#### Bit-rot\n\nAddress `DeprecationWarning: 'contextfunction' is renamed to\n'pass_context'` from Jinja2. Require `Jinja2>3`.\n\n#### OCDisms\n\nRun `pyupgrade --py36-plus` on source.\n\n\n### Release 0.5 (2021-05-04)\n\nMake `-o` option to `2up` sub-command optional.\n\nRemove support for python < 3.6.\n\n### Release 0.4 (2019-02-25)\n\n#### New Sub-Command: 2up\n\nNew `2up` sub-command to format PDFs for 2-up printing.  Pages are\npre-shuffled so that the 2-up pages do not need to be shuffled after\ncutting.\n\n\n### Release 0.3 (2019-02-20)\n\n#### `barnhunt pdfs`\n\n- Multi-page output support.\n\n  There is a new syntax to specify the output file basename for an overlay.\n  Multiple overlays which specify the same output file will all be saved to\n  the same file.\n\n- It is now possible to render course maps from multiple SVG files in a\n  single invocation.  (Just list all the files to be rendered on the\n  command line.)\n\n#### Tests\n\n- `test_layerinfo.test_layerflags_str`: Fix test to deal with\n  arbitrary ordering of `enum.Flag` flags.\n\n### Release 0.2 (2018-11-07)\n\n#### Templating\n\n- Do not expand text within hidden layers.  This avoids generating\n  error messages (e.g. \"'overlay' is undefined\") due to template\n  expansion of unused text.\n\n- Add optional `skip` argument to the `random_rats` function.\n  This allows the generation of more than one set of stable random rat\n  numbers per layer.  E.g. `random_rats(skip=5)` will generate a set\n  of random number totally uncorrelated to that generated by\n  `random_rats()`.  Using `skip` has the advantage over using\n  `seed=None` that the results are stable and do not vary from\n  render to render.\n\n### Release 0.1 (2018-11-07)\n\n- Python 3.7 is now supported.\n\n- The template for the output filename has been generalized to work\n  sensibly in the case where overlays are nested more than two deep.\n\n#### Templating\n\n- Added new attributes to layers:\n\n  `layer.is_overlay`\n      Boolean.  True if layer is an overlay.\n\n  `layer.lineage`\n      Sequence starting with layer and including each parent layer in\n      turn.\n\n  `layer.overlay`\n      Returns the nearest overlay layer.  If the layer is an overlay,\n      `layer.overlay` returns `layer`, otherwise it returns the\n      nearest parent layer which is an overlay.  If the layer is not\n      contained within an overlay, returns `None`.\n\n- Added new values to context when expanding text in SVG:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the text\n      element, in order from outermost to innermost.\n\n  `course`\n      The outermost overlay layer.  (Equivalent to `overlays[0]`.)\n      This value already existed in the context used for filename expansion.\n\n  `overlay`\n      If the element is at least two overlays deep, this is the\n      innermost overlay.  Otherwise it is unset.  This value already\n      existed in the context used for filename expansion.\n\n- Added new values to context when expanding output filenames:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the overlay\n      being expanded.\n\n#### Bugs\n\n- Templating: the `safepath` filter would fail with a `TypeError`\n  if applied to anything but a string.  Now it coerces its argument to\n  text.\n\n- Templating: (New style) layer flags in parent layers were not being\n  removed from the layer labels.  (E.g. `\"{{ layer.parent.label }}\"`\n  was expanding to `\"[o] Some Overlay\"`, when it should expand to\n  `\"Some Overlay\"`.)\n\n- Pexpect==4.4.0 appears to have a subtle brokenness when\n  `searchwindowsize` is set to something other than `None`.  The\n  problem seems to be in [pexpect.expect.py][], and is triggered when\n  multiple chunks of output are read before a match is found.\n\n[pexpect.expect.py]: <https://github.com/pexpect/pexpect/blob/606f368b4a0dc442e2523d439d722a389b6e54c6/pexpect/expect.py#L22>\n\n#### Bit-Rot\n\n- Use `log.warning`, rather than the deprecated `log.warn`.\n\n### Release 0.1a12 (2017-02-09)\n\n- Remove tags from layer.label when expanding templated text in SVG file.\n\n### Release 0.1a11 (2017-02-01)\n\n- Add `--version` command line option\n\n#### Pager for `coords`\n\n- A fancy pager (poor man's `less`) has been added for viewing the\n  output of the `barnhunt coords` sub-command.  If any of `sys.stdin`\n  or `sys.stdout` is not a tty, then the pager will be disabled.\n\n- Since there is now a fancy pager, the default for `--number-of-rows`\n  has been increased to 1000.\n\n### Release 0.1a10 (2017-01-30)\n\n#### Things still to be fixed\n\nThings still to be fixed: I'm pretty sure things are direly broken if\na drawing contains no overlays, and somewhat broken if a drawing\ncontains more than two layers of overlays.  The problems have to do\nwith how the output PDF filenames are determined...\n\n#### New layer flag scheme\n\nNew scheme for marking overlay and hidden layers.  One can now set\nbit-flags on layers by including the flags in square brackets at the\nbeginning of the layer label.  I.e. a label like `\"[o] Master Trial\n1\"` marks the layer as an overlay layer, while `\"[h] Prototypes\"`\nmarks a hidden layer.\n\nIf no layers have any flags, `barnhunt pdfs` will fall back to the\nold name-based heuristics for determining hidden and overlay layers.\n\n\n### Release 0.1a9 (2017-01-03)\n\n* When exporting PDFs, run `inkscape` with `--export-area-page`.\n\n#### Packaging\n\n* Fix MANIFEST.in. Tests were not being included in sdist.\n\n* Add `url` to package metadata.\n\n### Release 0.1a8 (2018-01-03)\n\n* Ignore *ring* layers when identifying *course* layers.  (Now a layer\n  labeled “C8 Ring” will not be treated as a course layer.)\n\n* `pdfs`: default `--output-directory` to `.` (avoiding exception when no\n  explicit output directory is specified.)\n\n### Release 0.1a7 (2017-11-18)\n\n* Change `barnhunt coords` so that it omits duplicate coordinates in its output.\n  Also increase the default for `--number-of-rows` to 50 and\n  add the `--group-size` parameter to separate output into groups.\n\n### Release 0.1a6 (2017-11-15)\n\n* Templating: `LabelAdapter` now stringifies to the layer label, and\n  `FileAdapter` now stringifies to the file name.\n* More refactoring, more tests\n* Run several inkscapes in parallel.  This results in a major speedup.\n\n### Release 0.1a5 (2017-11-13)\n\n* Expand text in SVG file.\n* Add tests.\n* Major code refactor.\n\n### Release 0.1a4 (2017-11-10)\n\n#### PDFS\n\n* Log unexpected output from inkscape.\n\n* Add `--no-shell-mode-inkscape` option to control whether shell-mode inkscape\n  optimization is used.\n\n### Release 0.1a3.post1 (2017-11-10)\n\n#### PDFS\n\n* Reverse order that layers are considered.  (Layers are listed from\n  bottom to top in the SVG file.)\n\n### Release 0.1a3 (2017-11-10)\n\n#### PDFS\n\nReplace spaces and other shell-unfriendly characters with underscores\nin output file names.\n\n### Release 0.1a2 (2017-11-09)\n\nAdd sub-commands for generating random numbers.\n\n### Release 0.1a1 (2017-11-07)\n\nInitial release.\n"
 content-type = "text/markdown"
 
 [tool.pdm.version]
 source = "scm"
 write_to = "barnhunt/_version.py"
 write_template = "__version__ = \"{}\""
```

### Comparing `barnhunt-1.2.1rc1/stubs/pexpect/popen_spawn.pyi` & `barnhunt-1.2.1rc2/stubs/pexpect/popen_spawn.pyi`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/stubs/pexpect/spawnbase.pyi` & `barnhunt-1.2.1rc2/stubs/pexpect/spawnbase.pyi`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/conftest.py` & `barnhunt-1.2.1rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/inkscape/dummy_inkscape.py` & `barnhunt-1.2.1rc2/tests/inkscape/dummy_inkscape.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/inkscape/test_css.py` & `barnhunt-1.2.1rc2/tests/inkscape/test_css.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/inkscape/test_runner.py` & `barnhunt-1.2.1rc2/tests/inkscape/test_runner.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/inkscape/test_shell_mode_integration.py` & `barnhunt-1.2.1rc2/tests/inkscape/test_shell_mode_integration.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/inkscape/test_svg.py` & `barnhunt-1.2.1rc2/tests/inkscape/test_svg.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/inkscape/test_utils.py` & `barnhunt-1.2.1rc2/tests/inkscape/test_utils.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/installer/ratelimit.py` & `barnhunt-1.2.1rc2/tests/installer/ratelimit.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/installer/test_github.py` & `barnhunt-1.2.1rc2/tests/installer/test_github.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/installer/test_installer.py` & `barnhunt-1.2.1rc2/tests/installer/test_installer.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/installer/test_metadata.py` & `barnhunt-1.2.1rc2/tests/installer/test_metadata.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test1.pdf` & `barnhunt-1.2.1rc2/tests/test1.pdf`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test2.pdf` & `barnhunt-1.2.1rc2/tests/test2.pdf`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test_cli.py` & `barnhunt-1.2.1rc2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test_coursemaps.py` & `barnhunt-1.2.1rc2/tests/test_coursemaps.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test_functional.py` & `barnhunt-1.2.1rc2/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test_layerinfo.py` & `barnhunt-1.2.1rc2/tests/test_layerinfo.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test_pager.py` & `barnhunt-1.2.1rc2/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/test_pdfutil.py` & `barnhunt-1.2.1rc2/tests/test_pdfutil.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tests/testlib.py` & `barnhunt-1.2.1rc2/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.1rc1/tox.ini` & `barnhunt-1.2.1rc2/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -67,26 +67,22 @@
     types-atomicwrites
     types-lxml
     types-requests
 commands =
     mypy barnhunt tests
 
 [flake8]
-max-line-length = 80
+max-line-length = 88
 
 exclude =
     .tox,
     .git,
     __pycache__,
     .eggs
 
-select = C,E,F,W,B,B950
+#select = C,E,F,W,B,B950
 extend-ignore =
     # whitespace before ':' (conflicts with black)
-    E203,
-    # line too long (B950 is better)
-    E501,
-    # line break occurred before a binary operator (defunct)
-    W503
+    E203
 
 per-file-ignores =
     *.pyi: E301,E302,E701,E704
```

### Comparing `barnhunt-1.2.1rc1/PKG-INFO` & `barnhunt-1.2.1rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barnhunt
-Version: 1.2.1rc1
+Version: 1.2.1rc2
 Summary: Helpers for drawing Barn Hunt course maps using Inkscape
 Keywords: barn hunt inkscape course maps
 Author-Email: Jeff Dairiki <dairiki@dairiki.org>
 License: GPL-3.0-only
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -21,14 +21,15 @@
 Requires-Dist: jinja2~=3.1
 Requires-Dist: lxml~=4.9
 Requires-Dist: marshmallow~=3.19
 Requires-Dist: marshmallow-dataclass~=8.5.13
 Requires-Dist: packaging~=23.1
 Requires-Dist: pexpect~=4.8
 Requires-Dist: pikepdf~=6.2
+Requires-Dist: rdflib~=6.3
 Requires-Dist: requests~=2.29
 Requires-Dist: tinycss2~=1.2
 Requires-Dist: typing-extensions~=4.5; python_version < "3.10"
 Description-Content-Type: text/markdown
 
 # Barn Hunt Map Helper
 
@@ -155,14 +156,27 @@
 [pipx]: https://pypa.github.io/pipx/ (The pipx home page)
 [pip]: https://pip.pypa.io/en/stable/ (Documentation for pip)
 [pikepdf]: https://pikepdf.readthedocs.io/en/latest/installation.html
 (The Installation section of the pikepdf documentation)
 
 ## Changes
 
+### Release 1.2.1rc2 (2023-06-06)
+
+#### New Features
+
+- Provide access to RDF metadata in the SVG source in string
+  templates.  E.g. the document description may be interpolated via
+  `{{ rdf['dc:description'] }}`.
+
+#### Bugs Fixed
+
+- Fix parsing of version strings reported by pre-release versions of
+  Inkscape.
+
 ### Release 1.2.1rc1 (2023-05-22)
 
 (There was no final release of 1.2.0. It is a long story. I mistakenly
 committed a couple of files to LFS. To clear out LFS storage for a
 GitHub repo, one has to [delete the whole repo](😬). As a result, the
 workflow `$GITHUB_RUN_NUMBER` has reset. Thus a micro-version bump
 is required to keep those PyOxidizer windows build version numbers —
```

