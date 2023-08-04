# Comparing `tmp/waffle_box-0.1.0.tar.gz` & `tmp/waffle_box-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_box-0.1.0.tar", max compression
+gzip compressed data, was "waffle_box-0.2.0.tar", max compression
```

## Comparing `waffle_box-0.1.0.tar` & `waffle_box-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      781 2023-07-27 05:40:09.951813 waffle_box-0.1.0/README.md
--rw-r--r--   0        0        0      141 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/__init__.py
--rw-r--r--   0        0        0     9411 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/app_manager.py
--rw-r--r--   0        0        0     2786 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/app_structure.py
--rw-r--r--   0        0        0     2304 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/nvinfer_config_parser.py
--rw-r--r--   0        0        0       83 2023-07-27 05:40:09.951813 waffle_box-0.1.0/maker_manager/__init__.py
--rw-r--r--   0        0        0     2476 2023-07-27 05:40:09.955814 waffle_box-0.1.0/maker_manager/convert_option.py
--rw-r--r--   0        0        0     9703 2023-07-27 05:40:09.955814 waffle_box-0.1.0/maker_manager/maker_manager.py
--rw-r--r--   0        0        0      645 2023-07-27 05:40:09.955814 waffle_box-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      119 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/__init__.py
--rw-r--r--   0        0        0     3231 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/bake_service.py
--rw-r--r--   0        0        0     6280 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/cli.py
--rw-r--r--   0        0        0     4486 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/convert_service.py
--rw-r--r--   0        0        0     2262 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/pull_service.py
--rw-r--r--   0        0        0       67 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box_exception/__init__.py
--rw-r--r--   0        0        0     1573 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box_exception/waffle_box_exception.py
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 waffle_box-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2095 2023-08-04 08:00:53.040078 waffle_box-0.2.0/README.md
+-rw-r--r--   0        0        0      141 2023-08-04 08:00:53.040078 waffle_box-0.2.0/app_manager/__init__.py
+-rw-r--r--   0        0        0     9582 2023-08-04 08:00:53.040078 waffle_box-0.2.0/app_manager/app_manager.py
+-rw-r--r--   0        0        0     2754 2023-08-04 08:00:53.040078 waffle_box-0.2.0/app_manager/app_structure.py
+-rw-r--r--   0        0        0     2294 2023-08-04 08:00:53.040078 waffle_box-0.2.0/app_manager/nvinfer_config_parser.py
+-rw-r--r--   0        0        0      147 2023-08-04 08:00:53.040078 waffle_box-0.2.0/maker_manager/__init__.py
+-rw-r--r--   0        0        0     2447 2023-08-04 08:00:53.040078 waffle_box-0.2.0/maker_manager/convert_option.py
+-rw-r--r--   0        0        0    11229 2023-08-04 08:00:53.040078 waffle_box-0.2.0/maker_manager/maker_manager.py
+-rw-r--r--   0        0        0     3284 2023-08-04 08:00:53.040078 waffle_box-0.2.0/maker_manager/thread_handler.py
+-rw-r--r--   0        0        0      668 2023-08-04 08:00:53.044078 waffle_box-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-08-04 08:00:53.044078 waffle_box-0.2.0/waffle_box/__init__.py
+-rw-r--r--   0        0        0     3760 2023-08-04 08:00:53.044078 waffle_box-0.2.0/waffle_box/bake_service.py
+-rw-r--r--   0        0        0     6644 2023-08-04 08:00:53.044078 waffle_box-0.2.0/waffle_box/cli.py
+-rw-r--r--   0        0        0     4867 2023-08-04 08:00:53.044078 waffle_box-0.2.0/waffle_box/convert_service.py
+-rw-r--r--   0        0        0     2259 2023-08-04 08:00:53.044078 waffle_box-0.2.0/waffle_box/pull_service.py
+-rw-r--r--   0        0        0       68 2023-08-04 08:00:53.044078 waffle_box-0.2.0/waffle_box_exception/__init__.py
+-rw-r--r--   0        0        0     1570 2023-08-04 08:00:53.044078 waffle_box-0.2.0/waffle_box_exception/waffle_box_exception.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 waffle_box-0.2.0/PKG-INFO
```

### Comparing `waffle_box-0.1.0/app_manager/app_manager.py` & `waffle_box-0.2.0/app_manager/app_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,117 +1,125 @@
-from app_manager import ModelInfo, AppStructure
-from app_manager import NvinferConfigParser
-from waffle_box_exception import WaffleBoxException, ExceptionCode
-
+import json
 import os
 import shutil
 from pathlib import Path
-from uuid import UUID
+from uuid import UUID, uuid4
 from zipfile import ZipFile
-import json
+
+from app_manager import AppStructure, ModelInfo, NvinferConfigParser
+from waffle_box_exception import ExceptionCode, WaffleBoxException
 
 
 class AppManager:
-    """ Base App을 파싱하고 새로운 App을 생성
+    """Base App을 파싱하고 새로운 App을 생성
 
     Base App을 파싱 후 모델을 교체해 새로운 App을 생성한다.
 
     Attributes:
         workspace (Path): 작업할 경로로 일반적으로 ~/.waffle_box 사용
         app_structure (AppStructure): 작업할 App의 구조
 
     """
 
     def __init__(self, workspace: Path, app_path: Path) -> None:
         """
-        Args: 
+        Args:
             workspace (Path): 작업할 경로
             app_path (Path): Base 앱 경로
 
         Raises:
             APP_STRUCTURE_EXCEPTION
             APP_CONFIG_ERROR
 
         """
-        self.workspace: Path = workspace
+        self.workspace: Path = workspace.joinpath(f"{uuid4()}/")
 
         self._app_structure: AppStructure = self._extract_app(app_path)
+    
+    def __del__(self):
+        if os.path.exists(self.workspace):
+            shutil.rmtree(self.workspace)
 
     def _extract_app(self, app_path: Path) -> AppStructure:
-        """ App 파일을 압축 해제하고 구조를 분석한다.
+        """App 파일을 압축 해제하고 구조를 분석한다.
 
         입력받은 App 파일을 workspace의 temp 폴더에 압축 해제한다.
         만약 temp 파일이 이미 존재한다면 폴더를 삭제하고 압축을 새로 해제한다.
 
-        App 파일 내부 모델도 모두 압축 해제 후 
+        App 파일 내부 모델도 모두 압축 해제 후
         model info를 담은 AppStructure를 반환한다.
 
         Args:
             app_path (Path): App 경로
 
         Raises:
             APP_STRUCTURE_EXCEPTION
             APP_CONFIG_ERROR
 
         """
         if not app_path.exists():
-            raise WaffleBoxException('Wrong input file.', ExceptionCode.APP_NO_SUCH_FILE)
-        
+            raise WaffleBoxException("Wrong input file.", ExceptionCode.APP_NO_SUCH_FILE)
+
         # app 압축을 풀 임시 폴더
-        temp_dir = self.workspace.joinpath('temp')
+        temp_dir = self.workspace.joinpath("temp")
 
         if temp_dir.exists():
             shutil.rmtree(temp_dir)
 
         zip_file = ZipFile(app_path)
         zip_file.extractall(temp_dir)
 
         # read app.json
-        app_json_f = open(temp_dir.joinpath('app.json'))
+        app_json_f = open(temp_dir.joinpath("app.json"))
         app_json = json.load(app_json_f)
 
-        app_id: UUID = UUID(app_json['id'])
+        app_id: UUID = UUID(app_json["id"])
 
         model_info_list: list[ModelInfo] = []
 
