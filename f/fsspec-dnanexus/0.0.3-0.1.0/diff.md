# Comparing `tmp/fsspec_dnanexus-0.0.3-py3-none-any.whl.zip` & `tmp/fsspec_dnanexus-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14326 bytes, number of entries: 10
--rw-r--r--  2.0 unx       70 b- defN 23-May-01 15:26 dxfsspec/__init__.py
--rw-r--r--  2.0 unx    16792 b- defN 23-May-15 08:23 dxfsspec/core.py
--rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 08:22 fsspec_dnanexus/__init__.py
--rw-r--r--  2.0 unx    20706 b- defN 23-Jun-05 08:22 fsspec_dnanexus/core.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5598 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      845 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/RECORD
-10 files, 45332 bytes uncompressed, 12870 bytes compressed:  71.6%
+Zip file size: 18056 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      292 b- defN 23-Aug-04 15:24 fsspec_dnanexus/__init__.py
+-rw-r--r--  2.0 unx    30564 b- defN 23-Aug-04 14:36 fsspec_dnanexus/core.py
+-rw-r--r--  2.0 unx    21901 b- defN 23-Aug-04 14:36 fsspec_dnanexus/dxfactory.py
+-rw-r--r--  2.0 unx     1872 b- defN 23-Aug-04 14:36 fsspec_dnanexus/utils.py
+-rw-r--r--  2.0 unx     1064 b- defN 23-Aug-04 15:37 fsspec_dnanexus-0.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     7118 b- defN 23-Aug-04 15:37 fsspec_dnanexus-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 15:37 fsspec_dnanexus-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Aug-04 15:37 fsspec_dnanexus-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-04 15:37 fsspec_dnanexus-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      864 b- defN 23-Aug-04 15:37 fsspec_dnanexus-0.1.0.dist-info/RECORD
+10 files, 63838 bytes uncompressed, 16568 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: dxfsspec/__init__.py
+Filename: fsspec_dnanexus/__init__.py
 Comment: 
 
-Filename: dxfsspec/core.py
+Filename: fsspec_dnanexus/core.py
 Comment: 
 
-Filename: fsspec_dnanexus/__init__.py
+Filename: fsspec_dnanexus/dxfactory.py
 Comment: 
 
-Filename: fsspec_dnanexus/core.py
+Filename: fsspec_dnanexus/utils.py
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.3.dist-info/LICENSE.txt
+Filename: fsspec_dnanexus-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.3.dist-info/METADATA
+Filename: fsspec_dnanexus-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.3.dist-info/WHEEL
+Filename: fsspec_dnanexus-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.3.dist-info/entry_points.txt
+Filename: fsspec_dnanexus-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.3.dist-info/top_level.txt
+Filename: fsspec_dnanexus-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.3.dist-info/RECORD
+Filename: fsspec_dnanexus-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fsspec_dnanexus/__init__.py

```diff
@@ -1,3 +1,9 @@
-from .core import DXFileSystem, DXFileSystemException, DXPathExtractor
+from .core import DXFileSystem, \
+                DXFileSystemException, \
+                DXPathExtractor, \
+                DXBufferedFileOnRay, \
+                DXBufferedFile
 
-__version__ = "0.0.3"
+from .utils import init_ray_with_fsspec_dnanexus, provision_dx_on_ray, get_n_partitions
+
+__version__ = "0.1.0"
```

## fsspec_dnanexus/core.py

