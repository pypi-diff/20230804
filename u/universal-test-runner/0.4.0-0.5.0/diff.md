# Comparing `tmp/universal_test_runner-0.4.0.tar.gz` & `tmp/universal_test_runner-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_test_runner-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "universal_test_runner-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `universal_test_runner-0.4.0.tar` & `universal_test_runner-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.4.0/LICENSE
--rw-r--r--   0        0        0     7088 2023-06-29 02:00:26.259769 universal_test_runner-0.4.0/README.md
--rw-r--r--   0        0        0     1364 2023-07-01 23:10:25.755823 universal_test_runner-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.4.0/universal_test_runner/__init__.py
--rw-r--r--   0        0        0      628 2023-06-19 22:38:42.426279 universal_test_runner-0.4.0/universal_test_runner/cli.py
--rw-r--r--   0        0        0     1791 2023-07-01 23:05:16.489107 universal_test_runner-0.4.0/universal_test_runner/context.py
--rw-r--r--   0        0        0     4996 2023-07-01 23:05:13.811691 universal_test_runner-0.4.0/universal_test_runner/matchers.py
--rw-r--r--   0        0        0     1027 2023-06-28 03:19:59.457422 universal_test_runner-0.4.0/universal_test_runner/runner.py
--rw-r--r--   0        0        0     8381 1970-01-01 00:00:00.000000 universal_test_runner-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8156 2023-08-04 04:43:41.936625 universal_test_runner-0.5.0/README.md
+-rw-r--r--   0        0        0     1410 2023-08-04 04:44:11.509957 universal_test_runner-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.5.0/universal_test_runner/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-19 22:38:42.426279 universal_test_runner-0.5.0/universal_test_runner/cli.py
+-rw-r--r--   0        0        0     1791 2023-07-01 23:05:16.489107 universal_test_runner-0.5.0/universal_test_runner/context.py
+-rw-r--r--   0        0        0     5208 2023-08-04 04:43:41.937247 universal_test_runner-0.5.0/universal_test_runner/matchers.py
+-rw-r--r--   0        0        0     1027 2023-06-28 03:19:59.457422 universal_test_runner-0.5.0/universal_test_runner/runner.py
+-rw-r--r--   0        0        0     9449 1970-01-01 00:00:00.000000 universal_test_runner-0.5.0/PKG-INFO
```

### Comparing `universal_test_runner-0.4.0/LICENSE` & `universal_test_runner-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.4.0/README.md` & `universal_test_runner-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # universal-test-runner
 
 The Universal Test Runner is a zero-configuration, language-aware way to run unit tests in any project. It installs a command, `t`, which will determine how to run your test suite (and then run it).
 
 <p align="center">
