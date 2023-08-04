# Comparing `tmp/DependiPy-1.0.9.tar.gz` & `tmp/DependiPy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DependiPy-1.0.9.tar", last modified: Wed Aug  2 12:33:48 2023, max compression
+gzip compressed data, was "DependiPy-1.1.0.tar", last modified: Fri Aug  4 09:09:59 2023, max compression
```

## Comparing `DependiPy-1.0.9.tar` & `DependiPy-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:33:48.134312 DependiPy-1.0.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:33:48.130312 DependiPy-1.0.9/DependiPy/
--rw-r--r--   0 root         (0) root         (0)       68 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21373 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/archive.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/librarian.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-08-02 12:33:47.000000 DependiPy-1.0.9/DependiPy/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:33:48.134312 DependiPy-1.0.9/DependiPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11507 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-08-02 12:33:48.000000 DependiPy-1.0.9/DependiPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1065 2023-08-02 12:33:47.000000 DependiPy-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11507 2023-08-02 12:33:48.134312 DependiPy-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11287 2023-08-02 12:33:47.000000 DependiPy-1.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 12:33:48.134312 DependiPy-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      921 2023-08-02 12:33:47.000000 DependiPy-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:09:59.887140 DependiPy-1.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:09:59.887140 DependiPy-1.1.0/DependiPy/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22055 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy/archive.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy/librarian.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:09:59.887140 DependiPy-1.1.0/DependiPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-04 09:09:59.000000 DependiPy-1.1.0/DependiPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-04 09:09:59.000000 DependiPy-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-08-04 09:09:59.887140 DependiPy-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11632 2023-08-04 09:09:59.000000 DependiPy-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 09:09:59.887140 DependiPy-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      921 2023-08-04 09:09:59.000000 DependiPy-1.1.0/setup.py
```

### Comparing `DependiPy-1.0.9/DependiPy/archive.py` & `DependiPy-1.1.0/DependiPy/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import numpy as np
 from tqdm import tqdm
 import pkg_resources
 
 
 class LibMapperTools:
 
-    def __init__(self, lib_name, remove, replace_dict, exclusion, librerie_private=None, mode='lib'):
+    def __init__(self, lib_name, remove, replace_dict, exclusion, force_version, librerie_private=None, mode='lib'):
         self.lib_name = lib_name
         self.remove = remove
         self.replace_dict = replace_dict
         self.exclusion = exclusion
+        self.force_version = force_version
         self.number_of_levels = 0
         self.librerie_private = librerie_private
         self.mode = mode
 
         # lista di colonne, serve per il codice
         self.saved_columns = ['file', 'req', 'path']
 
@@ -44,15 +45,15 @@
                             with open(dirpath + "/" + file, "r") as f:
                                 contents = f.read()
                             # il contenuto del file viene madato alla funzione che ne estrae le librerie
                             req = self.books_extraction(contents)
                             req_temp.loc[req_temp.index[i], 'file'] = file
                             req_temp.loc[req_temp.index[i], 'req'] = req
                         except:
-                            print(file, 'impossible to read')
+                            print(f'{file} is impossible to read')
                 # viene popolato un dataframe comune a tutti i file
                 df = pd.concat([df, req_temp], ignore_index=True)
                 # se un file non viene considerato perche non ha il .py con il drop viene eliminata la sua riga
                 df = df.dropna(subset=['file'])
 
         # si ottiene il numero di livelli di profondita della classe
         number_of_levels = df.columns.difference(self.saved_columns).shape[0]
@@ -237,24 +238,24 @@
         # tutti i requirements vengono messi in un unico dataframe
         res = pd.concat([res, df.loc[:, ['path', 'req']]], ignore_index=True).sort_values(by=['path'])
         return res
 
     def write_mapping(self, df, **kwargs):
 
         # per poter scrivere i requisiti nel posto giusto si riporta la posizione di lavoro nel punto di partenza se in modalita script
