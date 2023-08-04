# Comparing `tmp/artigraph-0.0.4.tar.gz` & `tmp/artigraph-0.0.5.tar.gz`

## Comparing `artigraph-0.0.4.tar` & `artigraph-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,54 @@
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 artigraph-0.0.4/Untitled.ipynb
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/__init__.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/db.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/py.typed
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/__init__.py
--rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/artifact.py
--rw-r--r--   0        0        0    12490 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/artifact_model.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/node.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/api/run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/__init__.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/artifact.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/base.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/node.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/orm/run.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/__init__.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/core.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/datetime.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/json.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/numpy.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/pandas.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/polars.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/serializer/pyarrow.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/__init__.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/aws.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/core.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 artigraph-0.0.4/src/artigraph/storage/file.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_db.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_storage.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/__init__.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_artifact.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_artifact_model.py
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_node.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_api/test_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_core.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_json.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_numpy.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_pandas.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_polars.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 artigraph-0.0.4/tests/test_serializer/test_pyarrow.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.4/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 artigraph-0.0.4/README.md
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 artigraph-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8369 2020-02-02 00:00:00.000000 artigraph-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 artigraph-0.0.5/_temp.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 artigraph-0.0.5/mkdocs.yml
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/index.md
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/serializers.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/storage.md
+-rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/usage.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/__init__.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/db.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/py.typed
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/__init__.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/artifact.py
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/artifact_model.py
+-rw-r--r--   0        0        0     7317 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/node.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/__init__.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/artifact.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/base.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/node.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/span.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/__init__.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/core.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/datetime.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/json.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/numpy.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/pandas.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/polars.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/pyarrow.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/__init__.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/aws.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/core.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/file.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_db.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_storage.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_artifact.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_artifact_model.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_node.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_core.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_json.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_numpy.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_pandas.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_polars.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_pyarrow.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 artigraph-0.0.5/README.md
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 artigraph-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 artigraph-0.0.5/PKG-INFO
```

### Comparing `artigraph-0.0.4/src/artigraph/db.py` & `artigraph-0.0.5/src/artigraph/db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 from contextlib import asynccontextmanager, contextmanager
 from contextvars import ContextVar
 from typing import Any, AsyncIterator, Callable, Iterator, TypeVar
 
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, async_sessionmaker
+from sqlalchemy.ext.asyncio import (
+    AsyncEngine,
+    AsyncSession,
+    async_sessionmaker,
+    create_async_engine,
+)
+from typing_extensions import ParamSpec
+
+from artigraph.orm.base import Base
 
 E = TypeVar("E", bound=AsyncEngine)
+P = ParamSpec("P")
+R = TypeVar("R")
 
+_CREATE_TABLES: ContextVar[bool] = ContextVar("CREATE_TABLES", default=False)
 _CURRENT_ENGINE: ContextVar[AsyncEngine] = ContextVar("CURRENT_ASYNC_ENGINE")
 _CURRENT_SESSION: ContextVar[AsyncSession] = ContextVar("CURRENT_ASYNC_SESSION")
 
 
 @contextmanager
-def engine_context(engine: E) -> Iterator[E]:
+def engine_context(
+    engine: AsyncEngine | str,
+    *,
+    create_tables: bool = False,
+) -> Iterator[AsyncEngine]:
     """Define which engine to use in the context."""
-    reset = set_engine(engine)
+    if isinstance(engine, str):
+        engine = create_async_engine(engine)
+    reset = set_engine(engine, create_tables=create_tables)
     try:
         yield engine
     finally:
         reset()
 
 
 @asynccontextmanager
 async def session_context(**kwargs: Any) -> AsyncIterator[AsyncSession]:
     """Define which session to use in the context."""
-    async with async_sessionmaker(get_engine(), **kwargs)() as session:
+    async with async_sessionmaker(await get_engine(), **kwargs)() as session:
         reset = set_session(session)
         try:
             yield session
         finally:
             reset()
 
 
