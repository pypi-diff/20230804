# Comparing `tmp/tensorage-0.0.9.tar.gz` & `tmp/tensorage-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.9.tar", last modified: Thu Aug  3 06:14:08 2023, max compression
+gzip compressed data, was "tensorage-0.1.0.tar", last modified: Fri Aug  4 10:11:01 2023, max compression
```

## Comparing `tensorage-0.0.9.tar` & `tensorage-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:14:08.458240 tensorage-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-03 06:13:57.000000 tensorage-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-03 06:13:57.000000 tensorage-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-03 06:14:08.458240 tensorage-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-03 06:13:57.000000 tensorage-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-03 06:13:57.000000 tensorage-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 06:14:08.458240 tensorage-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-08-03 06:13:57.000000 tensorage-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:14:08.458240 tensorage-0.0.9/tensorage/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/db_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     9615 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-08-03 06:13:57.000000 tensorage-0.0.9/tensorage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 06:14:08.458240 tensorage-0.0.9/tensorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-03 06:14:08.000000 tensorage-0.0.9/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:11:01.628144 tensorage-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-04 10:10:51.000000 tensorage-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-04 10:10:51.000000 tensorage-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-04 10:11:01.628144 tensorage-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-04 10:10:51.000000 tensorage-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-04 10:10:51.000000 tensorage-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 10:11:01.628144 tensorage-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-08-04 10:10:51.000000 tensorage-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:11:01.628144 tensorage-0.1.0/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:11:01.628144 tensorage-0.1.0/tensorage/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4277 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/backend/database.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/backend/storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3693 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8550 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-08-04 10:10:51.000000 tensorage-0.1.0/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:11:01.628144 tensorage-0.1.0/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-04 10:11:01.000000 tensorage-0.1.0/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-08-04 10:11:01.000000 tensorage-0.1.0/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 10:11:01.000000 tensorage-0.1.0/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-04 10:11:01.000000 tensorage-0.1.0/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-04 10:11:01.000000 tensorage-0.1.0/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.9/LICENSE` & `tensorage-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.9/setup.py` & `tensorage-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.9/tensorage/auth.py` & `tensorage-0.1.0/tensorage/auth.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.9/tensorage/db_init.py` & `tensorage-0.1.0/tensorage/db_init.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,49 +4,57 @@
 public.datasets (
     id bigint generated by default as identity not null,
     key character varying not null,
     ndim smallint not null,
     shape int[] not null,
     created_at timestamp with time zone null default now(),
     user_id uuid null,
-    is_public boolean not null default false,
+    is_shared boolean not null default false,
     constraint datasets_pkey primary key (id),
     constraint datasets_key_user_id_key unique (key, user_id),
     constraint datasets_user_id_fkey foreign key (user_id) references users (id) on delete set null
 ) tablespace pg_default;
 
   -- RLS policy
 ALTER TABLE public.datasets ENABLE ROW LEVEL SECURITY;
 CREATE POLICY "Allow all actions to the record owner" ON "public"."datasets"
 AS PERMISSIVE FOR ALL
 TO authenticated
-USING (is_public OR (auth.uid() = user_id))
-WITH CHECK (is_public OR (auth.uid() = user_id));
+USING (auth.uid() = user_id)
+WITH CHECK (auth.uid() = user_id);
+CREATE POLICY "Allow authenticated access to shared datasets" ON "public"."datasets"
+AS PERMISSIVE FOR SELECT
+TO authenticated
+USING (is_shared)
 
 
 -- tensor_float4 table
 create table
 public.tensors_float4 (
     data_id bigint not null,
     index bigint not null,
     tensor float4[] not null,
     user_id uuid not null,
-    is_public boolean not null default false,
+    is_shared boolean not null default false,
     constraint tensors_float4_pkey primary key (data_id, index, user_id),
     constraint tensors_float4_data_id_fkey foreign key (data_id) references datasets (id) on delete cascade,
     constraint tensors_float4_user_id_fkey foreign key (user_id) references users (id) on delete set null
 ) tablespace pg_default;
 
 -- RLS policy
 ALTER TABLE public.tensors_float4 ENABLE ROW LEVEL SECURITY;
 CREATE POLICY "Allow all actions to the record owner" ON "public"."tensors_float4"
 AS PERMISSIVE FOR ALL
 TO authenticated
