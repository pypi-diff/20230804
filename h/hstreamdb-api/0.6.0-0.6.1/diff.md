# Comparing `tmp/hstreamdb-api-0.6.0.tar.gz` & `tmp/hstreamdb-api-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hstreamdb-api-0.6.0.tar", last modified: Thu Jul 20 06:11:36 2023, max compression
+gzip compressed data, was "/home/runner/work/protocol/protocol/api/python/dist/tmp6m6g1m5o/hstreamdb-api-0.6.1.tar", last modified: Fri Aug  4 10:07:38 2023, max compression
```

## Comparing `hstreamdb-api-0.6.0.tar` & `hstreamdb-api-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 06:11:22.000000 hstreamdb-api-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 06:11:22.000000 hstreamdb-api-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/HStream/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/HStream/Server/
--rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/HStream/Server/HStreamApi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   101025 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/HStream/Server/HStreamApi_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 06:11:22.000000 hstreamdb-api-0.6.0/src/HStream/Server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 06:11:22.000000 hstreamdb-api-0.6.0/src/HStream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/hstreamdb_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/hstreamdb_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/hstreamdb_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/hstreamdb_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/hstreamdb_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 06:11:36.000000 hstreamdb-api-0.6.0/src/hstreamdb_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 10:07:22.000000 hstreamdb-api-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 10:07:22.000000 hstreamdb-api-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-04 10:07:37.000000 hstreamdb-api-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/HStream/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/HStream/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)    45691 2023-08-04 10:07:37.000000 hstreamdb-api-0.6.1/src/HStream/Server/HStreamApi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109431 2023-08-04 10:07:37.000000 hstreamdb-api-0.6.1/src/HStream/Server/HStreamApi_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:22.000000 hstreamdb-api-0.6.1/src/HStream/Server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:22.000000 hstreamdb-api-0.6.1/src/HStream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/hstreamdb_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/hstreamdb_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/hstreamdb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/hstreamdb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/hstreamdb_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 10:07:38.000000 hstreamdb-api-0.6.1/src/hstreamdb_api.egg-info/top_level.txt
```

### Comparing `hstreamdb-api-0.6.0/PKG-INFO` & `hstreamdb-api-0.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstreamdb-api
-Version: 0.6.0
+Version: 0.6.1
 Summary: HStreamDB api for Python
 Home-page: https://github.com/hstreamdb/hstream
 Author: lambda
 Author-email: lambda@emqx.io
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hstreamdb/hstream/issues
 Description: # hstreamdb-api
