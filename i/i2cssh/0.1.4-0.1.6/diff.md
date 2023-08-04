# Comparing `tmp/i2cssh-0.1.4.tar.gz` & `tmp/i2cssh-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cssh-0.1.4.tar", last modified: Wed Aug  2 15:56:36 2023, max compression
+gzip compressed data, was "i2cssh-0.1.6.tar", last modified: Fri Aug  4 08:36:31 2023, max compression
```

## Comparing `i2cssh-0.1.4.tar` & `i2cssh-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.379549 i2cssh-0.1.4/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.4/LICENSE.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.4/MANIFEST.in
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 15:56:36.378903 i2cssh-0.1.4/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.4/README.md
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 15:56:36.379821 i2cssh-0.1.4/setup.cfg
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1067 2023-08-02 13:38:22.000000 i2cssh-0.1.4/setup.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.341690 i2cssh-0.1.4/src/
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.355706 i2cssh-0.1.4/src/i2cssh/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.4/src/i2cssh/__init__.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24522 2023-08-02 15:54:34.000000 i2cssh-0.1.4/src/i2cssh/lib.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.4/src/i2cssh/main.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.377318 i2cssh-0.1.4/src/i2cssh/tests/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.4/src/i2cssh/tests/__init__.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    28775 2023-08-02 15:52:34.000000 i2cssh-0.1.4/src/i2cssh/tests/test_i2cssh.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 15:55:18.000000 i2cssh-0.1.4/src/i2cssh/version.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.371754 i2cssh-0.1.4/src/i2cssh.egg-info/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      391 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/SOURCES.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/dependency_links.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       37 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/entry_points.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/requires.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/top_level.txt
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.495392 i2cssh-0.1.6/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.6/LICENSE.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.6/MANIFEST.in
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-04 08:36:31.494830 i2cssh-0.1.6/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.6/README.md
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-04 08:36:31.495543 i2cssh-0.1.6/setup.cfg
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1074 2023-08-04 08:34:51.000000 i2cssh-0.1.6/setup.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.475824 i2cssh-0.1.6/src/
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.485187 i2cssh-0.1.6/src/i2cssh/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.6/src/i2cssh/__init__.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24432 2023-08-03 23:27:54.000000 i2cssh-0.1.6/src/i2cssh/lib.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.6/src/i2cssh/main.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.493249 i2cssh-0.1.6/src/i2cssh/tests/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.6/src/i2cssh/tests/__init__.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    36373 2023-08-04 00:04:47.000000 i2cssh-0.1.6/src/i2cssh/tests/test_i2cssh.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-04 08:35:38.000000 i2cssh-0.1.6/src/i2cssh/version.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.491399 i2cssh-0.1.6/src/i2cssh.egg-info/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      391 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/SOURCES.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/dependency_links.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       44 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/entry_points.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/requires.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/top_level.txt
```

### Comparing `i2cssh-0.1.4/LICENSE.txt` & `i2cssh-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.4/PKG-INFO` & `i2cssh-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.4
+Version: 0.1.6
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

### Comparing `i2cssh-0.1.4/README.md` & `i2cssh-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.4/setup.py` & `i2cssh-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup(
     name="i2cssh",
     version=version(),
     author="Wouter de Bie",
     author_email="wouter@evenflow.nl",
     description="csshX like ssh tool for iTerm2",
     url="http://github.com/wouterdebie/i2cssh",