-        if kwargs['mode'] == 'script': os.chdir(self.lib_name)
+        if self.mode == 'script': os.chdir(self.lib_name)
 
         # vengono trovate tutte le librerie usate nel progetto
         single_requirements = set([item for sublist in df['req'].tolist() for item in sublist])
 
         distribusion_not_found, requirements_variable, requirements_versioned, _ = self.clean_from_python_packages(single_requirements)
 
         print(f'list of distribution not found: {distribusion_not_found}')
 
-        if 'docs_only' in kwargs and kwargs.get('docs_only') == False or 'docs_only' not in kwargs:
+        if ('docs_only' in kwargs and kwargs.get('docs_only') == False) or 'docs_only' not in kwargs:
             # viene scritto il file dei requisiti
             with open("requirements.txt", "w") as f:
                 for s in requirements_versioned:
                     f.write(s + "\n")
 
         ###############################
         # da aggiungere la parte che costruisce la documentazione
@@ -269,25 +270,26 @@
                 contents_yml = f.readlines()
 
             for i in range(len(contents_yml)):
                 contents_yml[i] = contents_yml[i].split('\n')[0]
 
             # se sono presenti i marker per riscrivere le librerie vengono usati
             api_is_here = True
-            try:
-                if '  - API:' in contents_yml:
-                    yml_start = contents_yml.index('  - API:') + 1
-                    yml_stop = contents_yml[yml_start:].index('') + yml_start
-                else:
-                    yml_start = contents_yml.index('nav:') + 1
-                    yml_start = contents_yml[yml_start:].index('') + yml_start
-                    yml_stop = contents_yml[yml_start:].index('') + yml_start + 1
-                    api_is_here = False
-            except:
-                raise ValueError('missing version tag in the setup.py')
+            if '  - API:' in contents_yml:
+                yml_start = contents_yml.index('  - API:') + 1
+                yml_stop = contents_yml[yml_start:].index('') + yml_start
+            elif 'nav:' in contents_yml:
+                yml_start = contents_yml.index('nav:') + 1
+                yml_start = contents_yml[yml_start:].index('') + yml_start
+                yml_stop = contents_yml[yml_start:].index('') + yml_start + 1
+                api_is_here = False
+            else:
+                yml_start, yml_stop = 0, 0
+                print('missing the proper tag in the mkdocs.yml')
+                exit()
 
             #######################################################################################
             docs = []
             temp_to_add = None
             for i in range(df.shape[0]):
                 if df.loc[df.index[i], f'file'] != "__init__.py":
                     valid_col = df.loc[df.index[i], [f'level_{j}' for j in range(self.number_of_levels)]].notnull().sum() - 1
@@ -311,15 +313,15 @@
             contents_yml[yml_start:yml_start+1] = docs
 
             with open("mkdocs.yml", "w") as f:
                 for s in contents_yml:
                     f.write(str(s) + "\n")
 
         ###############################
-        if 'docs_only' in kwargs and kwargs.get('docs_only') == False or 'docs_only' not in kwargs:
+        if ('docs_only' in kwargs and kwargs.get('docs_only') == False) or 'docs_only' not in kwargs:
 
             if self.mode == 'script':
                 list_privat_reference = ['[' for _ in range(len(self.librerie_private))]
 
                 for ele in single_requirements:
                     if ele != 'waste':
                         for i, lib in enumerate(self.librerie_private):
@@ -346,57 +348,59 @@
                 with open("setup.py", "r") as f:
                     contents = f.readlines()
 
                 for i in range(len(contents)):
                     contents[i] = contents[i].split('\n')[0]
 
                 # controllare se ci sono gli star e end
-
                 # se sono presenti i marker per riscrivere le librerie vengono usati
-                try:
+                if '# version go' in contents and '# version end' in contents:
                     vers_start = contents.index('# version go') + 1
                     vers_stop = contents.index('# version end')