```

### Comparing `hstreamdb-api-0.6.0/setup.py` & `hstreamdb-api-0.6.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# sed "s/0.6.0/your_pkg_version/g" setup_temp.py > setup.py
+# sed "s/0.6.1/your_pkg_version/g" setup_temp.py > setup.py
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-verison = "0.6.0"
+verison = "0.6.1"
 
 setuptools.setup(
     name="hstreamdb-api",
     version=verison,
     author="lambda",
     author_email="lambda@emqx.io",
     description="HStreamDB api for Python",
```

### Comparing `hstreamdb-api-0.6.0/src/HStream/Server/HStreamApi_pb2.py` & `hstreamdb-api-0.6.1/src/HStream/Server/HStreamApi_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,53 +12,53 @@
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fHStream/Server/HStreamApi.proto\x12\x0ehstream.server\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\"@\n\x0fTimestampOffset\x12\x15\n\rtimestampInMs\x18\x01 \x01(\x03\x12\x16\n\x0estrictAccuracy\x18\x02 \x01(\x08\"\xbd\x01\n\x0bShardOffset\x12\x36\n\rspecialOffset\x18\x01 \x01(\x0e\x32\x1d.hstream.server.SpecialOffsetH\x00\x12\x30\n\x0crecordOffset\x18\x02 \x01(\x0b\x32\x18.hstream.server.RecordIdH\x00\x12:\n\x0ftimestampOffset\x18\x03 \x01(\x0b\x32\x1f.hstream.server.TimestampOffsetH\x00\x42\x08\n\x06offset\"\x1a\n\x0b\x45\x63hoRequest\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\x1b\n\x0c\x45\x63hoResponse\x12\x0b\n\x03msg\x18\x01 \x01(\t\"(\n\x11\x43ommandStreamTask\x12\x13\n\x0b\x63ommand_sql\x18\x01 \x01(\t\"1\n\x19\x43ommandStreamTaskResponse\x12\x14\n\x0c\x63ommand_resp\x18\x01 \x01(\t\"B\n\x0e\x43ommandConnect\x12\x16\n\x0e\x63lient_version\x18\x01 \x01(\t\x12\x18\n\x10protocol_version\x18\x02 \x01(\x05\"D\n\x10\x43ommandConnected\x12\x16\n\x0eserver_version\x18\x01 \x01(\t\x12\x18\n\x10protocol_version\x18\x02 \x01(\x05\"!\n\x0c\x43ommandQuery\x12\x11\n\tstmt_text\x18\x01 \x01(\t\"C\n\x14\x43ommandQueryResponse\x12+\n\nresult_set\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct\" \n\x10GetStreamRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\";\n\x11GetStreamResponse\x12&\n\x06stream\x18\x01 \x01(\x0b\x32\x16.hstream.server.Stream\"d\n\rAppendRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12.\n\x07records\x18\x03 \x01(\x0b\x32\x1d.hstream.server.BatchedRecord\"b\n\x0e\x41ppendResponse\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12+\n\trecordIds\x18\x03 \x03(\x0b\x32\x18.hstream.server.RecordId\"\xd1\x01\n\x0cSubscription\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12\x19\n\x11\x61\x63kTimeoutSeconds\x18\x03 \x01(\x05\x12\x19\n\x11maxUnackedRecords\x18\x04 \x01(\x05\x12-\n\x06offset\x18\x05 \x01(\x0e\x32\x1d.hstream.server.SpecialOffset\x12\x30\n\x0c\x63reationTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"6\n\x12SubscriptionOffset\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\x12\x0f\n\x07\x62\x61tchId\x18\x02 \x01(\x04\"$\n\x16GetSubscriptionRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x82\x01\n\x17GetSubscriptionResponse\x12\x32\n\x0csubscription\x18\x01 \x01(\x0b\x32\x1c.hstream.server.Subscription\x12\x33\n\x07offsets\x18\x02 \x03(\x0b\x32\".hstream.server.SubscriptionOffset\"B\n\x19\x44\x65leteSubscriptionRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"7\n\x1d\x43heckSubscriptionExistRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\"0\n\x1e\x43heckSubscriptionExistResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\"o\n\x15StreamingFetchRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12\x14\n\x0c\x63onsumerName\x18\x02 \x01(\t\x12(\n\x06\x61\x63kIds\x18\x03 \x03(\x0b\x32\x18.hstream.server.RecordId\"Q\n\x16StreamingFetchResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x01(\x0b\x32\x1e.hstream.server.ReceivedRecord\"l\n\x0eReceivedRecord\x12+\n\trecordIds\x18\x01 \x03(\x0b\x32\x18.hstream.server.RecordId\x12-\n\x06record\x18\x02 \x01(\x0b\x32\x1d.hstream.server.BatchedRecord\"P\n\x13\x44\x65leteStreamRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x16\n\x0eignoreNonExist\x18\x02 \x01(\x08\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\">\n\x13ListStreamsResponse\x12\'\n\x07streams\x18\x01 \x03(\x0b\x32\x16.hstream.server.Stream\"\x14\n\x12ListStreamsRequest\".\n\x1cListStreamsWithPrefixRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\"\x1a\n\x18ListSubscriptionsRequest\"4\n\"ListSubscriptionsWithPrefixRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\"O\n\x19ListSubscriptionsResponse\x12\x32\n\x0csubscription\x18\x01 \x03(\x0b\x32\x1c.hstream.server.Subscription\".\n\x14ListConsumersRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\"D\n\x15ListConsumersResponse\x12+\n\tconsumers\x18\x01 \x03(\x0b\x32\x18.hstream.server.Consumer\"X\n\x11TrimStreamRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12/\n\ttrimPoint\x18\x02 \x01(\x0b\x32\x1c.hstream.server.StreamOffset\"\x96\x01\n\x06Stream\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x19\n\x11replicationFactor\x18\x02 \x01(\r\x12\x17\n\x0f\x62\x61\x63klogDuration\x18\x03 \x01(\r\x12\x12\n\nshardCount\x18\x04 \x01(\r\x12\x30\n\x0c\x63reationTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9e\x01\n\rBatchedRecord\x12\x38\n\x0f\x63ompressionType\x18\x01 \x01(\x0e\x32\x1f.hstream.server.CompressionType\x12/\n\x0bpublishTime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tbatchSize\x18\x03 \x01(\r\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\"U\n\rHStreamRecord\x12\x33\n\x06header\x18\x01 \x01(\x0b\x32#.hstream.server.HStreamRecordHeader\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"E\n\x13\x42\x61tchHStreamRecords\x12.\n\x07records\x18\x01 \x03(\x0b\x32\x1d.hstream.server.HStreamRecord\"\xf1\x01\n\x13HStreamRecordHeader\x12\x36\n\x04\x66lag\x18\x01 \x01(\x0e\x32(.hstream.server.HStreamRecordHeader.Flag\x12G\n\nattributes\x18\x02 \x03(\x0b\x32\x33.hstream.server.HStreamRecordHeader.AttributesEntry\x12\x0b\n\x03key\x18\x03 \x01(\t\x1a\x31\n\x0f\x41ttributesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x19\n\x04\x46lag\x12\x08\n\x04JSON\x10\x00\x12\x07\n\x03RAW\x10\x01\"@\n\x08RecordId\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\x12\x0f\n\x07\x62\x61tchId\x18\x02 \x01(\x04\x12\x12\n\nbatchIndex\x18\x03 \x01(\r\"\x81\x01\n\x05Shard\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12\x19\n\x11startHashRangeKey\x18\x03 \x01(\t\x12\x17\n\x0f\x65ndHashRangeKey\x18\x04 \x01(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\x04\x12\x10\n\x08isActive\x18\x06 \x01(\x08\"\'\n\x11ListShardsRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\";\n\x12ListShardsResponse\x12%\n\x06shards\x18\x01 \x03(\x0b\x32\x15.hstream.server.Shard\"g\n\x10TrimShardRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12.\n\ttrimPoint\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\"\x94\x01\n\x18\x43reateShardReaderRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12\x30\n\x0bshardOffset\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x10\n\x08readerId\x18\x04 \x01(\t\x12\x0f\n\x07timeout\x18\x05 \x01(\r\"\x95\x01\n\x19\x43reateShardReaderResponse\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12\x30\n\x0bshardOffset\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x10\n\x08readerId\x18\x04 \x01(\t\x12\x0f\n\x07timeout\x18\x05 \x01(\r\"8\n\x10ReadShardRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x12\n\nmaxRecords\x18\x02 \x01(\r\",\n\x18\x44\x65leteShardReaderRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\"L\n\x11ReadShardResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"\x19\n\x17ListShardReadersRequest\",\n\x18ListShardReadersResponse\x12\x10\n\x08readerId\x18\x01 \x03(\t\"\xaa\x01\n\x16ReadShardStreamRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12)\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x16\n\x0emaxReadBatches\x18\x04 \x01(\x04\x12*\n\x05until\x18\x05 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\"R\n\x17ReadShardStreamResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"\x8c\x01\n\x0cStreamOffset\x12\x36\n\rspecialOffset\x18\x01 \x01(\x0e\x32\x1d.hstream.server.SpecialOffsetH\x00\x12:\n\x0ftimestampOffset\x18\x02 \x01(\x0b\x32\x1f.hstream.server.TimestampOffsetH\x00\x42\x08\n\x06offset\"\xaa\x01\n\x11ReadStreamRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12*\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1c.hstream.server.StreamOffset\x12+\n\x05until\x18\x04 \x01(\x0b\x32\x1c.hstream.server.StreamOffset\x12\x16\n\x0emaxReadBatches\x18\x05 \x01(\x04\"M\n\x12ReadStreamResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"\xb3\x01\n\x1cReadSingleShardStreamRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12)\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12*\n\x05until\x18\x04 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x16\n\x0emaxReadBatches\x18\x05 \x01(\x04\"X\n\x1dReadSingleShardStreamResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"(\n\x15TerminateQueryRequest\x12\x0f\n\x07queryId\x18\x01 \x01(\t\"4\n\x12\x43reateQueryRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x11\n\tqueryName\x18\x02 \x01(\t\"T\n\x1f\x43reateQueryWithNamespaceRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x11\n\tqueryName\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\"\x14\n\x12ListQueriesRequest\"=\n\x13ListQueriesResponse\x12&\n\x07queries\x18\x01 \x03(\x0b\x32\x15.hstream.server.Query\"\x1d\n\x0fGetQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\"8\n\x08\x43onsumer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x11\n\tuserAgent\x18\x03 \x01(\t\"\xc7\x01\n\x05Query\x12\n\n\x02id\x18\x01 \x01(\t\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x1c.hstream.server.TaskStatusPB\x12\x13\n\x0b\x63reatedTime\x18\x03 \x01(\x03\x12\x11\n\tqueryText\x18\x04 \x01(\t\x12\x0f\n\x07sources\x18\x05 \x03(\t\x12\x12\n\nresultName\x18\x06 \x01(\t\x12\'\n\x04type\x18\x07 \x01(\x0e\x32\x19.hstream.server.QueryType\x12\x0e\n\x06nodeId\x18\x08 \x01(\r\" \n\x12\x44\x65leteQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x12ResumeQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1f\n\x11PauseQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1e\n\x0fParseSqlRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\"P\n\x10ParseSqlResponse\x12\x35\n\x06\x65vqSql\x18\x01 \x01(\x0b\x32#.hstream.server.ExecuteViewQuerySqlH\x00\x42\x05\n\x03sql\"#\n\x13\x45xecuteViewQuerySql\x12\x0c\n\x04view\x18\x01 \x01(\t\"T\n\x16\x43reateConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0e\n\x06target\x18\x03 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x04 \x01(\t\"\x17\n\x15ListConnectorsRequest\"G\n\x16ListConnectorsResponse\x12-\n\nconnectors\x18\x01 \x03(\x0b\x32\x19.hstream.server.Connector\"#\n\x13GetConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"7\n\x17GetConnectorSpecRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06target\x18\x02 \x01(\t\"(\n\x18GetConnectorSpecResponse\x12\x0c\n\x04spec\x18\x01 \x01(\t\"E\n\x17GetConnectorLogsRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\"(\n\x18GetConnectorLogsResponse\x12\x0c\n\x04logs\x18\x01 \x01(\t\"\xf6\x01\n\tConnector\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0e\n\x06target\x18\x03 \x01(\t\x12\x30\n\x0c\x63reationTime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x06 \x01(\t\x12(\n\x07offsets\x18\x07 \x03(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06taskId\x18\x08 \x01(\t\x12\x0c\n\x04node\x18\t \x01(\t\x12\x14\n\x0c\x64ockerStatus\x18\n \x01(\t\x12\r\n\x05image\x18\x0b \x01(\t\"&\n\x16\x44\x65leteConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"%\n\x15PauseConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"&\n\x16ResumeConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\" \n\x0eGetViewRequest\x12\x0e\n\x06viewId\x18\x01 \x01(\t\";\n\x11\x44\x65leteViewRequest\x12\x0e\n\x06viewId\x18\x01 \x01(\t\x12\x16\n\x0eignoreNonExist\x18\x02 \x01(\x08\"\x12\n\x10ListViewsRequest\"8\n\x11ListViewsResponse\x12#\n\x05views\x18\x01 \x03(\x0b\x32\x14.hstream.server.View\"\x89\x01\n\x04View\x12\x0e\n\x06viewId\x18\x01 \x01(\t\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x1c.hstream.server.TaskStatusPB\x12\x13\n\x0b\x63reatedTime\x18\x03 \x01(\x03\x12\x0b\n\x03sql\x18\x04 \x01(\t\x12\x0e\n\x06schema\x18\x05 \x03(\t\x12\x11\n\tqueryName\x18\x06 \x01(\t\"D\n\x18\x45xecuteViewQueryResponse\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct\"&\n\x17\x45xecuteViewQueryRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\"F\n$ExecuteViewQueryWithNamespaceRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\"&\n\x11StatsIntervalVals\x12\x11\n\tintervals\x18\x01 \x03(\x05\"\x1f\n\x0fStatsDoubleVals\x12\x0c\n\x04vals\x18\x01 \x03(\x01\"&\n\x13\x41\x64minCommandRequest\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\"&\n\x14\x41\x64minCommandResponse\x12\x0e\n\x06result\x18\x01 \x01(\t\"{\n\x1fPerStreamTimeSeriesStatsRequest\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12\x34\n\tintervals\x18\x03 \x01(\x0b\x32!.hstream.server.StatsIntervalVals\"R\n PerStreamTimeSeriesStatsResponse\x12.\n\x05stats\x18\x01 \x01(\x0b\x32\x1f.hstream.server.StatsDoubleVals\"\xc3\x01\n#PerStreamTimeSeriesStatsAllResponse\x12M\n\x05stats\x18\x01 \x03(\x0b\x32>.hstream.server.PerStreamTimeSeriesStatsAllResponse.StatsEntry\x1aM\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.hstream.server.StatsDoubleVals:\x02\x38\x01\"j\n\"PerStreamTimeSeriesStatsAllRequest\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x34\n\tintervals\x18\x02 \x01(\x0b\x32!.hstream.server.StatsIntervalVals\"\xb7\x01\n\x17\x44\x65scribeClusterResponse\x12\x17\n\x0fprotocolVersion\x18\x01 \x01(\t\x12/\n\x0bserverNodes\x18\x02 \x03(\x0b\x32\x1a.hstream.server.ServerNode\x12;\n\x11serverNodesStatus\x18\x03 \x03(\x0b\x32 .hstream.server.ServerNodeStatus\x12\x15\n\rclusterUpTime\x18\x04 \x01(\x04\"e\n\nServerNode\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\x12/\n\x07version\x18\x04 \x01(\x0b\x32\x1e.hstream.server.HStreamVersion\"f\n\x10ServerNodeStatus\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x1a.hstream.server.ServerNode\x12(\n\x05state\x18\x02 \x01(\x0e\x32\x19.hstream.server.NodeState\"1\n\x0eHStreamVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x02 \x01(\t\"%\n\x12LookupShardRequest\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\"V\n\x13LookupShardResponse\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\x12.\n\nserverNode\x18\x02 \x01(\x0b\x32\x1a.hstream.server.ServerNode\"3\n\x19LookupSubscriptionRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\"d\n\x1aLookupSubscriptionResponse\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12.\n\nserverNode\x18\x02 \x01(\x0b\x32\x1a.hstream.server.ServerNode\",\n\x18LookupShardReaderRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\"]\n\x19LookupShardReaderResponse\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12.\n\nserverNode\x18\x02 \x01(\x0b\x32\x1a.hstream.server.ServerNode\"U\n\x15LookupResourceRequest\x12-\n\x07resType\x18\x01 \x01(\x0e\x32\x1c.hstream.server.ResourceType\x12\r\n\x05resId\x18\x02 \x01(\t\"=\n\x16GetTailRecordIdRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\"I\n\x17GetTailRecordIdResponse\x12.\n\x0ctailRecordId\x18\x01 \x01(\x0b\x32\x18.hstream.server.RecordId\"\x8f\x02\n\x08StatType\x12\x31\n\nstreamStat\x18\x01 \x01(\x0e\x32\x1b.hstream.server.StreamStatsH\x00\x12\x34\n\x07subStat\x18\x02 \x01(\x0e\x32!.hstream.server.SubscriptionStatsH\x00\x12\x32\n\x08\x63onnStat\x18\x03 \x01(\x0e\x32\x1e.hstream.server.ConnectorStatsH\x00\x12/\n\tqueryStat\x18\x04 \x01(\x0e\x32\x1a.hstream.server.QueryStatsH\x00\x12-\n\x08viewStat\x18\x05 \x01(\x0e\x32\x19.hstream.server.ViewStatsH\x00\x42\x06\n\x04stat\"\xa9\x01\n\tStatValue\x12*\n\x08statType\x18\x01 \x01(\x0b\x32\x18.hstream.server.StatType\x12=\n\nstatValues\x18\x02 \x03(\x0b\x32).hstream.server.StatValue.StatValuesEntry\x1a\x31\n\x0fStatValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"H\n\tStatError\x12*\n\x08statType\x18\x01 \x01(\x0b\x32\x18.hstream.server.StatType\x12\x0f\n\x07message\x18\x02 \x01(\t\":\n\x0fGetStatsRequest\x12\'\n\x05stats\x18\x01 \x03(\x0b\x32\x18.hstream.server.StatType\"m\n\x10GetStatsResponse\x12.\n\x0bstatsValues\x18\x01 \x03(\x0b\x32\x19.hstream.server.StatValue\x12)\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x19.hstream.server.StatError*)\n\rSpecialOffset\x12\x0c\n\x08\x45\x41RLIEST\x10\x00\x12\n\n\x06LATEST\x10\x01*/\n\x0f\x43ompressionType\x12\x08\n\x04None\x10\x00\x12\x08\n\x04Gzip\x10\x01\x12\x08\n\x04Zstd\x10\x02*\x90\x01\n\x0cTaskStatusPB\x12\x11\n\rTASK_CREATING\x10\x00\x12\x10\n\x0cTASK_RUNNING\x10\x01\x12\x10\n\x0cTASK_ABORTED\x10\x02\x12\x0f\n\x0bTASK_PAUSED\x10\x03\x12\x11\n\rTASK_RESUMING\x10\x04\x12\x13\n\x0fTASK_TERMINATED\x10\x05\x12\x10\n\x0cTASK_UNKNOWN\x10\x06*1\n\tQueryType\x12\x12\n\x0e\x43reateStreamAs\x10\x00\x12\x10\n\x0c\x43reateViewAs\x10\x01*A\n\tNodeState\x12\x0c\n\x08Starting\x10\x00\x12\x0b\n\x07Running\x10\x01\x12\x0f\n\x0bUnavailable\x10\x02\x12\x08\n\x04\x44\x65\x61\x64\x10\x03*\x81\x01\n\x0cResourceType\x12\r\n\tResStream\x10\x00\x12\x13\n\x0fResSubscription\x10\x01\x12\x0c\n\x08ResShard\x10\x02\x12\x12\n\x0eResShardReader\x10\x03\x12\x10\n\x0cResConnector\x10\x04\x12\x0c\n\x08ResQuery\x10\x05\x12\x0b\n\x07ResView\x10\x06*X\n\x0bStreamStats\x12\x11\n\rAppendInBytes\x10\x00\x12\x13\n\x0f\x41ppendInRecords\x10\x01\x12\x0f\n\x0b\x41ppendTotal\x10\x02\x12\x10\n\x0c\x41ppendFailed\x10\x03*\xcf\x01\n\x11SubscriptionStats\x12\x10\n\x0cSendOutBytes\x10\x00\x12\x12\n\x0eSendOutRecords\x10\x01\x12\x18\n\x14SendOutRecordsFailed\x10\x02\x12\x11\n\rResendRecords\x10\x03\x12\x17\n\x13ResendRecordsFailed\x10\x04\x12\x10\n\x0cReceivedAcks\x10\x05\x12\x13\n\x0fRequestMessages\x10\x06\x12\x14\n\x10ResponseMessages\x10\x07\x12\x11\n\rChecklistSize\x10\x08*>\n\x0e\x43onnectorStats\x12\x16\n\x12\x44\x65liveredInRecords\x10\x00\x12\x14\n\x10\x44\x65liveredInBytes\x10\x01*S\n\nQueryStats\x12\x15\n\x11TotalInputRecords\x10\x00\x12\x16\n\x12TotalOutputRecords\x10\x01\x12\x16\n\x12TotalExecuteErrors\x10\x02*$\n\tViewStats\x12\x17\n\x13TotalExecuteQueries\x10\x00*\xed\x08\n\tErrorCode\x12\x11\n\rInternalError\x10\x00\x12\x13\n\x0eStreamNotFound\x10\xc8\x01\x12\x11\n\x0cStreamExists\x10\xc9\x01\x12\x1c\n\x17StreamFoundSubscription\x10\xca\x01\x12\x1f\n\x1aStreamInvalidReplicaFactor\x10\xcb\x01\x12\"\n\x1dStreamInvalidObjectIdentifier\x10\xcc\x01\x12\x1c\n\x17StreamInvalidShardCount\x10\xcd\x01\x12\x1d\n\x18StreamEmptyBatchedRecord\x10\xce\x01\x12\x1c\n\x17StreamInvalidRecordSize\x10\xcf\x01\x12\x18\n\x13StreamInvalidOffset\x10\xd0\x01\x12\x19\n\x14SubscriptionNotFound\x10\xac\x02\x12\x17\n\x12SubscriptionExists\x10\xad\x02\x12,\n\'SubscriptionCreationOnNonExistentStream\x10\xae\x02\x12\x1e\n\x19SubscriptionInvalidOffset\x10\xaf\x02\x12(\n#SubscriptionInvalidObjectIdentifier\x10\xb0\x02\x12%\n SubscriptionFoundActiveConsumers\x10\xb1\x02\x12\x12\n\rQueryNotFound\x10\x90\x03\x12\x10\n\x0bQueryExists\x10\x91\x03\x12\x14\n\x0fQueryInvalidSQL\x10\x92\x03\x12\x1d\n\x18QueryFoundAssociatedView\x10\x93\x03\x12!\n\x1cQueryInvalidObjectIdentifier\x10\x94\x03\x12\x16\n\x11QueryStillRunning\x10\x95\x03\x12\x14\n\x0fQueryNotRunning\x10\x96\x03\x12\x17\n\x12QueryNotTerminated\x10\x97\x03\x12\x1b\n\x16QueryAlreadyTerminated\x10\x98\x03\x12\x11\n\x0cViewNotFound\x10\xf4\x03\x12\x0f\n\nViewExists\x10\xf5\x03\x12\x13\n\x0eViewInvalidSQL\x10\xf6\x03\x12 \n\x1bViewInvalidObjectIdentifier\x10\xf7\x03\x12\x16\n\x11\x43onnectorNotFound\x10\xd8\x04\x12\x14\n\x0f\x43onnectorExists\x10\xd9\x04\x12\x19\n\x14\x43onnectorInvalidType\x10\xda\x04\x12%\n ConnectorInvalidObjectIdentifier\x10\xdb\x04\x12\x19\n\x14\x43onnectorCheckFailed\x10\xdc\x04\x12\x1b\n\x16\x43onnectorUnimplemented\x10\xdd\x04\x12\x1b\n\x16\x43onnectorInvalidStatus\x10\xde\x04\x12\x10\n\x0bWrongServer\x10\xa0\x06\x12\'\n\"ShardReaderInvalidObjectIdentifier\x10\x84\x07\x12\x1e\n\x19ShardReaderConflictOffset\x10\x85\x07\x12\x1d\n\x18ShardReaderTooManyShards\x10\x86\x07\x32\x8a*\n\nHStreamApi\x12\x41\n\x04\x45\x63ho\x12\x1b.hstream.server.EchoRequest\x1a\x1c.hstream.server.EchoResponse\x12@\n\x0c\x43reateStream\x12\x16.hstream.server.Stream\x1a\x16.hstream.server.Stream\"\x00\x12M\n\x0c\x44\x65leteStream\x12#.hstream.server.DeleteStreamRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\nTrimStream\x12!.hstream.server.TrimStreamRequest\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\tGetStream\x12 .hstream.server.GetStreamRequest\x1a!.hstream.server.GetStreamResponse\"\x00\x12X\n\x0bListStreams\x12\".hstream.server.ListStreamsRequest\x1a#.hstream.server.ListStreamsResponse\"\x00\x12l\n\x15ListStreamsWithPrefix\x12,.hstream.server.ListStreamsWithPrefixRequest\x1a#.hstream.server.ListStreamsResponse\"\x00\x12X\n\x0bLookupShard\x12\".hstream.server.LookupShardRequest\x1a#.hstream.server.LookupShardResponse\"\x00\x12I\n\x06\x41ppend\x12\x1d.hstream.server.AppendRequest\x1a\x1e.hstream.server.AppendResponse\"\x00\x12\x64\n\x0fGetTailRecordId\x12&.hstream.server.GetTailRecordIdRequest\x1a\'.hstream.server.GetTailRecordIdResponse\"\x00\x12U\n\nListShards\x12!.hstream.server.ListShardsRequest\x1a\".hstream.server.ListShardsResponse\"\x00\x12G\n\tTrimShard\x12 .hstream.server.TrimShardRequest\x1a\x16.google.protobuf.Empty\"\x00\x12j\n\x11\x43reateShardReader\x12(.hstream.server.CreateShardReaderRequest\x1a).hstream.server.CreateShardReaderResponse\"\x00\x12j\n\x11LookupShardReader\x12(.hstream.server.LookupShardReaderRequest\x1a).hstream.server.LookupShardReaderResponse\"\x00\x12R\n\tReadShard\x12 .hstream.server.ReadShardRequest\x1a!.hstream.server.ReadShardResponse\"\x00\x12\x66\n\x0fReadShardStream\x12&.hstream.server.ReadShardStreamRequest\x1a\'.hstream.server.ReadShardStreamResponse\"\x00\x30\x01\x12g\n\x10ListShardReaders\x12\'.hstream.server.ListShardReadersRequest\x1a(.hstream.server.ListShardReadersResponse\"\x00\x12W\n\x11\x44\x65leteShardReader\x12(.hstream.server.DeleteShardReaderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\nReadStream\x12!.hstream.server.ReadStreamRequest\x1a\".hstream.server.ReadStreamResponse\"\x00\x30\x01\x12x\n\x15ReadSingleShardStream\x12,.hstream.server.ReadSingleShardStreamRequest\x1a-.hstream.server.ReadSingleShardStreamResponse\"\x00\x30\x01\x12R\n\x12\x43reateSubscription\x12\x1c.hstream.server.Subscription\x1a\x1c.hstream.server.Subscription\"\x00\x12\x64\n\x0fGetSubscription\x12&.hstream.server.GetSubscriptionRequest\x1a\'.hstream.server.GetSubscriptionResponse\"\x00\x12j\n\x11ListSubscriptions\x12(.hstream.server.ListSubscriptionsRequest\x1a).hstream.server.ListSubscriptionsResponse\"\x00\x12~\n\x1bListSubscriptionsWithPrefix\x12\x32.hstream.server.ListSubscriptionsWithPrefixRequest\x1a).hstream.server.ListSubscriptionsResponse\"\x00\x12^\n\rListConsumers\x12$.hstream.server.ListConsumersRequest\x1a%.hstream.server.ListConsumersResponse\"\x00\x12y\n\x16\x43heckSubscriptionExist\x12-.hstream.server.CheckSubscriptionExistRequest\x1a..hstream.server.CheckSubscriptionExistResponse\"\x00\x12Y\n\x12\x44\x65leteSubscription\x12).hstream.server.DeleteSubscriptionRequest\x1a\x16.google.protobuf.Empty\"\x00\x12m\n\x12LookupSubscription\x12).hstream.server.LookupSubscriptionRequest\x1a*.hstream.server.LookupSubscriptionResponse\"\x00\x12\x65\n\x0eStreamingFetch\x12%.hstream.server.StreamingFetchRequest\x1a&.hstream.server.StreamingFetchResponse\"\x00(\x01\x30\x01\x12T\n\x0f\x44\x65scribeCluster\x12\x16.google.protobuf.Empty\x1a\'.hstream.server.DescribeClusterResponse\"\x00\x12U\n\x0eLookupResource\x12%.hstream.server.LookupResourceRequest\x1a\x1a.hstream.server.ServerNode\"\x00\x12]\n\x10SendAdminCommand\x12#.hstream.server.AdminCommandRequest\x1a$.hstream.server.AdminCommandResponse\x12}\n\x18PerStreamTimeSeriesStats\x12/.hstream.server.PerStreamTimeSeriesStatsRequest\x1a\x30.hstream.server.PerStreamTimeSeriesStatsResponse\x12\x86\x01\n\x1bPerStreamTimeSeriesStatsAll\x12\x32.hstream.server.PerStreamTimeSeriesStatsAllRequest\x1a\x33.hstream.server.PerStreamTimeSeriesStatsAllResponse\x12M\n\x08GetStats\x12\x1f.hstream.server.GetStatsRequest\x1a .hstream.server.GetStatsResponse\x12R\n\x0c\x45xecuteQuery\x12\x1c.hstream.server.CommandQuery\x1a$.hstream.server.CommandQueryResponse\x12J\n\x0b\x43reateQuery\x12\".hstream.server.CreateQueryRequest\x1a\x15.hstream.server.Query\"\x00\x12\x64\n\x18\x43reateQueryWithNamespace\x12/.hstream.server.CreateQueryWithNamespaceRequest\x1a\x15.hstream.server.Query\"\x00\x12X\n\x0bListQueries\x12\".hstream.server.ListQueriesRequest\x1a#.hstream.server.ListQueriesResponse\"\x00\x12\x44\n\x08GetQuery\x12\x1f.hstream.server.GetQueryRequest\x1a\x15.hstream.server.Query\"\x00\x12Q\n\x0eTerminateQuery\x12%.hstream.server.TerminateQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12K\n\x0b\x44\x65leteQuery\x12\".hstream.server.DeleteQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12K\n\x0bResumeQuery\x12\".hstream.server.ResumeQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\nPauseQuery\x12!.hstream.server.PauseQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x08ParseSql\x12\x1f.hstream.server.ParseSqlRequest\x1a .hstream.server.ParseSqlResponse\"\x00\x12V\n\x0f\x43reateConnector\x12&.hstream.server.CreateConnectorRequest\x1a\x19.hstream.server.Connector\"\x00\x12\x61\n\x0eListConnectors\x12%.hstream.server.ListConnectorsRequest\x1a&.hstream.server.ListConnectorsResponse\"\x00\x12P\n\x0cGetConnector\x12#.hstream.server.GetConnectorRequest\x1a\x19.hstream.server.Connector\"\x00\x12g\n\x10GetConnectorSpec\x12\'.hstream.server.GetConnectorSpecRequest\x1a(.hstream.server.GetConnectorSpecResponse\"\x00\x12g\n\x10GetConnectorLogs\x12\'.hstream.server.GetConnectorLogsRequest\x1a(.hstream.server.GetConnectorLogsResponse\"\x00\x12S\n\x0f\x44\x65leteConnector\x12&.hstream.server.DeleteConnectorRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x0ePauseConnector\x12%.hstream.server.PauseConnectorRequest\x1a\x16.google.protobuf.Empty\"\x00\x12S\n\x0fResumeConnector\x12&.hstream.server.ResumeConnectorRequest\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\tListViews\x12 .hstream.server.ListViewsRequest\x1a!.hstream.server.ListViewsResponse\"\x00\x12\x41\n\x07GetView\x12\x1e.hstream.server.GetViewRequest\x1a\x14.hstream.server.View\"\x00\x12I\n\nDeleteView\x12!.hstream.server.DeleteViewRequest\x1a\x16.google.protobuf.Empty\"\x00\x12g\n\x10\x45xecuteViewQuery\x12\'.hstream.server.ExecuteViewQueryRequest\x1a(.hstream.server.ExecuteViewQueryResponse\"\x00\x12\x81\x01\n\x1d\x45xecuteViewQueryWithNamespace\x12\x34.hstream.server.ExecuteViewQueryWithNamespaceRequest\x1a(.hstream.server.ExecuteViewQueryResponse\"\x00\x42?\n\x13io.hstream.internalB\x0cHStreamProtoP\x01Z\x18hstreamdb/hstream/serverb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fHStream/Server/HStreamApi.proto\x12\x0ehstream.server\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\"@\n\x0fTimestampOffset\x12\x15\n\rtimestampInMs\x18\x01 \x01(\x03\x12\x16\n\x0estrictAccuracy\x18\x02 \x01(\x08\"\xbd\x01\n\x0bShardOffset\x12\x36\n\rspecialOffset\x18\x01 \x01(\x0e\x32\x1d.hstream.server.SpecialOffsetH\x00\x12\x30\n\x0crecordOffset\x18\x02 \x01(\x0b\x32\x18.hstream.server.RecordIdH\x00\x12:\n\x0ftimestampOffset\x18\x03 \x01(\x0b\x32\x1f.hstream.server.TimestampOffsetH\x00\x42\x08\n\x06offset\"\x1a\n\x0b\x45\x63hoRequest\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\x1b\n\x0c\x45\x63hoResponse\x12\x0b\n\x03msg\x18\x01 \x01(\t\"(\n\x11\x43ommandStreamTask\x12\x13\n\x0b\x63ommand_sql\x18\x01 \x01(\t\"1\n\x19\x43ommandStreamTaskResponse\x12\x14\n\x0c\x63ommand_resp\x18\x01 \x01(\t\"B\n\x0e\x43ommandConnect\x12\x16\n\x0e\x63lient_version\x18\x01 \x01(\t\x12\x18\n\x10protocol_version\x18\x02 \x01(\x05\"D\n\x10\x43ommandConnected\x12\x16\n\x0eserver_version\x18\x01 \x01(\t\x12\x18\n\x10protocol_version\x18\x02 \x01(\x05\"!\n\x0c\x43ommandQuery\x12\x11\n\tstmt_text\x18\x01 \x01(\t\"C\n\x14\x43ommandQueryResponse\x12+\n\nresult_set\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct\" \n\x10GetStreamRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\";\n\x11GetStreamResponse\x12&\n\x06stream\x18\x01 \x01(\x0b\x32\x16.hstream.server.Stream\"d\n\rAppendRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12.\n\x07records\x18\x03 \x01(\x0b\x32\x1d.hstream.server.BatchedRecord\"b\n\x0e\x41ppendResponse\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12+\n\trecordIds\x18\x03 \x03(\x0b\x32\x18.hstream.server.RecordId\"\xd1\x01\n\x0cSubscription\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12\x19\n\x11\x61\x63kTimeoutSeconds\x18\x03 \x01(\x05\x12\x19\n\x11maxUnackedRecords\x18\x04 \x01(\x05\x12-\n\x06offset\x18\x05 \x01(\x0e\x32\x1d.hstream.server.SpecialOffset\x12\x30\n\x0c\x63reationTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"6\n\x12SubscriptionOffset\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\x12\x0f\n\x07\x62\x61tchId\x18\x02 \x01(\x04\"$\n\x16GetSubscriptionRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x82\x01\n\x17GetSubscriptionResponse\x12\x32\n\x0csubscription\x18\x01 \x01(\x0b\x32\x1c.hstream.server.Subscription\x12\x33\n\x07offsets\x18\x02 \x03(\x0b\x32\".hstream.server.SubscriptionOffset\"B\n\x19\x44\x65leteSubscriptionRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"7\n\x1d\x43heckSubscriptionExistRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\"0\n\x1e\x43heckSubscriptionExistResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\"o\n\x15StreamingFetchRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12\x14\n\x0c\x63onsumerName\x18\x02 \x01(\t\x12(\n\x06\x61\x63kIds\x18\x03 \x03(\x0b\x32\x18.hstream.server.RecordId\"Q\n\x16StreamingFetchResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x01(\x0b\x32\x1e.hstream.server.ReceivedRecord\"l\n\x0eReceivedRecord\x12+\n\trecordIds\x18\x01 \x03(\x0b\x32\x18.hstream.server.RecordId\x12-\n\x06record\x18\x02 \x01(\x0b\x32\x1d.hstream.server.BatchedRecord\"P\n\x13\x44\x65leteStreamRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x16\n\x0eignoreNonExist\x18\x02 \x01(\x08\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\">\n\x13ListStreamsResponse\x12\'\n\x07streams\x18\x01 \x03(\x0b\x32\x16.hstream.server.Stream\"\x14\n\x12ListStreamsRequest\".\n\x1cListStreamsWithPrefixRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\"\x1a\n\x18ListSubscriptionsRequest\"4\n\"ListSubscriptionsWithPrefixRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\"O\n\x19ListSubscriptionsResponse\x12\x32\n\x0csubscription\x18\x01 \x03(\x0b\x32\x1c.hstream.server.Subscription\".\n\x14ListConsumersRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\"D\n\x15ListConsumersResponse\x12+\n\tconsumers\x18\x01 \x03(\x0b\x32\x18.hstream.server.Consumer\"X\n\x11TrimStreamRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12/\n\ttrimPoint\x18\x02 \x01(\x0b\x32\x1c.hstream.server.StreamOffset\"\x96\x01\n\x06Stream\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x19\n\x11replicationFactor\x18\x02 \x01(\r\x12\x17\n\x0f\x62\x61\x63klogDuration\x18\x03 \x01(\r\x12\x12\n\nshardCount\x18\x04 \x01(\r\x12\x30\n\x0c\x63reationTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9e\x01\n\rBatchedRecord\x12\x38\n\x0f\x63ompressionType\x18\x01 \x01(\x0e\x32\x1f.hstream.server.CompressionType\x12/\n\x0bpublishTime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tbatchSize\x18\x03 \x01(\r\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\"U\n\rHStreamRecord\x12\x33\n\x06header\x18\x01 \x01(\x0b\x32#.hstream.server.HStreamRecordHeader\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"E\n\x13\x42\x61tchHStreamRecords\x12.\n\x07records\x18\x01 \x03(\x0b\x32\x1d.hstream.server.HStreamRecord\"\xf1\x01\n\x13HStreamRecordHeader\x12\x36\n\x04\x66lag\x18\x01 \x01(\x0e\x32(.hstream.server.HStreamRecordHeader.Flag\x12G\n\nattributes\x18\x02 \x03(\x0b\x32\x33.hstream.server.HStreamRecordHeader.AttributesEntry\x12\x0b\n\x03key\x18\x03 \x01(\t\x1a\x31\n\x0f\x41ttributesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x19\n\x04\x46lag\x12\x08\n\x04JSON\x10\x00\x12\x07\n\x03RAW\x10\x01\"@\n\x08RecordId\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\x12\x0f\n\x07\x62\x61tchId\x18\x02 \x01(\x04\x12\x12\n\nbatchIndex\x18\x03 \x01(\r\"\x81\x01\n\x05Shard\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12\x19\n\x11startHashRangeKey\x18\x03 \x01(\t\x12\x17\n\x0f\x65ndHashRangeKey\x18\x04 \x01(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\x04\x12\x10\n\x08isActive\x18\x06 \x01(\x08\"\'\n\x11ListShardsRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\";\n\x12ListShardsResponse\x12%\n\x06shards\x18\x01 \x03(\x0b\x32\x15.hstream.server.Shard\"g\n\x10TrimShardRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12.\n\ttrimPoint\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\"\x94\x01\n\x18\x43reateShardReaderRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12\x30\n\x0bshardOffset\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x10\n\x08readerId\x18\x04 \x01(\t\x12\x0f\n\x07timeout\x18\x05 \x01(\r\"\x95\x01\n\x19\x43reateShardReaderResponse\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12\x30\n\x0bshardOffset\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x10\n\x08readerId\x18\x04 \x01(\t\x12\x0f\n\x07timeout\x18\x05 \x01(\r\"8\n\x10ReadShardRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x12\n\nmaxRecords\x18\x02 \x01(\r\",\n\x18\x44\x65leteShardReaderRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\"L\n\x11ReadShardResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"\x19\n\x17ListShardReadersRequest\",\n\x18ListShardReadersResponse\x12\x10\n\x08readerId\x18\x01 \x03(\t\"\xaa\x01\n\x16ReadShardStreamRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\x12)\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x16\n\x0emaxReadBatches\x18\x04 \x01(\x04\x12*\n\x05until\x18\x05 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\"R\n\x17ReadShardStreamResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"\x8c\x01\n\x0cStreamOffset\x12\x36\n\rspecialOffset\x18\x01 \x01(\x0e\x32\x1d.hstream.server.SpecialOffsetH\x00\x12:\n\x0ftimestampOffset\x18\x02 \x01(\x0b\x32\x1f.hstream.server.TimestampOffsetH\x00\x42\x08\n\x06offset\"\xaa\x01\n\x11ReadStreamRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12*\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1c.hstream.server.StreamOffset\x12+\n\x05until\x18\x04 \x01(\x0b\x32\x1c.hstream.server.StreamOffset\x12\x16\n\x0emaxReadBatches\x18\x05 \x01(\x04\"M\n\x12ReadStreamResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"\xbb\x01\n\x16ReadStreamByKeyRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12)\n\x04\x66rom\x18\x04 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12*\n\x05until\x18\x05 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x17\n\x0freadRecordCount\x18\x06 \x01(\x04\"~\n\x17ReadStreamByKeyResponse\x12+\n\trecordIds\x18\x01 \x03(\x0b\x32\x18.hstream.server.RecordId\x12\x36\n\x0freceivedRecords\x18\x02 \x03(\x0b\x32\x1d.hstream.server.HStreamRecord\"\xb3\x01\n\x1cReadSingleShardStreamRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12)\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12*\n\x05until\x18\x04 \x01(\x0b\x32\x1b.hstream.server.ShardOffset\x12\x16\n\x0emaxReadBatches\x18\x05 \x01(\x04\"X\n\x1dReadSingleShardStreamResponse\x12\x37\n\x0freceivedRecords\x18\x01 \x03(\x0b\x32\x1e.hstream.server.ReceivedRecord\"(\n\x15TerminateQueryRequest\x12\x0f\n\x07queryId\x18\x01 \x01(\t\"4\n\x12\x43reateQueryRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x11\n\tqueryName\x18\x02 \x01(\t\"T\n\x1f\x43reateQueryWithNamespaceRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x11\n\tqueryName\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\"\x14\n\x12ListQueriesRequest\"=\n\x13ListQueriesResponse\x12&\n\x07queries\x18\x01 \x03(\x0b\x32\x15.hstream.server.Query\"\x1d\n\x0fGetQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\"8\n\x08\x43onsumer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x11\n\tuserAgent\x18\x03 \x01(\t\"\xc7\x01\n\x05Query\x12\n\n\x02id\x18\x01 \x01(\t\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x1c.hstream.server.TaskStatusPB\x12\x13\n\x0b\x63reatedTime\x18\x03 \x01(\x03\x12\x11\n\tqueryText\x18\x04 \x01(\t\x12\x0f\n\x07sources\x18\x05 \x03(\t\x12\x12\n\nresultName\x18\x06 \x01(\t\x12\'\n\x04type\x18\x07 \x01(\x0e\x32\x19.hstream.server.QueryType\x12\x0e\n\x06nodeId\x18\x08 \x01(\r\" \n\x12\x44\x65leteQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x12ResumeQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1f\n\x11PauseQueryRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1e\n\x0fParseSqlRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\"P\n\x10ParseSqlResponse\x12\x35\n\x06\x65vqSql\x18\x01 \x01(\x0b\x32#.hstream.server.ExecuteViewQuerySqlH\x00\x42\x05\n\x03sql\"`\n\rColumnCatalog\x12\r\n\x05index\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x12\n\nisNullable\x18\x04 \x01(\x08\x12\x10\n\x08isHidden\x18\x05 \x01(\x08\"G\n\x06Schema\x12\r\n\x05owner\x18\x01 \x01(\t\x12.\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x1d.hstream.server.ColumnCatalog\"!\n\x10GetSchemaRequest\x12\r\n\x05owner\x18\x01 \x01(\t\"(\n\x17UnregisterSchemaRequest\x12\r\n\x05owner\x18\x01 \x01(\t\"#\n\x13\x45xecuteViewQuerySql\x12\x0c\n\x04view\x18\x01 \x01(\t\"T\n\x16\x43reateConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0e\n\x06target\x18\x03 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x04 \x01(\t\"\x17\n\x15ListConnectorsRequest\"G\n\x16ListConnectorsResponse\x12-\n\nconnectors\x18\x01 \x03(\x0b\x32\x19.hstream.server.Connector\"#\n\x13GetConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"7\n\x17GetConnectorSpecRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06target\x18\x02 \x01(\t\"(\n\x18GetConnectorSpecResponse\x12\x0c\n\x04spec\x18\x01 \x01(\t\"E\n\x17GetConnectorLogsRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\"(\n\x18GetConnectorLogsResponse\x12\x0c\n\x04logs\x18\x01 \x01(\t\"\xf6\x01\n\tConnector\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0e\n\x06target\x18\x03 \x01(\t\x12\x30\n\x0c\x63reationTime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x06 \x01(\t\x12(\n\x07offsets\x18\x07 \x03(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06taskId\x18\x08 \x01(\t\x12\x0c\n\x04node\x18\t \x01(\t\x12\x14\n\x0c\x64ockerStatus\x18\n \x01(\t\x12\r\n\x05image\x18\x0b \x01(\t\"&\n\x16\x44\x65leteConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"%\n\x15PauseConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"&\n\x16ResumeConnectorRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\" \n\x0eGetViewRequest\x12\x0e\n\x06viewId\x18\x01 \x01(\t\";\n\x11\x44\x65leteViewRequest\x12\x0e\n\x06viewId\x18\x01 \x01(\t\x12\x16\n\x0eignoreNonExist\x18\x02 \x01(\x08\"\x12\n\x10ListViewsRequest\"8\n\x11ListViewsResponse\x12#\n\x05views\x18\x01 \x03(\x0b\x32\x14.hstream.server.View\"\x89\x01\n\x04View\x12\x0e\n\x06viewId\x18\x01 \x01(\t\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x1c.hstream.server.TaskStatusPB\x12\x13\n\x0b\x63reatedTime\x18\x03 \x01(\x03\x12\x0b\n\x03sql\x18\x04 \x01(\t\x12\x0e\n\x06schema\x18\x05 \x03(\t\x12\x11\n\tqueryName\x18\x06 \x01(\t\"D\n\x18\x45xecuteViewQueryResponse\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct\"&\n\x17\x45xecuteViewQueryRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\"F\n$ExecuteViewQueryWithNamespaceRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\"&\n\x11StatsIntervalVals\x12\x11\n\tintervals\x18\x01 \x03(\x05\"\x1f\n\x0fStatsDoubleVals\x12\x0c\n\x04vals\x18\x01 \x03(\x01\"&\n\x13\x41\x64minCommandRequest\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\"&\n\x14\x41\x64minCommandResponse\x12\x0e\n\x06result\x18\x01 \x01(\t\"{\n\x1fPerStreamTimeSeriesStatsRequest\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x12\n\nstreamName\x18\x02 \x01(\t\x12\x34\n\tintervals\x18\x03 \x01(\x0b\x32!.hstream.server.StatsIntervalVals\"R\n PerStreamTimeSeriesStatsResponse\x12.\n\x05stats\x18\x01 \x01(\x0b\x32\x1f.hstream.server.StatsDoubleVals\"\xc3\x01\n#PerStreamTimeSeriesStatsAllResponse\x12M\n\x05stats\x18\x01 \x03(\x0b\x32>.hstream.server.PerStreamTimeSeriesStatsAllResponse.StatsEntry\x1aM\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.hstream.server.StatsDoubleVals:\x02\x38\x01\"j\n\"PerStreamTimeSeriesStatsAllRequest\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x34\n\tintervals\x18\x02 \x01(\x0b\x32!.hstream.server.StatsIntervalVals\"\xb7\x01\n\x17\x44\x65scribeClusterResponse\x12\x17\n\x0fprotocolVersion\x18\x01 \x01(\t\x12/\n\x0bserverNodes\x18\x02 \x03(\x0b\x32\x1a.hstream.server.ServerNode\x12;\n\x11serverNodesStatus\x18\x03 \x03(\x0b\x32 .hstream.server.ServerNodeStatus\x12\x15\n\rclusterUpTime\x18\x04 \x01(\x04\"e\n\nServerNode\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\x12/\n\x07version\x18\x04 \x01(\x0b\x32\x1e.hstream.server.HStreamVersion\"f\n\x10ServerNodeStatus\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x1a.hstream.server.ServerNode\x12(\n\x05state\x18\x02 \x01(\x0e\x32\x19.hstream.server.NodeState\"1\n\x0eHStreamVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x02 \x01(\t\"%\n\x12LookupShardRequest\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\"V\n\x13LookupShardResponse\x12\x0f\n\x07shardId\x18\x01 \x01(\x04\x12.\n\nserverNode\x18\x02 \x01(\x0b\x32\x1a.hstream.server.ServerNode\"3\n\x19LookupSubscriptionRequest\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\"d\n\x1aLookupSubscriptionResponse\x12\x16\n\x0esubscriptionId\x18\x01 \x01(\t\x12.\n\nserverNode\x18\x02 \x01(\x0b\x32\x1a.hstream.server.ServerNode\",\n\x18LookupShardReaderRequest\x12\x10\n\x08readerId\x18\x01 \x01(\t\"]\n\x19LookupShardReaderResponse\x12\x10\n\x08readerId\x18\x01 \x01(\t\x12.\n\nserverNode\x18\x02 \x01(\x0b\x32\x1a.hstream.server.ServerNode\"U\n\x15LookupResourceRequest\x12-\n\x07resType\x18\x01 \x01(\x0e\x32\x1c.hstream.server.ResourceType\x12\r\n\x05resId\x18\x02 \x01(\t\"(\n\x10LookupKeyRequest\x12\x14\n\x0cpartitionKey\x18\x01 \x01(\t\"=\n\x16GetTailRecordIdRequest\x12\x12\n\nstreamName\x18\x01 \x01(\t\x12\x0f\n\x07shardId\x18\x02 \x01(\x04\"I\n\x17GetTailRecordIdResponse\x12.\n\x0ctailRecordId\x18\x01 \x01(\x0b\x32\x18.hstream.server.RecordId\"\x8f\x02\n\x08StatType\x12\x31\n\nstreamStat\x18\x01 \x01(\x0e\x32\x1b.hstream.server.StreamStatsH\x00\x12\x34\n\x07subStat\x18\x02 \x01(\x0e\x32!.hstream.server.SubscriptionStatsH\x00\x12\x32\n\x08\x63onnStat\x18\x03 \x01(\x0e\x32\x1e.hstream.server.ConnectorStatsH\x00\x12/\n\tqueryStat\x18\x04 \x01(\x0e\x32\x1a.hstream.server.QueryStatsH\x00\x12-\n\x08viewStat\x18\x05 \x01(\x0e\x32\x19.hstream.server.ViewStatsH\x00\x42\x06\n\x04stat\"\xa9\x01\n\tStatValue\x12*\n\x08statType\x18\x01 \x01(\x0b\x32\x18.hstream.server.StatType\x12=\n\nstatValues\x18\x02 \x03(\x0b\x32).hstream.server.StatValue.StatValuesEntry\x1a\x31\n\x0fStatValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"H\n\tStatError\x12*\n\x08statType\x18\x01 \x01(\x0b\x32\x18.hstream.server.StatType\x12\x0f\n\x07message\x18\x02 \x01(\t\":\n\x0fGetStatsRequest\x12\'\n\x05stats\x18\x01 \x03(\x0b\x32\x18.hstream.server.StatType\"m\n\x10GetStatsResponse\x12.\n\x0bstatsValues\x18\x01 \x03(\x0b\x32\x19.hstream.server.StatValue\x12)\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x19.hstream.server.StatError*)\n\rSpecialOffset\x12\x0c\n\x08\x45\x41RLIEST\x10\x00\x12\n\n\x06LATEST\x10\x01*/\n\x0f\x43ompressionType\x12\x08\n\x04None\x10\x00\x12\x08\n\x04Gzip\x10\x01\x12\x08\n\x04Zstd\x10\x02*\x90\x01\n\x0cTaskStatusPB\x12\x11\n\rTASK_CREATING\x10\x00\x12\x10\n\x0cTASK_RUNNING\x10\x01\x12\x10\n\x0cTASK_ABORTED\x10\x02\x12\x0f\n\x0bTASK_PAUSED\x10\x03\x12\x11\n\rTASK_RESUMING\x10\x04\x12\x13\n\x0fTASK_TERMINATED\x10\x05\x12\x10\n\x0cTASK_UNKNOWN\x10\x06*1\n\tQueryType\x12\x12\n\x0e\x43reateStreamAs\x10\x00\x12\x10\n\x0c\x43reateViewAs\x10\x01*A\n\tNodeState\x12\x0c\n\x08Starting\x10\x00\x12\x0b\n\x07Running\x10\x01\x12\x0f\n\x0bUnavailable\x10\x02\x12\x08\n\x04\x44\x65\x61\x64\x10\x03*\x81\x01\n\x0cResourceType\x12\r\n\tResStream\x10\x00\x12\x13\n\x0fResSubscription\x10\x01\x12\x0c\n\x08ResShard\x10\x02\x12\x12\n\x0eResShardReader\x10\x03\x12\x10\n\x0cResConnector\x10\x04\x12\x0c\n\x08ResQuery\x10\x05\x12\x0b\n\x07ResView\x10\x06*X\n\x0bStreamStats\x12\x11\n\rAppendInBytes\x10\x00\x12\x13\n\x0f\x41ppendInRecords\x10\x01\x12\x0f\n\x0b\x41ppendTotal\x10\x02\x12\x10\n\x0c\x41ppendFailed\x10\x03*\xcf\x01\n\x11SubscriptionStats\x12\x10\n\x0cSendOutBytes\x10\x00\x12\x12\n\x0eSendOutRecords\x10\x01\x12\x18\n\x14SendOutRecordsFailed\x10\x02\x12\x11\n\rResendRecords\x10\x03\x12\x17\n\x13ResendRecordsFailed\x10\x04\x12\x10\n\x0cReceivedAcks\x10\x05\x12\x13\n\x0fRequestMessages\x10\x06\x12\x14\n\x10ResponseMessages\x10\x07\x12\x11\n\rChecklistSize\x10\x08*>\n\x0e\x43onnectorStats\x12\x16\n\x12\x44\x65liveredInRecords\x10\x00\x12\x14\n\x10\x44\x65liveredInBytes\x10\x01*S\n\nQueryStats\x12\x15\n\x11TotalInputRecords\x10\x00\x12\x16\n\x12TotalOutputRecords\x10\x01\x12\x16\n\x12TotalExecuteErrors\x10\x02*$\n\tViewStats\x12\x17\n\x13TotalExecuteQueries\x10\x00*\xed\x08\n\tErrorCode\x12\x11\n\rInternalError\x10\x00\x12\x13\n\x0eStreamNotFound\x10\xc8\x01\x12\x11\n\x0cStreamExists\x10\xc9\x01\x12\x1c\n\x17StreamFoundSubscription\x10\xca\x01\x12\x1f\n\x1aStreamInvalidReplicaFactor\x10\xcb\x01\x12\"\n\x1dStreamInvalidObjectIdentifier\x10\xcc\x01\x12\x1c\n\x17StreamInvalidShardCount\x10\xcd\x01\x12\x1d\n\x18StreamEmptyBatchedRecord\x10\xce\x01\x12\x1c\n\x17StreamInvalidRecordSize\x10\xcf\x01\x12\x18\n\x13StreamInvalidOffset\x10\xd0\x01\x12\x19\n\x14SubscriptionNotFound\x10\xac\x02\x12\x17\n\x12SubscriptionExists\x10\xad\x02\x12,\n\'SubscriptionCreationOnNonExistentStream\x10\xae\x02\x12\x1e\n\x19SubscriptionInvalidOffset\x10\xaf\x02\x12(\n#SubscriptionInvalidObjectIdentifier\x10\xb0\x02\x12%\n SubscriptionFoundActiveConsumers\x10\xb1\x02\x12\x12\n\rQueryNotFound\x10\x90\x03\x12\x10\n\x0bQueryExists\x10\x91\x03\x12\x14\n\x0fQueryInvalidSQL\x10\x92\x03\x12\x1d\n\x18QueryFoundAssociatedView\x10\x93\x03\x12!\n\x1cQueryInvalidObjectIdentifier\x10\x94\x03\x12\x16\n\x11QueryStillRunning\x10\x95\x03\x12\x14\n\x0fQueryNotRunning\x10\x96\x03\x12\x17\n\x12QueryNotTerminated\x10\x97\x03\x12\x1b\n\x16QueryAlreadyTerminated\x10\x98\x03\x12\x11\n\x0cViewNotFound\x10\xf4\x03\x12\x0f\n\nViewExists\x10\xf5\x03\x12\x13\n\x0eViewInvalidSQL\x10\xf6\x03\x12 \n\x1bViewInvalidObjectIdentifier\x10\xf7\x03\x12\x16\n\x11\x43onnectorNotFound\x10\xd8\x04\x12\x14\n\x0f\x43onnectorExists\x10\xd9\x04\x12\x19\n\x14\x43onnectorInvalidType\x10\xda\x04\x12%\n ConnectorInvalidObjectIdentifier\x10\xdb\x04\x12\x19\n\x14\x43onnectorCheckFailed\x10\xdc\x04\x12\x1b\n\x16\x43onnectorUnimplemented\x10\xdd\x04\x12\x1b\n\x16\x43onnectorInvalidStatus\x10\xde\x04\x12\x10\n\x0bWrongServer\x10\xa0\x06\x12\'\n\"ShardReaderInvalidObjectIdentifier\x10\x84\x07\x12\x1e\n\x19ShardReaderConflictOffset\x10\x85\x07\x12\x1d\n\x18ShardReaderTooManyShards\x10\x86\x07\x32\xa5-\n\nHStreamApi\x12\x41\n\x04\x45\x63ho\x12\x1b.hstream.server.EchoRequest\x1a\x1c.hstream.server.EchoResponse\x12@\n\x0c\x43reateStream\x12\x16.hstream.server.Stream\x1a\x16.hstream.server.Stream\"\x00\x12M\n\x0c\x44\x65leteStream\x12#.hstream.server.DeleteStreamRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\nTrimStream\x12!.hstream.server.TrimStreamRequest\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\tGetStream\x12 .hstream.server.GetStreamRequest\x1a!.hstream.server.GetStreamResponse\"\x00\x12X\n\x0bListStreams\x12\".hstream.server.ListStreamsRequest\x1a#.hstream.server.ListStreamsResponse\"\x00\x12l\n\x15ListStreamsWithPrefix\x12,.hstream.server.ListStreamsWithPrefixRequest\x1a#.hstream.server.ListStreamsResponse\"\x00\x12X\n\x0bLookupShard\x12\".hstream.server.LookupShardRequest\x1a#.hstream.server.LookupShardResponse\"\x00\x12I\n\x06\x41ppend\x12\x1d.hstream.server.AppendRequest\x1a\x1e.hstream.server.AppendResponse\"\x00\x12\x64\n\x0fGetTailRecordId\x12&.hstream.server.GetTailRecordIdRequest\x1a\'.hstream.server.GetTailRecordIdResponse\"\x00\x12U\n\nListShards\x12!.hstream.server.ListShardsRequest\x1a\".hstream.server.ListShardsResponse\"\x00\x12G\n\tTrimShard\x12 .hstream.server.TrimShardRequest\x1a\x16.google.protobuf.Empty\"\x00\x12j\n\x11\x43reateShardReader\x12(.hstream.server.CreateShardReaderRequest\x1a).hstream.server.CreateShardReaderResponse\"\x00\x12j\n\x11LookupShardReader\x12(.hstream.server.LookupShardReaderRequest\x1a).hstream.server.LookupShardReaderResponse\"\x00\x12R\n\tReadShard\x12 .hstream.server.ReadShardRequest\x1a!.hstream.server.ReadShardResponse\"\x00\x12\x66\n\x0fReadShardStream\x12&.hstream.server.ReadShardStreamRequest\x1a\'.hstream.server.ReadShardStreamResponse\"\x00\x30\x01\x12g\n\x10ListShardReaders\x12\'.hstream.server.ListShardReadersRequest\x1a(.hstream.server.ListShardReadersResponse\"\x00\x12W\n\x11\x44\x65leteShardReader\x12(.hstream.server.DeleteShardReaderRequest\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\nReadStream\x12!.hstream.server.ReadStreamRequest\x1a\".hstream.server.ReadStreamResponse\"\x00\x30\x01\x12x\n\x15ReadSingleShardStream\x12,.hstream.server.ReadSingleShardStreamRequest\x1a-.hstream.server.ReadSingleShardStreamResponse\"\x00\x30\x01\x12h\n\x0fReadStreamByKey\x12&.hstream.server.ReadStreamByKeyRequest\x1a\'.hstream.server.ReadStreamByKeyResponse\"\x00(\x01\x30\x01\x12R\n\x12\x43reateSubscription\x12\x1c.hstream.server.Subscription\x1a\x1c.hstream.server.Subscription\"\x00\x12\x64\n\x0fGetSubscription\x12&.hstream.server.GetSubscriptionRequest\x1a\'.hstream.server.GetSubscriptionResponse\"\x00\x12j\n\x11ListSubscriptions\x12(.hstream.server.ListSubscriptionsRequest\x1a).hstream.server.ListSubscriptionsResponse\"\x00\x12~\n\x1bListSubscriptionsWithPrefix\x12\x32.hstream.server.ListSubscriptionsWithPrefixRequest\x1a).hstream.server.ListSubscriptionsResponse\"\x00\x12^\n\rListConsumers\x12$.hstream.server.ListConsumersRequest\x1a%.hstream.server.ListConsumersResponse\"\x00\x12y\n\x16\x43heckSubscriptionExist\x12-.hstream.server.CheckSubscriptionExistRequest\x1a..hstream.server.CheckSubscriptionExistResponse\"\x00\x12Y\n\x12\x44\x65leteSubscription\x12).hstream.server.DeleteSubscriptionRequest\x1a\x16.google.protobuf.Empty\"\x00\x12m\n\x12LookupSubscription\x12).hstream.server.LookupSubscriptionRequest\x1a*.hstream.server.LookupSubscriptionResponse\"\x00\x12\x65\n\x0eStreamingFetch\x12%.hstream.server.StreamingFetchRequest\x1a&.hstream.server.StreamingFetchResponse\"\x00(\x01\x30\x01\x12T\n\x0f\x44\x65scribeCluster\x12\x16.google.protobuf.Empty\x1a\'.hstream.server.DescribeClusterResponse\"\x00\x12U\n\x0eLookupResource\x12%.hstream.server.LookupResourceRequest\x1a\x1a.hstream.server.ServerNode\"\x00\x12K\n\tLookupKey\x12 .hstream.server.LookupKeyRequest\x1a\x1a.hstream.server.ServerNode\"\x00\x12]\n\x10SendAdminCommand\x12#.hstream.server.AdminCommandRequest\x1a$.hstream.server.AdminCommandResponse\x12}\n\x18PerStreamTimeSeriesStats\x12/.hstream.server.PerStreamTimeSeriesStatsRequest\x1a\x30.hstream.server.PerStreamTimeSeriesStatsResponse\x12\x86\x01\n\x1bPerStreamTimeSeriesStatsAll\x12\x32.hstream.server.PerStreamTimeSeriesStatsAllRequest\x1a\x33.hstream.server.PerStreamTimeSeriesStatsAllResponse\x12M\n\x08GetStats\x12\x1f.hstream.server.GetStatsRequest\x1a .hstream.server.GetStatsResponse\x12R\n\x0c\x45xecuteQuery\x12\x1c.hstream.server.CommandQuery\x1a$.hstream.server.CommandQueryResponse\x12J\n\x0b\x43reateQuery\x12\".hstream.server.CreateQueryRequest\x1a\x15.hstream.server.Query\"\x00\x12\x64\n\x18\x43reateQueryWithNamespace\x12/.hstream.server.CreateQueryWithNamespaceRequest\x1a\x15.hstream.server.Query\"\x00\x12X\n\x0bListQueries\x12\".hstream.server.ListQueriesRequest\x1a#.hstream.server.ListQueriesResponse\"\x00\x12\x44\n\x08GetQuery\x12\x1f.hstream.server.GetQueryRequest\x1a\x15.hstream.server.Query\"\x00\x12Q\n\x0eTerminateQuery\x12%.hstream.server.TerminateQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12K\n\x0b\x44\x65leteQuery\x12\".hstream.server.DeleteQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12K\n\x0bResumeQuery\x12\".hstream.server.ResumeQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\nPauseQuery\x12!.hstream.server.PauseQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x08ParseSql\x12\x1f.hstream.server.ParseSqlRequest\x1a .hstream.server.ParseSqlResponse\"\x00\x12\x42\n\x0eRegisterSchema\x12\x16.hstream.server.Schema\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\tGetSchema\x12 .hstream.server.GetSchemaRequest\x1a\x16.hstream.server.Schema\"\x00\x12U\n\x10UnregisterSchema\x12\'.hstream.server.UnregisterSchemaRequest\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x0f\x43reateConnector\x12&.hstream.server.CreateConnectorRequest\x1a\x19.hstream.server.Connector\"\x00\x12\x61\n\x0eListConnectors\x12%.hstream.server.ListConnectorsRequest\x1a&.hstream.server.ListConnectorsResponse\"\x00\x12P\n\x0cGetConnector\x12#.hstream.server.GetConnectorRequest\x1a\x19.hstream.server.Connector\"\x00\x12g\n\x10GetConnectorSpec\x12\'.hstream.server.GetConnectorSpecRequest\x1a(.hstream.server.GetConnectorSpecResponse\"\x00\x12g\n\x10GetConnectorLogs\x12\'.hstream.server.GetConnectorLogsRequest\x1a(.hstream.server.GetConnectorLogsResponse\"\x00\x12S\n\x0f\x44\x65leteConnector\x12&.hstream.server.DeleteConnectorRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x0ePauseConnector\x12%.hstream.server.PauseConnectorRequest\x1a\x16.google.protobuf.Empty\"\x00\x12S\n\x0fResumeConnector\x12&.hstream.server.ResumeConnectorRequest\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\tListViews\x12 .hstream.server.ListViewsRequest\x1a!.hstream.server.ListViewsResponse\"\x00\x12\x41\n\x07GetView\x12\x1e.hstream.server.GetViewRequest\x1a\x14.hstream.server.View\"\x00\x12I\n\nDeleteView\x12!.hstream.server.DeleteViewRequest\x1a\x16.google.protobuf.Empty\"\x00\x12g\n\x10\x45xecuteViewQuery\x12\'.hstream.server.ExecuteViewQueryRequest\x1a(.hstream.server.ExecuteViewQueryResponse\"\x00\x12\x81\x01\n\x1d\x45xecuteViewQueryWithNamespace\x12\x34.hstream.server.ExecuteViewQueryWithNamespaceRequest\x1a(.hstream.server.ExecuteViewQueryResponse\"\x00\x42?\n\x13io.hstream.internalB\x0cHStreamProtoP\x01Z\x18hstreamdb/hstream/serverb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'HStream.Server.HStreamApi_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023io.hstream.internalB\014HStreamProtoP\001Z\030hstreamdb/hstream/server'
   _HSTREAMRECORDHEADER_ATTRIBUTESENTRY._options = None
   _HSTREAMRECORDHEADER_ATTRIBUTESENTRY._serialized_options = b'8\001'
   _PERSTREAMTIMESERIESSTATSALLRESPONSE_STATSENTRY._options = None
   _PERSTREAMTIMESERIESSTATSALLRESPONSE_STATSENTRY._serialized_options = b'8\001'
   _STATVALUE_STATVALUESENTRY._options = None
   _STATVALUE_STATVALUESENTRY._serialized_options = b'8\001'
-  _globals['_SPECIALOFFSET']._serialized_start=9757
-  _globals['_SPECIALOFFSET']._serialized_end=9798
-  _globals['_COMPRESSIONTYPE']._serialized_start=9800
-  _globals['_COMPRESSIONTYPE']._serialized_end=9847
-  _globals['_TASKSTATUSPB']._serialized_start=9850
-  _globals['_TASKSTATUSPB']._serialized_end=9994
-  _globals['_QUERYTYPE']._serialized_start=9996
-  _globals['_QUERYTYPE']._serialized_end=10045
-  _globals['_NODESTATE']._serialized_start=10047
-  _globals['_NODESTATE']._serialized_end=10112
-  _globals['_RESOURCETYPE']._serialized_start=10115
-  _globals['_RESOURCETYPE']._serialized_end=10244
-  _globals['_STREAMSTATS']._serialized_start=10246
-  _globals['_STREAMSTATS']._serialized_end=10334
-  _globals['_SUBSCRIPTIONSTATS']._serialized_start=10337
-  _globals['_SUBSCRIPTIONSTATS']._serialized_end=10544
-  _globals['_CONNECTORSTATS']._serialized_start=10546
-  _globals['_CONNECTORSTATS']._serialized_end=10608
-  _globals['_QUERYSTATS']._serialized_start=10610
-  _globals['_QUERYSTATS']._serialized_end=10693
-  _globals['_VIEWSTATS']._serialized_start=10695
-  _globals['_VIEWSTATS']._serialized_end=10731
-  _globals['_ERRORCODE']._serialized_start=10734
-  _globals['_ERRORCODE']._serialized_end=11867
+  _globals['_SPECIALOFFSET']._serialized_start=10365
+  _globals['_SPECIALOFFSET']._serialized_end=10406
+  _globals['_COMPRESSIONTYPE']._serialized_start=10408
+  _globals['_COMPRESSIONTYPE']._serialized_end=10455
+  _globals['_TASKSTATUSPB']._serialized_start=10458
+  _globals['_TASKSTATUSPB']._serialized_end=10602
+  _globals['_QUERYTYPE']._serialized_start=10604
+  _globals['_QUERYTYPE']._serialized_end=10653
+  _globals['_NODESTATE']._serialized_start=10655
+  _globals['_NODESTATE']._serialized_end=10720
+  _globals['_RESOURCETYPE']._serialized_start=10723
+  _globals['_RESOURCETYPE']._serialized_end=10852
+  _globals['_STREAMSTATS']._serialized_start=10854
+  _globals['_STREAMSTATS']._serialized_end=10942
+  _globals['_SUBSCRIPTIONSTATS']._serialized_start=10945
+  _globals['_SUBSCRIPTIONSTATS']._serialized_end=11152
+  _globals['_CONNECTORSTATS']._serialized_start=11154
+  _globals['_CONNECTORSTATS']._serialized_end=11216
+  _globals['_QUERYSTATS']._serialized_start=11218
+  _globals['_QUERYSTATS']._serialized_end=11301
+  _globals['_VIEWSTATS']._serialized_start=11303
+  _globals['_VIEWSTATS']._serialized_end=11339
+  _globals['_ERRORCODE']._serialized_start=11342
+  _globals['_ERRORCODE']._serialized_end=12475
   _globals['_TIMESTAMPOFFSET']._serialized_start=143
   _globals['_TIMESTAMPOFFSET']._serialized_end=207
   _globals['_SHARDOFFSET']._serialized_start=210
   _globals['_SHARDOFFSET']._serialized_end=399
   _globals['_ECHOREQUEST']._serialized_start=401
   _globals['_ECHOREQUEST']._serialized_end=427
   _globals['_ECHORESPONSE']._serialized_start=429
@@ -167,138 +167,152 @@
   _globals['_READSHARDSTREAMRESPONSE']._serialized_end=4531
   _globals['_STREAMOFFSET']._serialized_start=4534
   _globals['_STREAMOFFSET']._serialized_end=4674
   _globals['_READSTREAMREQUEST']._serialized_start=4677
   _globals['_READSTREAMREQUEST']._serialized_end=4847
   _globals['_READSTREAMRESPONSE']._serialized_start=4849
   _globals['_READSTREAMRESPONSE']._serialized_end=4926
-  _globals['_READSINGLESHARDSTREAMREQUEST']._serialized_start=4929
-  _globals['_READSINGLESHARDSTREAMREQUEST']._serialized_end=5108
-  _globals['_READSINGLESHARDSTREAMRESPONSE']._serialized_start=5110
-  _globals['_READSINGLESHARDSTREAMRESPONSE']._serialized_end=5198
-  _globals['_TERMINATEQUERYREQUEST']._serialized_start=5200
-  _globals['_TERMINATEQUERYREQUEST']._serialized_end=5240
-  _globals['_CREATEQUERYREQUEST']._serialized_start=5242
-  _globals['_CREATEQUERYREQUEST']._serialized_end=5294
-  _globals['_CREATEQUERYWITHNAMESPACEREQUEST']._serialized_start=5296
-  _globals['_CREATEQUERYWITHNAMESPACEREQUEST']._serialized_end=5380
-  _globals['_LISTQUERIESREQUEST']._serialized_start=5382
-  _globals['_LISTQUERIESREQUEST']._serialized_end=5402
-  _globals['_LISTQUERIESRESPONSE']._serialized_start=5404
-  _globals['_LISTQUERIESRESPONSE']._serialized_end=5465
-  _globals['_GETQUERYREQUEST']._serialized_start=5467
-  _globals['_GETQUERYREQUEST']._serialized_end=5496
-  _globals['_CONSUMER']._serialized_start=5498
-  _globals['_CONSUMER']._serialized_end=5554
-  _globals['_QUERY']._serialized_start=5557
-  _globals['_QUERY']._serialized_end=5756
-  _globals['_DELETEQUERYREQUEST']._serialized_start=5758
-  _globals['_DELETEQUERYREQUEST']._serialized_end=5790
-  _globals['_RESUMEQUERYREQUEST']._serialized_start=5792
-  _globals['_RESUMEQUERYREQUEST']._serialized_end=5824
-  _globals['_PAUSEQUERYREQUEST']._serialized_start=5826
-  _globals['_PAUSEQUERYREQUEST']._serialized_end=5857
-  _globals['_PARSESQLREQUEST']._serialized_start=5859
-  _globals['_PARSESQLREQUEST']._serialized_end=5889
-  _globals['_PARSESQLRESPONSE']._serialized_start=5891
-  _globals['_PARSESQLRESPONSE']._serialized_end=5971
-  _globals['_EXECUTEVIEWQUERYSQL']._serialized_start=5973
-  _globals['_EXECUTEVIEWQUERYSQL']._serialized_end=6008
-  _globals['_CREATECONNECTORREQUEST']._serialized_start=6010
-  _globals['_CREATECONNECTORREQUEST']._serialized_end=6094
-  _globals['_LISTCONNECTORSREQUEST']._serialized_start=6096
-  _globals['_LISTCONNECTORSREQUEST']._serialized_end=6119
-  _globals['_LISTCONNECTORSRESPONSE']._serialized_start=6121
-  _globals['_LISTCONNECTORSRESPONSE']._serialized_end=6192
-  _globals['_GETCONNECTORREQUEST']._serialized_start=6194
-  _globals['_GETCONNECTORREQUEST']._serialized_end=6229
-  _globals['_GETCONNECTORSPECREQUEST']._serialized_start=6231
-  _globals['_GETCONNECTORSPECREQUEST']._serialized_end=6286
-  _globals['_GETCONNECTORSPECRESPONSE']._serialized_start=6288
-  _globals['_GETCONNECTORSPECRESPONSE']._serialized_end=6328
-  _globals['_GETCONNECTORLOGSREQUEST']._serialized_start=6330
-  _globals['_GETCONNECTORLOGSREQUEST']._serialized_end=6399
-  _globals['_GETCONNECTORLOGSRESPONSE']._serialized_start=6401
-  _globals['_GETCONNECTORLOGSRESPONSE']._serialized_end=6441
-  _globals['_CONNECTOR']._serialized_start=6444
-  _globals['_CONNECTOR']._serialized_end=6690
-  _globals['_DELETECONNECTORREQUEST']._serialized_start=6692
-  _globals['_DELETECONNECTORREQUEST']._serialized_end=6730
-  _globals['_PAUSECONNECTORREQUEST']._serialized_start=6732
-  _globals['_PAUSECONNECTORREQUEST']._serialized_end=6769
-  _globals['_RESUMECONNECTORREQUEST']._serialized_start=6771
-  _globals['_RESUMECONNECTORREQUEST']._serialized_end=6809
-  _globals['_GETVIEWREQUEST']._serialized_start=6811
-  _globals['_GETVIEWREQUEST']._serialized_end=6843
-  _globals['_DELETEVIEWREQUEST']._serialized_start=6845
-  _globals['_DELETEVIEWREQUEST']._serialized_end=6904
-  _globals['_LISTVIEWSREQUEST']._serialized_start=6906
-  _globals['_LISTVIEWSREQUEST']._serialized_end=6924
-  _globals['_LISTVIEWSRESPONSE']._serialized_start=6926
-  _globals['_LISTVIEWSRESPONSE']._serialized_end=6982
-  _globals['_VIEW']._serialized_start=6985
-  _globals['_VIEW']._serialized_end=7122
-  _globals['_EXECUTEVIEWQUERYRESPONSE']._serialized_start=7124
-  _globals['_EXECUTEVIEWQUERYRESPONSE']._serialized_end=7192
-  _globals['_EXECUTEVIEWQUERYREQUEST']._serialized_start=7194
-  _globals['_EXECUTEVIEWQUERYREQUEST']._serialized_end=7232
-  _globals['_EXECUTEVIEWQUERYWITHNAMESPACEREQUEST']._serialized_start=7234
-  _globals['_EXECUTEVIEWQUERYWITHNAMESPACEREQUEST']._serialized_end=7304
-  _globals['_STATSINTERVALVALS']._serialized_start=7306
-  _globals['_STATSINTERVALVALS']._serialized_end=7344
-  _globals['_STATSDOUBLEVALS']._serialized_start=7346
-  _globals['_STATSDOUBLEVALS']._serialized_end=7377
-  _globals['_ADMINCOMMANDREQUEST']._serialized_start=7379
-  _globals['_ADMINCOMMANDREQUEST']._serialized_end=7417
-  _globals['_ADMINCOMMANDRESPONSE']._serialized_start=7419
-  _globals['_ADMINCOMMANDRESPONSE']._serialized_end=7457
-  _globals['_PERSTREAMTIMESERIESSTATSREQUEST']._serialized_start=7459
-  _globals['_PERSTREAMTIMESERIESSTATSREQUEST']._serialized_end=7582
-  _globals['_PERSTREAMTIMESERIESSTATSRESPONSE']._serialized_start=7584
-  _globals['_PERSTREAMTIMESERIESSTATSRESPONSE']._serialized_end=7666
-  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE']._serialized_start=7669
-  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE']._serialized_end=7864
-  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE_STATSENTRY']._serialized_start=7787
-  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE_STATSENTRY']._serialized_end=7864
-  _globals['_PERSTREAMTIMESERIESSTATSALLREQUEST']._serialized_start=7866
-  _globals['_PERSTREAMTIMESERIESSTATSALLREQUEST']._serialized_end=7972
-  _globals['_DESCRIBECLUSTERRESPONSE']._serialized_start=7975
-  _globals['_DESCRIBECLUSTERRESPONSE']._serialized_end=8158
-  _globals['_SERVERNODE']._serialized_start=8160
-  _globals['_SERVERNODE']._serialized_end=8261
-  _globals['_SERVERNODESTATUS']._serialized_start=8263
-  _globals['_SERVERNODESTATUS']._serialized_end=8365
-  _globals['_HSTREAMVERSION']._serialized_start=8367
-  _globals['_HSTREAMVERSION']._serialized_end=8416
-  _globals['_LOOKUPSHARDREQUEST']._serialized_start=8418
-  _globals['_LOOKUPSHARDREQUEST']._serialized_end=8455
-  _globals['_LOOKUPSHARDRESPONSE']._serialized_start=8457
-  _globals['_LOOKUPSHARDRESPONSE']._serialized_end=8543
-  _globals['_LOOKUPSUBSCRIPTIONREQUEST']._serialized_start=8545
-  _globals['_LOOKUPSUBSCRIPTIONREQUEST']._serialized_end=8596
-  _globals['_LOOKUPSUBSCRIPTIONRESPONSE']._serialized_start=8598
-  _globals['_LOOKUPSUBSCRIPTIONRESPONSE']._serialized_end=8698
-  _globals['_LOOKUPSHARDREADERREQUEST']._serialized_start=8700
-  _globals['_LOOKUPSHARDREADERREQUEST']._serialized_end=8744
-  _globals['_LOOKUPSHARDREADERRESPONSE']._serialized_start=8746
-  _globals['_LOOKUPSHARDREADERRESPONSE']._serialized_end=8839
-  _globals['_LOOKUPRESOURCEREQUEST']._serialized_start=8841
-  _globals['_LOOKUPRESOURCEREQUEST']._serialized_end=8926
-  _globals['_GETTAILRECORDIDREQUEST']._serialized_start=8928
-  _globals['_GETTAILRECORDIDREQUEST']._serialized_end=8989
-  _globals['_GETTAILRECORDIDRESPONSE']._serialized_start=8991
-  _globals['_GETTAILRECORDIDRESPONSE']._serialized_end=9064
-  _globals['_STATTYPE']._serialized_start=9067
-  _globals['_STATTYPE']._serialized_end=9338
-  _globals['_STATVALUE']._serialized_start=9341
-  _globals['_STATVALUE']._serialized_end=9510
-  _globals['_STATVALUE_STATVALUESENTRY']._serialized_start=9461
-  _globals['_STATVALUE_STATVALUESENTRY']._serialized_end=9510
-  _globals['_STATERROR']._serialized_start=9512
-  _globals['_STATERROR']._serialized_end=9584
-  _globals['_GETSTATSREQUEST']._serialized_start=9586
-  _globals['_GETSTATSREQUEST']._serialized_end=9644
-  _globals['_GETSTATSRESPONSE']._serialized_start=9646
-  _globals['_GETSTATSRESPONSE']._serialized_end=9755
-  _globals['_HSTREAMAPI']._serialized_start=11870
-  _globals['_HSTREAMAPI']._serialized_end=17256
+  _globals['_READSTREAMBYKEYREQUEST']._serialized_start=4929
+  _globals['_READSTREAMBYKEYREQUEST']._serialized_end=5116
+  _globals['_READSTREAMBYKEYRESPONSE']._serialized_start=5118
+  _globals['_READSTREAMBYKEYRESPONSE']._serialized_end=5244
+  _globals['_READSINGLESHARDSTREAMREQUEST']._serialized_start=5247
+  _globals['_READSINGLESHARDSTREAMREQUEST']._serialized_end=5426
+  _globals['_READSINGLESHARDSTREAMRESPONSE']._serialized_start=5428
+  _globals['_READSINGLESHARDSTREAMRESPONSE']._serialized_end=5516
+  _globals['_TERMINATEQUERYREQUEST']._serialized_start=5518
+  _globals['_TERMINATEQUERYREQUEST']._serialized_end=5558
+  _globals['_CREATEQUERYREQUEST']._serialized_start=5560
+  _globals['_CREATEQUERYREQUEST']._serialized_end=5612
+  _globals['_CREATEQUERYWITHNAMESPACEREQUEST']._serialized_start=5614
+  _globals['_CREATEQUERYWITHNAMESPACEREQUEST']._serialized_end=5698
+  _globals['_LISTQUERIESREQUEST']._serialized_start=5700
+  _globals['_LISTQUERIESREQUEST']._serialized_end=5720
+  _globals['_LISTQUERIESRESPONSE']._serialized_start=5722
+  _globals['_LISTQUERIESRESPONSE']._serialized_end=5783
+  _globals['_GETQUERYREQUEST']._serialized_start=5785
+  _globals['_GETQUERYREQUEST']._serialized_end=5814
+  _globals['_CONSUMER']._serialized_start=5816
+  _globals['_CONSUMER']._serialized_end=5872
+  _globals['_QUERY']._serialized_start=5875
+  _globals['_QUERY']._serialized_end=6074
+  _globals['_DELETEQUERYREQUEST']._serialized_start=6076
+  _globals['_DELETEQUERYREQUEST']._serialized_end=6108
+  _globals['_RESUMEQUERYREQUEST']._serialized_start=6110
+  _globals['_RESUMEQUERYREQUEST']._serialized_end=6142
+  _globals['_PAUSEQUERYREQUEST']._serialized_start=6144
+  _globals['_PAUSEQUERYREQUEST']._serialized_end=6175
+  _globals['_PARSESQLREQUEST']._serialized_start=6177
+  _globals['_PARSESQLREQUEST']._serialized_end=6207
+  _globals['_PARSESQLRESPONSE']._serialized_start=6209
+  _globals['_PARSESQLRESPONSE']._serialized_end=6289
+  _globals['_COLUMNCATALOG']._serialized_start=6291
+  _globals['_COLUMNCATALOG']._serialized_end=6387
+  _globals['_SCHEMA']._serialized_start=6389
+  _globals['_SCHEMA']._serialized_end=6460
+  _globals['_GETSCHEMAREQUEST']._serialized_start=6462
+  _globals['_GETSCHEMAREQUEST']._serialized_end=6495
+  _globals['_UNREGISTERSCHEMAREQUEST']._serialized_start=6497
+  _globals['_UNREGISTERSCHEMAREQUEST']._serialized_end=6537
+  _globals['_EXECUTEVIEWQUERYSQL']._serialized_start=6539
+  _globals['_EXECUTEVIEWQUERYSQL']._serialized_end=6574
+  _globals['_CREATECONNECTORREQUEST']._serialized_start=6576
+  _globals['_CREATECONNECTORREQUEST']._serialized_end=6660
+  _globals['_LISTCONNECTORSREQUEST']._serialized_start=6662
+  _globals['_LISTCONNECTORSREQUEST']._serialized_end=6685
+  _globals['_LISTCONNECTORSRESPONSE']._serialized_start=6687
+  _globals['_LISTCONNECTORSRESPONSE']._serialized_end=6758
+  _globals['_GETCONNECTORREQUEST']._serialized_start=6760
+  _globals['_GETCONNECTORREQUEST']._serialized_end=6795
+  _globals['_GETCONNECTORSPECREQUEST']._serialized_start=6797
+  _globals['_GETCONNECTORSPECREQUEST']._serialized_end=6852
+  _globals['_GETCONNECTORSPECRESPONSE']._serialized_start=6854
+  _globals['_GETCONNECTORSPECRESPONSE']._serialized_end=6894
+  _globals['_GETCONNECTORLOGSREQUEST']._serialized_start=6896
+  _globals['_GETCONNECTORLOGSREQUEST']._serialized_end=6965
+  _globals['_GETCONNECTORLOGSRESPONSE']._serialized_start=6967
+  _globals['_GETCONNECTORLOGSRESPONSE']._serialized_end=7007
+  _globals['_CONNECTOR']._serialized_start=7010
+  _globals['_CONNECTOR']._serialized_end=7256
+  _globals['_DELETECONNECTORREQUEST']._serialized_start=7258
+  _globals['_DELETECONNECTORREQUEST']._serialized_end=7296
+  _globals['_PAUSECONNECTORREQUEST']._serialized_start=7298
+  _globals['_PAUSECONNECTORREQUEST']._serialized_end=7335
+  _globals['_RESUMECONNECTORREQUEST']._serialized_start=7337
+  _globals['_RESUMECONNECTORREQUEST']._serialized_end=7375
+  _globals['_GETVIEWREQUEST']._serialized_start=7377
+  _globals['_GETVIEWREQUEST']._serialized_end=7409
+  _globals['_DELETEVIEWREQUEST']._serialized_start=7411
+  _globals['_DELETEVIEWREQUEST']._serialized_end=7470
+  _globals['_LISTVIEWSREQUEST']._serialized_start=7472
+  _globals['_LISTVIEWSREQUEST']._serialized_end=7490
+  _globals['_LISTVIEWSRESPONSE']._serialized_start=7492
+  _globals['_LISTVIEWSRESPONSE']._serialized_end=7548
+  _globals['_VIEW']._serialized_start=7551
+  _globals['_VIEW']._serialized_end=7688
+  _globals['_EXECUTEVIEWQUERYRESPONSE']._serialized_start=7690
+  _globals['_EXECUTEVIEWQUERYRESPONSE']._serialized_end=7758
+  _globals['_EXECUTEVIEWQUERYREQUEST']._serialized_start=7760
+  _globals['_EXECUTEVIEWQUERYREQUEST']._serialized_end=7798
+  _globals['_EXECUTEVIEWQUERYWITHNAMESPACEREQUEST']._serialized_start=7800
+  _globals['_EXECUTEVIEWQUERYWITHNAMESPACEREQUEST']._serialized_end=7870
+  _globals['_STATSINTERVALVALS']._serialized_start=7872
+  _globals['_STATSINTERVALVALS']._serialized_end=7910
+  _globals['_STATSDOUBLEVALS']._serialized_start=7912
+  _globals['_STATSDOUBLEVALS']._serialized_end=7943
+  _globals['_ADMINCOMMANDREQUEST']._serialized_start=7945
+  _globals['_ADMINCOMMANDREQUEST']._serialized_end=7983
+  _globals['_ADMINCOMMANDRESPONSE']._serialized_start=7985
+  _globals['_ADMINCOMMANDRESPONSE']._serialized_end=8023
+  _globals['_PERSTREAMTIMESERIESSTATSREQUEST']._serialized_start=8025
+  _globals['_PERSTREAMTIMESERIESSTATSREQUEST']._serialized_end=8148
+  _globals['_PERSTREAMTIMESERIESSTATSRESPONSE']._serialized_start=8150
+  _globals['_PERSTREAMTIMESERIESSTATSRESPONSE']._serialized_end=8232
+  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE']._serialized_start=8235
+  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE']._serialized_end=8430
+  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE_STATSENTRY']._serialized_start=8353
+  _globals['_PERSTREAMTIMESERIESSTATSALLRESPONSE_STATSENTRY']._serialized_end=8430
+  _globals['_PERSTREAMTIMESERIESSTATSALLREQUEST']._serialized_start=8432
+  _globals['_PERSTREAMTIMESERIESSTATSALLREQUEST']._serialized_end=8538
+  _globals['_DESCRIBECLUSTERRESPONSE']._serialized_start=8541
+  _globals['_DESCRIBECLUSTERRESPONSE']._serialized_end=8724
+  _globals['_SERVERNODE']._serialized_start=8726
+  _globals['_SERVERNODE']._serialized_end=8827
+  _globals['_SERVERNODESTATUS']._serialized_start=8829
+  _globals['_SERVERNODESTATUS']._serialized_end=8931
+  _globals['_HSTREAMVERSION']._serialized_start=8933
+  _globals['_HSTREAMVERSION']._serialized_end=8982
+  _globals['_LOOKUPSHARDREQUEST']._serialized_start=8984
+  _globals['_LOOKUPSHARDREQUEST']._serialized_end=9021
+  _globals['_LOOKUPSHARDRESPONSE']._serialized_start=9023
+  _globals['_LOOKUPSHARDRESPONSE']._serialized_end=9109
+  _globals['_LOOKUPSUBSCRIPTIONREQUEST']._serialized_start=9111
+  _globals['_LOOKUPSUBSCRIPTIONREQUEST']._serialized_end=9162
+  _globals['_LOOKUPSUBSCRIPTIONRESPONSE']._serialized_start=9164
+  _globals['_LOOKUPSUBSCRIPTIONRESPONSE']._serialized_end=9264
+  _globals['_LOOKUPSHARDREADERREQUEST']._serialized_start=9266
+  _globals['_LOOKUPSHARDREADERREQUEST']._serialized_end=9310
+  _globals['_LOOKUPSHARDREADERRESPONSE']._serialized_start=9312
+  _globals['_LOOKUPSHARDREADERRESPONSE']._serialized_end=9405
+  _globals['_LOOKUPRESOURCEREQUEST']._serialized_start=9407
+  _globals['_LOOKUPRESOURCEREQUEST']._serialized_end=9492
+  _globals['_LOOKUPKEYREQUEST']._serialized_start=9494
+  _globals['_LOOKUPKEYREQUEST']._serialized_end=9534
+  _globals['_GETTAILRECORDIDREQUEST']._serialized_start=9536
+  _globals['_GETTAILRECORDIDREQUEST']._serialized_end=9597
+  _globals['_GETTAILRECORDIDRESPONSE']._serialized_start=9599
+  _globals['_GETTAILRECORDIDRESPONSE']._serialized_end=9672
+  _globals['_STATTYPE']._serialized_start=9675
+  _globals['_STATTYPE']._serialized_end=9946
+  _globals['_STATVALUE']._serialized_start=9949
+  _globals['_STATVALUE']._serialized_end=10118
+  _globals['_STATVALUE_STATVALUESENTRY']._serialized_start=10069
+  _globals['_STATVALUE_STATVALUESENTRY']._serialized_end=10118
+  _globals['_STATERROR']._serialized_start=10120
+  _globals['_STATERROR']._serialized_end=10192
+  _globals['_GETSTATSREQUEST']._serialized_start=10194
+  _globals['_GETSTATSREQUEST']._serialized_end=10252
+  _globals['_GETSTATSRESPONSE']._serialized_start=10254
+  _globals['_GETSTATSRESPONSE']._serialized_end=10363
+  _globals['_HSTREAMAPI']._serialized_start=12478
+  _globals['_HSTREAMAPI']._serialized_end=18275
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hstreamdb-api-0.6.0/src/HStream/Server/HStreamApi_pb2_grpc.py` & `hstreamdb-api-0.6.1/src/HStream/Server/HStreamApi_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,19 @@
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamResponse.FromString,
                 )
         self.ReadSingleShardStream = channel.unary_stream(
                 '/hstream.server.HStreamApi/ReadSingleShardStream',
                 request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadSingleShardStreamRequest.SerializeToString,
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadSingleShardStreamResponse.FromString,
                 )
+        self.ReadStreamByKey = channel.stream_stream(
+                '/hstream.server.HStreamApi/ReadStreamByKey',
+                request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamByKeyRequest.SerializeToString,
+                response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamByKeyResponse.FromString,
+                )
         self.CreateSubscription = channel.unary_unary(
                 '/hstream.server.HStreamApi/CreateSubscription',
                 request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.Subscription.SerializeToString,
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.Subscription.FromString,
                 )
         self.GetSubscription = channel.unary_unary(
                 '/hstream.server.HStreamApi/GetSubscription',
@@ -169,14 +174,19 @@
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.DescribeClusterResponse.FromString,
                 )
         self.LookupResource = channel.unary_unary(
                 '/hstream.server.HStreamApi/LookupResource',
                 request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.LookupResourceRequest.SerializeToString,
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ServerNode.FromString,
                 )
+        self.LookupKey = channel.unary_unary(
+                '/hstream.server.HStreamApi/LookupKey',
+                request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.LookupKeyRequest.SerializeToString,
+                response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ServerNode.FromString,
+                )
         self.SendAdminCommand = channel.unary_unary(
                 '/hstream.server.HStreamApi/SendAdminCommand',
                 request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.AdminCommandRequest.SerializeToString,
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.AdminCommandResponse.FromString,
                 )
         self.PerStreamTimeSeriesStats = channel.unary_unary(
                 '/hstream.server.HStreamApi/PerStreamTimeSeriesStats',
@@ -239,14 +249,29 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.ParseSql = channel.unary_unary(
                 '/hstream.server.HStreamApi/ParseSql',
                 request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ParseSqlRequest.SerializeToString,
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ParseSqlResponse.FromString,
                 )
+        self.RegisterSchema = channel.unary_unary(
+                '/hstream.server.HStreamApi/RegisterSchema',
+                request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.Schema.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.GetSchema = channel.unary_unary(
+                '/hstream.server.HStreamApi/GetSchema',
+                request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.GetSchemaRequest.SerializeToString,
+                response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.Schema.FromString,
+                )
+        self.UnregisterSchema = channel.unary_unary(
+                '/hstream.server.HStreamApi/UnregisterSchema',
+                request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.UnregisterSchemaRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
         self.CreateConnector = channel.unary_unary(
                 '/hstream.server.HStreamApi/CreateConnector',
                 request_serializer=HStream_dot_Server_dot_HStreamApi__pb2.CreateConnectorRequest.SerializeToString,
                 response_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.Connector.FromString,
                 )
         self.ListConnectors = channel.unary_unary(
                 '/hstream.server.HStreamApi/ListConnectors',
@@ -434,14 +459,20 @@
 
     def ReadSingleShardStream(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ReadStreamByKey(self, request_iterator, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def CreateSubscription(self, request, context):
         """Subscribe APIs
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -502,14 +533,20 @@
 
     def LookupResource(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def LookupKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SendAdminCommand(self, request, context):
         """Admin Command
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -596,14 +633,32 @@
     def ParseSql(self, request, context):
         """parse query sql, return structuralized information
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def RegisterSchema(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSchema(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UnregisterSchema(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def CreateConnector(self, request, context):
         """connector related apis
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -779,14 +834,19 @@
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamResponse.SerializeToString,
             ),
             'ReadSingleShardStream': grpc.unary_stream_rpc_method_handler(
                     servicer.ReadSingleShardStream,
                     request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadSingleShardStreamRequest.FromString,
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadSingleShardStreamResponse.SerializeToString,
             ),
+            'ReadStreamByKey': grpc.stream_stream_rpc_method_handler(
+                    servicer.ReadStreamByKey,
+                    request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamByKeyRequest.FromString,
+                    response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamByKeyResponse.SerializeToString,
+            ),
             'CreateSubscription': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateSubscription,
                     request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.Subscription.FromString,
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.Subscription.SerializeToString,
             ),
             'GetSubscription': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSubscription,
@@ -834,14 +894,19 @@
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.DescribeClusterResponse.SerializeToString,
             ),
             'LookupResource': grpc.unary_unary_rpc_method_handler(
                     servicer.LookupResource,
                     request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.LookupResourceRequest.FromString,
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ServerNode.SerializeToString,
             ),
+            'LookupKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.LookupKey,
+                    request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.LookupKeyRequest.FromString,
+                    response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ServerNode.SerializeToString,
+            ),
             'SendAdminCommand': grpc.unary_unary_rpc_method_handler(
                     servicer.SendAdminCommand,
                     request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.AdminCommandRequest.FromString,
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.AdminCommandResponse.SerializeToString,
             ),
             'PerStreamTimeSeriesStats': grpc.unary_unary_rpc_method_handler(
                     servicer.PerStreamTimeSeriesStats,
@@ -904,14 +969,29 @@
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'ParseSql': grpc.unary_unary_rpc_method_handler(
                     servicer.ParseSql,
                     request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.ParseSqlRequest.FromString,
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.ParseSqlResponse.SerializeToString,
             ),
+            'RegisterSchema': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterSchema,
+                    request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.Schema.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'GetSchema': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSchema,
+                    request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.GetSchemaRequest.FromString,
+                    response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.Schema.SerializeToString,
+            ),
+            'UnregisterSchema': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterSchema,
+                    request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.UnregisterSchemaRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
             'CreateConnector': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateConnector,
                     request_deserializer=HStream_dot_Server_dot_HStreamApi__pb2.CreateConnectorRequest.FromString,
                     response_serializer=HStream_dot_Server_dot_HStreamApi__pb2.Connector.SerializeToString,
             ),
             'ListConnectors': grpc.unary_unary_rpc_method_handler(
                     servicer.ListConnectors,
@@ -1323,14 +1403,31 @@
         return grpc.experimental.unary_stream(request, target, '/hstream.server.HStreamApi/ReadSingleShardStream',
             HStream_dot_Server_dot_HStreamApi__pb2.ReadSingleShardStreamRequest.SerializeToString,
             HStream_dot_Server_dot_HStreamApi__pb2.ReadSingleShardStreamResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ReadStreamByKey(request_iterator,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_stream(request_iterator, target, '/hstream.server.HStreamApi/ReadStreamByKey',
+            HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamByKeyRequest.SerializeToString,
+            HStream_dot_Server_dot_HStreamApi__pb2.ReadStreamByKeyResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def CreateSubscription(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1510,14 +1607,31 @@
         return grpc.experimental.unary_unary(request, target, '/hstream.server.HStreamApi/LookupResource',
             HStream_dot_Server_dot_HStreamApi__pb2.LookupResourceRequest.SerializeToString,
             HStream_dot_Server_dot_HStreamApi__pb2.ServerNode.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def LookupKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/hstream.server.HStreamApi/LookupKey',
+            HStream_dot_Server_dot_HStreamApi__pb2.LookupKeyRequest.SerializeToString,
+            HStream_dot_Server_dot_HStreamApi__pb2.ServerNode.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SendAdminCommand(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1748,14 +1862,65 @@
         return grpc.experimental.unary_unary(request, target, '/hstream.server.HStreamApi/ParseSql',
             HStream_dot_Server_dot_HStreamApi__pb2.ParseSqlRequest.SerializeToString,
             HStream_dot_Server_dot_HStreamApi__pb2.ParseSqlResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def RegisterSchema(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/hstream.server.HStreamApi/RegisterSchema',
+            HStream_dot_Server_dot_HStreamApi__pb2.Schema.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSchema(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/hstream.server.HStreamApi/GetSchema',
+            HStream_dot_Server_dot_HStreamApi__pb2.GetSchemaRequest.SerializeToString,
+            HStream_dot_Server_dot_HStreamApi__pb2.Schema.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UnregisterSchema(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/hstream.server.HStreamApi/UnregisterSchema',
+            HStream_dot_Server_dot_HStreamApi__pb2.UnregisterSchemaRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def CreateConnector(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `hstreamdb-api-0.6.0/src/hstreamdb_api.egg-info/PKG-INFO` & `hstreamdb-api-0.6.1/src/hstreamdb_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstreamdb-api
-Version: 0.6.0
+Version: 0.6.1
 Summary: HStreamDB api for Python
 Home-page: https://github.com/hstreamdb/hstream
 Author: lambda
 Author-email: lambda@emqx.io
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hstreamdb/hstream/issues
 Description: # hstreamdb-api
```