-        if not app_json.get('models') or len(app_json['models']) == 0:
+        if not app_json.get("models") or len(app_json["models"]) == 0:
             raise WaffleBoxException(
-                'There is no model in app.', ExceptionCode.APP_STRUCTURE_EXCEPTION)
+                "There is no model in app.", ExceptionCode.APP_STRUCTURE_EXCEPTION
+            )
 
         # walk models
-        for model in app_json['models']:
+        for model in app_json["models"]:
             try:
-                model_id = model['id']
-                model_name = model['name']
-                model_precision = model['precision']
-                model_zip_path = temp_dir.joinpath(model['path'])
+                model_id = model["id"]
+                model_name = model["name"]
+                model_precision = model["precision"]
+                model_zip_path = temp_dir.joinpath(model["path"])
             except KeyError as e:
                 raise WaffleBoxException(
-                    f'In app.json, no such key: {e}', ExceptionCode.APP_CONFIG_ERROR)
+                    f"In app.json, no such key: {e}", ExceptionCode.APP_CONFIG_ERROR
+                )
             except Exception as e:
-                raise WaffleBoxException(
-                    str(e), ExceptionCode.APP_STRUCTURE_EXCEPTION)
+                raise WaffleBoxException(str(e), ExceptionCode.APP_STRUCTURE_EXCEPTION)
 
             model_path = self._extract_model(model_zip_path)
 
             model_info = self._make_model_info(
-                model_path=model_path, model_id=model_id,
-                model_name=model_name, model_precision=model_precision
+                model_path=model_path,
+                model_id=model_id,
+                model_name=model_name,
+                model_precision=model_precision,
             )
 
             model_info_list.append(model_info)
 
         app_structure = AppStructure(
-            id=app_id, models=model_info_list, path=temp_dir,
+            id=app_id,
+            models=model_info_list,
+            path=temp_dir,
         )
 
         return app_structure
 
     def _extract_model(self, model_path: Path) -> Path:
-        """ 모델 압축 풀기
+        """모델 압축 풀기
 
         모델 파일은 zip 파일 이름과 동일한 이름의 폴더에 압축을 푼다.
         예) PeopleNet.zip -> PeopleNet 폴더에 압축 풀기
 
         압축을 풀면 zip 파일을 삭제한다.
 
         Args:
@@ -128,67 +136,75 @@
         zip_file.extractall(model_dir)
         zip_file.close()
 
         os.remove(model_path)
 
         return model_dir
 
-    def _make_model_info(self, model_path: Path, model_id: UUID,
-                         model_name: str, model_precision: str) -> ModelInfo:
-        """ 압축 푼 모델 폴더에서 정보를 추출한다.
+    def _make_model_info(
+        self, model_path: Path, model_id: UUID, model_name: str, model_precision: str
+    ) -> ModelInfo:
+        """압축 푼 모델 폴더에서 정보를 추출한다.
 
         압축 푼 모델 폴더의 infer_nvinfer_config.txt 파일을 읽고
         필요한 정보들을 추출한다.
 
         Args:
             model_path (Path): 모델 경로
             model_id (UUID): 모델 id
             model_name (str): 모델 이름
             model_precision (str): 모델 precision
 
         Raises:
             APP_CONFIG_ERROR
 
         """
-        nvinfer_parser = NvinferConfigParser(
-            model_path.joinpath('infer_nvinfer_config.txt'))
+        nvinfer_parser = NvinferConfigParser(model_path.joinpath("infer_nvinfer_config.txt"))
 
-        engine_file_name = nvinfer_parser.get('model-engine-file')
+        engine_file_name = nvinfer_parser.get("model-engine-file")
         if not engine_file_name:
-            raise WaffleBoxException('In infer_nvinfer_config.txt, no such key model-engine-file',
-                                     ExceptionCode.APP_CONFIG_ERROR)
+            raise WaffleBoxException(
+                "In infer_nvinfer_config.txt, no such key model-engine-file",
+                ExceptionCode.APP_CONFIG_ERROR,
+            )
 
-        input_dims = nvinfer_parser.get('infer-dims')
+        input_dims = nvinfer_parser.get("infer-dims")
         if not input_dims:
-            raise WaffleBoxException('In infer_nvinfer_config.txt, no such key infer-dims',
-                                     ExceptionCode.APP_CONFIG_ERROR)
-        input_dims = input_dims.replace(';', 'x')
+            raise WaffleBoxException(
+                "In infer_nvinfer_config.txt, no such key infer-dims", ExceptionCode.APP_CONFIG_ERROR
+            )
+        input_dims = input_dims.replace(";", "x")
 
-        batch_size = nvinfer_parser.get('batch-size')
+        batch_size = nvinfer_parser.get("batch-size")
         if not batch_size:
-            raise WaffleBoxException('In infer_nvinfer_config.txt, no such key batch-size',
-                                     ExceptionCode.APP_CONFIG_ERROR)
+            raise WaffleBoxException(
+                "In infer_nvinfer_config.txt, no such key batch-size", ExceptionCode.APP_CONFIG_ERROR
+            )
         batch_size = int(batch_size)
 
         return ModelInfo(
-            id=model_id, name=model_name, precision=model_precision,
-            engine_file_name=engine_file_name, input_dims=input_dims,
-            max_batch_size=batch_size, path=model_path,
+            id=model_id,
+            name=model_name,
+            precision=model_precision,
+            engine_file_name=engine_file_name,
+            input_dims=input_dims,
+            max_batch_size=batch_size,
+            path=model_path,
         )
 
     def _remove_extention(self, file_name: str) -> str:
-        """ 파일 이름에서 마지막 확장자 명을 제거한다.
+        """파일 이름에서 마지막 확장자 명을 제거한다.
 
         Args:
             file_name (str): 확장자 명을 제거할 파일 경로 스트링
         """
-        return file_name[:file_name.rfind('.')]
+        return file_name[: file_name.rfind(".")]
 
     def replace_model(self, model_id: UUID, new_model: Path) -> None:
-        """ 모델의 trt 엔진 파일을 교체한다.
+        """모델의 trt 엔진 파일을 교체한다.
 
         입력한 id에 해당하는 모델의 trt 엔진 파일을 새로운 trt 엔진 파일로 교체한다.
 
         Args:
             model_id (UUID): 교체할 모델의 id
             new_model (Path): 새로운 모델 주소
 
@@ -197,83 +213,83 @@
                 새로운 모델 파일이 존재하지 않음
 
         """
         model = self._app_structure.find_model_by_id(model_id)
 
         if not model:
             raise WaffleBoxException(
-                f'No such model: ID - {model_id}', ExceptionCode.APP_NO_SUCH_FILE)
+                f"No such model: ID - {model_id}", ExceptionCode.APP_NO_SUCH_FILE
+            )
 
         # 기존 모델 파일 확인
         origin_model = model.path.joinpath(model.engine_file_name)
         if not origin_model.exists():
-            raise WaffleBoxException(
-                f'No such file: {origin_model}', ExceptionCode.APP_NO_SUCH_FILE)
+            raise WaffleBoxException(f"No such file: {origin_model}", ExceptionCode.APP_NO_SUCH_FILE)
 
         # 새로운 모델 파일 확인
         if not new_model.exists():
-            raise WaffleBoxException(
-                f'No such file: {new_model}', ExceptionCode.APP_NO_SUCH_FILE)
+            raise WaffleBoxException(f"No such file: {new_model}", ExceptionCode.APP_NO_SUCH_FILE)
 
         # 모델 교체
         os.remove(origin_model)
         shutil.copyfile(new_model, origin_model)
 
     def package(self, output: Path) -> None:
-        """ 새로운 App으로 생성한다.
+        """새로운 App으로 생성한다.
 
         엔진 파일 교체가 끝나면 새로운 App으로 패키징한다.
 
         Args:
             output (Path): App 저장 경로
 
         Raises:
             APP_FILE_ALREADY_EXIST: output 파일이 이미 존재함
 
         """
         if output.exists():
             raise WaffleBoxException(
-                f'File already exists: {output}', ExceptionCode.APP_FILE_ALREADY_EXIST)
+                f"File already exists: {output}", ExceptionCode.APP_FILE_ALREADY_EXIST
+            )
 
         for model in self._app_structure.models:
-            shutil.make_archive(str(model.path), 'zip', str(model.path))
+            shutil.make_archive(str(model.path), "zip", str(model.path))
             shutil.rmtree(model.path)
 
         # shutil에서 .zip을 붙이므로 마지막에 .zip이 붙어있다면
         # 없앤 이름을 넣어준다.
         output_name = str(output)
-        if len(output_name) > 4 and output_name[-4:] == '.zip':
+        if len(output_name) > 4 and output_name[-4:] == ".zip":
             output_name = output_name[:-4]
 
-        shutil.make_archive(output_name, 'zip', self._app_structure.path)
+        shutil.make_archive(output_name, "zip", self._app_structure.path)
 
     @property
     def app_structure(self) -> AppStructure:
-        """ App 구조를 반환한다.
-        """
+        """App 구조를 반환한다."""
         return self._app_structure
 
     def find_model_info_by_id(self, id: UUID) -> ModelInfo | None:
-        """ App의 모델 정보를 id로 찾는다.
+        """App의 모델 정보를 id로 찾는다.
 
-        App의 모델 정보를 id로 찾는다. 
+        App의 모델 정보를 id로 찾는다.
         만약 없다면 None을 리턴한다.
 
         Args:
             id (UUID): 찾고싶은 모델의 id
 
         """
         return self._app_structure.find_model_by_id(id)
 
     def find_model_info_by_name(self, name: str) -> ModelInfo | None:
-        """ App의 모델 정보를 이름으로 찾는다.
+        """App의 모델 정보를 이름으로 찾는다.
 
         App의 모델 정보를 이름으로 찾는다.
         만약 없다면 None을 리턴한다.
 
         Args:
             name (str): 찾고싶은 모델의 이름
         """
         return self._app_structure.find_model_by_name(name)
 
-if __name__ == '__main__':
-    ap = AppManager(Path('/'), Path('/'))
+
+if __name__ == "__main__":
+    ap = AppManager(Path("/"), Path("/"))
```

### Comparing `waffle_box-0.1.0/app_manager/app_structure.py` & `waffle_box-0.2.0/app_manager/app_structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from maker_manager import ONNXConvConfigs
-
 from dataclasses import dataclass
+from pathlib import Path
 from typing import List
 from uuid import UUID
-from pathlib import Path
+
+from maker_manager import ONNXConvConfigs
 
 
 @dataclass(frozen=True)
 class ModelInfo:
-    """ 모델 정보
+    """모델 정보
 
     모델의 기본 정보를 저장한다. (불변값)
 
     Attributes:
         id (UUID): model.json에 기술되어 있는 모델의 uuid
         name (str): model.json에 기술되어 있는 모델의 이름
-        precision (str): 모델의 precision, 
+        precision (str): 모델의 precision,
             fp32, fp16, int8 중 하나
         engine_file_name (str): engine 파일 이름, 보통 model.engine
         input_dims (str): 모델의 input shape, x로 구분
             예) 3x640x640
         max_batch_size (int): 모델의 batch size
             Autocare-D는 기본적으로 dynamic batch를 가정하므로
             모델에 적혀있는 batch-size는 max batch size로 간주한다.
@@ -32,45 +32,44 @@
     precision: str
     engine_file_name: str
     input_dims: str
     max_batch_size: int
     path: Path
 
     def to_onnx_config(self) -> ONNXConvConfigs:
-        """ ONNX 파일을 trt 엔진 파일로 변환하는데 필요한 정보
+        """ONNX 파일을 trt 엔진 파일로 변환하는데 필요한 정보
 
-        ONNX 파일을 trt 엔진 파일로 변환하는데 
+        ONNX 파일을 trt 엔진 파일로 변환하는데
         필요한 설정 값을 모델 정보에서 얻는다.
 
         """
         return ONNXConvConfigs(
-            precision=self.precision, 
-            input_shapes=self.input_dims,
-            max_batch=self.max_batch_size
+            precision=self.precision, input_shapes=self.input_dims, max_batch=self.max_batch_size
         )
 
 
 @dataclass(frozen=True)
 class AppStructure:
-    """ App 구조 정보
+    """App 구조 정보
 
     App의 구조 정보를 저장한다. (변경 불가)
 
-    Attributes: 
+    Attributes:
         id (UUID): app.json에 기술되어 있는 App의 UUID
         models (List[ModelInfo]): App이 모델 정보 리스트
         path (Path): App을 압축 푼 경로
 
     """
+
     id: UUID
     models: List[ModelInfo]
     path: Path
 
     def find_model_by_id(self, id: UUID) -> ModelInfo | None:
-        """ id 값으로 모델을 찾는다.
+        """id 값으로 모델을 찾는다.
 
         Args:
             id (UUID): 찾는 모델의 uuid
 
         Returns:
             ModelInfo: 입력한 id와 일치하는 모델
             None: 입력한 id와 일치하는 모델을 찾지 못했을 때
@@ -79,15 +78,15 @@
         for m in self.models:
             if m.id == id:
                 return m
 
         return None
 
     def find_model_by_name(self, name: str) -> ModelInfo | None:
-        """ 이름으로 모델을 찾는다.
+        """이름으로 모델을 찾는다.
 
         Args:
             name (str): 찾는 모델의 이름
 
         Returns:
             ModelInfo: 입력한 이름과 일치하는 모델
             None: 입력한 이름과 일치하는 모델을 찾지 못했을 때
```

### Comparing `waffle_box-0.1.0/app_manager/nvinfer_config_parser.py` & `waffle_box-0.2.0/app_manager/nvinfer_config_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
-from waffle_box_exception import WaffleBoxException, ExceptionCode
+
+from waffle_box_exception import ExceptionCode, WaffleBoxException
 
 
 class NvinferConfigParser:
-    """ nvinfer config 파일 분석
+    """nvinfer config 파일 분석
 
     정확한 trt 엔진 변환을하기 위해 nvinfer config 파일을 읽고
     변환 설정 값을 만들기 위해 사용된다.
 
     설정값 접근은 get함수로 config 파일의 key 값을 입력해 찾는다.
     key값이 없을 경우 Exception을 발생한다.
 
@@ -15,24 +16,24 @@
         _configs (dict[str, str]): config값을 저장하는 dictionary
 
     """
 
     def __init__(self, file: Path) -> None:
         """
         Args:
-            file (Path): config 파일 위치 
+            file (Path): config 파일 위치
                 예) /home/yoon/.waffle_box/temp/car_make_net_v0.1.0a/infer_nvinfer_config.txt
 
         """
         self._configs: dict[str, str] = {}
 
         self._read_config_file(file)
 
     def _read_config_file(self, file: Path) -> None:
-        """ config 파일 파싱
+        """config 파일 파싱
 
         config 파일을 읽고 설정 값만 _configs에 저장한다.
 
         Args:
             file (Path): nvinfer config 파일 경로
 
         Raises:
@@ -41,37 +42,38 @@
 
         """
         try:
             with open(file) as f:
                 lines = f.readlines()
 
                 for l in lines:
-                    sp = l.split('=')
+                    sp = l.split("=")
 
                     if len(sp) != 2:
                         continue
 
                     # remove white space and new line
-                    self._configs[sp[0].strip()] = sp[1].strip().replace(
-                        '\n', '')
+                    self._configs[sp[0].strip()] = sp[1].strip().replace("\n", "")
         except FileNotFoundError as e:
             raise WaffleBoxException(
-                f'No infer_nvinfer_config.txt file.', ExceptionCode.APP_NO_SUCH_FILE)
+                f"No infer_nvinfer_config.txt file.", ExceptionCode.APP_NO_SUCH_FILE
+            )
         except Exception as e:
             raise WaffleBoxException(
-                f'Error while reading infer_nvinfer_config.txt: {e}', ExceptionCode.APP_CONFIG_ERROR)
+                f"Error while reading infer_nvinfer_config.txt: {e}", ExceptionCode.APP_CONFIG_ERROR
+            )
 
     def get(self, key: str) -> str | None:
-        """ config 값 읽어오기
+        """config 값 읽어오기
 
         key를 통해 config 값을 읽어온다.
         key값이 존재하지 않을경우 None을 리턴한다.
 
         Args:
             key (str): 읽어올 설정값의 키
-        
+
         Returns:
             str: 읽어온 key의 값
             None: key 없음
 
         """
         return self._configs.get(key)
```

### Comparing `waffle_box-0.1.0/maker_manager/convert_option.py` & `waffle_box-0.2.0/maker_manager/convert_option.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 from dataclasses import dataclass
-from waffle_box_exception import WaffleBoxException, ExceptionCode
+
+from waffle_box_exception import ExceptionCode, WaffleBoxException
 
 
 @dataclass(frozen=True)
 class ONNXConvConfigs:
-    """ trt 엔진 변환을 위해 필요한 설정 값 정보
+    """trt 엔진 변환을 위해 필요한 설정 값 정보
 
     Attributes:
         precision (str): 모델의 precision,
             fp32, fp16, int8 중 하나
         input_shape (str): 모델의 input shape
-            dynamic batch를 사용하기 위해 trtexec에 
+            dynamic batch를 사용하기 위해 trtexec에
             min, opt, max input shape을 입력할 때 사용
         max_batch (int): 모델의 최대 batch 크기
             min, opt, max input shape의 batch 크기를 결정할 때 사용
 
     """
 
     precision: str
     input_shapes: str
     max_batch: int
 
     def to_trtexec_args(self) -> list[str]:
-        """ trtexec 변환에 필요한 argument 리스트로 변환
+        """trtexec 변환에 필요한 argument 리스트로 변환
 
         ONNXConvConfigs의 값을 trtexec 변환에 필요한 argument 리스트로 변환한다.
 
         precision:
             trtexec의 precision 기본값은 fp32이므로 fp32일때는 아무런 옵션을 생성하지 않는다.
             fp16일 경우 --fp16, int8일 경우 --int8을 리턴한다.
 
         input_shape & max_batch:
-            dynamic batch를 사용하기 위해 min, opt, max shape을 설정해야 한다.  
+            dynamic batch를 사용하기 위해 min, opt, max shape을 설정해야 한다.
             모델의 input_shape은 그대로 사용하며 batch size는 min=1, opt=max_batch/2, max=max_batch로 설정한다.
 
         output_name:
             App의 원본 엔진파일 이름을 맞추기 위해 설정한다.
             --saveEngine=<output_name>
-        
+
         Returns:
             list[str]: trtexec에 필요한 argument 리스트
 
         """
 
         args: list[str] = []
 
         # precision
-        if self.precision == 'fp16':
-            args.append('--fp16')
-        elif self.precision == 'int8':
-            args.append('--int8')
-        elif self.precision != 'fp32':
+        if self.precision == "fp16":
+            args.append("--fp16")
+        elif self.precision == "int8":
+            args.append("--int8")
+        elif self.precision != "fp32":
             raise WaffleBoxException(
-                f'Invalid precision: {self.precision}', ExceptionCode.APP_CONFIG_ERROR)
+                f"Invalid precision: {self.precision}", ExceptionCode.APP_CONFIG_ERROR
+            )
 
         # dynamic batch
         # 구체적인 layer 이름이 필요하지만 현재는 inputs 레이어 한개만 있다 가정
         # min
-        args.append(f'--minShapes=inputs:1x{self.input_shapes}')
+        args.append(f"--minShapes=inputs:1x{self.input_shapes}")
 
         # opt
         if self.max_batch > 2:
-            args.append(
-                f'--optShapes=inputs:{int(self.max_batch/2)}x{self.input_shapes}')
+            args.append(f"--optShapes=inputs:{int(self.max_batch/2)}x{self.input_shapes}")
 
         # max
-        args.append(
-            f'--maxShapes=inputs:{int(self.max_batch)}x{self.input_shapes}')
+        args.append(f"--maxShapes=inputs:{int(self.max_batch)}x{self.input_shapes}")
 
         return args
```

### Comparing `waffle_box-0.1.0/maker_manager/maker_manager.py` & `waffle_box-0.2.0/maker_manager/maker_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-import os
-import signal
 import atexit
+import os
 import shutil
+import subprocess
 import tarfile
+from pathlib import Path
+from typing import Union
+from uuid import uuid4
 
 import docker
-from pathlib import Path
 
 from maker_manager.convert_option import ONNXConvConfigs
-from waffle_box_exception.waffle_box_exception import WaffleBoxException, ExceptionCode
+from maker_manager.thread_handler import ConvertThreadHandler
+from waffle_box_exception.waffle_box_exception import ExceptionCode, WaffleBoxException
 
 
 class MakerManager:
     """Waffle Maker Manager
 
     ONNX 파일을 TensorRT 엔진 파일로 변환하는 Waffle Maker를 관리하는 클래스.
     이미지 다운로드, 모델 파일 변환 등의 기능을 제공한다.
 
     Attributes:
         img_tag (str): 실행할 이미지 태그
         gpu_num (int): 컨테이너를 동작할 gpu 번호
-        container_id (int | None): 실행한 컨테이너 ID로 
+        container_id (int | None): 실행한 컨테이너 ID로
             컨테이너를 정상적으로 종료시키지 못했을 때 회수하기 위해 저장한다.
             None일경우 회수할 컨테이너 없음
         workspace (Path): 압축푸는 작업 등 파일 관리를 위한 workspace
         client (DockerClient): 도커 클라이언트
-    
+
     """
 
     def __init__(self, img_tag: str, gpu_num: int, workspace: Path) -> None:
         """
-        Args: 
+        Args:
             img_tag (str): 실행할 이미지 태그
             gpu_num (str): 컨테이너를 동작할 gpu 번호
             workspace (Path): 작업할 경로, 일반적으로 ~/.waffle_box
