# Comparing `tmp/falcon_toolkit-3.1.2.tar.gz` & `tmp/falcon_toolkit-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_toolkit-3.1.2.tar", max compression
+gzip compressed data, was "falcon_toolkit-3.2.0.tar", max compression
```

## Comparing `falcon_toolkit-3.1.2.tar` & `falcon_toolkit-3.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/LICENSE.md
--rw-r--r--   0        0        0    20600 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/README.md
--rw-r--r--   0        0        0      188 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/__init__.py
--rw-r--r--   0        0        0      174 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/__init__.py
--rw-r--r--   0        0        0     1847 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth.py
--rw-r--r--   0        0        0      191 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/__init__.py
--rw-r--r--   0        0        0      449 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/default.py
--rw-r--r--   0        0        0     6069 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_mssp.py
--rw-r--r--   0        0        0     4087 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_single_cid.py
--rw-r--r--   0        0        0     2709 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/utils.py
--rw-r--r--   0        0        0     1831 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/cli.py
--rw-r--r--   0        0        0     7974 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/config.py
--rw-r--r--   0        0        0      962 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/console_utils.py
--rw-r--r--   0        0        0      385 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/constants.py
--rw-r--r--   0        0        0     2767 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/logging_config.py
--rw-r--r--   0        0        0      340 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/meta.py
--rw-r--r--   0        0        0     1599 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/namespace.py
--rw-r--r--   0        0        0     1944 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/common/utils.py
--rwxr-xr-x   0        0        0     7553 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/falcon.py
--rw-r--r--   0        0        0      116 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/hosts/__init__.py
--rw-r--r--   0        0        0     1016 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/hosts/cli.py
--rw-r--r--   0        0        0      941 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/hosts/host_search.py
--rw-r--r--   0        0        0      120 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/__init__.py
--rw-r--r--   0        0        0     5058 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/cli.py
--rw-r--r--   0        0        0     1049 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/constants.py
--rw-r--r--   0        0        0     3354 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/container.py
--rw-r--r--   0        0        0     3659 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/policies/describe.py
--rw-r--r--   0        0        0      160 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/__init__.py
--rw-r--r--   0        0        0     6397 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cli.py
--rw-r--r--   0        0        0      219 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/__init__.py
--rw-r--r--   0        0        0      335 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/common.py
--rw-r--r--   0        0        0     2583 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/reg.py
--rw-r--r--   0        0        0    18855 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/parsers.py
--rw-r--r--   0        0        0    40348 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/prompt.py
--rw-r--r--   0        0        0     1880 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/refresh.py
--rw-r--r--   0        0        0      681 2023-04-27 18:21:51.775285 falcon_toolkit-3.1.2/falcon_toolkit/shell/utils.py
--rw-r--r--   0        0        0     2075 2023-04-27 18:21:51.779285 falcon_toolkit-3.1.2/pyproject.toml
--rw-r--r--   0        0        0    22027 1970-01-01 00:00:00.000000 falcon_toolkit-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/LICENSE.md
+-rw-r--r--   0        0        0    20636 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/README.md
+-rw-r--r--   0        0        0      188 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/__init__.py
+-rw-r--r--   0        0        0      174 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/__init__.py
+-rw-r--r--   0        0        0     1847 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/auth.py
+-rw-r--r--   0        0        0      191 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/__init__.py
+-rw-r--r--   0        0        0      449 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/default.py
+-rw-r--r--   0        0        0     6254 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/public_mssp.py
+-rw-r--r--   0        0        0     4087 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/public_single_cid.py
+-rw-r--r--   0        0        0     2709 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/utils.py
+-rw-r--r--   0        0        0     1831 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/cli.py
+-rw-r--r--   0        0        0     7974 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/config.py
+-rw-r--r--   0        0        0      962 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/console_utils.py
+-rw-r--r--   0        0        0      550 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/constants.py
+-rw-r--r--   0        0        0     2767 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/logging_config.py
+-rw-r--r--   0        0        0      340 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/meta.py
+-rw-r--r--   0        0        0     1599 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/namespace.py
+-rw-r--r--   0        0        0     1944 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/common/utils.py
+-rwxr-xr-x   0        0        0     9943 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/falcon.py
+-rw-r--r--   0        0        0      116 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/hosts/__init__.py
+-rw-r--r--   0        0        0     1304 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/hosts/cli.py
+-rw-r--r--   0        0        0     1030 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/hosts/host_search.py
+-rw-r--r--   0        0        0      120 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/policies/__init__.py
+-rw-r--r--   0        0        0     5058 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/policies/cli.py
+-rw-r--r--   0        0        0     1049 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/policies/constants.py
+-rw-r--r--   0        0        0     3354 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/policies/container.py
+-rw-r--r--   0        0        0     3659 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/policies/describe.py
+-rw-r--r--   0        0        0      160 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/shell/__init__.py
+-rw-r--r--   0        0        0     6967 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/shell/cli.py
+-rw-r--r--   0        0        0      219 2023-08-04 21:41:29.629685 falcon_toolkit-3.2.0/falcon_toolkit/shell/cmd_generators/__init__.py
+-rw-r--r--   0        0        0      335 2023-08-04 21:41:29.633685 falcon_toolkit-3.2.0/falcon_toolkit/shell/cmd_generators/common.py
+-rw-r--r--   0        0        0     2583 2023-08-04 21:41:29.633685 falcon_toolkit-3.2.0/falcon_toolkit/shell/cmd_generators/reg.py
+-rw-r--r--   0        0        0    18855 2023-08-04 21:41:29.633685 falcon_toolkit-3.2.0/falcon_toolkit/shell/parsers.py
+-rw-r--r--   0        0        0    40348 2023-08-04 21:41:29.633685 falcon_toolkit-3.2.0/falcon_toolkit/shell/prompt.py
+-rw-r--r--   0        0        0     1880 2023-08-04 21:41:29.633685 falcon_toolkit-3.2.0/falcon_toolkit/shell/refresh.py
+-rw-r--r--   0        0        0      681 2023-08-04 21:41:29.633685 falcon_toolkit-3.2.0/falcon_toolkit/shell/utils.py
+-rw-r--r--   0        0        0     2150 2023-08-04 21:41:29.633685 falcon_toolkit-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    22108 1970-01-01 00:00:00.000000 falcon_toolkit-3.2.0/PKG-INFO
```

### Comparing `falcon_toolkit-3.1.2/LICENSE.md` & `falcon_toolkit-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/README.md` & `falcon_toolkit-3.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!--markdownlint-disable MD033-->
 # Falcon Toolkit
 
 ![CrowdStrike Falcon](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png)
 
 [![Twitter URL](https://img.shields.io/twitter/url?label=Follow%20%40CrowdStrike&style=social&url=https%3A%2F%2Ftwitter.com%2FCrowdStrike)](https://twitter.com/CrowdStrike)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/CrowdStrike/Falcon-Toolkit/Publish%20Python%20Package?label=build%20and%20deploy)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/CrowdStrike/Falcon-Toolkit/release-deploy.yml?label=build%20and%20deploy)
 [![PyPI](https://img.shields.io/pypi/v/Falcon-Toolkit)](https://pypi.org/project/Falcon-Toolkit)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Falcon-Toolkit)
 ![OSS Lifecycle](https://img.shields.io/osslifecycle/CrowdStrike/Falcon-Toolkit)
 
 ***automate all the things...remotely!***
 
 ## What Is This?
@@ -229,30 +229,30 @@
 
 ## Host Search
 
 Before jumping into an RTR shell, you may wish to see which hosts you would connect to if you used the `shell` command (covered below). To do so, use the `falcon host_search` command.
 
 As with the `shell` command, you must specify a profile (the name of a configuration you created using the `new` command above) if you have created more than one, and you can then optionally provide as many filters as you want using succesive `-f` switches. Some examples:
 
-List all Windows hosts that are not within the `London` site, within the one Falcon instance configured earlier.
+List all online Windows hosts that are not within the `London` site, within the one Falcon instance configured earlier.
 
 ```shell
-falcon host_search -f OS=Windows -f Site__NOT=London
+falcon host_search -f OS=Windows -f Site__NOT=London -o online
 ```
 
-List all Windows hosts not within the `075e03f5e5c04d83b4831374e7dc01c3` Group, wihtin the `MyCompany` Falcon tenant.
+List all Windows hosts not within the `075e03f5e5c04d83b4831374e7dc01c3` Group, within the `MyCompany` Falcon tenant.
 
 ```shell
 falcon -p MyCompany host_search -f OS=Windows -f GroupID__NOT=075e03f5e5c04d83b4831374e7dc01c3
 ```
 
-List all `MyOtherCompany` Windows servers or domain controllers not within an OU called `Protected`
+List all offline `MyOtherCompany` Windows servers or domain controllers not within an OU called `Protected`
 
 ```shell
-falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Server,DC -f OU__NOT=Protected
+falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Server,DC -f OU__NOT=Protected -o offline
 ```
 
 List all `MyOtherCompany` Windows Workstations that have checked in to Falcon within the past 30 minutes
 
 ```shell
 falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Workstation -f LastSeen__GTE=-30m
 ```
```

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/auth.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/auth.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_mssp.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/public_mssp.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     description = (
         "A Falcon Flight Control (MSSP) Falcon tenant with multiple child Customer IDs (CIDs). "
         "These tenants are used in cases where a customer has multiple subsidiaries under central "
         "management, or where many customers have outsouced their Falcon management to a third "
         "party. This option is compatible with all of CrowdStrike's public cloud environments. "
         "For EU-1, US-1 and US-2, only a Client ID and Client Secret are required. For US "
         "GovCloud, set the Cloud Name to usgov1 within the additional options. "
+        "This option should be used only when you are connecting to a Parent CID; if you only have "
+        "keys for a child CID, use the Single CID authentication backend instead. "
         "NOTE: Each time you connect to a Flight Control CID you will be prompted on screen to "
         "choose a child CID to connect to. To skip this, set the environment variable "
         "FALCON_MSSP_CHILD_CID to the CID you want to connect to."
     )
 
     def __init__(self, config: Dict = None):
         """Retrieve the details needed to configure FalconPy from the user."""
```

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/public_single_cid.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/public_single_cid.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/auth_backends/utils.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/auth_backends/utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/cli.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/config.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/config.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/console_utils.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/console_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/logging_config.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/logging_config.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/namespace.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/namespace.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/common/utils.py` & `falcon_toolkit-3.2.0/falcon_toolkit/common/utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/falcon.py` & `falcon_toolkit-3.2.0/falcon_toolkit/falcon.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,30 +23,35 @@
 - Loads a configuration JSON file from disk
 - Configures a passable context dictionary (ctx.obj) that can be loaded and used by each
     Click CLI command, as needed
 - Configures a global logger
 """
 import logging
 import os
+import shutil
+import sys
 
 import click
+import pick
 
 from caracara.filters.fql import FalconFilterAttribute
 from caracara.modules.hosts import FILTER_ATTRIBUTES as HOSTS_FILTER_ATTRIBUTES
 from colorama import (
     deinit as colorama_deinit,
     init as colorama_init,
 )
 
 from falcon_toolkit.common.config import FalconToolkitConfig
+from falcon_toolkit.common.console_utils import build_file_hyperlink
 from falcon_toolkit.common.constants import (
+    CONFIG_FILENAME,
     DEFAULT_CONFIG_DIR,
     LOG_SUB_DIR,
+    OLD_DEFAULT_CONFIG_DIR,
 )
-from falcon_toolkit.common.console_utils import build_file_hyperlink
 from falcon_toolkit.common.logging_config import configure_logger
 from falcon_toolkit.common.utils import configure_data_dir
 from falcon_toolkit.hosts.cli import cli_host_search
 from falcon_toolkit.policies.cli import cli_policies
 from falcon_toolkit.shell.cli import cli_shell
 
 
@@ -54,15 +59,15 @@
 @click.pass_context
 @click.option(
     '-c',
     '--config-path',
     envvar='FALCON_TOOLKIT_CONFIG_DIR',
     type=click.STRING,
     default=DEFAULT_CONFIG_DIR,
-    help="Path to the configuration directory (default: ~/.FalconToolkit/)",
+    help="Path to the configuration directory (default: %userappdata%/FalconToolkit/)",
 )
 @click.option(
     '-v',
     '--verbose',
     envvar='FALCON_TOOLKIT_VERBOSE',
     type=click.BOOL,
     is_flag=True,
@@ -114,22 +119,81 @@
     """
     # Enable colorama across the board
     colorama_init(autoreset=True)
 
     # Configure context that can be passed down to other options
     ctx.ensure_object(dict)
     click.echo(click.style("Falcon Toolkit", fg='blue', bold=True))
-    config_path = os.path.expanduser(config_path)
     hyperlink = build_file_hyperlink(config_path, config_path, "falcon_config_path")
     click.echo(click.style(f"Configuration Directory: {hyperlink}", fg='black'))
     if verbose:
         log_level = logging.INFO
     else:
         log_level = logging.CRITICAL
 
+    if (
+        config_path == DEFAULT_CONFIG_DIR and
+        os.path.exists(OLD_DEFAULT_CONFIG_DIR) and
+        not os.path.exists(config_path)
+    ):
+        # The user has used Falcon Toolkit before, and uses the default directory, so we
+        # offer to move the configuration folder for them.
+        choice, _ = pick.pick(
+            options=[
+                pick.Option(
+                    f"Please move my current folder contents to {config_path}",
+                    "MOVE_FOLDER",
+                ),
+                pick.Option(
+                    (
+                        f"Leave my old folder ({OLD_DEFAULT_CONFIG_DIR}) alone "
+                        f"and create a new one at {config_path}"
+                    ),
+                    "LEAVE_ALONE",
+                ),
+                pick.Option(
+                    (
+                        f"Leave my old folder ({OLD_DEFAULT_CONFIG_DIR}) alone, "
+                        f"create a new one at {config_path}, and copy my configuration "
+                        "file there."
+                    ),
+                    "COPY_CONFIG_ONLY",
+                ),
+                pick.Option(
+                    "Exit Falcon Toolkit and do nothing",
+                    "ABORT",
+                ),
+            ],
+            title=(
+                "As of Falcon Toolkit 3.3.0, the configuration directory has moved to a "
+                "platform-specific data configuration directory."
+            )
+        )
+
+        if choice.value == "MOVE_FOLDER":
+            click.echo(f"Moving {OLD_DEFAULT_CONFIG_DIR} to {config_path}")
+            os.rename(OLD_DEFAULT_CONFIG_DIR, config_path)
+        elif choice.value == "LEAVE_ALONE":
+            click.echo(
+                f"Creating a new, empty data directory at {config_path} "
+                "and leaving the original folder alone"
+            )
+        elif choice.value == "COPY_CONFIG_ONLY":
+            click.echo(
+                f"Creating a new, empty data directory at {config_path} "
+                "and copying the current configuration there"
+            )
+            os.mkdir(config_path)
+            shutil.copyfile(
+                os.path.join(OLD_DEFAULT_CONFIG_DIR, CONFIG_FILENAME),
+                os.path.join(config_path, CONFIG_FILENAME),
+            )
+        else:
+            sys.exit(1)
+
     # Configure and load the configuration object
     configure_data_dir(config_path)
     config = FalconToolkitConfig(config_path=config_path)
     ctx.obj['config'] = config
 
     # Configure the logger
     log_path = os.path.join(config_path, LOG_SUB_DIR)
```

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/hosts/cli.py` & `falcon_toolkit-3.2.0/falcon_toolkit/hosts/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 of the logic itself is contained in host_search.py
 """
 
 from typing import List
 
 import click
 
+from caracara.common.constants import OnlineState
+
 from falcon_toolkit.common.cli import (
     get_instance,
     parse_cli_filters,
 )
 from falcon_toolkit.hosts.host_search import host_search_cmd
 
 
@@ -25,17 +27,27 @@
     '--filter',
     'filter_kv_strings',
     type=click.STRING,
     multiple=True,
     required=False,
     help="Filter hosts to search based on standard Falcon filters",
 )
+@click.option(
+    '-o',
+    '--online_state',
+    'online_state',
+    type=click.Choice(OnlineState.VALUES),
+    multiple=False,
+    required=False,
+    help="Filter hosts by online state",
+)
 def cli_host_search(
     ctx: click.Context,
     filter_kv_strings: List[str],
+    online_state: str = None,
 ):
     """Implement the host_search CLI command."""
     instance = get_instance(ctx)
     client = instance.auth_backend.authenticate()
     filters = parse_cli_filters(filter_kv_strings, client)
 
-    host_search_cmd(client, filters)
+    host_search_cmd(client, filters, online_state)
```

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/hosts/host_search.py` & `falcon_toolkit-3.2.0/falcon_toolkit/hosts/host_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 
 This functionality allows users to search for hosts without connecting to them.
 Once a set of filters has been decided upon, swapping 'host_search' for 'shell' at the CLI will
 launch a batch RTR shell with these systems.
 """
 import logging
 
+from typing import Optional
+
 import click
 import click_spinner
 
 from caracara import Client
 from caracara.filters import FalconFilter
 
 
 def host_search_cmd(
     client: Client,
     filters: FalconFilter,
+    online_state: Optional[str],
 ):
     """Search for hosts that match the provided filters."""
     click.echo(click.style("Searching for hosts...", fg='magenta'))
 
     fql = filters.get_fql()
 
     with click_spinner.spinner():
-        host_data = client.hosts.describe_devices(filters=fql)
+        host_data = client.hosts.describe_devices(filters=fql, online_state=online_state)
 
     logging.debug(host_data)
     for aid in host_data.keys():
         hostname = host_data[aid].get("hostname", "<NO HOSTNAME>")
         click.echo(click.style(f"{hostname:16s}", fg='green'), nl=False)
         click.echo(f"- {aid}")
```

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/policies/cli.py` & `falcon_toolkit-3.2.0/falcon_toolkit/policies/cli.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/policies/constants.py` & `falcon_toolkit-3.2.0/falcon_toolkit/policies/constants.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/policies/container.py` & `falcon_toolkit-3.2.0/falcon_toolkit/policies/container.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/policies/describe.py` & `falcon_toolkit-3.2.0/falcon_toolkit/policies/describe.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/shell/cli.py` & `falcon_toolkit-3.2.0/falcon_toolkit/shell/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import click
 
 from click_option_group import (
     optgroup,
     MutuallyExclusiveOptionGroup,
 )
 
+from caracara.common.constants import OnlineState
+
 from falcon_toolkit.common.cli import (
     get_instance,
     parse_cli_filters,
 )
 from falcon_toolkit.shell.prompt import RTRPrompt
 
 
@@ -117,43 +119,50 @@
 
     Once we have all the required information together, we configure an RTRPrompt object then
     start the REPL command loop. This passes control over to the shell, via the Cmd2 library.
     """
     instance = get_instance(ctx)
     client = instance.auth_backend.authenticate()
 
+    # Show online hosts only if queueing is false
+    online_state = None if queueing else OnlineState.ONLINE
+    online_string = "" if queueing else "online "
+
     if filter_kv_strings:
         click.echo(click.style(
             "Connecting to all hosts that match the provided Falcon filters",
             fg='magenta',
             bold=True,
         ))
         logging.info("Connecting to all hosts that match the provided Falcon filters")
 
         filters = parse_cli_filters(filter_kv_strings, client).get_fql()
         click.echo(click.style("FQL filter string: ", bold=True), nl=False)
         click.echo(filters)
         logging.info(filters)
 
-        device_ids = client.hosts.get_device_ids(filters=filters)
+        device_ids = client.hosts.get_device_ids(filters=filters, online_state=online_state)
     elif device_id_list:
         click.echo(click.style(
             "Connecting to the device IDs provided on the command line",
             fg='magenta',
             bold=True,
         ))
         logging.info("Connecting to the device IDs provided on the command line")
 
         device_ids = set()
         for device_id in device_id_list.split(","):
             device_id = device_id.strip()
             if device_id:
                 device_ids.add(device_id)
 
-        device_ids = list(device_ids)
+        device_ids = client.hosts.filter_by_online_state(
+            list(device_ids),
+            online_state=online_state,
+        )
     elif device_id_file:
         click.echo(click.style(
             "Connecting to the device IDs listed in a file",
             fg='magenta',
             bold=True,
         ))
         click.echo(click.style("File path: ", bold=True), nl=False)
@@ -162,25 +171,32 @@
 
         with open(device_id_file, 'rt', encoding='ascii') as device_id_file_handle:
             device_ids = set()
             for line in device_id_file_handle:
                 line = line.strip()
                 if line:
                     device_ids.add(line)
-            device_ids = list(device_ids)
+            device_ids = client.hosts.filter_by_online_state(
+                list(device_ids),
+                online_state=online_state,
+            )
     else:
         click.echo(click.style(
-            "WARNING: Connecting to all hosts in the Falcon instance",
+            f"WARNING: Connecting to all {online_string}hosts in the Falcon instance",
             fg='yellow',
         ))
-        logging.info("Connecting to all hosts in the Falcon instance")
-        device_ids = client.hosts.get_device_ids()
+        logging.info("Connecting to all %shosts in the Falcon instance", online_string)
+        device_ids = client.hosts.get_device_ids(online_state=online_state)
 
     if not device_ids:
-        click.echo(click.style("No devices match the provided filters", fg='red', bold=True))
+        click.echo(click.style(
+            f"No {online_string}devices match the provided filters",
+            fg='red',
+            bold=True,
+        ))
         sys.exit(1)
 
     device_count = len(device_ids)
     click.echo(click.style(f"Connecting to {device_count} device(s)", bold=True))
     logging.info("Connecting to %d device(s)", device_count)
     logging.debug(device_ids)
```

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/shell/cmd_generators/reg.py` & `falcon_toolkit-3.2.0/falcon_toolkit/shell/cmd_generators/reg.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/shell/parsers.py` & `falcon_toolkit-3.2.0/falcon_toolkit/shell/parsers.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/shell/prompt.py` & `falcon_toolkit-3.2.0/falcon_toolkit/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/shell/refresh.py` & `falcon_toolkit-3.2.0/falcon_toolkit/shell/refresh.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/falcon_toolkit/shell/utils.py` & `falcon_toolkit-3.2.0/falcon_toolkit/shell/utils.py`

 * *Files identical despite different names*

### Comparing `falcon_toolkit-3.1.2/pyproject.toml` & `falcon_toolkit-3.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "falcon-toolkit"
-version = "3.1.2"
+version = "3.2.0"
 description = "Toolkit to interface with CrowdStrike Falcon via the API"
 license = "MIT"
 authors = [
     "Chris Hammond <chris.hammond@crowdstrike.com>",
+    "Kira Noël <kira.noel@crowdstrike.com>",
 ]
 repository = "http://github.com/CrowdStrike/Falcon-Toolkit"
 readme = "README.md"
 keywords = [
     "automation",
     "cli",
     "crowdstrike",
@@ -25,22 +26,23 @@
     "Topic :: Security",
     "Topic :: System :: Shells",
     "Topic :: Terminals",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-caracara = "^0.2.2"
+caracara = "^0.3.0"
 click = "^8.1.3"
 click-option-group = "^0.5.3"
 click-spinner = "^0.1.10"
 cmd2 = "^2.4"
 colorama = "^0.4.5"
-keyring = "^23"
+keyring = ">=23,<25"
 pick = "^2.0.2"
+platformdirs = "^3.5.1"
 tabulate = "^0.9.0"
 
 [tool.poetry.scripts]
 falcon = "falcon_toolkit.falcon:cli"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `falcon_toolkit-3.1.2/PKG-INFO` & `falcon_toolkit-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-toolkit
-Version: 3.1.2
+Version: 3.2.0
 Summary: Toolkit to interface with CrowdStrike Falcon via the API
 Home-page: http://github.com/CrowdStrike/Falcon-Toolkit
 License: MIT
 Keywords: automation,cli,crowdstrike,endpoint-protection,falcon,falcon-platform
 Author: Chris Hammond
 Author-email: chris.hammond@crowdstrike.com
 Requires-Python: >=3.9,<4.0
@@ -17,33 +17,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
-Requires-Dist: caracara (>=0.2.2,<0.3.0)
+Requires-Dist: caracara (>=0.3.0,<0.4.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.3,<0.6.0)
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0)
 Requires-Dist: cmd2 (>=2.4,<3.0)
 Requires-Dist: colorama (>=0.4.5,<0.5.0)
-Requires-Dist: keyring (>=23,<24)
+Requires-Dist: keyring (>=23,<25)
 Requires-Dist: pick (>=2.0.2,<3.0.0)
+Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, http://github.com/CrowdStrike/Falcon-Toolkit
 Description-Content-Type: text/markdown
 
 <!--markdownlint-disable MD033-->
 # Falcon Toolkit
 
 ![CrowdStrike Falcon](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png)
 
 [![Twitter URL](https://img.shields.io/twitter/url?label=Follow%20%40CrowdStrike&style=social&url=https%3A%2F%2Ftwitter.com%2FCrowdStrike)](https://twitter.com/CrowdStrike)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/CrowdStrike/Falcon-Toolkit/Publish%20Python%20Package?label=build%20and%20deploy)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/CrowdStrike/Falcon-Toolkit/release-deploy.yml?label=build%20and%20deploy)
 [![PyPI](https://img.shields.io/pypi/v/Falcon-Toolkit)](https://pypi.org/project/Falcon-Toolkit)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Falcon-Toolkit)
 ![OSS Lifecycle](https://img.shields.io/osslifecycle/CrowdStrike/Falcon-Toolkit)
 
 ***automate all the things...remotely!***
 
 ## What Is This?
@@ -264,30 +265,30 @@
 
 ## Host Search
 
 Before jumping into an RTR shell, you may wish to see which hosts you would connect to if you used the `shell` command (covered below). To do so, use the `falcon host_search` command.
 
 As with the `shell` command, you must specify a profile (the name of a configuration you created using the `new` command above) if you have created more than one, and you can then optionally provide as many filters as you want using succesive `-f` switches. Some examples:
 
-List all Windows hosts that are not within the `London` site, within the one Falcon instance configured earlier.
+List all online Windows hosts that are not within the `London` site, within the one Falcon instance configured earlier.
 
 ```shell
-falcon host_search -f OS=Windows -f Site__NOT=London
+falcon host_search -f OS=Windows -f Site__NOT=London -o online
 ```
 
-List all Windows hosts not within the `075e03f5e5c04d83b4831374e7dc01c3` Group, wihtin the `MyCompany` Falcon tenant.
+List all Windows hosts not within the `075e03f5e5c04d83b4831374e7dc01c3` Group, within the `MyCompany` Falcon tenant.
 
 ```shell
 falcon -p MyCompany host_search -f OS=Windows -f GroupID__NOT=075e03f5e5c04d83b4831374e7dc01c3
 ```
 
-List all `MyOtherCompany` Windows servers or domain controllers not within an OU called `Protected`
+List all offline `MyOtherCompany` Windows servers or domain controllers not within an OU called `Protected`
 
 ```shell
-falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Server,DC -f OU__NOT=Protected
+falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Server,DC -f OU__NOT=Protected -o offline
 ```
 
 List all `MyOtherCompany` Windows Workstations that have checked in to Falcon within the past 30 minutes
 
 ```shell
 falcon -p MyOtherCompany host_search -f OS=Windows -f Role=Workstation -f LastSeen__GTE=-30m
 ```
```

