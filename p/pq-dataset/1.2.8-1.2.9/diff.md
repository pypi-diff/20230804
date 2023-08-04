# Comparing `tmp/pq_dataset-1.2.8.tar.gz` & `tmp/pq_dataset-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pq_dataset-1.2.8.tar", last modified: Tue Mar 28 10:07:00 2023, max compression
+gzip compressed data, was "pq_dataset-1.2.9.tar", last modified: Fri Aug  4 11:17:13 2023, max compression
```

## Comparing `pq_dataset-1.2.8.tar` & `pq_dataset-1.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 10:07:00.890371 pq_dataset-1.2.8/
--rw-rw-rw-   0        0        0      224 2023-03-28 10:07:00.887376 pq_dataset-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       11 2022-11-29 07:52:53.000000 pq_dataset-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 10:07:00.795212 pq_dataset-1.2.8/pq_dataset/
--rw-rw-rw-   0        0        0        0 2023-02-15 06:36:59.000000 pq_dataset-1.2.8/pq_dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:07:00.851600 pq_dataset-1.2.8/pq_dataset/dataset_handling/
--rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.8/pq_dataset/dataset_handling/__init__.py
--rw-rw-rw-   0        0        0     2080 2023-03-17 08:30:27.000000 pq_dataset-1.2.8/pq_dataset/dataset_handling/csv_vukvo.py
--rw-rw-rw-   0        0        0     1466 2023-02-17 09:23:10.000000 pq_dataset-1.2.8/pq_dataset/dataset_handling/ds_functions.py
--rw-rw-rw-   0        0        0     7070 2023-02-15 08:13:57.000000 pq_dataset-1.2.8/pq_dataset/dataset_handling/parquet.py
--rw-rw-rw-   0        0        0     1782 2023-03-02 11:34:33.000000 pq_dataset-1.2.8/pq_dataset/dataset_handling/pd_clean_up_columns.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:07:00.862577 pq_dataset-1.2.8/pq_dataset/logging/
--rw-rw-rw-   0        0        0       97 2023-02-14 11:10:45.000000 pq_dataset-1.2.8/pq_dataset/logging/DummyLogger.py
--rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.8/pq_dataset/logging/__init__.py
--rw-rw-rw-   0        0        0     1469 2023-02-15 08:46:43.000000 pq_dataset-1.2.8/pq_dataset/logging/logger_setup.py
--rw-rw-rw-   0        0        0    16404 2023-03-17 08:31:32.000000 pq_dataset-1.2.8/pq_dataset/pq_dataset.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:07:00.874262 pq_dataset-1.2.8/pq_dataset/pqd_functions/
--rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.8/pq_dataset/pqd_functions/__init__.py
--rw-rw-rw-   0        0        0     1973 2023-02-15 15:57:10.000000 pq_dataset-1.2.8/pq_dataset/pqd_functions/extract_calculated_from_report_spec.py
--rw-rw-rw-   0        0        0     1939 2023-02-17 08:35:44.000000 pq_dataset-1.2.8/pq_dataset/pqd_functions/reduce_columns_based_on_input.py
--rw-rw-rw-   0        0        0     3184 2023-03-28 10:05:11.000000 pq_dataset-1.2.8/pq_dataset/room_specific_config.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:07:00.885371 pq_dataset-1.2.8/pq_dataset/utils/
--rw-rw-rw-   0        0        0      589 2023-02-13 12:36:26.000000 pq_dataset-1.2.8/pq_dataset/utils/InputFile.py
--rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.8/pq_dataset/utils/__init__.py
--rw-rw-rw-   0        0        0     4096 2023-02-17 13:03:23.000000 pq_dataset-1.2.8/pq_dataset/utils/variable_overview.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:07:00.831548 pq_dataset-1.2.8/pq_dataset.egg-info/
--rw-rw-rw-   0        0        0      224 2023-03-28 10:07:00.000000 pq_dataset-1.2.8/pq_dataset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-03-28 10:07:00.000000 pq_dataset-1.2.8/pq_dataset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 10:07:00.000000 pq_dataset-1.2.8/pq_dataset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-28 10:07:00.000000 pq_dataset-1.2.8/pq_dataset.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-28 10:07:00.000000 pq_dataset-1.2.8/pq_dataset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 10:07:00.890371 pq_dataset-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      588 2023-03-28 10:05:43.000000 pq_dataset-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:17:13.788955 pq_dataset-1.2.9/
+-rw-rw-rw-   0        0        0      224 2023-08-04 11:17:13.782344 pq_dataset-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2022-11-29 07:52:53.000000 pq_dataset-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 11:17:13.070405 pq_dataset-1.2.9/pq_dataset/
+-rw-rw-rw-   0        0        0        0 2023-02-15 06:36:59.000000 pq_dataset-1.2.9/pq_dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:17:13.357936 pq_dataset-1.2.9/pq_dataset/dataset_handling/
+-rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.9/pq_dataset/dataset_handling/__init__.py
+-rw-rw-rw-   0        0        0     1873 2023-06-13 07:42:12.000000 pq_dataset-1.2.9/pq_dataset/dataset_handling/csv_vukvo.py
+-rw-rw-rw-   0        0        0     1442 2023-08-04 11:01:51.000000 pq_dataset-1.2.9/pq_dataset/dataset_handling/ds_functions.py
+-rw-rw-rw-   0        0        0     7289 2023-08-04 11:10:58.000000 pq_dataset-1.2.9/pq_dataset/dataset_handling/parquet.py
+-rw-rw-rw-   0        0        0     1782 2023-03-02 11:34:33.000000 pq_dataset-1.2.9/pq_dataset/dataset_handling/pd_clean_up_columns.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:17:13.536366 pq_dataset-1.2.9/pq_dataset/logging/
+-rw-rw-rw-   0        0        0       97 2023-02-14 11:10:45.000000 pq_dataset-1.2.9/pq_dataset/logging/DummyLogger.py
+-rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.9/pq_dataset/logging/__init__.py
+-rw-rw-rw-   0        0        0     1469 2023-02-15 08:46:43.000000 pq_dataset-1.2.9/pq_dataset/logging/logger_setup.py
+-rw-rw-rw-   0        0        0    16565 2023-08-04 11:10:26.000000 pq_dataset-1.2.9/pq_dataset/pq_dataset.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:17:13.640212 pq_dataset-1.2.9/pq_dataset/pqd_functions/
+-rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.9/pq_dataset/pqd_functions/__init__.py
+-rw-rw-rw-   0        0        0     1973 2023-02-15 15:57:10.000000 pq_dataset-1.2.9/pq_dataset/pqd_functions/extract_calculated_from_report_spec.py
+-rw-rw-rw-   0        0        0     1939 2023-02-17 08:35:44.000000 pq_dataset-1.2.9/pq_dataset/pqd_functions/reduce_columns_based_on_input.py
+-rw-rw-rw-   0        0        0     3175 2023-08-04 10:19:44.000000 pq_dataset-1.2.9/pq_dataset/room_specific_config.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:17:13.772350 pq_dataset-1.2.9/pq_dataset/utils/
+-rw-rw-rw-   0        0        0      589 2023-02-13 12:36:26.000000 pq_dataset-1.2.9/pq_dataset/utils/InputFile.py
+-rw-rw-rw-   0        0        0        0 2023-02-06 11:39:18.000000 pq_dataset-1.2.9/pq_dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0     4096 2023-02-17 13:03:23.000000 pq_dataset-1.2.9/pq_dataset/utils/variable_overview.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:17:13.193047 pq_dataset-1.2.9/pq_dataset.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-08-04 11:17:11.000000 pq_dataset-1.2.9/pq_dataset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-08-04 11:17:12.000000 pq_dataset-1.2.9/pq_dataset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:17:11.000000 pq_dataset-1.2.9/pq_dataset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-08-04 11:17:11.000000 pq_dataset-1.2.9/pq_dataset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 11:17:11.000000 pq_dataset-1.2.9/pq_dataset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:17:13.789919 pq_dataset-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      588 2023-08-04 11:15:50.000000 pq_dataset-1.2.9/setup.py
```

### Comparing `pq_dataset-1.2.8/pq_dataset/dataset_handling/csv_vukvo.py` & `pq_dataset-1.2.9/pq_dataset/dataset_handling/csv_vukvo.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,46 +7,42 @@
 from pq_dataset.dataset_handling.pd_clean_up_columns import pd_clean_up_columns
 from pq_dataset.utils.variable_overview import VariableOverview
 
 @dataclass
 class CsvVukvoDataset:
     input_file: str
     json_file: str