-            
+
         Raises:
             DockerDaemonError: Docker daemon에 접속 불가
 
         """
         self.img_tag = img_tag
         self.gpu_num = gpu_num
         self.container_id = None
-        self.workspace = workspace
+        self.log = []
+        self.workspace = workspace.joinpath(f"{uuid4()}/")
+
+        os.mkdir(self.workspace)
 
         self.client = docker.from_env()
 
         atexit.register(self.exit_container_handler)
-        signal.signal(signal.SIGINT, self.exit_container_handler)
-        signal.signal(signal.SIGTERM, self.exit_container_handler)
 
         if not self.client.ping():
-            raise WaffleBoxException(
-                "Docker daemon eror.", ExceptionCode.DOCKER_EXCEPTION
-            )
+            raise WaffleBoxException("Docker daemon eror.", ExceptionCode.DOCKER_EXCEPTION)
+
+    def __del__(self):
+        os.rmdir(self.workspace)
 
     def check_image_exist_at_local(self) -> bool:
         """로컬에 이미지가 설치되어 있는지 확인한다.
 
         MakerManager를 생성할 때 입력한 이미지 태그가 로컬에 존재하는지 확인한다.
 
         Returns:
@@ -68,17 +73,15 @@
             self.client.images.get(self.img_tag)
 
         except Exception as e:
             return False
 
         return True
 
-    def pull_image_at_local(
-        self, print_output: bool, id: str = "", pw: str = ""
-    ) -> None:
+    def pull_image_at_local(self, print_output: bool, id: str = "", pw: str = "") -> None:
         """로컬에 이미지를 다운받는다.
 
         MakerManager를 생성할 때 입력한 이미지 태그를 로컬에 다운받는다.
         만약 id와 pw를 입력했다면 docker hub에 로그인을 한 후 다운받는다.
 
         Args:
             id (str): docker hub id, 빈값이라면 로그인을 하지 않는다.
@@ -91,187 +94,211 @@
 
         """
         if id and pw:
             try:
                 self.client.login(id, pw)
 
             except docker.errors.APIError as e:
-                raise WaffleBoxException(
-                    "Login error.", ExceptionCode.DOCKER_IMAGE_EXCEPTION
-                )
+                raise WaffleBoxException("Login error.", ExceptionCode.DOCKER_IMAGE_EXCEPTION)
 
         if self.check_image_exist_at_local():
-            raise WaffleBoxException(
-                "Image already exist.", ExceptionCode.DOCKER_IMAGE_EXCEPTION
-            )
+            raise WaffleBoxException("Image already exist.", ExceptionCode.DOCKER_IMAGE_EXCEPTION)
 
         try:
             if print_output:
+                progress = {}
+
                 for line in self.client.api.pull(self.img_tag, stream=True, decode=True):
-                    print(line)
+                    if line.get("id"):
+                        progress[line["id"]] = line
+
+                    subprocess.call("clear", shell=True)
+                    for i, val in progress.items():
+                        print(val)
 
             else:
                 self.client.images.pull(self.img_tag)
 
         except docker.errors.APIError as e:
-            raise WaffleBoxException(
-                "Permission error.", ExceptionCode.DOCKER_IMAGE_EXCEPTION
-            )
+            raise WaffleBoxException("Permission error.", ExceptionCode.DOCKER_IMAGE_EXCEPTION)
 
-    def run_container_at_local(self, print_output: bool) -> None:
+    def run_container_at_local(self, print_output: bool, allow_multiple_containers: bool) -> None:
         device_info = docker.types.DeviceRequest(
             device_ids=[str(self.gpu_num)], capabilities=[["gpu"]]
         )
 
+        if not allow_multiple_containers:
+            for i in self.client.api.containers():
+                if i["Image"] == self.img_tag:
+                    raise WaffleBoxException(
+                        "Already run container. If you want runing multiple_container, \
+                            set allow_multiple_containers=True.",
+                        ExceptionCode.DOCKER_RUN_EXCEPTION,
+                    )
         try:
             container = self.client.containers.run(
                 self.img_tag,
                 stdin_open=True,
                 detach=True,
                 auto_remove=True,
                 device_requests=[device_info],
             )
             self.container_id = container.id
 
         except docker.errors.ImageNotFound as e:
-            raise WaffleBoxException(
-                "Wrong image error.", ExceptionCode.DOCKER_RUN_EXCEPTION
-            )
+            raise WaffleBoxException("Wrong image error.", ExceptionCode.DOCKER_RUN_EXCEPTION)
 
         except docker.errors.APIError as e:
             raise WaffleBoxException("Http error.", ExceptionCode.DOCKER_RUN_EXCEPTION)
 
         except docker.errors.ContainerError as e:
-            raise WaffleBoxException(
-                "Container error.", ExceptionCode.DOCKER_RUN_EXCEPTION
-            )
+            raise WaffleBoxException("Container error.", ExceptionCode.DOCKER_RUN_EXCEPTION)
 
     def convert_onnx_to_engine_at_local(
         self,
         input: Path,
         output: Path,
         convert_config: ONNXConvConfigs,
         print_output: bool,
-    ) -> None:
-        """입력한 모델 파일을 trt 엔진으로 변환
-
-        입력한 모델을 컨테이너 내부에서 TensorRT 엔진으로 변환한다.
-        변환한 모델은 output path에 저장한다.
+        using_thread: bool,
+        allow_multiple_containers: bool,
+        thread_handler: ConvertThreadHandler,
+    ) -> Union[ConvertThreadHandler, None]:
+        def convert(
+            self,
+            input: Path,
+            output: Path,
+            convert_config: ONNXConvConfigs,
+            print_output: bool,
+            allow_multiple_containers: bool,
+        ) -> None:
+            """입력한 모델 파일을 trt 엔진으로 변환
+
+            입력한 모델을 컨테이너 내부에서 TensorRT 엔진으로 변환한다.
+            변환한 모델은 output path에 저장한다.
+
+            Args:
+                input (Path): 변환할 모델 경로
+                output (Path): 변환한 모델 저장 경로
+                convert_config (ONNXConvConfigs): trtexec를 실행할 os.remove('temp.tar') 때 필요한 설정값들
+                print_output (bool): container 출력 결과 표시 여부
+
+            Raises:
+                IOError: input 파일이 존재하지 않음, output 파일이 이미 존재함
+                ConvertError: 변환 실패
+
+            """
+
+            def create_tar_file(input_path: Path):
+                def set_permissions(tarinfo):
+                    tarinfo.mode = 0o777
+                    return tarinfo
 
-        Args:
-            input (Path): 변환할 모델 경로
-            output (Path): 변환한 모델 저장 경로
-            convert_config (ONNXConvConfigs): trtexec를 실행할 os.remove('temp.tar') 때 필요한 설정값들
-            print_output (bool): container 출력 결과 표시 여부
+                with tarfile.open(self.workspace.joinpath("model.tar"), "w") as tar:
+                    tar.add(input_path, filter=set_permissions, arcname=f"{file_name}.onnx")
 
-        Raises:
-            IOError: input 파일이 존재하지 않음, output 파일이 이미 존재함
-            ConvertError: 변환 실패
+            def get_tar_file(input_path: Path, output_path: Path):
+                container = self.client.containers.get(self.container_id)
+                data, _ = container.get_archive(input_path)
 
-        """
+                tar_path = self.workspace.joinpath("engine.tar")
 
-        def create_tar_file(input_path: Path):
-            def set_permissions(tarinfo):
-                tarinfo.mode = 0o777
-                return tarinfo
-
-            with tarfile.open(self.workspace.joinpath("model.tar"), "w") as tar:
-                tar.add(input_path, filter=set_permissions, arcname=f"{file_name}.onnx")
-            
+                with open(tar_path, "wb") as f:
+                    for chunk in data:
+                        f.write(chunk)
 