```diff
@@ -1,20 +1,21 @@
 import os
 import stat
 import json
 import logging
 import dxpy
+from pathlib import Path
 from typing import Tuple, Union
 from threading import Thread
 
 from dxpy import api, DXFile, DXError, new_dxfile
 from dxpy.exceptions import ResourceNotFound, InvalidAuthentication, PermissionDenied
 
 from fsspec.spec import AbstractFileSystem, AbstractBufferedFile
-from fsspec.utils import setup_logging
+from fsspec.utils import setup_logging, stringify_path
 
 logger = logging.getLogger("dxfs")
 
 if "FSSPEC_DNANEXUS_LOGGING_LEVEL" in os.environ:
     setup_logging(logger=logger, level=os.environ["FSSPEC_DNANEXUS_LOGGING_LEVEL"])
 
 PROTOCOL = "dnanexus"
@@ -65,14 +66,32 @@
         self.token = storage_options.get("token", None) or os.environ.get("FSSPEC_DNANEXUS_TOKEN")
 
         if storage_options.get("staging", False):
             self.api_host = "stagingapi.dnanexus.com"
 
         self.dx_login(token=self.token, api_host=self.api_host)
 
+    @classmethod
+    def _strip_protocol(cls, path):
+        """Turn path from fully-qualified to file-system-specific
+
+        May require FS-specific handling, e.g., for relative paths or links.
+        """
+        if isinstance(path, list):
+            return [cls._strip_protocol(p) for p in path]
+        path = stringify_path(path)
+        protos = (cls.protocol,) if isinstance(cls.protocol, str) else cls.protocol
+        for protocol in protos:
+            if path.startswith(protocol + "://"):
+                path = path[len(protocol) + 3 :]
+            elif path.startswith(protocol + "::"):
+                path = path[len(protocol) + 2 :]
+        # use of root_marker to make minimum required path, e.g., "/"
+        return path or cls.root_marker
+
     def dx_login(self, token=None, api_host="api.dnanexus.com"):
         # if token is not provided, dxfsspec uses thes token of dxpy by default
         if not token:
             return
         
         try:
             dxpy.set_api_server_info(host=api_host, protocol='https')
@@ -89,27 +108,42 @@
         cache_options=None,
         **kwargs):
         if block_size is None:
             block_size = self.block_size
         if cache_type is None:
             cache_type = self.cache_type
 
-        return DXBufferedFile(
+        from .utils import FILECLASS_DICT
+
+        dx_buffered_cls = self.storage_options.get("dx_buffered_cls", None)
+        dx_buffered_cls = FILECLASS_DICT[dx_buffered_cls] if dx_buffered_cls in FILECLASS_DICT else DXBufferedFile
+
+        return dx_buffered_cls(
             fs=self,
             path=path,
             mode=mode,
             block_size=block_size,
             cache_type=cache_type,
             autocommit=autocommit,
             cache_options=cache_options
         )
 
     def info(self, path, **kwargs):
         path = self._strip_protocol(path)
-        project_id, file_id, _ = self.dx_path_extractor.extract_path(path)
+
+        is_file = self.isfile(path)
+        is_dir = self.isdir(path)
+
+        if is_dir and is_file:
+            raise DXFileSystemException("The path is ambiguous. It matches file and folder.")
+
+        if is_dir:
+            return {"type": "directory", "name": path, "size": 0}
+
+        project_id, file_id, _ = self.dx_path_extractor.extract(path)
 
         if not project_id or not file_id:
             raise DXFileSystemException(f"ValueError: Unsupported format of this path {path}")
 
         logger.debug(f"Get info of '{file_id}' in '{project_id}'")
         try:
             desc = DXFile(file_id, project=project_id).describe()
@@ -119,25 +153,40 @@
             raise DXFileSystemException(f"FileNotFound: {e}")
 
     def exists(self, path, **kwargs):
         logger.debug(f"Check if {path} exists")
         describe = self._file_describe(path, **kwargs)
         return describe is not None
 
+    def isdir(self, path, **kwargs):
+        logger.debug(f"Check if {path} is directory")
+
+        path = self._strip_protocol(path)
+        project_id, _, fullpath = self.dx_path_extractor.extract(path)
+
+        if fullpath is None:
+            return False
+
+        try:
+            api.project_list_folder(project_id, input_params={"folder": fullpath, "only": "folders"})
+            return True
+        except ResourceNotFound:
+            return False
+
     def isfile(self, path, **kwargs):
         logger.debug(f"Check if {path} is file")
         describe = self._file_describe(path, **kwargs)
         if not describe:
             return False
         return describe['class'] == 'file'
 
     def _file_describe(self, path, **kwargs):
         path = self._strip_protocol(path)
         try:
-            project_id, file_id, _ = self.dx_path_extractor.extract_path(path)
+            project_id, file_id, _ = self.dx_path_extractor.extract(path)
             logger.debug(f"Describe {file_id} in {project_id}")
             if project_id and file_id:
                 return api.file_describe(file_id, input_params={"project": project_id})
         except (ResourceNotFound, DXFileSystemException):
             return None
         return None
 
@@ -154,19 +203,21 @@
                     # check the latest created time
                     if file["created"] > res[name]["created"]:
                         res[name] = file
             return list(res.values())
 
         path = self._strip_protocol(path)
 
-        project_id, _, folder_path = self.dx_path_extractor.extract_path(path, mode=None)
+        project_id, _, folder_path = self.dx_path_extractor.extract(path)
+
+        if folder_path is None:
+            raise DXFileSystemException(f"ResourceNotFound: The specified folder could not be found in {project_id}")
+
         logger.debug(f"List information about files and directories in folder '{folder_path}' of {project_id}")
-        if not project_id:
-            raise DXFileSystemException(f"ProjectNotFound: There is no project with path {path}")
-        
+
         try:
             results = api.project_list_folder(object_id=project_id, 
                                     input_params={"folder": folder_path,
                                                   "includeHidden": True,
                                                   "describe": dict(fields={"id": True,
                                                                            "project": True,
                                                                            "name": True,
@@ -213,57 +264,129 @@
             return folders + objects
 
         except ResourceNotFound as e:
             raise DXFileSystemException(f"ResourceNotFound: {e}")
         except DXError as e:
             raise DXFileSystemException(f"Unknown Error: {e}")
 
-
     def mkdir(self, path, create_parents=True, **kwargs):
         path = self._strip_protocol(path)
 
-        project_id, _, folder_path = self.dx_path_extractor.extract_path(path, mode=None)
+        project_id, _, folder_path = self.dx_path_extractor.extract(path)
         logger.debug(f"Create new folder '{folder_path}' in {project_id}.")
 
-        if not project_id:
-            raise DXFileSystemException(f"ProjectNotFound: There is no project with path {path}")
-
         try:
             return api.project_new_folder(object_id=project_id, input_params={
                                                             "folder": folder_path, 
                                                             "parents": create_parents})
         except ResourceNotFound as e:
             raise DXFileSystemException(f"ProjectNotFound: {e}")
         except DXError as e:
             raise DXFileSystemException(f"Unknown Error: {e}")
+        
+    def mkdirs(self, path, exist_ok=True, **kwargs):
+        if not exist_ok and self.isdir(path=path):
+            raise DXFileSystemException("ResourceExists: The folder in url {url} alread exists")
+        
+        path = self._strip_protocol(path)
+
+        project_id, _, folder_path = self.dx_path_extractor.extract(path)
+        logger.debug(f"Create new folder '{folder_path}' in {project_id}.")
+
+        try:
+            return api.project_new_folder(object_id=project_id, input_params={
+                                                            "folder": folder_path, 
+                                                            "parents": True})
+        except ResourceNotFound as e:
+            raise DXFileSystemException(f"ProjectNotFound: {e}")
+        except DXError as e:
+            raise DXFileSystemException(f"Unknown Error: {e}")
+        
+    def find(self, path, maxdepth=None, withdirs=False, detail=False, **kwargs):
+        """
+        When reading parquet file using pyarrow engine, pyarrow will call fs.find function
+        Modify the key of result to adapt our format project_id:file_id
+        Reference: https://github.com/apache/arrow/blob/3bdbd0d34cdfe6f34e1c2bf80df472faccdff3c0/python/pyarrow/fs.py#L355
+
+        List all files below path.
+
+        Like posix ``find`` command without conditions
+
+        Parameters
+        ----------
+        path : str
+        maxdepth: int or None
+            If not None, the maximum number of levels to descend
+        withdirs: bool
+            Whether to include directory paths in the output. This is True
+            when used by glob, but users usually only want files.
+        kwargs are passed to ``ls``.
+        """
+        # TODO: allow equivalent of -name parameter
+        path = self._strip_protocol(path)
+        out = dict()
+        for _, dirs, files in self.walk(path, maxdepth, detail=True, **kwargs):
+            if withdirs:
+                files.update(dirs)
+            out.update({info["name"]: info for name, info in files.items()})
+        if not out and self.isfile(path):
+            # walk works on directories, but find should also return [path]
+            # when path happens to be a file
+            out[path] = {}
+        names = sorted(out)
+        if not detail:
+            return names
+        else:
+            project, _ = path.split(":")
+            return {f"{project}:{name}": out[name] for name in names}
+    
+    def rename_folder(self, path: str, new_name: str):
+        path = self._strip_protocol(path)
+        project_id, _, folder_path = self.dx_path_extractor.extract(path=path)
+        api.project_rename_folder(project_id, input_params={
+            "folder": folder_path,
+            "name": new_name
+        })
+
+    def remove_files_in_folder(self, path: str):
+        objects = self.ls(path=path, detail=True)
+        if len(objects) == 0:
+            return
+        # only remove file
+        object_ids = [obj["id"] for obj in objects if obj["type"] == "file"]
+        proj_id = objects[0]['project']
+        api.project_remove_objects(proj_id, input_params={"objects": object_ids})
+
 
 class DXBufferedFile(AbstractBufferedFile):
 
     part_min = 5 * 2**20
     part_max = 5 * 2**30
 
     def __init__(self, 
                  fs,
                  path: str,
                  mode: str = "rb",
                  block_size: int = 5 * 2**20,
                  cache_type: str ="readahead",
                  autocommit: bool = True,
                  cache_options: dict = None):
-        
-        self.project_id, file_id, self.file_path = DXPathExtractor().extract_path(path, mode=mode)
-
-        # if self.project_id:
-        #     self.check_permissions(project_id=self.project_id, mode=mode)
-
-        self.dxfile: Union[DXFile, None] = DXFile(file_id, project=self.project_id) if file_id else None
+        self.dx_path_extractor = DXPathExtractor()
+        self.project_id, file_id, self.fullpath = self.dx_path_extractor.extract(path, mode=mode)
 
         if "r" in mode:
+            if not self.dx_path_extractor.is_dx_file_id(file_id):
+                raise DXFileSystemException("FileNotFound: Cannot find any file matching { name: '%s', folder: '%s', project: '%s' }" \
+                                    % (path, self.project_id, file_id ))
+            
+            self.dxfile: Union[DXFile, None] = DXFile(file_id, project=self.project_id) if file_id else None
+            
             if self.dxfile and self.dxfile._get_state() != "closed":
                 raise DXFileSystemException("NotSupportedError: Reading an open file is not supported.")
+            
             self.details = fs.info(path)
             self.size = self.details["size"]
 
         super().__init__(
             fs,
             path,
             mode,
@@ -330,18 +453,18 @@
             self.dx_handler.wait_on_close()
             self.dx_handler = None
 
         return not final
 
     def _initiate_upload(self):
         """Create remote file/upload"""
-        logger.debug("Initiate upload for %s" % self.file_path)
+        logger.debug("Initiate upload for %s" % self.fullpath)
 
-        folder = os.path.dirname(self.file_path)
-        filename = os.path.basename(self.file_path)
+        folder = os.path.dirname(self.fullpath)
+        filename = os.path.basename(self.fullpath)
 
         try:
             self.dx_handler = new_dxfile(name=filename,
                                      folder=folder,
                                      project=self.project_id,
                                      parents=True,
                                      mode="a")
@@ -379,14 +502,108 @@
         file_ids = [obj["id"] for obj in objects if obj["id"] != exclude_dxid]
         if len(file_ids) > 0:
             try:
                 api.project_remove_objects(project_id, input_params={"objects": file_ids, "force": True})
                 logger.debug(f"Removed: {file_ids}")
             except Exception as e:
                 logger.debug(f"DXFileSystemException: {e}")
+    
+class DXBufferedFileOnRay(DXBufferedFile):
+    def _upload_chunk(self, final=False):    
+        logger.debug(
+            f"Upload for {self}, final={final}, loc={self.loc}, buffer loc={self.buffer.tell()}"
+        )
+        self.buffer.seek(0)
+        data = self.buffer.read()
+
+        storage_options = self.fs.storage_options
+
+        is_last_partition = storage_options.get("n_partitions") - 1 == storage_options.get("partition_idx")
+
+        # to make sure DXFile writes only one part
+        # In DXFile, if _write_buffer_size_hint is less than length of data, it will write to multiple parts
+        self.dx_handler._write_buffer_size_hint = len(data)
+
+        desc = self.dx_handler.describe(fields={"parts": True})
+        parts = desc.get("parts", {})
+        
+        # write to the next part
+        self.dx_handler._cur_part = len(parts) + 1
+        self.dx_handler._num_uploaded_parts = self.dx_handler._cur_part
+        
+        if len(data) > 0:
+            # because DXFile is required to have at least 5MB for each part (except last part)
+            # we remove the file when writing any parts (except last) that is less than 5Mb
+            if not is_last_partition and len(data) < 5 * 2**20:
+                self.dx_handler._num_uploaded_parts = 0 # to upload empty byte before closing
+                self.dx_handler.close()
+                self.dx_handler.wait_on_close()
+                self.dx_handler.remove()
+                raise DXFileSystemException("InvalidState: Each part (except last) must be at least 5 MB")
+
+            self.dx_handler.write(data=data)
+            self.dx_handler.flush()
+        
+        if final:
+            try:
+                self.dx_handler.wait_until_parts_uploaded()
+            except DXError:
+                raise DXFileSystemException("File {} was not uploaded correctly!".format(self.dx_handler.name))
+            # close file if it's last partition
+            
+            if is_last_partition:
+                self.dx_handler.close()
+                self.dx_handler.wait_on_close()
+                self.dx_handler = None
+
+        return not final
+
+    def _initiate_upload(self):
+        """Create remote file/upload"""
+        logger.debug("Initiate upload for %s" % self)
+        
+        storage_options = self.fs.storage_options
+        # marker_id is passed from DXPandasOnRayIO 
+        marker_id = storage_options.get("marker_id")
+
+        folder = os.path.dirname(self.fullpath)
+        filename = os.path.basename(self.fullpath)
+
+        # get DXFile using marker_id
+        existing_file = dxpy.find_one_data_object(name=filename, 
+                                                 folder=folder, 
+                                                 project=self.project_id, 
+                                                 properties={"marker_id": marker_id},
+                                                 recurse=False,
+                                                 zero_ok=True)
+        if existing_file:
+            self.dx_handler = DXFile(existing_file["id"], 
+                                     project=existing_file["project"], 
+                                     mode="a")
+            return
+
+        try:
+            # create new file for writing
+            self.dx_handler = new_dxfile(name=filename,
+                                        folder=folder,
+                                        project=self.project_id,
+                                        parents=True,
+                                        mode="w")
+            
+            self.dx_handler.set_properties({"marker_id": marker_id})
+
+            # check file exists for first partition
+            if storage_options.get("partition_idx") == 0 and not storage_options.get("allow_duplicate_filenames"):
+                t = Thread(target=self.remove_duplicate_filenames, args=(filename,
+                                                                         folder,
+                                                                         self.project_id,
+                                                                         self.dx_handler.get_id()))
+                t.start()
+        except PermissionDenied as e:
+            raise DXFileSystemException(f"PermissionDenied: {e}")
 
 class DXPathExtractor():
     root_marker = "/"
 
     def __init__(self) -> None:
         pass
 
@@ -432,61 +649,81 @@
                 api.file_describe(id_or_path, input_params={"project": project_id, "fields": {"id": True}})
                 return id_or_path
             except ResourceNotFound as e:
                 raise DXFileSystemException(f"FileNotFound: {e}")
             except DXError as e:
                 raise DXFileSystemException(f"Unknown Error: {e}")
 
-        logger.debug(f"{id_or_path} is not DXProject ID. Try to find DXFile with name '{id_or_path}' in {project_id}")
+        logger.debug(f"{id_or_path} is not DXFile ID. Try to find DXFile with name '{id_or_path}' in {project_id}")
+        
+        id_or_path = id_or_path or self.root_marker
+        
         folder = os.path.dirname(id_or_path)
-        if not folder:
+        if not folder.startswith("/"):
             raise DXFileSystemException("ValueError: The folder path should start with '/'")
+        
         filename = os.path.basename(id_or_path)
+        if not filename:
+            return None
+        
         # check if dxfile exists by name and project
         dxfile_desc = None
         dxfiles = dxpy.find_data_objects(classname="file", 
                                             name=filename, 
                                             folder=folder, 
                                             project=project_id, 
                                             describe=True,
                                             recurse=False)
         for file in dxfiles:
             file_desc = file["describe"]
             if dxfile_desc is None or file_desc["created"] > dxfile_desc["created"]:
                 dxfile_desc = file_desc
         
         if dxfile_desc is None:
-            raise DXFileSystemException("FileNotFound: Cannot find any file matching { name: '%s', folder: '%s', project: '%s' }" \
-                                    % (filename, folder, project_id ))
+            return None
         
         return dxfile_desc["id"]
 
-    def extract_path(self, path: str, mode: Union[str, None] = "rb") -> Tuple[str, str, str]:
+    def extract(self, path: str, mode: Union[str, None] = None) -> Tuple[str, str, str]:
         logger.debug(f"Extract info from {path}")
+        
         project_id = None
         file_id = None
-        file_path = None # used for write case
+        fullpath = None
 
         file_info = path.split(":")
         # DX id format
         # project-xxx:file-yyyy
-        file_id_or_path = None
         if len(file_info) == 2:
-            project_id_or_name, file_id_or_path = file_info
-            
+            project_id_or_name, file_or_folder_path = file_info
+
             project_id = self.get_project_id(id_or_path=project_id_or_name)
             
-            if mode != None and "r" in mode:
-                file_id = self.get_file_id(id_or_path=file_id_or_path, project_id=project_id)
+            if mode != None and ("w" in mode or "a" in mode):
+                pass
             else:
-                file_path = file_id_or_path
+                file_id = self.get_file_id(id_or_path=file_or_folder_path, project_id=project_id)
+            
+            # if not file id, assign fullpath to origin path
+            if not self.is_dx_file_id(file_or_folder_path):
+                fullpath = file_or_folder_path
         else:
-            file_id_or_path = file_info[0]
-            if self.is_dx_file_id(file_id=file_id_or_path):
-                file_id = file_id_or_path
-                
+            file_or_folder_path = file_info[0]
+            if self.is_dx_file_id(file_id=file_or_folder_path):
+                file_id = file_or_folder_path
                 # find dx project based on dx file id
-                dxfile = DXFile(file_id)
+                dxfile = DXFile(file_or_folder_path)
                 dxfile_desc = dxfile.describe()
                 project_id = dxfile_desc["project"]
+            else:
+                fullpath = file_or_folder_path
+
+        if not project_id:
+            raise DXFileSystemException(f"ProjectNotFound: There is no project with path {path}")
+
+        # should remove "/"" at the end if fullpath is not root
+        # for case ls on root e.g dxfs.ls("dnanexus://project-xxx:/")
+        # for case read file e.g dxfs.ls("dnanexus://project-xxx:/path/to/file.csv/")
+        if fullpath and fullpath != self.root_marker:
+            fullpath = fullpath.rstrip("/")
 
-        return project_id, file_id, file_path or self.root_marker
+        return project_id, file_id, fullpath
```

