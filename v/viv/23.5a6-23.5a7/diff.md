# Comparing `tmp/viv-23.5a6.tar.gz` & `tmp/viv-23.5a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viv-23.5a6.tar", last modified: Mon Jul 31 16:47:45 2023, max compression
+gzip compressed data, was "viv-23.5a7.tar", last modified: Thu Aug  3 23:28:24 2023, max compression
```

## Comparing `viv-23.5a6.tar` & `viv-23.5a7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-06-02 13:44:22.530182 viv-23.5a6/LICENSE
--rw-r--r--   0        0        0     3666 2023-06-02 19:09:37.319887 viv-23.5a6/README.md
--rw-r--r--   0        0        0      821 2023-06-02 21:56:40.027575 viv-23.5a6/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-02 13:44:22.533515 viv-23.5a6/src/viv/__init__.py
--rw-r--r--   0        0        0       61 2023-06-02 13:44:22.536848 viv-23.5a6/src/viv/__main__.py
--rwxr-xr-x   0        0        0    55937 2023-07-31 16:42:47.061951 viv-23.5a6/src/viv/viv.py
--rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 viv-23.5a6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-02 13:44:22.530182 viv-23.5a7/LICENSE
+-rw-r--r--   0        0        0     4163 2023-08-03 23:16:31.419220 viv-23.5a7/README.md
+-rw-r--r--   0        0        0      821 2023-06-02 21:56:40.027575 viv-23.5a7/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-02 13:44:22.533515 viv-23.5a7/src/viv/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-02 13:44:22.536848 viv-23.5a7/src/viv/__main__.py
+-rwxr-xr-x   0        0        0    57081 2023-08-03 23:18:41.836139 viv-23.5a7/src/viv/viv.py
+-rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 viv-23.5a7/PKG-INFO
```

### Comparing `viv-23.5a6/LICENSE` & `viv-23.5a7/LICENSE`

 * *Files identical despite different names*

### Comparing `viv-23.5a6/README.md` & `viv-23.5a7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,22 +19,27 @@
 
 Try before you buy!
 ```sh
 python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay -- "viv isn't venv\!"
 ```
 ---
 
-`Viv` is a standalone dependency-free `venv` creator.
+`Viv` is a standalone dependency-free `venv` creator [^1].
+`Viv` helps you ignore silly things like managing temporary or rarely used virtual environments,
+while still unleashing the full power of python scripting with it's entire ecosystem at your disposal.
 
 `Viv`'s uncompromising insistence on portability means that it will always:
 
 1. only use the standard library
 2. never exceed a single script.
 
-For that reason any usage of the `CLI` can be accomplished using a remote copy as seen in the below install command.
+For that reason any usage of the `cli` can be accomplished using a remote copy as seen in the below install command.
+
+Currently, the project is in alpha and in particular the `cli` is under active development and is subject to change.
+The basic feature set surrounding virtual environment/dependency management should remain stable however.
 
 ## Setup
 
 Run the below command to install `viv`.
 
 ```sh
 python3 <(curl -fsSL viv.dayl.in/viv.py) manage install
@@ -121,7 +126,9 @@
 ```sh
 pipx (1.1.0)
 ├── argcomplete>=1.9.4 (2.1.1)
 ├── packaging>=20.0 (23.0)
 └── userpath>=1.6.0 (1.8.0)
     └── click (8.1.3)
 ```
+
+[^1]: You do need to have `pip` but surely you have `pip` already.
```

#### html2text {}

```diff
@@ -1,45 +1,51 @@
                                     [Logo]
                          ****** viv isn't venv ******
                                [cli screenshot]
                                  Documentation
 Try before you buy! ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay
 -- "viv isn't venv\!" ``` --- `Viv` is a standalone dependency-free `venv`