@@ -38,36 +55,47 @@
         session = get_session()
     except LookupError:
         pass
     else:
         yield session
         return
 
-    async with AsyncSession(get_engine()) as session:
+    async with AsyncSession(await get_engine()) as session:
         try:
             yield session
         except Exception:
             await session.rollback()
             raise
 
 
-def set_engine(engine: AsyncEngine) -> Callable[[], None]:
-    """Set the current engine."""
-    var = _CURRENT_ENGINE
-    token = var.set(engine)
-    return lambda: var.reset(token)
+def set_engine(engine: AsyncEngine | str, *, create_tables: bool = False) -> Callable[[], None]:
+    """Set the current engine and whether to try creating tables if they don't exist."""
+    if isinstance(engine, str):
+        engine = create_async_engine(engine)
+    current_engine_token = _CURRENT_ENGINE.set(engine)
+    create_tables_token = _CREATE_TABLES.set(create_tables)
+
+    def reset() -> None:
+        _CURRENT_ENGINE.reset(current_engine_token)
+        _CREATE_TABLES.reset(create_tables_token)
+
+    return reset
 
 
-def get_engine() -> AsyncEngine:
+async def get_engine() -> AsyncEngine:
     """Get the current engine."""
     try:
-        return _CURRENT_ENGINE.get()
+        engine = _CURRENT_ENGINE.get()
     except LookupError:  # nocov
         msg = "No current asynchronous engine"
         raise LookupError(msg) from None
+    if _CREATE_TABLES.get():
+        async with engine.begin() as conn:
+            await conn.run_sync(Base.metadata.create_all)
+    return engine
 
 
 def set_session(session: AsyncSession) -> Callable[[], None]:
     """Set the current session."""
     var = _CURRENT_SESSION
     token = var.set(session)
     return lambda: var.reset(token)
```

### Comparing `artigraph-0.0.4/src/artigraph/utils.py` & `artigraph-0.0.5/src/artigraph/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,19 +8,25 @@
 F = TypeVar("F", bound=Callable[..., Any])
 P = ParamSpec("P")
 R = TypeVar("R")
 
 SLUG_REPLACE_PATTERN = re.compile(r"[^a-z0-9]+")
 """A pattern for replacing non-alphanumeric characters in slugs"""
 
-UNDEFINED = cast(Any, type("UNDEFINED", (), {"__repr__": lambda _: "UNDEFINED"}))()
+
+def create_sentinel(name: str) -> Any:
+    """Create a sentinel object."""
+    return cast(Any, type(name, (), {"__repr__": lambda _: name}))()
+
+
+UNDEFINED = create_sentinel("UNDEFINED")
 """A sentinel for undefined values"""
 
 
 def slugify(string: str) -> str:
     """Convert a string to a slug."""
     return SLUG_REPLACE_PATTERN.sub("-", string.lower()).strip("-")
 
 
 async def run_in_thread(func: Callable[P, R], /, *args: P.args, **kwargs: P.kwargs) -> R:
-    """Run a sync function in a thread."""
+    """Span a sync function in a thread."""
     return await to_thread.run_sync(partial(func, *args, **kwargs))  # type: ignore
```

### Comparing `artigraph-0.0.4/src/artigraph/api/artifact.py` & `artigraph-0.0.5/src/artigraph/api/artifact.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     """Save the artifact to the database."""
     result = await create_artifacts([(artifact, value)])
     return result[0]
 
 
 async def read_artifact_by_id(artifact_id: int) -> QualifiedArtifact:
     """Load the artifact from the database."""
-    stmt = select(Node.node_type).where(Node.node_id == artifact_id)
+    cmd = select(Node.node_type).where(Node.node_id == artifact_id)
     async with current_session() as session:
-        result = await session.execute(stmt)
+        result = await session.execute(cmd)
         artifact_type = _get_artifact_type_by_name(result.scalar_one())