-    entry_points={"console_scripts": ["i2cssh=main:main"]},
+    entry_points={"console_scripts": ["i2cssh=i2cssh.main:main"]},
     license="MIT",
     keywords="ssh i2cssh csshX".split(),
     classifiers=[
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

### Comparing `i2cssh-0.1.4/src/i2cssh/lib.py` & `i2cssh-0.1.6/src/i2cssh/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from click_option_group import MutuallyExclusiveOptionGroup, optgroup
 from iterm2 import Session
 from iterm2.color import Color
 from iterm2.profile import LocalWriteOnlyProfile
 
 from i2cssh.version import version
 
+EXIT_CODE_NO_HOSTS = 255
+EXIT_CODE_UNKNOWN_CLUSTER = 254
+EXIT_CODE_NO_CURRENT_WINDOW = 253
+EXIT_CODE_INVALID_YAML = 252
+
 
 @click.command()
 @optgroup.group("General options")
 @optgroup.option(
     "--clusters",
     "-c",
     "cli_clusters",
@@ -143,16 +148,15 @@
     type=int,
     help="Number of rows (columns will be calculated)",
 )
 @optgroup.option(
     "--direction",
     "-d",
     multiple=False,
-    default="default",
-    type=click.Choice(["column", "row", "default"], case_sensitive=False),
+    type=click.Choice(["column", "row"], case_sensitive=False),
     help="Direction that new sessions are created (default: column)",
 )
 @click.argument(
     "hosts_or_cluster",
     nargs=-1,
 )
 def app(hosts_or_cluster, *_args, **cmdline_opts):
@@ -169,25 +173,19 @@
     valid_options = list(cmdline_opts.keys())
 
     # Load config file and get valid options. Since command line options take precedence, we
     # override the config file options with the command line options.
     config = read_config()
     if config:
         global_opts = filter_valid_options(config, valid_options)
-        # apply_opts(global_options_from_config, opts, valid_options)
-        # opts = global_options_from_config
 
     # Because we can split tabs based on cluster/hosts/arguments we first
     # create different groups inside the hosts list. If it turns out we
     # don't need to split tabs, we'll just have one group by flattening
-    # the list.
-
-    # List where we initially store the groups of hosts. Later we'll use these to apply options from
-    # different configuration places (cluster, global, command line), creating config_groups.
-    # Hosts are dictionaries with all the options necessary to spawn the SSH session
+    # the list. Hosts are dictionaries with all the options necessary to spawn the SSH session
     groups = []
 
     # If there's only one argument, we assume it's a cluster name (since there's
     # no need to use i2cssh for a single host) and we get hosts from the cluster
     # configuration. Otherwise we construct a list of hosts from the arguments.
     if len(hosts_or_cluster) == 1:
         # Single cluster, so we know there's only one list returned
@@ -226,20 +224,14 @@
                 groups.append(get_hosts([m]))
         else:
             groups.append(get_hosts(cmdline_opts.get("machines").split(",")))
 
     if filename := cmdline_opts.get("file"):
         groups.append(get_hosts(get_host_strs_from_file(filename)))
 
-    # Direction is a special case, since it has a default value in the command line options.
-    # In case it's default on the command line, we can assume wasn't set on the command line
-    # and we can delete it from the command opts alltogether. This way we can still use the
-    if cmdline_opts.get("direction") == "default":
-        cmdline_opts.pop("direction")
-
     # Each host might have additional options based on cluster config
     # or login@host syntax. We need to merge those options with the
     # global options specified in the config file and on the command line.
     #
     # Precedence is: global config < cluster config < host config < command line,
     # so we need to apply the options in that order.
 
@@ -248,16 +240,15 @@
             # Save login in order to apply it later
             login = host.get("login")
 
             if config:
                 apply_opts(host, global_opts, valid_options)
 
             # Apply cluster options from config file
-            cluster_options = host["cluster_options"]
-            apply_opts(host, cluster_options, valid_options)
+            apply_opts(host, host["cluster_options"], valid_options)
             host.pop("cluster_options")
 
             # Apply login from host config we saved it
             if login:
                 host["login"] = login
 
             # Apply options from command line
@@ -273,15 +264,15 @@
         or global_opts.get("tab_split_nogroup")
     ):
         groups = [flatten(groups)]
 
     # Bail if we don't have any hosts
     if len(flatten(groups)) == 0:
         click.echo("No hosts found")