-creator. `Viv`'s uncompromising insistence on portability means that it will
-always: 1. only use the standard library 2. never exceed a single script. For
-that reason any usage of the `CLI` can be accomplished using a remote copy as
-seen in the below install command. ## Setup Run the below command to install
-`viv`. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage install ``` To
-access `viv` from within scripts you should add it's location to your
-`PYTHONPATH`. By default `viv` will be installed to `$XDG_DATA_HOME/viv` or
-`~/.local/share/viv` you can customize this with `--src`. ```sh export
-PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv" ``` ### Pypi (Not Recommended)
-```sh pip install viv ``` Why is this *not recommended*? Mainly, because `viv`
-is all about hacking your `sys.path`. Placing it in it's own virtual
-environment or installing in a user site directory may complicate this
-endeavor. ## Usage In any python script with external dependencies you can add
-this line, to automate `vivenv` creation and installation of dependencies.
-```python __import__("viv").use("click") ``` To remove all `vivenvs` you can
-use the below command: ```sh viv remove $(viv list -q) ``` To remove `viv` all
-together you can use the included `purge` command: ```sh python3 <(curl -fsSL
-viv.dayl.in/viv.py) manage purge ``` ## Additional Features An experimental
-feature of `viv` is generating shim's that leverage the principles of `viv`.
-These shims would operate similar to `pipx` in which you can specify a command
-line app to "install". *Note* that `--standalone` will auto-generate a mini
-function version of `viv` to accomplish the same basic task as using a local
-copy of `viv`. After generating this standalone `shim` you can freely use this
-script across unix machines which have `python>3.8`. See [examples/black]
-(https://github.com/daylinmorgan/viv/blob/dev/examples/black) for output of
-below command. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) shim black -o ./
-black --standalone --freeze ``` ## Alternatives ### [pip-run](https://
-github.com/jaraco/pip-run) ```sh pip-run (10.0.5) âââ autocommand (2.2.2)
-âââ jaraco-context (4.3.0) âââ jaraco-functools (3.6.0) â
-âââ more-itertools (9.1.0) âââ jaraco-text (3.11.1) â âââ
-autocommand (2.2.2) â âââ inflect (6.0.2) â â âââ
-pydantic>=1.9.1 (1.10.5) â â âââ typing-extensions>=4.2.0 (4.5.0) â
-âââ jaraco-context>=4.1 (4.3.0) â âââ jaraco-functools (3.6.0)
-â â âââ more-itertools (9.1.0) â âââ more-itertools (9.1.0)
-âââ more-itertools>=8.3 (9.1.0) âââ packaging (23.0) âââ
-path>=15.1 (16.6.0) âââ pip>=19.3 (23.0.1) âââ platformdirs (3.1.0)
-``` ### [pipx](https://github.com/pypa/pipx/) ```sh pipx (1.1.0) âââ
-argcomplete>=1.9.4 (2.1.1) âââ packaging>=20.0 (23.0) âââ
-userpath>=1.6.0 (1.8.0) âââ click (8.1.3) ```
+creator [^1]. `Viv` helps you ignore silly things like managing temporary or
+rarely used virtual environments, while still unleashing the full power of
+python scripting with it's entire ecosystem at your disposal. `Viv`'s
+uncompromising insistence on portability means that it will always: 1. only use
+the standard library 2. never exceed a single script. For that reason any usage
+of the `cli` can be accomplished using a remote copy as seen in the below
+install command. Currently, the project is in alpha and in particular the `cli`
+is under active development and is subject to change. The basic feature set
+surrounding virtual environment/dependency management should remain stable
+however. ## Setup Run the below command to install `viv`. ```sh python3 <(curl
+-fsSL viv.dayl.in/viv.py) manage install ``` To access `viv` from within
+scripts you should add it's location to your `PYTHONPATH`. By default `viv`
+will be installed to `$XDG_DATA_HOME/viv` or `~/.local/share/viv` you can
+customize this with `--src`. ```sh export PYTHONPATH="$PYTHONPATH:$HOME/.local/
+share/viv" ``` ### Pypi (Not Recommended) ```sh pip install viv ``` Why is this
+*not recommended*? Mainly, because `viv` is all about hacking your `sys.path`.
+Placing it in it's own virtual environment or installing in a user site
+directory may complicate this endeavor. ## Usage In any python script with
+external dependencies you can add this line, to automate `vivenv` creation and
+installation of dependencies. ```python __import__("viv").use("click") ``` To
+remove all `vivenvs` you can use the below command: ```sh viv remove $(viv list
+-q) ``` To remove `viv` all together you can use the included `purge` command:
+```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge ``` ## Additional
+Features An experimental feature of `viv` is generating shim's that leverage
+the principles of `viv`. These shims would operate similar to `pipx` in which
+you can specify a command line app to "install". *Note* that `--standalone`
+will auto-generate a mini function version of `viv` to accomplish the same
+basic task as using a local copy of `viv`. After generating this standalone
+`shim` you can freely use this script across unix machines which have
+`python>3.8`. See [examples/black](https://github.com/daylinmorgan/viv/blob/
+dev/examples/black) for output of below command. ```sh python3 <(curl -fsSL
+viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze ``` ##
+Alternatives ### [pip-run](https://github.com/jaraco/pip-run) ```sh pip-run
+(10.0.5) âââ autocommand (2.2.2) âââ jaraco-context (4.3.0)
+âââ jaraco-functools (3.6.0) â âââ more-itertools (9.1.0)
+âââ jaraco-text (3.11.1) â âââ autocommand (2.2.2) â âââ
+inflect (6.0.2) â â âââ pydantic>=1.9.1 (1.10.5) â â âââ
+typing-extensions>=4.2.0 (4.5.0) â âââ jaraco-context>=4.1 (4.3.0) â
+âââ jaraco-functools (3.6.0) â â âââ more-itertools (9.1.0) â
+âââ more-itertools (9.1.0) âââ more-itertools>=8.3 (9.1.0)
+âââ packaging (23.0) âââ path>=15.1 (16.6.0) âââ pip>=19.3
+(23.0.1) âââ platformdirs (3.1.0) ``` ### [pipx](https://github.com/pypa/
+pipx/) ```sh pipx (1.1.0) âââ argcomplete>=1.9.4 (2.1.1) âââ
+packaging>=20.0 (23.0) âââ userpath>=1.6.0 (1.8.0) âââ click
+(8.1.3) ``` [^1]: You do need to have `pip` but surely you have `pip` already.
```