-   <a href="https://github.com/xavdid/test-runner-demo/raw/main/_demo/demo-min.gif">
-      <img src="https://github.com/xavdid/test-runner-demo/raw/main/_demo/demo-min.gif"/>
+   <a href="https://github.com/xavdid/test-runner-demo/blob/main/_demo/demo-min.gif">
+      <img src="https://raw.githubusercontent.com/xavdid/test-runner-demo/main/_demo/demo-min.gif"/>
    </a>
 </p>
 
 If you're working on a JS project, it runs `[your package manager here] test`. You've run `pytest` in this folder before? `pytest` it is. Rust project? `cargo test` coming right up. Is also clever about running all your `go` module tests (regardless of how they're organized). No matter the command, all args are passed directly into the test runner.
 
 Currently [supports 7 languages](#supported-languages) (and their respective test frameworks). Please open an issue if I'm missing your favorite!
 
 ## Installation
 
-Universal Test Runner is available on [PyPi](https://pypi.org/project/universal-test-runner/) (for installation via [pipx](https://pypa.github.io/pipx/)):
+The easiest way to install is by using [pipx](https://pypa.github.io/pipx/):
 
 ```bash
 pipx install universal-test-runner
 ```
 
+You can also use brew (which will build from source and take a little longer):
+
+```bash
+brew install xavdid/projects/universal-test-runner
+```
+
 ## Usage
 
 > You can also clone the [demo repo](https://github.com/xavdid/test-runner-demo) to play around with the test runner - it's got toy examples to show how tests are run in many languages!
 
 Once installed, the command `t` will be available. Run it in a project folder's root and it'll do its best to run your unit tests:
 
 ```
@@ -88,37 +94,47 @@
 ...
 
 [universal-test-runner]: no matching test handler. To add a new one, please file an issue: https://github.com/xavdid/universal-test-runner/issues
 ```
 
 ## Supported Languages
 
-This tree describes the rough priority order within each language (not the languages themselves).
+This list describes how each language behaves (but not the order in which languages are matched; use the [debugger](#debugging) for that).
+
+- Python
+  - checks for `manage.py` (Django)
+  - else uses `pytest` if you've run `pytest` before. You'll need to run pytest manually on clean installs before `t` will work
+  - looks for a `tests.py` file if not
+- Rust
+  - `cargo test`
+- Go
+  - if there's a `X_test.go`, then runs a plain `go test`
+  - if you pass any args at all, runs `go test your-args-here`
+  - otherwise, runs `go test ./...`
+- Elixir
+  - `mix test`
+- Clojure
+  - `lein test`
+- Javascript/Typescript
+  - if there's a `package.json` and it has a `test` script, runs `[package manager] test`, where `[package manager]` is:
+    - `npm` if there's a `package-lock.json`
+    - `yarn` if there's a `yarn.lock`
+    - `pnpm` if there's a `pnpm-lock.yaml`
+- [justfile](https://github.com/casey/just)
+  - uses the JSON api to find a `test` command
+- Makefile
+  - looks for a line that starts with `test:`
+
+### Exercism
+
+[Exercism](https://exercism.org/) is a platform for learning new programming languages. It has more than 65 tracks available. The Universal Test Runner supports nearly all of them out of the box using the [Exercism CLI](https://exercism.org/docs/using/solving-exercises/working-locally)'s `exercism test` command. Just like this tool, it knows how to run each track's tests and invokes the correct one automatically.
+
+Rather than re-implement all of the test commands `exercism` can handle, the runner will invoke the Exercism CLI when run from an exercise directory. This requires version `3.2.0` of the Exercism CLI installed.
 
-1. Python
-   - checks for `manage.py` (Django)
-   - else uses `pytest` if you've run `pytest` before. You'll need to run pytest manually on clean installs before `t` will work
-   - looks for a `tests.py` file if not
-2. Rust
-   - `cargo test`
-3. Go
-   - if there's a `X_test.go`, then runs a plain `go test`
-   - if you pass any args at all, runs `go test your-args-here`
-   - otherwise, runs `go test ./...`
-4. Elixir
-   - runs `mix test`
-5. Clojure
-   - runs `lein test`
-6. Makefile
-   - looks for a line that starts with `test:`
-7. Javascript/Typescript
-   - if there's a `package.json` and it has a `test` script, runs `[package manager] test`, where `[package manager]` is:
-     - `npm` if there's a `package-lock.json`
-     - `yarn` if there's a `yarn.lock`
-     - `pnpm` if there's a `pnpm-lock.yaml`
+> fun fact: I [added the test command](https://github.com/exercism/cli/pull/1092) after it was suggested in the [forum thread](https://forum.exercism.org/t/introducing-the-universal-test-runner/6228) where I announced the Universal Test Runner
 
 ## Motivation
 
 I work in a few languages at a time, so I've actually had a [version of this in my dotfiles](https://github.com/xavdid/dotfiles/blob/6bd5f56b1f9ad2dcef9f8b72413d30779b378aef/node/aliases.zsh#L45-L73) for a while. Also, as I've been doing [Exercism's #12in23 program](https://exercism.org/challenges/12in23), I'm _really_ switching languages. It's nice not to have to re-learn any muscle memory. Plus, increasingly complex `bash` was holding me back.
 
 ### Design Philosophy
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
 # universal-test-runner The Universal Test Runner is a zero-configuration,
 language-aware way to run unit tests in any project. It installs a command,
 `t`, which will determine how to run your test suite (and then run it).
-   [https://github.com/xavdid/test-runner-demo/raw/main/_demo/demo-min.gif]
+  [https://raw.githubusercontent.com/xavdid/test-runner-demo/main/_demo/demo-
+                                   min.gif]
 If you're working on a JS project, it runs `[your package manager here] test`.
 You've run `pytest` in this folder before? `pytest` it is. Rust project? `cargo
 test` coming right up. Is also clever about running all your `go` module tests
 (regardless of how they're organized). No matter the command, all args are
 passed directly into the test runner. Currently [supports 7 languages]
 (#supported-languages) (and their respective test frameworks). Please open an
-issue if I'm missing your favorite! ## Installation Universal Test Runner is
-available on [PyPi](https://pypi.org/project/universal-test-runner/) (for
-installation via [pipx](https://pypa.github.io/pipx/)): ```bash pipx install
-universal-test-runner ``` ## Usage > You can also clone the [demo repo](https:/
-/github.com/xavdid/test-runner-demo) to play around with the test runner - it's
-got toy examples to show how tests are run in many languages! Once installed,
-the command `t` will be available. Run it in a project folder's root and it'll
-do its best to run your unit tests: ``` % t -> pytest
+issue if I'm missing your favorite! ## Installation The easiest way to install
+is by using [pipx](https://pypa.github.io/pipx/): ```bash pipx install
+universal-test-runner ``` You can also use brew (which will build from source
+and take a little longer): ```bash brew install xavdid/projects/universal-test-
+runner ``` ## Usage > You can also clone the [demo repo](https://github.com/
+xavdid/test-runner-demo) to play around with the test runner - it's got toy
+examples to show how tests are run in many languages! Once installed, the
+command `t` will be available. Run it in a project folder's root and it'll do
+its best to run your unit tests: ``` % t -> pytest
 =============================== test session starts
 ================================ platform darwin -- Python 3.11.0, pytest-
 7.3.1, pluggy-1.0.0 rootdir: /Users/username/projects/test-runner collected 78
 items tests/test_cli.py ... [ 3%] tests/test_context.py .....................
 [ 30%] tests/test_matchers.py
 .................................................. [ 94%] tests/test_runner.py
 .... [100%] ================================ 78 passed in 0.08s
@@ -47,27 +49,40 @@
 [universal-test-runner]: Checking matcher 03/11: go_multi [universal-test-
 runner]: looking for: "go.mod" and no arguments [universal-test-runner]: no
 match, continuing [universal-test-runner]: Checking matcher 04/11: go_single
 [universal-test-runner]: looking for: "go.mod" or a file named "..._test.go"
 [universal-test-runner]: no match, continuing ... [universal-test-runner]: no
 matching test handler. To add a new one, please file an issue: https://
 github.com/xavdid/universal-test-runner/issues ``` ## Supported Languages This
-tree describes the rough priority order within each language (not the languages
-themselves). 1. Python - checks for `manage.py` (Django) - else uses `pytest`
-if you've run `pytest` before. You'll need to run pytest manually on clean
-installs before `t` will work - looks for a `tests.py` file if not 2. Rust -
-`cargo test` 3. Go - if there's a `X_test.go`, then runs a plain `go test` - if
-you pass any args at all, runs `go test your-args-here` - otherwise, runs `go
-test ./...` 4. Elixir - runs `mix test` 5. Clojure - runs `lein test` 6.
-Makefile - looks for a line that starts with `test:` 7. Javascript/Typescript -
-if there's a `package.json` and it has a `test` script, runs `[package manager]
-test`, where `[package manager]` is: - `npm` if there's a `package-lock.json` -
-`yarn` if there's a `yarn.lock` - `pnpm` if there's a `pnpm-lock.yaml` ##
-Motivation I work in a few languages at a time, so I've actually had a [version
-of this in my dotfiles](https://github.com/xavdid/dotfiles/blob/
+list describes how each language behaves (but not the order in which languages
+are matched; use the [debugger](#debugging) for that). - Python - checks for
+`manage.py` (Django) - else uses `pytest` if you've run `pytest` before. You'll
+need to run pytest manually on clean installs before `t` will work - looks for
+a `tests.py` file if not - Rust - `cargo test` - Go - if there's a `X_test.go`,
+then runs a plain `go test` - if you pass any args at all, runs `go test your-
+args-here` - otherwise, runs `go test ./...` - Elixir - `mix test` - Clojure -
+`lein test` - Javascript/Typescript - if there's a `package.json` and it has a
+`test` script, runs `[package manager] test`, where `[package manager]` is: -
+`npm` if there's a `package-lock.json` - `yarn` if there's a `yarn.lock` -
+`pnpm` if there's a `pnpm-lock.yaml` - [justfile](https://github.com/casey/
+just) - uses the JSON api to find a `test` command - Makefile - looks for a
+line that starts with `test:` ### Exercism [Exercism](https://exercism.org/) is
+a platform for learning new programming languages. It has more than 65 tracks
+available. The Universal Test Runner supports nearly all of them out of the box
+using the [Exercism CLI](https://exercism.org/docs/using/solving-exercises/
+working-locally)'s `exercism test` command. Just like this tool, it knows how
+to run each track's tests and invokes the correct one automatically. Rather
+than re-implement all of the test commands `exercism` can handle, the runner
+will invoke the Exercism CLI when run from an exercise directory. This requires
+version `3.2.0` of the Exercism CLI installed. > fun fact: I [added the test
+command](https://github.com/exercism/cli/pull/1092) after it was suggested in
+the [forum thread](https://forum.exercism.org/t/introducing-the-universal-test-
+runner/6228) where I announced the Universal Test Runner ## Motivation I work
+in a few languages at a time, so I've actually had a [version of this in my
+dotfiles](https://github.com/xavdid/dotfiles/blob/
 6bd5f56b1f9ad2dcef9f8b72413d30779b378aef/node/aliases.zsh#L45-L73) for a while.
 Also, as I've been doing [Exercism's #12in23 program](https://exercism.org/
 challenges/12in23), I'm _really_ switching languages. It's nice not to have to
 re-learn any muscle memory. Plus, increasingly complex `bash` was holding me
 back. ### Design Philosophy 1. The runner itself should need no configuration -
 it Just Works 2. It should pass all arguments through to the underlying test
 command 3. It should have wide language and test runner support; please open an
```

### Comparing `universal_test_runner-0.4.0/pyproject.toml` & `universal_test_runner-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "universal-test-runner"
-version = "0.4.0"
+version = "0.5.0"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Universal, language-aware unit test runner."
 readme = "README.md"
 license = { file = "LICENSE" }
 
 requires-python = ">=3.9"
@@ -19,15 +19,15 @@
 keywords = ["testing", "test-runner", "pytest"]
 
 dependencies = ["click==8.1.3", "colorama==0.4.6"]
 
 [project.optional-dependencies]
 test = ["pytest==7.3.1", "responses==0.23.1"]
 release = ["twine==4.0.2", "build==0.10.0"]
-ci = ["black==23.3.0", "isort==5.12.0", "pyright==1.1.309"]
+ci = ["black==23.3.0", "pyright==1.1.309", "ruff==0.0.277"]
 
 [project.urls]
 "Homepage" = "https://github.com/xavdid/universal-test-runner"
 "Bug Tracker" = "https://github.com/xavdid/universal-test-runner/issues"
 "Author" = "https://xavd.id"
 "Changelog" = "https://github.com/xavdid/universal-test-runner/blob/main/CHANGELOG.md"
 
@@ -38,9 +38,10 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 # needed so the LSP performs typechecking
 [tool.pyright]
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+select = ["E", "F", "I001"] # defaults & isort
+ignore = ["E501"]
```

### Comparing `universal_test_runner-0.4.0/universal_test_runner/cli.py` & `universal_test_runner-0.5.0/universal_test_runner/cli.py`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.4.0/universal_test_runner/context.py` & `universal_test_runner-0.5.0/universal_test_runner/context.py`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.4.0/universal_test_runner/matchers.py` & `universal_test_runner-0.5.0/universal_test_runner/matchers.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     "go test",
     debug_line='looking for: "go.mod" or a file named "..._test.go"',
 )
 
 makefile = Matcher(
     "makefile",
     lambda c: c.has_files("Makefile")
-    and any(l.startswith("test:") for l in c.read_file("Makefile")),
+    and any(line.startswith("test:") for line in c.read_file("Makefile")),
     "make test",
     debug_line='looking for: a "Makefile" and a "test:" line',
 )
 
 
 def _matches_justfile(c: Context) -> bool:
     # TODO: better capitalization support? the file is supposed to be case-insensitive
@@ -88,15 +88,15 @@
         return "test" in file.get("recipes", {})
 
     except (FileNotFoundError, subprocess.CalledProcessError):
         # either:
         # - just isn't installed
         # - something else went wrong (probably an invalid justfile)
         # in either case, fall back to a more basic check and let `just` error out if relevant
-        return any(re.match(r"^@?test(:| )", l) for l in c.read_file("justfile"))
+        return any(re.match(r"^@?test(:| )", line) for line in c.read_file("justfile"))
 
 
 justfile = Matcher(
     "justfile",
     _matches_justfile,
     "just test",
     debug_line='looking for: a "justfile" and a "test" or "@test" line',
@@ -112,21 +112,23 @@
 # misc simple cases
 pytest = Matcher.basic_builder("pytest", ".pytest_cache", "pytest")
 py = Matcher.basic_builder("py", "tests.py", "python tests.py")
 django = Matcher.basic_builder("django", "manage.py", "./manage.py test")
 elixir = Matcher.basic_builder("elixir", "mix.exs", "mix test")
 rust = Matcher.basic_builder("rust", "Cargo.toml", "cargo test")
 clojure = Matcher.basic_builder("clojure", "project.clj", "lein test")
+exercism = Matcher.basic_builder("exercism", ".exercism", "exercism test")
 
 # these are checked in order
 ALL_MATCHERS: list[Matcher] = [
     justfile,
+    exercism,
     makefile,
-    # anything that could run pytest should go before it
     django,
+    # anything that could run pytest should go before it
     pytest,
     py,
     # ensure ordering for go matchers
     go_multi,
     go_single,
     elixir,
     rust,
@@ -149,11 +151,12 @@
         if matcher.matches(context):
             context.debug("matched!", indent=4)
             context.debug(f"would have run: `{matcher._command}`", indent=6)
             return [*matcher.command, *context.args]
 
         context.debug("no match, continuing", indent=4)
 
+    # LOAD BEARING - the homebrew formula expects "no matching test handler" to be present if there's no match
     context.debug(
         "no matching test handler. To add a new one, please file an issue: https://github.com/xavdid/universal-test-runner/issues"
     )
     return []
```

### Comparing `universal_test_runner-0.4.0/universal_test_runner/runner.py` & `universal_test_runner-0.5.0/universal_test_runner/runner.py`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.4.0/PKG-INFO` & `universal_test_runner-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: universal-test-runner
-Version: 0.4.0
+Version: 0.5.0
 Summary: Universal, language-aware unit test runner.
 Keywords: testing,test-runner,pytest
 Author-email: David Brownman <beamneocube@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: click==8.1.3
 Requires-Dist: colorama==0.4.6
 Requires-Dist: black==23.3.0 ; extra == "ci"
-Requires-Dist: isort==5.12.0 ; extra == "ci"
 Requires-Dist: pyright==1.1.309 ; extra == "ci"
+Requires-Dist: ruff==0.0.277 ; extra == "ci"
 Requires-Dist: twine==4.0.2 ; extra == "release"
 Requires-Dist: build==0.10.0 ; extra == "release"
 Requires-Dist: pytest==7.3.1 ; extra == "test"
 Requires-Dist: responses==0.23.1 ; extra == "test"
 Project-URL: Author, https://xavd.id
 Project-URL: Bug Tracker, https://github.com/xavdid/universal-test-runner/issues
 Project-URL: Changelog, https://github.com/xavdid/universal-test-runner/blob/main/CHANGELOG.md
@@ -30,31 +30,37 @@
 Provides-Extra: test
 
 # universal-test-runner
 
 The Universal Test Runner is a zero-configuration, language-aware way to run unit tests in any project. It installs a command, `t`, which will determine how to run your test suite (and then run it).
 
 <p align="center">
-   <a href="https://github.com/xavdid/test-runner-demo/raw/main/_demo/demo-min.gif">
-      <img src="https://github.com/xavdid/test-runner-demo/raw/main/_demo/demo-min.gif"/>
+   <a href="https://github.com/xavdid/test-runner-demo/blob/main/_demo/demo-min.gif">
+      <img src="https://raw.githubusercontent.com/xavdid/test-runner-demo/main/_demo/demo-min.gif"/>
    </a>
 </p>
 
 If you're working on a JS project, it runs `[your package manager here] test`. You've run `pytest` in this folder before? `pytest` it is. Rust project? `cargo test` coming right up. Is also clever about running all your `go` module tests (regardless of how they're organized). No matter the command, all args are passed directly into the test runner.
 
 Currently [supports 7 languages](#supported-languages) (and their respective test frameworks). Please open an issue if I'm missing your favorite!
 
 ## Installation
 
-Universal Test Runner is available on [PyPi](https://pypi.org/project/universal-test-runner/) (for installation via [pipx](https://pypa.github.io/pipx/)):
+The easiest way to install is by using [pipx](https://pypa.github.io/pipx/):
 
 ```bash
 pipx install universal-test-runner
 ```
 
+You can also use brew (which will build from source and take a little longer):
+
+```bash
+brew install xavdid/projects/universal-test-runner
+```
+
 ## Usage
 
 > You can also clone the [demo repo](https://github.com/xavdid/test-runner-demo) to play around with the test runner - it's got toy examples to show how tests are run in many languages!
 
 Once installed, the command `t` will be available. Run it in a project folder's root and it'll do its best to run your unit tests:
 
 ```
@@ -119,37 +125,47 @@
 ...
 
 [universal-test-runner]: no matching test handler. To add a new one, please file an issue: https://github.com/xavdid/universal-test-runner/issues
 ```
 
 ## Supported Languages
 
-This tree describes the rough priority order within each language (not the languages themselves).
+This list describes how each language behaves (but not the order in which languages are matched; use the [debugger](#debugging) for that).
+
+- Python
+  - checks for `manage.py` (Django)
+  - else uses `pytest` if you've run `pytest` before. You'll need to run pytest manually on clean installs before `t` will work
+  - looks for a `tests.py` file if not
+- Rust
+  - `cargo test`
+- Go
+  - if there's a `X_test.go`, then runs a plain `go test`
+  - if you pass any args at all, runs `go test your-args-here`
+  - otherwise, runs `go test ./...`
+- Elixir
+  - `mix test`
+- Clojure
+  - `lein test`
+- Javascript/Typescript
+  - if there's a `package.json` and it has a `test` script, runs `[package manager] test`, where `[package manager]` is:
+    - `npm` if there's a `package-lock.json`
+    - `yarn` if there's a `yarn.lock`
+    - `pnpm` if there's a `pnpm-lock.yaml`
+- [justfile](https://github.com/casey/just)
+  - uses the JSON api to find a `test` command
+- Makefile
+  - looks for a line that starts with `test:`
+
+### Exercism
+
+[Exercism](https://exercism.org/) is a platform for learning new programming languages. It has more than 65 tracks available. The Universal Test Runner supports nearly all of them out of the box using the [Exercism CLI](https://exercism.org/docs/using/solving-exercises/working-locally)'s `exercism test` command. Just like this tool, it knows how to run each track's tests and invokes the correct one automatically.
+
+Rather than re-implement all of the test commands `exercism` can handle, the runner will invoke the Exercism CLI when run from an exercise directory. This requires version `3.2.0` of the Exercism CLI installed.
 
-1. Python
-   - checks for `manage.py` (Django)
-   - else uses `pytest` if you've run `pytest` before. You'll need to run pytest manually on clean installs before `t` will work
-   - looks for a `tests.py` file if not
-2. Rust
-   - `cargo test`
-3. Go
-   - if there's a `X_test.go`, then runs a plain `go test`
-   - if you pass any args at all, runs `go test your-args-here`
-   - otherwise, runs `go test ./...`
-4. Elixir
-   - runs `mix test`
-5. Clojure
-   - runs `lein test`
-6. Makefile
-   - looks for a line that starts with `test:`
-7. Javascript/Typescript
-   - if there's a `package.json` and it has a `test` script, runs `[package manager] test`, where `[package manager]` is:
-     - `npm` if there's a `package-lock.json`
-     - `yarn` if there's a `yarn.lock`
-     - `pnpm` if there's a `pnpm-lock.yaml`
+> fun fact: I [added the test command](https://github.com/exercism/cli/pull/1092) after it was suggested in the [forum thread](https://forum.exercism.org/t/introducing-the-universal-test-runner/6228) where I announced the Universal Test Runner
 
 ## Motivation
 
 I work in a few languages at a time, so I've actually had a [version of this in my dotfiles](https://github.com/xavdid/dotfiles/blob/6bd5f56b1f9ad2dcef9f8b72413d30779b378aef/node/aliases.zsh#L45-L73) for a while. Also, as I've been doing [Exercism's #12in23 program](https://exercism.org/challenges/12in23), I'm _really_ switching languages. It's nice not to have to re-learn any muscle memory. Plus, increasingly complex `bash` was holding me back.
 
 ### Design Philosophy
```

#### html2text {}

```diff
@@ -1,43 +1,45 @@
-Metadata-Version: 2.1 Name: universal-test-runner Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: universal-test-runner Version: 0.5.0 Summary:
 Universal, language-aware unit test runner. Keywords: testing,test-
 runner,pytest Author-email: David Brownman
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing Requires-Dist:
 click==8.1.3 Requires-Dist: colorama==0.4.6 Requires-Dist: black==23.3.0 ;
-extra == "ci" Requires-Dist: isort==5.12.0 ; extra == "ci" Requires-Dist:
-pyright==1.1.309 ; extra == "ci" Requires-Dist: twine==4.0.2 ; extra ==
-"release" Requires-Dist: build==0.10.0 ; extra == "release" Requires-Dist:
-pytest==7.3.1 ; extra == "test" Requires-Dist: responses==0.23.1 ; extra ==
-"test" Project-URL: Author, https://xavd.id Project-URL: Bug Tracker, https://
-github.com/xavdid/universal-test-runner/issues Project-URL: Changelog, https://
-github.com/xavdid/universal-test-runner/blob/main/CHANGELOG.md Project-URL:
-Homepage, https://github.com/xavdid/universal-test-runner Provides-Extra: ci
-Provides-Extra: release Provides-Extra: test # universal-test-runner The
-Universal Test Runner is a zero-configuration, language-aware way to run unit
-tests in any project. It installs a command, `t`, which will determine how to
-run your test suite (and then run it).
-   [https://github.com/xavdid/test-runner-demo/raw/main/_demo/demo-min.gif]
+extra == "ci" Requires-Dist: pyright==1.1.309 ; extra == "ci" Requires-Dist:
+ruff==0.0.277 ; extra == "ci" Requires-Dist: twine==4.0.2 ; extra == "release"
+Requires-Dist: build==0.10.0 ; extra == "release" Requires-Dist: pytest==7.3.1
+; extra == "test" Requires-Dist: responses==0.23.1 ; extra == "test" Project-
+URL: Author, https://xavd.id Project-URL: Bug Tracker, https://github.com/
+xavdid/universal-test-runner/issues Project-URL: Changelog, https://github.com/
+xavdid/universal-test-runner/blob/main/CHANGELOG.md Project-URL: Homepage,
+https://github.com/xavdid/universal-test-runner Provides-Extra: ci Provides-
+Extra: release Provides-Extra: test # universal-test-runner The Universal Test
+Runner is a zero-configuration, language-aware way to run unit tests in any
+project. It installs a command, `t`, which will determine how to run your test
+suite (and then run it).
+  [https://raw.githubusercontent.com/xavdid/test-runner-demo/main/_demo/demo-
+                                   min.gif]
 If you're working on a JS project, it runs `[your package manager here] test`.
 You've run `pytest` in this folder before? `pytest` it is. Rust project? `cargo
 test` coming right up. Is also clever about running all your `go` module tests
 (regardless of how they're organized). No matter the command, all args are
 passed directly into the test runner. Currently [supports 7 languages]
 (#supported-languages) (and their respective test frameworks). Please open an
-issue if I'm missing your favorite! ## Installation Universal Test Runner is
-available on [PyPi](https://pypi.org/project/universal-test-runner/) (for
-installation via [pipx](https://pypa.github.io/pipx/)): ```bash pipx install
-universal-test-runner ``` ## Usage > You can also clone the [demo repo](https:/
-/github.com/xavdid/test-runner-demo) to play around with the test runner - it's
-got toy examples to show how tests are run in many languages! Once installed,
-the command `t` will be available. Run it in a project folder's root and it'll
-do its best to run your unit tests: ``` % t -> pytest
+issue if I'm missing your favorite! ## Installation The easiest way to install
+is by using [pipx](https://pypa.github.io/pipx/): ```bash pipx install
+universal-test-runner ``` You can also use brew (which will build from source
+and take a little longer): ```bash brew install xavdid/projects/universal-test-
+runner ``` ## Usage > You can also clone the [demo repo](https://github.com/
+xavdid/test-runner-demo) to play around with the test runner - it's got toy
+examples to show how tests are run in many languages! Once installed, the
+command `t` will be available. Run it in a project folder's root and it'll do
+its best to run your unit tests: ``` % t -> pytest
 =============================== test session starts
 ================================ platform darwin -- Python 3.11.0, pytest-
 7.3.1, pluggy-1.0.0 rootdir: /Users/username/projects/test-runner collected 78
 items tests/test_cli.py ... [ 3%] tests/test_context.py .....................
 [ 30%] tests/test_matchers.py
 .................................................. [ 94%] tests/test_runner.py
 .... [100%] ================================ 78 passed in 0.08s
@@ -65,27 +67,40 @@
 [universal-test-runner]: Checking matcher 03/11: go_multi [universal-test-
 runner]: looking for: "go.mod" and no arguments [universal-test-runner]: no
 match, continuing [universal-test-runner]: Checking matcher 04/11: go_single
 [universal-test-runner]: looking for: "go.mod" or a file named "..._test.go"
 [universal-test-runner]: no match, continuing ... [universal-test-runner]: no
 matching test handler. To add a new one, please file an issue: https://
 github.com/xavdid/universal-test-runner/issues ``` ## Supported Languages This
-tree describes the rough priority order within each language (not the languages
-themselves). 1. Python - checks for `manage.py` (Django) - else uses `pytest`
-if you've run `pytest` before. You'll need to run pytest manually on clean
-installs before `t` will work - looks for a `tests.py` file if not 2. Rust -
-`cargo test` 3. Go - if there's a `X_test.go`, then runs a plain `go test` - if
-you pass any args at all, runs `go test your-args-here` - otherwise, runs `go
-test ./...` 4. Elixir - runs `mix test` 5. Clojure - runs `lein test` 6.
-Makefile - looks for a line that starts with `test:` 7. Javascript/Typescript -
-if there's a `package.json` and it has a `test` script, runs `[package manager]
-test`, where `[package manager]` is: - `npm` if there's a `package-lock.json` -
-`yarn` if there's a `yarn.lock` - `pnpm` if there's a `pnpm-lock.yaml` ##
-Motivation I work in a few languages at a time, so I've actually had a [version
-of this in my dotfiles](https://github.com/xavdid/dotfiles/blob/
+list describes how each language behaves (but not the order in which languages
+are matched; use the [debugger](#debugging) for that). - Python - checks for
+`manage.py` (Django) - else uses `pytest` if you've run `pytest` before. You'll
+need to run pytest manually on clean installs before `t` will work - looks for
+a `tests.py` file if not - Rust - `cargo test` - Go - if there's a `X_test.go`,
+then runs a plain `go test` - if you pass any args at all, runs `go test your-
+args-here` - otherwise, runs `go test ./...` - Elixir - `mix test` - Clojure -
+`lein test` - Javascript/Typescript - if there's a `package.json` and it has a
+`test` script, runs `[package manager] test`, where `[package manager]` is: -
+`npm` if there's a `package-lock.json` - `yarn` if there's a `yarn.lock` -
+`pnpm` if there's a `pnpm-lock.yaml` - [justfile](https://github.com/casey/
+just) - uses the JSON api to find a `test` command - Makefile - looks for a
+line that starts with `test:` ### Exercism [Exercism](https://exercism.org/) is
+a platform for learning new programming languages. It has more than 65 tracks
+available. The Universal Test Runner supports nearly all of them out of the box
+using the [Exercism CLI](https://exercism.org/docs/using/solving-exercises/
+working-locally)'s `exercism test` command. Just like this tool, it knows how
+to run each track's tests and invokes the correct one automatically. Rather
+than re-implement all of the test commands `exercism` can handle, the runner
+will invoke the Exercism CLI when run from an exercise directory. This requires
+version `3.2.0` of the Exercism CLI installed. > fun fact: I [added the test
+command](https://github.com/exercism/cli/pull/1092) after it was suggested in
+the [forum thread](https://forum.exercism.org/t/introducing-the-universal-test-
+runner/6228) where I announced the Universal Test Runner ## Motivation I work
+in a few languages at a time, so I've actually had a [version of this in my
+dotfiles](https://github.com/xavdid/dotfiles/blob/
 6bd5f56b1f9ad2dcef9f8b72413d30779b378aef/node/aliases.zsh#L45-L73) for a while.
 Also, as I've been doing [Exercism's #12in23 program](https://exercism.org/
 challenges/12in23), I'm _really_ switching languages. It's nice not to have to
 re-learn any muscle memory. Plus, increasingly complex `bash` was holding me
 back. ### Design Philosophy 1. The runner itself should need no configuration -
 it Just Works 2. It should pass all arguments through to the underlying test
 command 3. It should have wide language and test runner support; please open an
```