-    
+
     def __post_init__(self):
 
         if not InputFile(self.input_file).valid():
             raise OSError(f'{self.input_file} not found')
-        
+
     def load(self):
         raise NotImplementedError
-    
+
     def load_as_pandas_df(self, columns_subset: List[str] = [], root_var: str = '') -> pd.DataFrame:
-        
+
         def generate_var_overview(json_file: str) -> pd.DataFrame:
             return VariableOverview(json_file).var_overview
 
         def clean_root_data(df: pd.DataFrame, root_var: str) -> pd.DataFrame:
             query_string = f'{root_var}.notnull()'
             try:
                 df2 = df.query(query_string)
-            except KeyError: 
+            except KeyError:
                 # self.logger.debug('clean_root_data tried to filter df, but variable does not exist')
                 return df
             # self.logger.debug(f'clean_root_data removed {self.data.shape[0] - df2.shape[0]} cases from dataframe')
             return df2
-        
+
         if columns_subset:
             df = pd.read_csv(self.input_file, use_cols=columns_subset, encoding='utf-8-sig', sep=';', decimal=',', low_memory=False)
         else:
             df = pd.read_csv(self.input_file, encoding='utf-8-sig', sep=';', decimal=',', low_memory=False)
-        
-        df = df.rename(columns=lambda x: re.sub('(\/)','__',x)) # Replacing / with __
+
+        df = df.rename(columns=lambda x: re.sub(r'(\/)', '__', x))  # Replacing / with __
+        df.columns = [col.lower() for col in df.columns]
         if root_var:
             df = clean_root_data(df, root_var)
         df = pd_clean_up_columns(df)
-        
-        var_overview = generate_var_overview(self.json_file)
-        colnames_dict = dict(zip(var_overview.reference, var_overview.adj_name))
-        df.rename(columns=colnames_dict, inplace=True)        
-        
         return df
```

### Comparing `pq_dataset-1.2.8/pq_dataset/dataset_handling/ds_functions.py` & `pq_dataset-1.2.9/pq_dataset/dataset_handling/ds_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,26 +11,26 @@
     dataset_types = {'.parquet': 'parquet',
                      '.zip': 'parquet',
                      '.csv': 'csv'}
     file_extension = InputFile(input_file).file_type
     return dataset_types[file_extension]
 
 def dataset_loader(input_file: str, json_file: str, columns_subset: List[str] = [], root_var: str = '') -> pd.DataFrame:
-    
+
     logger = logging.getLogger(__name__) if logging.getLogger().hasHandlers else DummyLogger()
     logger.debug(f'Started preparing dataset from file: {input_file}')
-    
+
     if not InputFile(input_file).valid():
         raise OSError(f'{input_file} not found')
-    
+
     file_type = return_dataset_type(input_file)
