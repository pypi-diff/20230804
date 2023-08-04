# Comparing `tmp/ptsecurixt-0.0.2.tar.gz` & `tmp/ptsecurixt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsecurixt-0.0.2.tar", last modified: Mon Mar 28 16:57:22 2022, max compression
+gzip compressed data, was "ptsecurixt-1.0.0.tar", last modified: Fri Aug  4 11:48:41 2023, max compression
```

## Comparing `ptsecurixt-0.0.2.tar` & `ptsecurixt-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:57:22.978203 ptsecurixt-0.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2021-12-17 14:07:30.000000 ptsecurixt-0.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     2272 2022-03-28 16:57:22.978203 ptsecurixt-0.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1901 2022-03-28 16:57:10.000000 ptsecurixt-0.0.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:57:22.974205 ptsecurixt-0.0.2/ptsecurixt/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2021-12-17 14:07:30.000000 ptsecurixt-0.0.2/ptsecurixt/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5881 2022-03-28 16:57:16.000000 ptsecurixt-0.0.2/ptsecurixt/ptsecurixt.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:57:22.974205 ptsecurixt-0.0.2/ptsecurixt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2272 2022-03-28 16:57:22.000000 ptsecurixt-0.0.2/ptsecurixt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      280 2022-03-28 16:57:22.000000 ptsecurixt-0.0.2/ptsecurixt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-03-28 16:57:22.000000 ptsecurixt-0.0.2/ptsecurixt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       59 2022-03-28 16:57:22.000000 ptsecurixt-0.0.2/ptsecurixt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       23 2022-03-28 16:57:22.000000 ptsecurixt-0.0.2/ptsecurixt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2022-03-28 16:57:22.000000 ptsecurixt-0.0.2/ptsecurixt.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2022-03-28 16:57:22.978203 ptsecurixt-0.0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      824 2022-03-28 16:57:04.000000 ptsecurixt-0.0.2/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:48:41.634340 ptsecurixt-1.0.0/
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)    35823 2023-01-11 20:44:27.000000 ptsecurixt-1.0.0/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3291 2023-08-04 11:48:41.634340 ptsecurixt-1.0.0/PKG-INFO
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)     2832 2023-04-13 09:14:10.000000 ptsecurixt-1.0.0/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:48:41.634340 ptsecurixt-1.0.0/ptsecurixt/
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)        0 2023-01-11 20:44:27.000000 ptsecurixt-1.0.0/ptsecurixt/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-04-13 08:06:37.000000 ptsecurixt-1.0.0/ptsecurixt/_version.py
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)     6957 2023-04-18 10:15:21.000000 ptsecurixt-1.0.0/ptsecurixt/ptsecurixt.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:48:41.634340 ptsecurixt-1.0.0/ptsecurixt.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3291 2023-08-04 11:48:41.000000 ptsecurixt-1.0.0/ptsecurixt.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      303 2023-08-04 11:48:41.000000 ptsecurixt-1.0.0/ptsecurixt.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-04 11:48:41.000000 ptsecurixt-1.0.0/ptsecurixt.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2023-08-04 11:48:41.000000 ptsecurixt-1.0.0/ptsecurixt.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       22 2023-08-04 11:48:41.000000 ptsecurixt-1.0.0/ptsecurixt.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       11 2023-08-04 11:48:41.000000 ptsecurixt-1.0.0/ptsecurixt.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-04 11:48:41.634340 ptsecurixt-1.0.0/setup.cfg
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)     1009 2023-04-13 08:58:53.000000 ptsecurixt-1.0.0/setup.py
```

### Comparing `ptsecurixt-0.0.2/LICENSE` & `ptsecurixt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptsecurixt-0.0.2/PKG-INFO` & `ptsecurixt-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,86 @@
-Metadata-Version: 2.1
-Name: ptsecurixt
-Version: 0.0.2
-Summary: security.txt finder
-Home-page: https://www.penterep.com/
-Author: Penterep
-Author-email: info@penterep.com
-License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Environment :: Console
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
-
-# PTSECURIXT
-
-Script searches for **security.txt** file in known locations
-
-## Installation
-
-```
-pip install ptsecurixt
-```
-
-## Usage examples
-```
-ptsecurixt -u htttps://www.example.com/
-```
-
-## Options
-```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--H   --headers     <header:value>  Set custom header(s)
--ua  --user-agent  <ua>            Set User-Agent header
--c   --cookie      <cookie>        Set cookie
--j   --json                        Output in JSON format
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
-```
-
-
-## Dependencies
-   - requests
-   - ptlibs
-
-## Version History
-
-- 0.0.1 - 0.0.2
-    - Alpha releases
-
-## Licence
-
-Copyright (c) 2020 HACKER Consulting s.r.o.
-
-ptsecurixt is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-
-ptsecurixt is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with ptsecurixt. If not, see https://www.gnu.org/licenses/.
-
-## Warning
-
-You are only allowed to run the tool against the websites which
-you have been given permission to pentest. We do not accept any
-responsibility for any damage/harm that this application causes to your
-computer, or your network. Penterep is not responsible for any illegal
-or malicious use of this code. Be Ethical!
-
+![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+
+
+# PTSECURIXT
+![PyPI - License](https://img.shields.io/pypi/l/ptsecurixt?style=for-the-badge)
+![Platform](https://img.shields.io/badge/KaliLinux-2023.1-orange?style=for-the-badge)
+
+
+> security.txt finder
+
+ptsecurixt is a tool that searches for **security.txt** file in known locations.
+
+## Installation
+
+```
+pip install ptsecurixt
+```
+
+## Add to PATH
+If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
+source ~/.bashrc
+```
+
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
+## Usage examples
+```
+ptsecurixt -u htttps://www.example.com/
+```
+
+## Options
+```
+-u   --url         <url>           Connect to URL
+-p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout                     Set timeout for HTTP requests
+-c   --cookie      <cookie>        Set cookie
+-ua  --user-agent  <ua>            Set User-Agent header
+-H   --headers     <header:value>  Set custom header(s)
+-r   --redirects                   Follow redirects (default False)
+-C   --cache                       Cache HTTP communication (load from tmp in future)
+-j   --json                        Output in JSON format
+-v   --version                     Show script version and exit
+-h   --help                        Show this help message and exit
+```
+
+## Dependencies
+```
+requests
+ptlibs
+```
+
+## Version History
+```
+1.0.0
+    - Release ready
+0.0.4
+    - Refactored for latest ptlibs
+0.0.1 - 0.0.3
+    - Alpha releases
+```
+
+## License
+
+Copyright (c) 2023 Penterep Security s.r.o.
+
+ptsecurixt is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+ptsecurixt is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with ptsecurixt. If not, see https://www.gnu.org/licenses/.
+
+## Warning
+
+You are only allowed to run the tool against the websites which
+you have been given permission to pentest. We do not accept any
+responsibility for any damage/harm that this application causes to your
+computer, or your network. Penterep is not responsible for any illegal
+or malicious use of this code. Be Ethical!
```

### Comparing `ptsecurixt-0.0.2/ptsecurixt.egg-info/PKG-INFO` & `ptsecurixt-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,103 @@
 Metadata-Version: 2.1
 Name: ptsecurixt
-Version: 0.0.2
+Version: 1.0.0
 Summary: security.txt finder
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
 
+
 # PTSECURIXT
+![PyPI - License](https://img.shields.io/pypi/l/ptsecurixt?style=for-the-badge)
+![Platform](https://img.shields.io/badge/KaliLinux-2023.1-orange?style=for-the-badge)
+
+
+> security.txt finder
 
-Script searches for **security.txt** file in known locations
+ptsecurixt is a tool that searches for **security.txt** file in known locations.
 
 ## Installation
 
 ```
 pip install ptsecurixt
 ```
 
+## Add to PATH
+If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
+source ~/.bashrc
+```
+
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
 ## Usage examples
 ```
 ptsecurixt -u htttps://www.example.com/
 ```
 
 ## Options
 ```
 -u   --url         <url>           Connect to URL
 -p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--H   --headers     <header:value>  Set custom header(s)
--ua  --user-agent  <ua>            Set User-Agent header
+-T   --timeout                     Set timeout for HTTP requests
 -c   --cookie      <cookie>        Set cookie
+-ua  --user-agent  <ua>            Set User-Agent header
+-H   --headers     <header:value>  Set custom header(s)
+-r   --redirects                   Follow redirects (default False)
+-C   --cache                       Cache HTTP communication (load from tmp in future)
 -j   --json                        Output in JSON format
 -v   --version                     Show script version and exit
 -h   --help                        Show this help message and exit
 ```
 
-
 ## Dependencies
-   - requests
-   - ptlibs
+```
+requests
+ptlibs
+```
 
 ## Version History
-
-- 0.0.1 - 0.0.2
+```
+1.0.0
+    - Release ready
+0.0.4
+    - Refactored for latest ptlibs
+0.0.1 - 0.0.3
     - Alpha releases
+```
 
-## Licence
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptsecurixt is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptsecurixt is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptsecurixt. If not, see https://www.gnu.org/licenses/.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptsecurixt-0.0.2/setup.py` & `ptsecurixt-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import setuptools
+from ptsecurixt._version import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ptsecurixt",
-    version="0.0.2",
+    version=__version__,
     description="security.txt finder",
     author="Penterep",
     author_email="info@penterep.com",
     url="https://www.penterep.com/",
     license="GPLv3+",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Environment :: Console"
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Environment :: Console",
+        "Topic :: Security",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
     ],
     python_requires='>=3.6',
-    install_requires=["ptlibs>=0.0.6", "requests"],
+    install_requires=["ptlibs>=1,<2", "requests"],
     entry_points = {'console_scripts': ['ptsecurixt = ptsecurixt.ptsecurixt:main']},
     include_package_data= True,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

