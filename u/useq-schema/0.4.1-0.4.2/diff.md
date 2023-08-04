# Comparing `tmp/useq_schema-0.4.1.tar.gz` & `tmp/useq_schema-0.4.2.tar.gz`

## Comparing `useq_schema-0.4.1.tar` & `useq_schema-0.4.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 useq_schema-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/images/favicon.ico
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/axes.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/event.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/hardware_autofocus.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.4.1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_actions.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_base_model.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_channel.py
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_grid.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_hardware_autofocus.py
--rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_iter_sequence.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_mda_event.py
--rw-r--r--   0        0        0    15776 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_position.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_pydantic_compat.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_time.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_utils.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/py.typed
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 useq_schema-0.4.1/src/useq/pycromanager.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_autofocus.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_grid.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_misc.py
--rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_position_sequence.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_pycromanager.py
--rw-r--r--   0        0        0    13451 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_sequence.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/test_serialization.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/fixtures/mda.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.4.1/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.4.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.4.1/LICENSE
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 useq_schema-0.4.1/README.md
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 useq_schema-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 useq_schema-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 useq_schema-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 useq_schema-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 useq_schema-0.4.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 useq_schema-0.4.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/schema/axes.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/schema/event.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/schema/hardware_autofocus.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.4.2/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_actions.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_base_model.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_channel.py
+-rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_grid.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_hardware_autofocus.py
+-rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_iter_sequence.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    15837 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_position.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_time.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_utils.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/py.typed
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 useq_schema-0.4.2/src/useq/pycromanager.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/test_autofocus.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/test_grid.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/test_misc.py
+-rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/test_position_sequence.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/test_pycromanager.py
+-rw-r--r--   0        0        0    13451 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/test_sequence.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/test_serialization.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.4.2/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.4.2/LICENSE
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 useq_schema-0.4.2/README.md
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 useq_schema-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 useq_schema-0.4.2/PKG-INFO
```

### Comparing `useq_schema-0.4.1/.pre-commit-config.yaml` & `useq_schema-0.4.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -31,10 +31,10 @@
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
           - types-PyYAML
-          - pydantic>=2
-          - pydantic-compat
+          - pydantic >=2
+          - pydantic-compat >=0.0.4
         files: "^src/"
```

### Comparing `useq_schema-0.4.1/mkdocs.yml` & `useq_schema-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/.github/workflows/docs.yml` & `useq_schema-0.4.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/.github/workflows/test_and_deploy.yml` & `useq_schema-0.4.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/docs/index.md` & `useq_schema-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/docs/images/favicon.ico` & `useq_schema-0.4.2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/docs/schema/axes.md` & `useq_schema-0.4.2/docs/schema/axes.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/docs/stylesheets/extra.css` & `useq_schema-0.4.2/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/__init__.py` & `useq_schema-0.4.2/src/useq/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,9 +42,10 @@
     "ZAbsolutePositions",
     "ZRangeAround",
     "ZRelativePositions",
     "ZTopBottom",
 ]
 
 
-MDAEvent.model_rebuild(MDASequence=MDASequence)
-Position.model_rebuild(MDASequence=MDASequence)
+# type ignores because pydantic-compat consumes the kwargs
+MDAEvent.model_rebuild(MDASequence=MDASequence)  # type: ignore  [call-arg]
+Position.model_rebuild(MDASequence=MDASequence)  # type: ignore  [call-arg]
```

### Comparing `useq_schema-0.4.1/src/useq/_actions.py` & `useq_schema-0.4.2/src/useq/_actions.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_base_model.py` & `useq_schema-0.4.2/src/useq/_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,29 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import numpy as np
-from pydantic import BaseModel
-from pydantic_compat import PydanticCompatMixin
+from pydantic_compat import BaseModel
 
 if TYPE_CHECKING:
     from pydantic import ConfigDict
 
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
     IncEx = set[int] | set[str] | dict[int, Any] | dict[str, Any] | None
 
 __all__ = ["UseqModel", "FrozenModel"]
 
 _T = TypeVar("_T", bound="FrozenModel")
 _Y = TypeVar("_Y", bound="UseqModel")
 
 
-class FrozenModel(PydanticCompatMixin, BaseModel):
+class FrozenModel(BaseModel):
     model_config: ClassVar[ConfigDict] = {
         "populate_by_name": True,
         "extra": "ignore",
         "frozen": True,
         "json_encoders": {MappingProxyType: dict},
     }
```

### Comparing `useq_schema-0.4.1/src/useq/_channel.py` & `useq_schema-0.4.2/src/useq/_channel.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_grid.py` & `useq_schema-0.4.2/src/useq/_grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
 import contextlib
 import math
 from enum import Enum
 from functools import partial
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Iterator,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import numpy as np
-from pydantic import ConfigDict, Field
-from pydantic_compat import field_validator
+from pydantic_compat import Field, field_validator
 
 from useq._base_model import FrozenModel
-from useq._pydantic_compat import FROZEN
+
+if TYPE_CHECKING:
+    from pydantic import ConfigDict
 
 
 class RelativeTo(Enum):
     center = "center"
     top_left = "top_left"
 
 
