# Comparing `tmp/giza_cli-0.0.2.tar.gz` & `tmp/giza_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_cli-0.0.2.tar", max compression
+gzip compressed data, was "giza_cli-0.2.0.tar", max compression
```

## Comparing `giza_cli-0.0.2.tar` & `giza_cli-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rw-r--r--   0        0        0     1074 2023-07-13 09:38:22.745132 giza_cli-0.0.2/LICENSE
--rw-r--r--   0        0        0     4276 2023-07-13 09:38:22.745132 giza_cli-0.0.2/README.md
--rw-r--r--   0        0        0       61 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/__init__.py
--rw-r--r--   0        0        0       77 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/__main__.py
--rw-r--r--   0        0        0     1048 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/callbacks.py
--rw-r--r--   0        0        0     1145 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/cli.py
--rw-r--r--   0        0        0     9779 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/client.py
--rw-r--r--   0        0        0        0 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/__init__.py
--rw-r--r--   0        0        0     2126 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/transpile.py
--rw-r--r--   0        0        0     5159 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/users.py
--rw-r--r--   0        0        0      372 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/commands/version.py
--rw-r--r--   0        0        0      241 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/options.py
--rw-r--r--   0        0        0      107 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/schemas/token.py
--rw-r--r--   0        0        0      902 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/schemas/users.py
--rw-r--r--   0        0        0      771 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/utils/__init__.py
--rw-r--r--   0        0        0     1244 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/utils/decorators.py
--rw-r--r--   0        0        0     3568 2023-07-13 09:38:22.745132 giza_cli-0.0.2/giza/utils/echo.py
--rw-r--r--   0        0        0     1375 2023-07-13 09:38:22.745132 giza_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 giza_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-03 22:19:55.070398 giza_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4197 2023-08-03 22:19:55.070398 giza_cli-0.2.0/README.md
+-rw-r--r--   0        0        0       82 2023-08-03 22:19:55.070398 giza_cli-0.2.0/giza/__init__.py
+-rw-r--r--   0        0        0       77 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/__main__.py
+-rw-r--r--   0        0        0     1039 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/callbacks.py
+-rw-r--r--   0        0        0     1773 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/cli.py
+-rw-r--r--   0        0        0    19147 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/client.py
+-rw-r--r--   0        0        0        0 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/commands/__init__.py
+-rw-r--r--   0        0        0     4492 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/commands/models.py
+-rw-r--r--   0        0        0     3377 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/commands/prove.py
+-rw-r--r--   0        0        0     4533 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/commands/transpile.py
+-rw-r--r--   0        0        0     5071 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/commands/users.py
+-rw-r--r--   0        0        0      372 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/commands/version.py
+-rw-r--r--   0        0        0      241 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/options.py
+-rw-r--r--   0        0        0      426 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/schemas/jobs.py
+-rw-r--r--   0        0        0      457 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/schemas/models.py
+-rw-r--r--   0        0        0      194 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/schemas/proofs.py
+-rw-r--r--   0        0        0      107 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/schemas/token.py
+-rw-r--r--   0        0        0      902 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/schemas/users.py
+-rw-r--r--   0        0        0      791 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/utils/__init__.py
+-rw-r--r--   0        0        0     1244 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/utils/decorators.py
+-rw-r--r--   0        0        0     3720 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/utils/echo.py
+-rw-r--r--   0        0        0      462 2023-08-03 22:19:55.074398 giza_cli-0.2.0/giza/utils/enums.py
+-rw-r--r--   0        0        0     1426 2023-08-03 22:19:55.074398 giza_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 giza_cli-0.2.0/PKG-INFO
```

### Comparing `giza_cli-0.0.2/LICENSE` & `giza_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.2/README.md` & `giza_cli-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Giza Command Line Interface
 