-        stmt = select(artifact_type).where(artifact_type.node_id == artifact_id)
-        result = await session.execute(stmt)
+        cmd = select(artifact_type).where(artifact_type.node_id == artifact_id)
+        result = await session.execute(cmd)
         artifact = result.scalar_one()
 
     serializer = get_serialize_by_name(artifact.artifact_serializer)
     if isinstance(artifact, RemoteArtifact):
         storage = get_storage_by_name(artifact.remote_artifact_storage)
         value = serializer.deserialize(await storage.read(artifact.remote_artifact_location))
     elif isinstance(artifact, DatabaseArtifact):
@@ -88,16 +88,23 @@
     for artifact, location in zip(remote_artifacts, storage_locations):
         artifact.remote_artifact_location = location
 
     # Save records in the database
     async with current_session() as session:
         session.add_all(database_artifacts + remote_artifacts)
         await session.commit()
-        await asyncio.gather(*[session.refresh(a, ["node_id"]) for a, _ in qualified_artifacts])
-        return [a.node_id for a, _ in qualified_artifacts]
+
+        # We can't do this in asyncio.gather() because of issues with concurrent connections:
+        # https://docs.sqlalchemy.org/en/20/errors.html#illegalstatechangeerror-and-concurrency-exceptions
+        artifact_ids: list[int] = []
+        for a, _ in qualified_artifacts:
+            await session.refresh(a, ["node_id"])
+            artifact_ids.append(a.node_id)
+
+        return artifact_ids
 
 
 async def delete_artifacts(artifacts: Sequence[BaseArtifact]) -> None:
     """Delete the artifacts from the database."""
     remote_artifacts: list[RemoteArtifact] = []
     for artifact in artifacts:
         if isinstance(artifact, RemoteArtifact):
```

### Comparing `artigraph-0.0.4/src/artigraph/api/artifact_model.py` & `artigraph-0.0.5/src/artigraph/api/artifact_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,47 +67,55 @@
     """The serializer for the artifact model field."""
 
     storage: Storage | None
     """The storage for the artifact model field."""
 
 
 @dataclass_transform(field_specifiers=(artifact_field,))
-@dataclass
+@dataclass(frozen=True)
 class ArtifactModel:
     """A collection of artifacts that are saved together."""
 
     model_version: ClassVar[int] = 1
     """The version of the artifact model."""
 
     model_config: ClassVar[ArtifactModelConfig] = ArtifactModelConfig()
     """The configuration for the artifact model."""
 
+    node_id: int | None = field(init=False, default=None, compare=False)
+    """The ID of the node for this artifact model.
+
+    This is populated when the artifact model is saved to or loaded from the database.
+    """
+
     def __init_subclass__(
         cls,
         *,
         version: int,
         config: "ArtifactModelConfig | None" = None,
+        **kwargs: Any,
     ) -> None:
         if cls.__name__ in ARTIFACT_MODEL_TYPES_BY_NAME:
             msg = f"Artifact model named {cls.__name__!r} already exists"
             raise RuntimeError(msg)
         ARTIFACT_MODEL_TYPES_BY_NAME[cls.__name__] = cls
         cls.model_version = version
         cls.model_config = config or ArtifactModelConfig()
+        super().__init_subclass__(**kwargs)
 
     @classmethod
     def migrate(
         cls,
         version: int,  # noqa: ARG003
         data: dict[str, Any],
-    ) -> dict[str, Any]:
+    ) -> Self:
         """Migrate the artifact model to a new version."""
-        return data
+        return cls(**data)
 
-    async def save(self, label: str, parent_id: int | None = None) -> int:
+    async def create(self, label: str, parent_id: int | None = None) -> int:
         """Save the artifact model to the database."""
         parent_node = None if parent_id is None else await read_node(parent_id)
 
         models_by_path = _get_model_paths(self)
         nodes_by_path = {
             path: model._model_node(_get_model_label_from_path(path))
             for path, model in models_by_path.items()
@@ -132,18 +140,20 @@
                 [
                     fn
                     for path, model in models_by_path.items()
                     for fn in model._model_field_artifacts(nodes_by_path[path])
                 ]
             )
 
