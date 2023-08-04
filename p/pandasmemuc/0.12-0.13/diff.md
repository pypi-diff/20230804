# Comparing `tmp/pandasmemuc-0.12.tar.gz` & `tmp/pandasmemuc-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasmemuc-0.12.tar", last modified: Thu Aug  3 19:44:03 2023, max compression
+gzip compressed data, was "pandasmemuc-0.13.tar", last modified: Thu Aug  3 21:14:48 2023, max compression
```

## Comparing `pandasmemuc-0.12.tar` & `pandasmemuc-0.13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 19:44:03.231665 pandasmemuc-0.12/
--rw-rw-rw-   0        0        0     1148 2023-08-03 19:43:45.000000 pandasmemuc-0.12/LICENSE.rst
--rw-rw-rw-   0        0        0      104 2023-08-03 19:43:43.000000 pandasmemuc-0.12/MANIFEST.in
--rw-rw-rw-   0        0        0     2347 2023-08-03 19:44:03.231665 pandasmemuc-0.12/PKG-INFO
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 19:44:03.228736 pandasmemuc-0.12/pandasmemuc/
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.12/pandasmemuc/README.MD
--rw-rw-rw-   0        0        0   101447 2023-08-03 19:32:09.000000 pandasmemuc-0.12/pandasmemuc/__init__.py
--rw-rw-rw-   0        0        0      177 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc/requirements.txt
--rw-rw-rw-   0        0        0    35393 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-08-03 19:44:03.231665 pandasmemuc-0.12/pandasmemuc.egg-info/
--rw-rw-rw-   0        0        0     2347 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-08-03 19:44:03.000000 pandasmemuc-0.12/pandasmemuc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-08-03 19:44:03.233616 pandasmemuc-0.12/setup.cfg
--rw-rw-rw-   0        0        0     1656 2023-08-03 19:44:02.000000 pandasmemuc-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:14:48.801311 pandasmemuc-0.13/
+-rw-rw-rw-   0        0        0     1148 2023-08-03 21:14:24.000000 pandasmemuc-0.13/LICENSE.rst
+-rw-rw-rw-   0        0        0      104 2023-08-03 21:14:23.000000 pandasmemuc-0.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     2347 2023-08-03 21:14:48.801311 pandasmemuc-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 21:14:48.797322 pandasmemuc-0.13/pandasmemuc/
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.13/pandasmemuc/README.MD
+-rw-rw-rw-   0        0        0   102152 2023-08-03 21:02:57.000000 pandasmemuc-0.13/pandasmemuc/__init__.py
+-rw-rw-rw-   0        0        0      177 2023-08-03 21:14:47.000000 pandasmemuc-0.13/pandasmemuc/requirements.txt
+-rw-rw-rw-   0        0        0    35393 2023-08-03 21:14:47.000000 pandasmemuc-0.13/pandasmemuc/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-08-03 21:14:48.800314 pandasmemuc-0.13/pandasmemuc.egg-info/
+-rw-rw-rw-   0        0        0     2347 2023-08-03 21:14:48.000000 pandasmemuc-0.13/pandasmemuc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-08-03 21:14:48.000000 pandasmemuc-0.13/pandasmemuc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 21:14:48.000000 pandasmemuc-0.13/pandasmemuc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-08-03 21:14:48.000000 pandasmemuc-0.13/pandasmemuc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 21:14:48.000000 pandasmemuc-0.13/pandasmemuc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-08-03 21:14:48.802309 pandasmemuc-0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1656 2023-08-03 21:14:47.000000 pandasmemuc-0.13/setup.py
```

### Comparing `pandasmemuc-0.12/LICENSE.rst` & `pandasmemuc-0.13/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.12/PKG-INFO` & `pandasmemuc-0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.12
+Version: 0.13
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.12/README.md` & `pandasmemuc-0.13/README.md`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.12/pandasmemuc/README.MD` & `pandasmemuc-0.13/pandasmemuc/README.MD`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.12/pandasmemuc/__init__.py` & `pandasmemuc-0.13/pandasmemuc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,58 +61,74 @@
         tempfolder.name,
     )
 
 
 def get_hosts_files(
     allhosts=(
         "https://adaway.org/hosts.txt",
-        "https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts",
-        "https://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext",
-        "https://winhelp2002.mvps.org/hosts.txt",
+        # "https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts",
+        # "https://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext",
+        # "https://winhelp2002.mvps.org/hosts.txt",
     )
 ):