-![Logo](https://framerusercontent.com/images/dGhFEb4pIwUJ5SArbs7udVlSs.png)
 [![GitHub Workflow Status](https://github.com/gizatechxyz/giza-cli/actions/workflows/onpush.yml/badge.svg)](https://github.com/gizatechxyz/giza-cli/actions/workflows/onpush.yml)
 [![Project license](https://img.shields.io/github/license/gizatechxyz/orion.svg?style=flat-square)](LICENSE)
 [![Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg?style=flat-square)](https://github.com/gizatechxyz/orion/issues?q=is%3Aissue+is%3Aopen)
 [![Join the community](https://dcbadge.vercel.app/api/server/FR3Cd88x6r?style=flat-square)](https://discord.gg/FR3Cd88x6r)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
@@ -15,17 +14,17 @@
 |  |  __  |  | `---/  /     /  ^  \       |  ,----'|  |     |  |
 |  | |_ | |  |    /  /     /  /_\  \      |  |     |  |     |  |
 |  |__| | |  |   /  /----./  _____  \     |  `----.|  `----.|  |
  \______| |__|  /________/__/     \__\     \______||_______||__|
 
 ```
 
-Welcome to Giza`s Platform CLI!
+Welcome to Giza CLI!
 
-This CLI provides the utilities to interact with Giza Platform using the terminal.
+This CLI provides the utilities to interact with Giza using the terminal.
 
 **Discalimer**: this is still in an experimental stage so the functionality is subject to change.
 
 - [Giza Command Line Interface](#giza-command-line-interface)
   - [🚀 Installation](#-installation)
     - [Recomended installation with pipx](#recomended-installation-with-pipx)
     - [Install from PyPi](#install-from-pypi)
@@ -68,15 +67,15 @@
 
 ```bash
   pip install git+ssh://git@github.com/gizatechxyz/giza-cli.git
 ```
 
 ## 📚 Documentation
 
-You can check our official docs [here](https://giza-cli.gizatech.xyz/main).
+You can check our official docs [here](https://orion-giza.gitbook.io/main-1/welcome/readme).
 
 - **Examples** includes examples on how to use the CLI functionalities.
 
 - **Resources** brings the documentation of the different resources and actions that can be done with the CLI.
 
 - 🧠 **Reference** for the API reference and internals of the CLI.
```

#### html2text {}

```diff
@@ -1,47 +1,46 @@
-# Giza Command Line Interface ![Logo](https://framerusercontent.com/images/
-dGhFEb4pIwUJ5SArbs7udVlSs.png) [![GitHub Workflow Status](https://github.com/
+# Giza Command Line Interface [![GitHub Workflow Status](https://github.com/
 gizatechxyz/giza-cli/actions/workflows/onpush.yml/badge.svg)](https://
 github.com/gizatechxyz/giza-cli/actions/workflows/onpush.yml) [![Project
 license](https://img.shields.io/github/license/gizatechxyz/
 orion.svg?style=flat-square)](LICENSE) [![Pull Requests welcome](https://
 img.shields.io/badge/PRs-welcome-ff69b4.svg?style=flat-square)](https://
 github.com/gizatechxyz/orion/issues?q=is%3Aissue+is%3Aopen) [![Join the
 community](https://dcbadge.vercel.app/api/server/FR3Cd88x6r?style=flat-square)]
 (https://discord.gg/FR3Cd88x6r)  [![All Contributors](https://img.shields.io/
 badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-
 )  ```text _______ __ ________ ___ ______ __ __ / _____|| | | / / \ / || | | |
 | | __ | | `---/ / / ^ \ | ,----'| | | | | | |_ | | | / / / /_\ \ | | | | | | |
 |__| | | | / /----./ _____ \ | `----.| `----.| | \______| |__| /________/__/
-\__\ \______||_______||__| ``` Welcome to Giza`s Platform CLI! This CLI
-provides the utilities to interact with Giza Platform using the terminal.
-**Discalimer**: this is still in an experimental stage so the functionality is
-subject to change. - [Giza Command Line Interface](#giza-command-line-
-interface) - [ð Installation](#-installation) - [Recomended installation
-with pipx](#recomended-installation-with-pipx) - [Install from PyPi](#install-
-from-pypi) - [Installing from source](#installing-from-source) - [ð
-Documentation](#-documentation) - [ð What's new](#-whats-new) - [ð¤ Join
-the community!](#-join-the-community) - [Contributors â¨](#contributors-) -
-[License](#license) ## ð Installation ### Recomended installation with pipx
-[pipx](https://pypa.github.io/pipx/) allows to install the dependency in an
-isolated environment. With ths we can make sure that it does not conflict with
-any of our installed dependencies. ```bash pipx install giza-cli ``` ###
-Install from PyPi For the latest release: ```bash pip install giza-cli ``` ###
-Installing from source Clone the repository and install it with `pip`: ```bash
-git clone git@github.com:gizatechxyz/giza-cli.git cd giza-cli pip install . ```
-Or install it directly from the repo: ```bash pip install git+ssh://
+\__\ \______||_______||__| ``` Welcome to Giza CLI! This CLI provides the
+utilities to interact with Giza using the terminal. **Discalimer**: this is
+still in an experimental stage so the functionality is subject to change. -
+[Giza Command Line Interface](#giza-command-line-interface) - [ð
+Installation](#-installation) - [Recomended installation with pipx]
+(#recomended-installation-with-pipx) - [Install from PyPi](#install-from-pypi)
+- [Installing from source](#installing-from-source) - [ð Documentation](#-
+documentation) - [ð What's new](#-whats-new) - [ð¤ Join the community!](#-
+join-the-community) - [Contributors â¨](#contributors-) - [License](#license)
+## ð Installation ### Recomended installation with pipx [pipx](https://
+pypa.github.io/pipx/) allows to install the dependency in an isolated
+environment. With ths we can make sure that it does not conflict with any of
+our installed dependencies. ```bash pipx install giza-cli ``` ### Install from
+PyPi For the latest release: ```bash pip install giza-cli ``` ### Installing
+from source Clone the repository and install it with `pip`: ```bash git clone
+git@github.com:gizatechxyz/giza-cli.git cd giza-cli pip install . ``` Or
+install it directly from the repo: ```bash pip install git+ssh://
 git@github.com/gizatechxyz/giza-cli.git ``` ## ð Documentation You can check
-our official docs [here](https://giza-cli.gizatech.xyz/main). - **Examples**
-includes examples on how to use the CLI functionalities. - **Resources** brings
-the documentation of the different resources and actions that can be done with
-the CLI. - ð§  **Reference** for the API reference and internals of the CLI.
-## ð What's new For a detailed list of changes, please refer to the
-[CHANGELOG](CHANGELOG.md) file. ## ð¤ Join the community! Join the community
-and help build a safer and transparent AI in our [Discord](https://discord.gg/
-Kt24CsMb5k)! ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
+our official docs [here](https://orion-giza.gitbook.io/main-1/welcome/readme).
+- **Examples** includes examples on how to use the CLI functionalities. -
+**Resources** brings the documentation of the different resources and actions
+that can be done with the CLI. - ð§  **Reference** for the API reference and
+internals of the CLI. ## ð What's new For a detailed list of changes, please
+refer to the [CHANGELOG](CHANGELOG.md) file. ## ð¤ Join the community! Join
+the community and help build a safer and transparent AI in our [Discord](https:
+//discord.gg/Kt24CsMb5k)! ## Contributors â¨ Thanks goes to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 [Gonzalo_Mellizo]
  Gonzalo_Mellizo
       ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## License [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `giza_cli-0.0.2/giza/callbacks.py` & `giza_cli-0.2.0/giza/callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         value (bool): represents if the flag has been added or not to the call.
 
     Raises:
         Exit: exit the CLI execution
     """
     if value:
         echo(
-            f"🚀 [orange3]Giza[/orange3] Platform CLI, "
+            f"🚀 [orange3]Giza[/orange3] CLI, "
             f"version ~> [green]{__version__}[/green]",
         )
         raise typer.Exit()
 
 
 def debug_callback(_, value: bool):
     """
```

### Comparing `giza_cli-0.0.2/giza/cli.py` & `giza_cli-0.2.0/giza/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 import click
 import typer
 import typer.rich_utils
 from rich.traceback import install
 
+from giza.commands.models import app as models_app
+from giza.commands.prove import prove
 from giza.commands.transpile import transpile
 from giza.commands.users import app as users_app
 from giza.commands.version import version_entrypoint
 
 install(suppress=[click])
 
 app = typer.Typer(rich_markup_mode="markdown", pretty_exceptions_show_locals=False)
 app.add_typer(
     users_app,
     name="users",
     short_help="💻 Utilities for managing users",
     help="""💻 Utilities for managing users""",
 )
 
+app.add_typer(
+    models_app,
+    name="models",
+    short_help="💻 Utilities for managing models",
+    help="""💻 Utilities for managing models""",
+)
+
 app.callback(
     name="giza",
     help="""
-    🔶 Giza-CLI to manage the resources at Giza Platform 🔶.
+    🔶 Giza-CLI to manage the resources at Giza 🔶.
 """,
 )(version_entrypoint)
 
 
 app.command(
     name="transpile",
-    short_help="🔧 Sends the specified model for transpilation.",
-    help="""🔧 Sends the specified model for transpilation.
+    short_help="🔧 Sends the specified model for transpilation. Shortcut for `giza models transpile`.",
+    help="""🔧 Sends the specified model for transpilation. Shortcut for `giza models transpile`.
 
-    We take the specified ONNX model and send it for transpilation at Giza Platform 🔶
+    We take the specified ONNX model and send it for transpilation at Giza 🔶.
 
     This command can be used multiple times with different models to transpile.
     For transpiling new versions of a model make sure to change the name as of now model names must be unique per user.
+
+    This command will do a couple of things behind the scenes:
+
+        * Create a Model entity
+
+        * Upload the model
+
+        * Update the status of the model
+
+        * Poll the model until the status is either FAILED or COMPLETED
+
+        * If COMPLETED the model is downloaded
+
     """,
 )(transpile)
 
+app.command(name="prove")(prove)
+
 
 def entrypoint():
     app()
```

### Comparing `giza_cli-0.0.2/giza/commands/users.py` & `giza_cli-0.2.0/giza/commands/users.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from giza.schemas import users
 from giza.utils import echo, get_response_info
 
 app = typer.Typer()
 
 
 @app.command(
-    short_help="🔥 Creates a new user in Giza Platform.",
-    help="""🔥 Creates a new user in Giza Platform.
+    short_help="🔥 Creates a new user in Giza.",
+    help="""🔥 Creates a new user in Giza.
 
     This commands ask for a username, password and a valid email address,
     then a confirmation email will be sent to the provided one.
 
     Until the verification is complete the user won't be able to log in nor user other CLI capabilities.
 
     If a username or email is already registered and error will be raised.
@@ -39,15 +39,15 @@
     Raises:
         ValidationError: input fields are validated, if these are not suitable the exception is raised
         HTTPError: request error to the API, 4XX or 5XX
     """
     user = Prompt.ask("Enter your username :sunglasses:")
     password = Prompt.ask("Enter your password 🥷 ", password=True)
     email = Prompt.ask("Enter your email 📧")
-    echo("Creating user in Giza Platform ✅ ")
+    echo("Creating user in Giza ✅ ")
     try:
         user_create = users.UserCreate(
             username=user, password=SecretStr(password), email=EmailStr(email)
         )
         client = UsersClient(API_HOST)
         client.create(user_create)
     except ValidationError as e:
@@ -66,64 +66,64 @@
         if debug:
             raise e
         sys.exit(1)
     echo("User created ✅. Check for a verification email 📧")
 
 
 @app.command(
-    short_help="🔶 Log into Giza Platform.",
-    help="""🔶 Log into Giza Platform.
+    short_help="🔶 Log into Giza.",
+    help="""🔶 Log into Giza.
 
-    Log into Giza Platform using the provided credentials. This will retrieve a JWT
+    Log into Giza using the provided credentials. This will retrieve a JWT
     that will be used to authenticate the user.
 
     This will be saved at `~/.giza/.credentials.json` for later re-use until the token expires.
 
     Verification is needed to log in.
     """,
 )
 def login(
     renew: bool = typer.Option(False, help="Force the renewal of the JWT token"),
     debug: Optional[bool] = DEBUG_OPTION,
 ) -> None:
     """
-    Logs the current user to Giza Platform. Under the hood this will retrieve the token for the next requests.
+    Logs the current user into Giza. Under the hood this will retrieve the token for the next requests.
     This token will be saved at `home` directory for further usage.
 
     Args:
         renew (bool): Force the retrieval of the token to create a new one. Defaults to False.
         debug (Optional[bool]): Whether to add debug information, will show requests, extra logs and traceback if there is an Exception. Defaults to DEBUG_OPTION (False)
 
     Raises:
         HTTPError: request error to the API, 4XX or 5XX
     """
     user = Prompt.ask("Enter your username :sunglasses:")
     password = Prompt.ask("Enter your password 🥷 ", password=True)
 
-    echo("Log into Giza Platform")
+    echo("Log into Giza")
     client = UsersClient(API_HOST, debug=debug)
     try:
         client.retrieve_token(user, password, renew=renew)
     except HTTPError as e:
         info = get_response_info(e.response)
         echo.error("⛔️Could not authorize the user⛔️")
         echo.error(f"⛔️Detail -> {info.get('detail')}⛔️")
         echo.error(f"⛔️Status code -> {info.get('status_code')}⛔️")
         echo.error(f"⛔️Error message -> {info.get('content')}⛔️")
         if debug:
             raise e
         sys.exit(1)
-    echo("Successfully logged into Giza Platform ✅ ")
+    echo("Successfully logged into Giza ✅ ")
 
 
 @app.command(
     short_help="💻 Retrieve information about the current user",
     help="""💻 Retrieve information about the current user.
 
-    Makes an API call to retrieve user current information from Giza Platform.
+    Makes an API call to retrieve user current information from Giza.
 
     Verification and an active token is needed.
     """,
 )
 def me(debug: Optional[bool] = DEBUG_OPTION) -> None:
     """
     Retrieve information about the current user and print it as json to stdout.
```

### Comparing `giza_cli-0.0.2/giza/schemas/users.py` & `giza_cli-0.2.0/giza/schemas/users.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.2/giza/utils/__init__.py` & `giza_cli-0.2.0/giza/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,9 +22,10 @@
         dict: information about the returned response
     """
     try:
         content = response.json()
         detail = content.get("detail")
     except json.JSONDecodeError:
         content = response.text if len(response.text) < 255 else response.text[:255]
+        detail = ""
 
     return {"content": content, "detail": detail, "status_code": response.status_code}
```

### Comparing `giza_cli-0.0.2/giza/utils/decorators.py` & `giza_cli-0.2.0/giza/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.0.2/giza/utils/echo.py` & `giza_cli-0.2.0/giza/utils/echo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime as dt
+from typing import Optional
 
 import typer
 from rich import print as rich_print
 from rich import reconfigure
 
 reconfigure(soft_wrap=True)
 
@@ -10,14 +11,17 @@
 class Echo:
     """
     Helper class to use when printin output of the CLI.
 
     Provides utilities to print different levels of the messages and provides formatting capabilities to each of the levels.
     """
 
+    def __init__(self, debug: Optional[bool] = False) -> None:
+        self._debug = debug
+
     def format_message(
         self, message: str, field: str = "giza", color: str = "orange3"
     ) -> str:
         """
         Format a message with an specific field and color.
         Adds current time, provided field and prints it with the specified color.
 
@@ -89,16 +93,17 @@
     def debug(self, message: str) -> None:
         """
         Format and echo a debug message
 
         Args:
             message (str): debug message to format and echo
         """
-        formatted_message = self.format_debug(message)
-        self.echo(message, formatted_message)
+        if self._debug:
+            formatted_message = self.format_debug(message)
+            self.echo(message, formatted_message)
 
     def info(self, message: str) -> None:
         """
         Format and echo a message
 
         Args:
             message (str): message to format and echo
```

### Comparing `giza_cli-0.0.2/pyproject.toml` & `giza_cli-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "giza-cli"
-version = "0.0.2"
-description = "CLI for interacting with Giza Platform"
+version = "0.2.0"
+description = "CLI for interacting with Giza"
 authors = ["Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
 packages = [{include = "giza"}]
 
 [tool.poetry.scripts]
 giza = "giza.cli:entrypoint"
 
@@ -16,14 +16,16 @@
 click = ">=8.1.0,<9.0.0"
 rich = "12.6.0"
 typer = {version = "0.7.0", extras = ["all"]}
 pydantic = ">=1.10.8,<2.0.0"
 cryptography = ">=41.0.0,<42.0.0"
 python-jose = {version = "^3.3.0", extras = ["cryptography"]}
 email-validator = "^2.0.0.post2"
+types-python-jose = "^3.3.4.8"
+types-requests = "^2.31.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 black = ">=21,<23.3"
 isort = {extras = ["pyproject"], version = "^5.12.0"}
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
```

### Comparing `giza_cli-0.0.2/PKG-INFO` & `giza_cli-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: giza-cli
-Version: 0.0.2
-Summary: CLI for interacting with Giza Platform
+Version: 0.2.0
+Summary: CLI for interacting with Giza
 Author: Gonzalo Mellizo-Soto
 Author-email: gonzalo@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: cryptography (>=41.0.0,<42.0.0)
 Requires-Dist: email-validator (>=2.0.0.post2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: requests (>=2.30.1,<3.0.0)
 Requires-Dist: rich (==12.6.0)
 Requires-Dist: tenacity (>=8.2.2,<=9.0.0)
 Requires-Dist: typer[all] (==0.7.0)
+Requires-Dist: types-python-jose (>=3.3.4.8,<4.0.0.0)
+Requires-Dist: types-requests (>=2.31.0.2,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 # Giza Command Line Interface
 
-![Logo](https://framerusercontent.com/images/dGhFEb4pIwUJ5SArbs7udVlSs.png)
 [![GitHub Workflow Status](https://github.com/gizatechxyz/giza-cli/actions/workflows/onpush.yml/badge.svg)](https://github.com/gizatechxyz/giza-cli/actions/workflows/onpush.yml)
 [![Project license](https://img.shields.io/github/license/gizatechxyz/orion.svg?style=flat-square)](LICENSE)
 [![Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg?style=flat-square)](https://github.com/gizatechxyz/orion/issues?q=is%3Aissue+is%3Aopen)
 [![Join the community](https://dcbadge.vercel.app/api/server/FR3Cd88x6r?style=flat-square)](https://discord.gg/FR3Cd88x6r)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
@@ -35,17 +36,17 @@
 |  |  __  |  | `---/  /     /  ^  \       |  ,----'|  |     |  |
 |  | |_ | |  |    /  /     /  /_\  \      |  |     |  |     |  |
 |  |__| | |  |   /  /----./  _____  \     |  `----.|  `----.|  |
  \______| |__|  /________/__/     \__\     \______||_______||__|
 
 ```
 
-Welcome to Giza`s Platform CLI!
+Welcome to Giza CLI!
 
-This CLI provides the utilities to interact with Giza Platform using the terminal.
+This CLI provides the utilities to interact with Giza using the terminal.
 
 **Discalimer**: this is still in an experimental stage so the functionality is subject to change.
 
 - [Giza Command Line Interface](#giza-command-line-interface)
   - [🚀 Installation](#-installation)
     - [Recomended installation with pipx](#recomended-installation-with-pipx)
     - [Install from PyPi](#install-from-pypi)
@@ -88,15 +89,15 @@
 
 ```bash
   pip install git+ssh://git@github.com/gizatechxyz/giza-cli.git
 ```
 
 ## 📚 Documentation
 
-You can check our official docs [here](https://giza-cli.gizatech.xyz/main).
+You can check our official docs [here](https://orion-giza.gitbook.io/main-1/welcome/readme).
 
 - **Examples** includes examples on how to use the CLI functionalities.
 
 - **Resources** brings the documentation of the different resources and actions that can be done with the CLI.
 
 - 🧠 **Reference** for the API reference and internals of the CLI.
```

