# Comparing `tmp/ontouml_json2graph-1.0.0.tar.gz` & `tmp/ontouml_json2graph-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontouml_json2graph-1.0.0.tar", max compression
+gzip compressed data, was "ontouml_json2graph-1.0.1.tar", max compression
```

## Comparing `ontouml_json2graph-1.0.0.tar` & `ontouml_json2graph-1.0.1.tar`

### file list

```diff
@@ -1,177 +1,35 @@
--rw-r--r--   0        0        0    11558 2023-07-12 06:34:39.289637 ontouml_json2graph-1.0.0/LICENSE
--rw-r--r--   0        0        0       36 2023-07-24 18:48:39.910660 ontouml_json2graph-1.0.0/ontouml-json2graph/__init__.py
--rw-r--r--   0        0        0     4238 2023-07-24 13:02:21.457273 ontouml_json2graph-1.0.0/ontouml-json2graph/main.py
--rw-r--r--   0        0        0        0 2023-07-24 18:49:05.366684 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/__init__.py
--rw-r--r--   0        0        0     3973 2023-07-23 09:06:25.650949 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/arguments.py
--rw-r--r--   0        0        0        0 2023-07-24 18:49:05.346649 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/__init__.py
--rw-r--r--   0        0        0     9239 2023-07-24 13:57:18.274937 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_general.py
--rw-r--r--   0        0        0     9644 2023-07-24 15:25:16.489662 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_main.py
--rw-r--r--   0        0        0    20288 2023-07-24 12:35:45.810188 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_class.py
--rw-r--r--   0        0        0     3830 2023-07-24 15:26:58.764887 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_diagram.py
--rw-r--r--   0        0        0     4477 2023-07-24 15:26:58.786926 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_elementview.py
--rw-r--r--   0        0        0     2764 2023-07-24 15:26:58.720787 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_generalization.py
--rw-r--r--   0        0        0     4693 2023-07-24 15:25:13.845674 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_generalizationset.py
--rw-r--r--   0        0        0     4507 2023-07-24 15:26:31.657206 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_package.py
--rw-r--r--   0        0        0     2598 2023-07-24 15:26:16.275812 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_path.py
--rw-r--r--   0        0        0     5490 2023-07-24 15:26:16.162811 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_project.py
--rw-r--r--   0        0        0    14252 2023-07-24 15:26:16.195812 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_property.py
--rw-r--r--   0        0        0     3228 2023-07-24 15:26:16.237811 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_rectangularshape.py
--rw-r--r--   0        0        0     6653 2023-07-24 15:25:13.508069 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_relation.py
--rw-r--r--   0        0        0     2955 2023-07-12 06:34:39.303640 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/errors.py
--rw-r--r--   0        0        0     1614 2023-07-23 09:56:06.887203 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/globals.py
--rw-r--r--   0        0        0     3476 2023-07-12 06:34:39.303640 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/input_output.py
--rw-r--r--   0        0        0     2642 2023-07-12 06:34:39.303640 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/logger.py
--rw-r--r--   0        0        0     7258 2023-07-24 15:25:15.298673 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/messages.py
--rw-r--r--   0        0        0      878 2023-07-24 13:32:09.460632 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/sparql_queries.py
--rw-r--r--   0        0        0     1486 2023-07-12 06:34:39.303640 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/utils_general.py
--rw-r--r--   0        0        0     3213 2023-07-23 10:06:28.540573 ontouml_json2graph-1.0.0/ontouml-json2graph/modules/utils_graph.py
--rw-r--r--   0        0        0   260791 2023-07-19 08:27:42.951808 ontouml_json2graph-1.0.0/ontouml-json2graph/resources/Logo JSON2Graph Decoder.png
--rw-r--r--   0        0        0    18036 2023-07-12 06:34:39.311644 ontouml_json2graph-1.0.0/ontouml-json2graph/resources/ontouml_v100.ttl
--rw-r--r--   0        0        0    81820 2023-07-24 09:14:42.075736 ontouml_json2graph-1.0.0/ontouml-json2graph/resources/ontouml_v110.ttl
--rw-r--r--   0        0        0        0 2023-07-24 18:50:27.672038 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/__init__.py
--rw-r--r--   0        0        0     3215 2023-07-23 09:44:56.992460 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_aux.py
--rw-r--r--   0        0        0      736 2023-07-24 12:22:59.155533 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_clear.py
--rw-r--r--   0        0        0    25634 2023-07-24 14:41:23.387552 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/List of Tests.xlsx
--rw-r--r--   0        0        0      315 2023-07-12 06:34:39.313639 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_001.json
--rw-r--r--   0        0        0      601 2023-07-18 07:01:08.322848 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_001.ttl
--rw-r--r--   0        0        0      143 2023-07-12 06:34:39.310639 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_002.json
--rw-r--r--   0        0        0      412 2023-07-18 07:02:39.799620 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_002.ttl
--rw-r--r--   0        0        0      524 2023-07-12 06:34:39.313639 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_003.json
--rw-r--r--   0        0        0      829 2023-07-18 07:01:07.614926 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_003.ttl
--rw-r--r--   0        0        0      728 2023-07-12 06:34:39.321642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_004.json
--rw-r--r--   0        0        0      982 2023-07-18 07:01:09.730380 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_004.ttl
--rw-r--r--   0        0        0     1219 2023-07-12 06:34:39.321642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_005.json
--rw-r--r--   0        0        0     1440 2023-07-18 07:01:08.951527 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_005.ttl
--rw-r--r--   0        0        0     1475 2023-07-12 06:34:39.322747 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_006.json
--rw-r--r--   0        0        0     1675 2023-07-18 07:01:26.106205 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_006.ttl
--rw-r--r--   0        0        0     1732 2023-07-12 06:34:39.324641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_007.json
--rw-r--r--   0        0        0     1884 2023-07-18 07:01:25.672864 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_007.ttl
--rw-r--r--   0        0        0     1988 2023-07-12 06:34:39.325666 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_008.json
--rw-r--r--   0        0        0     2092 2023-07-18 07:01:10.390627 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_008.ttl
--rw-r--r--   0        0        0     2903 2023-07-12 06:34:39.331679 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_009.json
--rw-r--r--   0        0        0     3135 2023-07-24 15:25:15.890662 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_009.ttl
--rw-r--r--   0        0        0     3155 2023-07-12 06:34:39.338644 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_010.json
--rw-r--r--   0        0        0     3301 2023-07-22 03:41:43.613457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_010.ttl
--rw-r--r--   0        0        0     4018 2023-07-12 06:34:39.331679 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_011.json
--rw-r--r--   0        0        0     4307 2023-07-22 03:41:44.300456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_011.ttl
--rw-r--r--   0        0        0     4458 2023-07-12 06:34:39.339641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_012.json
--rw-r--r--   0        0        0     4623 2023-07-22 03:41:44.149458 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_012.ttl
--rw-r--r--   0        0        0    13813 2023-07-12 06:34:39.346640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_013.json
--rw-r--r--   0        0        0    16948 2023-07-22 03:41:43.976460 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_013.ttl
--rw-r--r--   0        0        0    15582 2023-07-12 06:34:39.350766 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_014.json
--rw-r--r--   0        0        0    19306 2023-07-22 03:41:43.864456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_014.ttl
--rw-r--r--   0        0        0    16593 2023-07-12 06:34:39.351655 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_015.json
--rw-r--r--   0        0        0    20186 2023-07-22 03:41:43.268500 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_015.ttl
--rw-r--r--   0        0        0    17603 2023-07-12 06:34:39.360643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_016.json
--rw-r--r--   0        0        0    21022 2023-07-24 15:25:14.830674 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_016.ttl
--rw-r--r--   0        0        0    19623 2023-07-12 06:34:39.360643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_017.json
--rw-r--r--   0        0        0    22777 2023-07-24 15:25:16.321661 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_017.ttl
--rw-r--r--   0        0        0     2334 2023-07-12 06:34:39.360643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_018.json
--rw-r--r--   0        0        0     3213 2023-07-22 03:41:44.232458 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_018.ttl
--rw-r--r--   0        0        0     2750 2023-07-12 06:34:39.379714 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_019.json
--rw-r--r--   0        0        0     3880 2023-07-22 03:41:44.121458 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_019.ttl
--rw-r--r--   0        0        0     4382 2023-07-12 06:34:39.367642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_020.json
--rw-r--r--   0        0        0     5062 2023-07-22 03:41:43.459460 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_020.ttl
--rw-r--r--   0        0        0     6016 2023-07-12 06:34:39.375659 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_021.json
--rw-r--r--   0        0        0     6351 2023-07-22 03:41:43.813457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_021.ttl
--rw-r--r--   0        0        0     6026 2023-07-12 06:34:39.378640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_022.json
--rw-r--r--   0        0        0     7403 2023-07-22 03:41:43.490458 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_022.ttl
--rw-r--r--   0        0        0    10450 2023-07-12 06:34:39.380644 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_023.json
--rw-r--r--   0        0        0    12665 2023-07-22 03:41:43.908457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_023.ttl
--rw-r--r--   0        0        0    10458 2023-07-12 06:34:39.389013 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_024.json
--rw-r--r--   0        0        0    12876 2023-07-22 03:41:43.521457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_024.ttl
--rw-r--r--   0        0        0    10582 2023-07-12 06:34:39.396655 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_025.json
--rw-r--r--   0        0        0    13051 2023-07-22 03:41:43.744943 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_025.ttl
--rw-r--r--   0        0        0     3244 2023-07-12 06:34:39.392640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_026.json
--rw-r--r--   0        0        0     4409 2023-07-22 03:41:44.011495 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_026.ttl
--rw-r--r--   0        0        0     5704 2023-07-12 06:34:39.399640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_027.json
--rw-r--r--   0        0        0     6302 2023-07-22 03:41:44.475456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_027.ttl
--rw-r--r--   0        0        0    14715 2023-07-12 06:34:39.400641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_028.json
--rw-r--r--   0        0        0    16121 2023-07-22 03:41:43.429458 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_028.ttl
--rw-r--r--   0        0        0    43888 2023-07-12 06:34:39.402654 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_029.json
--rw-r--r--   0        0        0    48921 2023-07-22 03:41:44.404457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_029.ttl
--rw-r--r--   0        0        0    46968 2023-07-12 06:34:39.404641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_030.json
--rw-r--r--   0        0        0    48692 2023-07-22 03:41:43.553456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_030.ttl
--rw-r--r--   0        0        0    47006 2023-07-12 06:34:39.413655 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_031.json
--rw-r--r--   0        0        0    51440 2023-07-22 03:41:44.369485 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_031.ttl
--rw-r--r--   0        0        0    48104 2023-07-19 07:11:53.398918 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_032.json
--rw-r--r--   0        0        0    55471 2023-07-22 03:41:43.334456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_032.ttl
--rw-r--r--   0        0        0    48087 2023-07-19 07:20:57.062908 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_033.json
--rw-r--r--   0        0        0    55542 2023-07-22 03:41:43.584456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_033.ttl
--rw-r--r--   0        0        0   100229 2023-07-19 07:20:56.963909 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_034.json
--rw-r--r--   0        0        0   108095 2023-07-22 03:41:43.368456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_034.ttl
--rw-r--r--   0        0        0   117660 2023-07-19 07:37:09.263532 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_035.json
--rw-r--r--   0        0        0   127674 2023-07-22 03:41:44.442457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_035.ttl
--rw-r--r--   0        0        0   127396 2023-07-12 06:34:39.435639 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_036.json
--rw-r--r--   0        0        0   139056 2023-07-22 03:41:44.051458 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_036.ttl
--rw-r--r--   0        0        0     2452 2023-07-12 06:34:39.433648 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_037.json
--rw-r--r--   0        0        0     3456 2023-07-18 07:01:37.054674 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_037.ttl
--rw-r--r--   0        0        0     4351 2023-07-12 06:34:39.436641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_038.json
--rw-r--r--   0        0        0     5821 2023-07-22 03:41:43.198459 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_038.ttl
--rw-r--r--   0        0        0     4350 2023-07-12 06:34:39.444640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_039.json
--rw-r--r--   0        0        0     5818 2023-07-22 03:41:43.399503 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_039.ttl
--rw-r--r--   0        0        0     4350 2023-07-12 06:34:39.447641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_040.json
--rw-r--r--   0        0        0     5816 2023-07-22 03:41:44.507455 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_040.ttl
--rw-r--r--   0        0        0     8572 2023-07-12 06:34:39.451698 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_041.json
--rw-r--r--   0        0        0    10018 2023-07-22 03:41:43.710458 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_041.ttl
--rw-r--r--   0        0        0    19623 2023-07-12 06:34:39.451698 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_042.json
--rw-r--r--   0        0        0    22889 2023-07-24 15:25:15.402674 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_042.ttl
--rw-r--r--   0        0        0    10582 2023-07-12 06:34:39.452641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_043.json
--rw-r--r--   0        0        0    13115 2023-07-22 03:41:44.193457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_043.ttl
--rw-r--r--   0        0        0    43888 2023-07-12 06:34:39.454658 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_044.json
--rw-r--r--   0        0        0    49044 2023-07-22 03:41:43.643457 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_044.ttl
--rw-r--r--   0        0        0   127396 2023-07-12 06:34:39.456642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_045.json
--rw-r--r--   0        0        0   139301 2023-07-22 03:41:44.087487 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_045.ttl
--rw-r--r--   0        0        0     8572 2023-07-12 06:34:39.454658 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_046.json
--rw-r--r--   0        0        0    10047 2023-07-22 03:41:43.945487 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_046.ttl
--rw-r--r--   0        0        0    84559 2023-07-12 10:16:27.308174 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_047.json
--rw-r--r--   0        0        0    84317 2023-07-22 03:41:43.233456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_047.ttl
--rw-r--r--   0        0        0   348435 2023-07-18 06:31:41.133218 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_048.json
--rw-r--r--   0        0        0   366162 2023-07-22 03:41:43.783456 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_048.ttl
--rw-r--r--   0        0        0    16381 2023-07-19 08:23:38.889841 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_049.json
--rw-r--r--   0        0        0    19904 2023-07-24 12:55:09.547353 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_049.ttl
--rw-r--r--   0        0        0    50812 2023-07-22 19:32:33.520780 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_050.json
--rw-r--r--   0        0        0    49170 2023-07-23 09:13:55.555320 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_050.ttl
--rw-r--r--   0        0        0    50812 2023-07-22 19:36:25.882437 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_051.json
--rw-r--r--   0        0        0    49196 2023-07-24 14:33:58.148234 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_051.ttl
--rw-r--r--   0        0        0    50721 2023-07-22 19:39:05.471975 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_052.json
--rw-r--r--   0        0        0    49171 2023-07-23 09:13:55.826415 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_052.ttl
--rw-r--r--   0        0        0    50721 2023-07-22 19:40:11.547187 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_053.json
--rw-r--r--   0        0        0    49195 2023-07-24 14:40:40.862214 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/test_053.ttl
--rw-r--r--   0        0        0   671744 2023-07-12 06:34:39.321642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_001.vpp
--rw-r--r--   0        0        0   692224 2023-07-12 06:34:39.322642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_003.vpp
--rw-r--r--   0        0        0   704512 2023-07-12 06:34:39.340992 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_008.vpp
--rw-r--r--   0        0        0   704512 2023-07-12 06:34:39.338644 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_009.vpp
--rw-r--r--   0        0        0   720896 2023-07-12 06:34:39.343091 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_010.vpp
--rw-r--r--   0        0        0   720896 2023-07-12 06:34:39.344642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_011.vpp
--rw-r--r--   0        0        0   724992 2023-07-12 06:34:39.363042 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_012.vpp
--rw-r--r--   0        0        0   757760 2023-07-12 06:34:39.355652 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_013.vpp
--rw-r--r--   0        0        0   774144 2023-07-12 06:34:39.359640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_014.vpp
--rw-r--r--   0        0        0   684032 2023-07-12 06:34:39.376641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_019.vpp
--rw-r--r--   0        0        0   684032 2023-07-12 06:34:39.378640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_020.vpp
--rw-r--r--   0        0        0   708608 2023-07-12 06:34:39.383647 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_021.vpp
--rw-r--r--   0        0        0   708608 2023-07-12 06:34:39.394643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_022.vpp
--rw-r--r--   0        0        0   708608 2023-07-12 06:34:39.394643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_023.vpp
--rw-r--r--   0        0        0   729088 2023-07-12 06:34:39.402654 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_024.vpp
--rw-r--r--   0        0        0   729088 2023-07-12 06:34:39.397642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_025.vpp
--rw-r--r--   0        0        0   585728 2023-07-12 06:34:39.401638 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_026.vpp
--rw-r--r--   0        0        0   667648 2023-07-12 06:34:39.410643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_027.vpp
--rw-r--r--   0        0        0   704512 2023-07-12 06:34:39.420643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_028.vpp
--rw-r--r--   0        0        0   782336 2023-07-12 06:34:39.421651 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_029.vpp
--rw-r--r--   0        0        0   765952 2023-07-12 06:34:39.420643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_030.vpp
--rw-r--r--   0        0        0   827392 2023-07-12 06:34:39.420643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_031.vpp
--rw-r--r--   0        0        0   835584 2023-07-12 06:34:39.427643 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_033.vpp
--rw-r--r--   0        0        0   962560 2023-07-12 06:34:39.437890 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_034.vpp
--rw-r--r--   0        0        0  1032192 2023-07-12 06:34:39.442642 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_035.vpp
--rw-r--r--   0        0        0  1069056 2023-07-12 06:34:39.441640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_036.vpp
--rw-r--r--   0        0        0   684032 2023-07-12 06:34:39.446644 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_037.vpp
--rw-r--r--   0        0        0   684032 2023-07-12 06:34:39.446644 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_038.vpp
--rw-r--r--   0        0        0   684032 2023-07-12 06:34:39.453641 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_039.vpp
--rw-r--r--   0        0        0   696320 2023-07-12 06:34:39.465640 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_040.vpp
--rw-r--r--   0        0        0   708608 2023-07-12 06:34:39.454658 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_041.vpp
--rw-r--r--   0        0        0   794624 2023-07-18 16:11:27.571471 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_049.vpp
--rw-r--r--   0        0        0   819200 2023-07-22 19:29:23.451386 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_files/VPP Files/test_050.vpp
--rw-r--r--   0        0        0     1150 2023-07-18 18:42:59.491150 ontouml_json2graph-1.0.0/ontouml-json2graph/tests/test_main.py
--rw-r--r--   0        0        0      750 2023-07-24 18:51:13.386788 ontouml_json2graph-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4944 2023-07-24 15:25:13.926674 ontouml_json2graph-1.0.0/README.md
--rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 16:01:41.550303 ontouml_json2graph-1.0.1/json2graph/__init__.py
+-rw-r--r--   0        0        0     6665 2023-08-04 07:14:52.925157 ontouml_json2graph-1.0.1/json2graph/decode.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.178418 ontouml_json2graph-1.0.1/json2graph/modules/__init__.py
+-rw-r--r--   0        0        0     6991 2023-08-04 07:14:52.927162 ontouml_json2graph-1.0.1/json2graph/modules/arguments.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:46:56.179420 ontouml_json2graph-1.0.1/json2graph/modules/decoder/__init__.py
+-rw-r--r--   0        0        0     9166 2023-08-04 07:14:52.929159 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_general.py
+-rw-r--r--   0        0        0     9537 2023-08-04 07:14:52.930158 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_main.py
+-rw-r--r--   0        0        0    20124 2023-08-04 07:14:52.932158 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_class.py
+-rw-r--r--   0        0        0     3826 2023-08-04 07:14:52.933159 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_diagram.py
+-rw-r--r--   0        0        0     4449 2023-08-04 07:14:52.934219 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_elementview.py
+-rw-r--r--   0        0        0     2738 2023-08-04 07:14:52.935159 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_generalization.py
+-rw-r--r--   0        0        0     4643 2023-08-04 07:14:52.936159 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_generalizationset.py
+-rw-r--r--   0        0        0     4490 2023-08-04 07:14:52.937157 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_package.py
+-rw-r--r--   0        0        0     2581 2023-08-04 07:14:52.938158 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_path.py
+-rw-r--r--   0        0        0     5455 2023-08-04 07:14:52.939157 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_project.py
+-rw-r--r--   0        0        0    14028 2023-08-04 07:14:52.941158 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_property.py
+-rw-r--r--   0        0        0     3211 2023-08-04 07:14:52.942158 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_rectangularshape.py
+-rw-r--r--   0        0        0     6576 2023-08-04 07:14:52.944249 ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_relation.py
+-rw-r--r--   0        0        0     2948 2023-08-04 07:14:52.945227 ontouml_json2graph-1.0.1/json2graph/modules/errors.py
+-rw-r--r--   0        0        0      997 2023-08-04 07:14:52.946159 ontouml_json2graph-1.0.1/json2graph/modules/globals.py
+-rw-r--r--   0        0        0     3462 2023-08-04 07:14:52.947158 ontouml_json2graph-1.0.1/json2graph/modules/input_output.py
+-rw-r--r--   0        0        0     2642 2023-08-02 10:46:56.193417 ontouml_json2graph-1.0.1/json2graph/modules/logger.py
+-rw-r--r--   0        0        0     7236 2023-08-04 07:14:52.948157 ontouml_json2graph-1.0.1/json2graph/modules/messages.py
+-rw-r--r--   0        0        0      878 2023-08-02 10:46:56.194418 ontouml_json2graph-1.0.1/json2graph/modules/sparql_queries.py
+-rw-r--r--   0        0        0     1486 2023-08-02 10:46:56.195420 ontouml_json2graph-1.0.1/json2graph/modules/utils_general.py
+-rw-r--r--   0        0        0     3667 2023-08-04 07:14:52.949159 ontouml_json2graph-1.0.1/json2graph/modules/utils_graph.py
+-rw-r--r--   0        0        0        0 2023-08-04 07:14:52.950158 ontouml_json2graph-1.0.1/json2graph/resources/__init__.py
+-rw-r--r--   0        0        0   102274 2023-08-04 09:42:00.662815 ontouml_json2graph-1.0.1/json2graph/resources/logo-json2graph.png
+-rw-r--r--   0        0        0     1020 2023-08-04 09:34:57.975454 ontouml_json2graph-1.0.1/json2graph/resources/metadata.yaml
+-rw-r--r--   0        0        0    18036 2023-08-02 10:46:56.198417 ontouml_json2graph-1.0.1/json2graph/resources/ontouml_v100.ttl
+-rw-r--r--   0        0        0    78196 2023-08-02 10:46:56.199418 ontouml_json2graph-1.0.1/json2graph/resources/ontouml_v110.ttl
+-rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1029 2023-08-04 09:34:23.998068 ontouml_json2graph-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9388 2023-08-04 12:27:16.260805 ontouml_json2graph-1.0.1/README.md
+-rw-r--r--   0        0        0    10160 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.1/PKG-INFO
```

### Comparing `ontouml_json2graph-1.0.0/LICENSE` & `ontouml_json2graph-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_general.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_general.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ General decoding functions. """
 
 from rdflib import Graph, URIRef, Literal, RDF
 
-import modules.arguments as args
-from modules.globals import URI_ONTOUML
-from modules.logger import initialize_logger
-from modules.sparql_queries import GET_ELEMENT_AND_TYPE
-from modules.utils_graph import load_ontouml_vocabulary
+from .. import arguments as args
+from ..logger import initialize_logger
+from ..sparql_queries import GET_ELEMENT_AND_TYPE
+from ..utils_graph import load_ontouml_vocabulary, ontouml_ref
 
 LOGGER = initialize_logger()
 
 
 def create_point(point_id: str, x_coord: int, y_coord: int, ontouml_graph: Graph) -> None:
     """ Creates a new instance of ontouml:Point with its ontouml:xCoordinate, and ontouml:yCoordinate properties.
 
