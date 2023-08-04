# Comparing `tmp/ECMpy2.0-1.0.0.tar.gz` & `tmp/ECMpy2.0-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ECMpy2.0-1.0.0.tar", last modified: Fri May 12 12:30:00 2023, max compression
+gzip compressed data, was "ECMpy2.0-1.0.1.tar", last modified: Fri Aug  4 02:46:59 2023, max compression
```

## Comparing `ECMpy2.0-1.0.0.tar` & `ECMpy2.0-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-x---   0 maozt    (1324801123) domain users (1324800513)        0 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/
-drwxr-x---   0 maozt    (1324801123) domain users (1324800513)        0 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/ECMpy2.0.egg-info/
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)      231 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/ECMpy2.0.egg-info/PKG-INFO
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)      251 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/ECMpy2.0.egg-info/SOURCES.txt
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)        1 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/ECMpy2.0.egg-info/dependency_links.txt
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)      124 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/ECMpy2.0.egg-info/requires.txt
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)        7 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/ECMpy2.0.egg-info/top_level.txt
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)      231 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/PKG-INFO
--rw-r--r--   0 maozt    (1324801123) domain users (1324800513)      619 2023-05-12 11:41:18.000000 ECMpy2.0-1.0.0/README.md
-drwxr-x---   0 maozt    (1324801123) domain users (1324800513)        0 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/script/
--rw-r--r--   0 maozt    (1324801123) domain users (1324800513)    93136 2023-05-12 11:41:18.000000 ECMpy2.0-1.0.0/script/AutoPACMEN_function.py
--rw-r--r--   0 maozt    (1324801123) domain users (1324800513)    65329 2023-05-12 11:41:18.000000 ECMpy2.0-1.0.0/script/ECMpy_function.py
--rw-r--r--   0 maozt    (1324801123) domain users (1324800513)       19 2023-05-12 11:41:18.000000 ECMpy2.0-1.0.0/script/__init__.py
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)       38 2023-05-12 12:30:05.000000 ECMpy2.0-1.0.0/setup.cfg
--rw-r-----   0 maozt    (1324801123) domain users (1324800513)      646 2023-05-12 12:07:51.000000 ECMpy2.0-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-08-04 02:46:59.634269 ECMpy2.0-1.0.1/ECMpy/
+-rw-rw-rw-   0        0        0    94027 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/AutoPACMEN_function.py
+-rw-rw-rw-   0        0        0   121429 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/ECMpy_function.py
+-rw-rw-rw-   0        0        0       19 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/__init__.py
+-rw-rw-rw-   0        0        0     4718 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/get_ecGEM_onestop.py
+-rw-rw-rw-   0        0        0     8905 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/model.py
+-rw-rw-rw-   0        0        0     9605 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/ECMpy/prediction_for_input.py
+drwxrwxrwx   0        0        0        0 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/
+-rw-rw-rw-   0        0        0      252 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      184 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 02:46:59.000000 ECMpy2.0-1.0.1/ECMpy2.0.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      252 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2883 2023-08-04 02:07:28.000000 ECMpy2.0-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 02:46:59.639977 ECMpy2.0-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      835 2023-08-04 02:40:07.000000 ECMpy2.0-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ECMpy2.0-1.0.0/script/AutoPACMEN_function.py` & `ECMpy2.0-1.0.1/ECMpy/AutoPACMEN_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,16 +445,19 @@
             },
             (...)
         },
         (...)
     }
     </pre>
     """
-    model: cobra.Model = cobra.io.read_sbml_model(sbml_path)
-
+    #model: cobra.Model = cobra.io.read_sbml_model(sbml_path)
+    if re.search('\.xml',sbml_path):
+        model = cobra.io.read_sbml_model(sbml_path)
+    elif re.search('\.json',sbml_path):
+        model = cobra.io.json.load_json_model(sbml_path)
     # Get EC numbers of the model's reactions
     ec_numbers_of_model: List[str] = []
     for reaction in model.reactions:
         if "ec-code" not in reaction.annotation.keys():
             continue
 
         ec_numbers_of_reaction = reaction.annotation["ec-code"]
@@ -1141,15 +1144,20 @@
 
     Arguments
     ----------
     * sbml_path: str ~ The model's SBML path.
     * json_output_path: str ~ The path of the JSON that shall be created
     """
     # LOAD SBML MODEL