-                except:
-                    raise ValueError('missing version tag in the setup.py')
+                else:
+                    vers_start, vers_stop = 0, 0
+                    print('missing version go/end tag')
+                    exit()
 
                 # vengono eliminate le librerie dentro i marker
                 del contents[vers_start: vers_stop]
 
                 # venogono aggiunte le nuove librerie alla lista da scrivere sul file
                 contents[vers_start:vers_start] = requirements_variable
 
-                try:
+                if '# start' in contents and '# stop' in contents:
                     start = contents.index('# start')
                     stop = contents.index('# stop')
-                except:
-                    raise ValueError('missing version tag in the setup.py')
 
-                packets = ['' for _ in range(df.shape[0])]
-                for i in range(df.shape[0]):
-                    packets[i] += f"'{df.loc[df.index[i], 'original']}': ["
-
-                    _, _, _, eles = self.clean_from_python_packages(df.loc[df.index[i], "req"])
-
-                    j = 0
-                    for ele in eles:
-                        if ele != 'waste':
-                            if j == 0:
-                                packets[i] += f'{ele}'
-                            else:
-                                packets[i] += f', {ele}'
-                            j += 1
-                    packets[i] += '],'
-
-                packets = ['requires_dict = {'] + packets
-                packets = packets + ['}']
-
-                new_set_up = ['' for _ in range(start+len(contents)-stop+len(packets))]
-                new_set_up[:start+1] = contents[:start+1]
-                new_set_up[start+1:len(packets)+1] = packets
-                new_set_up[start+1+len(packets):] = contents[stop:]
+                    packets = ['' for _ in range(df.shape[0])]
+                    for i in range(df.shape[0]):
+                        packets[i] += f"'{df.loc[df.index[i], 'original']}': ["
+
+                        _, _, _, eles = self.clean_from_python_packages(df.loc[df.index[i], "req"])
+
+                        j = 0
+                        for ele in eles:
+                            if ele != 'waste':
+                                if j == 0:
+                                    packets[i] += f'{ele}'
+                                else:
+                                    packets[i] += f', {ele}'
+                                j += 1
+                        packets[i] += '],'
+
+                    packets = ['requires_dict = {'] + packets
+                    packets = packets + ['}']
+
+                    new_set_up = ['' for _ in range(start+len(contents)-stop+len(packets))]
+                    new_set_up[:start+1] = contents[:start+1]
+                    new_set_up[start+1:len(packets)+1] = packets
+                    new_set_up[start+1+len(packets):] = contents[stop:]
+                else:
+                    print('missing version start/stop tag')
+                    new_set_up = contents
 
                 with open("setup.py", "w") as f:
                     for s in new_set_up:
                         f.write(str(s) + "\n")
 
                 print(os.getcwd()+"\\setup.py")
 
@@ -417,13 +421,16 @@
                     break
 
             if pass_card:
                 req_list = self.replace_dict[req] if req in self.replace_dict else [req]
                 for req_i in req_list:
                     try:
                         version = pkg_resources.get_distribution(req_i).version
-                        requirements_versioned.append(f'{req_i}=={version}')
-                        requirements_variable.append(f"{req_i.replace('-', '_')} = '{req_i}=={version}'")
+                        # se il pacchetto e' presente nella lista dei pacchetti di cui forzare la versione, viene usata la versione preimpostata
+                        # in caso contrario viene usata la versione di sistema
+                        version_str = self.force_version[req_i] if req_i in self.force_version else f'{req_i}=={version}'
+                        requirements_versioned.append(version_str)
+                        requirements_variable.append(f"{req_i.replace('-', '_')} = '{version_str}'")
                         variables.append(f"{req_i.replace('-', '_')}")
                     except pkg_resources.DistributionNotFound:
                         distribusion_not_found.append(req_i)
         return distribusion_not_found, requirements_variable, requirements_versioned, variables
```

### Comparing `DependiPy-1.0.9/DependiPy/librarian.py` & `DependiPy-1.1.0/DependiPy/librarian.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     print("privat libraries: ", librerie_private)
     # nome delle cartelle da non considerare per la mappatura
     exclusion = config.get('exclude_folder', [])
     # lista di librerie aggiuntive che non si vuole inseire nei requirements se fossero presenti
     remove = config.get('exclude_lib', [])
     # dizionario per sostituire alcuni nomi se serve
     replace_dict = config.get('replace_lib', {})