+        object.__setattr__(self, "node_id", root_node.node_id)
+
         return root_node.node_id
 
     @classmethod  # type: ignore
-    async def load(cls, node_id: int) -> Self:
+    async def read(cls, node_id: int) -> Self:
         """Load the artifact model from the database."""
         root_qaul_artifact = await read_artifact_by_id(node_id)
         if not is_qualified_artifact_model(root_qaul_artifact):
             msg = f"Node {node_id} is not an artifact model."
             raise ValueError(msg)
         root_node, root_metadata = root_qaul_artifact
         cls = get_artifact_model_type_by_name(root_metadata["model_type"])
@@ -257,20 +267,20 @@
                     artifacts_by_parent_id,
                 )
             else:
                 node, value = qual_artifact
                 kwargs[node.artifact_label] = value
 
         if model_metadata["model_version"] != cls.model_version:
-            kwargs = cls.migrate(model_metadata["model_version"], kwargs)
-
-        return cls(**kwargs)
+            return cls.migrate(model_metadata["model_version"], kwargs)
+        else:
+            return cls(**kwargs)
 
 
-class ArtifactMapping(ArtifactModel, Mapping[str, A], version=1):
+class ArtifactMapping(ArtifactModel, Mapping[str, A], version=1):  # type: ignore
     """A mapping whose values are other artifact models"""
 
     def __init__(self, *args: dict[str, A], **kwargs: A):
         self._data = dict(*args, **kwargs)
 
     def _model_data(self) -> dict[str, Any]:
         return self._data
@@ -284,22 +294,22 @@
     def __iter__(self) -> Iterator[str]:
         return iter(self._data)
 
     def __len__(self) -> int:
         return len(self._data)
 
 
-class ArtifactSequence(Sequence[A], ArtifactModel, version=1):
+class ArtifactSequence(Sequence[A], ArtifactModel, version=1):  # type: ignore
     """A sequence whose values are other artifact models"""
 
     def __init__(self, *args: Sequence[A], **kwargs: A) -> None:
         self._data = {str(i): v for i, v in enumerate(tuple(*args))}
         self._data.update(kwargs)
 
-    def _model_data(self):
+    def _model_data(self) -> dict[str, Any]:
         return self._data
 
     def _model_field_configs(self) -> dict[str, ArtifactFieldConfig]:
         return {}
 
     def __getitem__(self, key: int) -> A:
         return self._data[str(key)]
```

### Comparing `artigraph-0.0.4/src/artigraph/api/node.py` & `artigraph-0.0.5/src/artigraph/api/node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from collections.abc import Collection
 from dataclasses import fields
 from typing import Any, Literal, Sequence, TypeGuard, TypeVar, overload
 
 from sqlalchemy import Row, delete, join, select
 from sqlalchemy.orm import aliased
 
@@ -46,45 +45,48 @@
     ...
 
 
 async def read_node(
     node_id: int, node_type: type[N] = Node, *, allow_none: bool = False
 ) -> N | None:
     """Read a node by its ID."""
-    stmt = select(node_type).where(node_type.node_id == node_id)
+    cmd = select(node_type).where(node_type.node_id == node_id)
     async with current_session() as session:
-        result = await session.execute(stmt)
+        result = await session.execute(cmd)
         return result.scalar_one_or_none() if allow_none else result.scalar_one()
 
 
 async def node_exists(node_id: int, node_type: type[Node] = Node) -> bool:
     """Check if a node exists."""
-    stmt = select(node_type.node_id).where(node_type.node_id == node_id)
+    cmd = select(node_type.node_id).where(node_type.node_id == node_id)
     async with current_session() as session:
-        result = await session.execute(stmt)
+        result = await session.execute(cmd)
         return bool(result.one_or_none())
 
 
 async def delete_nodes(node_ids: Sequence[int]) -> None:
     """Delete nodes."""
     async with current_session() as session:
-        stmt = delete(Node).where(Node.node_id.in_(node_ids))
-        await session.execute(stmt)
+        cmd = delete(Node).where(Node.node_id.in_(node_ids))
+        await session.execute(cmd)
         await session.commit()
 
 
 async def create_nodes(
     nodes: Collection[Node], refresh_attributes: Sequence[str]
 ) -> Collection[Node]:
     """Create nodes and, if given, refresh their attributes."""
     async with current_session() as session:
         session.add_all(nodes)
         await session.commit()
         if refresh_attributes:
-            await asyncio.gather(*[session.refresh(n, refresh_attributes) for n in nodes])
+            # We can't do this in asyncio.gather() because of issues with concurrent connections:
+            # https://docs.sqlalchemy.org/en/20/errors.html#illegalstatechangeerror-and-concurrency-exceptions
+            for n in nodes:
+                await session.refresh(n, refresh_attributes)
     return nodes
 
 
 async def create_parent_child_relationships(
     parent_child_pairs: Sequence[tuple[Node | None, Node]]
 ) -> None:
     """Create parent-to-child links between nodes."""
@@ -93,24 +95,35 @@
             child.node_parent_id = None if parent is None else parent.node_id
             session.add(child)
         await session.commit()
 
 
 async def read_children(node_id: int, *node_types: type[N]) -> Sequence[N]:
     """Read the direct children of a node."""
-    stmt = select(Node).where(Node.node_parent_id == node_id)
+    cmd = select(Node).where(Node.node_parent_id == node_id)
     if node_types:
-        stmt = stmt.where(Node.node_type.in_([n.polymorphic_identity for n in node_types]))
+        cmd = cmd.where(Node.node_type.in_([n.polymorphic_identity for n in node_types]))
     async with current_session() as session:
-        result = await session.execute(stmt)
+        result = await session.execute(cmd)
         children = result.scalars().all()
     # we know we've filtered appropriately, so we can ignore the type check
     return children  # type: ignore
 
 