-        sys.exit(1)
+        sys.exit(EXIT_CODE_NO_HOSTS)
 
     # Attach a geometry and group options to each group. Here we take options the first host, since
     # we assume that all hosts in a group have the same group options. Also, we set a few defaults.
     groups = [
         {
             "hosts": hosts,
             "geometry": compute_geometry(
@@ -305,14 +296,18 @@
     Execute the SSH sessions in iTerm2
     This function takes in groups of hosts and global options and returns an
     async function that will be executed by iTerm2
     """
 
     async def inner(connection):
         window = await get_window(connection)
+        # Bail if we're not inside iterm
+        if window is None:
+            click.echo("No current window")
+            sys.exit(EXIT_CODE_NO_CURRENT_WINDOW)
 
         # Keep track of broadcast domains. This is later used to tell iTerm2 which tabs need to
         # have keyboard broadcasting enabled.
         broadcast_domains = []
 
         for i, group in enumerate(groups):
             profile_name = group.get("profile")
@@ -446,62 +441,67 @@
         # Enable broadcast input for all groups that require it
         await enable_broadcast(connection, broadcast_domains)
 
     return inner
 
 
 async def split_pane(profile_name, lwop, vertical, pane):
+    """Split a pane vertically or horizontally, depending on the vertical parameter"""
     pane = await pane.async_split_pane(
         vertical, profile_customizations=lwop, profile=profile_name
     )
     return pane
 
 
 def create_lwop(shell):
+    """Create a LocalWriteOnlyProfile that sets the shell to be used for the session"""
     lwop = LocalWriteOnlyProfile()
     lwop.set_use_custom_command("Yes")
     lwop.set_command(f"{shell}\n")
     return lwop
 
 
 async def sleep(s):
+    """Sleep for s seconds"""
     await asyncio.sleep(s)
 
 
 async def set_fullscreen(window):
+    """Set the window to fullscreen"""
     await window.async_set_fullscreen(True)
 
 
 async def get_window(connection):
+    """Get the current window"""
     # Setup iterm API connection
     app = await iterm2.async_get_app(connection)
     window = app.current_window
 
-    # Bail if we're not inside iterm
-    if window is None:
-        click.echo("No current window")
-        sys.exit(1)
     return window
 
 
 async def create_window(connection, window, profile_name, lwop):
+    """Create a new window"""
     return await window.async_create(
         connection, profile_name, profile_customizations=lwop
     )
 
 
 async def create_tab(window, profile_name, lwop):
+    """Create a new tab in the given window"""
     await window.async_create_tab(profile_name, profile_customizations=lwop)
 
 
 async def execute_command(pane, cmd):
+    """Executes a command in a pane"""
     await pane.async_send_text(cmd)
 
 
 async def create_unused_pane(pane):
+    """Creates an UNUSED pane"""
     profile = await pane.async_get_profile()
     await pane.async_send_text(f"unset HISTFILE\n")
     await asyncio.sleep(0.3)
     await profile.async_set_foreground_color(Color.from_hex("#ff0000"))
     crs = "\n" * 100
     await pane.async_send_text(
         f"stty -isig -icanon -echo && echo -e '{crs}UNUSED' && cat > /dev/null\n"
@@ -616,15 +616,20 @@
     Get hosts from a list of cluster names. Note that this returns
     a list of lists of hosts; one list per cluster.
 
     This function doesn't only create hosts from the cluster, but also applies
     the options from the cluster to the hosts.
     """
     clusters = []
+
     for cluster_name in cluster_names:
+        if cluster_name not in config["clusters"]:
+            click.echo(f"Cluster {cluster_name} not found")
+            sys.exit(EXIT_CODE_UNKNOWN_CLUSTER)
+
         host_strings = config["clusters"][cluster_name].get("hosts", [])
         cluster_options = filter_valid_options(
             config["clusters"][cluster_name], valid_options
         )
 
         # Include hosts from other clusters if specified. Note that
         # the cluster options from the included cluster are ignored.
@@ -652,23 +657,18 @@
         hosts.append(host)
     return hosts
 
 
 def apply_opts(target, overrides, valid_options):
     """
     Apply options from the config file and command line.
-    This function will recursively apply options to nested lists.
     """
-    if isinstance(target, list):
-        for host in target:
-            apply_opts(host, overrides, valid_options)
-    else:
-        for key in valid_options:
-            if key in overrides and overrides[key] not in (None, ()):
-                target[key] = overrides[key]
+    for key in valid_options:
+        if key in overrides and overrides[key] not in (None, ()):
+            target[key] = overrides[key]
 
 
 def parse_hostname(hostname):
     """Parse a [login@]hostname and return a tuple of (login, host)"""
     login = None
     host = hostname
     if "@" in hostname:
@@ -695,13 +695,15 @@
 
     # See if there's a config file and read from this first
     if os.path.isfile(config_file):
         with open(config_file, "r") as stream:
             try:
                 return yaml.safe_load(stream)
             except yaml.YAMLError as exc:
-                print(exc)
+                click.echo("Error parsing config file:")
+                click.echo(exc)
+                sys.exit(EXIT_CODE_INVALID_YAML)
 
 
 def flatten(l):
     """Flatten a list of lists"""
     return [item for sublist in l for item in sublist]
```

### Comparing `i2cssh-0.1.4/src/i2cssh/tests/test_i2cssh.py` & `i2cssh-0.1.6/src/i2cssh/tests/test_i2cssh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,124 @@
-from email.policy import default
+import asyncio
+import copy
 import unittest
+from email.policy import default
+from unittest.mock import ANY, AsyncMock, MagicMock, call, mock_open, patch
+
+import pytest
 from click.testing import CliRunner
+
 import i2cssh
 from i2cssh.lib import app
-from unittest.mock import MagicMock, patch, ANY, call
-import copy
+from i2cssh.version import version
 
 
 def test_help():
     runner = CliRunner()
-    result = runner.invoke(app, ["-h"])
-    assert result.exit_code == 2
+    result = runner.invoke(app, ["--help"])
+    assert result.exit_code == 0
     assert result.output.startswith("Usage:")
 
 
+def test_version():
+    runner = CliRunner()
+    result = runner.invoke(app, ["-v"])
+    assert result.exit_code == 0
+    assert result.output.startswith(version())
+
+
+@pytest.mark.asyncio
+@patch("asyncio.sleep", new_callable=AsyncMock)
+async def test_sleep(sleep_moc: AsyncMock):
+    await i2cssh.lib.sleep(1)
+    sleep_moc.assert_called_once_with(1)
+
+
+@pytest.mark.asyncio
+@patch("asyncio.sleep", new_callable=AsyncMock)
+async def test_create_unused_pane(sleep_moc: AsyncMock):
+    pane = AsyncMock()
+    profile = AsyncMock()
+    pane.async_get_profile.return_value = profile
+    await i2cssh.lib.create_unused_pane(pane)
+    pane.async_get_profile.assert_called_once()
+    sleep_moc.assert_called_once_with(0.3)
+    profile.async_set_foreground_color.assert_called_once()
+    pane.async_send_text.assert_has_calls(
+        [
+            call("unset HISTFILE\n"),
+            call(
+                "stty -isig -icanon -echo && echo -e '\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nUNUSED' && cat > /dev/null\n"
+            ),
+        ]
+    )
+
+
+@pytest.mark.asyncio
+async def test_fullscreen():
+    window = AsyncMock()
+    await i2cssh.lib.set_fullscreen(window)
+    window.async_set_fullscreen.assert_called_once_with(True)
+
+
+@pytest.mark.asyncio
+@patch("iterm2.async_get_app", new_callable=AsyncMock)
+async def test_get_window(iterm_mock: AsyncMock):
+    connection = AsyncMock()
+    await i2cssh.lib.get_window(connection)
+    iterm_mock.assert_called_once_with(connection)
+
+
+@pytest.mark.asyncio
+async def test_execute_command():
+    pane = AsyncMock()
+    cmd = MagicMock()
+    await i2cssh.lib.execute_command(pane, cmd)
+    pane.async_send_text.assert_called_once_with(cmd)
+
+
+def test_get_host_strs_from_file():
+    with patch("builtins.open", mock_open(read_data="foo\nbar\n")):
+        assert i2cssh.lib.get_host_strs_from_file("foo") == ["foo", "bar"]
+
+
 def invoke(args, config):
     with patch("i2cssh.lib.read_config") as mock_read_config, patch(
         "i2cssh.lib.get_window"
-    ):
+    ), patch("iterm2.run_until_complete", run_until_complete_mock):
         mock_read_config.return_value = config
         runner = CliRunner()
         result = runner.invoke(app, args)
         assert result.exit_code == 0
         return result
 
 
+def run_until_complete_mock(target):
+    connection = MagicMock()()
+    loop = asyncio.get_event_loop()
+    tasks = [loop.create_task(target(connection))]
+    loop.run_until_complete(asyncio.wait(tasks))
+
+
+class TestReadConfig(unittest.TestCase):
+    @patch("os.path.isfile", return_value=True)
+    @patch("builtins.open", mock_open(read_data="@"))
+    @patch("sys.exit")
+    def test_read_test_read_config_invalid_yaml(
+        self, exit_mock: MagicMock, open_mock: MagicMock
+    ):
+        i2cssh.lib.read_config()
+        exit_mock.assert_called_once_with(252)
+
+    @patch("os.path.isfile", return_value=True)
+    @patch("builtins.open", mock_open(read_data="version: 2\nfoo: bar\n"))
+    def test_read_config(self, open_mock: MagicMock):
+        assert i2cssh.lib.read_config() == {"foo": "bar", "version": 2}
+
+
 default_config = {
     "clusters": {
         "foo": {
             "hosts": ["foo1", "foo2"],
         }
     }
 }
@@ -46,14 +136,53 @@
         calls,
         any_order=True,
     )
 
 
 @patch("i2cssh.lib.execute_command")
 class TestParams(unittest.TestCase):
+    def test_no_args(self, mec: MagicMock):
+        with patch("i2cssh.lib.read_config") as mock_read_config, patch(
+            "i2cssh.lib.get_window"
+        ), patch("iterm2.run_until_complete", run_until_complete_mock):
+            mock_read_config.return_value = default_config
+            runner = CliRunner()
+            result = runner.invoke(app)
+            assert result.exit_code == 255
+
+    def test_unknown_cluster(self, mec: MagicMock):
+        with patch("i2cssh.lib.read_config") as mock_read_config, patch(
+            "i2cssh.lib.get_window"
+        ), patch("iterm2.run_until_complete", run_until_complete_mock):
+            mock_read_config.return_value = default_config
+            runner = CliRunner()
+            result = runner.invoke(app, ["unknown_cluster"])
+            assert result.exit_code == 254
+
+    def test_unknown_clusters_cli(self, mec: MagicMock):
+        with patch("i2cssh.lib.read_config") as mock_read_config, patch(
+            "i2cssh.lib.get_window"
+        ), patch("iterm2.run_until_complete", run_until_complete_mock):
+            mock_read_config.return_value = default_config
+            runner = CliRunner()
+            result = runner.invoke(app, ["-c", "unknown_cluster"])
+            assert result.exit_code == 254
+
+    def test_no_current_window_cli(self, mec: MagicMock):
+        with patch("i2cssh.lib.read_config") as mock_read_config, patch(
+            "i2cssh.lib.get_window"
+        ) as mock_get_window, patch(
+            "iterm2.run_until_complete", run_until_complete_mock
+        ):
+            mock_read_config.return_value = default_config
+            mock_get_window.return_value = None
+            runner = CliRunner()
+            result = runner.invoke(app, ["-c", "foo"])
+            assert result.exit_code == 253
+
     def test_clusters_cli(self, mec: MagicMock):
         invoke(["-c", "foo"], default_config)
         assert_options(mec, "")
 
     @patch("i2cssh.lib.create_tab")
     @patch("i2cssh.lib.create_window")
     def test_multiple_clusters_cli(
@@ -70,14 +199,29 @@
             }
         }
         invoke(["-c", "foo,bar"], config)
         assert_options(mec, "", ["foo1", "foo2", "bar1", "bar2"])
         mock_create_window.assert_called_once()
         self.assertEqual(mock_create_tab.call_count, 0)
 