+    # lista di librerie di cui si vuole forzare la versione
+    force_version = config.get('force_version', {})
 
     # percorso della libreria
     path = kwargs['path']
     os.chdir(path)
     os.chdir('..')
     # nome della cartella che contiene la libreria, rappresenta il livello 0
     lib_name = os.path.normpath(path).split('\\')
@@ -41,17 +43,18 @@
         lib_name = lib_name[-2]
     else:
         lib_name = lib_name[-1]
 
     # se trovo il file setup.py e non ho un mode dagli argomenti passati allora imposto mode come lib
     mode = 'lib' if os.path.exists('setup.py') else 'script'
     mode = kwargs['mode'] if kwargs['mode'] is not None else mode
+    print(f'selected mode: {mode}')
 
     lmt = LibMapperTools(lib_name=lib_name, remove=remove, replace_dict=replace_dict, exclusion=exclusion,
-                         librerie_private=librerie_private, mode=mode)
+                         force_version=force_version, librerie_private=librerie_private, mode=mode)
 
     requirements_pd = lmt.read_files()
 
     requirements_pd = lmt.add_path(requirements_pd)
 
     # applico la funzione che estrae le cross reference e la applico alla colonna delle librerie
     requirements_pd.loc[:, 'cross'] = requirements_pd.loc[:, 'req'].apply(lmt.cross_reference_extraction)
```

### Comparing `DependiPy-1.0.9/DependiPy.egg-info/PKG-INFO` & `DependiPy-1.1.0/DependiPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DependiPy
-Version: 1.0.9
+Version: 1.1.0
 Home-page: https://github.com/ajacassi/DependiPy.git
 Author: Andrea Jacassi
 Author-email: 
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -52,21 +52,23 @@
       "azure-core",
       "azure-identity",
       "azure-mgmt-consumption",
       "azure-mgmt-core",
       "azure-mgmt-costmanagement"
     ]},
   "exclude_lib": ["tensorflow", "setuptools"],
-  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"]
+  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"],
+  "force_version": {"pandas": "pandas==1.1.1", "numpy": "numpy"}
 }
 ```
 - **privat_lib**: sono le librerie private usate che non sono presenti su PyPi e che quindi non devono essere listate in un file di requirements, non potendo essere installate in automatico
 - **replace_lib**: sono le parole che devono essere sostituite nella ricerca delle librerie, dato che alcune librerie usano nomi diversi negli import dalle release su PyPi
 - **exclude_lib**: librerie che sono presenti nei file ma che non si vuole che vengano riportate
 - **exclude_folder**: cartelle che non devono essere considerate durante lo scan delle dipendenze
+- **force_version** sono le librerie di cui si vuole forzare una versione, viene usato un formato a dizionario dove la chiave e' la libreria identificata e il valore e' la stringa che si vuole usare dei requirements, si puo mettere una versione specifica o inserire solo il nome per non segnalare nessuna versione
 
 **Le librerie inserite nel requirements.txt sono sempre e solo quelle che devono essere installate, per cui non verranno mai riportate le dipendenze native di Python**
 
 ## lib/setup.py
 Se si sta lavorando in modalita lib, libraria produce un file alla fine della mappatura.
 Se il setup.py ha la forma seguente:
 ```python