-    model: cobra.Model = cobra.io.read_sbml_model(sbml_path)
+    #model: cobra.Model = cobra.io.read_sbml_model(sbml_path)
+    if re.search('\.xml',sbml_path):
+        model = cobra.io.read_sbml_model(sbml_path)
+    elif re.search('\.json',sbml_path):
+        model = cobra.io.json.load_json_model(sbml_path)
+
     parse_sabio_rk_for_model(model, json_output_path,
                              bigg_id_name_mapping_path)
     
 def create_combined_kcat_database(sabio_rk_kcat_database_path: str, brenda_kcat_database_path: str, output_path: str) -> None:
     """Creates a combined JSON of the given SABIO-K and BRENDA kcat databases with non-wildcard entries only.
 
     Arguments
@@ -1606,31 +1614,33 @@
     #            ori_kcat=species_kcat_mapping[species]#Mr.Mao 
     #    current_distance += 1
     ###change code by Mr.Mao###
     #First,kcat
     if organism in species_kcat_mapping.keys():
         kcat_list=species_kcat_mapping[organism]
         ori_kcat=species_kcat_mapping[organism]
+        kcat_extend='Database'
         #print('kcat',organism,kcat_list,ori_kcat)
     #Second,sa
     elif organism in complete_entry_sa.keys() and MW !='none':
         #print(complete_entry_sa[species],MW)
         kcat_list=[sa*MW/60 for sa in complete_entry_sa[organism]]####kg / mol  g/mmol kcat(s-1)
         ori_kcat=complete_entry_sa[organism]#Mr.Mao 
+        kcat_extend='Brenda_SA'
         #print('sa',organism,kcat_list,ori_kcat)
     #Last,other species
     else:
         while (len(kcat_list) < num_min_kcat_entries) and (current_distance <= maximal_distance):
             for species in score_dict.keys():
                 if species not in species_kcat_mapping.keys():  # e.g. soil bacterium -> bacterium
                     continue
                 if score_dict[species] == current_distance and species!=organism:#Mr.Mao
                     kcat_list += species_kcat_mapping[species]
                     species_list.append(species)
-                    kcat_extend='True'
+                    kcat_extend='Other_species'
                 #if species==organism:
                     #print(species)
                 #    ori_kcat=species_kcat_mapping[species]#Mr.Mao 
             current_distance += 1
     ##########################
     # Get the protein database kcat for this reaction (if there is one, otherwise it returns math.nan)
     if protein_kcat_database != {}:
@@ -1778,15 +1788,19 @@
     reaction_mw_mapping: Dict[str, float] = json_load(reaction_mw_path)#Mr.Mao
     if protein_kcat_database_path != "none":
         protein_kcat_database = json_load(protein_kcat_database_path)
     else:
         protein_kcat_database = {}
 
     # Load the given stoichiometric model
-    model = cobra.io.read_sbml_model(sbml_path)
+    #model = cobra.io.read_sbml_model(sbml_path)
+    if re.search('\.xml',sbml_path):
+        model = cobra.io.read_sbml_model(sbml_path)
+    elif re.search('\.json',sbml_path):
+        model = cobra.io.json.load_json_model(sbml_path)
 
     # Set-up dictionary which will be the content of the output JSON
     reactions_kcat_mapping: Dict[str, Dict[str, float]] = {}
     # Go through each reaction in order to assign kcats for it :D
     for reaction in model.reactions:
         # If no EC number is given in the reaction's annotations,
         # the protein-dependent database is read out in order to
@@ -1936,14 +1950,16 @@
         reactions_kcat_mapping[reaction.id]["forward_kcat_list"] = forward_kcat_list#Mr.Mao
         reactions_kcat_mapping[reaction.id]["forward_ori_kcat"] = ori_forward_kcat#Mr.Mao
         reactions_kcat_mapping[reaction.id]["forward_species_list"] = forward_species_list#Mr.Mao
         reactions_kcat_mapping[reaction.id]["reverse"] = reverse_kcat
         reactions_kcat_mapping[reaction.id]["reverse_kcat_list"] = reverse_kcat_list#Mr.Mao
         reactions_kcat_mapping[reaction.id]["reverse_ori_kcat"] = ori_reverse_kcat#Mr.Mao
         reactions_kcat_mapping[reaction.id]["reverse_species_list"] = reverse_species_list#Mr.Mao
+
+        reactions_kcat_mapping[reaction.id]["data_type"] =kcat_extend
         # display the found out kcats for this reaction \o/
         #_print_assigned_kcats(reaction.id, forward_kcat, reverse_kcat)
 
     # Export the kcat mapping results as JSON :D
     json_write(basepath+"_reactions_kcat_mapping_combined.json", reactions_kcat_mapping)
 
 def get_protein_mass_mapping(model: cobra.Model, project_folder: str, project_name: str) -> None:
@@ -2081,9 +2097,13 @@
 
     Arguments
     ----------
     * sbml_path: str ~ The path to the model's SBML
     * project_folder: str ~ The folder in which the JSON shall be created
     * project_name: str ~ The beginning of the JSON's file name
     """
-    model: cobra.Model = cobra.io.read_sbml_model(sbml_path)
+    #model: cobra.Model = cobra.io.read_sbml_model(sbml_path)
+    if re.search('\.xml',sbml_path):
+        model = cobra.io.read_sbml_model(sbml_path)
+    elif re.search('\.json',sbml_path):
+        model = cobra.io.json.load_json_model(sbml_path)
     get_protein_mass_mapping(model, project_folder, project_name)
```

### Comparing `ECMpy2.0-1.0.0/setup.py` & `ECMpy2.0-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ECMpy2.0',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
+    license='MIT',
+    zip_safe=False,
+    include_package_data=True,
     install_requires=[
-        'cobra',
+        'cobra==0.21.0',
         'openpyxl',
         'requests',
         'pebble',
         'xlsxwriter',
         'Bio',
         'Require',
         'quest',
         'scikit-learn',
         'RDKit',
         'seaborn',
         'pubchempy',
         'torch',
         'ipykernel',
-        'matplotlib',
-    ],
+        'bioservices==1.10.4',
+        'pyprobar',
+        'xmltodict',
+        'plotly',
+        'kaleido',
+        'nbformat',
+        ],
     author='Zhitao Mao',
     author_email='mao_zt@tib.cas.cn',
     description='Automated construction of enzyme constraint models using ECMpy workflow.',
     url='https://github.com/tibbdc/ECMpy2.0',
 )
```