### Comparing `viv-23.5a6/pyproject.toml` & `viv-23.5a7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 authors = [
     { name = "Daylin Morgan", email = "daylinmorgan@gmail.com" },
 ]
 dependencies = []
 requires-python = ">= 3.8"
 readme = "README.md"
 dynamic = []
-version = "23.5a6"
+version = "23.5a7"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/daylinmorgan/viv"
 repository = "https://github.com/daylinmorgan/viv"
```

### Comparing `viv-23.5a6/src/viv/viv.py` & `viv-23.5a7/src/viv/viv.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     TextIO,
     Tuple,
     Type,
 )
 from urllib.error import HTTPError
 from urllib.request import urlopen
 
-__version__ = "23.5a6"
+__version__ = "23.5a7"
 
 
 class Spinner:
     """spinner modified from:
     https://raw.githubusercontent.com/Tagar/stuff/master/spinner.py
     """
 
@@ -782,17 +782,19 @@
         spec: List[str] = [""],
         track_exe: bool = False,
         id: str | None = None,
         name: str = "",
         path: Path | None = None,
         skip_load: bool = False,
         metadata: Meta | None = None,
+        skip_validation: bool = False,
     ) -> None:
         self.loaded = False
-        spec = self._validate_spec(spec)
+        if not skip_validation:
+            spec = self._validate_spec(spec)
         id = id if id else get_hash(spec, track_exe)
 
         self.name = name if name else id[:8]
         self.set_path(path)
 
         if not metadata:
             if self.name in (d.name for d in Cache().venv.iterdir()):
