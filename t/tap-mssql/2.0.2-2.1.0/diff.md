# Comparing `tmp/tap-mssql-2.0.2.tar.gz` & `tmp/tap_mssql-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mssql-2.0.2.tar", max compression
+gzip compressed data, was "tap_mssql-2.1.0.tar", max compression
```

## Comparing `tap-mssql-2.0.2.tar` & `tap_mssql-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rwxr-xr-x   0        0        0    33005 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/LICENSE
--rwxr-xr-x   0        0        0    17787 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/README.md
--rw-r--r--   0        0        0     1100 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    28240 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/tap_mssql/__init__.py
--rwxr-xr-x   0        0        0     1515 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/tap_mssql/connection.py
--rwxr-xr-x   0        0        0        0 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/tap_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8500 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/tap_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2221 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/tap_mssql/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0     2751 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/tap_mssql/sync_strategies/incremental.py
--rw-r--r--   0        0        0    14867 2022-10-08 10:50:02.374924 tap-mssql-2.0.2/tap_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0    19221 1970-01-01 00:00:00.000000 tap-mssql-2.0.2/setup.py
--rw-r--r--   0        0        0    18771 1970-01-01 00:00:00.000000 tap-mssql-2.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0    33005 2023-08-04 10:15:52.026485 tap_mssql-2.1.0/LICENSE
+-rwxr-xr-x   0        0        0    19308 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/README.md
+-rw-r--r--   0        0        0     1180 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    28904 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/tap_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1723 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/tap_mssql/connection.py
+-rwxr-xr-x   0        0        0        0 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/tap_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     8774 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/tap_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2221 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/tap_mssql/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0     2751 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/tap_mssql/sync_strategies/incremental.py
+-rw-r--r--   0        0        0    15576 2023-08-04 10:15:52.030485 tap_mssql-2.1.0/tap_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0    20351 1970-01-01 00:00:00.000000 tap_mssql-2.1.0/PKG-INFO
```

### Comparing `tap-mssql-2.0.2/LICENSE` & `tap_mssql-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mssql-2.0.2/README.md` & `tap_mssql-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pipelinewise-tap-mssql
+![singer_sqlserver_tap](https://user-images.githubusercontent.com/84364906/220873968-8b2e7357-8539-421f-888f-97fb3a17975e.png)
 
 [Singer](https://www.singer.io/) tap that extracts data from a [mssql](https://www.mssql.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
 
 This is a [PipelineWise](https://transferwise.github.io/pipelinewise) compatible tap connector.
 
 ## How to use it
 
@@ -73,14 +74,20 @@
   "database": "db",
   "port": "3306",
   "user": "root",
   "password": "password"
 }
 ```
 
+Recommended optional settings
+
+* `"use_date_datatype": true`   - This will emit true timestamps and handle the time datatype.
+* `"use_singer_decimal": true`        - This will help avoid numeric rounding issues emitting as a string with a format of singer.decimal.
+* `"cursor_array_size": 10000` - This will help speed up extracts over a WAN or low latency network. The default is 1.
+
 Windows Authentication is available! Don't provide a user or password and pymssql will use the user that is running the process on windows to login.
 e.g.:
 
 ```json
 {
   "host": "localhost",
   "database": "db"
@@ -126,14 +133,48 @@
   "characterset": "utf8"
 }
 ```
 
 These are the same basic configuration properties used by the mssql command-line
 client (`mssql`).
 
+Optional:
+
+To emit all numeric values as strings and treat floats as string data types for the target, set use_singer_decimal to true. The resulting SCHEMA message will contain an attribute in additionalProperties containing the scale and precision of the discovered property:
+
+```json
+"property": {
+            "inclusion": "available",
+            "format": "singer.decimal",
+            "type": [
+              "null",
+              "number"
+            ],
+            "additionalProperties": {
+              "scale_precision": "(12,0)"
+            }
+```
+
+Usage:
+```json
+{
+  "use_singer_decimal": true
+}
+```
+
+Optional:
+
+A numeric setting adjusting the internal buffersize. The common query tuning scenario is for SELECT statements that return a large number of rows over a slow network. Increasing arraysize can improve performance by reducing the number of round-trips to the database. However increasing this value increases the amount of memory required.
+
+```json
+{
+  "cursor_array_size": 10000,
+}
+```
+
 ### Discovery mode
 
 The tap can be invoked in discovery mode to find the available tables and
 columns in the database:
 
 ```bash
 $ tap-mssql --config config.json --discover
```

### Comparing `tap-mssql-2.0.2/pyproject.toml` & `tap_mssql-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-mssql"
-version = "2.0.2"
+version = "2.1.0"
 description = "A pipelinewise compatible tap for connecting Microsoft SQL Server"
 authors = ["Rob Winters <wintersrd@gmail.com>"]
 license = "GNU Affero"
 readme = "README.md"
 homepage = "https://robertwinters.nl"
 repository = "https://github.com/wintersrd/pipelinewise-tap-mssql"
 keywords = ["singer", "meltano", "pipelinewise", "mssql"]
@@ -14,15 +14,16 @@
 tap-mssql = 'tap_mssql.__init__:main'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 attrs = ">=16.3.0"
 pendulum = ">=1.2.0"
 singer-python = "5.9.0"
-pymssql = ">=2.2.1"
+# pymssql==2.2.8 broken: https://github.com/pymssql/pymssql/issues/833
+pymssql = ">=2.1.1,!=2.2.8"
 backoff = ">=1.8.0"
 
 [tool.poetry.dev-dependencies]
 docker = "^5.0.3"
 pytest = "^7.0.0"
 pytest-cov = "^2.12.1"
 mypy = "^0.971"
@@ -32,9 +33,9 @@
 tox-poetry-installer = "^0.10.0"
 tox-docker = "4.0.0a2"
 pre-commit = "^2.17.0"
 bumpversion = "^0.6.0"
 tox = "^3.26.0"
 
 [build-system]
-requires = ["poetry>=1.2.0"]
+requires = ["poetry==1.4.2"]
 build-backend = "poetry.masonry.api"
```

### Comparing `tap-mssql-2.0.2/tap_mssql/__init__.py` & `tap_mssql-2.1.0/tap_mssql/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema
 
 import tap_mssql.sync_strategies.common as common
 import tap_mssql.sync_strategies.full_table as full_table
 import tap_mssql.sync_strategies.incremental as incremental
 import tap_mssql.sync_strategies.log_based as log_based
-from tap_mssql.connection import MSSQLConnection, connect_with_backoff
+from tap_mssql.connection import MSSQLConnection, connect_with_backoff, ResultIterator
+
+ARRAYSIZE = 1
 
 Column = collections.namedtuple(
     "Column",
     [
         "table_schema",
         "table_name",
         "column_name",
@@ -72,22 +74,29 @@
 
 VARIANT_TYPES = set(["json"])
 
 
 def default_date_format():
     return False
 
+def default_singer_decimal():
+    """
+    singer_decimal can be enabled in the the config, which will use singer.decimal as a format and string as the type
+    use this for large/precise numbers
+    """
+    return False
 
 def schema_for_column(c, config):
     """Returns the Schema object for the given Column."""
     data_type = c.data_type.lower()
 
     inclusion = "available"
 
-    use_date_data_type_format = config.get("use_date_datatype") or default_date_format()
+    use_date_data_type_format = config.get('use_date_datatype') or default_date_format()
+    use_singer_decimal = config.get('use_singer_decimal') or default_singer_decimal()
 
     if c.is_primary_key == 1:
         inclusion = "automatic"
 
     result = Schema(inclusion=inclusion)
 
     if data_type == "bit":
@@ -96,21 +105,29 @@
     elif data_type in BYTES_FOR_INTEGER_TYPE:
         result.type = ["null", "integer"]
         bits = BYTES_FOR_INTEGER_TYPE[data_type] * 8
         result.minimum = 0 - 2 ** (bits - 1)
         result.maximum = 2 ** (bits - 1) - 1
 
     elif data_type in FLOAT_TYPES:
-        result.type = ["null", "number"]
-        result.multipleOf = 10 ** (0 - (c.numeric_scale or 17))
+        if use_singer_decimal:
+            result.type = ["null","string"]
+            result.format = "singer.decimal"
+        else:
+            result.type = ["null", "number"]
+            result.multipleOf = 10 ** (0 - (c.numeric_scale or 17))
 
     elif data_type in DECIMAL_TYPES:
-        result.type = ["null", "number"]
-        result.multipleOf = 10 ** (0 - c.numeric_scale)
-        return result
+        if use_singer_decimal:
+            result.type = ["null","number"]
+            result.format = "singer.decimal"
+            result.additionalProperties = {"scale_precision": f"({c.character_maximum_length},{c.numeric_scale})"}
+        else:
+            result.type = ["null", "number"]
+            result.multipleOf = 10 ** (0 - c.numeric_scale)
 
     elif data_type in STRING_TYPES:
         result.type = ["null", "string"]
         # When length is -1 it is a long column type
         # https://docs.microsoft.com/en-us/sql/relational-databases/system-information-schema-views/columns-transact-sql?view=sql-server-ver15
         # -1 is not valid JSON schema
         # https://json-schema.org/understanding-json-schema/reference/string.html#length
@@ -232,24 +249,25 @@
 
                 left join constraint_columns cc
                     on cc.table_name = c.table_name
                     and cc.table_schema = c.table_schema
                     and cc.column_name = c.column_name
 
                 {}
-                ORDER BY c.table_schema, c.table_name
+                ORDER BY c.table_schema, c.table_name, c.ORDINAL_POSITION
         """.format(
                 table_schema_clause
             )
         )
         columns = []
-        rec = cur.fetchone()
-        while rec is not None:
+        LOGGER.info(f"{ARRAYSIZE=}")
+
+        for rec in ResultIterator(cur, ARRAYSIZE):
             columns.append(Column(*rec))
-            rec = cur.fetchone()
+
         LOGGER.info("Columns Fetched")
         entries = []
         for (k, cols) in itertools.groupby(columns, lambda c: (c.table_schema, c.table_name)):
             cols = list(cols)
             (table_schema, table_name) = k
             schema = Schema(
                 type="object",
@@ -433,18 +451,17 @@
     # Filter catalog to include only selected streams
     selected_streams = list(filter(lambda s: common.stream_is_selected(s), catalog.streams))
     streams_with_state = []
     streams_without_state = []
 
     for stream in selected_streams:
         stream_metadata = metadata.to_map(stream.metadata)
-        # if stream_metadata.table in ["aagaggpercols", "aagaggdef"]:
+
         for k, v in stream_metadata.get((), {}).items():
             LOGGER.info(f"{k}: {v}")
-            # LOGGER.info(stream_metadata.get((), {}).get("table-key-properties"))
         replication_method = stream_metadata.get((), {}).get("replication-method")
         stream_state = state.get("bookmarks", {}).get(stream.tap_stream_id)
 
         if not stream_state:
             if replication_method == "LOG_BASED":
                 LOGGER.info(
                     "LOG_BASED stream %s requires full historical sync", stream.tap_stream_id
@@ -480,15 +497,15 @@
     ordered_streams = streams_without_state + streams_with_state
 
     if currently_syncing:
         currently_syncing_stream = list(
             filter(
                 lambda s: s.tap_stream_id == currently_syncing
                 and is_valid_currently_syncing_stream(s, state),
-                streams_with_state,
+                ordered_streams,
             )
         )
 
         non_currently_syncing_streams = list(
             filter(lambda s: s.tap_stream_id != currently_syncing, ordered_streams)
         )
 
@@ -628,17 +645,16 @@
             )
 
         if replication_method == "INCREMENTAL" and not replication_key:
             LOGGER.info(
                 f"No replication key for {catalog_entry.table}, using full table replication"
             )
             replication_method = "FULL_TABLE"
-        if replication_method == "INCREMENTAL" and not primary_keys:
-            LOGGER.info(f"No primary key for {catalog_entry.table}, using full table replication")
-            replication_method = "FULL_TABLE"
+        # Check for INCREMENTAL load without primary keys removed
+        # INCREMENTAL loads can be performed without primary keys as long as there is a replication key
         if replication_method == "LOG_BASED" and not start_lsn:
             LOGGER.info(f"No initial load for {catalog_entry.table}, using full table replication")
         else:
             LOGGER.info(f"Table {catalog_entry.table} will use {replication_method} sync")
 
         database_name = common.get_database_name(catalog_entry)
 
@@ -653,15 +669,15 @@
                 LOGGER.info(f"syncing {catalog_entry.table} full table")
                 do_sync_full_table(mssql_conn, config, catalog_entry, state, columns)
             elif replication_method == "LOG_BASED":
                 LOGGER.info(f"syncing {catalog_entry.table} cdc tables")
                 do_sync_historical_log(mssql_conn, config, catalog_entry, state, columns)
             else:
                 raise Exception(
-                    "only INCREMENTAL, LOG_BASED and FULL TABLE replication methods are supported"
+                    "only INCREMENTAL, LOG_BASED and FULL_TABLE replication methods are supported"
                 )
 
     state = singer.set_currently_syncing(state, None)
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def sync_cdc_streams(mssql_conn, cdc_catalog, config, state):
@@ -725,18 +741,23 @@
                     *row,
                 )
         except:
             LOGGER.warning("Encountered error checking server params.")
 
 
 def main_impl():
+
+    global ARRAYSIZE
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     mssql_conn = MSSQLConnection(args.config)
     log_server_params(mssql_conn)
 
+    ARRAYSIZE = args.config.get('cursor_array_size',1)
+    common.ARRAYSIZE = ARRAYSIZE
+
     if args.discover:
         do_discover(mssql_conn, args.config)
     elif args.catalog:
         state = args.state or {}
         do_sync(mssql_conn, args.config, args.catalog, state)
     elif args.properties:
         catalog = Catalog.from_dict(args.properties)
```

### Comparing `tap-mssql-2.0.2/tap_mssql/connection.py` & `tap_mssql-2.1.0/tap_mssql/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,7 +50,15 @@
     class ConnectionWrapper(MSSQLConnection):
         def __init__(self, *args, **kwargs):
             super().__init__(config)
 
             connect_with_backoff(self)
 
     return ConnectionWrapper
+
+def ResultIterator(cursor, arraysize=1):
+    while True:
+        results = cursor.fetchmany(arraysize)
+        if not results:
+            break
+        for result in results:
+            yield result
```

### Comparing `tap-mssql-2.0.2/tap_mssql/sync_strategies/common.py` & `tap_mssql-2.1.0/tap_mssql/sync_strategies/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import time
 import uuid
 
 import singer
 import singer.metrics as metrics
 from singer import metadata, utils
 
+from tap_mssql.connection import ResultIterator
+
+ARRAYSIZE = 1
+
 LOGGER = singer.get_logger()
 
 
 def escape(string):
     if "`" in string:
         raise Exception(
             "Can't escape identifier {} because it contains a double quote".format(string)
@@ -80,28 +84,27 @@
     database_name = get_database_name(catalog_entry)
     escaped_db = escape(database_name)
     escaped_table = escape(catalog_entry.table)
     escaped_columns = [escape(c) for c in columns]
 
     select_sql = "SELECT {} FROM {}.{}".format(",".join(escaped_columns), escaped_db, escaped_table)
 
-    # escape percent signs
-    select_sql = select_sql.replace("%", "%%")
     return select_sql
 
 
 def default_date_format():
     return False
 
 
 def row_to_singer_record(catalog_entry, version, row, columns, time_extracted, config):
     row_to_persist = ()
     use_date_data_type_format = config.get("use_date_datatype") or default_date_format()
     for idx, elem in enumerate(row):
         property_type = catalog_entry.schema.properties[columns[idx]].type
+        property_format = catalog_entry.schema.properties[columns[idx]].format
         if isinstance(elem, datetime.datetime):
             row_to_persist += (elem.isoformat() + "+00:00",)
 
         elif isinstance(elem, datetime.time):
             if use_date_data_type_format:
                 # Writing Dates with a Date Datatype, not converting it to a datetime.
                 row_to_persist += (elem.isoformat(),)
@@ -137,14 +140,19 @@
             elif elem == 0:
                 boolean_representation = False
             else:
                 boolean_representation = True
             row_to_persist += (boolean_representation,)
         elif isinstance(elem, uuid.UUID):
             row_to_persist += (str(elem),)
+        elif property_format == 'singer.decimal':
+            if elem is None:
+                row_to_persist += (elem,)
+            else:
+                row_to_persist += (str(elem),)
         else:
             row_to_persist += (elem,)
     rec = dict(zip(columns, row_to_persist))
 
     return singer.RecordMessage(
         stream=catalog_entry.stream, record=rec, version=version, time_extracted=time_extracted
     )
@@ -163,24 +171,25 @@
     replication_key = singer.get_bookmark(state, catalog_entry.tap_stream_id, "replication_key")
 
     # query_string = cursor.mogrify(select_sql, params)
 
     time_extracted = utils.now()
     cursor.execute(select_sql, params)
 
-    row = cursor.fetchone()
-    rows_saved = 0
+    LOGGER.info(f"{ARRAYSIZE=}")
 
     database_name = get_database_name(catalog_entry)
 
+    rows_saved = 0
+
     with metrics.record_counter(None) as counter:
         counter.tags["database"] = database_name
         counter.tags["table"] = catalog_entry.table
-
-        while row:
+        
+        for row in ResultIterator(cursor, ARRAYSIZE):
             counter.increment()
             rows_saved += 1
             record_message = row_to_singer_record(
                 catalog_entry, stream_version, row, columns, time_extracted, config
             )
             singer.write_message(record_message)
             md_map = metadata.to_map(catalog_entry.metadata)
@@ -230,10 +239,8 @@
                         catalog_entry.tap_stream_id,
                         "replication_key_value",
                         record_message.record[replication_key],
                     )
             if rows_saved % 1000 == 0:
                 singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
-            row = cursor.fetchone()
-
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
```

### Comparing `tap-mssql-2.0.2/tap_mssql/sync_strategies/full_table.py` & `tap_mssql-2.1.0/tap_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `tap-mssql-2.0.2/tap_mssql/sync_strategies/incremental.py` & `tap_mssql-2.1.0/tap_mssql/sync_strategies/incremental.py`

 * *Files identical despite different names*

### Comparing `tap-mssql-2.0.2/tap_mssql/sync_strategies/log_based.py` & `tap_mssql-2.1.0/tap_mssql/sync_strategies/log_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             select_sql = """
                             SELECT {}
                                 ,'I' _sdc_operation_type
                                 , cast('1900-01-01' as datetime) _sdc_lsn_commit_timestamp
                                 , null _sdc_lsn_deleted_at
                                 , '00000000000000000000' _sdc_lsn_value
                                 , '00000000000000000000' _sdc_lsn_seq_value
-                                , 1 as _sdc_lsn_operation
+                                , 2 as _sdc_lsn_operation
                             FROM {}.{}
                             ;""".format(
                 ",".join(escaped_columns), schema_name, table_name
             )
             params = {}
 
             common.sync_query(
@@ -313,25 +313,39 @@
                             "The last lsn processed as per the state file %s, minimum available lsn"
                             " for extract table %s, and the maximum lsn is %s."
                         ),
                         state_last_lsn,
                         lsn_from,
                         lsn_to,
                     )
+                    if lsn_to == state_last_lsn:
+                        LOGGER.info(
+                            (
+                                "The last lsn processed as per the state file is equal to the max"
+                                " lsn available - no changes expected - state lsn will not be incremented"
+                            ),
+                        )
+                        from_lsn_expression = "{}".format(py_bin_to_mssql(state_last_lsn))
+                    else:
+                        from_lsn_expression = (
+                            (
+                                "sys.fn_cdc_increment_lsn({})"
+                            ).format(py_bin_to_mssql(state_last_lsn))
+                        )
                 else:
                     raise Exception(
                         (
                             "Error {}.{}: CDC changes have expired, the minimum lsn is {}, the last"
                             " processed lsn is {}. Recommend a full load as there may be missing data."
                         ).format(schema_name, table_name, lsn_from, state_last_lsn)
                     )
 
                 select_sql = """DECLARE @from_lsn binary (10), @to_lsn binary (10)
 
-                                SET @from_lsn = sys.fn_cdc_increment_lsn({})
+                                SET @from_lsn = {}
                                 SET @to_lsn = {}
 
                                 SELECT {}
                                     ,case __$operation
                                         when 2 then 'I'
                                         when 4 then 'U'
                                         when 1 then 'D'
@@ -343,15 +357,15 @@
                                         end _sdc_lsn_deleted_at
                                     , __$start_lsn _sdc_lsn_value
                                     , __$seqval _sdc_lsn_seq_value
                                     , __$operation _sdc_lsn_operation
                                 FROM cdc.fn_cdc_get_all_changes_{}(@from_lsn, @to_lsn, 'all')
                                 ORDER BY __$start_lsn, __$seqval, __$operation
                                 ;""".format(
-                    py_bin_to_mssql(state_last_lsn),
+                    from_lsn_expression,
                     py_bin_to_mssql(lsn_to),
                     ",".join(escaped_columns),
                     schema_table,
                 )
 
                 params = {}
```

### Comparing `tap-mssql-2.0.2/PKG-INFO` & `tap_mssql-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: tap-mssql
-Version: 2.0.2
+Version: 2.1.0
 Summary: A pipelinewise compatible tap for connecting Microsoft SQL Server
 Home-page: https://robertwinters.nl
 License: GNU Affero
 Keywords: singer,meltano,pipelinewise,mssql
 Author: Rob Winters
 Author-email: wintersrd@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Requires-Dist: attrs (>=16.3.0)
 Requires-Dist: backoff (>=1.8.0)
 Requires-Dist: pendulum (>=1.2.0)
-Requires-Dist: pymssql (>=2.2.1)
+Requires-Dist: pymssql (>=2.1.1,!=2.2.8)
 Requires-Dist: singer-python (==5.9.0)
 Project-URL: Repository, https://github.com/wintersrd/pipelinewise-tap-mssql
 Description-Content-Type: text/markdown
 
 # pipelinewise-tap-mssql
+![singer_sqlserver_tap](https://user-images.githubusercontent.com/84364906/220873968-8b2e7357-8539-421f-888f-97fb3a17975e.png)
 
 [Singer](https://www.singer.io/) tap that extracts data from a [mssql](https://www.mssql.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
 
 This is a [PipelineWise](https://transferwise.github.io/pipelinewise) compatible tap connector.
 
 ## How to use it
 
@@ -99,14 +101,20 @@
   "database": "db",
   "port": "3306",
   "user": "root",
   "password": "password"
 }
 ```
 
+Recommended optional settings
+
+* `"use_date_datatype": true`   - This will emit true timestamps and handle the time datatype.
+* `"use_singer_decimal": true`        - This will help avoid numeric rounding issues emitting as a string with a format of singer.decimal.
+* `"cursor_array_size": 10000` - This will help speed up extracts over a WAN or low latency network. The default is 1.
+
 Windows Authentication is available! Don't provide a user or password and pymssql will use the user that is running the process on windows to login.
 e.g.:
 
 ```json
 {
   "host": "localhost",
   "database": "db"
@@ -152,14 +160,48 @@
   "characterset": "utf8"
 }
 ```
 
 These are the same basic configuration properties used by the mssql command-line
 client (`mssql`).
 
+Optional:
+
+To emit all numeric values as strings and treat floats as string data types for the target, set use_singer_decimal to true. The resulting SCHEMA message will contain an attribute in additionalProperties containing the scale and precision of the discovered property:
+
+```json
+"property": {
+            "inclusion": "available",
+            "format": "singer.decimal",
+            "type": [
+              "null",
+              "number"
+            ],
+            "additionalProperties": {
+              "scale_precision": "(12,0)"
+            }
+```
+
+Usage:
+```json
+{
+  "use_singer_decimal": true
+}
+```
+
+Optional:
+
+A numeric setting adjusting the internal buffersize. The common query tuning scenario is for SELECT statements that return a large number of rows over a slow network. Increasing arraysize can improve performance by reducing the number of round-trips to the database. However increasing this value increases the amount of memory required.
+
+```json
+{
+  "cursor_array_size": 10000,
+}
+```
+
 ### Discovery mode
 
 The tap can be invoked in discovery mode to find the available tables and
 columns in the database:
 
 ```bash
 $ tap-mssql --config config.json --discover
```