@@ -20,24 +19,24 @@
     :type x_coord: int
     :param y_coord: Vertical coordinate of the new ontouml:Point.
     :type y_coord: int
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + point_id), RDF.type, URIRef(URI_ONTOUML + "Point")))
+    ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + point_id), RDF.type, ontouml_ref("Point")))
 
     # Setting x coordinate
     ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + point_id),
-                       URIRef(URI_ONTOUML + "xCoordinate"),
+                       ontouml_ref("xCoordinate"),
                        Literal(x_coord)))
 
     # Setting y coordinate
     ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + point_id),
-                       URIRef(URI_ONTOUML + "yCoordinate"),
+                       ontouml_ref("yCoordinate"),
                        Literal(y_coord)))
 
 
 def count_elements_graph(ontouml_graph: Graph) -> dict:
     """ Returns a dictionary with all element types on graphs and their respective quantity.
 
     :param ontouml_graph: Knowledge graph with loaded objects' ids and types
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_main.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """ JSON decode functions."""
 
 from rdflib import Graph, URIRef, Literal, RDF, XSD, OWL, RDFS
 
-import modules.arguments as args
-from modules.decoder.decode_general import clean_null_data, count_elements_graph
-from modules.decoder.decode_obj_class import create_class_properties
-from modules.decoder.decode_obj_diagram import create_diagram_properties
-from modules.decoder.decode_obj_elementview import create_elementview_properties
-from modules.decoder.decode_obj_generalization import create_generalization_properties
-from modules.decoder.decode_obj_generalizationset import create_generalizationset_properties
-from modules.decoder.decode_obj_package import create_package_properties
-from modules.decoder.decode_obj_path import create_path_properties
-from modules.decoder.decode_obj_project import create_project_properties
-from modules.decoder.decode_obj_property import create_property_properties
-from modules.decoder.decode_obj_rectangularshape import create_rectangularshape_properties
-from modules.decoder.decode_obj_relation import create_relation_properties
-from modules.globals import URI_ONTOUML, ELEMENT_VIEW_TYPES, SOFTWARE_NAME, SOFTWARE_VERSION, SOFTWARE_URL, \
-    CONFORMS_TO_VOCAB_VERSION
-from modules.logger import initialize_logger
-from modules.utils_general import get_date_time
+from .. import arguments as args
+from ..decoder.decode_general import clean_null_data, count_elements_graph
+from ..decoder.decode_obj_class import create_class_properties
+from ..decoder.decode_obj_diagram import create_diagram_properties
+from ..decoder.decode_obj_elementview import create_elementview_properties
+from ..decoder.decode_obj_generalization import create_generalization_properties
+from ..decoder.decode_obj_generalizationset import create_generalizationset_properties
+from ..decoder.decode_obj_package import create_package_properties
+from ..decoder.decode_obj_path import create_path_properties
+from ..decoder.decode_obj_project import create_project_properties
+from ..decoder.decode_obj_property import create_property_properties
+from ..decoder.decode_obj_rectangularshape import create_rectangularshape_properties
+from ..decoder.decode_obj_relation import create_relation_properties
+from ..globals import METADATA, ELEMENT_VIEW_TYPES
+from ..logger import initialize_logger
+from ..utils_general import get_date_time
+from ..utils_graph import ontouml_ref
 
 LOGGER = initialize_logger()
 
 
 def add_metadata(ontouml_graph: Graph) -> None:
     """ Adds basic metadata to the generated graph when not in test mode. The metadata added are:
-        - dct:conformsTo URI_ONTOUML
+        - dct:conformsTo METADATA["conformsToBase"]
         - dct:created (creation date)
         - dct:language (when user argument available)
         - type owl:Ontology
         - Decoder information as rdfs:comment and rdfs:seeAlso
 
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
@@ -37,17 +37,17 @@
 
     uri_dct = "http://purl.org/dc/terms/"
     ontouml_graph.bind("dct", uri_dct)
     uriref_ontology = URIRef(args.ARGUMENTS["base_uri"][:-1])
 
     # Adding conforms to
     dct_conforms_to = URIRef(uri_dct + "conformsTo")
-    vocab_uri = URIRef(URI_ONTOUML[:-1])
+    vocab_uri = URIRef(METADATA['conformsTo'])
     ontouml_graph.add((uriref_ontology, dct_conforms_to, vocab_uri))
-    ontouml_graph.add((uriref_ontology, dct_conforms_to, vocab_uri + "/vocabulary/v" + CONFORMS_TO_VOCAB_VERSION))
+    ontouml_graph.add((uriref_ontology, dct_conforms_to, vocab_uri + "/vocabulary/" + METADATA['conformsToVersion']))
 
     # Adding creation date
     date_format = "%Y-%m-%d"
     created_date = get_date_time(date_format)
     dct_created = URIRef(uri_dct + "created")
     ontouml_graph.add((uriref_ontology, dct_created, Literal(created_date, datatype=XSD.date)))
 
@@ -57,17 +57,17 @@
         language_uri = "http://dbpedia.org/resource/ISO_639:"
         ontouml_graph.add((uriref_ontology, dct_language, URIRef(language_uri + args.ARGUMENTS["language"])))
 
     # Adding type
     ontouml_graph.add((uriref_ontology, RDF.type, OWL.Ontology))
 
     # Adding generator information
