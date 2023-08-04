# Comparing `tmp/declearn-2.2.0.tar.gz` & `tmp/declearn-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declearn-2.2.0.tar", last modified: Thu May 11 14:38:00 2023, max compression
+gzip compressed data, was "declearn-2.2.1.tar", last modified: Fri Aug  4 08:52:56 2023, max compression
```

## Comparing `declearn-2.2.0.tar` & `declearn-2.2.1.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.838330 declearn-2.2.0/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1652 2023-05-04 10:01:14.000000 declearn-2.2.0/.gitlab-ci.yml
--rw-r--r--   0 paandrey (670133) magnet    (5235)      560 2023-04-26 13:33:08.000000 declearn-2.2.0/AUTHORS
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11357 2023-03-24 21:43:07.000000 declearn-2.2.0/LICENSE
--rw-r--r--   0 paandrey (670133) magnet    (5235)    19325 2023-05-11 14:38:00.838330 declearn-2.2.0/PKG-INFO
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4977 2023-05-04 10:01:14.000000 declearn-2.2.0/README.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2496 2023-05-10 13:11:18.000000 declearn-2.2.0/declearn/__init__.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/aggregator/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1705 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/aggregator/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5597 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/aggregator/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4167 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/aggregator/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4271 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/aggregator/_gma.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/communication/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3046 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8164 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/_build.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/communication/api/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1248 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     9146 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    13310 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/_server.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    16342 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/_service.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/communication/grpc/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1308 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/grpc/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4811 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8877 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/_server.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/communication/grpc/protobufs/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1398 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)      263 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/message.proto
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1841 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5239 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/communication/messaging/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2409 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/messaging/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6999 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/messaging/_messages.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1410 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/messaging/flags.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/communication/websockets/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1143 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/websockets/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5973 2023-03-31 13:39:10.000000 declearn-2.2.0/declearn/communication/websockets/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6514 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/websockets/_server.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3509 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/websockets/_tools.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/data_info/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2948 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/data_info/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8345 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/data_info/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7274 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/data_info/_fields.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/dataset/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2119 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6510 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/dataset/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    21645 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/_inmemory.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8307 2023-05-10 13:11:18.000000 declearn-2.2.0/declearn/dataset/_split_data.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/dataset/examples/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1053 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/examples/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3532 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/examples/_heart_uci.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3770 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/examples/_mnist.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/dataset/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1693 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4866 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/_save_load.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6022 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/_sparse.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7065 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/_split_classif.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2160 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    17375 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    28091 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/_server.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/config/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1739 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/config/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7695 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/config/_dataclasses.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5589 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/config/_run_config.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7888 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/main/config/_strategy.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/privacy/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      904 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/privacy/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10673 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/privacy/_dp_trainer.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2584 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    21365 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_checkpoint.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5064 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/main/utils/_constraints.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7442 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_data_info.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4007 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_early_stop.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    14134 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_training.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/metrics/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2861 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    12815 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8084 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_classif.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5249 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_mean.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11953 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_roc_auc.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5123 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_rsquared.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8185 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_wrapper.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/model/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2949 2023-05-10 12:36:04.000000 declearn-2.2.0/declearn/model/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1803 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/model/api/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1202 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/api/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11185 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/api/_model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15988 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/api/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/haiku/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1062 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/haiku/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    20958 2023-05-11 13:44:56.000000 declearn-2.2.0/declearn/model/haiku/_model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5742 2023-05-10 13:11:01.000000 declearn-2.2.0/declearn/model/haiku/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/haiku/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      857 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/haiku/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2751 2023-05-11 13:45:00.000000 declearn-2.2.0/declearn/model/haiku/utils/_gpu.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/sklearn/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1216 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/sklearn/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3957 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/sklearn/_np_vec.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15266 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/sklearn/_sgd.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/tensorflow/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1552 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15417 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/tensorflow/_model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10658 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/_optim.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10302 2023-05-10 13:11:01.000000 declearn-2.2.0/declearn/model/tensorflow/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/tensorflow/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1881 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4455 2023-05-11 13:45:00.000000 declearn-2.2.0/declearn/model/tensorflow/utils/_gpu.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4016 2023-03-27 10:07:29.000000 declearn-2.2.0/declearn/model/tensorflow/utils/_loss.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5360 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/utils/_slices.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/torch/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1474 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/torch/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    16535 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/torch/_model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    13026 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/torch/_optim.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6861 2023-05-10 13:11:01.000000 declearn-2.2.0/declearn/model/torch/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/torch/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1094 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/torch/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4641 2023-05-11 13:45:00.000000 declearn-2.2.0/declearn/model/torch/utils/_gpu.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/optimizer/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1711 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    19710 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3130 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/optimizer/modules/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2836 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11020 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_adaptive.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11323 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/modules/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2318 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_clipping.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6600 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_momentum.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6031 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/modules/_noise.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15038 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_scaffold.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/optimizer/regularizers/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1453 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/regularizers/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6166 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/regularizers/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3405 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/regularizers/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)        0 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/py.typed
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/quickrun/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1811 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/quickrun/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3938 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/quickrun/_config.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6652 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/quickrun/_parser.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     9386 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/quickrun/_run.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/declearn/test_utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1616 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/test_utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4704 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/test_utils/_argparse.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6683 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/test_utils/_assertions.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6040 2023-03-27 10:07:29.000000 declearn-2.2.0/declearn/test_utils/_gen_ssl.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1772 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/test_utils/_imports.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6524 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/test_utils/_vectors.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2096 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/typing.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/declearn/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5008 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7741 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/utils/_dataclass.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4174 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_device_policy.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7056 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_json.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2968 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_logging.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4938 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/utils/_multiprocess.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1575 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/utils/_numpy.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10530 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_register.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6342 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_serialize.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15250 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/utils/_toml_config.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn.egg-info/
--rw-r--r--   0 paandrey (670133) magnet    (5235)    19325 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/PKG-INFO
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6607 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/SOURCES.txt
--rw-r--r--   0 paandrey (670133) magnet    (5235)        1 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/dependency_links.txt
--rw-r--r--   0 paandrey (670133) magnet    (5235)      117 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/entry_points.txt
--rw-r--r--   0 paandrey (670133) magnet    (5235)      641 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/requires.txt
--rw-r--r--   0 paandrey (670133) magnet    (5235)        9 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/top_level.txt
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/docs/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      181 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/SUMMARY.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/docs/api-reference/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      416 2023-05-10 13:10:41.000000 declearn-2.2.0/docs/api-reference/index.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/docs/devs-guide/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      207 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/SUMMARY.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3650 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/contribute.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2930 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/docs-build.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10370 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/docs-style.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)      746 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/index.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6994 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/tests.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3884 2023-05-10 13:09:13.000000 declearn-2.2.0/docs/index.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)    12500 2023-05-10 13:11:18.000000 declearn-2.2.0/docs/quickstart.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4270 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/setup.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/docs/user-guide/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      230 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/SUMMARY.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4626 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/fl_process.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)      799 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/index.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4989 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/local_dp.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5087 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/package.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     9739 2023-05-11 13:53:19.000000 declearn-2.2.0/docs/user-guide/usage.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.806331 declearn-2.2.0/examples/
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/adding_rmsprop/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4600 2023-03-24 21:43:07.000000 declearn-2.2.0/examples/adding_rmsprop/readme.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/heart-uci/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3698 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/heart-uci/client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1642 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/heart-uci/data.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)      916 2023-03-24 21:43:07.000000 declearn-2.2.0/examples/heart-uci/gen_ssl.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4214 2023-04-26 13:33:08.000000 declearn-2.2.0/examples/heart-uci/readme.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2191 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/heart-uci/run.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4801 2023-04-26 13:33:08.000000 declearn-2.2.0/examples/heart-uci/server.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/mnist/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3826 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)      916 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/gen_ssl.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4882 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/readme.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2498 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/run.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5773 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/server.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/mnist_quickrun/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1628 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist_quickrun/config.toml
--rw-r--r--   0 paandrey (670133) magnet    (5235)    25127 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist_quickrun/mnist.ipynb
--rw-r--r--   0 paandrey (670133) magnet    (5235)      763 2023-05-11 14:00:17.000000 declearn-2.2.0/examples/mnist_quickrun/model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1167 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist_quickrun/readme.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1046 2023-05-04 10:01:14.000000 declearn-2.2.0/mkdocs.yml
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3586 2023-05-11 13:57:25.000000 declearn-2.2.0/pyproject.toml
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/scripts/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5402 2023-05-04 10:01:14.000000 declearn-2.2.0/scripts/gen_docs.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)       38 2023-05-11 14:38:00.838330 declearn-2.2.0/setup.cfg
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/aggregator/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3011 2023-05-10 12:05:04.000000 declearn-2.2.0/test/aggregator/test_aggregator.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/communication/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1680 2023-03-24 21:43:07.000000 declearn-2.2.0/test/communication/conftest.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     9311 2023-05-04 10:01:14.000000 declearn-2.2.0/test/communication/test_exchanges.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11813 2023-03-24 21:43:07.000000 declearn-2.2.0/test/communication/test_grpc.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    16395 2023-05-04 10:01:14.000000 declearn-2.2.0/test/communication/test_server.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1529 2023-05-04 10:01:14.000000 declearn-2.2.0/test/conftest.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/dataset/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2265 2023-05-04 10:01:14.000000 declearn-2.2.0/test/dataset/test_examples.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6439 2023-05-04 10:01:14.000000 declearn-2.2.0/test/dataset/test_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/functional/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      975 2023-04-26 13:33:08.000000 declearn-2.2.0/test/functional/conftest.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11484 2023-05-04 10:01:14.000000 declearn-2.2.0/test/functional/test_main.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2247 2023-05-10 12:05:04.000000 declearn-2.2.0/test/functional/test_quickrun.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    13698 2023-05-10 12:05:04.000000 declearn-2.2.0/test/functional/test_regression.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.834330 declearn-2.2.0/test/main/
--rw-r--r--   0 paandrey (670133) magnet    (5235)    19053 2023-04-26 13:33:08.000000 declearn-2.2.0/test/main/test_checkpoint.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11884 2023-03-24 21:43:07.000000 declearn-2.2.0/test/main/test_train_manager.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6919 2023-04-26 13:33:08.000000 declearn-2.2.0/test/main/test_train_manager_dp.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.834330 declearn-2.2.0/test/metrics/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7320 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/metric_testing.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4532 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_binary_apr.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7386 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_binary_roc.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3936 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_mae_mse.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6907 2023-03-24 21:43:07.000000 declearn-2.2.0/test/metrics/test_metricset.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3328 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_multi_apr.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3503 2023-04-26 13:33:08.000000 declearn-2.2.0/test/metrics/test_rsquared.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.834330 declearn-2.2.0/test/model/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8764 2023-05-11 12:55:46.000000 declearn-2.2.0/test/model/model_testing.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10752 2023-05-11 13:44:56.000000 declearn-2.2.0/test/model/test_haiku.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6022 2023-04-26 13:33:08.000000 declearn-2.2.0/test/model/test_sksgd.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8310 2023-05-11 07:58:34.000000 declearn-2.2.0/test/model/test_tflow.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11226 2023-05-10 12:05:04.000000 declearn-2.2.0/test/model/test_torch.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7354 2023-03-27 10:07:29.000000 declearn-2.2.0/test/model/test_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.838330 declearn-2.2.0/test/optimizer/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      985 2023-03-24 21:43:07.000000 declearn-2.2.0/test/optimizer/conftest.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5234 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/optim_testing.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6356 2023-05-03 08:56:42.000000 declearn-2.2.0/test/optimizer/test_modules.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3868 2023-03-24 21:43:07.000000 declearn-2.2.0/test/optimizer/test_noise.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15787 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/test_optimizer.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2189 2023-03-24 21:43:07.000000 declearn-2.2.0/test/optimizer/test_regularizers.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4924 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/test_scaffold.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8569 2023-04-26 13:33:08.000000 declearn-2.2.0/test/optimizer/test_tflow_optim.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     9702 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/test_torch_optim.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.838330 declearn-2.2.0/test/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5388 2023-03-24 21:43:07.000000 declearn-2.2.0/test/utils/test_json.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6623 2023-05-10 12:05:04.000000 declearn-2.2.0/test/utils/test_register.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5952 2023-03-24 21:43:07.000000 declearn-2.2.0/test/utils/test_serialize.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15940 2023-05-10 12:05:04.000000 declearn-2.2.0/test/utils/test_toml.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)      875 2023-05-10 12:05:04.000000 declearn-2.2.0/tox.ini
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.941892 declearn-2.2.1/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1652 2023-08-04 08:50:16.000000 declearn-2.2.1/.gitlab-ci.yml
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      560 2023-08-04 08:43:53.000000 declearn-2.2.1/AUTHORS
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11357 2023-03-24 21:43:07.000000 declearn-2.2.1/LICENSE
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19325 2023-08-04 08:52:56.941892 declearn-2.2.1/PKG-INFO
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4977 2023-08-04 08:50:16.000000 declearn-2.2.1/README.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.921893 declearn-2.2.1/declearn/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2496 2023-08-04 08:51:26.000000 declearn-2.2.1/declearn/__init__.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.921893 declearn-2.2.1/declearn/aggregator/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1705 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/aggregator/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5597 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/aggregator/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4167 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/aggregator/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4271 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/aggregator/_gma.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.921893 declearn-2.2.1/declearn/communication/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3046 2023-08-04 08:13:21.000000 declearn-2.2.1/declearn/communication/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8164 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/_build.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/communication/api/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1248 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/api/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9146 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/api/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    13310 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/communication/api/_server.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16342 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/api/_service.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/communication/grpc/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1308 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/grpc/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4811 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/communication/grpc/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8877 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/communication/grpc/_server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/communication/grpc/protobufs/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1398 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/grpc/protobufs/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      263 2023-08-02 12:54:57.000000 declearn-2.2.1/declearn/communication/grpc/protobufs/message.proto
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1841 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/communication/grpc/protobufs/message_pb2.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5239 2023-08-02 12:58:33.000000 declearn-2.2.1/declearn/communication/grpc/protobufs/message_pb2_grpc.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/communication/messaging/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2409 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/messaging/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6999 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/communication/messaging/_messages.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1410 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/messaging/flags.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/communication/websockets/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1143 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/communication/websockets/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5973 2023-03-31 13:39:10.000000 declearn-2.2.1/declearn/communication/websockets/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6514 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/communication/websockets/_server.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3509 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/communication/websockets/_tools.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/data_info/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2948 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/data_info/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8345 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/data_info/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7274 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/data_info/_fields.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/dataset/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2119 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6510 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    21645 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/_inmemory.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8307 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/_split_data.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/dataset/examples/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1053 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/examples/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5145 2023-08-04 08:51:09.000000 declearn-2.2.1/declearn/dataset/examples/_heart_uci.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3770 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/examples/_mnist.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/dataset/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1693 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4866 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/utils/_save_load.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6022 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/utils/_sparse.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7065 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/dataset/utils/_split_classif.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/main/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2160 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    17375 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/main/_client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    28091 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/main/_server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/main/config/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1739 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/config/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7695 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/config/_dataclasses.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5589 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/config/_run_config.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7888 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/main/config/_strategy.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.925892 declearn-2.2.1/declearn/main/privacy/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      904 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/privacy/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10673 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/privacy/_dp_trainer.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/main/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2584 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    21365 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/main/utils/_checkpoint.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5064 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/main/utils/_constraints.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7442 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/utils/_data_info.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4007 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/main/utils/_early_stop.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    14134 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/main/utils/_training.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/metrics/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2861 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/metrics/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12815 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/metrics/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8084 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/metrics/_classif.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5249 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/metrics/_mean.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11953 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/metrics/_roc_auc.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5123 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/metrics/_rsquared.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8185 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/metrics/_wrapper.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2949 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1803 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/model/_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/api/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1202 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/model/api/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11185 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/api/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15994 2023-08-04 08:50:23.000000 declearn-2.2.1/declearn/model/api/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/haiku/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1062 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/haiku/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    20958 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/haiku/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5742 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/haiku/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/haiku/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      857 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/haiku/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2751 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/haiku/utils/_gpu.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/sklearn/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1216 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/model/sklearn/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3957 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/sklearn/_np_vec.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15358 2023-08-04 08:51:01.000000 declearn-2.2.1/declearn/model/sklearn/_sgd.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/tensorflow/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1552 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/model/tensorflow/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15417 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/tensorflow/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10658 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/model/tensorflow/_optim.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10302 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/tensorflow/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/tensorflow/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1881 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/model/tensorflow/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4455 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/tensorflow/utils/_gpu.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4530 2023-08-04 08:50:48.000000 declearn-2.2.1/declearn/model/tensorflow/utils/_loss.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5360 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/model/tensorflow/utils/_slices.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.929892 declearn-2.2.1/declearn/model/torch/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1474 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/torch/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16535 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/torch/_model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    13026 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/model/torch/_optim.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6861 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/torch/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/declearn/model/torch/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1094 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/model/torch/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4641 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/model/torch/utils/_gpu.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/declearn/optimizer/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1711 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/optimizer/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19710 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/optimizer/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3130 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/optimizer/_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/declearn/optimizer/modules/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2836 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/optimizer/modules/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11020 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/optimizer/modules/_adaptive.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11323 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/optimizer/modules/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2374 2023-08-04 08:50:31.000000 declearn-2.2.1/declearn/optimizer/modules/_clipping.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6600 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/optimizer/modules/_momentum.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6031 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/optimizer/modules/_noise.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15038 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/optimizer/modules/_scaffold.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/declearn/optimizer/regularizers/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1453 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/optimizer/regularizers/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6166 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/optimizer/regularizers/_api.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3405 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/optimizer/regularizers/_base.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)        0 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/py.typed
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/declearn/quickrun/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1811 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/quickrun/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3938 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/quickrun/_config.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6652 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/quickrun/_parser.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9386 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/quickrun/_run.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/declearn/test_utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1616 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/test_utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4704 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/test_utils/_argparse.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6683 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/test_utils/_assertions.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6040 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/test_utils/_gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1772 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/test_utils/_imports.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6524 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/test_utils/_vectors.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2096 2023-08-03 15:48:00.000000 declearn-2.2.1/declearn/typing.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/declearn/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5008 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7741 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/utils/_dataclass.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4174 2023-08-04 08:43:53.000000 declearn-2.2.1/declearn/utils/_device_policy.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7056 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/utils/_json.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2968 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/utils/_logging.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4938 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/utils/_multiprocess.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1575 2023-03-24 21:43:07.000000 declearn-2.2.1/declearn/utils/_numpy.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10530 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/utils/_register.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6342 2023-05-04 10:01:14.000000 declearn-2.2.1/declearn/utils/_serialize.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15250 2023-08-04 08:50:16.000000 declearn-2.2.1/declearn/utils/_toml_config.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.921893 declearn-2.2.1/declearn.egg-info/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19325 2023-08-04 08:52:56.000000 declearn-2.2.1/declearn.egg-info/PKG-INFO
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6607 2023-08-04 08:52:56.000000 declearn-2.2.1/declearn.egg-info/SOURCES.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)        1 2023-08-04 08:52:56.000000 declearn-2.2.1/declearn.egg-info/dependency_links.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      117 2023-08-04 08:52:56.000000 declearn-2.2.1/declearn.egg-info/entry_points.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      641 2023-08-04 08:52:56.000000 declearn-2.2.1/declearn.egg-info/requires.txt
+-rw-r--r--   0 paandrey (670133) magnet   (208235)        9 2023-08-04 08:52:56.000000 declearn-2.2.1/declearn.egg-info/top_level.txt
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/docs/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      181 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/SUMMARY.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.933892 declearn-2.2.1/docs/api-reference/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      416 2023-08-04 08:50:16.000000 declearn-2.2.1/docs/api-reference/index.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/docs/devs-guide/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      207 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/devs-guide/SUMMARY.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3650 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/devs-guide/contribute.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2930 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/devs-guide/docs-build.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10370 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/devs-guide/docs-style.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      746 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/devs-guide/index.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6994 2023-08-04 08:13:21.000000 declearn-2.2.1/docs/devs-guide/tests.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3884 2023-08-04 08:43:53.000000 declearn-2.2.1/docs/index.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    12500 2023-08-04 08:50:16.000000 declearn-2.2.1/docs/quickstart.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4270 2023-08-04 08:50:16.000000 declearn-2.2.1/docs/setup.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/docs/user-guide/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      230 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/user-guide/SUMMARY.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4626 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/user-guide/fl_process.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      799 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/user-guide/index.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4989 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/user-guide/local_dp.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5087 2023-05-04 10:01:14.000000 declearn-2.2.1/docs/user-guide/package.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9739 2023-08-04 08:50:16.000000 declearn-2.2.1/docs/user-guide/usage.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.921893 declearn-2.2.1/examples/
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/examples/adding_rmsprop/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4600 2023-03-24 21:43:07.000000 declearn-2.2.1/examples/adding_rmsprop/readme.md
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/examples/heart-uci/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3698 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/heart-uci/client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1642 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/heart-uci/data.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      916 2023-03-24 21:43:07.000000 declearn-2.2.1/examples/heart-uci/gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4214 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/heart-uci/readme.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2191 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/heart-uci/run.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4801 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/heart-uci/server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/examples/mnist/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3826 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist/client.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      916 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist/gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4882 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist/readme.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2498 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist/run.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5773 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist/server.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/examples/mnist_quickrun/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1628 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist_quickrun/config.toml
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    25127 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist_quickrun/mnist.ipynb
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      763 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist_quickrun/model.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1167 2023-08-04 08:50:16.000000 declearn-2.2.1/examples/mnist_quickrun/readme.md
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1046 2023-05-04 10:01:14.000000 declearn-2.2.1/mkdocs.yml
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3586 2023-08-04 08:51:39.000000 declearn-2.2.1/pyproject.toml
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/scripts/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5402 2023-08-04 08:13:21.000000 declearn-2.2.1/scripts/gen_docs.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)       38 2023-08-04 08:52:56.941892 declearn-2.2.1/setup.cfg
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/test/
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/test/aggregator/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3011 2023-08-04 08:50:16.000000 declearn-2.2.1/test/aggregator/test_aggregator.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/test/communication/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1680 2023-03-24 21:43:07.000000 declearn-2.2.1/test/communication/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9311 2023-08-04 08:50:16.000000 declearn-2.2.1/test/communication/test_exchanges.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11813 2023-03-24 21:43:07.000000 declearn-2.2.1/test/communication/test_grpc.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    16395 2023-08-04 08:50:16.000000 declearn-2.2.1/test/communication/test_server.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     1529 2023-08-04 08:50:16.000000 declearn-2.2.1/test/conftest.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/test/dataset/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2259 2023-08-04 08:51:09.000000 declearn-2.2.1/test/dataset/test_examples.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6439 2023-08-04 08:50:16.000000 declearn-2.2.1/test/dataset/test_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/test/functional/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      975 2023-08-04 08:43:53.000000 declearn-2.2.1/test/functional/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11484 2023-08-04 08:50:16.000000 declearn-2.2.1/test/functional/test_main.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2247 2023-08-04 08:50:16.000000 declearn-2.2.1/test/functional/test_quickrun.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    13698 2023-08-04 08:50:16.000000 declearn-2.2.1/test/functional/test_regression.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.937892 declearn-2.2.1/test/main/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    19053 2023-08-04 08:50:16.000000 declearn-2.2.1/test/main/test_checkpoint.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11884 2023-06-07 13:10:40.000000 declearn-2.2.1/test/main/test_train_manager.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6919 2023-08-04 08:50:16.000000 declearn-2.2.1/test/main/test_train_manager_dp.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.941892 declearn-2.2.1/test/metrics/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7320 2023-08-04 08:43:53.000000 declearn-2.2.1/test/metrics/metric_testing.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4532 2023-08-04 08:43:53.000000 declearn-2.2.1/test/metrics/test_binary_apr.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7386 2023-08-04 08:43:53.000000 declearn-2.2.1/test/metrics/test_binary_roc.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3936 2023-08-04 08:43:53.000000 declearn-2.2.1/test/metrics/test_mae_mse.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6907 2023-03-24 21:43:07.000000 declearn-2.2.1/test/metrics/test_metricset.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3328 2023-08-04 08:43:53.000000 declearn-2.2.1/test/metrics/test_multi_apr.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3503 2023-08-04 08:43:53.000000 declearn-2.2.1/test/metrics/test_rsquared.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.941892 declearn-2.2.1/test/model/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8764 2023-08-04 08:43:53.000000 declearn-2.2.1/test/model/model_testing.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    10752 2023-08-04 08:50:16.000000 declearn-2.2.1/test/model/test_haiku.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6022 2023-08-04 08:50:16.000000 declearn-2.2.1/test/model/test_sksgd.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11400 2023-08-04 08:50:38.000000 declearn-2.2.1/test/model/test_tflow.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    11226 2023-08-04 08:50:16.000000 declearn-2.2.1/test/model/test_torch.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     7354 2023-08-04 08:43:53.000000 declearn-2.2.1/test/model/test_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.941892 declearn-2.2.1/test/optimizer/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      985 2023-03-24 21:43:07.000000 declearn-2.2.1/test/optimizer/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5234 2023-08-04 08:43:53.000000 declearn-2.2.1/test/optimizer/optim_testing.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6356 2023-08-04 08:43:53.000000 declearn-2.2.1/test/optimizer/test_modules.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     3868 2023-03-24 21:43:07.000000 declearn-2.2.1/test/optimizer/test_noise.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15787 2023-08-04 08:43:53.000000 declearn-2.2.1/test/optimizer/test_optimizer.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     2189 2023-08-04 08:13:21.000000 declearn-2.2.1/test/optimizer/test_regularizers.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     4924 2023-08-04 08:43:53.000000 declearn-2.2.1/test/optimizer/test_scaffold.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     8569 2023-08-04 08:43:53.000000 declearn-2.2.1/test/optimizer/test_tflow_optim.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     9702 2023-08-04 08:43:53.000000 declearn-2.2.1/test/optimizer/test_torch_optim.py
+drwxr-xr-x   0 paandrey (670133) magnet   (208235)        0 2023-08-04 08:52:56.941892 declearn-2.2.1/test/utils/
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5388 2023-03-24 21:43:07.000000 declearn-2.2.1/test/utils/test_json.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     6623 2023-08-04 08:50:16.000000 declearn-2.2.1/test/utils/test_register.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)     5952 2023-03-24 21:43:07.000000 declearn-2.2.1/test/utils/test_serialize.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)    15940 2023-08-04 08:50:16.000000 declearn-2.2.1/test/utils/test_toml.py
+-rw-r--r--   0 paandrey (670133) magnet   (208235)      875 2023-08-04 08:50:16.000000 declearn-2.2.1/tox.ini
```

### Comparing `declearn-2.2.0/.gitlab-ci.yml` & `declearn-2.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/AUTHORS` & `declearn-2.2.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/LICENSE` & `declearn-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/PKG-INFO` & `declearn-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: declearn
-Version: 2.2.0
+Version: 2.2.1
 Summary: Declearn - a python package for private decentralized learning.
 Author-email: Paul Andrey <paul.andrey@inria.fr>, Nathan Bigaud <nathan.bigaud@inria.fr>
 Maintainer-email: Paul Andrey <paul.andrey@inria.fr>, Nathan Bigaud <nathan.bigaud@inria.fr>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `declearn-2.2.0/README.md` & `declearn-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/__init__.py` & `declearn-2.2.1/declearn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,8 +61,8 @@
     metrics,
     model,
     optimizer,
     typing,
     utils,
 )
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
```