+    def test_include_from(self, mec: MagicMock):
+        config = {
+            "clusters": {
+                "foo": {
+                    "include_from": ["bar"],
+                    "hosts": ["foo1", "foo2"],
+                },
+                "bar": {
+                    "hosts": ["bar1", "bar2"],
+                },
+            }
+        }
+        invoke(["foo"], config)
+        assert_options(mec, "", ["foo1", "foo2", "bar1", "bar2"])
+
     @patch("i2cssh.lib.create_tab")
     @patch("i2cssh.lib.create_window")
     def test_tab_split_clusters_cli(
         self, mock_create_window: MagicMock, mock_create_tab: MagicMock, mec: MagicMock
     ):
         config = {
             "clusters": {
@@ -95,15 +239,15 @@
         invoke(["-c", "foo,bar,baz", "-t"], config)
         assert_options(mec, "", ["foo1", "foo2", "bar1", "bar2", "baz1", "baz2"])
         mock_create_window.assert_called_once()
         self.assertEqual(mock_create_tab.call_count, 2)
 
     @patch("i2cssh.lib.create_tab")
     @patch("i2cssh.lib.create_window")
-    def test_tab_split_clusters_config(
+    def test_tab_split_clusters_global_config(
         self, mock_create_window: MagicMock, mock_create_tab: MagicMock, mec: MagicMock
     ):
         config = {
             "tab_split": True,
             "clusters": {
                 "foo": {
                     "hosts": ["foo1", "foo2"],
@@ -159,15 +303,15 @@
         invoke(["-c", "foo,bar", "-m", "baz1,baz2", "-T"], config)
         assert_options(mec, "", ["foo1", "foo2", "bar1", "bar2", "baz1", "baz2"])
         mock_create_window.assert_called_once()
         self.assertEqual(mock_create_tab.call_count, 3)
 
     @patch("i2cssh.lib.create_tab")
     @patch("i2cssh.lib.create_window")
-    def test_tab_split_no_group_clusters_with_machines_config(
+    def test_tab_split_no_group_clusters_with_machines_global_config(
         self, mock_create_window: MagicMock, mock_create_tab: MagicMock, mec: MagicMock
     ):
         config = {
             "tab_split_nogroup": True,
             "clusters": {
                 "foo": {
                     "hosts": ["foo1", "foo2"],
@@ -220,15 +364,15 @@
         invoke(["-c", "foo,bar", "-m", "baz1,baz2", "-W"], config)
         assert_options(mec, "", ["foo1", "foo2", "bar1", "bar2", "baz1", "baz2"])
         self.assertEqual(mock_create_window.call_count, 0)
         self.assertEqual(mock_create_tab.call_count, 1)
 
     @patch("i2cssh.lib.create_tab")
     @patch("i2cssh.lib.create_window")
-    def test_clusters_same_window_no_group_config(
+    def test_clusters_same_window_no_group_global_config(
         self, mock_create_window: MagicMock, mock_create_tab: MagicMock, mec: MagicMock
     ):
         config = {
             "same_window": True,
             "clusters": {
                 "foo": {
                     "hosts": ["foo1", "foo2"],
@@ -247,61 +391,98 @@
         invoke(["foo"], default_config)
         assert_options(mec, "")
 
     def test_machines_cli(self, mec: MagicMock):
         invoke(["-m", "bar1,bar2"], default_config)
         assert_options(mec, "", ["bar1", "bar2"])
 
+    def test_multiple_hosts_cli(self, mec: MagicMock):
+        invoke(["bar1", "bar2"], default_config)
+        assert_options(mec, "", ["bar1", "bar2"])
+
+    @patch("i2cssh.lib.create_tab")
+    @patch("i2cssh.lib.create_window")
+    def test_hosts_same_window_no_group_cli(
+        self, mock_create_window: MagicMock, mock_create_tab: MagicMock, mec: MagicMock
+    ):
+        invoke(["-T", "bar1", "bar2"], default_config)
+        assert_options(mec, "", ["bar1", "bar2"])
+        self.assertEqual(mock_create_window.call_count, 1)
+        self.assertEqual(mock_create_tab.call_count, 1)
+
+    @patch("i2cssh.lib.create_tab")
+    @patch("i2cssh.lib.create_window")
+    def test_hosts_same_window_no_group_cli(
+        self, mock_create_window: MagicMock, mock_create_tab: MagicMock, mec: MagicMock
+    ):
+        invoke(["-t", "bar1", "bar2"], default_config)
+        assert_options(mec, "", ["bar1", "bar2"])
+        self.assertEqual(mock_create_window.call_count, 1)
+        self.assertEqual(mock_create_tab.call_count, 0)
+
     def test_forward_agent_cli(self, mec: MagicMock):
         invoke(["foo", "-A"], default_config)
         assert_options(mec, "-A")
 
-    def test_forward_agent_config_cluster(self, mec: MagicMock):
+    def test_forward_agent_cluster_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["forward_agent"] = True
         invoke(["foo"], config)
         assert_options(mec, "-A")
 
-    def test_forward_agent_config_global(self, mec: MagicMock):
+    def test_forward_agent_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["forward_agent"] = True
         invoke(["foo"], config)
         assert_options(mec, "-A")
 
     def test_login_cli(self, mec: MagicMock):
         invoke(["foo", "-l", "myuser"], default_config)
         assert_options(mec, "", ["myuser@foo1", "myuser@foo2"])
 
-    def test_login_config(self, mec: MagicMock):
+    def test_login_cluster_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["login"] = "myuser"
         invoke(["foo"], config)
         assert_options(mec, "", ["myuser@foo1", "myuser@foo2"])
 
-    def test_login_config_global(self, mec: MagicMock):
+    def test_login_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["login"] = "myuser"
         invoke(["foo"], config)
         assert_options(mec, "", ["myuser@foo1", "myuser@foo2"])
 
+    def test_login_host_config(self, mec: MagicMock):
+        config = {
+            "same_window": True,
+            "clusters": {
+                "foo": {
+                    "hosts": ["myuser@foo1", "myuser@foo2"],
+                },
+            },
+        }
+
+        invoke(["foo"], config)
+        assert_options(mec, "", ["myuser@foo1", "myuser@foo2"])
+
     def test_environment_cli(self, mec: MagicMock):
         invoke(["foo", "-e", "LC_FOO=foo,LC_BAR=bar"], default_config)
         assert_options(mec, "-o SendEnv=LC_FOO,LC_BAR")
 
-    def test_environment_config(self, mec: MagicMock):
+    def test_environment_cluster_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["environment"] = {"LC_FOO": "foo", "LC_BAR": "bar"}
         invoke(["foo"], config)
         assert_options(
             mec,
             "-o SendEnv=LC_FOO,LC_BAR",
             extra_calls=["export LC_FOO=foo; export LC_BAR=bar;\n"],
         )
 
-    def test_environment_config_global(self, mec: MagicMock):
+    def test_environment_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["environment"] = {"LC_FOO": "foo", "LC_BAR": "bar"}
         invoke(["foo"], config)
         assert_options(
             mec,
             "-o SendEnv=LC_FOO,LC_BAR",
             extra_calls=["export LC_FOO=foo; export LC_BAR=bar;\n"],
@@ -311,67 +492,67 @@
         invoke(["foo", "-r"], default_config)
         assert_options(
             mec,
             "-o SendEnv=LC_RANK",
             extra_calls=["export LC_RANK=0;\n", "export LC_RANK=1;\n"],
         )
 
-    def test_rank_config(self, mec: MagicMock):
+    def test_rank_cluster_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["rank"] = True
         invoke(["foo"], config)
         assert_options(
             mec,
             "-o SendEnv=LC_RANK",
             extra_calls=["export LC_RANK=0;\n", "export LC_RANK=1;\n"],
         )
 
-    def test_rank_config_global(self, mec: MagicMock):
+    def test_rank_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["rank"] = True
         invoke(["foo"], config)
         assert_options(
             mec,
             "-o SendEnv=LC_RANK",
             extra_calls=["export LC_RANK=0;\n", "export LC_RANK=1;\n"],
         )
 
     def test_extra_cli(self, mec: MagicMock):
-        invoke(["foo", "-Xi=myidentity.pem", "-Xp=2222"], default_config)
-        assert_options(mec, "-i myidentity.pem -p 2222")
+        invoke(["foo", "-Xi=myidentity.pem", "-Xp=2222", "-XZ"], default_config)
+        assert_options(mec, "-i myidentity.pem -p 2222 -Z")
 
-    def test_extra_config_list(self, mec: MagicMock):
+    def test_extra_cluster_config_list(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
-        config["clusters"]["foo"]["extra"] = ["i=myidentity.pem", "p=2222"]
+        config["clusters"]["foo"]["extra"] = ["i=myidentity.pem", "p=2222", "Z"]
         invoke(["foo"], config)
-        assert_options(mec, "-i myidentity.pem -p 2222")
+        assert_options(mec, "-i myidentity.pem -p 2222 -Z")
 
-    def test_extra_config_dict(self, mec: MagicMock):
+    def test_extra_cluster_config_dict(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["extra"] = {"i": "myidentity.pem", "p": 2222}
         invoke(["foo"], config)
         assert_options(mec, "-i myidentity.pem -p 2222")
 
-    def test_extra_config_global(self, mec: MagicMock):
+    def test_extra_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["extra"] = ["i=myidentity.pem", "p=2222"]
         invoke(["foo"], config)
         assert_options(mec, "-i myidentity.pem -p 2222")
 
     def test_gateway_cli(self, mec: MagicMock):
         invoke(["foo", "-g bar"], default_config)
         assert_options(mec, '-o ProxyCommand="ssh -W %h:%p bar"')
 
-    def test_gateway_config(self, mec: MagicMock):
+    def test_gateway_cluster_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["gateway"] = "bar"
         invoke(["foo"], config)
         assert_options(mec, '-o ProxyCommand="ssh -W %h:%p bar"')
 
-    def test_gateway_config_global(self, mec: MagicMock):
+    def test_gateway_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["gateway"] = "bar"
         invoke(["foo"], config)
         assert_options(mec, '-o ProxyCommand="ssh -W %h:%p bar"')
 
     def test_custom_command_cli(self, mec: MagicMock):
         invoke(["foo", "-x mycmd {host} -- bla"], default_config)
@@ -380,28 +561,28 @@
             [
                 call(ANY, f"unset HISTFILE && mycmd foo1 -- bla\n"),
                 call(ANY, f"unset HISTFILE && mycmd foo2 -- bla\n"),
             ],
             any_order=True,
         )
 
-    def test_custom_command_config(self, mec: MagicMock):
+    def test_custom_command_cluster_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["custom_command"] = "mycmd {host} -- bla"
         invoke(["foo"], config)
 
         mec.assert_has_calls(
             [
                 call(ANY, f"unset HISTFILE && mycmd foo1 -- bla\n"),
                 call(ANY, f"unset HISTFILE && mycmd foo2 -- bla\n"),
             ],
             any_order=True,
         )
 
-    def test_custom_command_config_global(self, mec: MagicMock):
+    def test_custom_command_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["custom_command"] = "mycmd {host} -- bla"
         invoke(["foo"], config)
 
         mec.assert_has_calls(
             [
                 call(ANY, f"unset HISTFILE && mycmd foo1 -- bla\n"),
@@ -419,15 +600,17 @@
     @patch("i2cssh.lib.set_fullscreen")
     def test_fullscreen_off_cli(self, mock_fullscreen: MagicMock, mec: MagicMock):
         invoke(["-c", "foo"], default_config)
         assert_options(mec, "")
         self.assertEqual(mock_fullscreen.call_count, 0)
 
     @patch("i2cssh.lib.set_fullscreen")
-    def test_fullscreen_on_config(self, mock_fullscreen: MagicMock, mec: MagicMock):
+    def test_fullscreen_on_global_config(
+        self, mock_fullscreen: MagicMock, mec: MagicMock
+    ):
         config = copy.deepcopy(default_config)
         config["fullscreen"] = True
         invoke(["foo"], config)
         assert_options(mec, "")
         mock_fullscreen.assert_called_once()
 
     def test_precedence_cli(self, mec: MagicMock):
@@ -464,28 +647,28 @@
             [
                 call(ANY, f"unset HISTFILE && exec ssh -o ControlMaster=no foo1\n"),
                 call(ANY, f"unset HISTFILE && exec ssh -o ControlMaster=no foo2\n"),
             ],
             any_order=True,
         )
 
-    def test_use_exec_config(self, mec: MagicMock):
+    def test_use_exec_cluster_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["exec"] = True
         invoke(["foo"], config)
 
         mec.assert_has_calls(
             [
                 call(ANY, f"unset HISTFILE && exec ssh -o ControlMaster=no foo1\n"),
                 call(ANY, f"unset HISTFILE && exec ssh -o ControlMaster=no foo2\n"),
             ],
             any_order=True,
         )
 
-    def test_use_exec_config_global(self, mec: MagicMock):
+    def test_use_exec_global_config(self, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["exec"] = True
         invoke(["foo"], config)
 
         mec.assert_has_calls(
             [
                 call(ANY, f"unset HISTFILE && exec ssh -o ControlMaster=no foo1\n"),
@@ -503,25 +686,23 @@
     @patch("i2cssh.lib.set_broadcast_domains")
     def test_broadcast_off_cli(self, mock_broadcast: MagicMock, mec: MagicMock):
         invoke(["-c", "foo"], default_config)
         assert_options(mec, "")
         mock_broadcast.assert_has_calls([call(ANY, [])])
 
     @patch("i2cssh.lib.set_broadcast_domains")
-    def test_broadcast_on_config(self, mock_broadcast: MagicMock, mec: MagicMock):
+    def test_broadcast_global_config(self, mock_broadcast: MagicMock, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["broadcast"] = True
         invoke(["foo"], config)
         assert_options(mec, "")
         mock_broadcast.assert_has_calls([call(ANY, [ANY])])
 
     @patch("i2cssh.lib.set_broadcast_domains")
-    def test_broadcast_on_config_cluster(
-        self, mock_broadcast: MagicMock, mec: MagicMock
-    ):
+    def test_broadcast_cluster_config(self, mock_broadcast: MagicMock, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["broadcast"] = True
         invoke(["foo"], config)
         assert_options(mec, "")
         mock_broadcast.assert_has_calls([call(ANY, [ANY])])
 
     @patch("i2cssh.lib.set_broadcast_domains")
@@ -550,15 +731,15 @@
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["nobroadcast"] = True
         invoke(["-c", "foo", "-nb"], config)
         assert_options(mec, "")
         mock_broadcast.assert_has_calls([call(ANY, [])])
 
     @patch("i2cssh.lib.set_broadcast_domains")
-    def test_broadcast_on_config_cluster(
+    def test_broadcast_on_cluster_config_override(
         self, mock_broadcast: MagicMock, mec: MagicMock
     ):
         config = copy.deepcopy(default_config)
         config["broadcast"] = True
         config["clusters"]["foo"]["nobroadcast"] = True
         invoke(["foo"], config)
         assert_options(mec, "")
@@ -608,45 +789,45 @@
     @patch("i2cssh.lib.sleep")
     def test_sleep_cli(self, mock_sleep: MagicMock, mec: MagicMock):
         invoke(["-c", "foo", "-s", "1"], default_config)
         assert_options(mec, "")
         self.assertEqual(mock_sleep.call_count, 2)
 
     @patch("i2cssh.lib.sleep")
-    def test_sleep_config(self, mock_sleep: MagicMock, mec: MagicMock):
+    def test_sleep_cluster_config(self, mock_sleep: MagicMock, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["sleep"] = 1
         invoke(["-c", "foo", "-s", "1"], config)
         assert_options(mec, "")
         self.assertEqual(mock_sleep.call_count, 2)
 
     @patch("i2cssh.lib.sleep")
-    def test_sleep_config_global(self, mock_sleep: MagicMock, mec: MagicMock):
+    def test_sleep_global_config(self, mock_sleep: MagicMock, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["sleep"] = 1
         invoke(["-c", "foo", "-s", "1"], config)
         assert_options(mec, "")
         self.assertEqual(mock_sleep.call_count, 2)
 
     @patch("i2cssh.lib.create_lwop")
     def test_shell_cli(self, mock_lwop: MagicMock, mec: MagicMock):
         invoke(["-c", "foo", "-S", "zsh"], default_config)
         assert_options(mec, "")
         mock_lwop.assert_has_calls([call("/usr/bin/env zsh -l")])
 
     @patch("i2cssh.lib.create_lwop")
-    def test_shell_config(self, mock_lwop: MagicMock, mec: MagicMock):
+    def test_shell_cluster_config(self, mock_lwop: MagicMock, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["clusters"]["foo"]["shell"] = "zsh"
         invoke(["-c", "foo"], config)
         assert_options(mec, "")
         mock_lwop.assert_has_calls([call("/usr/bin/env zsh -l")])
 
     @patch("i2cssh.lib.create_lwop")
-    def test_shell_config_global(self, mock_lwop: MagicMock, mec: MagicMock):
+    def test_shell_global_config(self, mock_lwop: MagicMock, mec: MagicMock):
         config = copy.deepcopy(default_config)
         config["shell"] = "zsh"
         invoke(["-c", "foo"], config)
         assert_options(mec, "")
         mock_lwop.assert_has_calls([call("/usr/bin/env zsh -l")])
 
     def test_compute_geometry(self, mec: MagicMock):
@@ -732,15 +913,15 @@
                 call("Default", ANY, True, ANY),
                 call("Default", ANY, False, ANY),
                 call("Default", ANY, False, ANY),
             ]
         )
 
     @patch("i2cssh.lib.split_pane")
-    def test_direction_row_config_global(
+    def test_direction_row_global_config(
         self, mock_split_pane: MagicMock, mec: MagicMock
     ):
         config = {
             "direction": "row",
             "clusters": {
                 "foo": {
                     "hosts": ["foo1", "foo2", "foo3", "foo4"],
@@ -755,15 +936,15 @@
                 call("Default", ANY, False, ANY),
                 call("Default", ANY, True, ANY),
                 call("Default", ANY, True, ANY),
             ]
         )
 
     @patch("i2cssh.lib.split_pane")
-    def test_direction_column_config_global(
+    def test_direction_column_global_config(
         self, mock_split_pane: MagicMock, mec: MagicMock
     ):
         config = {
             "direction": "column",
             "clusters": {
                 "foo": {
                     "hosts": ["foo1", "foo2", "foo3", "foo4"],
@@ -778,15 +959,17 @@
                 call("Default", ANY, True, ANY),
                 call("Default", ANY, False, ANY),
                 call("Default", ANY, False, ANY),
             ]
         )
 
     @patch("i2cssh.lib.split_pane")
-    def test_direction_row_config(self, mock_split_pane: MagicMock, mec: MagicMock):
+    def test_direction_row_cluster_config(
+        self, mock_split_pane: MagicMock, mec: MagicMock
+    ):
         config = {
             "clusters": {
                 "foo": {
                     "direction": "row",
                     "hosts": ["foo1", "foo2", "foo3", "foo4"],
                 },
             },
@@ -799,15 +982,17 @@
                 call("Default", ANY, False, ANY),
                 call("Default", ANY, True, ANY),
                 call("Default", ANY, True, ANY),
             ]
         )
 
     @patch("i2cssh.lib.split_pane")
-    def test_direction_column_config(self, mock_split_pane: MagicMock, mec: MagicMock):
+    def test_direction_column_cluster_config(
+        self, mock_split_pane: MagicMock, mec: MagicMock
+    ):
         config = {
             "clusters": {
                 "foo": {
                     "direction": "column",
                     "hosts": ["foo1", "foo2", "foo3", "foo4"],
                 },
             },
@@ -818,7 +1003,29 @@
         mock_split_pane.assert_has_calls(
             [
                 call("Default", ANY, True, ANY),
                 call("Default", ANY, False, ANY),
                 call("Default", ANY, False, ANY),
             ]
         )
+
+    @patch("i2cssh.lib.create_unused_pane")
+    def test_direction_column_cluster_config(
+        self, mock_create_unused_pane: MagicMock, mec: MagicMock
+    ):
+        config = {
+            "clusters": {
+                "foo": {
+                    "direction": "column",
+                    "hosts": ["foo1", "foo2", "foo3"],
+                },
+            },
+        }
+        invoke(["-c", "foo"], config)
+        assert_options(mec, "")
+        mock_create_unused_pane.assert_called_once()
+
+    @patch("i2cssh.lib.get_host_strs_from_file")
+    def test_file_cli(self, mock_get_host_strs_from_file: MagicMock, mec: MagicMock):
+        mock_get_host_strs_from_file.return_value = ["bar1", "bar2"]
+        invoke(["-f", "bar_hosts"], default_config)
+        assert_options(mec, "", ["bar1", "bar2"])
```

### Comparing `i2cssh-0.1.4/src/i2cssh.egg-info/PKG-INFO` & `i2cssh-0.1.6/src/i2cssh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.4
+Version: 0.1.6
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