-        def get_tar_file(input_path: Path, output_path: Path):
-            container = self.client.containers.get(self.container_id)
-            data, _ = container.get_archive(input_path)
+                with tarfile.open(tar_path, "r") as tar:
+                    tar.extractall(self.workspace)
 
-            tar_path = self.workspace.joinpath("engine.tar")
+                origin_path = self.workspace
 
-            with open(tar_path, "wb") as f:
-                for chunk in data:
-                    f.write(chunk)
-
-            with tarfile.open(tar_path, "r") as tar:
-                tar.extractall(self.workspace)
-            
-            origin_path = self.workspace
-            
-            os.rename(origin_path.joinpath(f"{file_name}.engine"), output_path)
-            os.remove(tar_path)
-
-        if not os.path.exists(input):
-            raise WaffleBoxException(
-                "Input_file not exists.", ExceptionCode.MODEL_IO_Eself.wXCEPTION
-            )
+                os.rename(origin_path.joinpath(f"{file_name}.engine"), output_path)
+                os.remove(tar_path)
 
-        if os.path.exists(output):
-            raise WaffleBoxException(
-                "Already output_file exists", ExceptionCode.MODEL_IO_EXCEPTION
-            )
+            if not os.path.exists(input):
+                raise WaffleBoxException("Input_file not exists.", ExceptionCode.MODEL_IO_EXCEPTION)
 
-        try:
-            self.run_container_at_local(print_output=print_output)
+            if os.path.exists(output):
+                raise WaffleBoxException(
+                    "Already output_file exists", ExceptionCode.MODEL_IO_EXCEPTION
+                )
 
-            tmp_input = "/" + str(input)
+            self.run_container_at_local(
+                print_output=print_output, allow_multiple_containers=allow_multiple_containers
+            )
 
-            file_name = tmp_input[tmp_input.rfind("/") + 1 : tmp_input.rfind(".")]
+            try:
+                tmp_input = "/" + str(input)
 
-            create_tar_file(input)
+                file_name = tmp_input[tmp_input.rfind("/") + 1 : tmp_input.rfind(".")]
 
-            with open(self.workspace.joinpath("model.tar"), "rb") as f:
-                container = self.client.containers.get(self.container_id)
-                result = container.put_archive(path="/opt", data=f.read())
+                create_tar_file(input)
 
-            if not result:
-                raise WaffleBoxException('put_archive error.', ExceptionCode.MODEL_IO_EXCEPTION)
+                with open(self.workspace.joinpath("model.tar"), "rb") as f:
+                    container = self.client.containers.get(self.container_id)
+                    result = container.put_archive(path="/opt", data=f.read())
 
-            if print_output:
-                print("Convert model...")
+                if not result:
+                    raise WaffleBoxException("put_archive error.", ExceptionCode.MODEL_IO_EXCEPTION)
 
                 convert_option_list = convert_config.to_trtexec_args()
-                convert_option = ' '.join(convert_option_list)
+                convert_option = " ".join(convert_option_list)
 
-                exec_result = self.client.api.exec_create(container=self.container_id,
-                                                          cmd=f"trtexec --onnx=/opt/{file_name}.onnx \
+                exec_result = self.client.api.exec_create(
+                    container=self.container_id,
+                    cmd=f"trtexec --onnx=/opt/{file_name}.onnx \
                                                                         {convert_option} \
                                                                         --saveEngine={file_name}.engine",
-                                                          privileged=True)
-                exec_output = self.client.api.exec_start(exec_result['Id'], stream=True)
+                    privileged=True,
+                )
+                exec_output = self.client.api.exec_start(exec_result["Id"], stream=True)
 
-                for line in exec_output:
-                    print(line.decode('utf-8'))
+                if print_output:
+                    for line in exec_output:
+                        temp = line.decode("utf-8")
+                        self.log.append(temp)
+                        print(temp)
+                else:
+                    for line in exec_output:
+                        temp = line.decode("utf-8")
+                        self.log.append(temp)
+
+                get_tar_file(
+                    Path(f"/workspace/{file_name}.engine"),
+                    Path(output),
+                )
 
-            else:
-               container.exec_run(
-                    f"trtexec --onnx=/opt/{file_name}.onnx\
-                                    --saveEngine={file_name}.engine",
-                    privileged=True,
-                ) 
+            except Exception as e:
+                raise WaffleBoxException("Convert error.", ExceptionCode.MODEL_CONVERT_EXCEPTION)
 
-            get_tar_file(
-                Path(f"/workspace/{file_name}.engine"),
-                Path(output),
-            )
+            finally:
+                os.remove(self.workspace.joinpath("model.tar"))
 
-        except Exception as e:
-            raise WaffleBoxException(
-                "Convert error.", ExceptionCode.MODEL_CONVERT_EXCEPTION
-            )
+                try:
+                    container = self.client.containers.get(self.container_id)
+                    container.kill()
 
-        finally:
-            os.remove(self.workspace.joinpath("model.tar"))
+                except Exception as e:
+                    print(e)
 
-            try:
-                container = self.client.containers.get(self.container_id)
-                container.kill()
+                if print_output:
+                    print("Convert finished.")
 
-            except Exception as e:
-                print(e)
+        if using_thread:
+            if thread_handler is None:
+                thread_handler = ConvertThreadHandler(convert)
+
+            thread_handler.add_work(self, input, output, convert_config, print_output, allow_multiple_containers)
+
+            return thread_handler
+
+        else:
+            convert(self, input, output, convert_config, print_output, allow_multiple_containers)
+            return None
 
-            if print_output:
-                print("Convert finished.")
-    
     def exit_container_handler(self):
         try:
             container = self.client.containers.get(self.container_id)
             container.kill()
-        
+
         except Exception as e:
             pass