+    if not isiter(allhosts):
+        allhosts = [allhosts]
     allurls = []
     for url in allhosts:
-        try:
-            resp = requests.get(url)
+        if os.path.exists(url):
+            with open(url,mode='r',encoding='utf-8') as f:
+                allurls.extend(
+                    [
+                        tuple(x.strip().split(maxsplit=1))
+                        for x in f.read().splitlines()
+                        if x and x[0] != "#"
+                    ]
+                )
+        else:
+            try:
+                resp = requests.get(url)
 
-            allurls.extend(
-                [
-                    tuple(x.strip().split(maxsplit=1))
-                    for x in resp.content.decode("utf-8").splitlines()
-                    if x and x[0] != "#"
-                ]
-            )
-        except Exception as fe:
-            print(fe)
-            continue
-    df = pd.DataFrame(sorted(list(set(allurls))))
-    df = df.loc[df[0] == "0.0.0.0"]
-    df = df.drop(df.loc[(df[0] == "0.0.0.0") & (df[1] == "0.0.0.0")].index[0])
-
-    newhostheader = """
-    127.0.0.1 localhost
-    127.0.0.1 localhost.localdomain
-    127.0.0.1 local
-    255.255.255.255 broadcasthost
-    ::1 localhost
-    ::1 ip6-localhost
-    ::1 ip6-loopback
-    fe80::1%lo0 localhost
-    ff00::0 ip6-localnet
-    ff00::0 ip6-mcastprefix
-    ff02::1 ip6-allnodes
-    ff02::2 ip6-allrouters
-    ff02::3 ip6-allhosts
-    0.0.0.0 0.0.0.0""".strip()
+                allurls.extend(
+                    [
+                        tuple(x.strip().split(maxsplit=1))
+                        for x in resp.content.decode("utf-8").splitlines()
+                        if x and x[0] != "#"
+                    ]
+                )
+            except Exception as fe:
+                print(fe)
+                continue
+    if len(allhosts) > 1:
 
-    newhost = "\n".join(
-        [x[0] + " " + x[1] for x in zip(df[0].to_list(), df[1].to_list())]
-    )
-    newhost = newhostheader + "\n" + newhost
+        df = pd.DataFrame(sorted(list(set(allurls))))
+        df = df.loc[(df[0] == "0.0.0.0") | (df[0] == "127.0.0.1")]
+        df = df.drop(df.loc[(df[0] == "0.0.0.0") & (df[1] == "0.0.0.0")].index[0])
+
+        newhostheader = """
+        127.0.0.1 localhost
+        127.0.0.1 localhost.localdomain
+        127.0.0.1 local
+        255.255.255.255 broadcasthost
+        ::1 localhost
+        ::1 ip6-localhost
+        ::1 ip6-loopback
+        fe80::1%lo0 localhost
+        ff00::0 ip6-localnet
+        ff00::0 ip6-mcastprefix
+        ff02::1 ip6-allnodes
+        ff02::2 ip6-allrouters
+        ff02::3 ip6-allhosts
+        0.0.0.0 0.0.0.0""".strip()
+
+        newhost = "\n".join(
+            [x[0] + " " + x[1] for x in zip(df[0].to_list(), df[1].to_list())]
+        )
+        newhost = newhostheader + "\n" + newhost
+    else:
+        newhost = '\n'.join([' '.join(list(x)) for x in allurls])
     fo = tempfolder_and_files(fileprefix="", numberoffiles=0, suffix="", zfill=0)[-1]
     if not os.path.exists(fo):
         os.makedirs(fo)
     hostfile = os.path.normpath(os.path.join(fo, "hosts"))
     with open(hostfile, "w", newline="\n", encoding="utf-8") as f:
         f.write(newhost)
     return hostfile
```

### Comparing `pandasmemuc-0.12/pandasmemuc/thirdparty.json` & `pandasmemuc-0.13/pandasmemuc/thirdparty.json`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.12/pandasmemuc.egg-info/PKG-INFO` & `pandasmemuc-0.13/pandasmemuc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.12
+Version: 0.13
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.12/setup.py` & `pandasmemuc-0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.12'''
+VERSION = '''0.13'''
 DESCRIPTION = '''Automating memu emulator with pandas'''
 
 # Setting up
 setup(
     name="pandasmemuc",
     version=VERSION,
     license='MIT',
```