### Comparing `declearn-2.2.0/declearn/aggregator/__init__.py` & `declearn-2.2.1/declearn/aggregator/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/aggregator/_api.py` & `declearn-2.2.1/declearn/aggregator/_api.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/aggregator/_base.py` & `declearn-2.2.1/declearn/aggregator/_base.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/aggregator/_gma.py` & `declearn-2.2.1/declearn/aggregator/_gma.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/__init__.py` & `declearn-2.2.1/declearn/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/_build.py` & `declearn-2.2.1/declearn/communication/_build.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/api/__init__.py` & `declearn-2.2.1/declearn/communication/api/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/api/_client.py` & `declearn-2.2.1/declearn/communication/api/_client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/api/_server.py` & `declearn-2.2.1/declearn/communication/api/_server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/api/_service.py` & `declearn-2.2.1/declearn/communication/api/_service.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/grpc/__init__.py` & `declearn-2.2.1/declearn/communication/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/grpc/_client.py` & `declearn-2.2.1/declearn/communication/grpc/_client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/grpc/_server.py` & `declearn-2.2.1/declearn/communication/grpc/_server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/grpc/protobufs/__init__.py` & `declearn-2.2.1/declearn/communication/grpc/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2.py` & `declearn-2.2.1/declearn/communication/grpc/protobufs/message_pb2.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py` & `declearn-2.2.1/declearn/communication/grpc/protobufs/message_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/messaging/__init__.py` & `declearn-2.2.1/declearn/communication/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/messaging/_messages.py` & `declearn-2.2.1/declearn/communication/messaging/_messages.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/messaging/flags.py` & `declearn-2.2.1/declearn/communication/messaging/flags.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/websockets/__init__.py` & `declearn-2.2.1/declearn/communication/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/websockets/_client.py` & `declearn-2.2.1/declearn/communication/websockets/_client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/websockets/_server.py` & `declearn-2.2.1/declearn/communication/websockets/_server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/communication/websockets/_tools.py` & `declearn-2.2.1/declearn/communication/websockets/_tools.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/data_info/__init__.py` & `declearn-2.2.1/declearn/data_info/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/data_info/_base.py` & `declearn-2.2.1/declearn/data_info/_base.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/data_info/_fields.py` & `declearn-2.2.1/declearn/data_info/_fields.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/__init__.py` & `declearn-2.2.1/declearn/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/_base.py` & `declearn-2.2.1/declearn/dataset/_base.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/_inmemory.py` & `declearn-2.2.1/declearn/dataset/_inmemory.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/_split_data.py` & `declearn-2.2.1/declearn/dataset/_split_data.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/examples/__init__.py` & `declearn-2.2.1/declearn/dataset/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/examples/_heart_uci.py` & `declearn-2.2.1/declearn/dataset/examples/_heart_uci.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,31 +13,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Util to download and pre-process the UCI Heart Disease dataset."""
 