@@ -840,14 +842,15 @@
 
     def create(self, quiet: bool = False) -> None:
         log.info(f"new unique vivenv: {a.bold}{self.name}{a.end}")
         log.debug(f"creating new venv at {self.path}")
         with Spinner("creating vivenv"):
             venv.create(
                 self.path,
+                prompt=f"viv-{self.name}",
                 clear=True,
                 symlinks=True,
             )
 
         self.meta.created = str(datetime.today())
 
     def install_pkgs(self) -> None:
@@ -1019,22 +1022,54 @@
     os.chmod(path, mode)
 
 
 def uses_viv(txt: str) -> bool:
     return bool(
         re.search(
             """
-            \s*__import__\(\s*["']viv["']\s*\).use\(.*
+            ^(?!\#)\s*
+            (?:__import__\(\s*["']viv["']\s*\))
             |
-            from\ viv\ import\ use
+            (?:from\ viv\ import\ use)
             |
-            import\ viv 
+            (?:import\ viv)
         """,
             txt,
-            re.VERBOSE,
+            re.VERBOSE | re.MULTILINE,
+        )
+    )
+
+
+def _read_metadata_block(txt: str) -> None:
+    """check for pep722 style metadata block and parse"""
+
+    lines = iter(txt.splitlines())
+    for line in lines:
+        if line.startswith("##"):
+            block_type, sep, extra = line[2:].strip().partition(":")
+            if not sep:
+                continue
+            block_data = []
+            for line in lines:
+                if not line.startswith("##"):
+                    break
+                line = line[2:].strip()
+                if not line:
+                    continue
+                block_data.append(line)
+            yield block_type, extra, block_data
+
+
+def deps_block(txt: str):
+    return list(
+        (
+            req
+            for block_type, extra, block_data in _read_metadata_block(txt)
+            for req in block_data
+            if block_type == "Script Dependencies"
         )
     )
 
 
 class Viv:
     def __init__(self) -> None:
         self.t = Template()
@@ -1347,31 +1382,88 @@
         examples:
           viv shim black
           viv shim yartsu -o ~/bin/yartsu --standalone
         """
         default_bin, bin = self._pick_bin(reqs, bin)
         output = Env().viv_bin_dir / default_bin if not output else output.absolute()
 
-        if output.is_file():
-            err_quit(f"{output} already exists...exiting")
-
         if freeze:
             spec = resolve_deps(reqs, requirements)
         else:
             spec = combined_spec(reqs, requirements)
 
+        if output.is_file():
+            log.warning(f"{output} already exists")
+
         if confirm(
             f"Write shim for {a.bold}{bin}{a.end} to {a.green}{output}{a.end}?",
             yes=yes,
         ):
             with output.open("w") as f:
                 f.write(self.t.shim(path, self.local_source, standalone, spec, bin))
 
             make_executable(output)
 
+    def _run_script(
+        self, spec: List[str], script: str, keep: bool, rest: List[str]
+    ) -> None:
+        env = os.environ
+        name = script.split("/")[-1]
+
+        # TODO: reduce boilerplate and dry out
+        with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
+            tmppath = Path(tmpdir)
+            scriptpath = tmppath / name
+            if not self.local_source:
+                (tmppath / "viv.py").write_text(
+                    # TODO: use latest tag once ready
+                    fetch_script(
+                        "https://raw.githubusercontent.com/daylinmorgan/viv/dev/src/viv/viv.py"
+                    )
+                )
+
+            if Path(script).is_file():
+                script_text = Path(script).read_text()
+            else:
+                script_text = fetch_script(script)
+
+            viv_used = uses_viv(script_text)
+            deps = deps_block(script_text)
+
+            if viv_used and deps_block:
+                error(
+                    "Script Dependencies block and "
+                    "`viv` API can't be used in the same script"
+                )
+
+            scriptpath.write_text(script_text)
+
+            if not keep:
+                env.update({"VIV_CACHE": tmpdir})
+                os.environ["VIV_CACHE"] = tmpdir
+
+            if viv_used:
+                env.update({"VIV_SPEC": " ".join(f"'{req}'" for req in spec)})
+
+                sys.exit(
+                    subprocess.run(
+                        [sys.executable, scriptpath, *rest], env=env
+                    ).returncode
+                )
+            else:
+                vivenv = ViVenv(spec + deps)
+                if not vivenv.loaded or Env().viv_force:
+                    vivenv.create()
+                    vivenv.install_pkgs()
+
+                vivenv.touch()
+                vivenv.meta.write()
+
+                sys.exit(subprocess.run([vivenv.python, scriptpath, *rest]).returncode)
+
     def run(
         self,
         reqs: List[str],
         requirements: Path,
         script: str,
         keep: bool,
         rest: List[str],
@@ -1385,62 +1477,15 @@
           viv r rich -b python -- -m rich
           viv r -s <remote python script>
         """
 
         spec = combined_spec(reqs, requirements)
 
         if script:
-            env = os.environ
-            name = script.split("/")[-1]
-
-            # TODO: reduce boilerplate and dry out
-            with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
-                tmppath = Path(tmpdir)
-                scriptpath = tmppath / name
-                if not self.local_source:
-                    (tmppath / "viv.py").write_text(
-                        # TODO: use latest tag once ready
-                        fetch_script(
-                            "https://raw.githubusercontent.com/daylinmorgan/viv/dev/src/viv/viv.py"
-                        )
-                    )
-
-                if Path(script).is_file():
-                    script_text = Path(script).read_text()
-                else:
-                    script_text = fetch_script(script)
-
-                viv_used = uses_viv(script_text)
-                scriptpath.write_text(script_text)
-
-                if not keep:
-                    env.update({"VIV_CACHE": tmpdir})
-                    os.environ["VIV_CACHE"] = tmpdir
-
-                if viv_used:
-                    env.update({"VIV_SPEC": " ".join(f"'{req}'" for req in spec)})
-
-                    sys.exit(
-                        subprocess.run(
-                            [sys.executable, scriptpath, *rest], env=env
-                        ).returncode
-                    )
-                else:
-                    vivenv = ViVenv(spec)
-                    if not vivenv.loaded or Env().viv_force:
-                        vivenv.create()
-                        vivenv.install_pkgs()
-
-                    vivenv.touch()
-                    vivenv.meta.write()
-
-                    sys.exit(
-                        subprocess.run([vivenv.python, scriptpath, *rest]).returncode
-                    )
-
+            self._run_script(spec, script, keep, rest)
         else:
             _, bin = self._pick_bin(reqs, bin)
             vivenv = ViVenv(spec)
 
             # TODO: respect a VIV_RUN_MODE env variable as the same as keep i.e.
             # ephemeral (default), semi-ephemeral (persist inside /tmp), or
             # persist (use c.cache)
@@ -1455,19 +1500,19 @@
                             subprocess.run(
                                 [vivenv.path / "bin" / bin, *rest]
                             ).returncode
                         )
                 else:
                     vivenv.create()
                     vivenv.install_pkgs()
-
-            vivenv.touch()
-            vivenv.meta.write()
-
-            sys.exit(subprocess.run([vivenv.path / "bin" / bin, *rest]).returncode)
+                    vivenv.touch()
+                    vivenv.meta.write()
+                    sys.exit(
+                        subprocess.run([vivenv.path / "bin" / bin, *rest]).returncode
+                    )
 
 
 class Arg:
     def __init__(self, *args: str, **kwargs: Any) -> None:
         self.args = args
         self.kwargs = kwargs
 
@@ -1655,57 +1700,59 @@
 
     def _add_args(self) -> None:
         for grp, args in self.args.items():
             for arg in args:
                 self.parsers[grp].add_argument(*arg.args, **arg.kwargs)
 
     def _validate_args(self, args: Namespace) -> None:
-        if args.func.__name__ in ("freeze", "shim"):
+        name = args.func.__name__
+        if name in ("freeze", "shim"):
             if not args.reqs:
                 error("must specify a requirement")
-        if args.func.__name__ in ("freeze", "shim"):
+
             if not self.viv.local_source and not (args.standalone or args.path):
                 log.warning(
                     "failed to find local copy of `viv` "
                     "make sure to add it to your PYTHONPATH "
                     "or consider using --path/--standalone"
                 )
 
             # TODO: move this since this is code logic not flag logic
             if args.path and not self.viv.local_source:
                 error("No local viv found to import from")
 
             if args.path and args.standalone:
                 error("-p/--path and -s/--standalone are mutually exclusive")
 
-        if args.func.__name__ == "manage_install" and self.viv.local_source:
+        if name == "manage_install" and self.viv.local_source:
             error(
                 f"found existing viv installation at {self.viv.local_source}",
                 "use "
                 + a.style("viv manage update", "bold")
                 + " to modify current installation.",
             )
 
-        if args.func.__name__ == "manage_update":
+        if name == "manage_update":
             if not self.viv.local_source:
                 error(
                     a.style("viv manage update", "bold")
                     + " should be used with an exisiting installation",
                 )
 
             if self.viv.git:
                 error(
                     a.style("viv manage update", "bold")
                     + " shouldn't be used with a git-based installation",
                 )
-        if args.func.__name__ == "run":
+
+        if name == "run":
             if not (args.reqs or args.script):
                 error("must specify a requirement or --script")
 