-    comment_message = f"Generated by {SOFTWARE_NAME} v{SOFTWARE_VERSION}"
+    comment_message = f"Generated by {METADATA['name']} v{METADATA['version']}"
     ontouml_graph.add((uriref_ontology, RDFS.comment, Literal(comment_message)))
-    ontouml_graph.add((uriref_ontology, RDFS.seeAlso, Literal(SOFTWARE_URL, datatype=XSD.anyURI)))
+    ontouml_graph.add((uriref_ontology, RDFS.seeAlso, Literal(METADATA['repository'], datatype=XSD.anyURI)))
 
 
 def decode_dictionary(dictionary_data: dict, ontouml_graph: Graph, language: str) -> None:
     """ Receives the full dictionary with the loaded JSON data and decode known allowed values to the OntoUML Graph.
     Recursively evaluates the dictionary to create all possible instances, setting their types and attributes.
 
     OntoUML-Vocabulary properties that are directly decoded in the general decoder:
@@ -93,15 +93,15 @@
         return
 
     # Creating instance
     instance_uri = args.ARGUMENTS["base_uri"] + dictionary_data["id"]
     new_instance = URIRef(instance_uri)
 
     # Setting instance type
-    instance_type = URIRef(URI_ONTOUML + dictionary_data["type"])
+    instance_type = ontouml_ref(dictionary_data["type"])
     ontouml_graph.add((new_instance, RDF.type, instance_type))
 
     # Adding other attributes
     for key in dictionary_data.keys():
 
         # if id or type was already treated, skip
         if key == "id" or key == "type":
@@ -122,17 +122,17 @@
         if type(dictionary_data[key]) is dict:
             decode_dictionary(dictionary_data[key], ontouml_graph, language)
             continue
 
         # Graph's PREDICATE definition
         # May be direct or mapped
         if key not in mapped_fields.keys():
-            new_predicate = URIRef(URI_ONTOUML + key)
+            new_predicate = ontouml_ref(key)
         else:
-            new_predicate = URIRef(URI_ONTOUML + mapped_fields[key])
+            new_predicate = ontouml_ref(mapped_fields[key])
 
         # Graph's OBJECT definition
         if (key == "name") and language != "":
             new_object = Literal(dictionary_data[key], lang=language)
         elif key in positive_integer_fields:
             # Checking if is not integer (as int or as string)
             if type(dictionary_data[key]) is not int:
@@ -160,15 +160,15 @@
     :type execution_mode: str
     :return: Knowledge graph that complies with the OntoUML Vocabulary
     :rtype: Graph
     """
 
     # Creating OntoUML Graph
     ontouml_graph = Graph()
-    ontouml_graph.bind("ontouml", URI_ONTOUML)
+    ontouml_graph.bind("ontouml", METADATA["conformsToBase"])
     ontouml_graph.bind("", args.ARGUMENTS["base_uri"])
 
     # Get clean data
     # Dictionary data is all the JSON data loaded as a dictionary to be manipulated
     dictionary_data = clean_null_data(json_data)
 
     # GENERAL DECODING: creating all instances and setting their types.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_class.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     - Functions that set both object and data properties are named: set_<subject>_properties.
 """
 
 import inspect
 
 from rdflib import Graph, URIRef, XSD, Literal
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
-from modules.errors import report_error_end_of_switch
-from modules.globals import URI_ONTOUML
-from modules.messages import print_decode_log_message
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
+from ..errors import report_error_end_of_switch
+from ..messages import print_decode_log_message
+from ..utils_graph import ontouml_ref
 
 
 def validate_class_attribute_constraints(class_dict: dict) -> None:
     """ Verifies all Class dictionaries and check if the constraints related to classes were correctly considered and
     fixes them when they are not.
 
     The pair of attribute/stereotype: isExtensional/collective and isPowertype/type checked constraints are:
@@ -118,35 +118,35 @@
 
     class_stereotype = get_stereotype(class_dict)
 
     # DCA1: Setting ontouml:isExtensional default value to False when it's not set in a class with stereotype collective
     if "isExtensional" not in class_dict and class_stereotype == "collective":
         print_decode_log_message(class_dict, "DCA1", property_name='isExtensional', att_valid_stereotype='collective')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isExtensional"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isExtensional"), Literal(False, datatype=XSD.boolean)))
 
     # DCA2, DCA3, and DCA4 use the same message DGA1, as they are not associated to their holder's stereotype
 
     # DCA2: Setting ontouml:isPowertype attribute default value
     if "isPowertype" not in class_dict:
         print_decode_log_message(class_dict, "DGA1", property_name='isPowertype')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isPowertype"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isPowertype"), Literal(False, datatype=XSD.boolean)))
 
     # DCA3: Setting ontouml:isDerived attribute default value
     if "isDerived" not in class_dict:
         print_decode_log_message(class_dict, "DGA1", property_name='isDerived')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isDerived"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isDerived"), Literal(False, datatype=XSD.boolean)))
 
     # DCA4: Setting ontouml:isAbstract attribute default value
     if "isAbstract" not in class_dict:
         print_decode_log_message(class_dict, "DGA1", property_name='isAbstract')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isAbstract"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isAbstract"), Literal(False, datatype=XSD.boolean)))
 
 
 def set_defaults_class_order(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Verifies a class dictionary and check if their non-nullable attribute order was set or not.
     If not, creates default values.
 
     Default values checked are:
@@ -167,21 +167,21 @@
     # Setting ORDER attribute default value. Do nothing if the stereotype is unknown.
     if ("order" not in class_dict) and (class_stereotype != 'null'):
 
         # DCO1: 'order' default value = 1 when stereotype is not 'type'
         if class_stereotype != 'type':
             print_decode_log_message(class_dict, "DCO1", property_name='order')
             ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                               URIRef(URI_ONTOUML + "order"), Literal(1, datatype=XSD.nonNegativeInteger)))
+                               ontouml_ref("order"), Literal(1, datatype=XSD.nonNegativeInteger)))
 
         # DCO2: 'order' default value = 2 when stereotype is 'type'
         elif class_stereotype == 'type':
             print_decode_log_message(class_dict, "DCO2", property_name='order')
             ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                               URIRef(URI_ONTOUML + "order"), Literal(2, datatype=XSD.nonNegativeInteger)))
+                               ontouml_ref("order"), Literal(2, datatype=XSD.nonNegativeInteger)))
 
         # Unexpected value received for class_stereotype
         else:
             current_function = inspect.stack()[0][3]
             report_error_end_of_switch("class_stereotype", current_function)
 
 
@@ -207,16 +207,16 @@
     class_type = class_dict["type"]
 
     # If stereotype not declared, report warning.
     if class_stereotype == "null":
         print_decode_log_message(class_dict, "VCS1", "stereotype")
     else:
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "stereotype"),
-                           URIRef(URI_ONTOUML + class_dict['stereotype'])))
+                           ontouml_ref("stereotype"),
+                           ontouml_ref(class_dict['stereotype'])))
 
         # If declared but invalid, create and report error. Uses generic message with code 'VCSG'.
         if class_stereotype not in ENUM_CLASS_STEREOTYPE:
             print_decode_log_message(class_dict, "VCSG", property_name="stereotype")
 
 
 def set_class_order_nonnegativeinteger(class_dict: dict, ontouml_graph: Graph) -> None:
@@ -236,25 +236,25 @@
     # Case A: if 'order' field is null, it will receive the default value (see function set_class_defaults)
     if "order" not in class_dict:
         return
 
     # Case C: receives 0, representing an orderless class.
     elif class_dict["order"] == "*":
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "order"),
+                           ontouml_ref("order"),
                            Literal(0, datatype=XSD.nonNegativeInteger)))
 
     # Case A: remove invalid information so the field can be treated as null and then receive the default value.
     elif (type(class_dict["order"]) is int) and (class_dict["order"] <= 0):
         class_dict.pop("order")
 
     # Case B
     elif type(class_dict["order"]):
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "order"),
+                           ontouml_ref("order"),
                            Literal(class_dict['order'], datatype=XSD.nonNegativeInteger)))
 
     # Case A: remove invalid information so the field can be treated as null and then receive the default value.
     else:
         class_dict.pop("order")
 
 
@@ -281,16 +281,16 @@
         "type": "typeNature"
     }
 
     if "restrictedTo" in class_dict:
 
         for restriction in class_dict["restrictedTo"]:
             ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                               URIRef(URI_ONTOUML + "restrictedTo"),