+import io
 import os
-from typing import Literal, Optional, Tuple
+import zipfile
+from typing import Literal, Optional, Tuple, Union
 
-import pandas as pd  # type: ignore
+import pandas as pd
+import requests
 
 __all__ = [
     "load_heart_uci",
 ]
 
 
 def load_heart_uci(
     name: Literal["cleveland", "hungarian", "switzerland", "va"],
     folder: Optional[str] = None,
 ) -> Tuple[pd.DataFrame, str]:
     """Load and/or download a pre-processed UCI Heart Disease dataset.
 
-    See [https://archive.ics.uci.edu/ml/datasets/Heart+Disease] for
+    See [https://archive.ics.uci.edu/dataset/45/heart+disease] for
     information on the UCI Heart Disease dataset.
 
     Arguments
     ---------
     name: str
         Name of a center, the dataset from which to return.
     folder: str or None, default=None
@@ -49,51 +52,93 @@
     data: pd.DataFrame
         Pre-processed dataset from the `name` center.
         May be passed as `data` of a declearn `InMemoryDataset`.
     target: str
         Name of the target column in `data`.
         May be passed as `target` of a declearn `InMemoryDataset`.
     """
-    # If the file already exists, read and return it.
+    # If the pre-processed file already exists, read and return it.
     if folder is not None:
         path = os.path.join(folder, f"data_{name}.csv")
         if os.path.isfile(path):
             data = pd.read_csv(path)
             return data, "num"