+async def read_parent(node_id: int, node_type: type[N] = Node) -> N | None:
+    """Read the direct parent of a node."""
+    async with current_session() as session:
+        node_cmd = select(node_type).where(node_type.node_id == node_id)
+        result = await session.execute(node_cmd)
+        node = result.scalar_one()
+        parent_cmd = select(node_type).where(node_type.node_id == node.node_parent_id)
+        result = await session.execute(parent_cmd)
+        return result.scalar_one_or_none()
+
+
 async def read_descendants(node_id: int, *node_types: type[N]) -> Sequence[N]:
     """Read all descendants of this node."""
 
     # Create a CTE to get the descendants recursively
     node_cte = (
         select(Node.node_id.label("descendant_id"), Node.node_parent_id)
         .where(Node.node_id == node_id)
@@ -122,33 +135,71 @@
     node_cte = node_cte.union_all(
         select(parent_node.node_id, parent_node.node_parent_id).where(
             parent_node.node_parent_id == node_cte.c.descendant_id
         )
     )
 
     # Join the CTE with the actual Node table to get the descendants
-    descendants_query = (
+    descendants_cmd = (
         select(Node.__table__)
         .select_from(join(Node, node_cte, Node.node_id == node_cte.c.descendant_id))
         .where(node_cte.c.descendant_id != node_id)  # Exclude the root node itself
     )
 
     if node_types:
-        descendants_query = descendants_query.where(
+        descendants_cmd = descendants_cmd.where(
             Node.node_type.in_([n.polymorphic_identity for n in node_types])
         )
 
     async with current_session() as session:
-        result = await session.execute(descendants_query)
+        result = await session.execute(descendants_cmd)
         descendants = result.all()
 
-    return _nodes_from_rows(descendants)
+    return load_nodes_from_rows(descendants)
+
+
+async def read_ancestors(node_id: int, *node_types: type[N]) -> Sequence[N]:
+    """Read all ancestors of this node."""
+
+    # Create a CTE to get the ancestors recursively
+    node_cte = (
+        select(Node.node_id.label("ancestor_id"), Node.node_parent_id)
+        .where(Node.node_id == node_id)
+        .cte(name="ancestors", recursive=True)
+    )
+
+    # Recursive case: select the parents of the current nodes
+    parent_node = aliased(Node)
+    node_cte = node_cte.union_all(
+        select(parent_node.node_id, parent_node.node_parent_id).where(
+            parent_node.node_id == node_cte.c.node_parent_id
+        )
+    )
+
+    # Join the CTE with the actual Node table to get the ancestors
+    ancestors_cmd = (
+        select(Node.__table__)
+        .select_from(join(Node, node_cte, Node.node_id == node_cte.c.ancestor_id))
+        .where(node_cte.c.ancestor_id != node_id)  # Exclude the root node itself
+    )
+
+    if node_types:
+        ancestors_cmd = ancestors_cmd.where(
+            Node.node_type.in_([n.polymorphic_identity for n in node_types])
+        )
+
+    async with current_session() as session:
+        result = await session.execute(ancestors_cmd)
+        ancestors = result.all()
+
+    return load_nodes_from_rows(ancestors)
 
 
-def _nodes_from_rows(rows: Sequence[Row[Any]]) -> Sequence[Any]:
+def load_nodes_from_rows(rows: Sequence[Row[Any]]) -> Sequence[Any]:
+    """Load the appropriate Node instances given a sequence of SQLAlchemy rows."""
     nodes: list[Any] = []
     for r in rows:
         node_type = Node.polymorphic_identity_mapping[r.node_type]
         kwargs: dict[str, Any] = {}
         attrs: dict[str, Any] = {}
         for f in fields(node_type):
             if f.init:
```

### Comparing `artigraph-0.0.4/src/artigraph/orm/artifact.py` & `artigraph-0.0.5/src/artigraph/orm/artifact.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/orm/node.py` & `artigraph-0.0.5/src/artigraph/orm/node.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,21 +20,23 @@
             table_args = cls.__table_args__
             for parent_cls in cls.mro():  # nocov (this)
                 if hasattr(parent_cls, "__tablename__"):
                     cls.__table_args__ += table_args
                     break
             del cls.__table_args__
 
-        if "polymorphic_identity" in cls.__dict__ or "polymorphic_identity" in cls.__mapper_args__:
-            if cls.polymorphic_identity != cls.__mapper_args__["polymorphic_identity"]:  # nocov
-                msg = (
-                    f"polymorphic_identity {cls.polymorphic_identity!r} doesn't match "
-                    f"__mapper_args__ {cls.__mapper_args__['polymorphic_identity']!r}"
-                )
-                raise ValueError(msg)
+        if "polymorphic_identity" in cls.__dict__:
+            cls.__mapper_args__ = {
+                **cls.__mapper_args__,
+                "polymorphic_identity": cls.polymorphic_identity,
+            }
+
+        if "__mapper_args__" in cls.__dict__:
+            if "polymorphic_on" in cls.__mapper_args__:
+                cls.polymorphic_identity = cls.__mapper_args__["polymorphic_on"]
 
         Node.polymorphic_identity_mapping[cls.polymorphic_identity] = cls
 
         super().__init_subclass__(**kwargs)
 
     polymorphic_identity: ClassVar[str] = "node"
     """The type of the node - should be overridden by subclasses and passed to mapper args."""
```

### Comparing `artigraph-0.0.4/src/artigraph/serializer/core.py` & `artigraph-0.0.5/src/artigraph/serializer/core.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/serializer/datetime.py` & `artigraph-0.0.5/src/artigraph/serializer/datetime.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/serializer/json.py` & `artigraph-0.0.5/src/artigraph/serializer/json.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/serializer/numpy.py` & `artigraph-0.0.5/src/artigraph/serializer/numpy.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/serializer/pandas.py` & `artigraph-0.0.5/src/artigraph/serializer/pandas.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/serializer/polars.py` & `artigraph-0.0.5/src/artigraph/serializer/polars.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/serializer/pyarrow.py` & `artigraph-0.0.5/src/artigraph/serializer/pyarrow.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/storage/aws.py` & `artigraph-0.0.5/src/artigraph/storage/aws.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/src/artigraph/storage/core.py` & `artigraph-0.0.5/src/artigraph/storage/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class Storage(ABC):
     """A storage backend for artifacts."""
 
     name: str
     """A globally unique name for this storage.
 
-    This will typically be of the form "library_name.StorageName". You should avoid
+    This will typically be of the form "library_name-storage_name". You should avoid
     using dynamic values like `__name__` or `__qualname__` as these may change between
     versions of the library or if you move the class to a different module.
 
     The storage name will be used to recover this class when loading data from records.
     It must not change between versions of the library. If you need to change the name,
     you should create and register a subclass with the new name and deprecate the old
     one.
```

### Comparing `artigraph-0.0.4/src/artigraph/storage/file.py` & `artigraph-0.0.5/src/artigraph/storage/file.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/tests/test_db.py` & `artigraph-0.0.5/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/tests/test_storage.py` & `artigraph-0.0.5/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/tests/test_api/test_artifact.py` & `artigraph-0.0.5/tests/test_api/test_artifact.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/tests/test_api/test_artifact_model.py` & `artigraph-0.0.5/tests/test_api/test_artifact_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,28 @@
     ArtifactSequence,
     artifact_field,
 )
 from artigraph.serializer.json import json_serializer
 from artigraph.storage.file import temp_file_storage
 
 
-@dataclass
+@dataclass(frozen=True)
 class SimpleArtifactModel(ArtifactModel, version=1):
     """A simple artifact model that stores a few basic artifact."""
 
     some_value: str
     remote_value: Any = artifact_field(serializer=json_serializer, storage=temp_file_storage)
     inner_model: "None | SimpleArtifactModel" = None
 
 
 async def test_save_load_simple_artifact_model():
     """Test saving and loading a simple artifact model."""
     artifact = SimpleArtifactModel(some_value="test-value", remote_value={"some": "data"})
-    artifact_id = await artifact.save(None)
-    loaded_artifact = await SimpleArtifactModel.load(artifact_id)
+    artifact_id = await artifact.create(None)
+    loaded_artifact = await SimpleArtifactModel.read(artifact_id)
     assert loaded_artifact == artifact
 
 
 async def test_save_load_simple_artifact_model_with_inner_model():
     """Test saving and loading a simple artifact model with an inner model."""
     inner_inner_artifact = SimpleArtifactModel(
         some_value="inner-inner-value",
@@ -41,20 +41,20 @@
     )
     artifact = SimpleArtifactModel(
         some_value="test-value",
         remote_value={"some": "data"},
         inner_model=inner_artifact,
     )
 
-    artifact_id = await artifact.save(None)
-    loaded_artifact = await SimpleArtifactModel.load(artifact_id)
+    artifact_id = await artifact.create(None)
+    loaded_artifact = await SimpleArtifactModel.read(artifact_id)
     assert loaded_artifact == artifact
 
 
-@dataclass
+@dataclass(frozen=True)
 class ComplexArtifactModel(ArtifactModel, version=1):
     """A complex artifact model that stores a few basic artifact."""
 
     simple: SimpleArtifactModel
     mapping: ArtifactMapping["ComplexArtifactModel"] = field(default_factory=dict)
     sequence: ArtifactSequence["ComplexArtifactModel"] = field(default_factory=dict)
 
@@ -78,10 +78,10 @@
                     simple=simple,
                     mapping=ArtifactMapping(key3=ComplexArtifactModel(simple=simple)),
                 ),
             ]
         ),
     )
 
-    artifact_id = await artifact.save(None)
-    loaded_artifact = await ComplexArtifactModel.load(artifact_id)
+    artifact_id = await artifact.create(None)
+    loaded_artifact = await ComplexArtifactModel.read(artifact_id)
     assert loaded_artifact == artifact
```

### Comparing `artigraph-0.0.4/tests/test_api/test_node.py` & `artigraph-0.0.5/tests/test_api/test_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 
 
 async def test_read_recursive_children_with_node_type():
     """Test reading the recursive children of a node with node types."""
     graph = await create_graph()
     root = graph.get_root()
     children = await read_descendants(root.node_id, ThingOne)
-    all_run_ids = {n.node_id for n in graph.get_all_nodes() if isinstance(n, ThingOne)}
-    expected_descendant_ids = all_run_ids - {root.node_id}
+    all_span_ids = {n.node_id for n in graph.get_all_nodes() if isinstance(n, ThingOne)}
+    expected_descendant_ids = all_span_ids - {root.node_id}
     assert {n.node_id for n in children} == expected_descendant_ids
 
 
 async def test_create_parent_child_relationships():
     """Test creating parent-to-child relationships between nodes."""
     async with session_context(expire_on_commit=False):
         grandparent = await create_node()
```

### Comparing `artigraph-0.0.4/tests/test_serializer/test_core.py` & `artigraph-0.0.5/tests/test_serializer/test_core.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/tests/test_serializer/test_numpy.py` & `artigraph-0.0.5/tests/test_serializer/test_numpy.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/tests/test_serializer/test_pyarrow.py` & `artigraph-0.0.5/tests/test_serializer/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/.gitignore` & `artigraph-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/LICENSE.txt` & `artigraph-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.4/pyproject.toml` & `artigraph-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "artigraph"
 dynamic = ["version"]
-description = "A library for interrelated graphs of artifacts and the runs that produce them."
+description = "A library for interrelated graphs of artifacts."
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
 keywords = []
 authors = [{ name = "U.N. Owen", email = "void@some.where" }]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -27,17 +27,17 @@
 aws = ["boto3>=1,<2"]
 pandas = ["pandas>=2,<3", "artigraph[pyarrow]"]
 numpy = ["numpy>=1,<2", "pandas>=2,<3", "artigraph[pyarrow]"]
 polars = ["polars<1", "artigraph[pyarrow]"]
 pyarrow = ["pyarrow>=12,<13"]
 
 [project.urls]
-Documentation = "https://github.com/unknown/artigraph#readme"
-Issues = "https://github.com/unknown/artigraph/issues"
-Source = "https://github.com/unknown/artigraph"
+Documentation = "https://github.com/rmorshea/artigraph#readme"
+Issues = "https://github.com/rmorshea/artigraph/issues"
+Source = "https://github.com/rmorshea/artigraph"
 
 # --- Hatch ----------------------------------------------------------------------------------------
 
 [tool.hatch.version]
 path = "src/artigraph/__init__.py"
 
 [tool.hatch.envs.default]
@@ -47,14 +47,16 @@
   "pytest-asyncio",
   "black>=23.1.0",
   "pyright>=1",
   "ruff>=0.0.243",
   "aiosqlite>=0.19,<1",
   "greenlet>=2,<3",
   "moto>=4,<5",
+  "mkdocs>=1.5,<2",
+  "mkdocs-material>=9,<10",
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = ["cov-test", "cov-report"]
 cov-report = ["- coverage combine", "coverage report"]
 cov-test = "coverage run -m pytest {args:tests}"
 format = ["black {args:.}", "ruff --fix {args:.}", "style"]
```

