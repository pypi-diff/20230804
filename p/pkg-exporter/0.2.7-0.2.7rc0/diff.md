# Comparing `tmp/pkg_exporter-0.2.7.tar.gz` & `tmp/pkg_exporter-0.2.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_exporter-0.2.7.tar", max compression
+gzip compressed data, was "pkg_exporter-0.2.7rc0.tar", max compression
```

## Comparing `pkg_exporter-0.2.7.tar` & `pkg_exporter-0.2.7rc0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-08-04 18:54:35.872925 pkg_exporter-0.2.7/LICENSE
--rw-r--r--   0        0        0     4337 2023-08-04 18:54:35.872925 pkg_exporter-0.2.7/README.md
--rw-r--r--   0        0        0      682 2023-08-04 18:54:57.820845 pkg_exporter-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-04 18:54:35.872925 pkg_exporter-0.2.7/src/pkg_exporter/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 18:54:35.872925 pkg_exporter-0.2.7/src/pkg_exporter/pkgmanager/__init__.py
--rw-r--r--   0        0        0     3961 2023-08-04 18:54:35.872925 pkg_exporter-0.2.7/src/pkg_exporter/pkgmanager/apt.py
--rw-r--r--   0        0        0      284 2023-08-04 18:54:35.872925 pkg_exporter-0.2.7/src/pkg_exporter/reboot.py
--rwxr-xr-x   0        0        0     1820 2023-08-04 18:54:35.872925 pkg_exporter-0.2.7/src/pkg_exporter/textfile.py
--rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 pkg_exporter-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-19 19:40:05.368367 pkg_exporter-0.2.7rc0/LICENSE
+-rw-r--r--   0        0        0     3948 2023-01-19 19:40:05.368367 pkg_exporter-0.2.7rc0/README.md
+-rw-r--r--   0        0        0      685 2023-01-19 19:40:37.916537 pkg_exporter-0.2.7rc0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-19 19:40:05.368367 pkg_exporter-0.2.7rc0/src/pkg_exporter/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-19 19:40:05.368367 pkg_exporter-0.2.7rc0/src/pkg_exporter/pkgmanager/__init__.py
+-rw-r--r--   0        0        0     3961 2023-01-19 19:40:05.368367 pkg_exporter-0.2.7rc0/src/pkg_exporter/pkgmanager/apt.py
+-rw-r--r--   0        0        0      284 2023-01-19 19:40:05.368367 pkg_exporter-0.2.7rc0/src/pkg_exporter/reboot.py
+-rwxr-xr-x   0        0        0     1820 2023-01-19 19:40:05.368367 pkg_exporter-0.2.7rc0/src/pkg_exporter/textfile.py
+-rw-r--r--   0        0        0     4921 1970-01-01 00:00:00.000000 pkg_exporter-0.2.7rc0/setup.py
+-rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 pkg_exporter-0.2.7rc0/PKG-INFO
```

### Comparing `pkg_exporter-0.2.7/LICENSE` & `pkg_exporter-0.2.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pkg_exporter-0.2.7/README.md` & `pkg_exporter-0.2.7rc0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pkg-exporter
+Version: 0.2.7rc0
+Summary: This project provides an textfile-based exporter for apt-repositories
+License: GPL3
+Author: Marvin Gaube
+Author-email: dev@marvingaube.de
+Requires-Python: >=3.6,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: prometheus-client (>=0.15.0,<0.16.0)
+Description-Content-Type: text/markdown
+
 # Prometheus PKG Exporter
 
 This project provides an textfile-based exporter for apt-repositories. 
 
 **The Project is in its early development phases. Interfaces may change without notice. Compatibility and Stability do vary.**
 
 For the changelog, use the [Releases-Section on GitHub](https://github.com/margau/pkg-exporter/releases/)
@@ -42,31 +61,21 @@
 
 ## Contributing
 
 Feel free to contribute improvements, as well as support for non-apt based systems.
 
 ## Installation
 
-### Global pip installation
 Run `pip3 install pkg-exporter`.
 
-### Install from source
 Clone the repository and run `poetry install` from the main directory.
 You can also use other standard installation methods for python packages, like directly installing from this git repository.
 
 The pyinstaller-based binary is not provided any more.
 
-### pipx
-If a global pip installation is not possible (e.g. from debian 12 onwards), you can use [pipx](https://pypa.github.io/pipx), either for install, and/or for running pkg-exporter ad hoc:
-```
-pipx run --system-site-packages pkg-exporter
-```
-
-`--system-site-packages` is necessary to provide access to the system python3-apt lib.
-
 ### apt-based systems
 
 Currently, only apt-based systems are supported. `python3-apt` needs to be installed on the system.
 
 ## Configuration and Usage
 
 The node exporter needs to be configured for textfiles using the `--collector.textfile.directory` option. This exporter needs to write the exported metrics into this directory.
```

### Comparing `pkg_exporter-0.2.7/pyproject.toml` & `pkg_exporter-0.2.7rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pkg-exporter"
-version = "0.2.7"
+version = "0.2.7rc0"
 description = "This project provides an textfile-based exporter for apt-repositories"
 authors = ["Marvin Gaube <dev@marvingaube.de>"]
 license = "GPL3"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `pkg_exporter-0.2.7/src/pkg_exporter/pkgmanager/apt.py` & `pkg_exporter-0.2.7rc0/src/pkg_exporter/pkgmanager/apt.py`

 * *Files identical despite different names*

### Comparing `pkg_exporter-0.2.7/src/pkg_exporter/textfile.py` & `pkg_exporter-0.2.7rc0/src/pkg_exporter/textfile.py`

 * *Files identical despite different names*

### Comparing `pkg_exporter-0.2.7/PKG-INFO` & `pkg_exporter-0.2.7rc0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,38 @@
-Metadata-Version: 2.1
-Name: pkg-exporter
-Version: 0.2.7
-Summary: This project provides an textfile-based exporter for apt-repositories
-License: GPL3
-Author: Marvin Gaube
-Author-email: dev@marvingaube.de
-Requires-Python: >=3.6,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: prometheus-client (>=0.15.0,<0.16.0)
-Description-Content-Type: text/markdown
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-# Prometheus PKG Exporter
+package_dir = \
+{'': 'src'}
 
-This project provides an textfile-based exporter for apt-repositories. 
+packages = \
+['pkg_exporter', 'pkg_exporter.pkgmanager']
 
-**The Project is in its early development phases. Interfaces may change without notice. Compatibility and Stability do vary.**
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['prometheus-client>=0.15.0,<0.16.0']
+
+entry_points = \
+{'console_scripts': ['pkg-exporter = pkg_exporter.textfile:main']}
+
+setup_kwargs = {
+    'name': 'pkg-exporter',
+    'version': '0.2.7rc0',
+    'description': 'This project provides an textfile-based exporter for apt-repositories',
+    'long_description': '# Prometheus PKG Exporter\n\nThis project provides an textfile-based exporter for apt-repositories. \n\n**The Project is in its early development phases. Interfaces may change without notice. Compatibility and Stability do vary.**\n\nFor the changelog, use the [Releases-Section on GitHub](https://github.com/margau/pkg-exporter/releases/)\n\n## Exported Metrics\n\nAt the moment, the packages installed, upgradable, broken and autoremovable are exported per repository as gauge. The label set depends on the packet manager type.\n\nAdditionally, `pkg_reboot_required` is exported to indicate that an reboot is needed.\n\n```\n# HELP pkg_reboot_required Node Requires an Reboot\n# TYPE pkg_reboot_required gauge\npkg_reboot_required 1.0\n# HELP pkg_update_start_time timestamp of last apt update start\n# TYPE pkg_update_start_time gauge\npkg_update_start_time 1.641382890503045e+09\n# HELP pkg_update_end_time Timestamp of last apt update finish\n# TYPE pkg_update_end_time gauge\npkg_update_end_time 1.641382892755024e+09\n# HELP pkg_update_time_available Availability of the apt update timestamp\n# TYPE pkg_update_time_available gauge\npkg_update_time_available 1.0\n# HELP pkg_installed Installed packages per origin\n# TYPE pkg_installed gauge\npkg_installed{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 672.0\n# HELP pkg_upgradable Upgradable packages per origin\n# TYPE pkg_upgradable gauge\npkg_upgradable{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 7.0\n# HELP pkg_auto_removable Auto-removable packages per origin\n# TYPE pkg_auto_removable gauge\npkg_auto_removable{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 6.0\n# HELP pkg_broken Broken packages per origin\n# TYPE pkg_broken gauge\npkg_broken{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 0.0\n\n```\n\n## Contributing\n\nFeel free to contribute improvements, as well as support for non-apt based systems.\n\n## Installation\n\nRun `pip3 install pkg-exporter`.\n\nClone the repository and run `poetry install` from the main directory.\nYou can also use other standard installation methods for python packages, like directly installing from this git repository.\n\nThe pyinstaller-based binary is not provided any more.\n\n### apt-based systems\n\nCurrently, only apt-based systems are supported. `python3-apt` needs to be installed on the system.\n\n## Configuration and Usage\n\nThe node exporter needs to be configured for textfiles using the `--collector.textfile.directory` option. This exporter needs to write the exported metrics into this directory. \n\nThe default path is `/var/prometheus/pkg-exporter.prom`, and may be changed via the `PKG_EXPORTER_FILE`-Environment Variable.\nIf the directory is not already present, it will be created by the exporter.\n\nThe command `pkg_exporter` provided by the package or the binary shall be executed in a appropriate interval, e.g. using cron or systemd timers.\nThe exporter needs to be executed with appropriate privileges, which are not necessarily root privileges.\n\nAn example configuration will be provided in this repository in the future.\n\n### apt hook\nTo enable monitoring for apt update calls, place the file under `docs/00-pve-exporter` in `/etc/apt/apt.conf.d` on your system.\nIt will place files under `/tmp`. To customize the filepath of the timestamp files, the the environment variables `PKG_EXPORTER_APT_PRE_FILE` & `PKG_EXPORTER_APT_POST_FILE` may be used.\nYou can see the success of monitoring the apt update timestamps if the following metric is 1: `pkg_update_time_available 1.0`\n\nPlease not that the presence of an timestamp does not mean that all repositories were updated without issues.\n\n## Alerting\n\nExample alerting rules will be provided in the future.\n\n## Roadmap\n\n- Support for other pkg managers\n- Deployment as dpkg-Packet',
+    'author': 'Marvin Gaube',
+    'author_email': 'dev@marvingaube.de',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'package_dir': package_dir,
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
+    'python_requires': '>=3.6,<4.0',
+}
 
-For the changelog, use the [Releases-Section on GitHub](https://github.com/margau/pkg-exporter/releases/)
-
-## Exported Metrics
-
-At the moment, the packages installed, upgradable, broken and autoremovable are exported per repository as gauge. The label set depends on the packet manager type.
-
-Additionally, `pkg_reboot_required` is exported to indicate that an reboot is needed.
-
-```
-# HELP pkg_reboot_required Node Requires an Reboot
-# TYPE pkg_reboot_required gauge
-pkg_reboot_required 1.0
-# HELP pkg_update_start_time timestamp of last apt update start
-# TYPE pkg_update_start_time gauge
-pkg_update_start_time 1.641382890503045e+09
-# HELP pkg_update_end_time Timestamp of last apt update finish
-# TYPE pkg_update_end_time gauge
-pkg_update_end_time 1.641382892755024e+09
-# HELP pkg_update_time_available Availability of the apt update timestamp
-# TYPE pkg_update_time_available gauge
-pkg_update_time_available 1.0
-# HELP pkg_installed Installed packages per origin
-# TYPE pkg_installed gauge
-pkg_installed{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 672.0
-# HELP pkg_upgradable Upgradable packages per origin
-# TYPE pkg_upgradable gauge
-pkg_upgradable{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 7.0
-# HELP pkg_auto_removable Auto-removable packages per origin
-# TYPE pkg_auto_removable gauge
-pkg_auto_removable{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 6.0
-# HELP pkg_broken Broken packages per origin
-# TYPE pkg_broken gauge
-pkg_broken{archive="focal-updates",component="main",label="Ubuntu",origin="Ubuntu",site="ftp.fau.de",trusted="True"} 0.0
-
-```
-
-## Contributing
-
-Feel free to contribute improvements, as well as support for non-apt based systems.
-
-## Installation
-
-### Global pip installation
-Run `pip3 install pkg-exporter`.
-
-### Install from source
-Clone the repository and run `poetry install` from the main directory.
-You can also use other standard installation methods for python packages, like directly installing from this git repository.
-
-The pyinstaller-based binary is not provided any more.
-
-### pipx
-If a global pip installation is not possible (e.g. from debian 12 onwards), you can use [pipx](https://pypa.github.io/pipx), either for install, and/or for running pkg-exporter ad hoc:
-```
-pipx run --system-site-packages pkg-exporter
-```
-
-`--system-site-packages` is necessary to provide access to the system python3-apt lib.
-
-### apt-based systems
-
-Currently, only apt-based systems are supported. `python3-apt` needs to be installed on the system.
-
-## Configuration and Usage
-
-The node exporter needs to be configured for textfiles using the `--collector.textfile.directory` option. This exporter needs to write the exported metrics into this directory. 
-
-The default path is `/var/prometheus/pkg-exporter.prom`, and may be changed via the `PKG_EXPORTER_FILE`-Environment Variable.
-If the directory is not already present, it will be created by the exporter.
-
-The command `pkg_exporter` provided by the package or the binary shall be executed in a appropriate interval, e.g. using cron or systemd timers.
-The exporter needs to be executed with appropriate privileges, which are not necessarily root privileges.
-
-An example configuration will be provided in this repository in the future.
-
-### apt hook
-To enable monitoring for apt update calls, place the file under `docs/00-pve-exporter` in `/etc/apt/apt.conf.d` on your system.
-It will place files under `/tmp`. To customize the filepath of the timestamp files, the the environment variables `PKG_EXPORTER_APT_PRE_FILE` & `PKG_EXPORTER_APT_POST_FILE` may be used.
-You can see the success of monitoring the apt update timestamps if the following metric is 1: `pkg_update_time_available 1.0`
-
-Please not that the presence of an timestamp does not mean that all repositories were updated without issues.
-
-## Alerting
-
-Example alerting rules will be provided in the future.
-
-## Roadmap
-
-- Support for other pkg managers
-- Deployment as dpkg-Packet
 
+setup(**setup_kwargs)
```