-    # Otherwise, download and pre-process the data, and optionally save it.
-    data = download_heart_uci_shard(name)
+    # Download (and optionally save) or read from the source zip file.
+    source = get_heart_uci_zipfile(folder)
+    # Extract the target shard and preprocess it.
+    data = extract_heart_uci_shard(name, source)
+    data = preprocess_heart_uci_dataframe(data)
+    # Optionally save the preprocessed shard to disk.
     if folder is not None:
-        os.makedirs(folder, exist_ok=True)
-        data.to_csv(path, index=False)
+        path = os.path.join(folder, f"data_{name}.csv")
+        data.to_csv(path, sep=",", encoding="utf-8", index=False)
     return data, "num"
 
 
-def download_heart_uci_shard(
+def get_heart_uci_zipfile(folder: Optional[str]) -> Union[str, bytes]:
+    """Download and opt. save the Heart Dataset zip file, or return its path.
+
+    Return either the path to the zip file, or its contents.
+    """
+    # Case when the data is to be downloaded and kept only in memory.
+    if folder is None:
+        return download_heart_uci()
+    # Case when the data can be read from a pre-existing file on disk.
+    path = os.path.join(folder, "heart+disease.zip")
+    if os.path.isfile(path):
+        return path
+    # Case when the data is to be donwloaded and saved on disk for re-use.
+    data = download_heart_uci()
+    with open(path, "wb") as file:
+        file.write(data)
+    return data
+
+
+def download_heart_uci() -> bytes:
+    """Download the Heart Disease UCI dataset source file."""
+    print("Downloading Heart Disease UCI dataset.")
+    url = "https://archive.ics.uci.edu/static/public/45/heart+disease.zip"
+    reply = requests.get(url, timeout=300)
+    try:
+        reply.raise_for_status()
+    except requests.HTTPError as exc:
+        raise RuntimeError(
+            "Failed to download Heart Disease UCI source file."
+        ) from exc
+    return reply.content
+
+
+def extract_heart_uci_shard(
     name: Literal["cleveland", "hungarian", "switzerland", "va"],
+    source: Union[str, bytes],
+) -> pd.DataFrame:
+    """Read a subset of the Heart UCI data, from in-memory or on-disk data."""
+    zdat = source if isinstance(source, str) else io.BytesIO(source)
+    with zipfile.ZipFile(zdat) as archive:  # type: ignore
+        with archive.open(f"processed.{name}.data") as path:
+            data = pd.read_csv(path, header=None, na_values="?")
+    return data
+
+
+def preprocess_heart_uci_dataframe(
+    data: pd.DataFrame,
 ) -> pd.DataFrame:
-    """Download and preprocess a subset of the Heart UCI dataset."""
-    print(f"Downloading Heart Disease UCI dataset from center {name}.")
-    url = (
-        "https://archive.ics.uci.edu/ml/machine-learning-databases/"
-        f"heart-disease/processed.{name}.data"
-    )
-    # Download the dataaset.
-    data = pd.read_csv(url, header=None, na_values="?")
+    """Preprocess a subset of the Heart UCI dataset."""
     columns = [
         # fmt: off
         "age", "sex", "cp", "trestbps", "chol", "fbs", "restecg",
         "thalach", "exang", "oldpeak", "slope", "ca", "thal", "num",
     ]
     data = data.set_axis(columns, axis=1, copy=False)
     # Drop unused columns and rows with missing values.
     data.drop(columns=["ca", "chol", "fbs", "slope", "thal"], inplace=True)
     data.dropna(inplace=True)
     data.reset_index(inplace=True, drop=True)
     # Normalize quantitative variables.
     for col in ("age", "trestbps", "thalach", "oldpeak"):
-        data[col] = (  # type: ignore
+        data[col] = (
             data[col] - data[col].mean() / data[col].std()  # type: ignore
         )
     # Binarize the target variable.
     data["num"] = (data["num"] > 0).astype(int)
     # Return the prepared dataframe.
     return data
```

### Comparing `declearn-2.2.0/declearn/dataset/examples/_mnist.py` & `declearn-2.2.1/declearn/dataset/examples/_mnist.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/utils/__init__.py` & `declearn-2.2.1/declearn/dataset/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/utils/_save_load.py` & `declearn-2.2.1/declearn/dataset/utils/_save_load.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/utils/_sparse.py` & `declearn-2.2.1/declearn/dataset/utils/_sparse.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/dataset/utils/_split_classif.py` & `declearn-2.2.1/declearn/dataset/utils/_split_classif.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/__init__.py` & `declearn-2.2.1/declearn/main/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/_client.py` & `declearn-2.2.1/declearn/main/_client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/_server.py` & `declearn-2.2.1/declearn/main/_server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/config/__init__.py` & `declearn-2.2.1/declearn/main/config/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/config/_dataclasses.py` & `declearn-2.2.1/declearn/main/config/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/config/_run_config.py` & `declearn-2.2.1/declearn/main/config/_run_config.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/config/_strategy.py` & `declearn-2.2.1/declearn/main/config/_strategy.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/privacy/__init__.py` & `declearn-2.2.1/declearn/main/privacy/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/privacy/_dp_trainer.py` & `declearn-2.2.1/declearn/main/privacy/_dp_trainer.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/utils/__init__.py` & `declearn-2.2.1/declearn/main/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/utils/_checkpoint.py` & `declearn-2.2.1/declearn/main/utils/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/utils/_constraints.py` & `declearn-2.2.1/declearn/main/utils/_constraints.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/utils/_data_info.py` & `declearn-2.2.1/declearn/main/utils/_data_info.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/utils/_early_stop.py` & `declearn-2.2.1/declearn/main/utils/_early_stop.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/main/utils/_training.py` & `declearn-2.2.1/declearn/main/utils/_training.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/metrics/__init__.py` & `declearn-2.2.1/declearn/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/metrics/_api.py` & `declearn-2.2.1/declearn/metrics/_api.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/metrics/_classif.py` & `declearn-2.2.1/declearn/metrics/_classif.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/metrics/_mean.py` & `declearn-2.2.1/declearn/metrics/_mean.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/metrics/_roc_auc.py` & `declearn-2.2.1/declearn/metrics/_roc_auc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/metrics/_rsquared.py` & `declearn-2.2.1/declearn/metrics/_rsquared.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/metrics/_wrapper.py` & `declearn-2.2.1/declearn/metrics/_wrapper.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/__init__.py` & `declearn-2.2.1/declearn/model/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/_utils.py` & `declearn-2.2.1/declearn/model/_utils.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/api/__init__.py` & `declearn-2.2.1/declearn/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/api/_model.py` & `declearn-2.2.1/declearn/model/api/_model.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/api/_vector.py` & `declearn-2.2.1/declearn/model/api/_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
     ) -> Self:
         return self._apply_operation(other, self._op_div)
 
     def __rtruediv__(
         self,
         other: Any,
     ) -> Self:
-        return self.__mul__(1 / other)
+        return self.__truediv__(other) ** -1
 
     def __pow__(
         self,
         other: Any,
     ) -> Self:
         return self._apply_operation(other, self._op_pow)
```

### Comparing `declearn-2.2.0/declearn/model/haiku/__init__.py` & `declearn-2.2.1/declearn/model/haiku/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/haiku/_model.py` & `declearn-2.2.1/declearn/model/haiku/_model.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/haiku/_vector.py` & `declearn-2.2.1/declearn/model/haiku/_vector.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/haiku/utils/__init__.py` & `declearn-2.2.1/declearn/model/haiku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/haiku/utils/_gpu.py` & `declearn-2.2.1/declearn/model/haiku/utils/_gpu.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/sklearn/__init__.py` & `declearn-2.2.1/declearn/model/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/sklearn/_np_vec.py` & `declearn-2.2.1/declearn/model/sklearn/_np_vec.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/sklearn/_sgd.py` & `declearn-2.2.1/declearn/model/sklearn/_sgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,16 +290,16 @@
         if not isinstance(weights, NumpyVector):
             raise TypeError("SklearnSGDModel requires NumpyVector weights.")
         for key in ("coef", "intercept"):
             if key not in weights.coefs:
                 raise KeyError(
                     f"Missing required '{key}' in the received vector."
                 )
-        self._model.coef_ = weights.coefs["coef"].copy()
-        self._model.intercept_ = weights.coefs["intercept"].copy()
+        self._model.coef_ = weights.coefs["coef"].astype("float64")
+        self._model.intercept_ = weights.coefs["intercept"].astype("float64")
 
     def compute_batch_gradients(
         self,
         batch: Batch,
         max_norm: Optional[float] = None,
     ) -> NumpyVector:
         # Unpack, validate and repack input data.
@@ -333,14 +333,15 @@
         x_data, y_data, s_wght = batch
         invalid = (y_data is None) or isinstance(y_data, list)
         if invalid or isinstance(x_data, list):
             raise TypeError(
                 "'SklearnSGDModel' requires (array, array, [array|None]) "
                 "data batches."
             )
+        x_data = x_data.astype("float64", copy=False)  # type: ignore
         return x_data, y_data, s_wght  # type: ignore
 
     def _compute_sample_gradient(
         self,
         x_smp: ArrayLike,
         y_smp: float,
     ) -> NumpyVector:
```

### Comparing `declearn-2.2.0/declearn/model/tensorflow/__init__.py` & `declearn-2.2.1/declearn/model/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/tensorflow/_model.py` & `declearn-2.2.1/declearn/model/tensorflow/_model.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/tensorflow/_optim.py` & `declearn-2.2.1/declearn/model/tensorflow/_optim.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/tensorflow/_vector.py` & `declearn-2.2.1/declearn/model/tensorflow/_vector.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/tensorflow/utils/__init__.py` & `declearn-2.2.1/declearn/model/tensorflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/tensorflow/utils/_gpu.py` & `declearn-2.2.1/declearn/model/tensorflow/utils/_gpu.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/tensorflow/utils/_loss.py` & `declearn-2.2.1/declearn/model/tensorflow/utils/_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,33 +81,49 @@
     -------
     loss_obj: tf.keras.losses.Loss
         Loss object, configured to apply the `reduction` scheme.
     """
     # Case when 'loss' is already a Loss object.
     if isinstance(loss, tf.keras.losses.Loss):
         loss.reduction = reduction
-    # Case when 'loss' is a string.
+    # Case when 'loss' is a string: deserialize and/or wrap into a Loss object.
     elif isinstance(loss, str):
-        cls = tf.keras.losses.deserialize(loss)
-        # Case when the string was deserialized into a function.
-        if inspect.isfunction(cls):
-            # Try altering the string to gather its object counterpart.
-            loss = "".join(word.capitalize() for word in loss.split("_"))
-            try:
-                loss = tf.keras.losses.deserialize(loss)
-                loss.reduction = reduction
-            # If this failed, try wrapping the function using LossFunction.
-            except ValueError:
-                loss = LossFunction(cls)
-        # Case when the string was deserialized into a class.
-        else:
-            loss = cls(reduction=reduction)
+        loss = get_keras_loss_from_string(name=loss, reduction=reduction)
     # Case when 'loss' is a function: wrap it up using LossFunction.
     elif inspect.isfunction(loss):
         loss = LossFunction(loss, reduction=reduction)
     # Case when 'loss' is of invalid type: raise a TypeError.
     if not isinstance(loss, tf.keras.losses.Loss):
         raise TypeError(
             "'loss' should be a keras Loss object or the name of one."
         )
     # Otherwise, properly configure the reduction scheme and return.
     return loss
+
+
+def get_keras_loss_from_string(
+    name: str,
+    reduction: str,
+) -> tf.keras.losses.Loss:
+    """Instantiate a keras Loss object from a registered string identifier.
+
+    - If `name` matches a Loss registration name, return an instance.
+    - If it matches a loss function registration name, return either
+      an instance from its name-matching Loss subclass, or a custom
+      Loss subclass instance wrapping the function.
+    - If it does not match anything, raise a ValueError.
+    """
+    loss = tf.keras.losses.deserialize(name)
+    if isinstance(loss, tf.keras.losses.Loss):
+        loss.reduction = reduction
+        return loss
+    if inspect.isfunction(loss):
+        try:
+            name = "".join(word.capitalize() for word in name.split("_"))
+            return get_keras_loss_from_string(name, reduction)
+        except ValueError:
+            return LossFunction(
+                loss, reduction=reduction, name=getattr(loss, "__name__", None)
+            )
+    raise ValueError(
+        f"Name '{loss}' cannot be deserialized into a keras loss."
+    )
```

### Comparing `declearn-2.2.0/declearn/model/tensorflow/utils/_slices.py` & `declearn-2.2.1/declearn/model/tensorflow/utils/_slices.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/torch/__init__.py` & `declearn-2.2.1/declearn/model/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/torch/_model.py` & `declearn-2.2.1/declearn/model/torch/_model.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/torch/_optim.py` & `declearn-2.2.1/declearn/model/torch/_optim.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/torch/_vector.py` & `declearn-2.2.1/declearn/model/torch/_vector.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/torch/utils/__init__.py` & `declearn-2.2.1/declearn/model/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/model/torch/utils/_gpu.py` & `declearn-2.2.1/declearn/model/torch/utils/_gpu.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/__init__.py` & `declearn-2.2.1/declearn/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/_base.py` & `declearn-2.2.1/declearn/optimizer/_base.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/_utils.py` & `declearn-2.2.1/declearn/optimizer/_utils.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/modules/__init__.py` & `declearn-2.2.1/declearn/optimizer/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/modules/_adaptive.py` & `declearn-2.2.1/declearn/optimizer/modules/_adaptive.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/modules/_api.py` & `declearn-2.2.1/declearn/optimizer/modules/_api.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/modules/_clipping.py` & `declearn-2.2.1/declearn/optimizer/modules/_clipping.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,20 @@
 
 
 class L2Clipping(OptiModule):
     """Fixed-threshold L2-norm gradient clipping module.
 
     This module implements the following algorithm:
 
-        Init(max_norm):
-        Step(max_norm):
-            norm = euclidean_norm(grads)
-            clip = min(norm, max_norm)
-            grads *= clip / max_norm
+        Init(max_norm, per_grad):
+            assign hyper-parameters
+        Step(grads):
+            norm = euclidean_norm(grads)  # parameter-wise
+            clip = max(max_norm / norm, 1.0)
+            grads *= clip
 
     In other words, (batch-averaged) gradients are clipped
     based on their L2 (euclidean) norm, based on a single,
     fixed threshold (as opposed to more complex algorithms
     that may use parameter-wise and/or adaptive clipping).
 
     This may notably be used to bound the contribution of
@@ -63,14 +64,14 @@
         self.max_norm = max_norm
 
     def run(
         self,
         gradients: Vector,
     ) -> Vector:
         l2_norm = (gradients**2).sum() ** 0.5
-        c_scale = (l2_norm / self.max_norm).minimum(1.0)
+        c_scale = (self.max_norm / l2_norm).minimum(1.0)
         return gradients * c_scale
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
         return {"max_norm": self.max_norm}
```

### Comparing `declearn-2.2.0/declearn/optimizer/modules/_momentum.py` & `declearn-2.2.1/declearn/optimizer/modules/_momentum.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/modules/_noise.py` & `declearn-2.2.1/declearn/optimizer/modules/_noise.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/modules/_scaffold.py` & `declearn-2.2.1/declearn/optimizer/modules/_scaffold.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/regularizers/__init__.py` & `declearn-2.2.1/declearn/optimizer/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/regularizers/_api.py` & `declearn-2.2.1/declearn/optimizer/regularizers/_api.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/optimizer/regularizers/_base.py` & `declearn-2.2.1/declearn/optimizer/regularizers/_base.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/quickrun/__init__.py` & `declearn-2.2.1/declearn/quickrun/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/quickrun/_config.py` & `declearn-2.2.1/declearn/quickrun/_config.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/quickrun/_parser.py` & `declearn-2.2.1/declearn/quickrun/_parser.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/quickrun/_run.py` & `declearn-2.2.1/declearn/quickrun/_run.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/test_utils/__init__.py` & `declearn-2.2.1/declearn/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/test_utils/_argparse.py` & `declearn-2.2.1/declearn/test_utils/_argparse.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/test_utils/_assertions.py` & `declearn-2.2.1/declearn/test_utils/_assertions.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/test_utils/_gen_ssl.py` & `declearn-2.2.1/declearn/test_utils/_gen_ssl.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/test_utils/_imports.py` & `declearn-2.2.1/declearn/test_utils/_imports.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/test_utils/_vectors.py` & `declearn-2.2.1/declearn/test_utils/_vectors.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/typing.py` & `declearn-2.2.1/declearn/typing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/__init__.py` & `declearn-2.2.1/declearn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_dataclass.py` & `declearn-2.2.1/declearn/utils/_dataclass.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_device_policy.py` & `declearn-2.2.1/declearn/utils/_device_policy.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_json.py` & `declearn-2.2.1/declearn/utils/_json.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_logging.py` & `declearn-2.2.1/declearn/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_multiprocess.py` & `declearn-2.2.1/declearn/utils/_multiprocess.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_numpy.py` & `declearn-2.2.1/declearn/utils/_numpy.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_register.py` & `declearn-2.2.1/declearn/utils/_register.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_serialize.py` & `declearn-2.2.1/declearn/utils/_serialize.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn/utils/_toml_config.py` & `declearn-2.2.1/declearn/utils/_toml_config.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn.egg-info/PKG-INFO` & `declearn-2.2.1/declearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: declearn
-Version: 2.2.0
+Version: 2.2.1
 Summary: Declearn - a python package for private decentralized learning.
 Author-email: Paul Andrey <paul.andrey@inria.fr>, Nathan Bigaud <nathan.bigaud@inria.fr>
 Maintainer-email: Paul Andrey <paul.andrey@inria.fr>, Nathan Bigaud <nathan.bigaud@inria.fr>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `declearn-2.2.0/declearn.egg-info/SOURCES.txt` & `declearn-2.2.1/declearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/declearn.egg-info/requires.txt` & `declearn-2.2.1/declearn.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/devs-guide/contribute.md` & `declearn-2.2.1/docs/devs-guide/contribute.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/devs-guide/docs-build.md` & `declearn-2.2.1/docs/devs-guide/docs-build.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/devs-guide/docs-style.md` & `declearn-2.2.1/docs/devs-guide/docs-style.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/devs-guide/index.md` & `declearn-2.2.1/docs/devs-guide/index.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/devs-guide/tests.md` & `declearn-2.2.1/docs/devs-guide/tests.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/index.md` & `declearn-2.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/quickstart.md` & `declearn-2.2.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/setup.md` & `declearn-2.2.1/docs/setup.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/user-guide/fl_process.md` & `declearn-2.2.1/docs/user-guide/fl_process.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/user-guide/index.md` & `declearn-2.2.1/docs/user-guide/index.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/user-guide/local_dp.md` & `declearn-2.2.1/docs/user-guide/local_dp.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/user-guide/package.md` & `declearn-2.2.1/docs/user-guide/package.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/docs/user-guide/usage.md` & `declearn-2.2.1/docs/user-guide/usage.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/adding_rmsprop/readme.md` & `declearn-2.2.1/examples/adding_rmsprop/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/heart-uci/client.py` & `declearn-2.2.1/examples/heart-uci/client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/heart-uci/data.py` & `declearn-2.2.1/examples/heart-uci/data.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/heart-uci/gen_ssl.py` & `declearn-2.2.1/examples/heart-uci/gen_ssl.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/heart-uci/readme.md` & `declearn-2.2.1/examples/heart-uci/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/heart-uci/run.py` & `declearn-2.2.1/examples/heart-uci/run.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/heart-uci/server.py` & `declearn-2.2.1/examples/heart-uci/server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist/client.py` & `declearn-2.2.1/examples/mnist/client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist/gen_ssl.py` & `declearn-2.2.1/examples/mnist/gen_ssl.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist/readme.md` & `declearn-2.2.1/examples/mnist/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist/run.py` & `declearn-2.2.1/examples/mnist/run.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist/server.py` & `declearn-2.2.1/examples/mnist/server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist_quickrun/config.toml` & `declearn-2.2.1/examples/mnist_quickrun/config.toml`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist_quickrun/mnist.ipynb` & `declearn-2.2.1/examples/mnist_quickrun/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist_quickrun/model.py` & `declearn-2.2.1/examples/mnist_quickrun/model.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/examples/mnist_quickrun/readme.md` & `declearn-2.2.1/examples/mnist_quickrun/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/mkdocs.yml` & `declearn-2.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/pyproject.toml` & `declearn-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "pip >= 19",
     "setuptools >= 62.0",
     "setuptools-scm[toml] >= 6.2",
 ]
 
 [project]
 name = "declearn"