-        if args.func.__name__ == "info":
+        if name == "info":
             if args.use_json and args.path:
                 error("--json and -p/--path are mutually exclusive")
 
     def _get_subcmd_parser(
         self,
         subparsers: _SubParsersAction[ArgumentParser],
         name: str,
@@ -1752,15 +1799,14 @@
                     subcmd_cmd_p.add_parser(
                         subcmd,
                         parents=[
                             self.parsers[k]
                             for k in self.cmd_arg_group_map[f"{cmd}|{subcmd}"]
                         ],
                         **kwargs,
-                        # ).set_defaults(func=getattr(self.viv, cmd), subcmd=subcmd)
                     ).set_defaults(func=getattr(self.viv, f"{cmd}_{subcmd}"))
 
             else:
                 self._get_subcmd_parser(
                     cmd_p,
                     cmd,
                     parents=[self.parsers.get(k) for k in self.cmd_arg_group_map[cmd]],
```

### Comparing `viv-23.5a6/PKG-INFO` & `viv-23.5a7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viv
-Version: 23.5a6
+Version: 23.5a7
 Summary: viv isn't venv
 License: MIT
 Author-email: Daylin Morgan <daylinmorgan@gmail.com>
 Requires-Python: >= 3.8
 Project-URL: homepage, https://github.com/daylinmorgan/viv
 Project-URL: repository, https://github.com/daylinmorgan/viv
 Description-Content-Type: text/markdown
@@ -30,22 +30,27 @@
 
 Try before you buy!
 ```sh
 python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay -- "viv isn't venv\!"
 ```
 ---
 
-`Viv` is a standalone dependency-free `venv` creator.
+`Viv` is a standalone dependency-free `venv` creator [^1].
+`Viv` helps you ignore silly things like managing temporary or rarely used virtual environments,
+while still unleashing the full power of python scripting with it's entire ecosystem at your disposal.
 
 `Viv`'s uncompromising insistence on portability means that it will always:
 
 1. only use the standard library
 2. never exceed a single script.
 
-For that reason any usage of the `CLI` can be accomplished using a remote copy as seen in the below install command.
+For that reason any usage of the `cli` can be accomplished using a remote copy as seen in the below install command.
+
+Currently, the project is in alpha and in particular the `cli` is under active development and is subject to change.
+The basic feature set surrounding virtual environment/dependency management should remain stable however.
 
 ## Setup
 
 Run the below command to install `viv`.
 
 ```sh
 python3 <(curl -fsSL viv.dayl.in/viv.py) manage install
@@ -133,7 +138,9 @@
 pipx (1.1.0)
 ├── argcomplete>=1.9.4 (2.1.1)
 ├── packaging>=20.0 (23.0)
 └── userpath>=1.6.0 (1.8.0)
     └── click (8.1.3)
 ```
 
+[^1]: You do need to have `pip` but surely you have `pip` already.
+
```

#### html2text {}

```diff
@@ -1,50 +1,56 @@
-Metadata-Version: 2.1 Name: viv Version: 23.5a6 Summary: viv isn't venv
+Metadata-Version: 2.1 Name: viv Version: 23.5a7 Summary: viv isn't venv
 License: MIT Author-email: Daylin Morgan
 gmail.com> Requires-Python: >= 3.8 Project-URL: homepage, https://github.com/
 daylinmorgan/viv Project-URL: repository, https://github.com/daylinmorgan/viv
 Description-Content-Type: text/markdown
                                     [Logo]
                          ****** viv isn't venv ******
                                [cli screenshot]
                                  Documentation
 Try before you buy! ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay
 -- "viv isn't venv\!" ``` --- `Viv` is a standalone dependency-free `venv`
-creator. `Viv`'s uncompromising insistence on portability means that it will
-always: 1. only use the standard library 2. never exceed a single script. For
-that reason any usage of the `CLI` can be accomplished using a remote copy as
-seen in the below install command. ## Setup Run the below command to install
-`viv`. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage install ``` To
-access `viv` from within scripts you should add it's location to your
-`PYTHONPATH`. By default `viv` will be installed to `$XDG_DATA_HOME/viv` or
-`~/.local/share/viv` you can customize this with `--src`. ```sh export
-PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv" ``` ### Pypi (Not Recommended)
-```sh pip install viv ``` Why is this *not recommended*? Mainly, because `viv`
-is all about hacking your `sys.path`. Placing it in it's own virtual
-environment or installing in a user site directory may complicate this
-endeavor. ## Usage In any python script with external dependencies you can add
-this line, to automate `vivenv` creation and installation of dependencies.
-```python __import__("viv").use("click") ``` To remove all `vivenvs` you can
-use the below command: ```sh viv remove $(viv list -q) ``` To remove `viv` all
-together you can use the included `purge` command: ```sh python3 <(curl -fsSL
-viv.dayl.in/viv.py) manage purge ``` ## Additional Features An experimental
-feature of `viv` is generating shim's that leverage the principles of `viv`.
-These shims would operate similar to `pipx` in which you can specify a command
-line app to "install". *Note* that `--standalone` will auto-generate a mini
-function version of `viv` to accomplish the same basic task as using a local
-copy of `viv`. After generating this standalone `shim` you can freely use this
-script across unix machines which have `python>3.8`. See [examples/black]
-(https://github.com/daylinmorgan/viv/blob/dev/examples/black) for output of
-below command. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) shim black -o ./
-black --standalone --freeze ``` ## Alternatives ### [pip-run](https://
-github.com/jaraco/pip-run) ```sh pip-run (10.0.5) âââ autocommand (2.2.2)
-âââ jaraco-context (4.3.0) âââ jaraco-functools (3.6.0) â
-âââ more-itertools (9.1.0) âââ jaraco-text (3.11.1) â âââ
-autocommand (2.2.2) â âââ inflect (6.0.2) â â âââ
-pydantic>=1.9.1 (1.10.5) â â âââ typing-extensions>=4.2.0 (4.5.0) â
-âââ jaraco-context>=4.1 (4.3.0) â âââ jaraco-functools (3.6.0)
-â â âââ more-itertools (9.1.0) â âââ more-itertools (9.1.0)
-âââ more-itertools>=8.3 (9.1.0) âââ packaging (23.0) âââ
-path>=15.1 (16.6.0) âââ pip>=19.3 (23.0.1) âââ platformdirs (3.1.0)
-``` ### [pipx](https://github.com/pypa/pipx/) ```sh pipx (1.1.0) âââ
-argcomplete>=1.9.4 (2.1.1) âââ packaging>=20.0 (23.0) âââ
-userpath>=1.6.0 (1.8.0) âââ click (8.1.3) ```
+creator [^1]. `Viv` helps you ignore silly things like managing temporary or
+rarely used virtual environments, while still unleashing the full power of
+python scripting with it's entire ecosystem at your disposal. `Viv`'s
+uncompromising insistence on portability means that it will always: 1. only use
+the standard library 2. never exceed a single script. For that reason any usage
+of the `cli` can be accomplished using a remote copy as seen in the below
+install command. Currently, the project is in alpha and in particular the `cli`
+is under active development and is subject to change. The basic feature set
+surrounding virtual environment/dependency management should remain stable
+however. ## Setup Run the below command to install `viv`. ```sh python3 <(curl
+-fsSL viv.dayl.in/viv.py) manage install ``` To access `viv` from within
+scripts you should add it's location to your `PYTHONPATH`. By default `viv`
+will be installed to `$XDG_DATA_HOME/viv` or `~/.local/share/viv` you can
+customize this with `--src`. ```sh export PYTHONPATH="$PYTHONPATH:$HOME/.local/
+share/viv" ``` ### Pypi (Not Recommended) ```sh pip install viv ``` Why is this
+*not recommended*? Mainly, because `viv` is all about hacking your `sys.path`.
+Placing it in it's own virtual environment or installing in a user site
+directory may complicate this endeavor. ## Usage In any python script with
+external dependencies you can add this line, to automate `vivenv` creation and
+installation of dependencies. ```python __import__("viv").use("click") ``` To
+remove all `vivenvs` you can use the below command: ```sh viv remove $(viv list
+-q) ``` To remove `viv` all together you can use the included `purge` command:
+```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge ``` ## Additional
+Features An experimental feature of `viv` is generating shim's that leverage
+the principles of `viv`. These shims would operate similar to `pipx` in which
+you can specify a command line app to "install". *Note* that `--standalone`
+will auto-generate a mini function version of `viv` to accomplish the same
+basic task as using a local copy of `viv`. After generating this standalone
+`shim` you can freely use this script across unix machines which have
+`python>3.8`. See [examples/black](https://github.com/daylinmorgan/viv/blob/
+dev/examples/black) for output of below command. ```sh python3 <(curl -fsSL
+viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze ``` ##
+Alternatives ### [pip-run](https://github.com/jaraco/pip-run) ```sh pip-run
+(10.0.5) âââ autocommand (2.2.2) âââ jaraco-context (4.3.0)
+âââ jaraco-functools (3.6.0) â âââ more-itertools (9.1.0)
+âââ jaraco-text (3.11.1) â âââ autocommand (2.2.2) â âââ
+inflect (6.0.2) â â âââ pydantic>=1.9.1 (1.10.5) â â âââ
+typing-extensions>=4.2.0 (4.5.0) â âââ jaraco-context>=4.1 (4.3.0) â
+âââ jaraco-functools (3.6.0) â â âââ more-itertools (9.1.0) â
+âââ more-itertools (9.1.0) âââ more-itertools>=8.3 (9.1.0)
+âââ packaging (23.0) âââ path>=15.1 (16.6.0) âââ pip>=19.3
+(23.0.1) âââ platformdirs (3.1.0) ``` ### [pipx](https://github.com/pypa/
+pipx/) ```sh pipx (1.1.0) âââ argcomplete>=1.9.4 (2.1.1) âââ
+packaging>=20.0 (23.0) âââ userpath>=1.6.0 (1.8.0) âââ click
+(8.1.3) ``` [^1]: You do need to have `pip` but surely you have `pip` already.
```