```

### Comparing `waffle_box-0.1.0/pyproject.toml` & `waffle_box-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "waffle-box"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["SangHyeukYoon <shyoon@snuailab.ai>"]
 readme = "README.md"
 packages = [
     { include = "waffle_box" },
     { include = "app_manager" },
     { include = "maker_manager" },
@@ -14,18 +14,19 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
 docker = "^6.1.3"
 black = "^23.7.0"
 pytest = "^7.4.0"
 pytest-html = "^3.2.0"
+pre-commit = "^3.3.3"
 
 [tool.poetry.scripts]
 wb = "waffle_box.cli:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [virtualenvs]
 create = true
-in-project = true
+in-project = true
```

### Comparing `waffle_box-0.1.0/waffle_box/bake_service.py` & `waffle_box-0.2.0/waffle_box/bake_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+import re
+from pathlib import Path
+
 from maker_manager import MakerManager, ONNXConvConfigs
+from maker_manager.thread_handler import ConvertThreadHandler
 from waffle_box_exception.waffle_box_exception import ExceptionCode, WaffleBoxException
 
-from pathlib import Path
-import re
-
 
 class BakeService:
-    """ ONNX 모델을 trt 엔진으로 변환
+    """ONNX 모델을 trt 엔진으로 변환
 
     사용자가 입력한 ONNX 모델을 타겟 Autocare-D 버전에 맞춰 trt 엔진 파일로 변환한다.
 
     실행 순서:
-        1. is_local_maker_installed: Waffle Maker 이미지가 
+        1. is_local_maker_installed: Waffle Maker 이미지가
             로컬에 설치되어 있는지 확인한다.
         2. convert_model: 모델을 trt 엔진으로 변환한다.
 
     Attributes:
         workspace (Path): 작업할 경로, 일반적으로 ~/.waffle_box
         origin_app_path (Path): 사용자가 입력한 기존 App 경로
         final_app_path (Path): 새로운 App을 저장할 경로
         img_tag (str): trt 변환을 위한 컨테이너 태그명
         maker_manager (MakerManager): maker manager
 
     """
 
-    def __init__(self, workspace: Path, input: Path, output: Path, dx_target_version: str, gpu_num: int) -> None:
+    def __init__(
+        self, workspace: Path, input: Path, output: Path, dx_target_version: str, gpu_num: int
+    ) -> None:
         """
         Args:
             workspace (Path): 작업할 경로
             input (Path): 변환할 모델 경로
             output (Path): 변환한 trt 엔진 파일을 저장할 경로
             dx_target_version (str): 변환할 App의 target Autocare-D 버전
             gpu_num (int): 작업할 GPU 번호
@@ -38,46 +41,63 @@
 
         """
         self.workspace: Path = workspace
         self.origin_model_path: Path = input
         self.final_model_path: Path = output
 
         # TODO: make image tag converter
-        self.img_tag = 'snuailab/trt:8.5.2.2'
+        self.img_tag = "snuailab/trt:8.5.2.2"
 
         self.maker_manager = MakerManager(self.img_tag, gpu_num, workspace)
 
     def is_local_maker_installed(self) -> bool:
-        """ Waffle maker가 local에 설치되어 있는가?
+        """Waffle maker가 local에 설치되어 있는가?
 
         Returns:
             True: 설치되어 있음
             False: 설치되어 있지 않음
         """
         return self.maker_manager.check_image_exist_at_local()
 
-    def convert_model(self, print_output: bool, precision: str, input_shapes: str, max_batch: int) -> None:
-        """ 모델 변환
+    def convert_model(
+        self,
+        print_output: bool,
+        precision: str,
+        input_shapes: str,
+        max_batch: int,
+        using_thread: bool = False,
+        allow_multiple_containers: bool = False,
+        thread_handler: ConvertThreadHandler = None,
+    ) -> ConvertThreadHandler | None:
+        """모델 변환
 
         Args:
             print_output (bool): 변환 과정 출력 여부
             precision (str): 모델의 precision,
                 fp32, fp16, int8 중 하나
             input_shapes (str): 모델의 인풋 크기, {channel}x{width}x{height} 포맷
                 예) 3x640x640
+            using_thread (bool): thread로 동작할지 여부
+            allow_multiple_containers (bool): convert container 실행 중복 허용 여부
 
         Raises:
             INVALID_ARGUMENT: input shapes의 포맷이 잘못됨
 
         """
         # validate input shapes
-        p = re.compile(r'\d+x\d+x\d+')
+        p = re.compile(r"\d+x\d+x\d+")
         m = p.match(input_shapes)
 
         if m == None or m.start() != 0 or m.end() != len(input_shapes):
-            raise WaffleBoxException('Invalid input shapes', ExceptionCode.INVALID_ARGUMENT)
-
+            raise WaffleBoxException("Invalid input shapes", ExceptionCode.INVALID_ARGUMENT)
         onnx_config = ONNXConvConfigs(precision, input_shapes, max_batch)
-        self.maker_manager.convert_onnx_to_engine_at_local(input=self.origin_model_path,
-                                                           output=self.final_model_path,
-                                                           convert_config=onnx_config,
-                                                           print_output=print_output)
+        handler = self.maker_manager.convert_onnx_to_engine_at_local(
+            input=self.origin_model_path,
+            output=self.final_model_path,
+            convert_config=onnx_config,
+            print_output=print_output,
+            using_thread=using_thread,
+            allow_multiple_containers=allow_multiple_containers,
+            thread_handler=thread_handler
+        )
+
+        return handler if handler is not None else None
```

### Comparing `waffle_box-0.1.0/waffle_box/convert_service.py` & `waffle_box-0.2.0/waffle_box/convert_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from app_manager import AppManager, ModelInfo, AppStructure
-from maker_manager import MakerManager
-
+import os
 from pathlib import Path
 from uuid import UUID
-import os
+from uuid import uuid4
+
+from app_manager import AppManager, AppStructure, ModelInfo
+from maker_manager import MakerManager
+from maker_manager.thread_handler import ConvertThreadHandler
 
 
 class ConvertService:
-    """ 기존 앱을 바탕으로 새로운 앱을 생성
+    """기존 앱을 바탕으로 새로운 앱을 생성
 
     기존 앱에서 모델을 교체해 새로운 앱을 생성한다.
 
     실행 순서:
         1. is_local_maker_installed: waffle maker가 local에 설치되어 있는지 확인한다.
         2. get_model_info: 입력한 App의 모델 정보를 받아온다.
         3. add_convert_info: 모델 정보를 바탕으로 변경할 모델들을 입력한다.
@@ -25,15 +27,17 @@
         img_tag (str): trt 변환을 위한 컨테이너 태그명
         convert_list (dict[UUID, Path]): 변경할 모델 리스트
         app_manager (AppManager): app manager
         maker_manager (MakerManager): maker manager
 
     """
 
-    def __init__(self, workspace: Path, input: Path, output: Path, dx_target_version: str, gpu_num: int) -> None:
+    def __init__(
+        self, workspace: Path, input: Path, output: Path, dx_target_version: str, gpu_num: int
+    ) -> None:
         """
         Args:
             workspace (Path): 작업할 경로
             input (Path): 변환할 App 경로
             output (Path): 새로운 App을 저장할 경로
             dx_target_version (str): 변환할 App의 target Autocare-D 버전
             gpu_num (int): 작업할 GPU 번호
@@ -44,85 +48,91 @@
 
         """
         self.workspace: Path = workspace
         self.origin_app_path: Path = input
         self.final_app_path: Path = output
 
         # TODO: make image tag converter
-        self.img_tag = 'snuailab/trt:8.5.2.2'
+        self.img_tag = "snuailab/trt:8.5.2.2"
 
         self.convert_list: dict[UUID, Path] = {}
 
         self.app_manager = AppManager(self.workspace, self.origin_app_path)
-        self.maker_manager = MakerManager(
-            self.img_tag, gpu_num=gpu_num, workspace=self.workspace)
+        self.maker_manager = MakerManager(self.img_tag, gpu_num=gpu_num, workspace=self.workspace)
 
     def is_local_maker_installed(self) -> bool:
-        """ Waffle maker가 local에 설치되어 있는가?
+        """Waffle maker가 local에 설치되어 있는가?
 
         Returns:
             True: 이미지가 설치되어 있음
             False: 이미지가 설치되어 있지 않음
         """
         return self.maker_manager.check_image_exist_at_local()
 
     def get_model_info(self) -> list[ModelInfo]:
-        """ 모델 정보 받아오기
+        """모델 정보 받아오기
 
         사용자가 입력한 App의 모델 정보들을 리스트로 반환한다.
 
         Returns:
             list[ModelInfo]: 모델 정보 리스트
 
         """
         return self.app_manager.app_structure.models
 
     def add_convert_info(self, model_id: UUID, new_model_path: Path) -> None:
-        """ 변환할 모델 정보 등록
+        """변환할 모델 정보 등록
 
         변환할 모델 정보를 등록한다. App의 모델 id와 새로운 모델 경로를 등록한다.
         등록할 만큼 호출한다.
 
         Args:
             model_id (UUID): 교체할 모델의 UUID
             new_model_path (Path): 새로운 모델 파일 경로
 
         """
         self.convert_list[model_id] = new_model_path
 
-    def convert_models(self, print_output: bool) -> None:
-        """ 모델 변화
+    def convert_models(self, print_output: bool, using_thread: bool = False,
+                        allow_multiple_containers: bool = False,
+                        thread_handler: ConvertThreadHandler = None) -> ConvertThreadHandler:
+        """모델 변화
 
         사용자가 등록한 모델들을 변환한다.
 
         Args:
             print_output (bool): 변환 과정을 출력 여부
 
         Raises:
             AppManager
             MakerManager
 
         """
+        replace_remove_data = []
+
         for id, file_path in self.convert_list.items():
             model_info = self.app_manager.find_model_info_by_id(id)
 
             if not model_info:
                 return
 
             onnx_config = model_info.to_onnx_config()
 
-            engine_file_path = self.workspace.joinpath(
-                model_info.engine_file_name)
+            engine_file_path = self.workspace.joinpath(f"{uuid4()}_{model_info.engine_file_name}")
 
-            self.maker_manager.convert_onnx_to_engine_at_local(input=file_path, output=engine_file_path,
-                                                               convert_config=onnx_config,
-                                                               print_output=print_output)
+            thread_handler = self.maker_manager.convert_onnx_to_engine_at_local(
+                input=file_path,
+                output=engine_file_path,
+                convert_config=onnx_config,
+                print_output=print_output,
+                using_thread=using_thread,
+                allow_multiple_containers=allow_multiple_containers,
+                thread_handler=thread_handler
+            )
 
-            self.app_manager.replace_model(id, engine_file_path)
+            replace_remove_data.append([id, engine_file_path])
 
-            # remove converted files
-            os.remove(engine_file_path)
+        return thread_handler, replace_remove_data
 
     def package_app(self) -> None:
-        """ 새로운 App 생성
-        """
+        """새로운 App 생성"""
         self.app_manager.package(self.final_app_path)
```

### Comparing `waffle_box-0.1.0/waffle_box/pull_service.py` & `waffle_box-0.2.0/waffle_box/pull_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from pathlib import Path
+
 from maker_manager import MakerManager
 
-from pathlib import Path
 
 class PullService:
-    """ Waffle Maker 이미지 설치
+    """Waffle Maker 이미지 설치
 
     Target Autocare-D 버전에 맞춰 Waffle Maker 이미지를 설치한다.
 
     실행 순서:
         1. is_local_maker_installed: Waffle Maker가 local pc에 설치되어 있는지 확인한다.
         2. (Optional) set_login_info: 필요하다면 docker hub에 로그인할 정보를 설정한다.
         3. pull_image_to_local: 이미지를 로컬 pc에 다운로드 한다.
@@ -27,44 +28,44 @@
             dx_target_version (str): 타겟 Autocare-D 버전
 
         Raises:
             MakerManagerException
 
         """
         # Docker Hub
-        self.dh_id: str = ''
-        self.dh_pw: str = ''
+        self.dh_id: str = ""
+        self.dh_pw: str = ""
 
         # TODO: make image tag converter
-        self.img_tag = 'snuailab/trt:8.5.2.2'
+        self.img_tag = "snuailab/trt:8.5.2.2"
 
         self.maker_manager = MakerManager(self.img_tag, gpu_num=0, workspace=workspace)
 
     def is_local_maker_installed(self) -> bool:
-        """ Waffle Maker 이미지가 로컬 pc에 설치되어 있는지 확인한다.
+        """Waffle Maker 이미지가 로컬 pc에 설치되어 있는지 확인한다.
 
         Returns:
             True: 설치되어 있음
             False: 설치되어 있지 않음
         """
         return self.maker_manager.check_image_exist_at_local()
 
     def set_login_info(self, id: str, pw: str) -> None:
-        """ 로그인 정보 입력
+        """로그인 정보 입력
 
         Args:
             id (str): docker hub id
             pw (str): docker hub password
 
         """
         self.dh_id = id
         self.dh_pw = pw
 
     def pull_image_to_local(self, print_output: bool) -> None:
-        """ Waffle Maker 이미지를 로컬 pc에 설치
+        """Waffle Maker 이미지를 로컬 pc에 설치
 
         Args:
             print_output (bool): 설치 과정 출력 여부
 
         Raises:
             MakerManagerException
```

### Comparing `waffle_box-0.1.0/waffle_box_exception/waffle_box_exception.py` & `waffle_box-0.2.0/waffle_box_exception/waffle_box_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from enum import Enum
 
 
 class ExceptionCode(Enum):
-    """ Waffle Box에서 생성하는 예외 리스트
+    """Waffle Box에서 생성하는 예외 리스트
 
     Waffle Box에서 생성하는 예외 리스트.
 
     100번대:
         Maker Manager에서 발생한 예외
-    200번대: 
+    200번대:
         App Manager에서 발생한 예외
     300번대:
         service에서 발생한 예외
 
     """
 
     ### Maker Manager ###
-    DOCKER_EXCEPTION = (100, 'DOCKER_EXCEPTION')
-    DOCKER_IMAGE_EXCEPTION = (101, 'DOCKER_IMAGE_EXCEPTION')
-    DOCKER_RUN_EXCEPTION = (102, 'DOCKER_RUN_EXCEPTION')
-    MODEL_IO_EXCEPTION = (103, 'IO_EXCEPTION')
-    MODEL_CONVERT_EXCEPTION = (104, 'MODEL_CONVERT_EXCEPTION')
+    DOCKER_EXCEPTION = (100, "DOCKER_EXCEPTION")
+    DOCKER_IMAGE_EXCEPTION = (101, "DOCKER_IMAGE_EXCEPTION")
+    DOCKER_RUN_EXCEPTION = (102, "DOCKER_RUN_EXCEPTION")
+    MODEL_IO_EXCEPTION = (103, "IO_EXCEPTION")
+    MODEL_CONVERT_EXCEPTION = (104, "MODEL_CONVERT_EXCEPTION")
 
     ### App Manager ###
-    APP_STRUCTURE_EXCEPTION = (200, 'APP_STRUCTURE_EXCEPTION')
-    APP_NO_SUCH_FILE = (201, 'APP_NO_SUCH_FILE')
-    APP_FILE_ALREADY_EXIST = (202, 'APP_FILE_ALREADY_EXIST')
-    APP_CONFIG_ERROR = (203, 'APP_CONFIG_ERROR')
+    APP_STRUCTURE_EXCEPTION = (200, "APP_STRUCTURE_EXCEPTION")
+    APP_NO_SUCH_FILE = (201, "APP_NO_SUCH_FILE")
+    APP_FILE_ALREADY_EXIST = (202, "APP_FILE_ALREADY_EXIST")
+    APP_CONFIG_ERROR = (203, "APP_CONFIG_ERROR")
 
     ### Service ###
-    INVALID_ARGUMENT = (300, 'INVALID_ARGUMENT')
-
+    INVALID_ARGUMENT = (300, "INVALID_ARGUMENT")
 
     def __init__(self, code, desc) -> None:
         super().__init__()
 
         self._code: int = code
         self._desc: str = desc
 
@@ -51,12 +50,12 @@
     def __init__(self, msg: str, code: ExceptionCode) -> None:
         super().__init__(msg)
 
         self._msg = msg
         self._code = code
 
     def __str__(self) -> str:
-        return f'[{self._code.desc}]: {self._msg}'
+        return f"[{self._code.desc}]: {self._msg}"
 
     @property
     def code(self) -> int:
         return self._code.code
```