-                               URIRef(URI_ONTOUML + restriction_nature_mapping[restriction])))
+                               ontouml_ref("restrictedTo"),
+                               ontouml_ref(restriction_nature_mapping[restriction])))
 
 
 def set_class_attributes(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Defines the ontouml:isPowertype and ontouml:isExtensional data properties of an ontouml:Class in the graph.
 
     This function must be called after the function set_class_defaults, as the received value may change because of
     identified problems.
@@ -299,20 +299,20 @@
     :type class_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     if "isExtensional" in class_dict:
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isExtensional"),
+                           ontouml_ref("isExtensional"),
                            Literal(class_dict["isExtensional"], datatype=XSD.boolean)))
 
     if "isPowertype" in class_dict:
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isPowertype"),
+                           ontouml_ref("isPowertype"),
                            Literal(class_dict["isPowertype"], datatype=XSD.boolean)))
 
 
 def set_class_attribute_property(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:attribute relation between an ontouml:Class and an ontouml:Property.
 
     :param class_dict: Class object loaded as a dictionary.
@@ -321,15 +321,15 @@
     :type ontouml_graph: Graph
     """
 
     list_related_properties = get_list_subdictionaries_for_specific_type(class_dict, "Property")
 
     for related_property in list_related_properties:
         statement_subject = URIRef(args.ARGUMENTS["base_uri"] + class_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "attribute")
+        statement_predicate = ontouml_ref("attribute")
         statement_object = URIRef(args.ARGUMENTS["base_uri"] + related_property["id"])
 
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_class_literal_literal(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:literal relation between an ontouml:Class and its related ontouml:Literal individuals.
@@ -340,15 +340,15 @@
     :type ontouml_graph: Graph
     """
 
     list_related_literals = get_list_subdictionaries_for_specific_type(class_dict, "Literal")
 
     for related_literal in list_related_literals:
         statement_subject = URIRef(args.ARGUMENTS["base_uri"] + class_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "literal")
+        statement_predicate = ontouml_ref("literal")
         statement_object = URIRef(args.ARGUMENTS["base_uri"] + related_literal["id"])
 
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def create_class_properties(json_data: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Main function for decoding an object of type 'Class'.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_diagram.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_diagram.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,31 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.globals import URI_ONTOUML, ELEMENT_VIEW_TYPES
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..globals import ELEMENT_VIEW_TYPES
+from ..utils_graph import ontouml_ref
 
 
 def set_diagram_owner_modelelement(diagram_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:owner property between an ontouml:Diagram and its related ontouml:Package.
 
     :param diagram_dict: Diagram object loaded as a dictionary.
     :type diagram_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     statement_subject = URIRef(args.ARGUMENTS["base_uri"] + diagram_dict["id"])
-    statement_predicate = URIRef(URI_ONTOUML + "owner")
+    statement_predicate = ontouml_ref("owner")
     statement_object = URIRef(args.ARGUMENTS["base_uri"] + diagram_dict["owner"]["id"])
     ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_diagram_containsview_elementview(diagram_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:containsView property between an ontouml:Diagram and its related ontouml:ElementView.
 
@@ -42,15 +43,15 @@
     list_related_elementviews = []
 
     for view_type in ELEMENT_VIEW_TYPES:
         list_related_elementviews += get_list_subdictionaries_for_specific_type(diagram_dict, view_type)
 
     for related_elementview in list_related_elementviews:
         statement_subject = URIRef(args.ARGUMENTS["base_uri"] + diagram_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "containsView")
+        statement_predicate = ontouml_ref("containsView")
         statement_object = URIRef(args.ARGUMENTS["base_uri"] + related_elementview["id"])
 
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def create_diagram_properties(json_data: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Main function for decoding objects of type 'Diagram'.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_elementview.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_elementview.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,19 @@
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 import inspect
 
 from rdflib import Graph, URIRef
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.errors import report_error_end_of_switch
-from modules.globals import URI_ONTOUML, ELEMENT_VIEW_TYPES
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..errors import report_error_end_of_switch
+from ..globals import ELEMENT_VIEW_TYPES
+from ..utils_graph import ontouml_ref
 
 
 def set_elementview_relations(elementview_dict: dict, ontouml_graph: Graph) -> None:
     """ Set an ontouml:ElementView's ontouml:shape and ontouml:isViewOf object properties in the resulting graph.
 
     :param elementview_dict: ElementView object loaded as a dictionary.
     :type elementview_dict: dict
@@ -36,32 +37,32 @@
         shape_name += "_path"
     else:
         current_function = inspect.stack()[0][3]
         report_error_end_of_switch("classview_dict['shape']['type']", current_function)
 
     # Setting shape property
     ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
-                       URIRef(URI_ONTOUML + "shape"),
+                       ontouml_ref("shape"),
                        URIRef(args.ARGUMENTS["base_uri"] + shape_name)))
 
     # Setting isViewOf property
     if "modelElement" in elementview_dict:
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
-                           URIRef(URI_ONTOUML + "isViewOf"),
+                           ontouml_ref("isViewOf"),
                            URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['modelElement']['id'])))
 
     # Setting sourceView and targetView properties
     if "source" in elementview_dict:
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
-                           URIRef(URI_ONTOUML + "sourceView"),
+                           ontouml_ref("sourceView"),
                            URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['source']['id'])))
 
     if "target" in elementview_dict:
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
-                           URIRef(URI_ONTOUML + "targetView"),
+                           ontouml_ref("targetView"),
                            URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['target']['id'])))
 
 
 def create_elementview_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type ElementView.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_generalization.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_generalization.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.globals import URI_ONTOUML
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..utils_graph import ontouml_ref
 
 
 def set_generalization_relations(generalization_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:general and ontouml:specific properties in the resulting graph.
 
     :param generalization_dict: Generalization object loaded as a dictionary.
     :type generalization_dict: dict
@@ -24,16 +24,16 @@
     :type ontouml_graph: Graph
     """
 
     generalization_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict['id'])
     general_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict["general"]['id'])
     specific_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict["specific"]['id'])
 
-    ontouml_graph.add((generalization_individual, URIRef(URI_ONTOUML + "general"), general_individual))
-    ontouml_graph.add((generalization_individual, URIRef(URI_ONTOUML + "specific"), specific_individual))
+    ontouml_graph.add((generalization_individual, ontouml_ref("general"), general_individual))
+    ontouml_graph.add((generalization_individual, ontouml_ref("specific"), specific_individual))
 
 
 def create_generalization_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type Generalization.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
     object's type is domain of.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_generalizationset.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_generalizationset.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef, Literal, XSD
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.globals import URI_ONTOUML
-from modules.messages import print_decode_log_message
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..messages import print_decode_log_message
+from ..utils_graph import ontouml_ref
 
 
 def set_generalizationset_defaults(generalizationset_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the default values to ontouml:generalizationSets to the resulting graph.
 
     - Default isDisjoint: If isDisjoint is null, set as False.
     - Default isComplete: If isComplete is null, set as False.
@@ -29,35 +29,35 @@
     """
 
     generalizationset_individual = URIRef(args.ARGUMENTS["base_uri"] + generalizationset_dict['id'])
     set_false = Literal(False, datatype=XSD.boolean)
 
     if "isDisjoint" not in generalizationset_dict:
         print_decode_log_message(generalizationset_dict, "DGA1", property_name="isDisjoint")
-        is_disjoint_property = URIRef(URI_ONTOUML + "isDisjoint")
+        is_disjoint_property = ontouml_ref("isDisjoint")
         ontouml_graph.add((generalizationset_individual, is_disjoint_property, set_false))
 
     if "isComplete" not in generalizationset_dict:
         print_decode_log_message(generalizationset_dict, "DGA1", property_name="isComplete")
-        is_complete_property = URIRef(URI_ONTOUML + "isComplete")
+        is_complete_property = ontouml_ref("isComplete")
         ontouml_graph.add((generalizationset_individual, is_complete_property, set_false))
 
 
 def set_generalizationset_relations(generalizationset_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the ontouml:generalization and ontouml:categorizer property to the resulting graph.
 
     :param generalizationset_dict: GeneralizationSet object loaded as a dictionary.
     :type generalizationset_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     generalizationset_individual = URIRef(args.ARGUMENTS["base_uri"] + generalizationset_dict['id'])
-    generalization_property = URIRef(URI_ONTOUML + "generalization")
-    categorizer_property = URIRef(URI_ONTOUML + "categorizer")
+    generalization_property = ontouml_ref("generalization")
+    categorizer_property = ontouml_ref("categorizer")
 
     # Setting ontouml:generalization property
     for generalization_dict in generalizationset_dict["generalizations"]:
         generalization_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict["id"])
         ontouml_graph.add((generalizationset_individual, generalization_property, generalization_individual))
 
     # Setting ontouml:categorizer property
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_package.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.globals import URI_ONTOUML
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..utils_graph import ontouml_ref
 
 
 def get_package_contents(package_dict: dict, package_id: str, list_contents: list = []) -> list[dict]:
     """ Receives the dictionary with all loaded JSON data and returns the value of the 'contents' field for a given
     object (defined by the received value of its ID).
 
     :param package_dict: Package's data to have its fields decoded.
@@ -80,15 +80,15 @@
         list_related_ids = []
         for content in package_id_contents_list:
             list_related_ids.append(content["id"])
 
         # Include found related elements in graph using ontouml:containsModelElement
         for related_id in list_related_ids:
             ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + package_dict["id"]),
-                               URIRef(URI_ONTOUML + "containsModelElement"),
+                               ontouml_ref("containsModelElement"),
                                URIRef(args.ARGUMENTS["base_uri"] + related_id)))
 
 
 def create_package_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type Package.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_path.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
-from modules.globals import URI_ONTOUML
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
+from ..utils_graph import ontouml_ref
 
 
 def set_path_path_point(path_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:point of an ontouml:Path.
 
     :param path_dict: Path object loaded as a dictionary.
     :type path_dict: dict
@@ -30,15 +30,15 @@
     for point_dict in path_dict["points"]:
         # Creating new Point instance
         point_name = base_point_name + str(point_counter)
         create_point(point_name, point_dict["x"], point_dict["y"], ontouml_graph)
 
         # Associating new Point with the Path
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + path_dict["id"]),
-                           URIRef(URI_ONTOUML + "point"),
+                           ontouml_ref("point"),
                            URIRef(args.ARGUMENTS["base_uri"] + point_name)))
 
         point_counter += 1
 
 
 def create_path_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type Path.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_project.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_all_ids_of_specific_type, get_list_subdictionaries_for_specific_type
