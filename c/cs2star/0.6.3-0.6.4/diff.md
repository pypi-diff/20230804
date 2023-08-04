# Comparing `tmp/cs2star-0.6.3.tar.gz` & `tmp/cs2star-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2star-0.6.3.tar", last modified: Tue Aug  1 10:31:26 2023, max compression
+gzip compressed data, was "cs2star-0.6.4.tar", last modified: Fri Aug  4 16:03:40 2023, max compression
```

## Comparing `cs2star-0.6.3.tar` & `cs2star-0.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-01 10:31:26.533424 cs2star-0.6.3/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.6.3/.gitignore
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.6.3/LICENSE
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-08-01 10:31:26.533424 cs2star-0.6.3/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.6.3/README.md
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-01 10:31:26.533424 cs2star-0.6.3/cs2star/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.6.3/cs2star/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-08-01 10:31:26.000000 cs2star-0.6.3/cs2star/_version.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    11794 2023-08-01 10:30:38.000000 cs2star-0.6.3/cs2star/cs2star.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3422 2023-03-29 12:13:31.000000 cs2star-0.6.3/cs2star/job_parser.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-01 10:31:26.533424 cs2star-0.6.3/cs2star.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-08-01 10:31:26.000000 cs2star-0.6.3/cs2star.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-08-01 10:31:26.000000 cs2star-0.6.3/cs2star.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-08-01 10:31:26.000000 cs2star-0.6.3/cs2star.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-08-01 10:31:26.000000 cs2star-0.6.3/cs2star.egg-info/entry_points.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-08-01 10:31:26.000000 cs2star-0.6.3/cs2star.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-08-01 10:31:26.000000 cs2star-0.6.3/cs2star.egg-info/top_level.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2023-07-31 12:44:31.000000 cs2star-0.6.3/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-08-01 10:31:26.533424 cs2star-0.6.3/setup.cfg
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 16:03:40.474975 cs2star-0.6.4/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.6.4/.gitignore
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.6.4/LICENSE
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-08-04 16:03:40.474975 cs2star-0.6.4/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.6.4/README.md
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 16:03:40.471642 cs2star-0.6.4/cs2star/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.6.4/cs2star/__init__.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-08-04 16:03:40.000000 cs2star-0.6.4/cs2star/_version.py
+-rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    11782 2023-08-04 15:51:13.000000 cs2star-0.6.4/cs2star/cs2star.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3454 2023-08-04 16:00:53.000000 cs2star-0.6.4/cs2star/job_parser.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 16:03:40.474975 cs2star-0.6.4/cs2star.egg-info/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-08-04 16:03:40.000000 cs2star-0.6.4/cs2star.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-08-04 16:03:40.000000 cs2star-0.6.4/cs2star.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-08-04 16:03:40.000000 cs2star-0.6.4/cs2star.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-08-04 16:03:40.000000 cs2star-0.6.4/cs2star.egg-info/entry_points.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-08-04 16:03:40.000000 cs2star-0.6.4/cs2star.egg-info/requires.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-08-04 16:03:40.000000 cs2star-0.6.4/cs2star.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2023-07-31 12:44:31.000000 cs2star-0.6.4/pyproject.toml
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-08-04 16:03:40.474975 cs2star-0.6.4/setup.cfg
```

### Comparing `cs2star-0.6.3/LICENSE` & `cs2star-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.3/PKG-INFO` & `cs2star-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.6.3
+Version: 0.6.4
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.6.3/README.md` & `cs2star-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.3/cs2star/cs2star.py` & `cs2star-0.6.4/cs2star/cs2star.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     particles = sorted(job_files['particles']['cs'])
     if not particles:
         print('[red]No usable particle files were found')
         sys.exit(1)
 
     particles_passthrough = sorted(job_files['particles']['passthrough'])
-    micrographs = sorted(job_files['micrographs']['cs'])
+    mic_files = sorted(job_files['micrographs']['cs'])
     micrographs_passthrough = sorted(job_files['micrographs']['passthrough'])
 
     dest_dir = Path(dest_dir)
     dest_star = dest_dir / 'particles.star'
     dest_mic_star = dest_dir / 'micrographs.star'
     to_create = [dest_dir]
     if micrographs:
@@ -100,15 +100,15 @@
 
     log = cleandoc(f'''
         Particle files:
         {', '.join(str(f) for f in particles)}
         Particle Passthrough files:
         {', '.join(str(f) for f in particles_passthrough)}
         Micrograph files:
-        {', '.join(str(f) for f in micrographs)}
+        {', '.join(str(f) for f in mic_files)}
         Micrograph Passthrough files:
         {', '.join(str(f) for f in micrographs_passthrough)}
         Will create: {', '.join(str(f) for f in to_create + [dest_star, dest_mic_star])}
     ''')
     if dry_run:
         print(Panel(log))
         sys.exit()
@@ -131,23 +131,23 @@
         else:
             raise ValueError(
                 'Number of passthrough files and particle files is incompatible:\n'
                 f'particles: {particles}\n'
                 f'passthroughs: {particles_passthrough}'
             )
 
-    if len(micrographs) != len(micrographs_passthrough):
+    if len(mic_files) != len(micrographs_passthrough):
         if len(micrographs_passthrough) == 0:
             pass
         elif len(micrographs_passthrough) == 1:
-            micrographs_passthrough = micrographs_passthrough * len(micrographs)
+            micrographs_passthrough = micrographs_passthrough * len(mic_files)
         else:
             raise ValueError(
                 'Number of passthrough files and micrographs files is incompatible:\n'
-                f'micrographs: {micrographs}\n'
+                f'micrographs: {mic_files}\n'
                 f'passthroughs: {micrographs_passthrough}'
             )
 
     if dest_star.is_file() and overwrite == 0:
         raise click.UsageError('particle file already exists. To overwrite, use -f')
     if dest_star.is_file() and overwrite == 0:
         raise click.UsageError('micrographs file already exists. To overwrite, use -f')
@@ -164,15 +164,15 @@
 
         if classes is not None:
             classes = classes.split(',')
             print(f'selecting classes: {", ".join(classes)}')
             df_part = pyem.star.select_classes(df_part, classes)
 
         df_mic = pd.DataFrame()
-        for f, p in progress.track(list(zip(micrographs, micrographs_passthrough)), description='Loading micrograph data...'):
+        for f, p in progress.track(list(zip(mic_files, micrographs_passthrough)), description='Loading micrograph data...'):
             data = np.load(f)
             df_mic_i = pyem.metadata.cryosparc_2_cs_movie_parameters(
                 data, passthroughs=[p], trajdir=str(f.parent.parent),
             )
             df_mic = pd.concat([df_mic, df_mic_i], ignore_index=True)
 
         # clean up
```

### Comparing `cs2star-0.6.3/cs2star/job_parser.py` & `cs2star-0.6.4/cs2star/job_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,26 +43,26 @@
         return files
 
     j_type = job['type']
     for output in job['output_results']:
         metafiles = output['metafiles']
         passthrough = output['passthrough']
         k2 = 'passthrough' if passthrough else 'cs'
-        if j_type == 'hetero_refine':
-            # hetero refine is special because the "good" output is split into multiple files
+        if j_type in ('hetero_refine', 'homo_abinit', 'class_3D'):
+            # refine is special because the "good" output is split into multiple files
             if (not passthrough and 'particles_class_' in output['group_name']) or (passthrough and output['group_name'] == 'particles_all_classes'):
                 files['particles'][k2].add(job_dir.parent / metafiles[-1])
         elif j_type == 'particle_sets':
             if (matched := re.search(r'split_(\d+)', output['group_name'])) is not None:
                 if sets is None or int(matched[1]) in [int(s) for s in sets]:
                     files['particles'][k2].add(job_dir.parent / metafiles[-1])
         else:
             # every remaining job type is covered by this generic loop
             for file in metafiles:
-                if any(bad in file for bad in ('excluded', 'incomplete', 'remainder', 'rejected', 'uncategorized')):
+                if any(bad in file for bad in ('excluded', 'incomplete', 'remainder', 'rejected', 'uncategorized', 'unused')):
                     continue
                 if 'particles' in file:
                     k1 = 'particles'
                 elif 'micrographs' in file:
                     k1 = 'micrographs'
                 else:
                     continue
```

### Comparing `cs2star-0.6.3/cs2star.egg-info/PKG-INFO` & `cs2star-0.6.4/cs2star.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.6.3
+Version: 0.6.4
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.6.3/pyproject.toml` & `cs2star-0.6.4/pyproject.toml`

 * *Files identical despite different names*