-    
+
     if file_type == 'parquet':
         df = ParquetDataset(input_file, json_file).load_as_pandas_df(columns_subset, root_var)
     elif file_type == 'csv':
         df = CsvVukvoDataset(input_file, json_file).load_as_pandas_df(columns_subset, root_var)
     else:
         raise ValueError(f'{file_type} is not supported')
-    
+
     logger.debug(f'Done loading {input_file} (type: {file_type}) as pd.DataFrame')
-    
+
     return df
```

### Comparing `pq_dataset-1.2.8/pq_dataset/dataset_handling/parquet.py` & `pq_dataset-1.2.9/pq_dataset/dataset_handling/parquet.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,129 +14,153 @@
 from pq_dataset.logging.DummyLogger import DummyLogger
 
 
 @dataclass
 class ParquetDataset:
     input_file: str
     json_file: str
-    
+
     def __post_init__(self):
-        
-        self.logger = logging.getLogger(__name__) if logging.getLogger().hasHandlers else DummyLogger()        
-        self.logger.debug(f'Instantiated {self.__class__.__name__} from {self.input_file}')
-       
+
+        self.logger = logging.getLogger(
+            __name__) if logging.getLogger().hasHandlers else DummyLogger()
+        self.logger.debug(
+            f'Instantiated {self.__class__.__name__} from {self.input_file}')
+
         if not InputFile(self.input_file).valid():
             raise OSError(f'{self.input_file} not found')
 
         self.type = InputFile(self.input_file).file_type
-        
+
     def load(self) -> pa.Table:
         return self.__read_file_to_table()
 
     def load_as_pandas_df(self, columns_subset: List[str] = [], root_var: str = '') -> pd.DataFrame:
-        
-        self.logger.debug(f'Started loading parquet file as pandas df')
-        
+
+        self.logger.debug('Started loading parquet file as pandas df')
+
         def generate_var_overview(json_file: str) -> pd.DataFrame:
             return VariableOverview(json_file).var_overview
-        
+
         if not columns_subset:
             try:
                 df = self.__read_file_to_table(root_var=root_var).to_pandas()
             except MemoryError:
-                raise MemoryError(f'{self.input_file} cannot be read due to memory issues. Consider reducing the amount of columns')
+                raise MemoryError(
+                    f'{self.input_file} cannot be read due to memory issues. Consider reducing the amount of columns')
         else:
-            columns_subset_renamed = self.__convert_varnames_to_varrefs(columns_subset)
-            df = self.__read_file_to_table(columns_subset_renamed, root_var).to_pandas()
+            columns_subset_renamed = self.__convert_varnames_to_varrefs(
+                columns_subset)
+            df = self.__read_file_to_table(
+                columns_subset_renamed, root_var).to_pandas()
 
         var_overview = generate_var_overview(self.json_file)
-        colnames_dict = dict(zip(var_overview.reference, var_overview.adj_name))
+        colnames_dict = dict(
+            zip(var_overview.reference, var_overview.adj_name))
         df.rename(columns=colnames_dict, inplace=True)
-        
-        self.logger.debug(f'Finished loading parquet file as pandas df')
+
+        self.logger.debug('Finished loading parquet file as pandas df')
         return df
-    
+
     def __convert_varnames_to_varrefs(self, list_of_cols: List[str]) -> List[str]:
         var_map = VariableOverview(self.json_file).var_map
         list_of_varsrefs = [var_map[col] for col in list_of_cols]
         return list_of_varsrefs
 
     def __read_file_to_table(self, columns_subset: List[str] = [], root_var: str = '') -> pa.Table:
-        
+
         def clean_up_root_variable(pa_table: pa.Table, root_var: str) -> pa.Table:
-            root_var_renamed = self.__convert_varnames_to_varrefs([root_var])[0]
+            root_var_renamed = self.__convert_varnames_to_varrefs([root_var])[
+                0]
             exp = pc.is_valid(pa_table.column(root_var_renamed))
             table_temp = pa_table.filter(exp)
-            self.logger.debug(f'clean_up_root_variable deleted {pa_table.num_rows-table_temp.num_rows} cases where {root_var} is null')
+            self.logger.debug(
+                f'clean_up_root_variable deleted {pa_table.num_rows-table_temp.num_rows} cases where {root_var} is null')
             return table_temp
 
         def drop_columns_with_all_nulls(pa_table: pa.Table) -> pa.Table:
-            columns_with_all_nulls = [col_name for col_name in pa_table.column_names if pc.count(pa_table.column(col_name), mode='only_null').as_py() == pa_table.num_rows]
-            self.logger.debug(f'drop_columns_with_all_nulls deleted {len(columns_with_all_nulls)} columns')
+            columns_with_all_nulls = [col_name for col_name in pa_table.column_names if pc.count(
+                pa_table.column(col_name), mode='only_null').as_py() == pa_table.num_rows]
+            self.logger.debug(
+                f'drop_columns_with_all_nulls deleted {len(columns_with_all_nulls)} columns')
             return pa_table.drop(columns_with_all_nulls)
-        
+
         def drop_static_zero_columns(pa_table: pa.Table) -> pa.Table:
             static_cols: List[str] = []
-            numeric_cols = [col for col in pa_table.column_names if pa_table.column(col).type not in ['binary', 'string']]
+            numeric_cols = [col for col in pa_table.column_names if pa_table.column(
+                col).type not in ['binary', 'string']]
             for col in numeric_cols:
                 if pc.count_distinct(pa_table.column(col), mode='all').as_py() == 1:
                     if pc.mean(pa_table.column(col)).as_py() == 0:
                         static_cols.append(col)
-            self.logger.debug(f'drop_static_zero_columns deleted {len(static_cols)} columns')
+            self.logger.debug(
+                f'drop_static_zero_columns deleted {len(static_cols)} columns')
             return pa_table.drop(static_cols)