@@ -106,18 +108,18 @@
 # stop
 
 setup(
     name='utilities',
     version=version,
     packages=find_packages(include=['utilities']),
     license='',
-    author='Andrea Jacassi',
+    author='John Do',
     author_email='',
     description='',
-    url="https://github.com/utilities.git",
+    url="https://github.com/rep.git",
     extras_require=requires_dict,
     install_requires=[],
 )
 ```
 Sono necessarie le seguenti chiavi nel setup.py: **# start**, uno **# stop**, uno **# version go** e uno **# version end**.
 Librarian andra a scrivere la mappatura direttamente nel setup.py.
 
@@ -227,29 +229,29 @@
           accent: lime
     
     repo_name: name repository github
     repo_url: url repository github
     
     plugins:
       - mkdocstrings
-        - search
+      - search
     
     markdown_extensions:
       - pymdownx.highlight:
           anchor_linenums: true
-        - pymdownx.inlinehilite
-        - pymdownx.snippets
-        - admonition
-        - pymdownx.arithmatex:
-            generic: true
-        - footnotes
-        - pymdownx.details
-        - pymdownx.superfences
-        - pymdownx.mark
-        - attr_list
+      - pymdownx.inlinehilite
+      - pymdownx.snippets
+      - admonition
+      - pymdownx.arithmatex:
+          generic: true
+      - footnotes
+      - pymdownx.details
+      - pymdownx.superfences
+      - pymdownx.mark
+      - attr_list
     
     nav:
       - index.md
       - Installation: installation.md
       - User Guide: user_guide.md
       - Developer Guide: dev_guide.md
       - XA information: info.md
```

### Comparing `DependiPy-1.0.9/LICENSE` & `DependiPy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DependiPy-1.0.9/PKG-INFO` & `DependiPy-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DependiPy
-Version: 1.0.9
+Version: 1.1.0
 Home-page: https://github.com/ajacassi/DependiPy.git
 Author: Andrea Jacassi
 Author-email: 
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -52,21 +52,23 @@
       "azure-core",
       "azure-identity",
       "azure-mgmt-consumption",
       "azure-mgmt-core",
       "azure-mgmt-costmanagement"
     ]},
   "exclude_lib": ["tensorflow", "setuptools"],
-  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"]
+  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"],
+  "force_version": {"pandas": "pandas==1.1.1", "numpy": "numpy"}
 }
 ```
 - **privat_lib**: sono le librerie private usate che non sono presenti su PyPi e che quindi non devono essere listate in un file di requirements, non potendo essere installate in automatico
 - **replace_lib**: sono le parole che devono essere sostituite nella ricerca delle librerie, dato che alcune librerie usano nomi diversi negli import dalle release su PyPi
 - **exclude_lib**: librerie che sono presenti nei file ma che non si vuole che vengano riportate
 - **exclude_folder**: cartelle che non devono essere considerate durante lo scan delle dipendenze
+- **force_version** sono le librerie di cui si vuole forzare una versione, viene usato un formato a dizionario dove la chiave e' la libreria identificata e il valore e' la stringa che si vuole usare dei requirements, si puo mettere una versione specifica o inserire solo il nome per non segnalare nessuna versione
 
 **Le librerie inserite nel requirements.txt sono sempre e solo quelle che devono essere installate, per cui non verranno mai riportate le dipendenze native di Python**
 
 ## lib/setup.py
 Se si sta lavorando in modalita lib, libraria produce un file alla fine della mappatura.
 Se il setup.py ha la forma seguente:
 ```python
@@ -106,18 +108,18 @@
 # stop
 
 setup(
     name='utilities',
     version=version,
     packages=find_packages(include=['utilities']),
     license='',
-    author='Andrea Jacassi',
+    author='John Do',
     author_email='',
     description='',
-    url="https://github.com/utilities.git",
+    url="https://github.com/rep.git",
     extras_require=requires_dict,
     install_requires=[],
 )
 ```
 Sono necessarie le seguenti chiavi nel setup.py: **# start**, uno **# stop**, uno **# version go** e uno **# version end**.
 Librarian andra a scrivere la mappatura direttamente nel setup.py.
 
@@ -227,29 +229,29 @@
           accent: lime
     
     repo_name: name repository github
     repo_url: url repository github
     
     plugins:
       - mkdocstrings
-        - search
+      - search
     
     markdown_extensions:
       - pymdownx.highlight:
           anchor_linenums: true
-        - pymdownx.inlinehilite
-        - pymdownx.snippets
-        - admonition
-        - pymdownx.arithmatex:
-            generic: true
-        - footnotes
-        - pymdownx.details
-        - pymdownx.superfences
-        - pymdownx.mark
-        - attr_list
+      - pymdownx.inlinehilite
+      - pymdownx.snippets
+      - admonition
+      - pymdownx.arithmatex:
+          generic: true
+      - footnotes
+      - pymdownx.details
+      - pymdownx.superfences
+      - pymdownx.mark
+      - attr_list
     
     nav:
       - index.md
       - Installation: installation.md
       - User Guide: user_guide.md
       - Developer Guide: dev_guide.md
       - XA information: info.md
```