## Comparing `fsspec_dnanexus-0.0.3.dist-info/LICENSE.txt` & `fsspec_dnanexus-0.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fsspec_dnanexus-0.0.3.dist-info/METADATA` & `fsspec_dnanexus-0.1.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec-dnanexus
-Version: 0.0.3
+Version: 0.1.0
 Summary: fsspec backend for the DNAnexus platform
 Maintainer: DNAnexus-xVantage
 Maintainer-email: tphan@dnanexus.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -90,37 +90,63 @@
 
 * allow_duplicate_filenames: False - [default] removes existing file(s) with the same path and writes the new file (just like file:// s3:// and other backends would)
 * allow_duplicate_filenames: True - writes the file at specified path disregarding existing files
 
 If the user's token allows for file writing but does not allow for the removal of the file (e.g. protected projects), the behaviour falls
 back to allow_duplicate_filenames: True to ensure no data loss.
 
+## Modin and ray
+### Required Initialization
+When using fsspec_dnanexus under modin and ray, you'll need to invoke an initialization function.
+
+For most users, the following function would perform the necessary initialization for fsspec_dnanexus to work under modin and ray
+
+    from fsspec_dnanexus import init_ray_with_fsspec_dnanexus
+    init_ray_with_fsspec_dnanexus()
+
+For advanced users there are two ways to customize this behaviour
+
+1. Manually set the number of partitions. This impacts the number of chunks modin uses to process the dataframe in parallel and affects the number of files
+
+        from fsspec_dnanexus import init_ray_with_fsspec_dnanexus
+        init_ray_with_fsspec_dnanexus(n_partitions=20)
+
+2. Or if you already have ray.init happening elsewhere, you can simply invoke the following
+
+        from fsspec_dnanexus import provision_dx_on_ray
+        provision_dx_on_ray()
+
+### Parquet folder
+
+Note that when using df.to_parquet, each partition will simultaneously write a part of the dataframe and the resultant output is
+a folder containing many parts rather than a single file.
+
 
 ## Credentials
-The credentials used by fsspec_dnanexus to access DNAnexus is resolved in the following order:
+The credentials used by fsspec_dnanexus to access DNAnexus is determined by the following methods:
+
+1. By default fsspec_dnanexus inherits the credentials currently used by dxpy. If you're using a DNAnexus workstation, this is a good place to start as you don't have to do anything.
+
+        df = pd.read_csv("dnanexus://my-dx-project:/folder/filename1.csv")
 
-1. The token parameter passed in using storage_options
+2. If the FSSPEC_DNANEXUS_TOKEN environment variable is set, it will be used over dx-toolkit's credentials
+
+        os.environ['FSSPEC_DNANEXUS_TOKEN'] = "YOUR_DNANEXUS_TOKEN"
+        df = pd.read_csv("dnanexus://my-dx-project:/folder/filename1.csv")
+
+3. If a DNAnexus token parameter passed in using storage_options, this takes priority over the two methods above
 
         # Option 1a
         dxfs = fsspec.filesystem("dnanexus", storage_options = {"token": "YOUR_DNANEXUS_TOKEN"})
 
         # Option 1b
         df = pd.read_csv("dnanexus://my-dx-project:/folder/filename1.csv", storage_options={
             "token": "YOUR_DNANEXUS_TOKEN",
         })
 
-2. The FSSPEC_DNANEXUS_TOKEN environment variable
-
-        os.environ['FSSPEC_DNANEXUS_TOKEN'] = "YOUR_DNANEXUS_TOKEN"
-        df = pd.read_csv("dnanexus://my-dx-project:/folder/filename1.csv")
-
-3. Inherits the credentials currently used by dxpy. If you're using a DNAnexus workstation, this is a good place to start.
-
-        df = pd.read_csv("dnanexus://my-dx-project:/folder/filename1.csv")
-
 
 ## Limitations
 
 1. The following commands are currently unsupported:
     * dxfs.touch
     * dxfs.cat
     * dxfs.copy
@@ -137,14 +163,19 @@
     os.environ["FSSPEC_DNANEXUS_LOGGING_LEVEL"] = "DEBUG"
 
 Valid logging levels are listed here: https://docs.python.org/3/library/logging.html#levels
 
 
 ## Changelog
 
+#### 0.1.0 (2023-08-04)
+* Feature: Support for modin + ray
+* Known issues:
+    * Under modin and ray, when writing a small csv file would result in an exception. The workaround is to set n_partition mentioned above to a low number 
+
 #### 0.0.3 (2023-06-05)
 * Fixed: When using PyArrow to read parquet, `pd.read_parquet` can be invoked directly, no longer requiring
   passing in file handler from `fsspec.open()`.
 
 #### 0.0.2 (2023-05-29)
 * Fixed: Project description in PyPi, corrected import statement in README
```

## Comparing `fsspec_dnanexus-0.0.3.dist-info/RECORD` & `fsspec_dnanexus-0.1.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-dxfsspec/__init__.py,sha256=TCNrpMLRzKRTpk403TFZZzyTCysYJ-tQrIjfVjRFkzM,70
-dxfsspec/core.py,sha256=jjRUhHmNi3JeJHVsLB69eWEapNuTlwJGXH_897gBwLE,16792
-fsspec_dnanexus/__init__.py,sha256=Qp9IeL8XHC2QMgudO2nDfrhKybOUpXC9ikoOeRJcN0Q,94
-fsspec_dnanexus/core.py,sha256=xgfiC1nxZ-gBXMXlO5tlAXyuwkCL7oX4ebCpw3CoTiI,20706
-fsspec_dnanexus-0.0.3.dist-info/LICENSE.txt,sha256=xw5rRrmGcck7yjci2gFi_mdLQMqoJ4z_wj9V-v1f8kc,1064
-fsspec_dnanexus-0.0.3.dist-info/METADATA,sha256=wpyEn7LBrcc8jdex4y9-TpR90SkiuiRBrOwEAL93ocw,5598
-fsspec_dnanexus-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fsspec_dnanexus-0.0.3.dist-info/entry_points.txt,sha256=zedbecJMg3jDda3NJosZuAeXyQcyvjjtxoPOUzaxvpA,55
-fsspec_dnanexus-0.0.3.dist-info/top_level.txt,sha256=fhiQuqx3PFbiSpzgyHwTk5k8oC2um96uzf3YTKNwpIE,16
-fsspec_dnanexus-0.0.3.dist-info/RECORD,,
+fsspec_dnanexus/__init__.py,sha256=3RhM-MUgaANMllev0ujJh3oLU_vYnzylJn7SlY8EyGw,292
+fsspec_dnanexus/core.py,sha256=QIPebenm3EDOlFLq40J143hmqDq_gmGYYd_T2-26FOM,30564
+fsspec_dnanexus/dxfactory.py,sha256=8yBF1uHhG9AmmxxVrwba10P-8LcfjhFiIAreXvxqVt8,21901
+fsspec_dnanexus/utils.py,sha256=KHRMoHT4MwD8MSzHOsU8vosZdPSy3Ry0XaCLtFNEebY,1872
+fsspec_dnanexus-0.1.0.dist-info/LICENSE.txt,sha256=xw5rRrmGcck7yjci2gFi_mdLQMqoJ4z_wj9V-v1f8kc,1064
+fsspec_dnanexus-0.1.0.dist-info/METADATA,sha256=n8gQZnYspwe4ojWVmZSAK2qRHyX0-sfRDoqpjARvATs,7118
+fsspec_dnanexus-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fsspec_dnanexus-0.1.0.dist-info/entry_points.txt,sha256=zedbecJMg3jDda3NJosZuAeXyQcyvjjtxoPOUzaxvpA,55
+fsspec_dnanexus-0.1.0.dist-info/top_level.txt,sha256=fhiQuqx3PFbiSpzgyHwTk5k8oC2um96uzf3YTKNwpIE,16
+fsspec_dnanexus-0.1.0.dist-info/RECORD,,
```