-        
+
         def drop_static_ptypets(pa_table: pa.Table, var_map: dict['str': 'str']) -> pa.Table:
-            ptypes = {key: var_map[key] for key in var_map if key.startswith('background__ptype')}
-            ptypes_reduced = {key: ptypes[key] for key, value in ptypes.items() if value in pa_table.column_names}
-            binary_cols = [col for col in list(ptypes_reduced.values()) if pa_table.column(col).type in ['binary', 'string']]
+            ptypes = {key: var_map[key] for key in var_map if key.startswith(
+                'background__ptype')}
+            ptypes_reduced = {key: ptypes[key] for key, value in ptypes.items(
+            ) if value in pa_table.column_names}
+            binary_cols = [col for col in list(ptypes_reduced.values(
+            )) if pa_table.column(col).type in ['binary', 'string']]
             cols_to_drop: List[str] = []
             for col in binary_cols:
                 if pc.count_distinct(pa_table.column(col), mode='all').as_py() == 1:
                     cols_to_drop.append(col)
 
-            cols_to_drop.extend([ptypes_reduced[col[:-1]] for col, value in ptypes_reduced.items() if value in cols_to_drop])            
-            self.logger.debug(f'drop_static_ptypets deleted {len(cols_to_drop)} columns')
+            cols_to_drop.extend([ptypes_reduced[col[:-1]] for col,
+                                value in ptypes_reduced.items() if value in cols_to_drop])
+            self.logger.debug(
+                f'drop_static_ptypets deleted {len(cols_to_drop)} columns')
             return pa_table.drop(cols_to_drop)
-        
+
         def convert_binaries_to_strings(pa_table: pa.Table) -> pa.Table:
-            binary_cols = [col for col in pa_table.column_names if pa_table.column(col).type == 'binary']
+            binary_cols = [col for col in pa_table.column_names if pa_table.column(
+                col).type == 'binary']
             for col in binary_cols:
-                decoded = pc.cast(pa_table.column(col), target_type=pa.string())
-                pa_table = pa_table.set_column(pa_table.schema.get_field_index(col), col, decoded)
-            self.logger.debug(f'Converted all binary columns to utf-8 strings')
+                decoded = pc.cast(pa_table.column(
+                    col), target_type=pa.string())
+                pa_table = pa_table.set_column(
+                    pa_table.schema.get_field_index(col), col, decoded)
+            self.logger.debug('Converted all binary columns to utf-8 strings')
             return pa_table
-            
+
         file_name = InputFile(self.input_file).full_path_filename
         file_path = InputFile(self.input_file).full_path
-        
-        self.logger.debug(f'__read_file_to_table started handling parqet file of type: {self.type}')
-        
+
+        self.logger.debug(
+            f'__read_file_to_table started handling parqet file of type: {self.type}')
+
         if self.type == '.zip':
-            
+
             with ZipFile(file_name, 'r') as zip_obj:
                 zip_obj.extractall('temp_parq')
 
-            self.logger.debug(f'Finished extracting zip-archive')
+            self.logger.debug('Finished extracting zip-archive')
 
             upd_path = Path(file_path) / 'temp_parq'
-            table = pq.ParquetDataset(Path(upd_path)).read(columns=columns_subset) if columns_subset else pq.ParquetDataset(Path(upd_path)).read()
-            self.logger.debug(f'Loaded unpacked files as table')
-            
+            table = pq.ParquetDataset(Path(upd_path)).read(
+                columns=columns_subset) if columns_subset else pq.ParquetDataset(Path(upd_path)).read()
+            self.logger.debug('Loaded unpacked files as table')
+
             if Path(upd_path).exists():
-                shutil.rmtree(upd_path)    
-            self.logger.debug(f'Deleted unpacked files and folder')
-            
+                shutil.rmtree(upd_path)
+            self.logger.debug('Deleted unpacked files and folder')
+
         elif self.type == '.parquet':
-            
-            table = pq.read_table(file_name, columns=columns_subset) if columns_subset else pq.read_table(file_name)
+
+            table = pq.read_table(
+                file_name, columns=columns_subset) if columns_subset else pq.read_table(file_name)
 
         # Stupid - vildere klovn vildere
         if root_var:
             table = clean_up_root_variable(table, root_var)
         # erstat med functools.reduce
         table = drop_columns_with_all_nulls(table)
         table = drop_static_zero_columns(table)
-        table = drop_static_ptypets(table, VariableOverview(self.json_file).var_map)
+        table = drop_static_ptypets(
+            table, VariableOverview(self.json_file).var_map)
         table = convert_binaries_to_strings(table)
-            
-        self.logger.debug(f'__read_file_to_table finished')
-        return table
+
+        self.logger.debug('__read_file_to_table finished')
+        return table
```

### Comparing `pq_dataset-1.2.8/pq_dataset/dataset_handling/pd_clean_up_columns.py` & `pq_dataset-1.2.9/pq_dataset/dataset_handling/pd_clean_up_columns.py`

 * *Files identical despite different names*

### Comparing `pq_dataset-1.2.8/pq_dataset/logging/logger_setup.py` & `pq_dataset-1.2.9/pq_dataset/logging/logger_setup.py`

 * *Files identical despite different names*

### Comparing `pq_dataset-1.2.8/pq_dataset/pq_dataset.py` & `pq_dataset-1.2.9/pq_dataset/pq_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,342 +15,376 @@
 from pq_dataset.utils.variable_overview import VariableOverview
 from pq_dataset.dataset_handling.ds_functions import dataset_loader, return_dataset_type
 from pq_dataset.dataset_handling.pd_clean_up_columns import pd_clean_up_columns
 from pq_dataset.utils.InputFile import InputFile
 from pq_dataset.pqd_functions.reduce_columns_based_on_input import reduce_columns_based_on_input
 from pq_dataset.logging.logger_setup import start_logging
 