-USING (is_public OR (auth.uid() = user_id))
-WITH CHECK (is_public OR (auth.uid() = user_id));
+USING (is_shared OR (auth.uid() = user_id))
+WITH CHECK (is_shared OR (auth.uid() = user_id));
+CREATE POLICY "Allow authenticated access to shared datasets" ON "public"."tensors_float4"
+AS PERMISSIVE FOR SELECT
+TO authenticated
+USING (is_shared)
 
 -- create the slicing database function
 CREATE OR REPLACE FUNCTION public.tensor_float4_slice(name character varying, index_low integer, index_up integer, slice_low integer[], slice_up integer[])
 RETURNS table(tensor float4[])
 AS
 $$
 DECLARE
@@ -70,15 +78,15 @@
 -- add usage statistics views
 create view
   public.user_usage_details as
 select
   users.id,
   users.email,
   datasets.key as dataset,
-  sum(pg_column_size(tensors_float4.tensor)::real) / 1024.0::double precision / 1024.0::double precision / 1024.0::double precision as total_size_gb,
+  sum(pg_column_size(tensors_float4.tensor)::real) / 1024.0::real / 1024.0::real / 1024.0::real as total_size_gb,
   pg_size_pretty(sum(pg_column_size(tensors_float4.tensor))) as size
 from
   tensors_float4
   join users on tensors_float4.user_id = users.id
   join datasets on datasets.id = tensors_float4.data_id
 group by
   users.id,
@@ -86,15 +94,15 @@
   datasets.key;
 
 create view
   public.user_usage_aggregate as
 select
   users.id,
   users.email,
-  sum(pg_column_size(tensors_float4.tensor)::real) / 1024.0::double precision / 1024.0::double precision / 1024.0::double precision as total_size_gb,
+  sum(pg_column_size(tensors_float4.tensor)::real) / 1024.0::real / 1024.0::real / 1024.0::real as total_size_gb,
   pg_size_pretty(sum(pg_column_size(tensors_float4.tensor))) as size
 from
   tensors_float4
   join users on tensors_float4.user_id = users.id
 group by
   users.id,
   users.email;
```

### Comparing `tensorage-0.0.9/tensorage/store.py` & `tensorage-0.1.0/tensorage/store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,102 @@
-from typing import TYPE_CHECKING, Tuple, Union, List
+from typing import TYPE_CHECKING, Tuple, Union, List, Optional, Any
+from typing_extensions import Literal
 from dataclasses import dataclass, field
 import warnings
 
 from tqdm import tqdm
 import numpy as np
-from postgrest.exceptions import APIError
+
+from tensorage.types import Dataset
 
 if TYPE_CHECKING:
     from tensorage.session import BackendSession
-from .types import Dataset
 
 
 @dataclass
 class TensorStore(object):
-    _session: 'BackendSession' = field(repr=False)
+    backend: 'BackendSession' = field(repr=False)
     quiet: bool = field(default=False)
 
+    engine: Union[Literal['database'], Literal['storage']] = field(default='database')
+
     # some stuff for upload
     chunk_size: int = field(default=100000, repr=False)
 
+    # add some internal metadata
+    _keys: List[str] = field(default_factory=list, repr=False)
+
     def __post_init__(self):
         # check if the schema is installed
-        with self._session as context:
-            if not context.check_schema_installed():
+        with self.backend.database() as db:
+            if not db.check_schema_installed():
                 from tensorage.db_init import SQL
                 warnings.warn(f"The schema for the TensorStore is not installed. Please connect the database and run the following script:\n\n--------8<--------\n{SQL}\n\n--------8<--------\n")
+        
+        # get the current keys
+        self.keys()
 