-from modules.globals import URI_ONTOUML
+from .. import arguments as args
+from ..decoder.decode_general import get_all_ids_of_specific_type, get_list_subdictionaries_for_specific_type
+from ..utils_graph import ontouml_ref
 
 
 def set_ontoumlelement_project_project(project_dict: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Sets the ontouml:project object property between an ontouml:Project (obj) and all its related entities (subj).
 
     :param project_dict: Project's data to have its fields decoded.
     :type project_dict: dict
@@ -34,15 +34,15 @@
             continue
 
         # Get every project's related objects' ids
         list_objects_ids = get_all_ids_of_specific_type(project_dict, available_type)
 
         for json_object_id in list_objects_ids:
             statement_subject = URIRef(args.ARGUMENTS["base_uri"] + json_object_id)
-            statement_predicate = URIRef(URI_ONTOUML + "project")
+            statement_predicate = ontouml_ref("project")
             statement_object = URIRef(args.ARGUMENTS["base_uri"] + project_dict["id"])
             ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_project_model_package(project_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:model relation between an ontouml:Project and its related model.
 
@@ -50,15 +50,15 @@
     :type project_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     if "model" in project_dict:
         statement_subject = URIRef(args.ARGUMENTS["base_uri"] + project_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "model")
+        statement_predicate = ontouml_ref("model")
         statement_object = URIRef(args.ARGUMENTS["base_uri"] + project_dict["model"]["id"])
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_project_diagram_diagram(project_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the ontouml:diagram object property between an ontouml:Project and its related ontouml:Diagram entities.
 
@@ -69,15 +69,15 @@
     """
 
     # Getting all Diagrams for a specific Project
     list_all_diagram_ids = get_all_ids_of_specific_type(project_dict, "Diagram")
 
     for diagram_id in list_all_diagram_ids:
         statement_subject = URIRef(args.ARGUMENTS["base_uri"] + project_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "diagram")
+        statement_predicate = ontouml_ref("diagram")
         statement_object = URIRef(args.ARGUMENTS["base_uri"] + diagram_id)
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def create_project_properties(json_data: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Main function for decoding objects of type 'Project'.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_property.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_property.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,35 +6,34 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef, RDF, Literal, XSD
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
-from modules.globals import URI_ONTOUML
-from modules.logger import initialize_logger
-from modules.messages import print_decode_log_message
-from modules.sparql_queries import GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE
-from modules.utils_graph import load_ontouml_vocabulary
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
+from ..logger import initialize_logger
+from ..messages import print_decode_log_message
+from ..sparql_queries import GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE
+from ..utils_graph import load_ontouml_vocabulary, ontouml_ref
 
 LOGGER = initialize_logger()
 
 
 def validate_property_stereotype(ontouml_graph: Graph) -> None:
     """ Performs syntactical and semantic validations on an ontouml:Property's stereotype.
 
     Differently from what is used in the validation of other JSON objects, this function manipulates the graph itself,
     not the JSON object. This is because it is much straightforward to access all the necessary property elements.
 
     Validations performed:
     VPS1) Reports invalid property stereotypes (i.e., stereotypes different from ontouml:begin or ontouml:end).
     VPS2) Reports if a property stereotype is used in association with an invalid class stereotype.
-        I.e., a class stereotype that is known and different from 'event'.
+    I.e., a class stereotype that is known and different from 'event'.
     VPS3) Sets class stereotype as 'event' when it is associated to a property that has an assigned valid stereotype.
 
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     if not args.ARGUMENTS["correct"]:
@@ -66,16 +65,16 @@
         elif class_stereotype == "null":
 
             dict_argument = {"type": "Class", "name": class_name, "id": class_id, "stereotype": class_stereotype,
                              "propID": property_id, "propST": property_stereotype}
             print_decode_log_message(dict_argument, "VPS3")
 
             ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_id),
-                               URIRef(URI_ONTOUML + "stereotype"),
-                               URIRef(URI_ONTOUML + "event")))
+                               ontouml_ref("stereotype"),
+                               ontouml_ref("event")))
 
 
 def set_property_defaults(property_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets default values for ontouml:Property elements that do not present them. The defaults are:
     
     DPA1) ontouml:isDerived default value = False
     DPA2) ontouml:isOrdered default value = False
@@ -89,27 +88,27 @@
 
     # DPA1, DPA2, and DPA3 use the same message DGA1, as they are not associated to their holder's stereotype.
 
     # DPA1: Setting ontouml:isDerived attribute default value
     if "isDerived" not in property_dict:
         print_decode_log_message(property_dict, "DGA1", property_name='isDerived')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + property_dict['id']),
-                           URIRef(URI_ONTOUML + "isDerived"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isDerived"), Literal(False, datatype=XSD.boolean)))
 
     # DPA2: Setting ontouml:isOrdered attribute default value
     if "isOrdered" not in property_dict:
         print_decode_log_message(property_dict, "DGA1", property_name='isOrdered')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + property_dict['id']),
-                           URIRef(URI_ONTOUML + "isOrdered"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isOrdered"), Literal(False, datatype=XSD.boolean)))
 
     # DPA3: Setting ontouml:isReadOnly attribute default value
     if "isReadOnly" not in property_dict:
         print_decode_log_message(property_dict, "DGA1", property_name='isReadOnly')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + property_dict['id']),
-                           URIRef(URI_ONTOUML + "isReadOnly"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isReadOnly"), Literal(False, datatype=XSD.boolean)))
 
 
 def set_property_relations(property_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the ontouml:aggregationKind and ontouml:propertyType object properties between an ontouml:Property and
     its related elements.
 
     :param property_dict: Property object loaded as a dictionary.
@@ -118,44 +117,44 @@
     :type ontouml_graph: Graph
     """
 
     statement_subject = URIRef(args.ARGUMENTS["base_uri"] + property_dict["id"])
 
     # Setting ontouml:aggregationKind
     if "aggregationKind" not in property_dict:
-        statement_object = URIRef(URI_ONTOUML + "none")
+        statement_object = ontouml_ref("none")
     else:
-        statement_object = URIRef(URI_ONTOUML + property_dict["aggregationKind"].lower())
+        statement_object = ontouml_ref(property_dict["aggregationKind"].lower())
 
-    statement_predicate = URIRef(URI_ONTOUML + "aggregationKind")
+    statement_predicate = ontouml_ref("aggregationKind")
     ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:propertyType
     if "propertyType" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "propertyType")
+        statement_predicate = ontouml_ref("propertyType")
         statement_object = URIRef(args.ARGUMENTS["base_uri"] + property_dict["propertyType"]["id"])
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:stereotype. Its validation is performed later in function validate_property_stereotype
     if "stereotype" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "stereotype")
-        statement_object = URIRef(URI_ONTOUML + property_dict["stereotype"])
+        statement_predicate = ontouml_ref("stereotype")
+        statement_object = ontouml_ref(property_dict["stereotype"])
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:subsetsProperty
     if "subsettedProperties" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "subsetsProperty")
+        statement_predicate = ontouml_ref("subsetsProperty")
 
         for subsetted_prop_dict in property_dict["subsettedProperties"]:
             statement_object = URIRef(args.ARGUMENTS["base_uri"] + subsetted_prop_dict["id"])
             ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:redefinesProperty
     if "redefinedProperties" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "redefinesProperty")
+        statement_predicate = ontouml_ref("redefinesProperty")
 
         for redefined_prop_dict in property_dict["redefinedProperties"]:
             statement_object = URIRef(args.ARGUMENTS["base_uri"] + redefined_prop_dict["id"])
             ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def determine_cardinality_bounds(cardinalities: str, property_id: str) -> (str, str, str):
@@ -201,20 +200,20 @@
     :type ontouml_graph: Graph
     """
 
     if "cardinality" in property_dict:
         ontology_property_individual = URIRef(args.ARGUMENTS["base_uri"] + property_dict["id"])
         ontology_cardinality_individual = URIRef(args.ARGUMENTS["base_uri"] + property_dict["id"] + '_cardinality')
 
-        ontouml_cardinality_class = URIRef(URI_ONTOUML + "Cardinality")
-        ontouml_cardinality_property = URIRef(URI_ONTOUML + "cardinality")
+        ontouml_cardinality_class = ontouml_ref("Cardinality")
+        ontouml_cardinality_property = ontouml_ref("cardinality")
 
-        ontouml_cardinalityvalue_property = URIRef(URI_ONTOUML + "cardinalityValue")
-        ontouml_lowerbound_property = URIRef(URI_ONTOUML + "lowerBound")
-        ontouml_upperbound_property = URIRef(URI_ONTOUML + "upperBound")
+        ontouml_cardinalityvalue_property = ontouml_ref("cardinalityValue")
+        ontouml_lowerbound_property = ontouml_ref("lowerBound")
+        ontouml_upperbound_property = ontouml_ref("upperBound")
 
         # Creating ontouml:Cardinality individuals (named after its related Property's name + '_cardinality' string)
         ontouml_graph.add((ontology_cardinality_individual, RDF.type, ontouml_cardinality_class))
 
         # Setting the ontouml:cardinality between an ontouml:Property and its ontouml:Cardinality
         ontouml_graph.add((ontology_property_individual, ontouml_cardinality_property, ontology_cardinality_individual))
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_rectangularshape.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_rectangularshape.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
-from modules.globals import URI_ONTOUML
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
+from ..utils_graph import ontouml_ref
 
 
 def set_rectangularshape_coordinates(rectangularshape_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:topLeftPosition of an ontouml:RectangularShape.
 
     :param rectangularshape_dict: RectangularShape object loaded as a dictionary.
     :type rectangularshape_dict: dict
@@ -26,15 +26,15 @@
 
     # Creating new Point instance
     point_name = rectangularshape_dict["id"] + "_point"
     create_point(point_name, rectangularshape_dict["x"], rectangularshape_dict["y"], ontouml_graph)
 
     # Associating new Point with Rectangle
     ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + rectangularshape_dict["id"]),
-                       URIRef(URI_ONTOUML + "topLeftPosition"),
+                       ontouml_ref("topLeftPosition"),
                        URIRef(args.ARGUMENTS["base_uri"] + point_name)))
 
 
 def create_rectangularshape_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type RectangularShape.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/decoder/decode_obj_relation.py` & `ontouml_json2graph-1.0.1/json2graph/modules/decoder/decode_obj_relation.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef, Literal, XSD
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
-from modules.globals import URI_ONTOUML
-from modules.messages import print_decode_log_message
+from .. import arguments as args
+from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
+from ..messages import print_decode_log_message
+from ..utils_graph import ontouml_ref
 
 
 def set_relation_defaults(relation_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the following attribute's default values for ontouml:Relation:
 
     DRA1) ontouml:isDerived default value = False
     DRA2) ontouml:isAbstract default value = False