+
 @dataclass
 class PQDataset:
-    """A class making it easier to work with dataset from H&H. 
-    
+    """A class making it easier to work with dataset from H&H.
+
     Attributes
     ----------
     input_file: int
         The file containing data.
     json_file: str
         json map of variables from graphQL query
     input_path: str
         Path of the input files (datasets, json strings with grapql export etc.)
     output_path: str
         Path of the output_path files generated
     room_id: int
-        The source of the datasets - 
-        491, 729 or 999999 are valid entries. 999999 indicates non-H&H Results room. 
+        The source of the datasets -
+        491, 729 or 999999 are valid entries. 999999 indicates non-H&H Results room.
     debug: bool, default: False
         If True debugging information is logged to file
     relevant_scopes: List[str]
-        List of strings matching scopes or parts of scopes. Every variable matching the string will be included in the dataframe. 
+        List of strings matching scopes or parts of scopes. Every variable matching the string will be included in the dataframe.
         E.g. 'background__ptype' includes every ptype variable
     relevant_variables: List[str]
         List of variables to be included in the dataframe
-        
+
     Output
     ------
     When initiated this class adds two dataframes to the class.
     .data which holds the data as a pandas dataframe
     .var_overview which holds a variable overview of the full dataset
-    
+
     E.g. 'sprog = PQDataset()' allows for sprog.data and sprog.var_overview to be called
-    
+
     Methods
     -------
     The class have the following methods which can be called
-    
+
     .clients_only(): Returns a dataset which only contains clients data - the selection depends on the room (491 or 729)
     .identify_relevante_data_ftp(): Allows for identifying which variables are relevant for data which are to be made avaiable for our clients
-    .create_json_ftp_config(): 
-    
+    .create_json_ftp_config():
+
     Config
     ------
     The file room_specific_config.py holds basic configuration for each of the allowed Results rooms
-   
-    
+
+
     """
-    
+
     input_file: str
     json_file: str
     input_path: str
     output_path: str
     room_id: int
     debug: bool = False
     relevant_scopes: Optional[List[str]] = None
     relevant_variables: Optional[List[str]] = None
-    
+
     def __post_init__(self):
         # Move most of this to main()
         os.chdir(self.input_path)
         self.file_extensions = ['.csv', '.zip', '.parquet']
         self.accepted_rooms = [491, 729, 999999]
-        
+
         start_logging(self.input_file, self.debug)
-                        
+
         self.logger = logging.getLogger(__name__)
-        self.logger.info(f'*** START *** Initializing PQDataset from file: {self.input_file}')
-        
+        self.logger.info(
+            f'*** START *** Initializing PQDataset from file: {self.input_file}')
+
         self.file_type = return_dataset_type(self.input_file)
-       
+
         if not self.__validate_inputs():
             self.logger.error('Invalid inputs found')
             raise ValueError('Unrecognized inputs')
-        
+
         self.config = room_config.setup_config(self.room_id)
-        self.var_map = VariableOverview(self.json_file).var_map # Probably no need for making this a class attribute
+        # Probably no need for making this a class attribute
+        self.var_map = VariableOverview(self.json_file).var_map
         self.data = self.__load_data()
         # self.data = self.__clean_root_data() #Already implemented for parquet - csv_vukvo still needs implementation
 
-        self.logger.info(f'*** END *** Done preparing data from {self.input_file}. You can access the dataframe by appending .data to the object that you created - i.e. barnbg.data')
-  
+        self.logger.info(
+            f'*** END *** Done preparing data from {self.input_file}. You can access the dataframe by appending .data to the object that you created - i.e. barnbg.data')
+
     def __load_data(self) -> pd.DataFrame:
-        root_var = self.__return_config_parameter('root_variable')[0] if self.__return_config_parameter('root_variable') else ''
+        root_var = self.__return_config_parameter(
+            'root_variable')[0] if self.__return_config_parameter('root_variable') else ''
         if self.relevant_scopes or self.relevant_variables:
             list_of_cols = list(self.__create_dict_of_cols())
             return dataset_loader(self.input_file, self.json_file, columns_subset=list_of_cols, root_var=root_var)
         else:
             return dataset_loader(self.input_file, self.json_file, root_var=root_var)
 
     def __create_dict_of_cols(self) -> dict[str: str]:
         # Not exactly needed as renaming of variables in parquet datasets have been moved to dataset_handling
         relevant_cols = {}
 
         if self.relevant_scopes:
             for scope in self.relevant_scopes:
-                temp_cols = {var: self.var_map[var] for var in self.var_map if var.startswith(scope)}
+                temp_cols = {var: self.var_map[var]
+                             for var in self.var_map if var.startswith(scope)}
             if not temp_cols:
-                self.logger.warning(f'No variables starting with {self.relevant_scopes} was found in data')
+                self.logger.warning(
+                    f'No variables starting with {self.relevant_scopes} was found in data')
             else:
                 relevant_cols.update(temp_cols)
 
         if self.relevant_variables:
-            temp_vars = {var: self.var_map[var] for var in self.var_map if var in self.relevant_variables}
+            rel_vars_lower = [var.lower() for var in self.relevant_variables]
+            temp_vars = {
+                var: self.var_map[var] for var in self.var_map if var in rel_vars_lower}
             if not temp_vars:
-                self.logger.warning(f'No variables from {self.relevant_variables} was found in data')
+                self.logger.warning(
+                    f'No variables from {self.relevant_variables} was found in data')
             else:
-                relevant_cols.update(temp_vars)    
+                relevant_cols.update(temp_vars)
 
         return relevant_cols
-    
+
     def __create_list_of_config_vars(self, include_cpr: bool = True) -> List[str]:
         config_vars_to_include: List[str] = []
 
         if include_cpr:
             for var in self.__return_config_parameter('cpr_variables'):
                 if var in self.data.columns:
                     config_vars_to_include.append(var)
-        
+
         # Appending variables which should always be included
-        config_vars_to_include.extend(self.__return_config_parameter('must_include_variables'))
+        config_vars_to_include.extend(
+            self.__return_config_parameter('must_include_variables'))
 
         # Adding room specific variables to be indcluded in dataset
-        config_vars_to_include.extend(self.__return_config_parameter('room_specific_variables'))        
+        config_vars_to_include.extend(
+            self.__return_config_parameter('room_specific_variables'))
 
         return config_vars_to_include
 
     def __validate_inputs(self) -> bool:
-        
+
         if not InputFile(self.input_file).valid():
             self.logger.critical(f'{self.input_file} is not valid ')
             return False
         if not InputFile(self.json_file).valid():
-            self.logger.critical(f'{self.json_file} is not valid ')        
+            self.logger.critical(f'{self.json_file} is not valid ')
             return False
         if not Path(self.input_path).exists():
             self.logger.critical(f'The path {self.input_path} does not exist.')
             return False
         if not Path(self.output_path).exists():
-            self.logger.critical(f'The path {self.output_path} does not exist.')
+            self.logger.critical(
+                f'The path {self.output_path} does not exist.')
             return False
-        if not self.room_id in self.accepted_rooms:
+        if self.room_id not in self.accepted_rooms:
             self.logger.critical(f'Unknown room id {self.room_id}')
             return False
-        self.logger.debug(f'All inputs are ok.')
+        self.logger.debug('All inputs are ok.')
         return True
-    
+
     def __return_config_parameter(self, parameter_name: str) -> List[str]:
-        return self.config.get(parameter_name)    
-    
+        return self.config.get(parameter_name)
+
     def clean_up_data(self,
                       clients_only: bool = True,
                       remove_testareas: bool = True,
                       remove_archive: bool = False,
                       predaycare_only: bool = False,
                       relevant_scopes: List[str] = [],
                       relevant_variables: List[str] = []) -> pd.DataFrame:
         """Missing description