-    def __getitem__(self, key: Union[str, Tuple[Union[str, slice, int]]]):
+    def get_context(self):
+        raise NotImplementedError
+        if self.engine == 'database':
+            return self.backend.database()
+        elif self.engine == 'storage':
+            return self.backend.storage()
+        else:
+            raise ValueError(f"Unknown engine '{self.engine}'.")
+
+    def get_select_indices(self, key: Union[str, Tuple[Union[str, slice, int]]]) -> Tuple[str, Tuple[int, int], List[Tuple[int, int]]]:
         # first get key
         if isinstance(key, str):
+            key = (key, )
             name = key
         elif isinstance(key[0], str):
             name = key[0]
         else:
             raise KeyError('You need to pass the key as first argument.')
+
+        # use the Slicer
+        name, index, slices = StoreSlicer(self, name)(*key[1:])
         
-        # load the dataset
-        with self._session as context:
-            dataset = context.get_dataset(name)
+        # return the name, index and slices
+        return name, index, slices
 
-        # now we need to figure out, what kind of slice we need to pass
+    def __getitem__(self, key: Union[str, Tuple[Union[str, slice, int]]]):
+        # the user has to pass the key
         if isinstance(key, str):
-            index = [1, dataset.shape[0] + 1]
-            slices = [[1, dataset.shape[i] + 1] for i in range(1, dataset.ndim)]
-        
-        # handle all the tuple cases
+            key = (key, )  #make it a tuple
+            name = key
+        elif isinstance(key[0], str):
+            name = key[0]
         else:
-            # index
-            if isinstance(key[1], int):
-                index = [key[1] + 1, key[1] + 2]
-            elif isinstance(key[1], slice):
-                index = [key[1].start + 1, key[1].stop + 2]
-            else:
-                raise KeyError('Batch index needs to be passed as int or slice.')
-            
-            # slices
-            if len(key) == 2:
-                slices = [[1, dataset.shape[i] + 1] for i in range(2, dataset.ndim)]
-            else:  # more than 2
-                slices = []
-                for i, arg in enumerate(key[2:]):
-                    if isinstance(arg, int):
-                        slices.append([arg + 1, arg + 1])
-                    elif isinstance(arg, slice):
-                        slices.append([arg.start + 1 if arg.start is not None else 1, arg.stop + 1 if arg.stop is not None else dataset.shape[i + 1] + 1])
-                    else:
-                        raise KeyError('Slice needs to be passed as int or slice.')
-                
-                # check if we have all slices
-                if len(slices) + 1 != dataset.ndim:
-                    for i in range(len(slices) + 1, dataset.ndim):
-                        slices.append([1, dataset.shape[i] + 1])
-        
-        # now, name, index and slices are set
-        with self._session as context:
-            # load the tensor
-            arr = context.get_tensor(name, index[0], index[1], [s[0] for s in slices], [s[1] for s in slices])
+            raise KeyError('You need to pass the key as first argument.')
         
-        # TODO now we can transform to other libaries
-        return arr
+        # instatiate a Slicer
+        slicer = StoreSlicer(self, name)
+
+        # for now, we accept only iloc-style indexing
+        # TODO if we use the axes, we need to transform here, before instatiating the StoreSlicer
+        return slicer.__getitem__(key[1:])
+
+    def __getattr__(self, key: str):
+        # getattribute did not return anything, so now check if the key is in the keys
+        if key in self._keys:
+            return StoreSlicer(self, key)
+        else:
+            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{key}'")
+
+    def __dir__(self):
+        return super().__dir__() + self._keys
 
     def __setitem__(self, key: str, value: Union[List[list], np.ndarray]):
+        # check if the key is already in the database
+        if key in self.keys():
+            # TODO here we need to update the dataset in the database
+            raise NotImplementedError('Updating datasets is not implemented yet.')
+
         # first make a numpy array from it
         if isinstance(value, list):
             value = np.asarray(value)
 
         # make at least 2D 
         if value.ndim == 1:
             value = value.reshape(1, -1)        
@@ -108,28 +120,31 @@
             
             # build the 
             batches = [(i * batch_size, value[up:low]) for i, (up, low) in enumerate(batch_index)]
         else:
             batches = [(0, value)]
 
         # connect
-        with self._session as context:
+        with self.backend.database() as db:
             # insert the dataset