@@ -30,21 +30,21 @@
 
     # DRA1, and DRA2 use the same message DGA1, as they are not associated to their holder's stereotype.
 
     # DCA3: Setting ontouml:isDerived attribute default value
     if "isDerived" not in relation_dict:
         print_decode_log_message(relation_dict, "DGA1", property_name='isDerived')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id']),
-                           URIRef(URI_ONTOUML + "isDerived"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isDerived"), Literal(False, datatype=XSD.boolean)))
 
     # DCA4: Setting ontouml:isAbstract attribute default value
     if "isAbstract" not in relation_dict:
         print_decode_log_message(relation_dict, "DGA1", property_name='isAbstract')
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id']),
-                           URIRef(URI_ONTOUML + "isAbstract"), Literal(False, datatype=XSD.boolean)))
+                           ontouml_ref("isAbstract"), Literal(False, datatype=XSD.boolean)))
 
 
 def set_relation_stereotype(relation_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:stereotype property between an instance of ontouml:Relation and an instance representing an
     ontouml:RelationStereotype.
 
     Warning messages:
@@ -61,16 +61,16 @@
                                 "manifestation", "material", "mediation", "memberOf", "participation",
                                 "participational", "subCollectionOf", "subQuantityOf", "termination", "triggers"]
 
     relation_stereotype = get_stereotype(relation_dict)
 
     if relation_stereotype != "null":
         ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id']),
-                           URIRef(URI_ONTOUML + "stereotype"),
-                           URIRef(URI_ONTOUML + relation_dict['stereotype'])))
+                           ontouml_ref("stereotype"),
+                           ontouml_ref(relation_dict['stereotype'])))
 
         # If declared but invalid, create and report error. Uses generic message with code 'VCSG'.
         if relation_stereotype not in ENUM_RELATION_STEREOTYPE:
             print_decode_log_message(relation_dict, "VCSG", property_name="stereotype")
 
 
 def set_relation_relations(relation_dict: dict, ontouml_graph: Graph) -> None:
@@ -82,17 +82,17 @@
     :param relation_dict: Relation object loaded as a dictionary.
     :type relation_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     relation_individual = URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id'])
-    uri_relation_end = URIRef(URI_ONTOUML + "relationEnd")
-    uri_relation_sourceend = URIRef(URI_ONTOUML + "sourceEnd")
-    uri_relation_targetend = URIRef(URI_ONTOUML + "targetEnd")
+    uri_relation_end = ontouml_ref("relationEnd")
+    uri_relation_sourceend = ontouml_ref("sourceEnd")
+    uri_relation_targetend = ontouml_ref("targetEnd")
 
     ends_list = []
     for property_dict in relation_dict["properties"]:
         ends_list.append(property_dict["id"])
 
     source_id = URIRef(args.ARGUMENTS["base_uri"] + ends_list[0])
     target_id = URIRef(args.ARGUMENTS["base_uri"] + ends_list[1])
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/errors.py` & `ontouml_json2graph-1.0.1/json2graph/modules/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Functions related to the verification and treatment of identified ERROR cases. """
 
-from modules.logger import initialize_logger
+from .logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def report_error_requirement_not_met(error_message: str) -> None:
     """ Reports the error caused when a requirement is not met. As this is a generic function, the error message
     parameter must be used to identify the error to the user.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/input_output.py` & `ontouml_json2graph-1.0.1/json2graph/modules/input_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import json
 import os
 from pathlib import Path
 
 from rdflib import Graph
 
-from modules.errors import report_error_io_read, report_error_io_write
-from modules.logger import initialize_logger
+from .errors import report_error_io_read, report_error_io_write
+from .logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def create_directory_if_not_exists(directory_path: str, file_description: str) -> None:
     """ Checks if the directory that has the path received as argument exists.
     If it does, do nothing. If it does not, create it.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/logger.py` & `ontouml_json2graph-1.0.1/json2graph/modules/logger.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/messages.py` & `ontouml_json2graph-1.0.1/json2graph/modules/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Decoding messages to be displayed to users must be concentrated in this module whenever possibile. """
 import inspect
 
-import modules.arguments as args
-from modules.decoder.decode_general import get_stereotype
-from modules.errors import report_error_end_of_switch
-from modules.logger import initialize_logger
+from . import arguments as args
+from .decoder.decode_general import get_stereotype
+from .errors import report_error_end_of_switch
+from .logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def get_decode_log_message(object_dict: dict, warning_code: str, property_name: str,
                            att_valid_stereotype: str = "") -> str:
     """ Mounts and returns a warning message according to the information received as parameter.
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/sparql_queries.py` & `ontouml_json2graph-1.0.1/json2graph/modules/sparql_queries.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/utils_general.py` & `ontouml_json2graph-1.0.1/json2graph/modules/utils_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/modules/utils_graph.py` & `ontouml_json2graph-1.0.1/json2graph/modules/utils_graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 """ Util functions related to graphs. """
 
 from rdflib import Graph, URIRef, RDF
 
-from modules.errors import report_error_io_read
-from modules.globals import URI_ONTOUML, CONFORMS_TO_VOCAB_VERSION
-from modules.logger import initialize_logger
+from .errors import report_error_io_read
+from .globals import METADATA
+from .logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
+def ontouml_ref(entity: str) -> URIRef:
+    """ Receives the name of the OntoUML Vocabulary's entity as a string and returns the corresponding URIRef.
+
+    :param entity: OntoUML Vocabulary entity (class, property, or individual) to have its URIRef returned.
+    :type entity: str
+    :return: URIRef of the informed OntoUML Vocabulary's entity.
+    :rtype: URIRef
+    """
+
+    entity_uri = METADATA["conformsTo"] + "#" + entity
+
+    entity_uriref = URIRef(entity_uri)
+
+    return entity_uriref
+
+
 def load_ontouml_vocabulary() -> Graph:
     """ Loads the OntoUML Vocabulary to the working memory. First tries to load from web resource, if fails, it tries to
     load form the local resource. If both options fail, calls error reporting function.
 
     :return: RDFLib graph loaded as object.
     :rtype: Graph
     """
 
     ontology_graph = Graph()
 
-    remote_option = "https://github.com/OntoUML/ontouml-vocabulary/releases/download/v" + \
-                    CONFORMS_TO_VOCAB_VERSION + "/ontouml.ttl"
+    remote_option = "https://github.com/OntoUML/ontouml-vocabulary/releases/download/" + \
+                    METADATA['conformsToVersion'] + "/ontouml.ttl"
     local_option = "resources/ontouml_v110.ttl"
 
     try:
         ontology_graph.parse(remote_option, encoding='utf-8', format="ttl")
-        LOGGER.debug(f"OntoUML Vocabulary successfully loaded to working memory from remote option.")
+        LOGGER.debug("OntoUML Vocabulary successfully loaded to working memory from remote option.")
     except:
         try:
             ontology_graph.parse(local_option, encoding='utf-8', format="ttl")
-            LOGGER.debug(f"OntoUML Vocabulary successfully loaded to working memory from local option.")
+            LOGGER.debug("OntoUML Vocabulary successfully loaded to working memory from local option.")
         except OSError as error:
             report_error_io_read("OntoUML Vocabulary", "from remote or local sources the", error)
 
     return ontology_graph
 
 
 def load_graph_safely(ontology_file: str, format: str = "not_provided") -> Graph:
@@ -72,12 +88,12 @@
     :param element_type: Type of the element (originally a JSON object) to be queried to have their ids returned .
     :type element_type: list[str]
     """
 
     list_of_ids_of_type = []
 
     # Getting the ID of all OntoUML Elements that are of element_type
-    for element in ontology_graph.subjects(RDF.type, URIRef(URI_ONTOUML + element_type)):
+    for element in ontology_graph.subjects(RDF.type, ontouml_ref(element_type)):
         element = element.fragment
         list_of_ids_of_type.append(element)
 
     return list_of_ids_of_type