-version = "2.2.0"
+version = "2.2.1"
 description = "Declearn - a python package for private decentralized learning."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Paul Andrey", email = "paul.andrey@inria.fr"},
     {name = "Nathan Bigaud", email = "nathan.bigaud@inria.fr"},
```

### Comparing `declearn-2.2.0/scripts/gen_docs.py` & `declearn-2.2.1/scripts/gen_docs.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/aggregator/test_aggregator.py` & `declearn-2.2.1/test/aggregator/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/communication/conftest.py` & `declearn-2.2.1/test/communication/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/communication/test_exchanges.py` & `declearn-2.2.1/test/communication/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/communication/test_grpc.py` & `declearn-2.2.1/test/communication/test_grpc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/communication/test_server.py` & `declearn-2.2.1/test/communication/test_server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/conftest.py` & `declearn-2.2.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/dataset/test_examples.py` & `declearn-2.2.1/test/dataset/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """Functional tests for 'declearn.dataset.example.load_heart_uci'."""
     # Test that downloading the dataset works.
     data, tcol = load_heart_uci("va", folder=tmpdir)
     assert isinstance(data, pd.DataFrame)
     assert tcol in data.columns
     # Test that re-loading the dataset works.
     with mock.patch(
-        "declearn.dataset.examples._heart_uci.download_heart_uci_shard"
+        "declearn.dataset.examples._heart_uci.download_heart_uci"
     ) as patch_download:
         data_bis, tcol_bis = load_heart_uci("va", folder=tmpdir)
         patch_download.assert_not_called()
     assert np.allclose(data.values, data_bis.values)
     assert tcol == tcol_bis