-            dataset = context.insert_dataset(key, shape, dim)
+            dataset = db.insert_dataset(key, shape, dim)
 
             # make the iterator
             _iterator = tqdm(batches, desc=f'Uploading {key} [{len(batches)} batches of {batch_size}]') if not self.quiet else batches
 
             # insert the tensor
             for offset, batch in _iterator:
-                context.insert_tensor(dataset.id, [tensor for tensor in batch], offset=offset)
-
+                db.insert_tensor(dataset.id, [tensor for tensor in batch], offset=offset)
+            
+            # finally update the keys
+            self._keys = db.list_dataset_keys()
+ 
     def __delitem__(self, key: str):
-        with self._session as context:
-            context.remove_dataset(key)
+        with self.backend.database() as db:
+            db.remove_dataset(key)
     
     def __contains__(self, key: str):
         # get the keys
         keys = self.keys()
 
         # check if key is in keys
         return key in keys
@@ -139,140 +154,86 @@
         keys = self.keys()
 
         # return the length
         return len(keys)
 
     def keys(self) -> List[str]:
         # get the keys from the database
-        with self._session as context:
-            keys = context.list_tensor_keys()
+        with self.backend.database() as db:
+            keys = db.list_dataset_keys()
         
-        # TODO: here caching could be added
+        # update the internal keys list
+        self._keys = keys
+
         return keys
 
 
 @dataclass
-class StoreContext(object):
-    # This is the OPENED session, as we are in the StoreContext
-    backend: 'BackendSession' = field(repr=False)
-    _anon_key: str = field(init=False, repr=False)
+class StoreSlicer:
+    _store: TensorStore = field(repr=False)
+    key: str
+    dataset: Optional[Dataset] = field(default=None, repr=False)
 
-    def __setup_auth(self):
-        # store the current JWT token
-        self._anon_key = self.backend.client.supabase_key
+    def __post_init__(self):
+        if self.dataset is None:
+            with self._store.backend.database() as db:
+                self.dataset = db.get_dataset(self.key)
+
+    def get_iloc_slices(self, *args: Union[int, Tuple[int], slice]) -> Tuple[str, Tuple[int, int], List[Tuple[int, int]]]:
+        # check the length of the args
+        if len(args) == 0:
+            # use the dataset to load the full sample
+            return (
+                self.key, 
+                [1, self.dataset.shape[0] + 1], 
+                [[1, self.dataset.shape[i] + 1] for i in range(1, self.dataset.ndim)]
+            )
+
+        # slicing is actually needed
+        
+        # get the index
+        if isinstance(args[0], int):
+            index = [args[0] + 1, args[0] + 2]
+        elif isinstance(args[0], slice):
+            index = [args[0].start + 1, args[0].stop + 2]
+        else:
+            raise KeyError('Batch index needs to be passed as int or slice.')
 
-        # set the JWT of the authenticated user as the new token
-        self.backend.client.postgrest.auth(self.backend._session.access_token)
-    
-    def __restore_auth(self):
-        # restore the original JWT
-        self.backend.client.postgrest.auth(self._anon_key)
-
-    def check_schema_installed(self) -> bool:
-        # setup auth token
-        self.__setup_auth()
-
-        # check if the datasets and tensor_float4 tables exist
-        missing_table = False
-
-        for table in ('datasets', 'tensors_float4'):
-            try:
-                self.backend.client.table(table).select('*', count='exact').limit(1).execute()
-            except APIError as e:
-                if e.code == '42P01':
-                    missing_table = True
+        # get the slices
+        if len(args) == 1:
+            slices = [[1, self.dataset.shape[i] + 1] for i in range(2, self.dataset.ndim)]
+        else:  # 2 or more beyond index
+            slices = []
+            for i, arg in enumerate(args[1:]):
+                if isinstance(arg, int):
+                    slices.append([arg + 1, arg + 1])
+                elif isinstance(arg, slice):
+                    slices.append([arg.start + 1 if arg.start is not None else 1, arg.stop + 1 if arg.stop is not None else self.dataset.shape[i + 1] + 1])
                 else:
-                    raise e
-        
-        # check if any of the needed tables was not found
-        return not missing_table
-
-    @property
-    def user_id(self) -> str:
-        return self.backend._user.id
-
-    def insert_dataset(self, key: str, shape: Tuple[int], dim: int) -> Dataset:
-        # run the insert
-        self.__setup_auth()
-        response = self.backend.client.table('datasets').insert({'key': key, 'shape': shape, 'ndim': dim, 'user_id': self.user_id}).execute()
-        self.__restore_auth()
-
-        # return an instance of Dataset
-        data = response.data[0]
-        return Dataset(id=data['id'], key=data['key'], shape=data['shape'], ndim=data['ndim'])
+                    raise KeyError('Slice needs to be passed as int or slice.')
+            
+            # maybe the user does not want to slice all dimensions, append the others
+            if len(slices) + 1 != self.dataset.ndim:   # +1 for the index
+                for i in range(len(slices) + 1, self.dataset.ndim):
+                    slices.append([1, self.dataset.shape[i] + 1])
+
+        # finally return the full slice index for the database
+        return (
+            self.key,
+            index,
+            slices
+        )
     
-    def insert_tensor(self, data_id: int, data: List[np.ndarray], offset: int = 0) -> bool:
-        # setup auth token
-        self.__setup_auth()
-
-        # run the insert
-        try:
-            self.backend.client.table('tensors_float4').insert([{'data_id': data_id, 'index': int(i + 1 + offset), 'user_id': self.user_id, 'tensor': chunk.tolist()} for i, chunk in enumerate(data)]).execute()
-        except APIError as e:
-            # TODO check if we expired here and refresh the token
-            raise e
-        
-        # restore old token
-        self.__restore_auth()
-
-        # return 
-        return True
-
-    def get_dataset(self, key: str) -> Dataset:
-        # setup auth token
-        self.__setup_auth()
-
-        # get the dataset
-        response = self.backend.client.table('datasets').select('*').eq('key', key).execute()
-
-        # restore old token
-        self.__restore_auth()
-
-        # grab the data
-        data = response.data[0]
-
-        # return as Dataset
-        return Dataset(id=data['id'], key=data['key'], shape=data['shape'], ndim=data['ndim'])
-
-    def get_tensor(self, name: str, index_low: int, index_up: int, slice_low: List[int], slice_up: List[int]) -> np.ndarray:
-        # setup auth token
-        self.__setup_auth()
+    def __getitem__(self, args: Union[int, Tuple[int], slice]) -> np.ndarray:
+        # get the slices
+        _, index, slices = self.get_iloc_slices(*args)
 
-        # get the requested chunk
-        response = self.backend.client.rpc('tensor_float4_slice', {'name': name, 'index_low': index_low, 'index_up': index_up, 'slice_low': slice_low, 'slice_up': slice_up}).execute()
-
-        # restore old token
-        self.__restore_auth()
-
-        # grab the data
-        data = response.data[0]['tensor']
-
-        # return as np.ndarray
-        return np.asarray(data)
-
-    def remove_dataset(self, key: str) -> bool:
-        # setup auth token
-        self.__setup_auth()
-
-        # remove the dataset
-        self.backend.client.table('datasets').delete().eq('key', key).execute()
-
-        # restore old token
-        self.__restore_auth()
+        # load the tensor
+        with self._store.backend.database() as db:
+            # load the tensor
+            arr = db.get_tensor(self.key, index[0], index[1], [s[0] for s in slices], [s[1] for s in slices])
         
-        # return
-        return True
-
-    def list_tensor_keys(self) -> List[str]:
-        # setup auth token
-        self.__setup_auth()
-
-        # get the keys
-        response = self.backend.client.table('datasets').select('key').execute()
-
-        # restore old token
-        self.__restore_auth()
-
-        return [row['key'] for row in response.data]
+        # TODO now we can transform to other libaries
+        return arr
 
-    def __del__(self):
-        self.backend.logout()
+    def __call__(self, *args: Union[int, Tuple[int], slice]) -> Tuple[str, Tuple[int, int], List[Tuple[int, int]]]:
+        return self.get_iloc_slices(*args)
```