```

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/resources/ontouml_v100.ttl` & `ontouml_json2graph-1.0.1/json2graph/resources/ontouml_v100.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0/ontouml-json2graph/resources/ontouml_v110.ttl` & `ontouml_json2graph-1.0.1/json2graph/resources/ontouml_v110.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -1,94 +1,87 @@
-@prefix :        <https://w3id.org/ontouml#> .
 @prefix dcat:    <http://www.w3.org/ns/dcat#> .
 @prefix dct:     <http://purl.org/dc/terms/> .
 @prefix foaf:    <http://xmlns.com/foaf/0.1/> .
 @prefix ontouml: <https://w3id.org/ontouml#> .
 @prefix owl:     <http://www.w3.org/2002/07/owl#> .
 @prefix rdf:     <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rdfs:    <http://www.w3.org/2000/01/rdf-schema#> .
-@prefix sdo:     <https://schema.org/> .
 @prefix vann:    <http://purl.org/vocab/vann/> .
 @prefix xml:     <http://www.w3.org/XML/1998/namespace> .
 @prefix xsd:     <http://www.w3.org/2001/XMLSchema#> .
 @base <https://w3id.org/ontouml> .
 
+
 #################################################################
 #    Metadata
 #################################################################
 
 <https://w3id.org/ontouml>
-    rdf:type                                                                                    owl:Ontology,
-                                                                                                dct:Standard ;
+    rdf:type                      owl:Ontology, dct:Standard ;
 
 ################################################################# VERSIONING
 
-    owl:versionIRI                                                                              <https://w3id.org/ontouml/1.1.0> ;
-    owl:versionInfo                                                                             "General review for compliance with the OntoUML Metamodel 1.1.0."@en ;
-    owl:priorVersion                                                                            <https://w3id.org/ontouml/1.0.0> ;
-    dct:issued                                                                                  "2022-04-03"^^xsd:date ;
-    dct:modified                                                                                "2023-07-23"^^xsd:date ;
+    owl:versionIRI                <https://w3id.org/ontouml/vocabulary/v1.1.0> ;
+    owl:versionInfo               "General review for compliance with the OntoUML Metamodel 1.1.1."@en ;
+    owl:priorVersion              <https://w3id.org/ontouml/vocabulary/v1.0.0> ;
+    dct:issued                    "2022-04-03"^^xsd:date ;
+    dct:modified                  "2023-07-27"^^xsd:date ;
 
 ################################################################# IDENTIFICATION
 
-    dct:title                                                                                   "OntoUML Metamodel Vocabulary"@en ;
-    dct:description                                                                             "A reference implementation of the OntoUML Metamodel in OWL."@en ;
-    dct:identifier                                                                              "https://w3id.org/ontouml"^^xsd:anyURI ;
-    dct:license                                                                                 <https://creativecommons.org/licenses/by-sa/4.0> ;
-    dct:conformsTo                                                                              <https://w3id.org/ontouml/metamodel/v1.1.0> ;
-    dcat:landingPage                                                                            <https://w3id.org/ontouml/vocabulary> ;
-    vann:preferredNamespacePrefix                                                               "ontouml" ;
-    vann:preferredNamespaceUri                                                                  "https://w3id.org/ontouml#"^^xsd:anyURI ;
-    foaf:homepage                                                                               <https://purl.org/> ;
-    dct:language                                                                                <http://id.loc.gov/vocabulary/iso639-1/en> ;
-    dct:isReferencedBy                                                                          <https://dblp.org/rec/conf/jowo/FonsecaSVFGA21.html>,
-                                                                                                <https://doi.org/10.1007/978-3-031-17995-2_1> ;
-    dcat:keyword                                                                                "OntoUML"@en,
-                                                                                                "OntoUML-Metamodel"@en,
-                                                                                                "OntoUML-Vocabulary"@en,
-                                                                                                "Ontology-Driven Conceptual Modeling"@en ;
+    dct:title                     "OntoUML Vocabulary"@en ;
+    dct:description               "An OWL vocabulary to allow the serialization and exchanging of OntoUML models in conformance with the Ontouml Metamodel."@en ;
+    dct:identifier                "https://w3id.org/ontouml"^^xsd:anyURI ;
+    dct:license                   <https://creativecommons.org/licenses/by-sa/4.0> ;
+    dct:conformsTo                <https://w3id.org/ontouml/metamodel/v1.1.1> ;
+    dcat:landingPage              <https://w3id.org/ontouml/vocabulary> ;
+    foaf:homepage                 <https://w3id.org/ontouml/vocabulary/docs> ;
+    vann:preferredNamespacePrefix "ontouml" ;
+    vann:preferredNamespaceUri    "https://w3id.org/ontouml#"^^xsd:anyURI ;
+    dct:language                  <http://id.loc.gov/vocabulary/iso639-1/en> ;
+    dct:isReferencedBy            <https://dblp.org/rec/conf/jowo/FonsecaSVFGA21.html>,
+                                  <https://doi.org/10.1007/978-3-031-17995-2_1> ;
+    dcat:keyword                  "OntoUML"@en, "OntoUML-Metamodel"@en, "Ontology-Driven Conceptual Modeling"@en ;
 
 ################################################################# AUTHORSHIP
 
-    dct:publisher                                                                               <https://www.utwente.nl/en/eemcs/scs/> ;
-    dct:creator                                                                                 [ sdo:name
-                                                                                                          "Tiago Prince Sales"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0002-5385-5761> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.utwente.nl/en/eemcs/scs/> ; ],
-                                                                                                [ sdo:name
-                                                                                                          "Claudenir M. Fonseca"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0003-2528-3118> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.utwente.nl/en/eemcs/scs/> ; ],
-                                                                                                [ sdo:name
-                                                                                                          "Pedro Paulo Favato Barcelos"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0003-2736-7817> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.utwente.nl/en/eemcs/scs/> ; ] ;
-    dct:contributor                                                                             [ sdo:name
-                                                                                                          "Mattia Fumagalli"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0003-3385-4769> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.inf.unibz.it/krdb/> ; ] .
-
+    dct:publisher                 <https://www.utwente.nl/en/eemcs/scs/> ;
+    dct:creator                   <https://orcid.org/0000-0002-5385-5761>, <https://orcid.org/0000-0003-2528-3118>,
+                                  <https://orcid.org/0000-0003-2736-7817> ;
+    dct:contributor               <https://orcid.org/0000-0003-3385-4769> .
 
 <https://www.inf.unibz.it/krdb/>
-    rdf:type sdo:Organization ;
-    sdo:name "KRDB Research Centre for Knowledge and Data, Free University of Bozen-Bolzano, Italy" ;
-    sdo:url  "https://www.inf.unibz.it/krdb/"^^xsd:anyURI .
+    rdf:type      foaf:Organization ;
+    foaf:name     "KRDB Research Centre for Knowledge and Data, Free University of Bozen-Bolzano, Italy" ;
+    foaf:homepage "https://www.inf.unibz.it/krdb/"^^xsd:anyURI ;
+    foaf:member   <https://orcid.org/0000-0003-3385-4769> .
 
 <https://www.utwente.nl/en/eemcs/scs/>
-    rdf:type sdo:Organization ;
-    sdo:name "Semantics, Cybersecurity & Services (SCS), University of Twente, the Netherlands" ;
-    sdo:url  "https://www.utwente.nl/en/eemcs/scs/"^^xsd:anyURI .
+    rdf:type      foaf:Organization ;
+    foaf:name     "Semantics, Cybersecurity & Services (SCS), University of Twente, the Netherlands" ;
+    foaf:homepage "https://www.utwente.nl/en/eemcs/scs/"^^xsd:anyURI ;
+    foaf:member   <https://orcid.org/0000-0002-5385-5761>, <https://orcid.org/0000-0003-2528-3118>,
+                  <https://orcid.org/0000-0003-2736-7817> .
+
+<https://orcid.org/0000-0003-3385-4769>
+    foaf:name "Mattia Fumagalli" ;
+    foaf:mbox "mattia.fumagalli@unibz.it" .
+
+<https://orcid.org/0000-0002-5385-5761>
+    foaf:name "Tiago Prince Sales" ;
+    foaf:mbox "t.princesales@utwente.nl" .
+
+<https://orcid.org/0000-0003-2528-3118>
+    foaf:name "Claudenir M. Fonseca" ;
+    foaf:mbox "c.moraisfonseca@utwente.nl" .
+
+<https://orcid.org/0000-0003-2736-7817>
+    foaf:name "Pedro Paulo Favato Barcelos" ;
+    foaf:mbox "p.p.favatobarcelos@uwente.nl" .
+
 
 #################################################################
 #    Object Properties
 #################################################################
 
 ###  https://w3id.org/ontouml#aggregationKind
 ontouml:aggregationKind
@@ -124,16 +117,16 @@
 ###  https://w3id.org/ontouml#categorizer
 ontouml:categorizer
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:GeneralizationSet ;
     rdfs:range       ontouml:Class ;
     rdfs:label       "categorizer"@en ;
     rdfs:isDefinedBy <https://w3id.org/ontouml> ;
-    rdfs:comment     "Identifies individuals of an ontouml:GeneralizationSet that are instances of a higher order ontouml:Class."@en ;
-    rdfs:seeAlso     <https://doi.org/10.1007/978-3-319-39696-5_19> .
+    rdfs:comment     " Identifies the ontouml:Class that is instantiated by the specific classes of the ontouml:Generalization type composing the ontouml:GeneralizationSet"@en ;
+    rdfs:seeAlso     <https://doi.org/10.1016/j.datak.2022.102012>, <https://doi.org/10.1007/978-3-031-17995-2_2> .
 
 
 ###  https://w3id.org/ontouml#containsModelElement
 ontouml:containsModelElement
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:Package ;
     rdfs:range       ontouml:ModelElement ;
@@ -344,15 +337,15 @@
 ###  https://w3id.org/ontouml#stereotype
 ontouml:stereotype
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:DecoratableElement ;
     rdfs:range       ontouml:Stereotype ;
     rdfs:label       "stereotype"@en ;
     rdfs:isDefinedBy <https://w3id.org/ontouml> ;
-    rdfs:comment     "Identifies an ontouml:Stereotype applied to an ontouml:DecoratableElement."@en .
+    rdfs:comment     "Identifies the ontouml:Stereotype applied to the ontouml:DecoratableElement."@en .
 
 
 ###  https://w3id.org/ontouml#subsetsProperty
 ontouml:subsetsProperty
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:Property ;
     rdfs:range       ontouml:Property ;
@@ -375,15 +368,15 @@
 ###  https://w3id.org/ontouml#targetView
 ontouml:targetView
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:ConnectorView ;
     rdfs:range       ontouml:ElementView ;
     rdfs:label       "targetView"@en ;
     rdfs:isDefinedBy <https://w3id.org/ontouml> ;
-    rdfs:comment     "Identifies an ontouml:ElementView that participates as target of an ontouml:RelationView or ontouml:GeneralizationView."@en .
+    rdfs:comment     "Identifies an ontouml:ElementView that participates as target of an ontouml:ConnectorView."@en .
 
 
 ###  https://w3id.org/ontouml#topLeftPosition
 ontouml:topLeftPosition
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:RectangularShape ;
     rdfs:range       ontouml:Point ;
```