### Comparing `DependiPy-1.0.9/README.md` & `DependiPy-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,23 @@
       "azure-core",
       "azure-identity",
       "azure-mgmt-consumption",
       "azure-mgmt-core",
       "azure-mgmt-costmanagement"
     ]},
   "exclude_lib": ["tensorflow", "setuptools"],
-  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"]
+  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"],
+  "force_version": {"pandas": "pandas==1.1.1", "numpy": "numpy"}
 }
 ```
 - **privat_lib**: sono le librerie private usate che non sono presenti su PyPi e che quindi non devono essere listate in un file di requirements, non potendo essere installate in automatico
 - **replace_lib**: sono le parole che devono essere sostituite nella ricerca delle librerie, dato che alcune librerie usano nomi diversi negli import dalle release su PyPi
 - **exclude_lib**: librerie che sono presenti nei file ma che non si vuole che vengano riportate
 - **exclude_folder**: cartelle che non devono essere considerate durante lo scan delle dipendenze
+- **force_version** sono le librerie di cui si vuole forzare una versione, viene usato un formato a dizionario dove la chiave e' la libreria identificata e il valore e' la stringa che si vuole usare dei requirements, si puo mettere una versione specifica o inserire solo il nome per non segnalare nessuna versione
 
 **Le librerie inserite nel requirements.txt sono sempre e solo quelle che devono essere installate, per cui non verranno mai riportate le dipendenze native di Python**
 
 ## lib/setup.py
 Se si sta lavorando in modalita lib, libraria produce un file alla fine della mappatura.
 Se il setup.py ha la forma seguente:
 ```python
@@ -96,18 +98,18 @@
 # stop
 
 setup(
     name='utilities',
     version=version,
     packages=find_packages(include=['utilities']),
     license='',
-    author='Andrea Jacassi',
+    author='John Do',
     author_email='',
     description='',
-    url="https://github.com/utilities.git",
+    url="https://github.com/rep.git",
     extras_require=requires_dict,
     install_requires=[],
 )
 ```
 Sono necessarie le seguenti chiavi nel setup.py: **# start**, uno **# stop**, uno **# version go** e uno **# version end**.
 Librarian andra a scrivere la mappatura direttamente nel setup.py.
 
@@ -217,29 +219,29 @@
           accent: lime
     
     repo_name: name repository github
     repo_url: url repository github
     
     plugins:
       - mkdocstrings
-        - search
+      - search
     
     markdown_extensions:
       - pymdownx.highlight:
           anchor_linenums: true
-        - pymdownx.inlinehilite
-        - pymdownx.snippets
-        - admonition
-        - pymdownx.arithmatex:
-            generic: true
-        - footnotes
-        - pymdownx.details
-        - pymdownx.superfences
-        - pymdownx.mark
-        - attr_list
+      - pymdownx.inlinehilite
+      - pymdownx.snippets
+      - admonition
+      - pymdownx.arithmatex:
+          generic: true
+      - footnotes
+      - pymdownx.details
+      - pymdownx.superfences
+      - pymdownx.mark
+      - attr_list
     
     nav:
       - index.md
       - Installation: installation.md
       - User Guide: user_guide.md
       - Developer Guide: dev_guide.md
       - XA information: info.md
```

### Comparing `DependiPy-1.0.9/setup.py` & `DependiPy-1.1.0/setup.py`

 * *Files identical despite different names*