-        
-        
-        
-        
+
+
+
+
         """
-        
+
         def general_setup_check(df: pd.DataFrame, parameter_bool: bool, parameter_variables: List[str]) -> bool:
 
             parameter_should_be_included_in_query = True
-            
+
             if not parameter_bool:
-                self.logger.debug(f'clean_up_data: Skipping parameter as it is false')
+                self.logger.debug(
+                    'clean_up_data: Skipping parameter as it is false')
                 parameter_should_be_included_in_query = False
                 return parameter_should_be_included_in_query
-            
+
             if not parameter_variables:
-                self.logger.debug(f'clean_up_data: List of variables is empty')
+                self.logger.debug('clean_up_data: List of variables is empty')
                 parameter_should_be_included_in_query = False
                 return parameter_should_be_included_in_query
-            
-            variables_in_df = [var for var in parameter_variables if var in df.columns]
-            
+
+            variables_in_df = [
+                var for var in parameter_variables if var in df.columns]
+
             if not variables_in_df:
-                self.logger.debug(f'clean_up_data: None of the variables supplied is present in dataframe')                
+                self.logger.debug(
+                    'clean_up_data: None of the variables supplied is present in dataframe')
                 parameter_should_be_included_in_query = False
                 return parameter_should_be_included_in_query
-            
+
             return parameter_should_be_included_in_query
-       
+
         def parse_testarea_setup(df: pd.DataFrame, remove_testareas: bool, testarea_variables: List[str]) -> str:
-            
+
             if general_setup_check(df, remove_testareas, testarea_variables):
-                
-                testarea_variables_reduced = [var for var in testarea_variables if var in df.columns]
-                testarea_variables_queries = [f'not({col}.str.startswith("*Test", na=False).values)' for col in testarea_variables_reduced]
+
+                testarea_variables_reduced = [
+                    var for var in testarea_variables if var in df.columns]
+                testarea_variables_queries = [
+                    f'not({col}.str.startswith("*Test", na=False).values)' for col in testarea_variables_reduced]
                 testarea_query = ' and '.join(testarea_variables_queries)
                 return testarea_query
-            
-            return None             
-        
+
+            return None
+
         def parse_archive_setup(df: pd.DataFrame, remove_archive: bool, archive_variables: List[str]) -> str:
-            
+
             if general_setup_check(df, remove_archive, archive_variables):
-                
-                archive_variables_reduced = [var for var in archive_variables if var in df.columns]
-                archive_queries = [f'{var}.isnull()' for var in archive_variables_reduced if var in df.columns]
-                
+
+                archive_variables_reduced = [
+                    var for var in archive_variables if var in df.columns]
+                archive_queries = [
+                    f'{var}.isnull()' for var in archive_variables_reduced if var in df.columns]
+
                 archive_query = ' and '.join(archive_queries)
-                
+
                 return archive_query
-            
+
             return None
 
-        query_string_total  = []
+        query_string_total = []
         archive_variables = self.__return_config_parameter('archive_variables')
-        testarea_variables = self.__return_config_parameter('testarea_variables')
-        
+        testarea_variables = self.__return_config_parameter(
+            'testarea_variables')
+
         df = self.data
 
         if clients_only:
             clients_query = self.__return_config_parameter('clients_query')
             if clients_query:
                 query_string_total.append(f'{clients_query[0]}')
-            
+
         if parse_archive_setup(df, remove_archive, archive_variables):
-            query_string_total.append(f'({parse_archive_setup(df, remove_archive, archive_variables)})')
+            query_string_total.append(
+                f'({parse_archive_setup(df, remove_archive, archive_variables)})')
 
         if parse_testarea_setup(df, remove_testareas, testarea_variables):
-            query_string_total.append(f'({(parse_testarea_setup(df, remove_testareas, testarea_variables))})')
+            query_string_total.append(
+                f'({(parse_testarea_setup(df, remove_testareas, testarea_variables))})')
 
         if query_string_total:
             query_string_total_str = ' and '.join(query_string_total)
             df_temp = df.query(f'{query_string_total_str}', engine='python')
         else:
             df_temp = df
 
         if relevant_scopes or relevant_variables:
             relevant_variables.extend(self.__create_list_of_config_vars())
-            df_temp = reduce_columns_based_on_input(df_temp, relevant_scopes, relevant_variables)
+            df_temp = reduce_columns_based_on_input(
+                df_temp, relevant_scopes, relevant_variables)
 
         return df_temp
-    
-    def identify_relevante_data_ftp(self, 
+
+    def identify_relevante_data_ftp(self,
                                     analysis_id: int,
-                                    reduced_data: pd.DataFrame = None, 
-                                    relevant_scopes: List[str] = ['background__ptype', 'questionnaire__'],
+                                    reduced_data: pd.DataFrame = None,
+                                    relevant_scopes: List[str] = [
+                                        'background__ptype', 'questionnaire__'],
                                     relevant_variables: List[str] = [],
                                     include_calculated_from_report: str = '',
                                     save_variable_overview: bool = True
                                     ) -> None:
-        """Prepares and returns client relevant dataset (pandas dataframe) and variables. 
-        
+        """Prepares and returns client relevant dataset (pandas dataframe) and variables.
+
         Parameters
         ----------
         analysis_id: int
 
         reduced_data : pd.DataFrame, optional (default=None)
-            Useful if 
+            Useful if
         relevant_scopes : List[str], optional (default=[background__ptype] and [questionnaire__])
             Specifies which scopes should be included. If not specified then [background__ptype] and [questionnaire__] scope is included.
         relevant_variables : List[str], optional (default=None)
             Specifies which specfic variables should be included. This is used if only certain variables from a specific scope are relevant
         include_calculated_from_report : str, optional (default=None)
             This is useful for a 'automated' mode for indentifying relevant variables. The supplied string should be the name of the file with the xml config of the relevant report. In most cases this would be the report on child level and not aggregated.
         save_variable_overview : bool, optional (default=True)
-            Whether or not an excel-file with a description of the included variables should be saved.  
-        
+            Whether or not an excel-file with a description of the included variables should be saved.
+
         """
