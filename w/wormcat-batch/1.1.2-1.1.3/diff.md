# Comparing `tmp/wormcat_batch-1.1.2.tar.gz` & `tmp/wormcat_batch-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormcat_batch-1.1.2.tar", last modified: Wed Aug  2 17:17:10 2023, max compression
+gzip compressed data, was "wormcat_batch-1.1.3.tar", last modified: Fri Aug  4 16:16:54 2023, max compression
```

## Comparing `wormcat_batch-1.1.2.tar` & `wormcat_batch-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-02 17:17:10.100752 wormcat_batch-1.1.2/
--rw-r--r--   0 dan        (501) staff       (20)      135 2023-08-02 13:35:39.000000 wormcat_batch-1.1.2/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-02 17:17:10.100603 wormcat_batch-1.1.2/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2733 2023-08-01 19:34:44.000000 wormcat_batch-1.1.2/README.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-08-02 17:17:10.100790 wormcat_batch-1.1.2/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      703 2023-08-02 17:16:21.000000 wormcat_batch-1.1.2/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-02 17:17:10.099310 wormcat_batch-1.1.2/wormcat_batch/
--rw-r--r--   0 dan        (501) staff       (20)     3324 2023-08-02 16:46:39.000000 wormcat_batch-1.1.2/wormcat_batch/create_sunburst.py
--rw-r--r--   0 dan        (501) staff       (20)     3947 2023-08-01 17:11:31.000000 wormcat_batch-1.1.2/wormcat_batch/create_wormcat_xlsx.py
--rw-r--r--   0 dan        (501) staff       (20)     2522 2023-08-01 19:01:04.000000 wormcat_batch-1.1.2/wormcat_batch/execute_r.py
--rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.2/wormcat_batch/is_wormcat_installed.R
--rwxr-xr-x   0 dan        (501) staff       (20)     9162 2023-08-02 16:42:21.000000 wormcat_batch-1.1.2/wormcat_batch/run_wormcat_batch.py
--rw-r--r--   0 dan        (501) staff       (20)   227410 2023-08-02 13:20:17.000000 wormcat_batch-1.1.2/wormcat_batch/sunburst.template
--rwxr-xr-x   0 dan        (501) staff       (20)     1484 2023-07-31 16:25:55.000000 wormcat_batch-1.1.2/wormcat_batch/worm_cat.R
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-02 17:17:10.100309 wormcat_batch-1.1.2/wormcat_batch.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      516 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       32 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       14 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-04 16:16:54.180033 wormcat_batch-1.1.3/
+-rw-r--r--   0 dan        (501) staff       (20)      135 2023-08-02 13:35:39.000000 wormcat_batch-1.1.3/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-04 16:16:54.179885 wormcat_batch-1.1.3/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2733 2023-08-01 19:34:44.000000 wormcat_batch-1.1.3/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-08-04 16:16:54.180074 wormcat_batch-1.1.3/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      703 2023-08-04 16:15:55.000000 wormcat_batch-1.1.3/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-04 16:16:54.178479 wormcat_batch-1.1.3/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     3888 2023-08-04 13:35:59.000000 wormcat_batch-1.1.3/wormcat_batch/create_sunburst.py
+-rw-r--r--   0 dan        (501) staff       (20)     4628 2023-08-04 13:51:15.000000 wormcat_batch-1.1.3/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2909 2023-08-04 14:01:40.000000 wormcat_batch-1.1.3/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.3/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     9530 2023-08-04 13:22:35.000000 wormcat_batch-1.1.3/wormcat_batch/run_wormcat_batch.py
+-rw-r--r--   0 dan        (501) staff       (20)   227410 2023-08-02 13:20:17.000000 wormcat_batch-1.1.3/wormcat_batch/sunburst.template
+-rwxr-xr-x   0 dan        (501) staff       (20)     1807 2023-08-04 12:54:01.000000 wormcat_batch-1.1.3/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-04 16:16:54.179684 wormcat_batch-1.1.3/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-04 16:16:54.000000 wormcat_batch-1.1.3/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      516 2023-08-04 16:16:54.000000 wormcat_batch-1.1.3/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-04 16:16:54.000000 wormcat_batch-1.1.3/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-08-04 16:16:54.000000 wormcat_batch-1.1.3/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-04 16:16:54.000000 wormcat_batch-1.1.3/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       32 2023-08-04 16:16:54.000000 wormcat_batch-1.1.3/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-08-04 16:16:54.000000 wormcat_batch-1.1.3/wormcat_batch.egg-info/top_level.txt
```

### Comparing `wormcat_batch-1.1.2/README.md` & `wormcat_batch-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.2/setup.py` & `wormcat_batch-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # rm -rf dist
 # python setup.py sdist
 # pip install dist/wormcat_batch-1.0.1.tar.gz
 # twine check dist/*
 # twine upload --repository pypi dist/*
 
 setup(name='wormcat_batch',
-      version='1.1.2',
+      version='1.1.3',
       description='Batch processing for Wormcat data',
       url='https://github.com/dphiggs01/Wormcat_batch',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
       license='MIT',
 
       packages=['wormcat_batch'],
```

### Comparing `wormcat_batch-1.1.2/wormcat_batch/create_sunburst.py` & `wormcat_batch-1.1.3/wormcat_batch/create_sunburst.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-import pandas as pd
+"""
+Create sunburt HTML file with Regulated Gene Set Data (RGS)
+"""
 import json
 import os
 import pkg_resources
+import pandas as pd
 
 
 def read_rgs_and_categories(file_nm_in):
+    """
+    Read the RGS Data and creat JSON based on Category 3 info
+    """
     nodes_dict = {}
     try:
         df = pd.read_csv(file_nm_in)
         node1_list= []
         nodes_dict = {"name":"rgs", "children":node1_list}
 
         cat3 = df.groupby(["Category.3"]).count()
@@ -34,31 +40,40 @@
     except Exception as e:
         print("Error in read_rgs_and_categories:", e)
         pass
     return nodes_dict
 
 
 def create_sunburst(dir_nm):
+    """
+    1. Read the sunburst template file 
+    2. Find the line "insert json here" in the template
+    3. Inject the Cat3 JSON Data at this point in the file
+    4. Save the file as sunburst.html
+    """
     file_nm_sunburst_html = f"{dir_nm}{os.path.sep}sunburst.html"
     file_nm_rgs_and_categories = f"{dir_nm}{os.path.sep}rgs_and_categories.csv"
     data = read_sunburst_template()
     json_data = json.dumps(read_rgs_and_categories(file_nm_rgs_and_categories))
     
 
     with open(file_nm_sunburst_html, "w") as file:
         for d in data:
             file.write(d)
             if "insert json here" in d:
                 json_data = json.dumps(read_rgs_and_categories(file_nm_rgs_and_categories))
-                json_var = "var json_data = {}".format(json_data)
+                json_var = f"var json_data = {json_data}"
                 file.write(json_var)
 
 
 
 def getChildrenFor(parent, nodes_dict):
+    """
+    Utility function getChildrenFor given parent
+    """
     children = nodes_dict['children']
     node_list = None
     for key in children:
         if parent == key['name']:
             if 'children' in key:
                 node_list = key['children']
             break
@@ -66,14 +81,17 @@
     if node_list is None:
         node_list = []
         children.append({"name":parent, "children":node_list})
     return node_list
 
 
 def getChildrenFor2(grand_parent, parent, nodes_dict):
+    """
+    Utility function getChildrenFor given grand parent
+    """
     children = getChildrenFor(grand_parent, nodes_dict)
     node_list = None
     for key in children:
         if parent == key['name']:
             if 'children' in key:
                 node_list = key['children']
             break
@@ -81,24 +99,27 @@
     if node_list is None:
         node_list = []
         children.append({"name":parent, "children":node_list})
 
     return node_list
 
 def read_sunburst_template():
+    """
+    Utility function to fined the template file in the package directory
+    """
     try:
         data = []
         #data = pkg_resources.resource_string(__name__, 'sunburst.template').decode('utf-8')
         data_file = pkg_resources.resource_filename(__name__, 'sunburst.template')
         with open(data_file, "r") as file:
             data = file.readlines()
         return data
     except Exception as e:
         print("Error reading sunburst_template:", e)
         return None
 
 
 if __name__ == "__main__":
-    print("starting {}".format(os.getcwd()))
+    print(f"starting {os.getcwd()}")
     create_sunburst('RGS_Feb-14-2020-11_45_54')
```

### Comparing `wormcat_batch-1.1.2/wormcat_batch/execute_r.py` & `wormcat_batch-1.1.3/wormcat_batch/execute_r.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+"""
+Module to delegate calls to R program execution
+"""
 from subprocess import Popen, PIPE
 import sys
 import os
 import platform
 import logging
 
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 
 class ExecuteR(object):
+    """
+    Class to mange R exection
+    """
     wormcat_r = f'{os.path.dirname(__file__)}{os.path.sep}worm_cat.R'
 
     worm_cat_function = [wormcat_r,
                                '--file', 0,
                                '--title', 1,
                                '--out_dir', 2,
                                '--rm_dir', 3,
@@ -25,39 +31,50 @@
 
     if platform.system() == 'Windows':
         wormcat_library_path.insert(0,'rscript.exe')
         worm_cat_function.insert(0,'rscript.exe')
 
 
     def wormcat_library_path_fun(self):
+        """
+        Utility function to get the R library path to the Wormcat function
+        """
         ret_val = self.run(self.wormcat_library_path,"")
         return ret_val
 
     def worm_cat_fun(self, file_name, out_dir, title, annotation_file, input_type):
+        """
+        Utility function to setup the call to Wormcat function
+        """
         print(f"Calling Wormcat with {os.path.basename(file_name)[:-4]} data")
         ret_val = self.run(self.worm_cat_function, file_name, title, out_dir, "False", annotation_file, input_type, "False")
         return ret_val
 
     def run(self, arg_list, *args):
+        """
+        Execute the R script
+        """
         try:
             processed_args = self.process_args(arg_list, *args)
             process = Popen(processed_args, stdout=PIPE)
             out, err = process.communicate()
             out = str(out, 'utf-8')
             if not out:
                 out = None
             #sys.stderr.write("run: out={} err={}\n".format(out,err))
             return out
-        except Exception as e:
-            sys.stderr.write("ERROR: command line error %s\n" % args)
-            sys.stderr.write("ERROR: %s\n" % e)
+        except Exception as err:
+            sys.stderr.write(f"ERROR: command line error {args}\n")
+            sys.stderr.write(f"ERROR: %{err}\n")
             sys.exit(-1)
 
     def process_args(self, arg_tuple, *args):
-        # process the arg
+        """
+        Utility function to build the arg list
+        """
         arg_list = list(arg_tuple)
         for index in range(0, len(arg_list)):
             if type(arg_list[index]) == int:
                 # substitue for args passed in
                 if arg_list[index] < len(args):
                     arg_list[index] = args[arg_list[index]]
                 # if we have more substitutions than args passed delete the extras
```

### Comparing `wormcat_batch-1.1.2/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.1.3/wormcat_batch/run_wormcat_batch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,143 +1,163 @@
+"""
+Module provides functionality for running Wormcat in batch mode at the command linr
+"""
 import os
 import sys
 import argparse
-import pandas as pd
 import shutil
 import zipfile
 import importlib.metadata
 from datetime import datetime
+import warnings
+import pandas as pd
 from wormcat_batch.execute_r import ExecuteR
 from wormcat_batch.create_wormcat_xlsx import process_category_files
 from wormcat_batch.create_sunburst import create_sunburst
 
-import warnings
 warnings.filterwarnings('ignore', category=UserWarning, module='openpyxl')
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
+
 def extract_csv_files(input_excel_nm, csv_file_path):
-    '''
+    """
     Create CSV Files from the given Excel spreadsheet
-    '''
+    """
     input_excel = pd.ExcelFile(input_excel_nm)
     for sheet in input_excel.sheet_names:
         sheet_df = input_excel.parse(sheet)
-        sheet_df.to_csv(f'{csv_file_path}{os.path.sep}{sheet}.csv', index=False)
+        sheet_df.to_csv(
+            f'{csv_file_path}{os.path.sep}{sheet}.csv', index=False)
+
 
-        
 def process_csv_files(csv_file_path, wormcat_out_path, annotation_file):
-    '''
+    """
     Read the csv data files and process each individually through Wormcat
-    '''
+    """
     for dir_content in os.listdir(csv_file_path):
         conetnt_full_path = os.path.join(csv_file_path, dir_content)
         if os.path.isfile(conetnt_full_path):
             with open(conetnt_full_path, 'r') as file:
                 header_line = file.readline().strip()
             wormcat_input_type = header_line.replace(' ', '.')
             csv_file_nm = os.path.basename(conetnt_full_path)
-            file_nm_wo_ext = csv_file_nm[:-4] # Remove .csv from file name
+            file_nm_wo_ext = csv_file_nm[:-4]  # Remove .csv from file name
             title = file_nm_wo_ext.replace('_', ' ')
             wormcat_output_dir = f'{wormcat_out_path}{os.path.sep}{file_nm_wo_ext}'
-            executeR = ExecuteR()
-            executeR.worm_cat_fun(conetnt_full_path, wormcat_output_dir, title, annotation_file, wormcat_input_type)
+            execute_r = ExecuteR()
+            execute_r.worm_cat_fun(
+                conetnt_full_path, wormcat_output_dir, title, annotation_file, wormcat_input_type)
             create_sunburst(wormcat_output_dir)
     return wormcat_out_path
 
+
 def create_summary_spreadsheet(wormcat_out_path, annotation_file, out_xsl_file_nm):
-    '''
+    """
     After all the sheets on the Excel have been executed or CSV files processed 
     create a dataframe that can be used to summarize the results.
     This dataframe is used to create the output Excel.
-    '''
+    """
     process_lst = []
     for dir_nm in os.listdir(wormcat_out_path):
-        for cat_num in [1,2,3]:
+        for cat_num in [1, 2, 3]:
             rgs_fisher = f"{wormcat_out_path}{os.path.sep}{dir_nm}{os.path.sep}rgs_fisher_cat{cat_num}.csv"
             cat_nm = f"Cat{cat_num}"
-            row = {'sheet': cat_nm, 'category': cat_num, 'file': rgs_fisher,'label': dir_nm}
+            row = {'sheet': cat_nm, 'category': cat_num,
+                   'file': rgs_fisher, 'label': dir_nm}
             process_lst.append(row)
 
-    df_process = pd.DataFrame(process_lst, columns=['sheet', 'category', 'file','label'])
+    df_process = pd.DataFrame(process_lst, columns=[
+                              'sheet', 'category', 'file', 'label'])
     process_category_files(df_process, annotation_file, out_xsl_file_nm)
 
-## Wormcat Utility functions
+# Wormcat Utility functions
+
 
 def get_wormcat_lib():
     '''
     Find the location where the R Wormcat program is installed
     '''
-    executeR = ExecuteR()
-    path = executeR.wormcat_library_path_fun()
+    execute_r = ExecuteR()
+    path = execute_r.wormcat_library_path_fun()
     if path:
-        first_quote=path.find('"')
-        last_quote=path.rfind('"')
+        first_quote = path.find('"')
+        last_quote = path.rfind('"')
         if last_quote == -1:
             print("Wormcat is not installed or cannot be found.")
             exit(-1)
         path = path[first_quote+1:last_quote]
     # print(f"wormcat_lib_path={path}")
     return path
 
+
 def get_category_files(path):
-    '''
+    """
     Get the list of available annotation files for Wormcat.
     These files exist in the R wormcat install under the "extdata" directory
-    '''
-    category_files=[]
-    index=1
-    path = "{}{}extdata".format(path, os.path.sep)
+    """
+    category_files = []
+    index = 1
+    path = f"{path}{os.path.sep}extdata"
     for root, dirs, files in os.walk(path):
         for filename in files:
             category_files.append(filename)
-            index +=1
+            index += 1
 
     return category_files
 
-## Utility functions
+# Utility functions
+
 
 def create_directory(directory, with_backup=False):
-    '''
+    """
     Utility function to create a directory and backup the original if it exists and has content
-    '''
+    """
     if with_backup and os.path.exists(directory) and os.listdir(directory):
         print(f"Creating backup of existing directory [{directory}]")
         # Create backup directory name with a unique timestamp suffix
         timestamp = datetime.now().strftime("%Y%m%d-%H%M%S")
         backup_dir = f"{directory}_{timestamp}.bk"
         shutil.move(directory, backup_dir)
 
     os.makedirs(directory, exist_ok=True)
 
+
 def zip_directory(directory_path, zip_file_name):
-    '''
+    """
     Compress the content of a directory in zip format.
-    '''
+    """
     with zipfile.ZipFile(zip_file_name, 'w') as zipf:
         for root, _, files in os.walk(directory_path):
             for file in files:
                 file_path = os.path.join(root, file)
-                zipf.write(file_path, os.path.relpath(file_path, directory_path))
+                zipf.write(file_path, os.path.relpath(
+                    file_path, directory_path))
+
+# main application functions
 
-## main application functions 
 
 def process_command_arguments():
-    '''
+    """
     The process_command_arguments method validates and sets the input arguments 
     to conform with downstream processing
-    '''
+    """
     parser = argparse.ArgumentParser()
-    help_statement="wormcat_cli --input-excel <path_to_excel> | --input-csv-path <path_to_csv> --output-path <path_to_out_dir> --annotation-file 'whole_genome_v2_nov-11-2021.csv' --clean-temp False"
-    parser.add_argument('-i', '--input-excel', help='Input file in Excel/Wormcat format')
-    parser.add_argument('-c', '--input-csv-path', help='Input path to a collection of CSV files in Wormcat format')
+    help_statement = "wormcat_cli --input-excel <path_to_excel> | --input-csv-path <path_to_csv> --output-path <path_to_out_dir> --annotation-file 'whole_genome_v2_nov-11-2021.csv' --clean-temp False"
+    parser.add_argument('-i', '--input-excel',
+                        help='Input file in Excel/Wormcat format')
+    parser.add_argument('-c', '--input-csv-path',
+                        help='Input path to a collection of CSV files in Wormcat format')
     parser.add_argument('-o', '--output-path', help='Output path')
-    parser.add_argument('-a', '--annotation-file', default='whole_genome_v2_nov-11-2021.csv', help='Annotation file name or path default=whole_genome_v2_nov-11-2021.csv')
-    parser.add_argument('-t', '--clean-temp', default='True', help='Remove files created while processing default=False')
+    parser.add_argument('-a', '--annotation-file', default='whole_genome_v2_nov-11-2021.csv',
+                        help='Annotation file name or path default=whole_genome_v2_nov-11-2021.csv')
+    parser.add_argument('-t', '--clean-temp', default='True',
+                        help='Remove files created while processing default=False')
 
-    parser.add_argument('-v', '--version', action='version', version=f'%(prog)s v{importlib.metadata.version("wormcat_batch")}')
+    parser.add_argument('-v', '--version', action='version',
+                        version=f'%(prog)s v{importlib.metadata.version("wormcat_batch")}')
     args = parser.parse_args()
 
     if not args.input_excel and not args.input_csv_path:
         print(help_statement)
         print("An Excel Input file or a path to CSV files is required.")
         sys.exit(-1)
 
@@ -147,33 +167,36 @@
         sys.exit(-1)
 
     # if args.annotation_file is not a path to an annotation file
     # vaildate the input name and set the full path
     if not (os.path.sep in args.annotation_file):
         wormcat_path = get_wormcat_lib()
         annotation_files = get_category_files(wormcat_path)
-         
+        
         if not args.annotation_file or not args.annotation_file in annotation_files:
             print(help_statement)
             print("Missing or incorrect annotation-file-nm.")
-            print("Available names: {}".format(annotation_files))
+            print(f"Available names: {annotation_files}")
             sys.exit(-1)
         args.annotation_file = f"{wormcat_path}{os.path.sep}extdata{os.path.sep}{args.annotation_file}"
-    
+
     # Support TRUE or True as input to clean temp
     # otherwise set to False
     if args.clean_temp.lower().title() == 'True':
         args.clean_temp = True
     else:
         args.clean_temp = False
 
     return args
 
 
 def main():
+    """
+    Main control execution of Wormcat Batch
+    """
     print("Starting Wormcat Batch")
 
     # Validate the command line arguments
     args = process_command_arguments()
 
     # Create the output directory if it does not exsist.
     # If it does exist and has content create a backup.
@@ -194,37 +217,38 @@
     if args.input_excel:
         base_input_excel = os.path.basename(args.input_excel)
         input_data_nm = os.path.splitext(base_input_excel)[0]
     else:
         input_data_nm = os.path.basename(args.input_csv_path)
 
     timestamp = datetime.now().strftime("%Y%m%d-%H%M%S")
-    output_base_dir =f"{input_data_nm}_{timestamp}"
+    output_base_dir = f"{input_data_nm}_{timestamp}"
     wormcat_out_path = f"{args.output_path}{os.path.sep}{output_base_dir}"
     create_directory(wormcat_out_path)
 
     print(f"{args.input_excel=}")
     print(f"{args.input_csv_path=}")
     print(f"{args.output_path=}")
     print(f"{args.annotation_file=}")
     print(f"{args.clean_temp=}")
 
     # Call Wormcat on each CSV file
     process_csv_files(csv_file_path, wormcat_out_path, args.annotation_file)
 
     # Create a summary spreadsheet of all CSV runs
     out_xsl_file_nm = f"{wormcat_out_path}{os.path.sep}Out_{input_data_nm}.xlsx"
-    create_summary_spreadsheet(wormcat_out_path, args.annotation_file, out_xsl_file_nm)
-    
+    create_summary_spreadsheet(
+        wormcat_out_path, args.annotation_file, out_xsl_file_nm)
+
     # Zip the results
     zip_dir_nm = f"{args.output_path}{os.path.sep}{output_base_dir}.zip"
     zip_directory(wormcat_out_path, zip_dir_nm)
-    
+
     # If set Remove files created while processing
     if args.clean_temp:
         shutil.rmtree(wormcat_out_path)
         if args.input_excel:
             shutil.rmtree(csv_file_path)
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `wormcat_batch-1.1.2/wormcat_batch/sunburst.template` & `wormcat_batch-1.1.3/wormcat_batch/sunburst.template`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.2/wormcat_batch/worm_cat.R` & `wormcat_batch-1.1.3/wormcat_batch/worm_cat.R`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,39 @@
 
 parser$add_argument("-r", "--rm_dir", default=TRUE, help="Remove temp directory [default]")
 
 parser$add_argument("-z", "--zip_files", default=TRUE, help="Create a zip file of the results directory [default]")
 
 args <- parser$parse_args()
 
-if (is.null(args$file)){
-  stop("At least one argument must be supplied (input file).n", call.=FALSE)
+if (is.null(args$file)) {
+  stop("At least one argument must be supplied (input file).n", call.= FALSE)
 }
 
-print(paste("worm_cat_fun", args$file, args$title, args$out_dir, args$rm_dir, args$annotation_file, args$input_type, args$zip_files))
+# con <- file("worm_cat_fun.log") # nolint
+# sink(con, append = TRUE) # nolint
+# sink(con, append = TRUE, type = "message") # nolint
+
+
+#print(paste("worm_cat_fun", args$file, args$title, args$out_dir, args$rm_dir, args$annotation_file, args$input_type, args$zip_files)) # nolint
+
+if (toupper(args$rm_dir) == "TRUE") {
+    rm_dir <- TRUE
+} else {
+    rm_dir <- FALSE
+}
+
+if (toupper(args$zip_files) == "TRUE") {
+    zip_files <- TRUE
+} else {
+    zip_files <- FALSE
+}
 
 worm_cat_fun(
     file_to_process = args$file,
     title = args$title,
     output_dir = args$out_dir,
-    rm_dir = args$rm_dir,
+    rm_dir = rm_dir,
     annotation_file = args$annotation_file,
     input_type = args$input_type,
-    zip_files = args$zip_files
+    zip_files = zip_files
 )
-
```

### Comparing `wormcat_batch-1.1.2/wormcat_batch.egg-info/SOURCES.txt` & `wormcat_batch-1.1.3/wormcat_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