@@ -132,16 +134,16 @@
         should use current height of the FOV based on the current objective and camera.
         Engines MAY override this even if provided.
     """
 
     # Overriding FrozenModel to make fov_width and fov_height mutable.
     model_config: ClassVar[ConfigDict] = {"validate_assignment": True, "frozen": False}
 
-    overlap: Tuple[float, float] = Field((0.0, 0.0), **FROZEN)  # type: ignore
-    mode: OrderMode = Field(OrderMode.row_wise_snake, **FROZEN)  # type: ignore
+    overlap: Tuple[float, float] = Field((0.0, 0.0), frozen=True)
+    mode: OrderMode = Field(OrderMode.row_wise_snake, frozen=True)
     fov_width: Optional[float] = Field(None)
     fov_height: Optional[float] = Field(None)
 
     @field_validator("overlap", mode="before")
     def _validate_overlap(cls, v: Any) -> Tuple[float, float]:
         with contextlib.suppress(TypeError, ValueError):
             v = float(v)
@@ -233,18 +235,18 @@
     bottom : float
         Bottom stage position of the bounding area
     right : float
         Right stage position of the bounding area
     """
 
     # everything but fov_width and fov_height is immutable
-    top: float = Field(..., **FROZEN)  # type: ignore
-    left: float = Field(..., **FROZEN)  # type: ignore
-    bottom: float = Field(..., **FROZEN)  # type: ignore
-    right: float = Field(..., **FROZEN)  # type: ignore
+    top: float = Field(..., frozen=True)
+    left: float = Field(..., frozen=True)
+    bottom: float = Field(..., frozen=True)
+    right: float = Field(..., frozen=True)
 
     def _nrows(self, dy: float) -> int:
         total_height = abs(self.top - self.bottom) + dy
         return math.ceil(total_height / dy)
 
     def _ncolumns(self, dx: float) -> int:
         total_width = abs(self.right - self.left) + dx
@@ -269,17 +271,17 @@
     relative_to : RelativeTo
         Point in the grid to which the coordinates are relative. If "center", the grid
         is centered around the origin. If "top_left", the grid is positioned such that
         the top left corner is at the origin.
     """
 
     # everything but fov_width and fov_height is immutable
-    rows: int = Field(..., **FROZEN)  # type: ignore
-    columns: int = Field(..., **FROZEN)  # type: ignore
-    relative_to: RelativeTo = Field(RelativeTo.center, **FROZEN)  # type: ignore
+    rows: int = Field(..., frozen=True)
+    columns: int = Field(..., frozen=True)
+    relative_to: RelativeTo = Field(RelativeTo.center, frozen=True)
 
     @property
     def is_relative(self) -> bool:
         return True
 
     def _nrows(self, dy: float) -> int:
         return self.rows
```

### Comparing `useq_schema-0.4.1/src/useq/_hardware_autofocus.py` & `useq_schema-0.4.2/src/useq/_hardware_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_iter_sequence.py` & `useq_schema-0.4.2/src/useq/_iter_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_mda_event.py` & `useq_schema-0.4.2/src/useq/_mda_event.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_mda_sequence.py` & `useq_schema-0.4.2/src/useq/_mda_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,15 +325,16 @@
             if isinstance(autofocus_plan, AxesBasedAF):
                 raise ValueError(err)
             for p in stage_positions:
                 if p.sequence is not None and p.sequence.autofocus_plan:
                     raise ValueError(err)
 
     def __str__(self) -> str:
-        return "Multi-Dimensional Acquisition ▶ " + ", ".join(self.sizes)
+        sizes = ", ".join(f"n{k}={v}" for k, v in self.sizes.items() if v)
+        return f"Multi-Dimensional Acquisition with: {sizes}"
 
     @property
     def shape(self) -> Tuple[int, ...]:
         """Return the shape of this sequence.
 
         !!! note
             This doesn't account for jagged arrays, like channels that exclude z
```

### Comparing `useq_schema-0.4.1/src/useq/_position.py` & `useq_schema-0.4.2/src/useq/_position.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_time.py` & `useq_schema-0.4.2/src/useq/_time.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_utils.py` & `useq_schema-0.4.2/src/useq/_utils.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/_z.py` & `useq_schema-0.4.2/src/useq/_z.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/src/useq/pycromanager.py` & `useq_schema-0.4.2/src/useq/pycromanager.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/conftest.py` & `useq_schema-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/test_autofocus.py` & `useq_schema-0.4.2/tests/test_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/test_grid.py` & `useq_schema-0.4.2/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/test_misc.py` & `useq_schema-0.4.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/test_position_sequence.py` & `useq_schema-0.4.2/tests/test_position_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/test_sequence.py` & `useq_schema-0.4.2/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/test_serialization.py` & `useq_schema-0.4.2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/fixtures/mda.json` & `useq_schema-0.4.2/tests/fixtures/mda.json`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/tests/fixtures/mda.yaml` & `useq_schema-0.4.2/tests/fixtures/mda.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/.gitignore` & `useq_schema-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/LICENSE` & `useq_schema-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/README.md` & `useq_schema-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.4.1/pyproject.toml` & `useq_schema-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Software Development",
     "Topic :: System :: Hardware",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic >=1.7", "numpy", "pydantic-compat >=0.0.1"]
+dependencies = ["pydantic >=1.7", "numpy", "pydantic-compat >=0.0.4"]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 yaml = ["PyYAML"]
 test = ["pytest>=6.0", "pytest-cov", "PyYAML"]
 dev = [
```

### Comparing `useq_schema-0.4.1/PKG-INFO` & `useq_schema-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.4.1
+Version: 0.4.2
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
@@ -23,15 +23,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Hardware
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: numpy
-Requires-Dist: pydantic-compat>=0.0.1
+Requires-Dist: pydantic-compat>=0.0.4
 Requires-Dist: pydantic>=1.7
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
```