-        self.logger.info(f'Started identify_relevant_data_ftp')
-        
-        if not reduced_data is None:
+        self.logger.info('Started identify_relevant_data_ftp')
+
+        if reduced_data is not None:
             df = pd_clean_up_columns(reduced_data)
         else:
             df = self.data
 
         if include_calculated_from_report:
-            used_calc_vars = extract_calculated_from_report_spec(self.input_path, include_calculated_from_report, analysis_id, VariableOverview(self.json_file).var_overview)
+            used_calc_vars = extract_calculated_from_report_spec(
+                self.input_path, include_calculated_from_report, analysis_id, VariableOverview(self.json_file).var_overview)
             relevant_variables.extend(used_calc_vars)
 
         relevant_variables.extend(self.__create_list_of_config_vars())
-        df = reduce_columns_based_on_input(df, relevant_scopes, relevant_variables)
-        
+        df = reduce_columns_based_on_input(
+            df, relevant_scopes, relevant_variables)
+
         self.data_ftp = df
         var_overview = VariableOverview(self.json_file).var_overview
-        self.var_overview_reduced = var_overview[var_overview['adj_name'].isin(self.data_ftp.columns)]
-        
+        self.var_overview_reduced = var_overview[var_overview['adj_name'].isin(
+            self.data_ftp.columns)]
+
         if save_variable_overview:
             file_name = f'{InputFile(self.input_file).file_name_wo_ext}_variabel_beskrivelse.xlsx'
             file_path = f'{self.output_path}\{file_name}'
-            relevant_cols = ['adj_name', 'name', 'referenceType', 'text', 'choice_value']
+            relevant_cols = ['adj_name', 'name',
+                             'referenceType', 'text', 'choice_value']
             try:
-                self.var_overview_reduced[relevant_cols].to_excel(file_path, index=False)
-                self.logger.info(f'Saved description of variables to be transferred to ftp as {file_path}')
+                self.var_overview_reduced[relevant_cols].to_excel(
+                    file_path, index=False)
+                self.logger.info(
+                    f'Saved description of variables to be transferred to ftp as {file_path}')
             except PermissionError:
-                self.logger.info(f'Error saving file as a file with ({file_name}) is already open.')
-        
-        self.logger.info(f'Ended identify_relevant_data_ftp. Data can be accessed by appending .data_ftp to your object.')
-        
+                self.logger.info(
+                    f'Error saving file as a file with ({file_name}) is already open.')
+
+        self.logger.info(
+            'Ended identify_relevant_data_ftp. Data can be accessed by appending .data_ftp to your object.')
+
         return None
-        
+
     def create_json_ftp_config(self, name: str, analysis: int, ftp_path: str) -> None:
-        
+
         json_output = {'name': name,
-                    'analysisId': analysis,
-                    'output': ftp_path,
-                    'variables': []
-                    }
+                       'analysisId': analysis,
+                       'output': ftp_path,
+                       'variables': []
+                       }
 
         for index, row in self.var_overview_reduced.iterrows():
             if row['referenceType'] == 'TypeChoiceSingle':
                 continue