```

### Comparing `declearn-2.2.0/test/dataset/test_utils.py` & `declearn-2.2.1/test/dataset/test_utils.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/functional/conftest.py` & `declearn-2.2.1/test/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/functional/test_main.py` & `declearn-2.2.1/test/functional/test_main.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/functional/test_quickrun.py` & `declearn-2.2.1/test/functional/test_quickrun.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/functional/test_regression.py` & `declearn-2.2.1/test/functional/test_regression.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/main/test_checkpoint.py` & `declearn-2.2.1/test/main/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/main/test_train_manager.py` & `declearn-2.2.1/test/main/test_train_manager.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/main/test_train_manager_dp.py` & `declearn-2.2.1/test/main/test_train_manager_dp.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/metrics/metric_testing.py` & `declearn-2.2.1/test/metrics/metric_testing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/metrics/test_binary_apr.py` & `declearn-2.2.1/test/metrics/test_binary_apr.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/metrics/test_binary_roc.py` & `declearn-2.2.1/test/metrics/test_binary_roc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/metrics/test_mae_mse.py` & `declearn-2.2.1/test/metrics/test_mae_mse.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/metrics/test_metricset.py` & `declearn-2.2.1/test/metrics/test_metricset.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/metrics/test_multi_apr.py` & `declearn-2.2.1/test/metrics/test_multi_apr.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/metrics/test_rsquared.py` & `declearn-2.2.1/test/metrics/test_rsquared.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/model/model_testing.py` & `declearn-2.2.1/test/model/model_testing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/model/test_haiku.py` & `declearn-2.2.1/test/model/test_haiku.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/model/test_sksgd.py` & `declearn-2.2.1/test/model/test_sksgd.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/model/test_torch.py` & `declearn-2.2.1/test/model/test_torch.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/model/test_vector.py` & `declearn-2.2.1/test/model/test_vector.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/conftest.py` & `declearn-2.2.1/test/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/optim_testing.py` & `declearn-2.2.1/test/optimizer/optim_testing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/test_modules.py` & `declearn-2.2.1/test/optimizer/test_modules.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/test_noise.py` & `declearn-2.2.1/test/optimizer/test_noise.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/test_optimizer.py` & `declearn-2.2.1/test/optimizer/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/test_regularizers.py` & `declearn-2.2.1/test/optimizer/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/test_scaffold.py` & `declearn-2.2.1/test/optimizer/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/test_tflow_optim.py` & `declearn-2.2.1/test/optimizer/test_tflow_optim.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/optimizer/test_torch_optim.py` & `declearn-2.2.1/test/optimizer/test_torch_optim.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/utils/test_json.py` & `declearn-2.2.1/test/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/utils/test_register.py` & `declearn-2.2.1/test/utils/test_register.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/utils/test_serialize.py` & `declearn-2.2.1/test/utils/test_serialize.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/test/utils/test_toml.py` & `declearn-2.2.1/test/utils/test_toml.py`

 * *Files identical despite different names*

### Comparing `declearn-2.2.0/tox.ini` & `declearn-2.2.1/tox.ini`

 * *Files identical despite different names*