-            json_output['variables'].append({'reference':row['reference'], 'displayName':row['adj_name']})
+            json_output['variables'].append(
+                {'reference': row['reference'], 'displayName': row['adj_name']})
 
         file_name = f'{InputFile(self.input_file).file_name_wo_ext}_ftp_config.json'
 
         json_output_file = self.output_path + os.path.sep + file_name
 
-        with codecs.open(json_output_file,'w','UTF-8-SIG') as outfile:
+        with codecs.open(json_output_file, 'w', 'UTF-8-SIG') as outfile:
             json.dump(json_output, outfile, indent=4)
-            
+
         print(f'Json file saved as {file_name} in {self.output_path}')
 
         return None
-    
+
+
 if __name__ == '__main__':
-    
+
     print('Running basic functions for development purposes and for demonstration of the basic functions')
     inputs = r'C:\Users\ctf\pq_data\sprog'
     outputs = r'C:\Users\ctf\pq_data\sprog\1_outputs'
-    
+
     testData = PQDataset(
         '1963749.zip',
         '1963749.json',
         inputs,
         outputs,
         729
-        )
-
+    )
```

### Comparing `pq_dataset-1.2.8/pq_dataset/pqd_functions/extract_calculated_from_report_spec.py` & `pq_dataset-1.2.9/pq_dataset/pqd_functions/extract_calculated_from_report_spec.py`

 * *Files identical despite different names*

### Comparing `pq_dataset-1.2.8/pq_dataset/pqd_functions/reduce_columns_based_on_input.py` & `pq_dataset-1.2.9/pq_dataset/pqd_functions/reduce_columns_based_on_input.py`

 * *Files identical despite different names*

### Comparing `pq_dataset-1.2.8/pq_dataset/room_specific_config.py` & `pq_dataset-1.2.9/pq_dataset/room_specific_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List
 
 def setup_config(room_id: int) -> Dict[str, List[str]]:
     """Setup room specific configuration
-    
+
     Config types
     ------------
     root_variable : string
         Variable which may not be null - this might be redundant. Consider logging to check if this actually removes cases.
     closed_ptype_variable : string
         ptypeXc variables which are removed from data.
     cpr_variable : string
@@ -14,19 +14,19 @@
     room_specific_variables : List[str]
         Individual variables which are relevant for the specific room - i.e. uni id for 729
     archive_variables : List[str]
         List of variables storing information on archive ptypes
     clients_query : string
         Query string selecting only client area(s)
     testarea_variables : List[str]
-        List of variables from which test areas should be removed 
+        List of variables from which test areas should be removed
+
 
-    
     """
-    
+
     room_specific_config = {
         'root_variable': {
             491: ['background__ptype24'],
             729: ['background__ptype1'],
             2897: ['background__ptype3'],
             999999: []
         },
@@ -39,15 +39,15 @@
         'cpr_variables': {
             491: ['barnbg__cpr', 'barnbackground__cpr'],
             729: ['barnbg__cpr', 'barnbackground__cpr'],
             2897: [],
             999999: []
         },
         'room_specific_variables': {
-            491: [],
+            491: ['daginstitutionbg__inr'],
             729: ['skolebg__uni_id'],
             2897: [],
             999999: []
         },
         'consent_variables': {
             491: ['barnbg__s_2', 'barnbg__s_5'],
             729: [],
@@ -63,30 +63,30 @@
         'clients_query': {
             491: ['(background__ptype65 == 7352477)'],
             729: ['(background__ptype2 == 23318479 or background__ptype2 == 9523670 or background__ptype2 == 178975647)'],
             2897: ['(background__ptype2 == 181905908)'],
             999999: []
         },
         'testarea_variables': {
-            491: ['background__ptype20t', 'background__ptype25t'], 
+            491: ['background__ptype20t', 'background__ptype25t'],
             729: [],
             2897: [],
             999999: []
         },
         'municipality_variable': {
             491: ['background__ptype24'],
             729: ['background__ptype3'],
             2897: ['background__ptype3'],
             999999: []
         }
     }
-    
+
     config = {}
 
     # Adding the room specific configuration
     for key in room_specific_config:
         config[key] = room_specific_config[key].get(room_id)
-    
+
     # Adding general configuration types
     config['must_include_variables'] = ['respondent__created', 'respondent__closetime', 'respondent__respondentid']
-            
-    return config
+
+    return config
```

### Comparing `pq_dataset-1.2.8/pq_dataset/utils/InputFile.py` & `pq_dataset-1.2.9/pq_dataset/utils/InputFile.py`

 * *Files identical despite different names*

### Comparing `pq_dataset-1.2.8/pq_dataset/utils/variable_overview.py` & `pq_dataset-1.2.9/pq_dataset/utils/variable_overview.py`

 * *Files identical despite different names*

### Comparing `pq_dataset-1.2.8/pq_dataset.egg-info/SOURCES.txt` & `pq_dataset-1.2.9/pq_dataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pq_dataset-1.2.8/setup.py` & `pq_dataset-1.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 setuptools.setup(
     name='pq_dataset',
-    version='1.2.8',
+    version='1.2.9',
     license='MIT',
     author="Christian Frost",
     author_email='anon@anon.com',
     packages=['pq_dataset', 'pq_dataset.dataset_handling', 'pq_dataset.logging', 'pq_dataset.pqd_functions', 'pq_dataset.utils'],
     url='https://github.com/ctf76/pqdataset',
     keywords='Project for working with dataset exports',
     install_requires=[
-          'datetime',
-          'numpy',
-          'pandas',
-          'pathlib',
-          'lxml',
-          'bs4',
-          'openpyxl'
-      ],
-)
+        'pyarrow',
+        'datetime',
+        'numpy',
+        'pandas',
+        'pathlib',
+        'lxml',
+        'bs4',
+        'openpyxl'],
+)
```

