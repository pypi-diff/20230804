# Comparing `tmp/frouros-0.5.1.tar.gz` & `tmp/frouros-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.5.1.tar", last modified: Sat Jul 22 14:52:29 2023, max compression
+gzip compressed data, was "frouros-0.6.0.tar", last modified: Fri Aug  4 15:43:35 2023, max compression
```

## Comparing `frouros-0.5.1.tar` & `frouros-0.6.0.tar`

### file list

```diff
@@ -1,135 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.180122 frouros-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-22 14:52:16.000000 frouros-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-22 14:52:16.000000 frouros-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-22 14:52:29.180122 frouros-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    22052 2023-07-22 14:52:16.000000 frouros-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5358 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     7281 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9068 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    15055 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.180122 frouros-0.5.1/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/kernels.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7360 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-22 14:52:28.000000 frouros-0.5.1/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4962 2023-07-22 14:52:29.000000 frouros-0.5.1/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:52:28.000000 frouros-0.5.1/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:52:28.000000 frouros-0.5.1/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-22 14:52:29.000000 frouros-0.5.1/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-22 14:52:29.000000 frouros-0.5.1/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-22 14:52:16.000000 frouros-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 14:52:29.180122 frouros-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-07-22 14:52:16.000000 frouros-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.379654 frouros-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-08-04 15:43:22.000000 frouros-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-04 15:43:22.000000 frouros-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    25160 2023-08-04 15:43:35.379654 frouros-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23539 2023-08-04 15:43:22.000000 frouros-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.367653 frouros-0.6.0/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6974 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/batch/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/callbacks/streaming/history.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2611 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3779 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6610 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5905 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11592 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3401 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3190 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11060 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6852 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13602 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26281 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10871 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20156 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6859 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8954 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6535 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3818 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2745 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7954 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3993 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7900 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4445 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4755 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15083 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.375654 frouros-0.6.0/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.379654 frouros-0.6.0/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.379654 frouros-0.6.0/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21475 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/utils/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7563 2023-08-04 15:43:22.000000 frouros-0.6.0/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 15:43:35.371653 frouros-0.6.0/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25160 2023-08-04 15:43:34.000000 frouros-0.6.0/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4822 2023-08-04 15:43:35.000000 frouros-0.6.0/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 15:43:34.000000 frouros-0.6.0/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 15:43:34.000000 frouros-0.6.0/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-08-04 15:43:35.000000 frouros-0.6.0/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-08-04 15:43:35.000000 frouros-0.6.0/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-08-04 15:43:22.000000 frouros-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 15:43:35.379654 frouros-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-08-04 15:43:22.000000 frouros-0.6.0/setup.py
```

### Comparing `frouros-0.5.1/LICENSE` & `frouros-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/PKG-INFO` & `frouros-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,1480 +1,1472 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6672 6f75  : 2.1.Name: frou
-00000020: 726f 730a 5665 7273 696f 6e3a 2030 2e35  ros.Version: 0.5
-00000030: 2e31 0a53 756d 6d61 7279 3a20 416e 206f  .1.Summary: An o
-00000040: 7065 6e2d 736f 7572 6365 2050 7974 686f  pen-source Pytho
-00000050: 6e20 6c69 6272 6172 7920 666f 7220 6472  n library for dr
-00000060: 6966 7420 6465 7465 6374 696f 6e20 696e  ift detection in
-00000070: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
-00000080: 6720 7379 7374 656d 730a 486f 6d65 2d70  g systems.Home-p
-00000090: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-000000a0: 6875 622e 636f 6d2f 4946 4341 2f66 726f  hub.com/IFCA/fro
-000000b0: 7572 6f73 0a41 7574 686f 723a 204a 6169  uros.Author: Jai
-000000c0: 6d65 2043 c3a9 7370 6564 6573 2053 6973  me C..spedes Sis
-000000d0: 6e69 6567 610a 4175 7468 6f72 2d65 6d61  niega.Author-ema
-000000e0: 696c 3a20 6365 7370 6564 6573 4069 6663  il: cespedes@ifc
-000000f0: 612e 756e 6963 616e 2e65 730a 4d61 696e  a.unican.es.Main
-00000100: 7461 696e 6572 3a20 4a61 696d 6520 43c3  tainer: Jaime C.
-00000110: a973 7065 6465 7320 5369 736e 6965 6761  .spedes Sisniega
-00000120: 0a4d 6169 6e74 6169 6e65 722d 656d 6169  .Maintainer-emai
-00000130: 6c3a 2063 6573 7065 6465 7340 6966 6361  l: cespedes@ifca
-00000140: 2e75 6e69 6361 6e2e 6573 0a4c 6963 656e  .unican.es.Licen
-00000150: 7365 3a20 4253 442d 332d 436c 6175 7365  se: BSD-3-Clause
-00000160: 0a50 726f 6a65 6374 2d55 524c 3a20 686f  .Project-URL: ho
-00000170: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
-00000180: 6672 6f75 726f 732e 7265 6164 7468 6564  frouros.readthed
-00000190: 6f63 732e 696f 0a50 726f 6a65 6374 2d55  ocs.io.Project-U
-000001a0: 524c 3a20 7265 706f 7369 746f 7279 2c20  RL: repository, 
-000001b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001c0: 6f6d 2f49 4643 412f 6672 6f75 726f 730a  om/IFCA/frouros.
-000001d0: 5072 6f6a 6563 742d 5552 4c3a 2064 6f63  Project-URL: doc
-000001e0: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
-000001f0: 733a 2f2f 6672 6f75 726f 732e 7265 6164  s://frouros.read
-00000200: 7468 6564 6f63 732e 696f 0a50 726f 6a65  thedocs.io.Proje
-00000210: 6374 2d55 524c 3a20 646f 776e 6c6f 6164  ct-URL: download
-00000220: 2c20 6874 7470 733a 2f2f 7079 7069 2e6f  , https://pypi.o
-00000230: 7267 2f70 726f 6a65 6374 2f66 726f 7572  rg/project/frour
-00000240: 6f73 2f0a 4b65 7977 6f72 6473 3a20 6472  os/.Keywords: dr
-00000250: 6966 742d 6465 7465 6374 696f 6e2c 636f  ift-detection,co
-00000260: 6e63 6570 742d 6472 6966 742c 6461 7461  ncept-drift,data
-00000270: 2d64 7269 6674 2c6d 6163 6869 6e65 2d6c  -drift,machine-l
-00000280: 6561 726e 696e 672c 6461 7461 2d73 6369  earning,data-sci
-00000290: 656e 6365 2c6d 6163 6869 6e65 2d6c 6561  ence,machine-lea
-000002a0: 726e 696e 672d 6f70 6572 6174 696f 6e73  rning-operations
-000002b0: 2c6d 6163 6869 6e65 2d6c 6561 726e 696e  ,machine-learnin
-000002c0: 672d 7379 7374 656d 730a 506c 6174 666f  g-systems.Platfo
-000002d0: 726d 3a20 554e 4b4e 4f57 4e0a 436c 6173  rm: UNKNOWN.Clas
-000002e0: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
-000002f0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-00000300: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-00000310: 626c 650a 436c 6173 7369 6669 6572 3a20  ble.Classifier: 
-00000320: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000330: 6520 3a3a 2044 6576 656c 6f70 6572 730a  e :: Developers.
-00000340: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-00000350: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000360: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
-00000370: 680a 436c 6173 7369 6669 6572 3a20 4c69  h.Classifier: Li
-00000380: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000390: 726f 7665 6420 3a3a 2042 5344 204c 6963  roved :: BSD Lic
-000003a0: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-000003b0: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
-000003c0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-000003d0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-000003e0: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
-000003f0: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
-00000400: 4172 7469 6669 6369 616c 2049 6e74 656c  Artificial Intel
-00000410: 6c69 6765 6e63 650a 436c 6173 7369 6669  ligence.Classifi
-00000420: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
-00000430: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-00000440: 696e 6720 3a3a 204d 6174 6865 6d61 7469  ing :: Mathemati
-00000450: 6373 0a43 6c61 7373 6966 6965 723a 2054  cs.Classifier: T
-00000460: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-00000470: 2044 6576 656c 6f70 6d65 6e74 0a43 6c61   Development.Cla
-00000480: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000490: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-000004a0: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-000004b0: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
-000004c0: 6475 6c65 730a 436c 6173 7369 6669 6572  dules.Classifier
-000004d0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000004e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000004f0: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000500: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000510: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000520: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
-00000530: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000540: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000550: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
-00000560: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000570: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000580: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
-00000590: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000005a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000005b0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-000005c0: 3a3a 204f 6e6c 790a 5265 7175 6972 6573  :: Only.Requires
-000005d0: 2d50 7974 686f 6e3a 203e 3d33 2e38 2c3c  -Python: >=3.8,<
-000005e0: 332e 3132 0a44 6573 6372 6970 7469 6f6e  3.12.Description
-000005f0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-00000600: 6578 742f 6d61 726b 646f 776e 0a50 726f  ext/markdown.Pro
-00000610: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
-00000620: 730a 5072 6f76 6964 6573 2d45 7874 7261  s.Provides-Extra
-00000630: 3a20 6e6f 7465 626f 6f6b 730a 4c69 6365  : notebooks.Lice
-00000640: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-00000650: 450a 0a3c 7020 616c 6967 6e3d 2263 656e  E..<p align="cen
-00000660: 7465 7222 3e0a 2020 3c69 6d67 2068 6569  ter">.  <img hei
-00000670: 6768 743d 2231 3135 7078 2220 7372 633d  ght="115px" src=
-00000680: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00000690: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-000006a0: 6f6d 2f49 4643 412f 6672 6f75 726f 732f  om/IFCA/frouros/
-000006b0: 6d61 696e 2f69 6d61 6765 732f 6c6f 676f  main/images/logo
-000006c0: 2e70 6e67 2220 616c 743d 226c 6f67 6f22  .png" alt="logo"
-000006d0: 3e0a 3c2f 703e 0a0a 2d2d 2d0a 0a3c 7020  >.</p>..---..<p 
-000006e0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-000006f0: 2020 3c21 2d2d 2043 4920 2d2d 3e0a 2020    <!-- CI -->.  
-00000700: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000710: 2f67 6974 6875 622e 636f 6d2f 4946 4341  /github.com/IFCA
-00000720: 2f66 726f 7572 6f73 2f61 6374 696f 6e73  /frouros/actions
-00000730: 2f77 6f72 6b66 6c6f 7773 2f63 692e 796d  /workflows/ci.ym
-00000740: 6c22 3e0a 2020 2020 3c69 6d67 2073 7263  l">.    <img src
-00000750: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000760: 2e63 6f6d 2f49 4643 412f 6672 6f75 726f  .com/IFCA/frouro
-00000770: 732f 6163 7469 6f6e 732f 776f 726b 666c  s/actions/workfl
-00000780: 6f77 732f 6369 2e79 6d6c 2f62 6164 6765  ows/ci.yml/badge
-00000790: 2e73 7667 3f73 7479 6c65 3d66 6c61 742d  .svg?style=flat-
-000007a0: 7371 7561 7265 2220 616c 743d 2263 6922  square" alt="ci"
-000007b0: 2f3e 0a20 203c 2f61 3e0a 2020 3c21 2d2d  />.  </a>.  <!--
-000007c0: 2043 6f64 6520 636f 7665 7261 6765 202d   Code coverage -
-000007d0: 2d3e 0a20 203c 6120 6872 6566 3d22 6874  ->.  <a href="ht
-000007e0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-000007f0: 2f67 682f 4946 4341 2f66 726f 7572 6f73  /gh/IFCA/frouros
-00000800: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
-00000810: 2268 7474 7073 3a2f 2f63 6f64 6563 6f76  "https://codecov
-00000820: 2e69 6f2f 6768 2f49 4643 412f 6672 6f75  .io/gh/IFCA/frou
-00000830: 726f 732f 6272 616e 6368 2f6d 6169 6e2f  ros/branch/main/
-00000840: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
-00000850: 746f 6b65 6e3d 444c 4b51 5357 5954 594d  token=DLKQSWYTYM
-00000860: 2220 616c 743d 2263 6f76 6572 6167 6522  " alt="coverage"
-00000870: 2f3e 0a20 203c 2f61 3e0a 2020 3c21 2d2d  />.  </a>.  <!--
-00000880: 2044 6f63 756d 656e 7461 7469 6f6e 202d   Documentation -
-00000890: 2d3e 0a20 203c 6120 6872 6566 3d22 6874  ->.  <a href="ht
-000008a0: 7470 733a 2f2f 6672 6f75 726f 732e 7265  tps://frouros.re
-000008b0: 6164 7468 6564 6f63 732e 696f 2f22 3e0a  adthedocs.io/">.
-000008c0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000008d0: 7470 733a 2f2f 7265 6164 7468 6564 6f63  tps://readthedoc
-000008e0: 732e 6f72 672f 7072 6f6a 6563 7473 2f66  s.org/projects/f
-000008f0: 726f 7572 6f73 2f62 6164 6765 2f3f 7665  rouros/badge/?ve
-00000900: 7273 696f 6e3d 6c61 7465 7374 2220 616c  rsion=latest" al
-00000910: 743d 2264 6f63 756d 656e 7461 7469 6f6e  t="documentation
-00000920: 222f 3e0a 2020 3c2f 613e 0a20 203c 212d  "/>.  </a>.  <!-
-00000930: 2d20 446f 776e 6c6f 6164 7320 2d2d 3e0a  - Downloads -->.
-00000940: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000950: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
-00000960: 6a65 6374 2f66 726f 7572 6f73 223e 0a20  ject/frouros">. 
-00000970: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000980: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
-00000990: 2e74 6563 682f 6261 6467 652f 6672 6f75  .tech/badge/frou
-000009a0: 726f 7322 2061 6c74 3d22 646f 776e 6c6f  ros" alt="downlo
-000009b0: 6164 7322 2f3e 0a20 203c 2f61 3e0a 2020  ads"/>.  </a>.  
-000009c0: 3c21 2d2d 2050 7950 4920 2d2d 3e0a 2020  <!-- PyPI -->.  
-000009d0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000009e0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-000009f0: 742f 6672 6f75 726f 7322 3e0a 2020 2020  t/frouros">.    
-00000a00: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000a10: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000a20: 2f70 7970 692f 762f 6672 6f75 726f 732e  /pypi/v/frouros.
-00000a30: 7376 673f 6c61 6265 6c3d 7265 6c65 6173  svg?label=releas
-00000a40: 6526 636f 6c6f 723d 626c 7565 2220 616c  e&color=blue" al
-00000a50: 743d 2270 7970 6922 3e0a 2020 3c2f 613e  t="pypi">.  </a>
-00000a60: 0a20 203c 212d 2d20 5079 7468 6f6e 202d  .  <!-- Python -
-00000a70: 2d3e 0a20 203c 6120 6872 6566 3d22 6874  ->.  <a href="ht
-00000a80: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000a90: 726f 6a65 6374 2f66 726f 7572 6f73 223e  roject/frouros">
-00000aa0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000ab0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000ac0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000ad0: 7369 6f6e 732f 6672 6f75 726f 7322 2061  sions/frouros" a
-00000ae0: 6c74 3d22 7079 7468 6f6e 223e 0a20 203c  lt="python">.  <
-00000af0: 2f61 3e0a 2020 3c21 2d2d 204c 6963 656e  /a>.  <!-- Licen
-00000b00: 7365 202d 2d3e 0a20 203c 6120 6872 6566  se -->.  <a href
-00000b10: 3d22 6874 7470 733a 2f2f 6f70 656e 736f  ="https://openso
-00000b20: 7572 6365 2e6f 7267 2f6c 6963 656e 7365  urce.org/license
-00000b30: 732f 4253 442d 332d 436c 6175 7365 223e  s/BSD-3-Clause">
-00000b40: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000b50: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000b60: 6473 2e69 6f2f 6261 6467 652f 6c69 6365  ds.io/badge/lice
-00000b70: 6e73 652d 4253 4425 3230 332d 2d43 6c61  nse-BSD%203--Cla
-00000b80: 7573 652d 626c 7565 2e73 7667 2220 616c  use-blue.svg" al
-00000b90: 743d 2262 7364 5f33 5f6c 6963 656e 7365  t="bsd_3_license
-00000ba0: 223e 0a20 203c 2f61 3e0a 2020 3c21 2d2d  ">.  </a>.  <!--
-00000bb0: 2061 7258 6976 202d 2d3e 0a20 203c 6120   arXiv -->.  <a 
-00000bc0: 6872 6566 3d22 6874 7470 733a 2f2f 6172  href="https://ar
-00000bd0: 7869 762e 6f72 672f 6162 732f 3232 3038  xiv.org/abs/2208
-00000be0: 2e30 3638 3638 223e 0a20 2020 203c 696d  .06868">.    <im
-00000bf0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000c00: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000c10: 6467 652f 6172 5869 762d 3232 3038 2e30  dge/arXiv-2208.0
-00000c20: 3638 3638 2d62 6c75 652e 7376 6722 2061  6868-blue.svg" a
-00000c30: 6c74 3d22 6172 7869 7622 3e0a 2020 3c2f  lt="arxiv">.  </
-00000c40: 613e 0a3c 2f70 3e0a 0a46 726f 7572 6f73  a>.</p>..Frouros
-00000c50: 2069 7320 6120 5079 7468 6f6e 206c 6962   is a Python lib
-00000c60: 7261 7279 2066 6f72 2064 7269 6674 2064  rary for drift d
-00000c70: 6574 6563 7469 6f6e 2069 6e20 6d61 6368  etection in mach
-00000c80: 696e 6520 6c65 6172 6e69 6e67 2073 7973  ine learning sys
-00000c90: 7465 6d73 2074 6861 7420 7072 6f76 6964  tems that provid
-00000ca0: 6573 2061 2063 6f6d 6269 6e61 7469 6f6e  es a combination
-00000cb0: 206f 6620 636c 6173 7369 6361 6c20 616e   of classical an
-00000cc0: 6420 6d6f 7265 2072 6563 656e 7420 616c  d more recent al
-00000cd0: 676f 7269 7468 6d73 2066 6f72 2062 6f74  gorithms for bot
-00000ce0: 6820 636f 6e63 6570 7420 616e 6420 6461  h concept and da
-00000cf0: 7461 2064 7269 6674 2064 6574 6563 7469  ta drift detecti
-00000d00: 6f6e 2e0a 0a3c 7020 616c 6967 6e3d 2263  on...<p align="c
-00000d10: 656e 7465 7222 3e0a 2020 2020 3c69 3e0a  enter">.    <i>.
-00000d20: 2020 2020 2020 2020 2245 7665 7279 7468          "Everyth
-00000d30: 696e 6720 6368 616e 6765 7320 616e 6420  ing changes and 
-00000d40: 6e6f 7468 696e 6720 7374 616e 6473 2073  nothing stands s
-00000d50: 7469 6c6c 220a 2020 2020 3c2f 693e 0a3c  till".    </i>.<
-00000d60: 2f70 3e0a 3c70 2061 6c69 676e 3d22 6365  /p>.<p align="ce
-00000d70: 6e74 6572 223e 0a20 2020 203c 693e 0a20  nter">.    <i>. 
-00000d80: 2020 2020 2020 2022 596f 7520 636f 756c         "You coul
-00000d90: 6420 6e6f 7420 7374 6570 2074 7769 6365  d not step twice
-00000da0: 2069 6e74 6f20 7468 6520 7361 6d65 2072   into the same r
-00000db0: 6976 6572 220a 2020 2020 3c2f 693e 0a3c  iver".    </i>.<
-00000dc0: 2f70 3e0a 3c64 6976 2061 6c69 676e 3d22  /p>.<div align="
-00000dd0: 6365 6e74 6572 2220 7374 796c 653d 2277  center" style="w
-00000de0: 6964 7468 3a20 3730 253b 223e 0a20 2020  idth: 70%;">.   
-00000df0: 203c 7020 616c 6967 6e3d 2272 6967 6874   <p align="right
-00000e00: 223e 0a20 2020 2020 2020 203c 693e 0a20  ">.        <i>. 
-00000e10: 2020 2020 2020 2020 2020 2048 6572 6163             Herac
-00000e20: 6c69 7475 7320 6f66 2045 7068 6573 7573  litus of Ephesus
-00000e30: 2028 3533 352d 3437 3520 4243 452e 290a   (535-475 BCE.).
-00000e40: 2020 2020 2020 2020 3c2f 693e 0a20 2020          </i>.   
-00000e50: 203c 2f70 3e0a 3c2f 6469 763e 0a0a 2d2d   </p>.</div>..--
-00000e60: 2d2d 0a0a 2323 20e2 9aa1 efb8 8f20 5175  --..## ...... Qu
-00000e70: 6963 6b73 7461 7274 0a0a 2323 2320 436f  ickstart..### Co
-00000e80: 6e63 6570 7420 6472 6966 740a 0a41 7320  ncept drift..As 
-00000e90: 6120 7175 6963 6b20 6578 616d 706c 652c  a quick example,
-00000ea0: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
-00000eb0: 7769 6e65 2064 6174 6173 6574 2074 6f20  wine dataset to 
-00000ec0: 7768 6963 6820 636f 6e63 6570 7420 6472  which concept dr
-00000ed0: 6966 7420 6974 2069 7320 696e 6475 6365  ift it is induce
-00000ee0: 6420 696e 206f 7264 6572 2074 6f20 7368  d in order to sh
-00000ef0: 6f77 2074 6865 2075 7365 206f 6620 6120  ow the use of a 
-00000f00: 636f 6e63 6570 7420 6472 6966 7420 6465  concept drift de
-00000f10: 7465 6374 6f72 206c 696b 6520 4444 4d20  tector like DDM 
-00000f20: 2844 7269 6674 2044 6574 6563 7469 6f6e  (Drift Detection
-00000f30: 204d 6574 686f 6429 2e0a 0a60 6060 7079   Method)...```py
-00000f40: 7468 6f6e 0a69 6d70 6f72 7420 6e75 6d70  thon.import nump
-00000f50: 7920 6173 206e 700a 6672 6f6d 2073 6b6c  y as np.from skl
-00000f60: 6561 726e 2e64 6174 6173 6574 7320 696d  earn.datasets im
-00000f70: 706f 7274 206c 6f61 645f 7769 6e65 0a66  port load_wine.f
-00000f80: 726f 6d20 736b 6c65 6172 6e2e 6c69 6e65  rom sklearn.line
-00000f90: 6172 5f6d 6f64 656c 2069 6d70 6f72 7420  ar_model import 
-00000fa0: 4c6f 6769 7374 6963 5265 6772 6573 7369  LogisticRegressi
-00000fb0: 6f6e 0a66 726f 6d20 736b 6c65 6172 6e2e  on.from sklearn.
-00000fc0: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e20  model_selection 
-00000fd0: 696d 706f 7274 2074 7261 696e 5f74 6573  import train_tes
-00000fe0: 745f 7370 6c69 740a 6672 6f6d 2073 6b6c  t_split.from skl
-00000ff0: 6561 726e 2e70 6970 656c 696e 6520 696d  earn.pipeline im
-00001000: 706f 7274 2050 6970 656c 696e 650a 6672  port Pipeline.fr
-00001010: 6f6d 2073 6b6c 6561 726e 2e70 7265 7072  om sklearn.prepr
-00001020: 6f63 6573 7369 6e67 2069 6d70 6f72 7420  ocessing import 
-00001030: 5374 616e 6461 7264 5363 616c 6572 0a0a  StandardScaler..
-00001040: 6672 6f6d 2066 726f 7572 6f73 2e64 6574  from frouros.det
-00001050: 6563 746f 7273 2e63 6f6e 6365 7074 5f64  ectors.concept_d
-00001060: 7269 6674 2069 6d70 6f72 7420 4444 4d2c  rift import DDM,
-00001070: 2044 444d 436f 6e66 6967 0a0a 6e70 2e72   DDMConfig..np.r
-00001080: 616e 646f 6d2e 7365 6564 2873 6565 643d  andom.seed(seed=
-00001090: 3331 290a 0a23 204c 6f61 6420 7769 6e65  31)..# Load wine
-000010a0: 2064 6174 6173 6574 0a58 2c20 7920 3d20   dataset.X, y = 
-000010b0: 6c6f 6164 5f77 696e 6528 7265 7475 726e  load_wine(return
-000010c0: 5f58 5f79 3d54 7275 6529 0a0a 2320 5370  _X_y=True)..# Sp
-000010d0: 6c69 7420 7472 6169 6e20 2837 3025 2920  lit train (70%) 
-000010e0: 616e 6420 7465 7374 2028 3330 2529 0a28  and test (30%).(
-000010f0: 0a20 2020 2058 5f74 7261 696e 2c0a 2020  .    X_train,.  
-00001100: 2020 585f 7465 7374 2c0a 2020 2020 795f    X_test,.    y_
-00001110: 7472 6169 6e2c 0a20 2020 2079 5f74 6573  train,.    y_tes
-00001120: 742c 0a29 203d 2074 7261 696e 5f74 6573  t,.) = train_tes
-00001130: 745f 7370 6c69 7428 582c 2079 2c20 7472  t_split(X, y, tr
-00001140: 6169 6e5f 7369 7a65 3d30 2e37 2c20 7261  ain_size=0.7, ra
-00001150: 6e64 6f6d 5f73 7461 7465 3d33 3129 0a0a  ndom_state=31)..
-00001160: 2320 494d 504f 5254 414e 543a 2049 6e64  # IMPORTANT: Ind
-00001170: 7563 652f 7369 6d75 6c61 7465 2063 6f6e  uce/simulate con
-00001180: 6365 7074 2064 7269 6674 2069 6e20 7468  cept drift in th
-00001190: 6520 6c61 7374 2070 6172 7420 2832 3025  e last part (20%
-000011a0: 290a 2320 6f66 2079 5f74 6573 7420 6279  ).# of y_test by
-000011b0: 206d 6f64 6966 7969 6e67 2073 6f6d 6520   modifying some 
-000011c0: 6c61 6265 6c73 2028 3530 2520 6170 7072  labels (50% appr
-000011d0: 6f78 292e 2054 6865 7265 666f 7265 2c20  ox). Therefore, 
-000011e0: 6368 616e 6769 6e67 2050 2879 7c58 2929  changing P(y|X))
-000011f0: 0a64 7269 6674 5f73 697a 6520 3d20 696e  .drift_size = in
-00001200: 7428 795f 7465 7374 2e73 6861 7065 5b30  t(y_test.shape[0
-00001210: 5d20 2a20 302e 3229 0a79 5f74 6573 745f  ] * 0.2).y_test_
-00001220: 6472 6966 7420 3d20 795f 7465 7374 5b2d  drift = y_test[-
-00001230: 6472 6966 745f 7369 7a65 3a5d 0a6d 6f64  drift_size:].mod
-00001240: 6966 795f 6964 7820 3d20 6e70 2e72 616e  ify_idx = np.ran
-00001250: 646f 6d2e 7261 6e64 282a 795f 7465 7374  dom.rand(*y_test
-00001260: 5f64 7269 6674 2e73 6861 7065 2920 3c3d  _drift.shape) <=
-00001270: 2030 2e35 0a79 5f74 6573 745f 6472 6966   0.5.y_test_drif
-00001280: 745b 6d6f 6469 6679 5f69 6478 5d20 3d20  t[modify_idx] = 
-00001290: 2879 5f74 6573 745f 6472 6966 745b 6d6f  (y_test_drift[mo
-000012a0: 6469 6679 5f69 6478 5d20 2b20 3129 2025  dify_idx] + 1) %
-000012b0: 206c 656e 286e 702e 756e 6971 7565 2879   len(np.unique(y
-000012c0: 5f74 6573 7429 290a 795f 7465 7374 5b2d  _test)).y_test[-
-000012d0: 6472 6966 745f 7369 7a65 3a5d 203d 2079  drift_size:] = y
-000012e0: 5f74 6573 745f 6472 6966 740a 0a23 2044  _test_drift..# D
-000012f0: 6566 696e 6520 616e 6420 6669 7420 6d6f  efine and fit mo
-00001300: 6465 6c0a 7069 7065 6c69 6e65 203d 2050  del.pipeline = P
-00001310: 6970 656c 696e 6528 0a20 2020 205b 0a20  ipeline(.    [. 
-00001320: 2020 2020 2020 2028 2273 6361 6c65 7222         ("scaler"
-00001330: 2c20 5374 616e 6461 7264 5363 616c 6572  , StandardScaler
-00001340: 2829 292c 0a20 2020 2020 2020 2028 226d  ()),.        ("m
-00001350: 6f64 656c 222c 204c 6f67 6973 7469 6352  odel", LogisticR
-00001360: 6567 7265 7373 696f 6e28 2929 2c0a 2020  egression()),.  
-00001370: 2020 5d0a 290a 7069 7065 6c69 6e65 2e66    ].).pipeline.f
-00001380: 6974 2858 3d58 5f74 7261 696e 2c20 793d  it(X=X_train, y=
-00001390: 795f 7472 6169 6e29 0a0a 2320 4465 7465  y_train)..# Dete
-000013a0: 6374 6f72 2063 6f6e 6669 6775 7261 7469  ctor configurati
-000013b0: 6f6e 2061 6e64 2069 6e73 7461 6e74 6961  on and instantia
-000013c0: 7469 6f6e 0a63 6f6e 6669 6720 3d20 4444  tion.config = DD
-000013d0: 4d43 6f6e 6669 6728 7761 726e 696e 675f  MConfig(warning_
-000013e0: 6c65 7665 6c3d 322e 302c 0a20 2020 2020  level=2.0,.     
-000013f0: 2020 2020 2020 2020 2020 2020 2020 6472                dr
-00001400: 6966 745f 6c65 7665 6c3d 332e 302c 0a20  ift_level=3.0,. 
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 2020 6d69 6e5f 6e75 6d5f 696e 7374 616e    min_num_instan
-00001430: 6365 733d 3330 2c29 0a64 6574 6563 746f  ces=30,).detecto
-00001440: 7220 3d20 4444 4d28 636f 6e66 6967 3d63  r = DDM(config=c
-00001450: 6f6e 6669 6729 0a0a 2320 5369 6d75 6c61  onfig)..# Simula
-00001460: 7465 2064 6174 6120 7374 7265 616d 2028  te data stream (
-00001470: 6173 7375 6d69 6e67 2074 6573 7420 6c61  assuming test la
-00001480: 6265 6c20 6176 6169 6c61 626c 6520 6166  bel available af
-00001490: 7465 7220 7072 6564 6963 7469 6f6e 290a  ter prediction).
-000014a0: 666f 7220 692c 2028 582c 2079 2920 696e  for i, (X, y) in
-000014b0: 2065 6e75 6d65 7261 7465 287a 6970 2858   enumerate(zip(X
-000014c0: 5f74 6573 742c 2079 5f74 6573 7429 293a  _test, y_test)):
-000014d0: 0a20 2020 2079 5f70 7265 6420 3d20 7069  .    y_pred = pi
-000014e0: 7065 6c69 6e65 2e70 7265 6469 6374 2858  peline.predict(X
-000014f0: 2e72 6573 6861 7065 2831 2c20 2d31 2929  .reshape(1, -1))
-00001500: 0a20 2020 2065 7272 6f72 203d 2031 202d  .    error = 1 -
-00001510: 2069 6e74 2879 5f70 7265 6420 3d3d 2079   int(y_pred == y
-00001520: 290a 2020 2020 6465 7465 6374 6f72 2e75  ).    detector.u
-00001530: 7064 6174 6528 7661 6c75 653d 6572 726f  pdate(value=erro
-00001540: 7229 0a20 2020 2073 7461 7475 7320 3d20  r).    status = 
-00001550: 6465 7465 6374 6f72 2e73 7461 7475 730a  detector.status.
-00001560: 2020 2020 6966 2073 7461 7475 735b 2264      if status["d
-00001570: 7269 6674 225d 3a0a 2020 2020 2020 2020  rift"]:.        
-00001580: 7072 696e 7428 6622 4472 6966 7420 6465  print(f"Drift de
-00001590: 7465 6374 6564 2061 7420 696e 6465 7820  tected at index 
-000015a0: 7b69 7d22 290a 2020 2020 2020 2020 6272  {i}").        br
-000015b0: 6561 6b0a 0a3e 3e20 4472 6966 7420 6465  eak..>> Drift de
-000015c0: 7465 6374 6564 2061 7420 696e 6465 7820  tected at index 
-000015d0: 3434 0a60 6060 0a0a 4d6f 7265 2063 6f6e  44.```..More con
-000015e0: 6365 7074 2064 7269 6674 2065 7861 6d70  cept drift examp
-000015f0: 6c65 7320 6361 6e20 6265 2066 6f75 6e64  les can be found
-00001600: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-00001610: 6672 6f75 726f 732e 7265 6164 7468 6564  frouros.readthed
-00001620: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00001630: 2f65 7861 6d70 6c65 732e 6874 6d6c 2364  /examples.html#d
-00001640: 6174 612d 6472 6966 7429 2e0a 0a23 2323  ata-drift)...###
-00001650: 2044 6174 6120 6472 6966 740a 0a41 7320   Data drift..As 
-00001660: 6120 7175 6963 6b20 6578 616d 706c 652c  a quick example,
-00001670: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
-00001680: 6972 6973 2064 6174 6173 6574 2074 6f20  iris dataset to 
-00001690: 7768 6963 6820 6461 7461 2064 7269 6674  which data drift
-000016a0: 2069 6e20 6f72 6465 7220 746f 2073 686f   in order to sho
-000016b0: 7720 7468 6520 7573 6520 6f66 2061 2064  w the use of a d
-000016c0: 6174 6120 6472 6966 7420 6465 7465 6374  ata drift detect
-000016d0: 6f72 206c 696b 6520 4b6f 6c6d 6f67 6f72  or like Kolmogor
-000016e0: 6f76 2d53 6d69 726e 6f76 2074 6573 742e  ov-Smirnov test.
-000016f0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-00001700: 7274 206e 756d 7079 2061 7320 6e70 0a66  rt numpy as np.f
-00001710: 726f 6d20 736b 6c65 6172 6e2e 6461 7461  rom sklearn.data
-00001720: 7365 7473 2069 6d70 6f72 7420 6c6f 6164  sets import load
-00001730: 5f69 7269 730a 6672 6f6d 2073 6b6c 6561  _iris.from sklea
-00001740: 726e 2e6d 6f64 656c 5f73 656c 6563 7469  rn.model_selecti
-00001750: 6f6e 2069 6d70 6f72 7420 7472 6169 6e5f  on import train_
-00001760: 7465 7374 5f73 706c 6974 0a66 726f 6d20  test_split.from 
-00001770: 736b 6c65 6172 6e2e 7472 6565 2069 6d70  sklearn.tree imp
-00001780: 6f72 7420 4465 6369 7369 6f6e 5472 6565  ort DecisionTree
-00001790: 436c 6173 7369 6669 6572 0a0a 6672 6f6d  Classifier..from
-000017a0: 2066 726f 7572 6f73 2e64 6574 6563 746f   frouros.detecto
-000017b0: 7273 2e64 6174 615f 6472 6966 7420 696d  rs.data_drift im
-000017c0: 706f 7274 204b 5354 6573 740a 0a6e 702e  port KSTest..np.
-000017d0: 7261 6e64 6f6d 2e73 6565 6428 7365 6564  random.seed(seed
-000017e0: 3d33 3129 0a0a 2320 4c6f 6164 2069 7269  =31)..# Load iri
-000017f0: 7320 6461 7461 7365 740a 582c 2079 203d  s dataset.X, y =
-00001800: 206c 6f61 645f 6972 6973 2872 6574 7572   load_iris(retur
-00001810: 6e5f 585f 793d 5472 7565 290a 0a23 2053  n_X_y=True)..# S
-00001820: 706c 6974 2074 7261 696e 2028 3730 2529  plit train (70%)
-00001830: 2061 6e64 2074 6573 7420 2833 3025 290a   and test (30%).
-00001840: 280a 2020 2020 585f 7472 6169 6e2c 0a20  (.    X_train,. 
-00001850: 2020 2058 5f74 6573 742c 0a20 2020 2079     X_test,.    y
-00001860: 5f74 7261 696e 2c0a 2020 2020 795f 7465  _train,.    y_te
-00001870: 7374 2c0a 2920 3d20 7472 6169 6e5f 7465  st,.) = train_te
-00001880: 7374 5f73 706c 6974 2858 2c20 792c 2074  st_split(X, y, t
-00001890: 7261 696e 5f73 697a 653d 302e 372c 2072  rain_size=0.7, r
-000018a0: 616e 646f 6d5f 7374 6174 653d 3331 290a  andom_state=31).
-000018b0: 0a23 2053 6574 2074 6865 2066 6561 7475  .# Set the featu
-000018c0: 7265 2069 6e64 6578 2074 6f20 7768 6963  re index to whic
-000018d0: 6820 6465 7465 6374 6f72 2069 7320 6170  h detector is ap
-000018e0: 706c 6965 640a 6469 6d5f 6964 7820 3d20  plied.dim_idx = 
-000018f0: 300a 0a23 2049 4d50 4f52 5441 4e54 3a20  0..# IMPORTANT: 
-00001900: 496e 6475 6365 2f73 696d 756c 6174 6520  Induce/simulate 
-00001910: 6461 7461 2064 7269 6674 2069 6e20 7468  data drift in th
-00001920: 6520 7365 6c65 6374 6564 2066 6561 7475  e selected featu
-00001930: 7265 206f 6620 795f 7465 7374 2062 790a  re of y_test by.
-00001940: 2320 6170 706c 7969 6e67 2073 6f6d 6520  # applying some 
-00001950: 6761 7573 7369 616e 206e 6f69 7365 2e20  gaussian noise. 
-00001960: 5468 6572 6566 6f72 652c 2063 6861 6e67  Therefore, chang
-00001970: 696e 6720 5028 5829 290a 585f 7465 7374  ing P(X)).X_test
-00001980: 5b3a 2c20 6469 6d5f 6964 785d 202b 3d20  [:, dim_idx] += 
-00001990: 6e70 2e72 616e 646f 6d2e 6e6f 726d 616c  np.random.normal
-000019a0: 280a 2020 2020 6c6f 633d 302e 302c 0a20  (.    loc=0.0,. 
-000019b0: 2020 2073 6361 6c65 3d33 2e30 2c0a 2020     scale=3.0,.  
-000019c0: 2020 7369 7a65 3d58 5f74 6573 742e 7368    size=X_test.sh
-000019d0: 6170 655b 305d 2c0a 290a 0a23 2044 6566  ape[0],.)..# Def
-000019e0: 696e 6520 616e 6420 6669 7420 6d6f 6465  ine and fit mode
-000019f0: 6c0a 6d6f 6465 6c20 3d20 4465 6369 7369  l.model = Decisi
-00001a00: 6f6e 5472 6565 436c 6173 7369 6669 6572  onTreeClassifier
-00001a10: 2872 616e 646f 6d5f 7374 6174 653d 3331  (random_state=31
-00001a20: 290a 6d6f 6465 6c2e 6669 7428 583d 585f  ).model.fit(X=X_
-00001a30: 7472 6169 6e2c 2079 3d79 5f74 7261 696e  train, y=y_train
-00001a40: 290a 0a23 2053 6574 2073 6967 6e69 6669  )..# Set signifi
-00001a50: 6361 6e63 6520 6c65 7665 6c20 666f 7220  cance level for 
-00001a60: 6879 706f 7468 6573 6973 2074 6573 7469  hypothesis testi
-00001a70: 6e67 0a61 6c70 6861 203d 2030 2e30 3031  ng.alpha = 0.001
-00001a80: 0a23 2044 6566 696e 6520 616e 6420 6669  .# Define and fi
-00001a90: 7420 6465 7465 6374 6f72 0a64 6574 6563  t detector.detec
-00001aa0: 746f 7220 3d20 4b53 5465 7374 2829 0a64  tor = KSTest().d
-00001ab0: 6574 6563 746f 722e 6669 7428 583d 585f  etector.fit(X=X_
-00001ac0: 7472 6169 6e5b 3a2c 2064 696d 5f69 6478  train[:, dim_idx
-00001ad0: 5d29 0a0a 2320 4170 706c 7920 6465 7465  ])..# Apply dete
-00001ae0: 6374 6f72 2074 6f20 7468 6520 7365 6c65  ctor to the sele
-00001af0: 6374 6564 2066 6561 7475 7265 206f 6620  cted feature of 
-00001b00: 585f 7465 7374 0a72 6573 756c 7420 3d20  X_test.result = 
-00001b10: 6465 7465 6374 6f72 2e63 6f6d 7061 7265  detector.compare
-00001b20: 2858 3d58 5f74 6573 745b 3a2c 2064 696d  (X=X_test[:, dim
-00001b30: 5f69 6478 5d29 0a0a 2320 4368 6563 6b20  _idx])..# Check 
-00001b40: 6966 2064 7269 6674 2069 7320 7461 6b69  if drift is taki
-00001b50: 6e67 2070 6c61 6365 0a72 6573 756c 745b  ng place.result[
-00001b60: 305d 2e70 5f76 616c 7565 203c 2061 6c70  0].p_value < alp
-00001b70: 6861 0a3e 3e20 5472 7565 2023 2044 6174  ha.>> True # Dat
-00001b80: 6120 6472 6966 7420 6465 7465 6374 6564  a drift detected
-00001b90: 2e0a 2320 5468 6572 6566 6f72 652c 2077  ..# Therefore, w
-00001ba0: 6520 6361 6e20 7265 6a65 6374 2048 3020  e can reject H0 
-00001bb0: 2862 6f74 6820 7361 6d70 6c65 7320 636f  (both samples co
-00001bc0: 6d65 2066 726f 6d20 7468 6520 7361 6d65  me from the same
-00001bd0: 2064 6973 7472 6962 7574 696f 6e29 2e0a   distribution)..
-00001be0: 6060 600a 0a4d 6f72 6520 6461 7461 2064  ```..More data d
-00001bf0: 7269 6674 2065 7861 6d70 6c65 7320 6361  rift examples ca
-00001c00: 6e20 6265 2066 6f75 6e64 205b 6865 7265  n be found [here
-00001c10: 5d28 6874 7470 733a 2f2f 6672 6f75 726f  ](https://frouro
-00001c20: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
-00001c30: 2f65 6e2f 6c61 7465 7374 2f65 7861 6d70  /en/latest/examp
-00001c40: 6c65 732e 6874 6d6c 2364 6174 612d 6472  les.html#data-dr
-00001c50: 6966 7429 2e0a 0a23 2320 f09f 9ba0 2049  ift)...## .... I
-00001c60: 6e73 7461 6c6c 6174 696f 6e0a 0a46 726f  nstallation..Fro
-00001c70: 7572 6f73 2063 616e 2062 6520 696e 7374  uros can be inst
-00001c80: 616c 6c65 6420 7669 6120 7069 703a 0a0a  alled via pip:..
-00001c90: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
-00001ca0: 616c 6c20 6672 6f75 726f 730a 6060 600a  all frouros.```.
-00001cb0: 0a23 2320 f09f 95b5 f09f 8fbb e280 8de2  .## ............
-00001cc0: 9982 efb8 8fef b88f 2044 7269 6674 2064  ........ Drift d
-00001cd0: 6574 6563 7469 6f6e 206d 6574 686f 6473  etection methods
-00001ce0: 0a0a 5468 6520 6375 7272 656e 746c 7920  ..The currently 
-00001cf0: 696d 706c 656d 656e 7465 6420 6465 7465  implemented dete
-00001d00: 6374 6f72 7320 6172 6520 6c69 7374 6564  ctors are listed
-00001d10: 2069 6e20 7468 6520 666f 6c6c 6f77 696e   in the followin
-00001d20: 6720 7461 626c 652e 0a0a 3c74 6162 6c65  g table...<table
-00001d30: 2073 7479 6c65 3d22 7769 6474 683a 2031   style="width: 1
-00001d40: 3030 253b 2074 6578 742d 616c 6967 6e3a  00%; text-align:
-00001d50: 2063 656e 7465 723b 2062 6f72 6465 722d   center; border-
-00001d60: 636f 6c6c 6170 7365 3a20 636f 6c6c 6170  collapse: collap
-00001d70: 7365 3b20 626f 7264 6572 3a20 3170 7820  se; border: 1px 
-00001d80: 736f 6c69 6420 6772 6579 3b22 3e0a 2020  solid grey;">.  
-00001d90: 3c74 6865 6164 3e0a 2020 2020 3c74 723e  <thead>.    <tr>
-00001da0: 0a20 2020 203c 7468 2073 7479 6c65 3d22  .    <th style="
-00001db0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00001dc0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00001dd0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00001de0: 696e 673a 2034 7078 3b22 3e44 7269 6674  ing: 4px;">Drift
-00001df0: 2064 6574 6563 746f 723c 2f74 683e 0a20   detector</th>. 
-00001e00: 2020 203c 7468 2073 7479 6c65 3d22 7465     <th style="te
-00001e10: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00001e20: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00001e30: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00001e40: 673a 2034 7078 3b22 3e54 7970 653c 2f74  g: 4px;">Type</t
-00001e50: 683e 0a20 2020 203c 7468 2073 7479 6c65  h>.    <th style
-00001e60: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00001e70: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00001e80: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00001e90: 6464 696e 673a 2034 7078 3b22 3e46 616d  dding: 4px;">Fam
-00001ea0: 696c 793c 2f74 683e 0a20 2020 203c 7468  ily</th>.    <th
-00001eb0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00001ec0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00001ed0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00001ee0: 6579 3b20 7061 6464 696e 673a 2034 7078  ey; padding: 4px
-00001ef0: 3b22 3e55 6e69 7661 7269 6174 6520 2855  ;">Univariate (U
-00001f00: 2920 2f20 4d75 6c74 6976 6172 6961 7465  ) / Multivariate
-00001f10: 2028 4d29 3c2f 7468 3e0a 2020 2020 3c74   (M)</th>.    <t
-00001f20: 6820 7374 796c 653d 2274 6578 742d 616c  h style="text-al
-00001f30: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00001f40: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00001f50: 7265 793b 2070 6164 6469 6e67 3a20 3470  rey; padding: 4p
-00001f60: 783b 223e 4e75 6d65 7269 6361 6c20 284e  x;">Numerical (N
-00001f70: 2920 2f20 4361 7465 676f 7269 6361 6c20  ) / Categorical 
-00001f80: 2843 293c 2f74 683e 0a20 2020 203c 7468  (C)</th>.    <th
-00001f90: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00001fa0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00001fb0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00001fc0: 6579 3b20 7061 6464 696e 673a 2034 7078  ey; padding: 4px
-00001fd0: 3b22 3e4d 6574 686f 643c 2f74 683e 0a20  ;">Method</th>. 
-00001fe0: 2020 203c 7468 2073 7479 6c65 3d22 7465     <th style="te
-00001ff0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002000: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002010: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002020: 673a 2034 7078 3b22 3e52 6566 6572 656e  g: 4px;">Referen
-00002030: 6365 3c2f 7468 3e0a 2020 2020 3c2f 7472  ce</th>.    </tr
-00002040: 3e0a 2020 3c2f 7468 6561 643e 0a20 203c  >.  </thead>.  <
-00002050: 7462 6f64 793e 0a20 203c 7472 3e0a 2020  tbody>.  <tr>.  
-00002060: 2020 3c74 6420 726f 7773 7061 6e3d 2231    <td rowspan="1
-00002070: 3322 2073 7479 6c65 3d22 7465 7874 2d61  3" style="text-a
-00002080: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002090: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-000020a0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-000020b0: 7078 3b22 3e43 6f6e 6365 7074 2064 7269  px;">Concept dri
-000020c0: 6674 3c2f 7464 3e0a 2020 2020 3c74 6420  ft</td>.    <td 
-000020d0: 726f 7773 7061 6e3d 2231 3322 2073 7479  rowspan="13" sty
-000020e0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-000020f0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00002100: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00002110: 7061 6464 696e 673a 2038 7078 3b22 3e53  padding: 8px;">S
-00002120: 7472 6561 6d69 6e67 3c2f 7464 3e0a 2020  treaming</td>.  
-00002130: 2020 3c74 6420 726f 7773 7061 6e3d 2234    <td rowspan="4
-00002140: 2220 7374 796c 653d 2274 6578 742d 616c  " style="text-al
-00002150: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00002160: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00002170: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00002180: 783b 223e 4368 616e 6765 2064 6574 6563  x;">Change detec
-00002190: 7469 6f6e 3c2f 7464 3e0a 2020 2020 3c74  tion</td>.    <t
-000021a0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000021b0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-000021c0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-000021d0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-000021e0: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
-000021f0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00002200: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002210: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00002220: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00002230: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
-00002240: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00002250: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00002260: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002270: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002280: 3870 783b 223e 424f 4344 3c2f 7464 3e0a  8px;">BOCD</td>.
-00002290: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-000022a0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-000022b0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-000022c0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-000022d0: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
-000022e0: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
-000022f0: 7267 2f31 302e 3438 3535 302f 6172 5869  rg/10.48550/arXi
-00002300: 762e 3037 3130 2e33 3734 3222 3e41 6461  v.0710.3742">Ada
-00002310: 6d73 2061 6e64 204d 6163 4b61 7920 2832  ms and MacKay (2
-00002320: 3030 3729 3c2f 613e 3c2f 7464 3e0a 2020  007)</a></td>.  
-00002330: 3c2f 7472 3e0a 2020 3c74 723e 0a20 2020  </tr>.  <tr>.   
-00002340: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002350: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00002360: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00002370: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00002380: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
-00002390: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-000023a0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-000023b0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000023c0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000023d0: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
-000023e0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000023f0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002400: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002410: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002420: 673a 2038 7078 3b22 3e43 5553 554d 3c2f  g: 8px;">CUSUM</
-00002430: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00002440: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00002450: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00002460: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00002470: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
-00002480: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-00002490: 6f69 2e6f 7267 2f31 302e 3233 3037 2f32  oi.org/10.2307/2
-000024a0: 3333 3330 3039 223e 5061 6765 2028 3139  333009">Page (19
-000024b0: 3534 293c 2f61 3e3c 2f74 643e 0a20 203c  54)</a></td>.  <
-000024c0: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
-000024d0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000024e0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000024f0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002500: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002510: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
-00002520: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002530: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00002540: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00002550: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00002560: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
-00002570: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00002580: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00002590: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000025a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000025b0: 3a20 3870 783b 223e 4765 6f6d 6574 7269  : 8px;">Geometri
-000025c0: 6320 6d6f 7669 6e67 2061 7665 7261 6765  c moving average
-000025d0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-000025e0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000025f0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00002600: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00002610: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00002620: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00002630: 2f64 6f69 2e6f 7267 2f31 302e 3233 3037  /doi.org/10.2307
-00002640: 2f31 3236 3634 3433 223e 526f 6265 7274  /1266443">Robert
-00002650: 7320 2831 3935 3929 3c2f 613e 3c2f 7464  s (1959)</a></td
-00002660: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
-00002670: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00002680: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00002690: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-000026a0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-000026b0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
-000026c0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000026d0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000026e0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000026f0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002700: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
-00002710: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002720: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002730: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002740: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002750: 6464 696e 673a 2038 7078 3b22 3e50 6167  dding: 8px;">Pag
-00002760: 6520 4869 6e6b 6c65 793c 2f74 643e 0a20  e Hinkley</td>. 
-00002770: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00002780: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002790: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000027a0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000027b0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-000027c0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-000027d0: 672f 3130 2e32 3330 372f 3233 3333 3030  g/10.2307/233300
-000027e0: 3922 3e50 6167 6520 2831 3935 3429 3c2f  9">Page (1954)</
-000027f0: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
-00002800: 2020 3c74 723e 0a20 2020 203c 7464 2072    <tr>.    <td r
-00002810: 6f77 7370 616e 3d22 3622 2073 7479 6c65  owspan="6" style
-00002820: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002830: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002840: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002850: 6464 696e 673a 2038 7078 3b22 3e53 7461  dding: 8px;">Sta
-00002860: 7469 7374 6963 616c 2070 726f 6365 7373  tistical process
-00002870: 2063 6f6e 7472 6f6c 3c2f 7464 3e0a 2020   control</td>.  
-00002880: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00002890: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-000028a0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000028b0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000028c0: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
-000028d0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000028e0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000028f0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002900: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002910: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
-00002920: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00002930: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00002940: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00002950: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002960: 6e67 3a20 3870 783b 223e 4444 4d3c 2f74  ng: 8px;">DDM</t
-00002970: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002980: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002990: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-000029a0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-000029b0: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
-000029c0: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-000029d0: 692e 6f72 672f 3130 2e31 3030 372f 3937  i.org/10.1007/97
-000029e0: 382d 332d 3534 302d 3238 3634 352d 355f  8-3-540-28645-5_
-000029f0: 3239 223e 4761 6d61 2065 7420 616c 2e20  29">Gama et al. 
-00002a00: 2832 3030 3429 3c2f 613e 3c2f 7464 3e0a  (2004)</a></td>.
-00002a10: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
-00002a20: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00002a30: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002a40: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002a50: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002a60: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
-00002a70: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00002a80: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00002a90: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00002aa0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002ab0: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
-00002ac0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00002ad0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00002ae0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00002af0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00002b00: 696e 673a 2038 7078 3b22 3e45 4344 442d  ing: 8px;">ECDD-
-00002b10: 5754 3c2f 7464 3e0a 2020 2020 3c74 6420  WT</td>.    <td 
-00002b20: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00002b30: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00002b40: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00002b50: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00002b60: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
-00002b70: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
-00002b80: 3136 2f6a 2e70 6174 7265 632e 3230 3131  16/j.patrec.2011
-00002b90: 2e30 382e 3031 3922 3e52 6f73 7320 6574  .08.019">Ross et
-00002ba0: 2061 6c2e 2028 3230 3132 293c 2f61 3e3c   al. (2012)</a><
-00002bb0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-00002bc0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-00002bd0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00002be0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00002bf0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00002c00: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00002c10: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00002c20: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00002c30: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00002c40: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00002c50: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00002c60: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00002c70: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00002c80: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00002c90: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00002ca0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00002cb0: 4544 444d 3c2f 7464 3e0a 2020 2020 3c74  EDDM</td>.    <t
-00002cc0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00002cd0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00002ce0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00002cf0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00002d00: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
-00002d10: 7073 3a2f 2f77 7777 2e72 6573 6561 7263  ps://www.researc
-00002d20: 6867 6174 652e 6e65 742f 7075 626c 6963  hgate.net/public
-00002d30: 6174 696f 6e2f 3234 3539 3939 3730 345f  ation/245999704_
-00002d40: 4561 726c 795f 4472 6966 745f 4465 7465  Early_Drift_Dete
-00002d50: 6374 696f 6e5f 4d65 7468 6f64 223e 4261  ction_Method">Ba
-00002d60: 656e 612d 4761 7263 c4b1 6120 6574 2061  ena-Garc..a et a
-00002d70: 6c2e 2028 3230 3036 293c 2f61 3e3c 2f74  l. (2006)</a></t
-00002d80: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-00002d90: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00002da0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00002db0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00002dc0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002dd0: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
-00002de0: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002df0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002e00: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002e10: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002e20: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
-00002e30: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00002e40: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00002e50: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00002e60: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00002e70: 6164 6469 6e67 3a20 3870 783b 223e 4844  adding: 8px;">HD
-00002e80: 444d 2d41 3c2f 7464 3e0a 2020 2020 3c74  DM-A</td>.    <t
-00002e90: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00002ea0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00002eb0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00002ec0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00002ed0: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
-00002ee0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00002ef0: 3131 3039 2f54 4b44 452e 3230 3134 2e32  1109/TKDE.2014.2
-00002f00: 3334 3533 3832 223e 4672 6961 732d 426c  345382">Frias-Bl
-00002f10: 616e 636f 2065 7420 616c 2e20 2832 3031  anco et al. (201
-00002f20: 3429 3c2f 613e 3c2f 7464 3e0a 2020 3c2f  4)</a></td>.  </
-00002f30: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
-00002f40: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00002f50: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002f60: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00002f70: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00002f80: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
-00002f90: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00002fa0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00002fb0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002fc0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002fd0: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
-00002fe0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002ff0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00003000: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00003010: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00003020: 2038 7078 3b22 3e48 4444 4d2d 573c 2f74   8px;">HDDM-W</t
-00003030: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00003040: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00003050: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00003060: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00003070: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
-00003080: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-00003090: 692e 6f72 672f 3130 2e31 3130 392f 544b  i.org/10.1109/TK
-000030a0: 4445 2e32 3031 342e 3233 3435 3338 3222  DE.2014.2345382"
-000030b0: 3e46 7269 6173 2d42 6c61 6e63 6f20 6574  >Frias-Blanco et
-000030c0: 2061 6c2e 2028 3230 3134 293c 2f61 3e3c   al. (2014)</a><
-000030d0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-000030e0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-000030f0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003100: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00003110: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003120: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00003130: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00003140: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003150: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003160: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003170: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00003180: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003190: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000031a0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-000031b0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000031c0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000031d0: 5244 444d 3c2f 7464 3e0a 2020 2020 3c74  RDDM</td>.    <t
-000031e0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000031f0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00003200: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00003210: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00003220: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
-00003230: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00003240: 3130 3136 2f6a 2e65 7377 612e 3230 3137  1016/j.eswa.2017
-00003250: 2e30 382e 3032 3322 3e42 6172 726f 7320  .08.023">Barros 
-00003260: 6574 2061 6c2e 2028 3230 3137 293c 2f61  et al. (2017)</a
-00003270: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
-00003280: 203c 7472 3e0a 2020 2020 3c74 6420 726f   <tr>.    <td ro
-00003290: 7773 7061 6e3d 2233 2220 7374 796c 653d  wspan="3" style=
-000032a0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000032b0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000032c0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000032d0: 6469 6e67 3a20 3870 783b 223e 5769 6e64  ding: 8px;">Wind
-000032e0: 6f77 2062 6173 6564 3c2f 7464 3e0a 2020  ow based</td>.  
-000032f0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00003300: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00003310: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00003320: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00003330: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
-00003340: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00003350: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00003360: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00003370: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00003380: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
-00003390: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-000033a0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-000033b0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-000033c0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-000033d0: 6e67 3a20 3870 783b 223e 4144 5749 4e3c  ng: 8px;">ADWIN<
-000033e0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-000033f0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003400: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003410: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003420: 7061 6464 696e 673a 2038 7078 3b22 3e3c  padding: 8px;"><
-00003430: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00003440: 646f 692e 6f72 672f 3130 2e31 3133 372f  doi.org/10.1137/
-00003450: 312e 3937 3831 3631 3139 3732 3737 312e  1.9781611972771.
-00003460: 3432 223e 4269 6665 7420 616e 6420 4761  42">Bifet and Ga
-00003470: 7661 6c64 6120 2832 3030 3729 3c2f 613e  valda (2007)</a>
-00003480: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00003490: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
-000034a0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-000034b0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-000034c0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-000034d0: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
-000034e0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-000034f0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003500: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003510: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003520: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003530: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
-00003540: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003550: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003560: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003570: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003580: 3e4b 5357 494e 3c2f 7464 3e0a 2020 2020  >KSWIN</td>.    
-00003590: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000035a0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000035b0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000035c0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-000035d0: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-000035e0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-000035f0: 302e 3130 3136 2f6a 2e6e 6575 636f 6d2e  0.1016/j.neucom.
-00003600: 3230 3139 2e31 312e 3131 3122 3e52 6161  2019.11.111">Raa
-00003610: 6220 6574 2061 6c2e 2028 3230 3230 293c  b et al. (2020)<
-00003620: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
-00003630: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
-00003640: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00003650: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00003660: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00003670: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00003680: 223e 553c 2f74 643e 0a20 2020 203c 7464  ">U</td>.    <td
-00003690: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000036a0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-000036b0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-000036c0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-000036d0: 3b22 3e4e 3c2f 7464 3e0a 2020 2020 3c74  ;">N</td>.    <t
-000036e0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000036f0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00003700: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00003710: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00003720: 783b 223e 5354 4550 443c 2f74 643e 0a20  x;">STEPD</td>. 
-00003730: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00003740: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00003750: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00003760: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00003770: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-00003780: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-00003790: 672f 3130 2e31 3030 372f 3937 382d 332d  g/10.1007/978-3-
-000037a0: 3534 302d 3735 3438 382d 365f 3237 223e  540-75488-6_27">
-000037b0: 4e69 7368 6964 6120 616e 6420 5961 6d61  Nishida and Yama
-000037c0: 7563 6869 2028 3230 3037 293c 2f61 3e3c  uchi (2007)</a><
-000037d0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-000037e0: 7472 3e0a 2020 2020 3c74 6420 726f 7773  tr>.    <td rows
-000037f0: 7061 6e3d 2231 3622 2073 7479 6c65 3d22  pan="16" style="
-00003800: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00003810: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00003820: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00003830: 696e 673a 2038 7078 3b22 3e44 6174 6120  ing: 8px;">Data 
-00003840: 6472 6966 743c 2f74 643e 0a20 2020 203c  drift</td>.    <
-00003850: 7464 2072 6f77 7370 616e 3d22 3134 2220  td rowspan="14" 
-00003860: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00003870: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00003880: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00003890: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-000038a0: 223e 4261 7463 683c 2f74 643e 0a20 2020  ">Batch</td>.   
-000038b0: 203c 7464 2072 6f77 7370 616e 3d22 3922   <td rowspan="9"
-000038c0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000038d0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-000038e0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-000038f0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00003900: 3b22 3e44 6973 7461 6e63 6520 6261 7365  ;">Distance base
-00003910: 643c 2f74 643e 0a20 2020 203c 7464 2073  d</td>.    <td s
-00003920: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003930: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003940: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003950: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003960: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-00003970: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00003980: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00003990: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-000039a0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-000039b0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-000039c0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000039d0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-000039e0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-000039f0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00003a00: 3b22 3e41 6e64 6572 736f 6e2d 4461 726c  ;">Anderson-Darl
-00003a10: 696e 6720 7465 7374 3c2f 7464 3e0a 2020  ing test</td>.  
-00003a20: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00003a30: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00003a40: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00003a50: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00003a60: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
-00003a70: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
-00003a80: 2f31 302e 3233 3037 2f32 3238 3838 3035  /10.2307/2288805
-00003a90: 223e 5363 686f 6c7a 2061 6e64 2053 7465  ">Scholz and Ste
-00003aa0: 7068 656e 7320 2831 3938 3729 3c2f 613e  phens (1987)</a>
-00003ab0: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00003ac0: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
-00003ad0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003ae0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003af0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003b00: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
-00003b10: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003b20: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003b30: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003b40: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003b50: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003b60: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
-00003b70: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003b80: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003b90: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003ba0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003bb0: 3e42 6861 7474 6163 6861 7279 7961 2064  >Bhattacharyya d
-00003bc0: 6973 7461 6e63 653c 2f74 643e 0a20 2020  istance</td>.   
-00003bd0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00003be0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00003bf0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00003c00: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00003c10: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
-00003c20: 6874 7470 733a 2f2f 7777 772e 6a73 746f  https://www.jsto
-00003c30: 722e 6f72 672f 7374 6162 6c65 2f32 3530  r.org/stable/250
-00003c40: 3437 3838 3222 3e42 6861 7474 6163 6861  47882">Bhattacha
-00003c50: 7279 7961 2028 3139 3436 293c 2f61 3e3c  ryya (1946)</a><
-00003c60: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-00003c70: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-00003c80: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003c90: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00003ca0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003cb0: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00003cc0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00003cd0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003ce0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003cf0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003d00: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00003d10: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003d20: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003d30: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003d40: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003d50: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003d60: 4561 7274 6820 4d6f 7665 7227 7320 6469  Earth Mover's di
-00003d70: 7374 616e 6365 3c2f 7464 3e0a 2020 2020  stance</td>.    
-00003d80: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00003d90: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00003da0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00003db0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00003dc0: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-00003dd0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00003de0: 302e 3130 3233 2f41 3a31 3032 3635 3433  0.1023/A:1026543
-00003df0: 3930 3030 3534 223e 5275 626e 6572 2065  900054">Rubner e
-00003e00: 7420 616c 2e20 2832 3030 3029 3c2f 613e  t al. (2000)</a>
-00003e10: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00003e20: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
-00003e30: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003e40: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003e50: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003e60: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
-00003e70: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003e80: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003e90: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003ea0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003eb0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003ec0: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
-00003ed0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003ee0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003ef0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003f00: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003f10: 3e48 656c 6c69 6e67 6572 2064 6973 7461  >Hellinger dista
-00003f20: 6e63 653c 2f74 643e 0a20 2020 203c 7464  nce</td>.    <td
-00003f30: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00003f40: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00003f50: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00003f60: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00003f70: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
-00003f80: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
-00003f90: 3531 352f 4352 4c4c 2e31 3930 392e 3133  515/CRLL.1909.13
-00003fa0: 362e 3231 3022 3e48 656c 6c69 6e67 6572  6.210">Hellinger
-00003fb0: 2028 3139 3039 293c 2f61 3e3c 2f74 643e   (1909)</a></td>
-00003fc0: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
-00003fd0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00003fe0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00003ff0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004000: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004010: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
-00004020: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004030: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004040: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004050: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004060: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
-00004070: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00004080: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00004090: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000040a0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000040b0: 6469 6e67 3a20 3870 783b 223e 4869 7374  ding: 8px;">Hist
-000040c0: 6f67 7261 6d20 696e 7465 7273 6563 7469  ogram intersecti
-000040d0: 6f6e 206e 6f72 6d61 6c69 7a65 6420 636f  on normalized co
-000040e0: 6d70 6c65 6d65 6e74 3c2f 7464 3e0a 2020  mplement</td>.  
-000040f0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00004100: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00004110: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00004120: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00004130: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
-00004140: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
-00004150: 2f31 302e 3130 3037 2f42 4630 3031 3330  /10.1007/BF00130
-00004160: 3438 3722 3e53 7761 696e 2061 6e64 2042  487">Swain and B
-00004170: 616c 6c61 7264 2028 3139 3931 293c 2f61  allard (1991)</a
-00004180: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
-00004190: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
-000041a0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000041b0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-000041c0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000041d0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000041e0: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
-000041f0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004200: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004210: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004220: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004230: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
-00004240: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00004250: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00004260: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00004270: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00004280: 223e 4a65 6e73 656e 2d53 6861 6e6e 6f6e  ">Jensen-Shannon
-00004290: 2064 6973 7461 6e63 653c 2f74 643e 0a20   distance</td>. 
-000042a0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000042b0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000042c0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000042d0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000042e0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-000042f0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-00004300: 672f 3130 2e31 3130 392f 3138 2e36 3131  g/10.1109/18.611
-00004310: 3135 223e 4c69 6e20 2831 3939 3129 3c2f  15">Lin (1991)</
-00004320: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
-00004330: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
-00004340: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004350: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004360: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004370: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004380: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-00004390: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-000043a0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-000043b0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-000043c0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-000043d0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-000043e0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000043f0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004400: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004410: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004420: 3b22 3e4b 756c 6c62 6163 6b2d 4c65 6962  ;">Kullback-Leib
-00004430: 6c65 7220 6469 7665 7267 656e 6365 3c2f  ler divergence</
-00004440: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00004450: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00004460: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00004470: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00004480: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
-00004490: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-000044a0: 6f69 2e6f 7267 2f31 302e 3132 3134 2f61  oi.org/10.1214/a
-000044b0: 6f6d 732f 3131 3737 3732 3936 3934 223e  oms/1177729694">
-000044c0: 4b75 6c6c 6261 636b 2061 6e64 204c 6569  Kullback and Lei
-000044d0: 626c 6572 2028 3139 3531 293c 2f61 3e3c  bler (1951)</a><
-000044e0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-000044f0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-00004500: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00004510: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00004520: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00004530: 6164 6469 6e67 3a20 3870 783b 223e 4d3c  adding: 8px;">M<
-00004540: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00004550: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00004560: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00004570: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00004580: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00004590: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-000045a0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000045b0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-000045c0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000045d0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000045e0: 4d4d 443c 2f74 643e 0a20 2020 203c 7464  MMD</td>.    <td
-000045f0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004600: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004610: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004620: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004630: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
-00004640: 733a 2f2f 646c 2e61 636d 2e6f 7267 2f64  s://dl.acm.org/d
-00004650: 6f69 2f31 302e 3535 3535 2f32 3138 3833  oi/10.5555/21883
-00004660: 3835 2e32 3138 3834 3130 223e 4772 6574  85.2188410">Gret
-00004670: 746f 6e20 6574 2061 6c2e 2028 3230 3132  ton et al. (2012
-00004680: 293c 2f61 3e3c 2f74 643e 0a20 203c 2f74  )</a></td>.  </t
-00004690: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
-000046a0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000046b0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-000046c0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-000046d0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-000046e0: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
-000046f0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00004700: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00004710: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00004720: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00004730: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
-00004740: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00004750: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00004760: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00004770: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00004780: 3870 783b 223e 5053 493c 2f74 643e 0a20  8px;">PSI</td>. 
-00004790: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000047a0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000047b0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000047c0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000047d0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-000047e0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-000047f0: 672f 3130 2e31 3035 372f 6a6f 7273 2e32  g/10.1057/jors.2
-00004800: 3030 382e 3134 3422 3e57 7520 616e 6420  008.144">Wu and 
-00004810: 4f6c 736f 6e20 2832 3031 3029 3c2f 613e  Olson (2010)</a>
-00004820: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00004830: 3c74 723e 0a20 2020 203c 7464 2072 6f77  <tr>.    <td row
-00004840: 7370 616e 3d22 3522 2073 7479 6c65 3d22  span="5" style="
-00004850: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004860: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004870: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004880: 696e 673a 2038 7078 3b22 3e53 7461 7469  ing: 8px;">Stati
-00004890: 7374 6963 616c 2074 6573 743c 2f74 643e  stical test</td>
-000048a0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-000048b0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-000048c0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-000048d0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-000048e0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
-000048f0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00004900: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00004910: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00004920: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00004930: 6469 6e67 3a20 3870 783b 223e 433c 2f74  ding: 8px;">C</t
-00004940: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00004950: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00004960: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00004970: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00004980: 6464 696e 673a 2038 7078 3b22 3e43 6869  dding: 8px;">Chi
-00004990: 2d73 7175 6172 6520 7465 7374 3c2f 7464  -square test</td
-000049a0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000049b0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000049c0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000049d0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000049e0: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
-000049f0: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
-00004a00: 2e6f 7267 2f31 302e 3130 3830 2f31 3437  .org/10.1080/147
-00004a10: 3836 3434 3030 3039 3436 3338 3937 223e  86440009463897">
-00004a20: 5065 6172 736f 6e20 2831 3930 3029 3c2f  Pearson (1900)</
-00004a30: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
-00004a40: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
-00004a50: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004a60: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004a70: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004a80: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004a90: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-00004aa0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00004ab0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00004ac0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00004ad0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00004ae0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-00004af0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004b00: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004b10: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004b20: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004b30: 3b22 3e43 7261 6dc3 a972 2d76 6f6e 204d  ;">Cram..r-von M
-00004b40: 6973 6573 2074 6573 743c 2f74 643e 0a20  ises test</td>. 
-00004b50: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00004b60: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00004b70: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00004b80: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00004b90: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-00004ba0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-00004bb0: 672f 3130 2e31 3038 302f 3033 3436 3132  g/10.1080/034612
-00004bc0: 3338 2e31 3932 382e 3130 3431 3638 3632  38.1928.10416862
-00004bd0: 223e 4372 616d c3a9 7220 2831 3930 3229  ">Cram..r (1902)
-00004be0: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
-00004bf0: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
-00004c00: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004c10: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004c20: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004c30: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004c40: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
-00004c50: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00004c60: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00004c70: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00004c80: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00004c90: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
-00004ca0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00004cb0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00004cc0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00004cd0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00004ce0: 7078 3b22 3e4b 6f6c 6d6f 676f 726f 762d  px;">Kolmogorov-
-00004cf0: 536d 6972 6e6f 7620 7465 7374 3c2f 7464  Smirnov test</td
-00004d00: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00004d10: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00004d20: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00004d30: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00004d40: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
-00004d50: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
-00004d60: 2e6f 7267 2f31 302e 3233 3037 2f32 3238  .org/10.2307/228
-00004d70: 3030 3935 223e 4d61 7373 6579 204a 7220  0095">Massey Jr 
-00004d80: 2831 3935 3129 3c2f 613e 3c2f 7464 3e0a  (1951)</a></td>.
-00004d90: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
-00004da0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00004db0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00004dc0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00004dd0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00004de0: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
-00004df0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00004e00: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00004e10: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004e20: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004e30: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
-00004e40: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004e50: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004e60: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004e70: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004e80: 696e 673a 2038 7078 3b22 3e4d 616e 6e2d  ing: 8px;">Mann-
-00004e90: 5768 6974 6e65 7920 5520 7465 7374 3c2f  Whitney U test</
-00004ea0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00004eb0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00004ec0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00004ed0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00004ee0: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
-00004ef0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-00004f00: 6f69 2e6f 7267 2f31 302e 3132 3134 2f61  oi.org/10.1214/a
-00004f10: 6f6d 732f 3131 3737 3733 3034 3931 223e  oms/1177730491">
-00004f20: 4d61 6e6e 2061 6e64 2057 6869 746e 6579  Mann and Whitney
-00004f30: 2028 3139 3437 293c 2f61 3e3c 2f74 643e   (1947)</a></td>
-00004f40: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
-00004f50: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00004f60: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00004f70: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004f80: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004f90: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
-00004fa0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004fb0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004fc0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004fd0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004fe0: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
-00004ff0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00005000: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00005010: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00005020: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00005030: 6469 6e67 3a20 3870 783b 223e 5765 6c63  ding: 8px;">Welc
-00005040: 6827 7320 742d 7465 7374 3c2f 7464 3e0a  h's t-test</td>.
-00005050: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00005060: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00005070: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00005080: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00005090: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
-000050a0: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
-000050b0: 7267 2f31 302e 3233 3037 2f32 3333 3235  rg/10.2307/23325
-000050c0: 3130 223e 5765 6c63 6820 2831 3934 3729  10">Welch (1947)
-000050d0: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
-000050e0: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
-000050f0: 2072 6f77 7370 616e 3d22 3222 2073 7479   rowspan="2" sty
-00005100: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00005110: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00005120: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00005130: 7061 6464 696e 673a 2038 7078 3b22 3e53  padding: 8px;">S
-00005140: 7472 6561 6d69 6e67 3c2f 7464 3e0a 2020  treaming</td>.  
-00005150: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00005160: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00005170: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00005180: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00005190: 3a20 3870 783b 223e 4469 7374 616e 6365  : 8px;">Distance
-000051a0: 2062 6173 6564 3c2f 7464 3e0a 2020 2020   based</td>.    
-000051b0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000051c0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000051d0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000051e0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-000051f0: 3870 783b 223e 4d3c 2f74 643e 0a20 2020  8px;">M</td>.   
-00005200: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00005210: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00005220: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00005230: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00005240: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
-00005250: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00005260: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00005270: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00005280: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00005290: 3a20 3870 783b 223e 4d4d 443c 2f74 643e  : 8px;">MMD</td>
-000052a0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-000052b0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-000052c0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-000052d0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-000052e0: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
-000052f0: 6566 3d22 6874 7470 733a 2f2f 646c 2e61  ef="https://dl.a
-00005300: 636d 2e6f 7267 2f64 6f69 2f31 302e 3535  cm.org/doi/10.55
-00005310: 3535 2f32 3138 3833 3835 2e32 3138 3834  55/2188385.21884
-00005320: 3130 223e 4772 6574 746f 6e20 6574 2061  10">Gretton et a
-00005330: 6c2e 2028 3230 3132 293c 2f61 3e3c 2f74  l. (2012)</a></t
-00005340: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-00005350: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00005360: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00005370: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00005380: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00005390: 6469 6e67 3a20 3870 783b 223e 5374 6174  ding: 8px;">Stat
-000053a0: 6973 7469 6361 6c20 7465 7374 3c2f 7464  istical test</td
-000053b0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000053c0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000053d0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000053e0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000053f0: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
-00005400: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00005410: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00005420: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00005430: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00005440: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
-00005450: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00005460: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00005470: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00005480: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00005490: 6164 6469 6e67 3a20 3870 783b 223e 496e  adding: 8px;">In
-000054a0: 6372 656d 656e 7461 6c20 4b6f 6c6d 6f67  cremental Kolmog
-000054b0: 6f72 6f76 2d53 6d69 726e 6f76 2074 6573  orov-Smirnov tes
-000054c0: 743c 2f74 643e 0a20 2020 203c 7464 2073  t</td>.    <td s
-000054d0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-000054e0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-000054f0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00005500: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00005510: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00005520: 2f2f 646f 692e 6f72 672f 3130 2e31 3134  //doi.org/10.114
-00005530: 352f 3239 3339 3637 322e 3239 3339 3833  5/2939672.293983
-00005540: 3622 3e64 6f73 2052 6569 7320 6574 2061  6">dos Reis et a
-00005550: 6c2e 2028 3230 3136 293c 2f61 3e3c 2f74  l. (2016)</a></t
-00005560: 643e 0a20 203c 2f74 723e 0a3c 2f74 626f  d>.  </tr>.</tbo
-00005570: 6479 3e0a 3c2f 7461 626c 653e 0a0a 2323  dy>.</table>..##
-00005580: 20e2 9d97 2057 6861 7420 6973 2061 6e64   ... What is and
-00005590: 2077 6861 7420 6973 206e 6f74 2046 726f   what is not Fro
-000055a0: 7572 6f73 3f0a 0a55 6e6c 696b 6520 6f74  uros?..Unlike ot
-000055b0: 6865 7220 6c69 6272 6172 6965 7320 7468  her libraries th
-000055c0: 6174 2069 6e20 6164 6469 7469 6f6e 2074  at in addition t
-000055d0: 6f20 7072 6f76 6964 6520 6472 6966 7420  o provide drift 
-000055e0: 6465 7465 6374 696f 6e20 616c 676f 7269  detection algori
-000055f0: 7468 6d73 2c20 696e 636c 7564 6520 6f74  thms, include ot
-00005600: 6865 7220 6675 6e63 7469 6f6e 616c 6974  her functionalit
-00005610: 6965 7320 7375 6368 2061 7320 616e 6f6d  ies such as anom
-00005620: 616c 792f 6f75 746c 6965 7220 6465 7465  aly/outlier dete
-00005630: 6374 696f 6e2c 2061 6476 6572 7361 7269  ction, adversari
-00005640: 616c 2064 6574 6563 7469 6f6e 2c20 696d  al detection, im
-00005650: 6261 6c61 6e63 6520 6c65 6172 6e69 6e67  balance learning
-00005660: 2c20 616d 6f6e 6720 6f74 6865 7273 2c20  , among others, 
-00005670: 4672 6f75 726f 7320 6861 7320 616e 6420  Frouros has and 
-00005680: 7769 6c6c 202a 2a4f 4e4c 592a 2a20 6861  will **ONLY** ha
-00005690: 7665 206f 6e65 2070 7572 706f 7365 3a20  ve one purpose: 
-000056a0: 2a2a 6472 6966 7420 6465 7465 6374 696f  **drift detectio
-000056b0: 6e2a 2a2e 0a0a 5765 2066 6972 6d6c 7920  n**...We firmly 
-000056c0: 6265 6c69 6576 6520 7468 6174 206d 6163  believe that mac
-000056d0: 6869 6e65 206c 6561 726e 696e 6720 7265  hine learning re
-000056e0: 6c61 7465 6420 6c69 6272 6172 6965 7320  lated libraries 
-000056f0: 6f72 2066 7261 6d65 776f 726b 7320 7368  or frameworks sh
-00005700: 6f75 6c64 206e 6f74 2066 6f6c 6c6f 7720  ould not follow 
-00005710: 5b4a 6163 6b20 6f66 2061 6c6c 2074 7261  [Jack of all tra
-00005720: 6465 732c 206d 6173 7465 7220 6f66 206e  des, master of n
-00005730: 6f6e 655d 2868 7474 7073 3a2f 2f65 6e2e  one](https://en.
-00005740: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-00005750: 6b69 2f4a 6163 6b5f 6f66 5f61 6c6c 5f74  ki/Jack_of_all_t
-00005760: 7261 6465 732c 5f6d 6173 7465 725f 6f66  rades,_master_of
-00005770: 5f6e 6f6e 6529 2070 7269 6e63 6970 6c65  _none) principle
-00005780: 2e20 496e 7374 6561 642c 2074 6865 7920  . Instead, they 
-00005790: 7368 6f75 6c64 2062 6520 666f 6375 7365  should be focuse
-000057a0: 6420 6f6e 2061 2073 696e 676c 6520 7461  d on a single ta
-000057b0: 736b 2061 6e64 2064 6f20 6974 2077 656c  sk and do it wel
-000057c0: 6c2e 0a0a 2323 20e2 9c85 2057 686f 2069  l...## ... Who i
-000057d0: 7320 7573 696e 6720 4672 6f75 726f 733f  s using Frouros?
-000057e0: 0a0a 4672 6f75 726f 7320 6973 2061 6374  ..Frouros is act
-000057f0: 6976 656c 7920 6265 696e 6720 7573 6564  ively being used
-00005800: 2062 7920 7468 6520 666f 6c6c 6f77 696e   by the followin
-00005810: 6720 7072 6f6a 6563 7473 2074 6f20 696d  g projects to im
-00005820: 706c 656d 656e 7420 6472 6966 740a 6465  plement drift.de
-00005830: 7465 6374 696f 6e20 696e 206d 6163 6869  tection in machi
-00005840: 6e65 206c 6561 726e 696e 6720 7069 7065  ne learning pipe
-00005850: 6c69 6e65 733a 0a0a 202a 205b 4149 3445  lines:.. * [AI4E
-00005860: 4f53 435d 2868 7474 7073 3a2f 2f61 6934  OSC](https://ai4
-00005870: 656f 7363 2e65 7529 2e0a 202a 205b 694d  eosc.eu).. * [iM
-00005880: 6167 696e 655d 2868 7474 7073 3a2f 2f69  agine](https://i
-00005890: 6d61 6769 6e65 2d61 692e 6575 292e 0a0a  magine-ai.eu)...
-000058a0: 4966 2079 6f75 2077 616e 7420 796f 7572  If you want your
-000058b0: 2070 726f 6a65 6374 206c 6973 7465 6420   project listed 
-000058c0: 6865 7265 2c20 646f 206e 6f74 2068 6573  here, do not hes
-000058d0: 6974 6174 6520 746f 2073 656e 6420 7573  itate to send us
-000058e0: 2061 2070 756c 6c20 7265 7175 6573 742e   a pull request.
-000058f0: 0a0a 2323 20f0 9f91 8d20 436f 6e74 7269  ..## .... Contri
-00005900: 6275 7469 6e67 0a0a 4368 6563 6b20 6f75  buting..Check ou
-00005910: 7420 7468 6520 5b63 6f6e 7472 6962 7574  t the [contribut
-00005920: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
-00005930: 6875 622e 636f 6d2f 4946 4341 2f66 726f  hub.com/IFCA/fro
-00005940: 7572 6f73 2f62 6c6f 622f 6d61 696e 2f43  uros/blob/main/C
-00005950: 4f4e 5452 4942 5554 494e 472e 6d64 2920  ONTRIBUTING.md) 
-00005960: 7365 6374 696f 6e2e 0a0a 2323 20f0 9f92  section...## ...
-00005970: ac20 4369 7461 7469 6f6e 0a0a 416c 7468  . Citation..Alth
-00005980: 6f75 6768 2046 726f 7572 6f73 2070 6170  ough Frouros pap
-00005990: 6572 2069 7320 7374 696c 6c20 696e 2070  er is still in p
-000059a0: 7265 7072 696e 742c 2069 6620 796f 7520  reprint, if you 
-000059b0: 7761 6e74 2074 6f20 6369 7465 2069 7420  want to cite it 
-000059c0: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-000059d0: 5b70 7265 7072 696e 745d 2868 7474 7073  [preprint](https
-000059e0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-000059f0: 2f32 3230 382e 3036 3836 3829 2076 6572  /2208.06868) ver
-00005a00: 7369 6f6e 2028 746f 2062 6520 7265 706c  sion (to be repl
-00005a10: 6163 6564 2062 7920 7468 6520 7061 7065  aced by the pape
-00005a20: 7220 6f6e 6365 2069 7320 7075 626c 6973  r once is publis
-00005a30: 6865 6429 2e0a 0a60 6060 6269 6274 6578  hed)...```bibtex
-00005a40: 0a40 6172 7469 636c 657b 6365 7370 6564  .@article{cesped
-00005a50: 6573 3230 3232 6672 6f75 726f 732c 0a20  es2022frouros,. 
-00005a60: 2074 6974 6c65 3d7b 4672 6f75 726f 733a   title={Frouros:
-00005a70: 2041 2050 7974 686f 6e20 6c69 6272 6172   A Python librar
-00005a80: 7920 666f 7220 6472 6966 7420 6465 7465  y for drift dete
-00005a90: 6374 696f 6e20 696e 206d 6163 6869 6e65  ction in machine
-00005aa0: 206c 6561 726e 696e 6720 7379 7374 656d   learning system
-00005ab0: 737d 2c0a 2020 6175 7468 6f72 3d7b 437b  s},.  author={C{
-00005ac0: 5c27 657d 7370 6564 6573 2d53 6973 6e69  \'e}spedes-Sisni
-00005ad0: 6567 612c 204a 6169 6d65 2061 6e64 204c  ega, Jaime and L
-00005ae0: 7b5c 276f 7d70 657a 2d47 6172 637b 5c27  {\'o}pez-Garc{\'
-00005af0: 5c69 7d61 2c20 7b5c 2741 7d6c 7661 726f  \i}a, {\'A}lvaro
-00005b00: 207d 2c0a 2020 6a6f 7572 6e61 6c3d 7b61   },.  journal={a
-00005b10: 7258 6976 2070 7265 7072 696e 7420 6172  rXiv preprint ar
-00005b20: 5869 763a 3232 3038 2e30 3638 3638 7d2c  Xiv:2208.06868},
-00005b30: 0a20 2079 6561 723d 7b32 3032 327d 0a7d  .  year={2022}.}
-00005b40: 0a60 6060 0a0a 2323 20f0 9f93 9d20 4c69  .```..## .... Li
-00005b50: 6365 6e73 650a 0a46 726f 7572 6f73 2069  cense..Frouros i
-00005b60: 7320 616e 206f 7065 6e2d 736f 7572 6365  s an open-source
-00005b70: 2073 6f66 7477 6172 6520 6c69 6365 6e73   software licens
-00005b80: 6564 2075 6e64 6572 2074 6865 205b 4253  ed under the [BS
-00005b90: 442d 332d 436c 6175 7365 206c 6963 656e  D-3-Clause licen
-00005ba0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-00005bb0: 7562 2e63 6f6d 2f49 4643 412f 6672 6f75  ub.com/IFCA/frou
-00005bc0: 726f 732f 626c 6f62 2f6d 6169 6e2f 4c49  ros/blob/main/LI
-00005bd0: 4345 4e53 4529 2e0a 0a23 2320 f09f 998f  CENSE)...## ....
-00005be0: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
-00005bf0: 730a 0a46 726f 7572 6f73 2068 6173 2072  s..Frouros has r
-00005c00: 6563 6569 7665 6420 6675 6e64 696e 6720  eceived funding 
-00005c10: 6672 6f6d 2074 6865 2041 6765 6e63 6961  from the Agencia
-00005c20: 2045 7374 6174 616c 2064 6520 496e 7665   Estatal de Inve
-00005c30: 7374 6967 6163 69c3 b36e 2c20 556e 6964  stigaci..n, Unid
-00005c40: 6164 2064 6520 4578 6365 6c65 6e63 6961  ad de Excelencia
-00005c50: 204d 6172 c3ad 6120 6465 204d 6165 7a74   Mar..a de Maezt
-00005c60: 752c 2072 6566 2e20 4d44 4d2d 3230 3137  u, ref. MDM-2017
-00005c70: 2d30 3736 352e 0a0a 0a                   -0765....
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 203c 696d 6720 6865 6967 6874  ">.  <img height
+00000020: 3d22 3131 3570 7822 2073 7263 3d22 6874  ="115px" src="ht
+00000030: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000040: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000050: 4946 4341 2f66 726f 7572 6f73 2f6d 6169  IFCA/frouros/mai
+00000060: 6e2f 696d 6167 6573 2f6c 6f67 6f2e 706e  n/images/logo.pn
+00000070: 6722 2061 6c74 3d22 6c6f 676f 223e 0a3c  g" alt="logo">.<
+00000080: 2f70 3e0a 0a2d 2d2d 0a0a 3c70 2061 6c69  /p>..---..<p ali
+00000090: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
+000000a0: 212d 2d20 4349 202d 2d3e 0a20 203c 6120  !-- CI -->.  <a 
+000000b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000000c0: 7468 7562 2e63 6f6d 2f49 4643 412f 6672  thub.com/IFCA/fr
+000000d0: 6f75 726f 732f 6163 7469 6f6e 732f 776f  ouros/actions/wo
+000000e0: 726b 666c 6f77 732f 6369 2e79 6d6c 223e  rkflows/ci.yml">
+000000f0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000110: 6d2f 4946 4341 2f66 726f 7572 6f73 2f61  m/IFCA/frouros/a
+00000120: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000130: 2f63 692e 796d 6c2f 6261 6467 652e 7376  /ci.yml/badge.sv
+00000140: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
+00000150: 6172 6522 2061 6c74 3d22 6369 222f 3e0a  are" alt="ci"/>.
+00000160: 2020 3c2f 613e 0a20 203c 212d 2d20 436f    </a>.  <!-- Co
+00000170: 6465 2063 6f76 6572 6167 6520 2d2d 3e0a  de coverage -->.
+00000180: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000190: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+000001a0: 2f49 4643 412f 6672 6f75 726f 7322 3e0a  /IFCA/frouros">.
+000001b0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000001c0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000001d0: 2f67 682f 4946 4341 2f66 726f 7572 6f73  /gh/IFCA/frouros
+000001e0: 2f62 7261 6e63 682f 6d61 696e 2f67 7261  /branch/main/gra
+000001f0: 7068 2f62 6164 6765 2e73 7667 3f74 6f6b  ph/badge.svg?tok
+00000200: 656e 3d44 4c4b 5153 5759 5459 4d22 2061  en=DLKQSWYTYM" a
+00000210: 6c74 3d22 636f 7665 7261 6765 222f 3e0a  lt="coverage"/>.
+00000220: 2020 3c2f 613e 0a20 203c 212d 2d20 446f    </a>.  <!-- Do
+00000230: 6375 6d65 6e74 6174 696f 6e20 2d2d 3e0a  cumentation -->.
+00000240: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000250: 3a2f 2f66 726f 7572 6f73 2e72 6561 6474  ://frouros.readt
+00000260: 6865 646f 6373 2e69 6f2f 223e 0a20 2020  hedocs.io/">.   
+00000270: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000280: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
+00000290: 7267 2f70 726f 6a65 6374 732f 6672 6f75  rg/projects/frou
+000002a0: 726f 732f 6261 6467 652f 3f76 6572 7369  ros/badge/?versi
+000002b0: 6f6e 3d6c 6174 6573 7422 2061 6c74 3d22  on=latest" alt="
+000002c0: 646f 6375 6d65 6e74 6174 696f 6e22 2f3e  documentation"/>
+000002d0: 0a20 203c 2f61 3e0a 2020 3c21 2d2d 2044  .  </a>.  <!-- D
+000002e0: 6f77 6e6c 6f61 6473 202d 2d3e 0a20 203c  ownloads -->.  <
+000002f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000300: 7065 7079 2e74 6563 682f 7072 6f6a 6563  pepy.tech/projec
+00000310: 742f 6672 6f75 726f 7322 3e0a 2020 2020  t/frouros">.    
+00000320: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000330: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
+00000340: 6368 2f62 6164 6765 2f66 726f 7572 6f73  ch/badge/frouros
+00000350: 2220 616c 743d 2264 6f77 6e6c 6f61 6473  " alt="downloads
+00000360: 222f 3e0a 2020 3c2f 613e 0a20 203c 212d  "/>.  </a>.  <!-
+00000370: 2d20 5079 5049 202d 2d3e 0a20 203c 6120  - PyPI -->.  <a 
+00000380: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000390: 7069 2e6f 7267 2f70 726f 6a65 6374 2f66  pi.org/project/f
+000003a0: 726f 7572 6f73 223e 0a20 2020 203c 696d  rouros">.    <im
+000003b0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+000003c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000003d0: 7069 2f76 2f66 726f 7572 6f73 2e73 7667  pi/v/frouros.svg
+000003e0: 3f6c 6162 656c 3d72 656c 6561 7365 2663  ?label=release&c
+000003f0: 6f6c 6f72 3d62 6c75 6522 2061 6c74 3d22  olor=blue" alt="
+00000400: 7079 7069 223e 0a20 203c 2f61 3e0a 2020  pypi">.  </a>.  
+00000410: 3c21 2d2d 2050 7974 686f 6e20 2d2d 3e0a  <!-- Python -->.
+00000420: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000430: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000440: 6563 742f 6672 6f75 726f 7322 3e0a 2020  ect/frouros">.  
+00000450: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000460: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000470: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+00000480: 6e73 2f66 726f 7572 6f73 2220 616c 743d  ns/frouros" alt=
+00000490: 2270 7974 686f 6e22 3e0a 2020 3c2f 613e  "python">.  </a>
+000004a0: 0a20 203c 212d 2d20 4c69 6365 6e73 6520  .  <!-- License 
+000004b0: 2d2d 3e0a 2020 3c61 2068 7265 663d 2268  -->.  <a href="h
+000004c0: 7474 7073 3a2f 2f6f 7065 6e73 6f75 7263  ttps://opensourc
+000004d0: 652e 6f72 672f 6c69 6365 6e73 6573 2f42  e.org/licenses/B
+000004e0: 5344 2d33 2d43 6c61 7573 6522 3e0a 2020  SD-3-Clause">.  
+000004f0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000500: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000510: 696f 2f62 6164 6765 2f6c 6963 656e 7365  io/badge/license
+00000520: 2d42 5344 2532 3033 2d2d 436c 6175 7365  -BSD%203--Clause
+00000530: 2d62 6c75 652e 7376 6722 2061 6c74 3d22  -blue.svg" alt="
+00000540: 6273 645f 335f 6c69 6365 6e73 6522 3e0a  bsd_3_license">.
+00000550: 2020 3c2f 613e 0a20 203c 212d 2d20 6172    </a>.  <!-- ar
+00000560: 5869 7620 2d2d 3e0a 2020 3c61 2068 7265  Xiv -->.  <a hre
+00000570: 663d 2268 7474 7073 3a2f 2f61 7278 6976  f="https://arxiv
+00000580: 2e6f 7267 2f61 6273 2f32 3230 382e 3036  .org/abs/2208.06
+00000590: 3836 3822 3e0a 2020 2020 3c69 6d67 2073  868">.    <img s
+000005a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000005b0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000005c0: 2f61 7258 6976 2d32 3230 382e 3036 3836  /arXiv-2208.0686
+000005d0: 382d 626c 7565 2e73 7667 2220 616c 743d  8-blue.svg" alt=
+000005e0: 2261 7278 6976 223e 0a20 203c 2f61 3e0a  "arxiv">.  </a>.
+000005f0: 3c2f 703e 0a0a 4672 6f75 726f 7320 6973  </p>..Frouros is
+00000600: 2061 2050 7974 686f 6e20 6c69 6272 6172   a Python librar
+00000610: 7920 666f 7220 6472 6966 7420 6465 7465  y for drift dete
+00000620: 6374 696f 6e20 696e 206d 6163 6869 6e65  ction in machine
+00000630: 206c 6561 726e 696e 6720 7379 7374 656d   learning system
+00000640: 7320 7468 6174 2070 726f 7669 6465 7320  s that provides 
+00000650: 6120 636f 6d62 696e 6174 696f 6e20 6f66  a combination of
+00000660: 2063 6c61 7373 6963 616c 2061 6e64 206d   classical and m
+00000670: 6f72 6520 7265 6365 6e74 2061 6c67 6f72  ore recent algor
+00000680: 6974 686d 7320 666f 7220 626f 7468 2063  ithms for both c
+00000690: 6f6e 6365 7074 2061 6e64 2064 6174 6120  oncept and data 
+000006a0: 6472 6966 7420 6465 7465 6374 696f 6e2e  drift detection.
+000006b0: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+000006c0: 6572 223e 0a20 2020 203c 693e 0a20 2020  er">.    <i>.   
+000006d0: 2020 2020 2022 4576 6572 7974 6869 6e67       "Everything
+000006e0: 2063 6861 6e67 6573 2061 6e64 206e 6f74   changes and not
+000006f0: 6869 6e67 2073 7461 6e64 7320 7374 696c  hing stands stil
+00000700: 6c22 0a20 2020 203c 2f69 3e0a 3c2f 703e  l".    </i>.</p>
+00000710: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000720: 7222 3e0a 2020 2020 3c69 3e0a 2020 2020  r">.    <i>.    
+00000730: 2020 2020 2259 6f75 2063 6f75 6c64 206e      "You could n
+00000740: 6f74 2073 7465 7020 7477 6963 6520 696e  ot step twice in
+00000750: 746f 2074 6865 2073 616d 6520 7269 7665  to the same rive
+00000760: 7222 0a20 2020 203c 2f69 3e0a 3c2f 703e  r".    </i>.</p>
+00000770: 0a3c 6469 7620 616c 6967 6e3d 2263 656e  .<div align="cen
+00000780: 7465 7222 2073 7479 6c65 3d22 7769 6474  ter" style="widt
+00000790: 683a 2037 3025 3b22 3e0a 2020 2020 3c70  h: 70%;">.    <p
+000007a0: 2061 6c69 676e 3d22 7269 6768 7422 3e0a   align="right">.
+000007b0: 2020 2020 2020 2020 3c69 3e0a 2020 2020          <i>.    
+000007c0: 2020 2020 2020 2020 4865 7261 636c 6974          Heraclit
+000007d0: 7573 206f 6620 4570 6865 7375 7320 2835  us of Ephesus (5
+000007e0: 3335 2d34 3735 2042 4345 2e29 0a20 2020  35-475 BCE.).   
+000007f0: 2020 2020 203c 2f69 3e0a 2020 2020 3c2f       </i>.    </
+00000800: 703e 0a3c 2f64 6976 3e0a 0a2d 2d2d 2d0a  p>.</div>..----.
+00000810: 0a23 2320 e29a a1ef b88f 2051 7569 636b  .## ...... Quick
+00000820: 7374 6172 740a 0a23 2323 2043 6f6e 6365  start..### Conce
+00000830: 7074 2064 7269 6674 0a0a 4173 2061 2071  pt drift..As a q
+00000840: 7569 636b 2065 7861 6d70 6c65 2c20 7765  uick example, we
+00000850: 2063 616e 2075 7365 2074 6865 2062 7265   can use the bre
+00000860: 6173 7420 6361 6e63 6572 2064 6174 6173  ast cancer datas
+00000870: 6574 2074 6f20 7768 6963 6820 636f 6e63  et to which conc
+00000880: 6570 7420 6472 6966 7420 6974 2069 7320  ept drift it is 
+00000890: 696e 6475 6365 6420 616e 6420 7368 6f77  induced and show
+000008a0: 2074 6865 2075 7365 206f 6620 6120 636f   the use of a co
+000008b0: 6e63 6570 7420 6472 6966 7420 6465 7465  ncept drift dete
+000008c0: 6374 6f72 206c 696b 6520 4444 4d20 2844  ctor like DDM (D
+000008d0: 7269 6674 2044 6574 6563 7469 6f6e 204d  rift Detection M
+000008e0: 6574 686f 6429 2e20 5765 2063 616e 2073  ethod). We can s
+000008f0: 6565 2068 6f77 2063 6f6e 6365 7074 2064  ee how concept d
+00000900: 7269 6674 2061 6666 6563 7473 2074 6865  rift affects the
+00000910: 2070 6572 666f 726d 616e 6365 2069 6e20   performance in 
+00000920: 7465 726d 7320 6f66 2061 6363 7572 6163  terms of accurac
+00000930: 792e 0a0a 6060 6070 7974 686f 6e0a 696d  y...```python.im
+00000940: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+00000950: 0a66 726f 6d20 736b 6c65 6172 6e2e 6461  .from sklearn.da
+00000960: 7461 7365 7473 2069 6d70 6f72 7420 6c6f  tasets import lo
+00000970: 6164 5f62 7265 6173 745f 6361 6e63 6572  ad_breast_cancer
+00000980: 0a66 726f 6d20 736b 6c65 6172 6e2e 6c69  .from sklearn.li
+00000990: 6e65 6172 5f6d 6f64 656c 2069 6d70 6f72  near_model impor
+000009a0: 7420 4c6f 6769 7374 6963 5265 6772 6573  t LogisticRegres
+000009b0: 7369 6f6e 0a66 726f 6d20 736b 6c65 6172  sion.from sklear
+000009c0: 6e2e 6d6f 6465 6c5f 7365 6c65 6374 696f  n.model_selectio
+000009d0: 6e20 696d 706f 7274 2074 7261 696e 5f74  n import train_t
+000009e0: 6573 745f 7370 6c69 740a 6672 6f6d 2073  est_split.from s
+000009f0: 6b6c 6561 726e 2e70 6970 656c 696e 6520  klearn.pipeline 
+00000a00: 696d 706f 7274 2050 6970 656c 696e 650a  import Pipeline.
+00000a10: 6672 6f6d 2073 6b6c 6561 726e 2e70 7265  from sklearn.pre
+00000a20: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
+00000a30: 7420 5374 616e 6461 7264 5363 616c 6572  t StandardScaler
+00000a40: 0a0a 6672 6f6d 2066 726f 7572 6f73 2e64  ..from frouros.d
+00000a50: 6574 6563 746f 7273 2e63 6f6e 6365 7074  etectors.concept
+00000a60: 5f64 7269 6674 2069 6d70 6f72 7420 4444  _drift import DD
+00000a70: 4d2c 2044 444d 436f 6e66 6967 0a66 726f  M, DDMConfig.fro
+00000a80: 6d20 6672 6f75 726f 732e 6d65 7472 6963  m frouros.metric
+00000a90: 7320 696d 706f 7274 2050 7265 7175 656e  s import Prequen
+00000aa0: 7469 616c 4572 726f 720a 0a6e 702e 7261  tialError..np.ra
+00000ab0: 6e64 6f6d 2e73 6565 6428 7365 6564 3d33  ndom.seed(seed=3
+00000ac0: 3129 0a0a 2320 4c6f 6164 2062 7265 6173  1)..# Load breas
+00000ad0: 7420 6361 6e63 6572 2064 6174 6173 6574  t cancer dataset
+00000ae0: 0a58 2c20 7920 3d20 6c6f 6164 5f62 7265  .X, y = load_bre
+00000af0: 6173 745f 6361 6e63 6572 2872 6574 7572  ast_cancer(retur
+00000b00: 6e5f 585f 793d 5472 7565 290a 0a23 2053  n_X_y=True)..# S
+00000b10: 706c 6974 2074 7261 696e 2028 3730 2529  plit train (70%)
+00000b20: 2061 6e64 2074 6573 7420 2833 3025 290a   and test (30%).
+00000b30: 280a 2020 2020 585f 7472 6169 6e2c 0a20  (.    X_train,. 
+00000b40: 2020 2058 5f74 6573 742c 0a20 2020 2079     X_test,.    y
+00000b50: 5f74 7261 696e 2c0a 2020 2020 795f 7465  _train,.    y_te
+00000b60: 7374 2c0a 2920 3d20 7472 6169 6e5f 7465  st,.) = train_te
+00000b70: 7374 5f73 706c 6974 2858 2c20 792c 2074  st_split(X, y, t
+00000b80: 7261 696e 5f73 697a 653d 302e 372c 2072  rain_size=0.7, r
+00000b90: 616e 646f 6d5f 7374 6174 653d 3331 290a  andom_state=31).
+00000ba0: 0a23 2044 6566 696e 6520 616e 6420 6669  .# Define and fi
+00000bb0: 7420 6d6f 6465 6c0a 7069 7065 6c69 6e65  t model.pipeline
+00000bc0: 203d 2050 6970 656c 696e 6528 0a20 2020   = Pipeline(.   
+00000bd0: 205b 0a20 2020 2020 2020 2028 2273 6361   [.        ("sca
+00000be0: 6c65 7222 2c20 5374 616e 6461 7264 5363  ler", StandardSc
+00000bf0: 616c 6572 2829 292c 0a20 2020 2020 2020  aler()),.       
+00000c00: 2028 226d 6f64 656c 222c 204c 6f67 6973   ("model", Logis
+00000c10: 7469 6352 6567 7265 7373 696f 6e28 2929  ticRegression())
+00000c20: 2c0a 2020 2020 5d0a 290a 7069 7065 6c69  ,.    ].).pipeli
+00000c30: 6e65 2e66 6974 2858 3d58 5f74 7261 696e  ne.fit(X=X_train
+00000c40: 2c20 793d 795f 7472 6169 6e29 0a0a 2320  , y=y_train)..# 
+00000c50: 4465 7465 6374 6f72 2063 6f6e 6669 6775  Detector configu
+00000c60: 7261 7469 6f6e 2061 6e64 2069 6e73 7461  ration and insta
+00000c70: 6e74 6961 7469 6f6e 0a63 6f6e 6669 6720  ntiation.config 
+00000c80: 3d20 4444 4d43 6f6e 6669 6728 0a20 2020  = DDMConfig(.   
+00000c90: 2077 6172 6e69 6e67 5f6c 6576 656c 3d32   warning_level=2
+00000ca0: 2e30 2c0a 2020 2020 6472 6966 745f 6c65  .0,.    drift_le
+00000cb0: 7665 6c3d 332e 302c 0a20 2020 206d 696e  vel=3.0,.    min
+00000cc0: 5f6e 756d 5f69 6e73 7461 6e63 6573 3d32  _num_instances=2
+00000cd0: 352c 2020 2320 6d69 6e69 6d75 6d20 6e75  5,  # minimum nu
+00000ce0: 6d62 6572 206f 6620 696e 7374 616e 6365  mber of instance
+00000cf0: 7320 6265 666f 7265 2063 6865 636b 696e  s before checkin
+00000d00: 6720 666f 7220 636f 6e63 6570 7420 6472  g for concept dr
+00000d10: 6966 740a 290a 6465 7465 6374 6f72 203d  ift.).detector =
+00000d20: 2044 444d 2863 6f6e 6669 673d 636f 6e66   DDM(config=conf
+00000d30: 6967 290a 0a23 204d 6574 7269 6320 746f  ig)..# Metric to
+00000d40: 2063 6f6d 7075 7465 2061 6363 7572 6163   compute accurac
+00000d50: 790a 6d65 7472 6963 203d 2050 7265 7175  y.metric = Prequ
+00000d60: 656e 7469 616c 4572 726f 7228 616c 7068  entialError(alph
+00000d70: 613d 312e 3029 2020 2320 616c 7068 613d  a=1.0)  # alpha=
+00000d80: 312e 3020 6973 2065 7175 6976 616c 656e  1.0 is equivalen
+00000d90: 7420 746f 206e 6f72 6d61 6c20 6163 6375  t to normal accu
+00000da0: 7261 6379 0a0a 6465 6620 7374 7265 616d  racy..def stream
+00000db0: 5f74 6573 7428 585f 7465 7374 2c20 795f  _test(X_test, y_
+00000dc0: 7465 7374 2c20 792c 206d 6574 7269 632c  test, y, metric,
+00000dd0: 2064 6574 6563 746f 7229 3a0a 2020 2020   detector):.    
+00000de0: 2222 2253 696d 756c 6174 6520 6461 7461  """Simulate data
+00000df0: 2073 7472 6561 6d20 6f76 6572 2058 5f74   stream over X_t
+00000e00: 6573 7420 616e 6420 795f 7465 7374 2e20  est and y_test. 
+00000e10: 7920 6973 2074 6865 2074 7275 6520 6c61  y is the true la
+00000e20: 6265 6c2e 2222 220a 2020 2020 6472 6966  bel.""".    drif
+00000e30: 745f 666c 6167 203d 2046 616c 7365 0a20  t_flag = False. 
+00000e40: 2020 2066 6f72 2069 2c20 2858 2c20 7929     for i, (X, y)
+00000e50: 2069 6e20 656e 756d 6572 6174 6528 7a69   in enumerate(zi
+00000e60: 7028 585f 7465 7374 2c20 795f 7465 7374  p(X_test, y_test
+00000e70: 2929 3a0a 2020 2020 2020 2020 795f 7072  )):.        y_pr
+00000e80: 6564 203d 2070 6970 656c 696e 652e 7072  ed = pipeline.pr
+00000e90: 6564 6963 7428 582e 7265 7368 6170 6528  edict(X.reshape(
+00000ea0: 312c 202d 3129 290a 2020 2020 2020 2020  1, -1)).        
+00000eb0: 6572 726f 7220 3d20 3120 2d20 2879 5f70  error = 1 - (y_p
+00000ec0: 7265 642e 6974 656d 2829 203d 3d20 792e  red.item() == y.
+00000ed0: 6974 656d 2829 290a 2020 2020 2020 2020  item()).        
+00000ee0: 6d65 7472 6963 5f65 7272 6f72 203d 206d  metric_error = m
+00000ef0: 6574 7269 6328 6572 726f 725f 7661 6c75  etric(error_valu
+00000f00: 653d 6572 726f 7229 0a20 2020 2020 2020  e=error).       
+00000f10: 205f 203d 2064 6574 6563 746f 722e 7570   _ = detector.up
+00000f20: 6461 7465 2876 616c 7565 3d65 7272 6f72  date(value=error
+00000f30: 290a 2020 2020 2020 2020 7374 6174 7573  ).        status
+00000f40: 203d 2064 6574 6563 746f 722e 7374 6174   = detector.stat
+00000f50: 7573 0a20 2020 2020 2020 2069 6620 7374  us.        if st
+00000f60: 6174 7573 5b22 6472 6966 7422 5d20 616e  atus["drift"] an
+00000f70: 6420 6e6f 7420 6472 6966 745f 666c 6167  d not drift_flag
+00000f80: 3a0a 2020 2020 2020 2020 2020 2020 6472  :.            dr
+00000f90: 6966 745f 666c 6167 203d 2054 7275 650a  ift_flag = True.
+00000fa0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000fb0: 7428 6622 436f 6e63 6570 7420 6472 6966  t(f"Concept drif
+00000fc0: 7420 6465 7465 6374 6564 2061 7420 7374  t detected at st
+00000fd0: 6570 207b 697d 2e20 4163 6375 7261 6379  ep {i}. Accuracy
+00000fe0: 3a20 7b31 202d 206d 6574 7269 635f 6572  : {1 - metric_er
+00000ff0: 726f 723a 2e34 667d 2229 0a20 2020 2069  ror:.4f}").    i
+00001000: 6620 6e6f 7420 6472 6966 745f 666c 6167  f not drift_flag
+00001010: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00001020: 224e 6f20 636f 6e63 6570 7420 6472 6966  "No concept drif
+00001030: 7420 6465 7465 6374 6564 2229 0a20 2020  t detected").   
+00001040: 2070 7269 6e74 2866 2246 696e 616c 2061   print(f"Final a
+00001050: 6363 7572 6163 793a 207b 3120 2d20 6d65  ccuracy: {1 - me
+00001060: 7472 6963 5f65 7272 6f72 3a2e 3466 7d5c  tric_error:.4f}\
+00001070: 6e22 290a 0a23 2053 696d 756c 6174 6520  n")..# Simulate 
+00001080: 6461 7461 2073 7472 6561 6d20 2861 7373  data stream (ass
+00001090: 756d 696e 6720 7465 7374 206c 6162 656c  uming test label
+000010a0: 2061 7661 696c 6162 6c65 2061 6674 6572   available after
+000010b0: 2065 6163 6820 7072 6564 6963 7469 6f6e   each prediction
+000010c0: 290a 2320 4e6f 2063 6f6e 6365 7074 2064  ).# No concept d
+000010d0: 7269 6674 2069 7320 6578 7065 6374 6564  rift is expected
+000010e0: 2074 6f20 6f63 6375 720a 7374 7265 616d   to occur.stream
+000010f0: 5f74 6573 7428 0a20 2020 2058 5f74 6573  _test(.    X_tes
+00001100: 743d 585f 7465 7374 2c0a 2020 2020 795f  t=X_test,.    y_
+00001110: 7465 7374 3d79 5f74 6573 742c 0a20 2020  test=y_test,.   
+00001120: 2079 3d79 2c0a 2020 2020 6d65 7472 6963   y=y,.    metric
+00001130: 3d6d 6574 7269 632c 0a20 2020 2064 6574  =metric,.    det
+00001140: 6563 746f 723d 6465 7465 6374 6f72 2c0a  ector=detector,.
+00001150: 290a 2320 3e3e 204e 6f20 636f 6e63 6570  ).# >> No concep
+00001160: 7420 6472 6966 7420 6465 7465 6374 6564  t drift detected
+00001170: 0a23 203e 3e20 4669 6e61 6c20 6163 6375  .# >> Final accu
+00001180: 7261 6379 3a20 302e 3937 3636 0a0a 2320  racy: 0.9766..# 
+00001190: 494d 504f 5254 414e 543a 2049 6e64 7563  IMPORTANT: Induc
+000011a0: 652f 7369 6d75 6c61 7465 2063 6f6e 6365  e/simulate conce
+000011b0: 7074 2064 7269 6674 2069 6e20 7468 6520  pt drift in the 
+000011c0: 6c61 7374 2070 6172 7420 2832 3025 290a  last part (20%).
+000011d0: 2320 6f66 2079 5f74 6573 7420 6279 206d  # of y_test by m
+000011e0: 6f64 6966 7969 6e67 2073 6f6d 6520 6c61  odifying some la
+000011f0: 6265 6c73 2028 3530 2520 6170 7072 6f78  bels (50% approx
+00001200: 292e 2054 6865 7265 666f 7265 2c20 6368  ). Therefore, ch
+00001210: 616e 6769 6e67 2050 2879 7c58 2929 0a64  anging P(y|X)).d
+00001220: 7269 6674 5f73 697a 6520 3d20 696e 7428  rift_size = int(
+00001230: 795f 7465 7374 2e73 6861 7065 5b30 5d20  y_test.shape[0] 
+00001240: 2a20 302e 3229 0a79 5f74 6573 745f 6472  * 0.2).y_test_dr
+00001250: 6966 7420 3d20 795f 7465 7374 5b2d 6472  ift = y_test[-dr
+00001260: 6966 745f 7369 7a65 3a5d 0a6d 6f64 6966  ift_size:].modif
+00001270: 795f 6964 7820 3d20 6e70 2e72 616e 646f  y_idx = np.rando
+00001280: 6d2e 7261 6e64 282a 795f 7465 7374 5f64  m.rand(*y_test_d
+00001290: 7269 6674 2e73 6861 7065 2920 3c3d 2030  rift.shape) <= 0
+000012a0: 2e35 0a79 5f74 6573 745f 6472 6966 745b  .5.y_test_drift[
+000012b0: 6d6f 6469 6679 5f69 6478 5d20 3d20 2879  modify_idx] = (y
+000012c0: 5f74 6573 745f 6472 6966 745b 6d6f 6469  _test_drift[modi
+000012d0: 6679 5f69 6478 5d20 2b20 3129 2025 206c  fy_idx] + 1) % l
+000012e0: 656e 286e 702e 756e 6971 7565 2879 5f74  en(np.unique(y_t
+000012f0: 6573 7429 290a 795f 7465 7374 5b2d 6472  est)).y_test[-dr
+00001300: 6966 745f 7369 7a65 3a5d 203d 2079 5f74  ift_size:] = y_t
+00001310: 6573 745f 6472 6966 740a 0a23 2052 6573  est_drift..# Res
+00001320: 6574 2064 6574 6563 746f 7220 616e 6420  et detector and 
+00001330: 6d65 7472 6963 0a64 6574 6563 746f 722e  metric.detector.
+00001340: 7265 7365 7428 290a 6d65 7472 6963 2e72  reset().metric.r
+00001350: 6573 6574 2829 0a0a 2320 5369 6d75 6c61  eset()..# Simula
+00001360: 7465 2064 6174 6120 7374 7265 616d 2028  te data stream (
+00001370: 6173 7375 6d69 6e67 2074 6573 7420 6c61  assuming test la
+00001380: 6265 6c20 6176 6169 6c61 626c 6520 6166  bel available af
+00001390: 7465 7220 6561 6368 2070 7265 6469 6374  ter each predict
+000013a0: 696f 6e29 0a23 2043 6f6e 6365 7074 2064  ion).# Concept d
+000013b0: 7269 6674 2069 7320 6578 7065 6374 6564  rift is expected
+000013c0: 2074 6f20 6f63 6375 7220 6265 6361 7573   to occur becaus
+000013d0: 6520 6f66 2074 6865 206c 6162 656c 206d  e of the label m
+000013e0: 6f64 6966 6963 6174 696f 6e0a 7374 7265  odification.stre
+000013f0: 616d 5f74 6573 7428 0a20 2020 2058 5f74  am_test(.    X_t
+00001400: 6573 743d 585f 7465 7374 2c0a 2020 2020  est=X_test,.    
+00001410: 795f 7465 7374 3d79 5f74 6573 742c 0a20  y_test=y_test,. 
+00001420: 2020 2079 3d79 2c0a 2020 2020 6d65 7472     y=y,.    metr
+00001430: 6963 3d6d 6574 7269 632c 0a20 2020 2064  ic=metric,.    d
+00001440: 6574 6563 746f 723d 6465 7465 6374 6f72  etector=detector
+00001450: 2c0a 290a 2320 3e3e 2043 6f6e 6365 7074  ,.).# >> Concept
+00001460: 2064 7269 6674 2064 6574 6563 7465 6420   drift detected 
+00001470: 6174 2073 7465 7020 3134 322e 2041 6363  at step 142. Acc
+00001480: 7572 6163 793a 2030 2e39 3531 300a 2320  uracy: 0.9510.# 
+00001490: 3e3e 2046 696e 616c 2061 6363 7572 6163  >> Final accurac
+000014a0: 793a 2030 2e38 3438 300a 6060 600a 0a4d  y: 0.8480.```..M
+000014b0: 6f72 6520 636f 6e63 6570 7420 6472 6966  ore concept drif
+000014c0: 7420 6578 616d 706c 6573 2063 616e 2062  t examples can b
+000014d0: 6520 666f 756e 6420 5b68 6572 655d 2868  e found [here](h
+000014e0: 7474 7073 3a2f 2f66 726f 7572 6f73 2e72  ttps://frouros.r
+000014f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00001500: 2f6c 6174 6573 742f 6578 616d 706c 6573  /latest/examples
+00001510: 2f63 6f6e 6365 7074 5f64 7269 6674 2e68  /concept_drift.h
+00001520: 746d 6c29 2e0a 0a23 2323 2044 6174 6120  tml)...### Data 
+00001530: 6472 6966 740a 0a41 7320 6120 7175 6963  drift..As a quic
+00001540: 6b20 6578 616d 706c 652c 2077 6520 6361  k example, we ca
+00001550: 6e20 7573 6520 7468 6520 6972 6973 2064  n use the iris d
+00001560: 6174 6173 6574 2074 6f20 7768 6963 6820  ataset to which 
+00001570: 6461 7461 2064 7269 6674 2069 7320 696e  data drift is in
+00001580: 6475 6365 6420 616e 6420 7368 6f77 2074  duced and show t
+00001590: 6865 2075 7365 206f 6620 6120 6461 7461  he use of a data
+000015a0: 2064 7269 6674 2064 6574 6563 746f 7220   drift detector 
+000015b0: 6c69 6b65 204b 6f6c 6d6f 676f 726f 762d  like Kolmogorov-
+000015c0: 536d 6972 6e6f 7620 7465 7374 2e0a 0a60  Smirnov test...`
+000015d0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+000015e0: 6e75 6d70 7920 6173 206e 700a 6672 6f6d  numpy as np.from
+000015f0: 2073 6b6c 6561 726e 2e64 6174 6173 6574   sklearn.dataset
+00001600: 7320 696d 706f 7274 206c 6f61 645f 6972  s import load_ir
+00001610: 6973 0a66 726f 6d20 736b 6c65 6172 6e2e  is.from sklearn.
+00001620: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e20  model_selection 
+00001630: 696d 706f 7274 2074 7261 696e 5f74 6573  import train_tes
+00001640: 745f 7370 6c69 740a 6672 6f6d 2073 6b6c  t_split.from skl
+00001650: 6561 726e 2e74 7265 6520 696d 706f 7274  earn.tree import
+00001660: 2044 6563 6973 696f 6e54 7265 6543 6c61   DecisionTreeCla
+00001670: 7373 6966 6965 720a 0a66 726f 6d20 6672  ssifier..from fr
+00001680: 6f75 726f 732e 6465 7465 6374 6f72 732e  ouros.detectors.
+00001690: 6461 7461 5f64 7269 6674 2069 6d70 6f72  data_drift impor
+000016a0: 7420 4b53 5465 7374 0a0a 6e70 2e72 616e  t KSTest..np.ran
+000016b0: 646f 6d2e 7365 6564 2873 6565 643d 3331  dom.seed(seed=31
+000016c0: 290a 0a23 204c 6f61 6420 6972 6973 2064  )..# Load iris d
+000016d0: 6174 6173 6574 0a58 2c20 7920 3d20 6c6f  ataset.X, y = lo
+000016e0: 6164 5f69 7269 7328 7265 7475 726e 5f58  ad_iris(return_X
+000016f0: 5f79 3d54 7275 6529 0a0a 2320 5370 6c69  _y=True)..# Spli
+00001700: 7420 7472 6169 6e20 2837 3025 2920 616e  t train (70%) an
+00001710: 6420 7465 7374 2028 3330 2529 0a28 0a20  d test (30%).(. 
+00001720: 2020 2058 5f74 7261 696e 2c0a 2020 2020     X_train,.    
+00001730: 585f 7465 7374 2c0a 2020 2020 795f 7472  X_test,.    y_tr
+00001740: 6169 6e2c 0a20 2020 2079 5f74 6573 742c  ain,.    y_test,
+00001750: 0a29 203d 2074 7261 696e 5f74 6573 745f  .) = train_test_
+00001760: 7370 6c69 7428 582c 2079 2c20 7472 6169  split(X, y, trai
+00001770: 6e5f 7369 7a65 3d30 2e37 2c20 7261 6e64  n_size=0.7, rand
+00001780: 6f6d 5f73 7461 7465 3d33 3129 0a0a 2320  om_state=31)..# 
+00001790: 5365 7420 7468 6520 6665 6174 7572 6520  Set the feature 
+000017a0: 696e 6465 7820 746f 2077 6869 6368 2064  index to which d
+000017b0: 6574 6563 746f 7220 6973 2061 7070 6c69  etector is appli
+000017c0: 6564 0a66 6561 7475 7265 5f69 6478 203d  ed.feature_idx =
+000017d0: 2030 0a0a 2320 494d 504f 5254 414e 543a   0..# IMPORTANT:
+000017e0: 2049 6e64 7563 652f 7369 6d75 6c61 7465   Induce/simulate
+000017f0: 2064 6174 6120 6472 6966 7420 696e 2074   data drift in t
+00001800: 6865 2073 656c 6563 7465 6420 6665 6174  he selected feat
+00001810: 7572 6520 6f66 2079 5f74 6573 7420 6279  ure of y_test by
+00001820: 0a23 2061 7070 6c79 696e 6720 736f 6d65  .# applying some
+00001830: 2067 6175 7373 6961 6e20 6e6f 6973 652e   gaussian noise.
+00001840: 2054 6865 7265 666f 7265 2c20 6368 616e   Therefore, chan
+00001850: 6769 6e67 2050 2858 2929 0a58 5f74 6573  ging P(X)).X_tes
+00001860: 745b 3a2c 2066 6561 7475 7265 5f69 6478  t[:, feature_idx
+00001870: 5d20 2b3d 206e 702e 7261 6e64 6f6d 2e6e  ] += np.random.n
+00001880: 6f72 6d61 6c28 0a20 2020 206c 6f63 3d30  ormal(.    loc=0
+00001890: 2e30 2c0a 2020 2020 7363 616c 653d 332e  .0,.    scale=3.
+000018a0: 302c 0a20 2020 2073 697a 653d 585f 7465  0,.    size=X_te
+000018b0: 7374 2e73 6861 7065 5b30 5d2c 0a29 0a0a  st.shape[0],.)..
+000018c0: 2320 4465 6669 6e65 2061 6e64 2066 6974  # Define and fit
+000018d0: 206d 6f64 656c 0a6d 6f64 656c 203d 2044   model.model = D
+000018e0: 6563 6973 696f 6e54 7265 6543 6c61 7373  ecisionTreeClass
+000018f0: 6966 6965 7228 7261 6e64 6f6d 5f73 7461  ifier(random_sta
+00001900: 7465 3d33 3129 0a6d 6f64 656c 2e66 6974  te=31).model.fit
+00001910: 2858 3d58 5f74 7261 696e 2c20 793d 795f  (X=X_train, y=y_
+00001920: 7472 6169 6e29 0a0a 2320 5365 7420 7369  train)..# Set si
+00001930: 676e 6966 6963 616e 6365 206c 6576 656c  gnificance level
+00001940: 2066 6f72 2068 7970 6f74 6865 7369 7320   for hypothesis 
+00001950: 7465 7374 696e 670a 616c 7068 6120 3d20  testing.alpha = 
+00001960: 302e 3030 310a 2320 4465 6669 6e65 2061  0.001.# Define a
+00001970: 6e64 2066 6974 2064 6574 6563 746f 720a  nd fit detector.
+00001980: 6465 7465 6374 6f72 203d 204b 5354 6573  detector = KSTes
+00001990: 7428 290a 5f20 3d20 6465 7465 6374 6f72  t()._ = detector
+000019a0: 2e66 6974 2858 3d58 5f74 7261 696e 5b3a  .fit(X=X_train[:
+000019b0: 2c20 6665 6174 7572 655f 6964 785d 290a  , feature_idx]).
+000019c0: 0a23 2041 7070 6c79 2064 6574 6563 746f  .# Apply detecto
+000019d0: 7220 746f 2074 6865 2073 656c 6563 7465  r to the selecte
+000019e0: 6420 6665 6174 7572 6520 6f66 2058 5f74  d feature of X_t
+000019f0: 6573 740a 7265 7375 6c74 2c20 5f20 3d20  est.result, _ = 
+00001a00: 6465 7465 6374 6f72 2e63 6f6d 7061 7265  detector.compare
+00001a10: 2858 3d58 5f74 6573 745b 3a2c 2066 6561  (X=X_test[:, fea
+00001a20: 7475 7265 5f69 6478 5d29 0a0a 2320 4368  ture_idx])..# Ch
+00001a30: 6563 6b20 6966 2064 7269 6674 2069 7320  eck if drift is 
+00001a40: 7461 6b69 6e67 2070 6c61 6365 0a69 6620  taking place.if 
+00001a50: 7265 7375 6c74 2e70 5f76 616c 7565 203c  result.p_value <
+00001a60: 3d20 616c 7068 613a 0a20 2020 2070 7269  = alpha:.    pri
+00001a70: 6e74 2866 2244 6174 6120 6472 6966 7420  nt(f"Data drift 
+00001a80: 6465 7465 6374 6564 2061 7420 6665 6174  detected at feat
+00001a90: 7572 6520 7b66 6561 7475 7265 5f69 6478  ure {feature_idx
+00001aa0: 7d22 290a 656c 7365 3a0a 2020 2020 7072  }").else:.    pr
+00001ab0: 696e 7428 6622 4e6f 2064 6174 6120 6472  int(f"No data dr
+00001ac0: 6966 7420 6465 7465 6374 6564 2061 7420  ift detected at 
+00001ad0: 6665 6174 7572 6520 7b66 6561 7475 7265  feature {feature
+00001ae0: 5f69 6478 7d22 290a 2320 3e3e 2044 6174  _idx}").# >> Dat
+00001af0: 6120 6472 6966 7420 6465 7465 6374 6564  a drift detected
+00001b00: 2061 7420 6665 6174 7572 6520 300a 2320   at feature 0.# 
+00001b10: 5468 6572 6566 6f72 652c 2077 6520 6361  Therefore, we ca
+00001b20: 6e20 7265 6a65 6374 2048 3020 2862 6f74  n reject H0 (bot
+00001b30: 6820 7361 6d70 6c65 7320 636f 6d65 2066  h samples come f
+00001b40: 726f 6d20 7468 6520 7361 6d65 2064 6973  rom the same dis
+00001b50: 7472 6962 7574 696f 6e29 2e0a 6060 600a  tribution)..```.
+00001b60: 0a4d 6f72 6520 6461 7461 2064 7269 6674  .More data drift
+00001b70: 2065 7861 6d70 6c65 7320 6361 6e20 6265   examples can be
+00001b80: 2066 6f75 6e64 205b 6865 7265 5d28 6874   found [here](ht
+00001b90: 7470 733a 2f2f 6672 6f75 726f 732e 7265  tps://frouros.re
+00001ba0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00001bb0: 6c61 7465 7374 2f65 7861 6d70 6c65 732f  latest/examples/
+00001bc0: 6461 7461 5f64 7269 6674 2e68 746d 6c29  data_drift.html)
+00001bd0: 2e0a 0a23 2320 f09f 9ba0 2049 6e73 7461  ...## .... Insta
+00001be0: 6c6c 6174 696f 6e0a 0a46 726f 7572 6f73  llation..Frouros
+00001bf0: 2063 616e 2062 6520 696e 7374 616c 6c65   can be installe
+00001c00: 6420 7669 6120 7069 703a 0a0a 6060 6062  d via pip:..```b
+00001c10: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+00001c20: 6672 6f75 726f 730a 6060 600a 0a23 2320  frouros.```..## 
+00001c30: f09f 95b5 f09f 8fbb e280 8de2 9982 efb8  ................
+00001c40: 8fef b88f 2044 7269 6674 2064 6574 6563  .... Drift detec
+00001c50: 7469 6f6e 206d 6574 686f 6473 0a0a 5468  tion methods..Th
+00001c60: 6520 6375 7272 656e 746c 7920 696d 706c  e currently impl
+00001c70: 656d 656e 7465 6420 6465 7465 6374 6f72  emented detector
+00001c80: 7320 6172 6520 6c69 7374 6564 2069 6e20  s are listed in 
+00001c90: 7468 6520 666f 6c6c 6f77 696e 6720 7461  the following ta
+00001ca0: 626c 652e 0a0a 3c74 6162 6c65 2073 7479  ble...<table sty
+00001cb0: 6c65 3d22 7769 6474 683a 2031 3030 253b  le="width: 100%;
+00001cc0: 2074 6578 742d 616c 6967 6e3a 2063 656e   text-align: cen
+00001cd0: 7465 723b 2062 6f72 6465 722d 636f 6c6c  ter; border-coll
+00001ce0: 6170 7365 3a20 636f 6c6c 6170 7365 3b20  apse: collapse; 
+00001cf0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00001d00: 6420 6772 6579 3b22 3e0a 2020 3c74 6865  d grey;">.  <the
+00001d10: 6164 3e0a 2020 2020 3c74 723e 0a20 2020  ad>.    <tr>.   
+00001d20: 203c 7468 2073 7479 6c65 3d22 7465 7874   <th style="text
+00001d30: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00001d40: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00001d50: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00001d60: 2034 7078 3b22 3e44 7269 6674 2064 6574   4px;">Drift det
+00001d70: 6563 746f 723c 2f74 683e 0a20 2020 203c  ector</th>.    <
+00001d80: 7468 2073 7479 6c65 3d22 7465 7874 2d61  th style="text-a
+00001d90: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00001da0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00001db0: 6772 6579 3b20 7061 6464 696e 673a 2034  grey; padding: 4
+00001dc0: 7078 3b22 3e54 7970 653c 2f74 683e 0a20  px;">Type</th>. 
+00001dd0: 2020 203c 7468 2073 7479 6c65 3d22 7465     <th style="te
+00001de0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00001df0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00001e00: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00001e10: 673a 2034 7078 3b22 3e46 616d 696c 793c  g: 4px;">Family<
+00001e20: 2f74 683e 0a20 2020 203c 7468 2073 7479  /th>.    <th sty
+00001e30: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00001e40: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00001e50: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00001e60: 7061 6464 696e 673a 2034 7078 3b22 3e55  padding: 4px;">U
+00001e70: 6e69 7661 7269 6174 6520 2855 2920 2f20  nivariate (U) / 
+00001e80: 4d75 6c74 6976 6172 6961 7465 2028 4d29  Multivariate (M)
+00001e90: 3c2f 7468 3e0a 2020 2020 3c74 6820 7374  </th>.    <th st
+00001ea0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00001eb0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00001ec0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00001ed0: 2070 6164 6469 6e67 3a20 3470 783b 223e   padding: 4px;">
+00001ee0: 4e75 6d65 7269 6361 6c20 284e 2920 2f20  Numerical (N) / 
+00001ef0: 4361 7465 676f 7269 6361 6c20 2843 293c  Categorical (C)<
+00001f00: 2f74 683e 0a20 2020 203c 7468 2073 7479  /th>.    <th sty
+00001f10: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00001f20: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00001f30: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00001f40: 7061 6464 696e 673a 2034 7078 3b22 3e4d  padding: 4px;">M
+00001f50: 6574 686f 643c 2f74 683e 0a20 2020 203c  ethod</th>.    <
+00001f60: 7468 2073 7479 6c65 3d22 7465 7874 2d61  th style="text-a
+00001f70: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00001f80: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00001f90: 6772 6579 3b20 7061 6464 696e 673a 2034  grey; padding: 4
+00001fa0: 7078 3b22 3e52 6566 6572 656e 6365 3c2f  px;">Reference</
+00001fb0: 7468 3e0a 2020 2020 3c2f 7472 3e0a 2020  th>.    </tr>.  
+00001fc0: 3c2f 7468 6561 643e 0a20 203c 7462 6f64  </thead>.  <tbod
+00001fd0: 793e 0a20 203c 7472 3e0a 2020 2020 3c74  y>.  <tr>.    <t
+00001fe0: 6420 726f 7773 7061 6e3d 2231 3322 2073  d rowspan="13" s
+00001ff0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00002000: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00002010: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00002020: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00002030: 3e43 6f6e 6365 7074 2064 7269 6674 3c2f  >Concept drift</
+00002040: 7464 3e0a 2020 2020 3c74 6420 726f 7773  td>.    <td rows
+00002050: 7061 6e3d 2231 3322 2073 7479 6c65 3d22  pan="13" style="
+00002060: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00002070: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00002080: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00002090: 696e 673a 2038 7078 3b22 3e53 7472 6561  ing: 8px;">Strea
+000020a0: 6d69 6e67 3c2f 7464 3e0a 2020 2020 3c74  ming</td>.    <t
+000020b0: 6420 726f 7773 7061 6e3d 2234 2220 7374  d rowspan="4" st
+000020c0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+000020d0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+000020e0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+000020f0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00002100: 4368 616e 6765 2064 6574 6563 7469 6f6e  Change detection
+00002110: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00002120: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00002130: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00002140: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00002150: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00002160: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00002170: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00002180: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00002190: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+000021a0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+000021b0: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+000021c0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000021d0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000021e0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000021f0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00002200: 223e 424f 4344 3c2f 7464 3e0a 2020 2020  ">BOCD</td>.    
+00002210: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00002220: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00002230: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00002240: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00002250: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
+00002260: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
+00002270: 302e 3438 3535 302f 6172 5869 762e 3037  0.48550/arXiv.07
+00002280: 3130 2e33 3734 3222 3e41 6461 6d73 2061  10.3742">Adams a
+00002290: 6e64 204d 6163 4b61 7920 2832 3030 3729  nd MacKay (2007)
+000022a0: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
+000022b0: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
+000022c0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+000022d0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+000022e0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000022f0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00002300: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
+00002310: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00002320: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00002330: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00002340: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00002350: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
+00002360: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00002370: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00002380: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00002390: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+000023a0: 7078 3b22 3e43 5553 554d 3c2f 7464 3e0a  px;">CUSUM</td>.
+000023b0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+000023c0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+000023d0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000023e0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000023f0: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
+00002400: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
+00002410: 7267 2f31 302e 3233 3037 2f32 3333 3330  rg/10.2307/23330
+00002420: 3039 223e 5061 6765 2028 3139 3534 293c  09">Page (1954)<
+00002430: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
+00002440: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
+00002450: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00002460: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00002470: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00002480: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00002490: 223e 553c 2f74 643e 0a20 2020 203c 7464  ">U</td>.    <td
+000024a0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+000024b0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+000024c0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000024d0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000024e0: 3b22 3e4e 3c2f 7464 3e0a 2020 2020 3c74  ;">N</td>.    <t
+000024f0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00002500: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00002510: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00002520: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00002530: 783b 223e 4765 6f6d 6574 7269 6320 6d6f  x;">Geometric mo
+00002540: 7669 6e67 2061 7665 7261 6765 3c2f 7464  ving average</td
+00002550: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00002560: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002570: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002580: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002590: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
+000025a0: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
+000025b0: 2e6f 7267 2f31 302e 3233 3037 2f31 3236  .org/10.2307/126
+000025c0: 3634 3433 223e 526f 6265 7274 7320 2831  6443">Roberts (1
+000025d0: 3935 3929 3c2f 613e 3c2f 7464 3e0a 2020  959)</a></td>.  
+000025e0: 3c2f 7472 3e0a 2020 3c74 723e 0a20 2020  </tr>.  <tr>.   
+000025f0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002600: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002610: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002620: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00002630: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
+00002640: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00002650: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00002660: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002670: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002680: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
+00002690: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+000026a0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000026b0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000026c0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000026d0: 673a 2038 7078 3b22 3e50 6167 6520 4869  g: 8px;">Page Hi
+000026e0: 6e6b 6c65 793c 2f74 643e 0a20 2020 203c  nkley</td>.    <
+000026f0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00002700: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00002710: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00002720: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00002730: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+00002740: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00002750: 2e32 3330 372f 3233 3333 3030 3922 3e50  .2307/2333009">P
+00002760: 6167 6520 2831 3935 3429 3c2f 613e 3c2f  age (1954)</a></
+00002770: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00002780: 723e 0a20 2020 203c 7464 2072 6f77 7370  r>.    <td rowsp
+00002790: 616e 3d22 3622 2073 7479 6c65 3d22 7465  an="6" style="te
+000027a0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000027b0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000027c0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000027d0: 673a 2038 7078 3b22 3e53 7461 7469 7374  g: 8px;">Statist
+000027e0: 6963 616c 2070 726f 6365 7373 2063 6f6e  ical process con
+000027f0: 7472 6f6c 3c2f 7464 3e0a 2020 2020 3c74  trol</td>.    <t
+00002800: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00002810: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00002820: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00002830: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00002840: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
+00002850: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00002860: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00002870: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00002880: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00002890: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
+000028a0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+000028b0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+000028c0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+000028d0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+000028e0: 3870 783b 223e 4444 4d3c 2f74 643e 0a20  8px;">DDM</td>. 
+000028f0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00002900: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00002910: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00002920: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00002930: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
+00002940: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+00002950: 672f 3130 2e31 3030 372f 3937 382d 332d  g/10.1007/978-3-
+00002960: 3534 302d 3238 3634 352d 355f 3239 223e  540-28645-5_29">
+00002970: 4761 6d61 2065 7420 616c 2e20 2832 3030  Gama et al. (200
+00002980: 3429 3c2f 613e 3c2f 7464 3e0a 2020 3c2f  4)</a></td>.  </
+00002990: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
+000029a0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+000029b0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+000029c0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+000029d0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+000029e0: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
+000029f0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00002a00: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00002a10: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00002a20: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00002a30: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
+00002a40: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002a50: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002a60: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002a70: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00002a80: 2038 7078 3b22 3e45 4344 442d 5754 3c2f   8px;">ECDD-WT</
+00002a90: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+00002aa0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00002ab0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00002ac0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00002ad0: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
+00002ae0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00002af0: 6f69 2e6f 7267 2f31 302e 3130 3136 2f6a  oi.org/10.1016/j
+00002b00: 2e70 6174 7265 632e 3230 3131 2e30 382e  .patrec.2011.08.
+00002b10: 3031 3922 3e52 6f73 7320 6574 2061 6c2e  019">Ross et al.
+00002b20: 2028 3230 3132 293c 2f61 3e3c 2f74 643e   (2012)</a></td>
+00002b30: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+00002b40: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00002b50: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00002b60: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00002b70: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00002b80: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
+00002b90: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00002ba0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00002bb0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00002bc0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00002bd0: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
+00002be0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00002bf0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002c00: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002c10: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002c20: 6469 6e67 3a20 3870 783b 223e 4544 444d  ding: 8px;">EDDM
+00002c30: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00002c40: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00002c50: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00002c60: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00002c70: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00002c80: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002c90: 2f77 7777 2e72 6573 6561 7263 6867 6174  /www.researchgat
+00002ca0: 652e 6e65 742f 7075 626c 6963 6174 696f  e.net/publicatio
+00002cb0: 6e2f 3234 3539 3939 3730 345f 4561 726c  n/245999704_Earl
+00002cc0: 795f 4472 6966 745f 4465 7465 6374 696f  y_Drift_Detectio
+00002cd0: 6e5f 4d65 7468 6f64 223e 4261 656e 612d  n_Method">Baena-
+00002ce0: 4761 7263 c4b1 6120 6574 2061 6c2e 2028  Garc..a et al. (
+00002cf0: 3230 3036 293c 2f61 3e3c 2f74 643e 0a20  2006)</a></td>. 
+00002d00: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
+00002d10: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00002d20: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00002d30: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002d40: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002d50: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
+00002d60: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00002d70: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00002d80: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00002d90: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00002da0: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
+00002db0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00002dc0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00002dd0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00002de0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00002df0: 6e67 3a20 3870 783b 223e 4844 444d 2d41  ng: 8px;">HDDM-A
+00002e00: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00002e10: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00002e20: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00002e30: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00002e40: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00002e50: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002e60: 2f64 6f69 2e6f 7267 2f31 302e 3131 3039  /doi.org/10.1109
+00002e70: 2f54 4b44 452e 3230 3134 2e32 3334 3533  /TKDE.2014.23453
+00002e80: 3832 223e 4672 6961 732d 426c 616e 636f  82">Frias-Blanco
+00002e90: 2065 7420 616c 2e20 2832 3031 3429 3c2f   et al. (2014)</
+00002ea0: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
+00002eb0: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
+00002ec0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00002ed0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00002ee0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00002ef0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00002f00: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
+00002f10: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00002f20: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00002f30: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00002f40: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00002f50: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
+00002f60: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00002f70: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00002f80: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00002f90: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00002fa0: 3b22 3e48 4444 4d2d 573c 2f74 643e 0a20  ;">HDDM-W</td>. 
+00002fb0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00002fc0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00002fd0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00002fe0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00002ff0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
+00003000: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+00003010: 672f 3130 2e31 3130 392f 544b 4445 2e32  g/10.1109/TKDE.2
+00003020: 3031 342e 3233 3435 3338 3222 3e46 7269  014.2345382">Fri
+00003030: 6173 2d42 6c61 6e63 6f20 6574 2061 6c2e  as-Blanco et al.
+00003040: 2028 3230 3134 293c 2f61 3e3c 2f74 643e   (2014)</a></td>
+00003050: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+00003060: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00003070: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00003080: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00003090: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000030a0: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
+000030b0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+000030c0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000030d0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+000030e0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000030f0: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
+00003100: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00003110: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00003120: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00003130: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00003140: 6469 6e67 3a20 3870 783b 223e 5244 444d  ding: 8px;">RDDM
+00003150: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00003160: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00003170: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00003180: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00003190: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+000031a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000031b0: 2f64 6f69 2e6f 7267 2f31 302e 3130 3136  /doi.org/10.1016
+000031c0: 2f6a 2e65 7377 612e 3230 3137 2e30 382e  /j.eswa.2017.08.
+000031d0: 3032 3322 3e42 6172 726f 7320 6574 2061  023">Barros et a
+000031e0: 6c2e 2028 3230 3137 293c 2f61 3e3c 2f74  l. (2017)</a></t
+000031f0: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
+00003200: 3e0a 2020 2020 3c74 6420 726f 7773 7061  >.    <td rowspa
+00003210: 6e3d 2233 2220 7374 796c 653d 2274 6578  n="3" style="tex
+00003220: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00003230: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00003240: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00003250: 3a20 3870 783b 223e 5769 6e64 6f77 2062  : 8px;">Window b
+00003260: 6173 6564 3c2f 7464 3e0a 2020 2020 3c74  ased</td>.    <t
+00003270: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00003280: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00003290: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+000032a0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+000032b0: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
+000032c0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+000032d0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+000032e0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+000032f0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00003300: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
+00003310: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00003320: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00003330: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00003340: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00003350: 3870 783b 223e 4144 5749 4e3c 2f74 643e  8px;">ADWIN</td>
+00003360: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00003370: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003380: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003390: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000033a0: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
+000033b0: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
+000033c0: 6f72 672f 3130 2e31 3133 372f 312e 3937  org/10.1137/1.97
+000033d0: 3831 3631 3139 3732 3737 312e 3432 223e  81611972771.42">
+000033e0: 4269 6665 7420 616e 6420 4761 7661 6c64  Bifet and Gavald
+000033f0: 6120 2832 3030 3729 3c2f 613e 3c2f 7464  a (2007)</a></td
+00003400: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+00003410: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00003420: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003430: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003440: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00003450: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
+00003460: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00003470: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00003480: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00003490: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+000034a0: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
+000034b0: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+000034c0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000034d0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000034e0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000034f0: 6464 696e 673a 2038 7078 3b22 3e4b 5357  dding: 8px;">KSW
+00003500: 494e 3c2f 7464 3e0a 2020 2020 3c74 6420  IN</td>.    <td 
+00003510: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003520: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003530: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003540: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003550: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00003560: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
+00003570: 3136 2f6a 2e6e 6575 636f 6d2e 3230 3139  16/j.neucom.2019
+00003580: 2e31 312e 3131 3122 3e52 6161 6220 6574  .11.111">Raab et
+00003590: 2061 6c2e 2028 3230 3230 293c 2f61 3e3c   al. (2020)</a><
+000035a0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+000035b0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
+000035c0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000035d0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000035e0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000035f0: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
+00003600: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003610: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003620: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003630: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003640: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
+00003650: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00003660: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00003670: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00003680: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00003690: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+000036a0: 5354 4550 443c 2f74 643e 0a20 2020 203c  STEPD</td>.    <
+000036b0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+000036c0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+000036d0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+000036e0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+000036f0: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+00003700: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00003710: 2e31 3030 372f 3937 382d 332d 3534 302d  .1007/978-3-540-
+00003720: 3735 3438 382d 365f 3237 223e 4e69 7368  75488-6_27">Nish
+00003730: 6964 6120 616e 6420 5961 6d61 7563 6869  ida and Yamauchi
+00003740: 2028 3230 3037 293c 2f61 3e3c 2f74 643e   (2007)</a></td>
+00003750: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+00003760: 2020 2020 3c74 6420 726f 7773 7061 6e3d      <td rowspan=
+00003770: 2231 3622 2073 7479 6c65 3d22 7465 7874  "16" style="text
+00003780: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00003790: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+000037a0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+000037b0: 2038 7078 3b22 3e44 6174 6120 6472 6966   8px;">Data drif
+000037c0: 743c 2f74 643e 0a20 2020 203c 7464 2072  t</td>.    <td r
+000037d0: 6f77 7370 616e 3d22 3134 2220 7374 796c  owspan="14" styl
+000037e0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000037f0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003800: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003810: 6164 6469 6e67 3a20 3870 783b 223e 4261  adding: 8px;">Ba
+00003820: 7463 683c 2f74 643e 0a20 2020 203c 7464  tch</td>.    <td
+00003830: 2072 6f77 7370 616e 3d22 3922 2073 7479   rowspan="9" sty
+00003840: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003850: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003860: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003870: 7061 6464 696e 673a 2038 7078 3b22 3e44  padding: 8px;">D
+00003880: 6973 7461 6e63 6520 6261 7365 643c 2f74  istance based</t
+00003890: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+000038a0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000038b0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000038c0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000038d0: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+000038e0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000038f0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00003900: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003910: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003920: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00003930: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003940: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003950: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003960: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003970: 7061 6464 696e 673a 2038 7078 3b22 3e41  padding: 8px;">A
+00003980: 6e64 6572 736f 6e2d 4461 726c 696e 6720  nderson-Darling 
+00003990: 7465 7374 3c2f 7464 3e0a 2020 2020 3c74  test</td>.    <t
+000039a0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+000039b0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+000039c0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+000039d0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+000039e0: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
+000039f0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00003a00: 3233 3037 2f32 3238 3838 3035 223e 5363  2307/2288805">Sc
+00003a10: 686f 6c7a 2061 6e64 2053 7465 7068 656e  holz and Stephen
+00003a20: 7320 2831 3938 3729 3c2f 613e 3c2f 7464  s (1987)</a></td
+00003a30: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+00003a40: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00003a50: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003a60: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003a70: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00003a80: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
+00003a90: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00003aa0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00003ab0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00003ac0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00003ad0: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
+00003ae0: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00003af0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00003b00: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00003b10: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00003b20: 6464 696e 673a 2038 7078 3b22 3e42 6861  dding: 8px;">Bha
+00003b30: 7474 6163 6861 7279 7961 2064 6973 7461  ttacharyya dista
+00003b40: 6e63 653c 2f74 643e 0a20 2020 203c 7464  nce</td>.    <td
+00003b50: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00003b60: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00003b70: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00003b80: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00003b90: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
+00003ba0: 733a 2f2f 7777 772e 6a73 746f 722e 6f72  s://www.jstor.or
+00003bb0: 672f 7374 6162 6c65 2f32 3530 3437 3838  g/stable/2504788
+00003bc0: 3222 3e42 6861 7474 6163 6861 7279 7961  2">Bhattacharyya
+00003bd0: 2028 3139 3436 293c 2f61 3e3c 2f74 643e   (1946)</a></td>
+00003be0: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+00003bf0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00003c00: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00003c10: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00003c20: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00003c30: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
+00003c40: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00003c50: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003c60: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003c70: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00003c80: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
+00003c90: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00003ca0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00003cb0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00003cc0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00003cd0: 6469 6e67 3a20 3870 783b 223e 4561 7274  ding: 8px;">Eart
+00003ce0: 6820 4d6f 7665 7227 7320 6469 7374 616e  h Mover's distan
+00003cf0: 6365 3c2f 7464 3e0a 2020 2020 3c74 6420  ce</td>.    <td 
+00003d00: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003d10: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003d20: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003d30: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003d40: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00003d50: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
+00003d60: 3233 2f41 3a31 3032 3635 3433 3930 3030  23/A:10265439000
+00003d70: 3534 223e 5275 626e 6572 2065 7420 616c  54">Rubner et al
+00003d80: 2e20 2832 3030 3029 3c2f 613e 3c2f 7464  . (2000)</a></td
+00003d90: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+00003da0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00003db0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003dc0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003dd0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00003de0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
+00003df0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00003e00: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00003e10: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00003e20: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00003e30: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
+00003e40: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00003e50: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00003e60: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00003e70: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00003e80: 6464 696e 673a 2038 7078 3b22 3e48 656c  dding: 8px;">Hel
+00003e90: 6c69 6e67 6572 2064 6973 7461 6e63 653c  linger distance<
+00003ea0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003eb0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003ec0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003ed0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003ee0: 7061 6464 696e 673a 2038 7078 3b22 3e3c  padding: 8px;"><
+00003ef0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00003f00: 646f 692e 6f72 672f 3130 2e31 3531 352f  doi.org/10.1515/
+00003f10: 4352 4c4c 2e31 3930 392e 3133 362e 3231  CRLL.1909.136.21
+00003f20: 3022 3e48 656c 6c69 6e67 6572 2028 3139  0">Hellinger (19
+00003f30: 3039 293c 2f61 3e3c 2f74 643e 0a20 203c  09)</a></td>.  <
+00003f40: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
+00003f50: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00003f60: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00003f70: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00003f80: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00003f90: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
+00003fa0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00003fb0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00003fc0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00003fd0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00003fe0: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
+00003ff0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004000: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004010: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00004020: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00004030: 3a20 3870 783b 223e 4869 7374 6f67 7261  : 8px;">Histogra
+00004040: 6d20 696e 7465 7273 6563 7469 6f6e 206e  m intersection n
+00004050: 6f72 6d61 6c69 7a65 6420 636f 6d70 6c65  ormalized comple
+00004060: 6d65 6e74 3c2f 7464 3e0a 2020 2020 3c74  ment</td>.    <t
+00004070: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00004080: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00004090: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+000040a0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+000040b0: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
+000040c0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+000040d0: 3130 3037 2f42 4630 3031 3330 3438 3722  1007/BF00130487"
+000040e0: 3e53 7761 696e 2061 6e64 2042 616c 6c61  >Swain and Balla
+000040f0: 7264 2028 3139 3931 293c 2f61 3e3c 2f74  rd (1991)</a></t
+00004100: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
+00004110: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00004120: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00004130: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00004140: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00004150: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
+00004160: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00004170: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00004180: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00004190: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000041a0: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
+000041b0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000041c0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000041d0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000041e0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000041f0: 6164 6469 6e67 3a20 3870 783b 223e 4a65  adding: 8px;">Je
+00004200: 6e73 656e 2d53 6861 6e6e 6f6e 2064 6973  nsen-Shannon dis
+00004210: 7461 6e63 653c 2f74 643e 0a20 2020 203c  tance</td>.    <
+00004220: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004230: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004240: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004250: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004260: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+00004270: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00004280: 2e31 3130 392f 3138 2e36 3131 3135 223e  .1109/18.61115">
+00004290: 4c69 6e20 2831 3939 3129 3c2f 613e 3c2f  Lin (1991)</a></
+000042a0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+000042b0: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+000042c0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000042d0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000042e0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000042f0: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+00004300: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+00004310: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00004320: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00004330: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00004340: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00004350: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00004360: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004370: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004380: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004390: 7061 6464 696e 673a 2038 7078 3b22 3e4b  padding: 8px;">K
+000043a0: 756c 6c62 6163 6b2d 4c65 6962 6c65 7220  ullback-Leibler 
+000043b0: 6469 7665 7267 656e 6365 3c2f 7464 3e0a  divergence</td>.
+000043c0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+000043d0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+000043e0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000043f0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004400: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
+00004410: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
+00004420: 7267 2f31 302e 3132 3134 2f61 6f6d 732f  rg/10.1214/aoms/
+00004430: 3131 3737 3732 3936 3934 223e 4b75 6c6c  1177729694">Kull
+00004440: 6261 636b 2061 6e64 204c 6569 626c 6572  back and Leibler
+00004450: 2028 3139 3531 293c 2f61 3e3c 2f74 643e   (1951)</a></td>
+00004460: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+00004470: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00004480: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004490: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000044a0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000044b0: 6e67 3a20 3870 783b 223e 4d3c 2f74 643e  ng: 8px;">M</td>
+000044c0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+000044d0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000044e0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+000044f0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00004500: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
+00004510: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00004520: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00004530: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00004540: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00004550: 6469 6e67 3a20 3870 783b 223e 4d4d 443c  ding: 8px;">MMD<
+00004560: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00004570: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004580: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004590: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+000045a0: 7061 6464 696e 673a 2038 7078 3b22 3e3c  padding: 8px;"><
+000045b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000045c0: 646c 2e61 636d 2e6f 7267 2f64 6f69 2f31  dl.acm.org/doi/1
+000045d0: 302e 3535 3535 2f32 3138 3833 3835 2e32  0.5555/2188385.2
+000045e0: 3138 3834 3130 223e 4772 6574 746f 6e20  188410">Gretton 
+000045f0: 6574 2061 6c2e 2028 3230 3132 293c 2f61  et al. (2012)</a
+00004600: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+00004610: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
+00004620: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00004630: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00004640: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00004650: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004660: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00004670: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00004680: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00004690: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+000046a0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+000046b0: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+000046c0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000046d0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000046e0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000046f0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00004700: 223e 5053 493c 2f74 643e 0a20 2020 203c  ">PSI</td>.    <
+00004710: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004720: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004730: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004740: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004750: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+00004760: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00004770: 2e31 3035 372f 6a6f 7273 2e32 3030 382e  .1057/jors.2008.
+00004780: 3134 3422 3e57 7520 616e 6420 4f6c 736f  144">Wu and Olso
+00004790: 6e20 2832 3031 3029 3c2f 613e 3c2f 7464  n (2010)</a></td
+000047a0: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+000047b0: 0a20 2020 203c 7464 2072 6f77 7370 616e  .    <td rowspan
+000047c0: 3d22 3522 2073 7479 6c65 3d22 7465 7874  ="5" style="text
+000047d0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+000047e0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+000047f0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004800: 2038 7078 3b22 3e53 7461 7469 7374 6963   8px;">Statistic
+00004810: 616c 2074 6573 743c 2f74 643e 0a20 2020  al test</td>.   
+00004820: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00004830: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00004840: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00004850: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004860: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
+00004870: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004880: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004890: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000048a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000048b0: 3a20 3870 783b 223e 433c 2f74 643e 0a20  : 8px;">C</td>. 
+000048c0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+000048d0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000048e0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000048f0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00004900: 673a 2038 7078 3b22 3e43 6869 2d73 7175  g: 8px;">Chi-squ
+00004910: 6172 6520 7465 7374 3c2f 7464 3e0a 2020  are test</td>.  
+00004920: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004930: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004940: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00004950: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00004960: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00004970: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00004980: 2f31 302e 3130 3830 2f31 3437 3836 3434  /10.1080/1478644
+00004990: 3030 3039 3436 3338 3937 223e 5065 6172  0009463897">Pear
+000049a0: 736f 6e20 2831 3930 3029 3c2f 613e 3c2f  son (1900)</a></
+000049b0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+000049c0: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+000049d0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000049e0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000049f0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00004a00: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+00004a10: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+00004a20: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00004a30: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00004a40: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00004a50: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00004a60: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00004a70: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004a80: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004a90: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004aa0: 7061 6464 696e 673a 2038 7078 3b22 3e43  padding: 8px;">C
+00004ab0: 7261 6dc3 a972 2d76 6f6e 204d 6973 6573  ram..r-von Mises
+00004ac0: 2074 6573 743c 2f74 643e 0a20 2020 203c   test</td>.    <
+00004ad0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004ae0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004af0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004b00: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004b10: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+00004b20: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00004b30: 2e31 3038 302f 3033 3436 3132 3338 2e31  .1080/03461238.1
+00004b40: 3932 382e 3130 3431 3638 3632 223e 4372  928.10416862">Cr
+00004b50: 616d c3a9 7220 2831 3930 3229 3c2f 613e  am..r (1902)</a>
+00004b60: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
+00004b70: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
+00004b80: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004b90: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004ba0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004bb0: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
+00004bc0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00004bd0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00004be0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00004bf0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00004c00: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004c10: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
+00004c20: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00004c30: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00004c40: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00004c50: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00004c60: 3e4b 6f6c 6d6f 676f 726f 762d 536d 6972  >Kolmogorov-Smir
+00004c70: 6e6f 7620 7465 7374 3c2f 7464 3e0a 2020  nov test</td>.  
+00004c80: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004c90: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004ca0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00004cb0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00004cc0: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00004cd0: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00004ce0: 2f31 302e 3233 3037 2f32 3238 3030 3935  /10.2307/2280095
+00004cf0: 223e 4d61 7373 6579 204a 7220 2831 3935  ">Massey Jr (195
+00004d00: 3129 3c2f 613e 3c2f 7464 3e0a 2020 3c2f  1)</a></td>.  </
+00004d10: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
+00004d20: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004d30: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004d40: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004d50: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004d60: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
+00004d70: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00004d80: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00004d90: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00004da0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00004db0: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
+00004dc0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00004dd0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00004de0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00004df0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004e00: 2038 7078 3b22 3e4d 616e 6e2d 5768 6974   8px;">Mann-Whit
+00004e10: 6e65 7920 5520 7465 7374 3c2f 7464 3e0a  ney U test</td>.
+00004e20: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00004e30: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004e40: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00004e50: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004e60: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
+00004e70: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
+00004e80: 7267 2f31 302e 3132 3134 2f61 6f6d 732f  rg/10.1214/aoms/
+00004e90: 3131 3737 3733 3034 3931 223e 4d61 6e6e  1177730491">Mann
+00004ea0: 2061 6e64 2057 6869 746e 6579 2028 3139   and Whitney (19
+00004eb0: 3437 293c 2f61 3e3c 2f74 643e 0a20 203c  47)</a></td>.  <
+00004ec0: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
+00004ed0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00004ee0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00004ef0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00004f00: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00004f10: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
+00004f20: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00004f30: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00004f40: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00004f50: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004f60: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
+00004f70: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004f80: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004f90: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00004fa0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00004fb0: 3a20 3870 783b 223e 5765 6c63 6827 7320  : 8px;">Welch's 
+00004fc0: 742d 7465 7374 3c2f 7464 3e0a 2020 2020  t-test</td>.    
+00004fd0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00004fe0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00004ff0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00005000: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00005010: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
+00005020: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
+00005030: 302e 3233 3037 2f32 3333 3235 3130 223e  0.2307/2332510">
+00005040: 5765 6c63 6820 2831 3934 3729 3c2f 613e  Welch (1947)</a>
+00005050: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
+00005060: 3c74 723e 0a20 2020 203c 7464 2072 6f77  <tr>.    <td row
+00005070: 7370 616e 3d22 3222 2073 7479 6c65 3d22  span="2" style="
+00005080: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00005090: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+000050a0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000050b0: 696e 673a 2038 7078 3b22 3e53 7472 6561  ing: 8px;">Strea
+000050c0: 6d69 6e67 3c2f 7464 3e0a 2020 2020 3c74  ming</td>.    <t
+000050d0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+000050e0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+000050f0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00005100: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00005110: 783b 223e 4469 7374 616e 6365 2062 6173  x;">Distance bas
+00005120: 6564 3c2f 7464 3e0a 2020 2020 3c74 6420  ed</td>.    <td 
+00005130: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00005140: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00005150: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00005160: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00005170: 223e 4d3c 2f74 643e 0a20 2020 203c 7464  ">M</td>.    <td
+00005180: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00005190: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+000051a0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000051b0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000051c0: 3b22 3e4e 3c2f 7464 3e0a 2020 2020 3c74  ;">N</td>.    <t
+000051d0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+000051e0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+000051f0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00005200: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00005210: 783b 223e 4d4d 443c 2f74 643e 0a20 2020  x;">MMD</td>.   
+00005220: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00005230: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00005240: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00005250: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00005260: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
+00005270: 6874 7470 733a 2f2f 646c 2e61 636d 2e6f  https://dl.acm.o
+00005280: 7267 2f64 6f69 2f31 302e 3535 3535 2f32  rg/doi/10.5555/2
+00005290: 3138 3833 3835 2e32 3138 3834 3130 223e  188385.2188410">
+000052a0: 4772 6574 746f 6e20 6574 2061 6c2e 2028  Gretton et al. (
+000052b0: 3230 3132 293c 2f61 3e3c 2f74 643e 0a20  2012)</a></td>. 
+000052c0: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
+000052d0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+000052e0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000052f0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00005300: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00005310: 3a20 3870 783b 223e 5374 6174 6973 7469  : 8px;">Statisti
+00005320: 6361 6c20 7465 7374 3c2f 7464 3e0a 2020  cal test</td>.  
+00005330: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00005340: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00005350: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00005360: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00005370: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
+00005380: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00005390: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000053a0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000053b0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000053c0: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
+000053d0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+000053e0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+000053f0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00005400: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00005410: 6e67 3a20 3870 783b 223e 496e 6372 656d  ng: 8px;">Increm
+00005420: 656e 7461 6c20 4b6f 6c6d 6f67 6f72 6f76  ental Kolmogorov
+00005430: 2d53 6d69 726e 6f76 2074 6573 743c 2f74  -Smirnov test</t
+00005440: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00005450: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00005460: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00005470: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00005480: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
+00005490: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+000054a0: 692e 6f72 672f 3130 2e31 3134 352f 3239  i.org/10.1145/29
+000054b0: 3339 3637 322e 3239 3339 3833 3622 3e64  39672.2939836">d
+000054c0: 6f73 2052 6569 7320 6574 2061 6c2e 2028  os Reis et al. (
+000054d0: 3230 3136 293c 2f61 3e3c 2f74 643e 0a20  2016)</a></td>. 
+000054e0: 203c 2f74 723e 0a3c 2f74 626f 6479 3e0a   </tr>.</tbody>.
+000054f0: 3c2f 7461 626c 653e 0a0a 2323 20e2 9d97  </table>..## ...
+00005500: 2057 6861 7420 6973 2061 6e64 2077 6861   What is and wha
+00005510: 7420 6973 206e 6f74 2046 726f 7572 6f73  t is not Frouros
+00005520: 3f0a 0a55 6e6c 696b 6520 6f74 6865 7220  ?..Unlike other 
+00005530: 6c69 6272 6172 6965 7320 7468 6174 2069  libraries that i
+00005540: 6e20 6164 6469 7469 6f6e 2074 6f20 7072  n addition to pr
+00005550: 6f76 6964 6520 6472 6966 7420 6465 7465  ovide drift dete
+00005560: 6374 696f 6e20 616c 676f 7269 7468 6d73  ction algorithms
+00005570: 2c20 696e 636c 7564 6520 6f74 6865 7220  , include other 
+00005580: 6675 6e63 7469 6f6e 616c 6974 6965 7320  functionalities 
+00005590: 7375 6368 2061 7320 616e 6f6d 616c 792f  such as anomaly/
+000055a0: 6f75 746c 6965 7220 6465 7465 6374 696f  outlier detectio
+000055b0: 6e2c 2061 6476 6572 7361 7269 616c 2064  n, adversarial d
+000055c0: 6574 6563 7469 6f6e 2c20 696d 6261 6c61  etection, imbala
+000055d0: 6e63 6520 6c65 6172 6e69 6e67 2c20 616d  nce learning, am
+000055e0: 6f6e 6720 6f74 6865 7273 2c20 4672 6f75  ong others, Frou
+000055f0: 726f 7320 6861 7320 616e 6420 7769 6c6c  ros has and will
+00005600: 202a 2a4f 4e4c 592a 2a20 6861 7665 206f   **ONLY** have o
+00005610: 6e65 2070 7572 706f 7365 3a20 2a2a 6472  ne purpose: **dr
+00005620: 6966 7420 6465 7465 6374 696f 6e2a 2a2e  ift detection**.
+00005630: 0a0a 5765 2066 6972 6d6c 7920 6265 6c69  ..We firmly beli
+00005640: 6576 6520 7468 6174 206d 6163 6869 6e65  eve that machine
+00005650: 206c 6561 726e 696e 6720 7265 6c61 7465   learning relate
+00005660: 6420 6c69 6272 6172 6965 7320 6f72 2066  d libraries or f
+00005670: 7261 6d65 776f 726b 7320 7368 6f75 6c64  rameworks should
+00005680: 206e 6f74 2066 6f6c 6c6f 7720 5b4a 6163   not follow [Jac
+00005690: 6b20 6f66 2061 6c6c 2074 7261 6465 732c  k of all trades,
+000056a0: 206d 6173 7465 7220 6f66 206e 6f6e 655d   master of none]
+000056b0: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
+000056c0: 7065 6469 612e 6f72 672f 7769 6b69 2f4a  pedia.org/wiki/J
+000056d0: 6163 6b5f 6f66 5f61 6c6c 5f74 7261 6465  ack_of_all_trade
+000056e0: 732c 5f6d 6173 7465 725f 6f66 5f6e 6f6e  s,_master_of_non
+000056f0: 6529 2070 7269 6e63 6970 6c65 2e20 496e  e) principle. In
+00005700: 7374 6561 642c 2074 6865 7920 7368 6f75  stead, they shou
+00005710: 6c64 2062 6520 666f 6375 7365 6420 6f6e  ld be focused on
+00005720: 2061 2073 696e 676c 6520 7461 736b 2061   a single task a
+00005730: 6e64 2064 6f20 6974 2077 656c 6c2e 0a0a  nd do it well...
+00005740: 2323 20e2 9c85 2057 686f 2069 7320 7573  ## ... Who is us
+00005750: 696e 6720 4672 6f75 726f 733f 0a0a 4672  ing Frouros?..Fr
+00005760: 6f75 726f 7320 6973 2061 6374 6976 656c  ouros is activel
+00005770: 7920 6265 696e 6720 7573 6564 2062 7920  y being used by 
+00005780: 7468 6520 666f 6c6c 6f77 696e 6720 7072  the following pr
+00005790: 6f6a 6563 7473 2074 6f20 696d 706c 656d  ojects to implem
+000057a0: 656e 7420 6472 6966 740a 6465 7465 6374  ent drift.detect
+000057b0: 696f 6e20 696e 206d 6163 6869 6e65 206c  ion in machine l
+000057c0: 6561 726e 696e 6720 7069 7065 6c69 6e65  earning pipeline
+000057d0: 733a 0a0a 202a 205b 4149 3445 4f53 435d  s:.. * [AI4EOSC]
+000057e0: 2868 7474 7073 3a2f 2f61 6934 656f 7363  (https://ai4eosc
+000057f0: 2e65 7529 2e0a 202a 205b 694d 6167 696e  .eu).. * [iMagin
+00005800: 655d 2868 7474 7073 3a2f 2f69 6d61 6769  e](https://imagi
+00005810: 6e65 2d61 692e 6575 292e 0a0a 4966 2079  ne-ai.eu)...If y
+00005820: 6f75 2077 616e 7420 796f 7572 2070 726f  ou want your pro
+00005830: 6a65 6374 206c 6973 7465 6420 6865 7265  ject listed here
+00005840: 2c20 646f 206e 6f74 2068 6573 6974 6174  , do not hesitat
+00005850: 6520 746f 2073 656e 6420 7573 2061 2070  e to send us a p
+00005860: 756c 6c20 7265 7175 6573 742e 0a0a 2323  ull request...##
+00005870: 20f0 9f91 8d20 436f 6e74 7269 6275 7469   .... Contributi
+00005880: 6e67 0a0a 4368 6563 6b20 6f75 7420 7468  ng..Check out th
+00005890: 6520 5b63 6f6e 7472 6962 7574 696f 6e5d  e [contribution]
+000058a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000058b0: 636f 6d2f 4946 4341 2f66 726f 7572 6f73  com/IFCA/frouros
+000058c0: 2f62 6c6f 622f 6d61 696e 2f43 4f4e 5452  /blob/main/CONTR
+000058d0: 4942 5554 494e 472e 6d64 2920 7365 6374  IBUTING.md) sect
+000058e0: 696f 6e2e 0a0a 2323 20f0 9f92 ac20 4369  ion...## .... Ci
+000058f0: 7461 7469 6f6e 0a0a 416c 7468 6f75 6768  tation..Although
+00005900: 2046 726f 7572 6f73 2070 6170 6572 2069   Frouros paper i
+00005910: 7320 7374 696c 6c20 696e 2070 7265 7072  s still in prepr
+00005920: 696e 742c 2069 6620 796f 7520 7761 6e74  int, if you want
+00005930: 2074 6f20 6369 7465 2069 7420 796f 7520   to cite it you 
+00005940: 6361 6e20 7573 6520 7468 6520 5b70 7265  can use the [pre
+00005950: 7072 696e 745d 2868 7474 7073 3a2f 2f61  print](https://a
+00005960: 7278 6976 2e6f 7267 2f61 6273 2f32 3230  rxiv.org/abs/220
+00005970: 382e 3036 3836 3829 2076 6572 7369 6f6e  8.06868) version
+00005980: 2028 746f 2062 6520 7265 706c 6163 6564   (to be replaced
+00005990: 2062 7920 7468 6520 7061 7065 7220 6f6e   by the paper on
+000059a0: 6365 2069 7320 7075 626c 6973 6865 6429  ce is published)
+000059b0: 2e0a 0a60 6060 6269 6274 6578 0a40 6172  ...```bibtex.@ar
+000059c0: 7469 636c 657b 6365 7370 6564 6573 3230  ticle{cespedes20
+000059d0: 3232 6672 6f75 726f 732c 0a20 2074 6974  22frouros,.  tit
+000059e0: 6c65 3d7b 4672 6f75 726f 733a 2041 2050  le={Frouros: A P
+000059f0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+00005a00: 7220 6472 6966 7420 6465 7465 6374 696f  r drift detectio
+00005a10: 6e20 696e 206d 6163 6869 6e65 206c 6561  n in machine lea
+00005a20: 726e 696e 6720 7379 7374 656d 737d 2c0a  rning systems},.
+00005a30: 2020 6175 7468 6f72 3d7b 437b 5c27 657d    author={C{\'e}
+00005a40: 7370 6564 6573 2d53 6973 6e69 6567 612c  spedes-Sisniega,
+00005a50: 204a 6169 6d65 2061 6e64 204c 7b5c 276f   Jaime and L{\'o
+00005a60: 7d70 657a 2d47 6172 637b 5c27 5c69 7d61  }pez-Garc{\'\i}a
+00005a70: 2c20 7b5c 2741 7d6c 7661 726f 207d 2c0a  , {\'A}lvaro },.
+00005a80: 2020 6a6f 7572 6e61 6c3d 7b61 7258 6976    journal={arXiv
+00005a90: 2070 7265 7072 696e 7420 6172 5869 763a   preprint arXiv:
+00005aa0: 3232 3038 2e30 3638 3638 7d2c 0a20 2079  2208.06868},.  y
+00005ab0: 6561 723d 7b32 3032 327d 0a7d 0a60 6060  ear={2022}.}.```
+00005ac0: 0a0a 2323 20f0 9f93 9d20 4c69 6365 6e73  ..## .... Licens
+00005ad0: 650a 0a46 726f 7572 6f73 2069 7320 616e  e..Frouros is an
+00005ae0: 206f 7065 6e2d 736f 7572 6365 2073 6f66   open-source sof
+00005af0: 7477 6172 6520 6c69 6365 6e73 6564 2075  tware licensed u
+00005b00: 6e64 6572 2074 6865 205b 4253 442d 332d  nder the [BSD-3-
+00005b10: 436c 6175 7365 206c 6963 656e 7365 5d28  Clause license](
+00005b20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00005b30: 6f6d 2f49 4643 412f 6672 6f75 726f 732f  om/IFCA/frouros/
+00005b40: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00005b50: 4529 2e0a 0a23 2320 f09f 998f 2041 636b  E)...## .... Ack
+00005b60: 6e6f 776c 6564 6765 6d65 6e74 730a 0a46  nowledgements..F
+00005b70: 726f 7572 6f73 2068 6173 2072 6563 6569  rouros has recei
+00005b80: 7665 6420 6675 6e64 696e 6720 6672 6f6d  ved funding from
+00005b90: 2074 6865 2041 6765 6e63 6961 2045 7374   the Agencia Est
+00005ba0: 6174 616c 2064 6520 496e 7665 7374 6967  atal de Investig
+00005bb0: 6163 69c3 b36e 2c20 556e 6964 6164 2064  aci..n, Unidad d
+00005bc0: 6520 4578 6365 6c65 6e63 6961 204d 6172  e Excelencia Mar
+00005bd0: c3ad 6120 6465 204d 6165 7a74 752c 2072  ..a de Maeztu, r
+00005be0: 6566 2e20 4d44 4d2d 3230 3137 2d30 3736  ef. MDM-2017-076
+00005bf0: 352e 0a                                  5..
```

### Comparing `frouros-0.5.1/README.md` & `frouros-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,1093 +1,1093 @@
-00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a20 203c 696d 6720 6865 6967 6874  ">.  <img height
-00000020: 3d22 3131 3570 7822 2073 7263 3d22 6874  ="115px" src="ht
-00000030: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000040: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000050: 4946 4341 2f66 726f 7572 6f73 2f6d 6169  IFCA/frouros/mai
-00000060: 6e2f 696d 6167 6573 2f6c 6f67 6f2e 706e  n/images/logo.pn
-00000070: 6722 2061 6c74 3d22 6c6f 676f 223e 0a3c  g" alt="logo">.<
-00000080: 2f70 3e0a 0a2d 2d2d 0a0a 3c70 2061 6c69  /p>..---..<p ali
-00000090: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
-000000a0: 212d 2d20 4349 202d 2d3e 0a20 203c 6120  !-- CI -->.  <a 
-000000b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000000c0: 7468 7562 2e63 6f6d 2f49 4643 412f 6672  thub.com/IFCA/fr
-000000d0: 6f75 726f 732f 6163 7469 6f6e 732f 776f  ouros/actions/wo
-000000e0: 726b 666c 6f77 732f 6369 2e79 6d6c 223e  rkflows/ci.yml">
-000000f0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000110: 6d2f 4946 4341 2f66 726f 7572 6f73 2f61  m/IFCA/frouros/a
-00000120: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000130: 2f63 692e 796d 6c2f 6261 6467 652e 7376  /ci.yml/badge.sv
-00000140: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
-00000150: 6172 6522 2061 6c74 3d22 6369 222f 3e0a  are" alt="ci"/>.
-00000160: 2020 3c2f 613e 0a20 203c 212d 2d20 436f    </a>.  <!-- Co
-00000170: 6465 2063 6f76 6572 6167 6520 2d2d 3e0a  de coverage -->.
-00000180: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000190: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-000001a0: 2f49 4643 412f 6672 6f75 726f 7322 3e0a  /IFCA/frouros">.
-000001b0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000001c0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-000001d0: 2f67 682f 4946 4341 2f66 726f 7572 6f73  /gh/IFCA/frouros
-000001e0: 2f62 7261 6e63 682f 6d61 696e 2f67 7261  /branch/main/gra
-000001f0: 7068 2f62 6164 6765 2e73 7667 3f74 6f6b  ph/badge.svg?tok
-00000200: 656e 3d44 4c4b 5153 5759 5459 4d22 2061  en=DLKQSWYTYM" a
-00000210: 6c74 3d22 636f 7665 7261 6765 222f 3e0a  lt="coverage"/>.
-00000220: 2020 3c2f 613e 0a20 203c 212d 2d20 446f    </a>.  <!-- Do
-00000230: 6375 6d65 6e74 6174 696f 6e20 2d2d 3e0a  cumentation -->.
-00000240: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000250: 3a2f 2f66 726f 7572 6f73 2e72 6561 6474  ://frouros.readt
-00000260: 6865 646f 6373 2e69 6f2f 223e 0a20 2020  hedocs.io/">.   
-00000270: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000280: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
-00000290: 7267 2f70 726f 6a65 6374 732f 6672 6f75  rg/projects/frou
-000002a0: 726f 732f 6261 6467 652f 3f76 6572 7369  ros/badge/?versi
-000002b0: 6f6e 3d6c 6174 6573 7422 2061 6c74 3d22  on=latest" alt="
-000002c0: 646f 6375 6d65 6e74 6174 696f 6e22 2f3e  documentation"/>
-000002d0: 0a20 203c 2f61 3e0a 2020 3c21 2d2d 2044  .  </a>.  <!-- D
-000002e0: 6f77 6e6c 6f61 6473 202d 2d3e 0a20 203c  ownloads -->.  <
-000002f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000300: 7065 7079 2e74 6563 682f 7072 6f6a 6563  pepy.tech/projec
-00000310: 742f 6672 6f75 726f 7322 3e0a 2020 2020  t/frouros">.    
-00000320: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000330: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
-00000340: 6368 2f62 6164 6765 2f66 726f 7572 6f73  ch/badge/frouros
-00000350: 2220 616c 743d 2264 6f77 6e6c 6f61 6473  " alt="downloads
-00000360: 222f 3e0a 2020 3c2f 613e 0a20 203c 212d  "/>.  </a>.  <!-
-00000370: 2d20 5079 5049 202d 2d3e 0a20 203c 6120  - PyPI -->.  <a 
-00000380: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000390: 7069 2e6f 7267 2f70 726f 6a65 6374 2f66  pi.org/project/f
-000003a0: 726f 7572 6f73 223e 0a20 2020 203c 696d  rouros">.    <im
-000003b0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-000003c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000003d0: 7069 2f76 2f66 726f 7572 6f73 2e73 7667  pi/v/frouros.svg
-000003e0: 3f6c 6162 656c 3d72 656c 6561 7365 2663  ?label=release&c
-000003f0: 6f6c 6f72 3d62 6c75 6522 2061 6c74 3d22  olor=blue" alt="
-00000400: 7079 7069 223e 0a20 203c 2f61 3e0a 2020  pypi">.  </a>.  
-00000410: 3c21 2d2d 2050 7974 686f 6e20 2d2d 3e0a  <!-- Python -->.
-00000420: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000430: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000440: 6563 742f 6672 6f75 726f 7322 3e0a 2020  ect/frouros">.  
-00000450: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000460: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000470: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
-00000480: 6e73 2f66 726f 7572 6f73 2220 616c 743d  ns/frouros" alt=
-00000490: 2270 7974 686f 6e22 3e0a 2020 3c2f 613e  "python">.  </a>
-000004a0: 0a20 203c 212d 2d20 4c69 6365 6e73 6520  .  <!-- License 
-000004b0: 2d2d 3e0a 2020 3c61 2068 7265 663d 2268  -->.  <a href="h
-000004c0: 7474 7073 3a2f 2f6f 7065 6e73 6f75 7263  ttps://opensourc
-000004d0: 652e 6f72 672f 6c69 6365 6e73 6573 2f42  e.org/licenses/B
-000004e0: 5344 2d33 2d43 6c61 7573 6522 3e0a 2020  SD-3-Clause">.  
-000004f0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000500: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000510: 696f 2f62 6164 6765 2f6c 6963 656e 7365  io/badge/license
-00000520: 2d42 5344 2532 3033 2d2d 436c 6175 7365  -BSD%203--Clause
-00000530: 2d62 6c75 652e 7376 6722 2061 6c74 3d22  -blue.svg" alt="
-00000540: 6273 645f 335f 6c69 6365 6e73 6522 3e0a  bsd_3_license">.
-00000550: 2020 3c2f 613e 0a20 203c 212d 2d20 6172    </a>.  <!-- ar
-00000560: 5869 7620 2d2d 3e0a 2020 3c61 2068 7265  Xiv -->.  <a hre
-00000570: 663d 2268 7474 7073 3a2f 2f61 7278 6976  f="https://arxiv
-00000580: 2e6f 7267 2f61 6273 2f32 3230 382e 3036  .org/abs/2208.06
-00000590: 3836 3822 3e0a 2020 2020 3c69 6d67 2073  868">.    <img s
-000005a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000005b0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-000005c0: 2f61 7258 6976 2d32 3230 382e 3036 3836  /arXiv-2208.0686
-000005d0: 382d 626c 7565 2e73 7667 2220 616c 743d  8-blue.svg" alt=
-000005e0: 2261 7278 6976 223e 0a20 203c 2f61 3e0a  "arxiv">.  </a>.
-000005f0: 3c2f 703e 0a0a 4672 6f75 726f 7320 6973  </p>..Frouros is
-00000600: 2061 2050 7974 686f 6e20 6c69 6272 6172   a Python librar
-00000610: 7920 666f 7220 6472 6966 7420 6465 7465  y for drift dete
-00000620: 6374 696f 6e20 696e 206d 6163 6869 6e65  ction in machine
-00000630: 206c 6561 726e 696e 6720 7379 7374 656d   learning system
-00000640: 7320 7468 6174 2070 726f 7669 6465 7320  s that provides 
-00000650: 6120 636f 6d62 696e 6174 696f 6e20 6f66  a combination of
-00000660: 2063 6c61 7373 6963 616c 2061 6e64 206d   classical and m
-00000670: 6f72 6520 7265 6365 6e74 2061 6c67 6f72  ore recent algor
-00000680: 6974 686d 7320 666f 7220 626f 7468 2063  ithms for both c
-00000690: 6f6e 6365 7074 2061 6e64 2064 6174 6120  oncept and data 
-000006a0: 6472 6966 7420 6465 7465 6374 696f 6e2e  drift detection.
-000006b0: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-000006c0: 6572 223e 0a20 2020 203c 693e 0a20 2020  er">.    <i>.   
-000006d0: 2020 2020 2022 4576 6572 7974 6869 6e67       "Everything
-000006e0: 2063 6861 6e67 6573 2061 6e64 206e 6f74   changes and not
-000006f0: 6869 6e67 2073 7461 6e64 7320 7374 696c  hing stands stil
-00000700: 6c22 0a20 2020 203c 2f69 3e0a 3c2f 703e  l".    </i>.</p>
-00000710: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00000720: 7222 3e0a 2020 2020 3c69 3e0a 2020 2020  r">.    <i>.    
-00000730: 2020 2020 2259 6f75 2063 6f75 6c64 206e      "You could n
-00000740: 6f74 2073 7465 7020 7477 6963 6520 696e  ot step twice in
-00000750: 746f 2074 6865 2073 616d 6520 7269 7665  to the same rive
-00000760: 7222 0a20 2020 203c 2f69 3e0a 3c2f 703e  r".    </i>.</p>
-00000770: 0a3c 6469 7620 616c 6967 6e3d 2263 656e  .<div align="cen
-00000780: 7465 7222 2073 7479 6c65 3d22 7769 6474  ter" style="widt
-00000790: 683a 2037 3025 3b22 3e0a 2020 2020 3c70  h: 70%;">.    <p
-000007a0: 2061 6c69 676e 3d22 7269 6768 7422 3e0a   align="right">.
-000007b0: 2020 2020 2020 2020 3c69 3e0a 2020 2020          <i>.    
-000007c0: 2020 2020 2020 2020 4865 7261 636c 6974          Heraclit
-000007d0: 7573 206f 6620 4570 6865 7375 7320 2835  us of Ephesus (5
-000007e0: 3335 2d34 3735 2042 4345 2e29 0a20 2020  35-475 BCE.).   
-000007f0: 2020 2020 203c 2f69 3e0a 2020 2020 3c2f       </i>.    </
-00000800: 703e 0a3c 2f64 6976 3e0a 0a2d 2d2d 2d0a  p>.</div>..----.
-00000810: 0a23 2320 e29a a1ef b88f 2051 7569 636b  .## ...... Quick
-00000820: 7374 6172 740a 0a23 2323 2043 6f6e 6365  start..### Conce
-00000830: 7074 2064 7269 6674 0a0a 4173 2061 2071  pt drift..As a q
-00000840: 7569 636b 2065 7861 6d70 6c65 2c20 7765  uick example, we
-00000850: 2063 616e 2075 7365 2074 6865 2077 696e   can use the win
-00000860: 6520 6461 7461 7365 7420 746f 2077 6869  e dataset to whi
-00000870: 6368 2063 6f6e 6365 7074 2064 7269 6674  ch concept drift
-00000880: 2069 7420 6973 2069 6e64 7563 6564 2069   it is induced i
-00000890: 6e20 6f72 6465 7220 746f 2073 686f 7720  n order to show 
-000008a0: 7468 6520 7573 6520 6f66 2061 2063 6f6e  the use of a con
-000008b0: 6365 7074 2064 7269 6674 2064 6574 6563  cept drift detec
-000008c0: 746f 7220 6c69 6b65 2044 444d 2028 4472  tor like DDM (Dr
-000008d0: 6966 7420 4465 7465 6374 696f 6e20 4d65  ift Detection Me
-000008e0: 7468 6f64 292e 0a0a 6060 6070 7974 686f  thod)...```pytho
-000008f0: 6e0a 696d 706f 7274 206e 756d 7079 2061  n.import numpy a
-00000900: 7320 6e70 0a66 726f 6d20 736b 6c65 6172  s np.from sklear
-00000910: 6e2e 6461 7461 7365 7473 2069 6d70 6f72  n.datasets impor
-00000920: 7420 6c6f 6164 5f77 696e 650a 6672 6f6d  t load_wine.from
-00000930: 2073 6b6c 6561 726e 2e6c 696e 6561 725f   sklearn.linear_
-00000940: 6d6f 6465 6c20 696d 706f 7274 204c 6f67  model import Log
-00000950: 6973 7469 6352 6567 7265 7373 696f 6e0a  isticRegression.
-00000960: 6672 6f6d 2073 6b6c 6561 726e 2e6d 6f64  from sklearn.mod
-00000970: 656c 5f73 656c 6563 7469 6f6e 2069 6d70  el_selection imp
-00000980: 6f72 7420 7472 6169 6e5f 7465 7374 5f73  ort train_test_s
-00000990: 706c 6974 0a66 726f 6d20 736b 6c65 6172  plit.from sklear
-000009a0: 6e2e 7069 7065 6c69 6e65 2069 6d70 6f72  n.pipeline impor
-000009b0: 7420 5069 7065 6c69 6e65 0a66 726f 6d20  t Pipeline.from 
-000009c0: 736b 6c65 6172 6e2e 7072 6570 726f 6365  sklearn.preproce
-000009d0: 7373 696e 6720 696d 706f 7274 2053 7461  ssing import Sta
-000009e0: 6e64 6172 6453 6361 6c65 720a 0a66 726f  ndardScaler..fro
-000009f0: 6d20 6672 6f75 726f 732e 6465 7465 6374  m frouros.detect
-00000a00: 6f72 732e 636f 6e63 6570 745f 6472 6966  ors.concept_drif
-00000a10: 7420 696d 706f 7274 2044 444d 2c20 4444  t import DDM, DD
-00000a20: 4d43 6f6e 6669 670a 0a6e 702e 7261 6e64  MConfig..np.rand
-00000a30: 6f6d 2e73 6565 6428 7365 6564 3d33 3129  om.seed(seed=31)
-00000a40: 0a0a 2320 4c6f 6164 2077 696e 6520 6461  ..# Load wine da
-00000a50: 7461 7365 740a 582c 2079 203d 206c 6f61  taset.X, y = loa
-00000a60: 645f 7769 6e65 2872 6574 7572 6e5f 585f  d_wine(return_X_
-00000a70: 793d 5472 7565 290a 0a23 2053 706c 6974  y=True)..# Split
-00000a80: 2074 7261 696e 2028 3730 2529 2061 6e64   train (70%) and
-00000a90: 2074 6573 7420 2833 3025 290a 280a 2020   test (30%).(.  
-00000aa0: 2020 585f 7472 6169 6e2c 0a20 2020 2058    X_train,.    X
-00000ab0: 5f74 6573 742c 0a20 2020 2079 5f74 7261  _test,.    y_tra
-00000ac0: 696e 2c0a 2020 2020 795f 7465 7374 2c0a  in,.    y_test,.
-00000ad0: 2920 3d20 7472 6169 6e5f 7465 7374 5f73  ) = train_test_s
-00000ae0: 706c 6974 2858 2c20 792c 2074 7261 696e  plit(X, y, train
-00000af0: 5f73 697a 653d 302e 372c 2072 616e 646f  _size=0.7, rando
-00000b00: 6d5f 7374 6174 653d 3331 290a 0a23 2049  m_state=31)..# I
-00000b10: 4d50 4f52 5441 4e54 3a20 496e 6475 6365  MPORTANT: Induce
-00000b20: 2f73 696d 756c 6174 6520 636f 6e63 6570  /simulate concep
-00000b30: 7420 6472 6966 7420 696e 2074 6865 206c  t drift in the l
-00000b40: 6173 7420 7061 7274 2028 3230 2529 0a23  ast part (20%).#
-00000b50: 206f 6620 795f 7465 7374 2062 7920 6d6f   of y_test by mo
-00000b60: 6469 6679 696e 6720 736f 6d65 206c 6162  difying some lab
-00000b70: 656c 7320 2835 3025 2061 7070 726f 7829  els (50% approx)
-00000b80: 2e20 5468 6572 6566 6f72 652c 2063 6861  . Therefore, cha
-00000b90: 6e67 696e 6720 5028 797c 5829 290a 6472  nging P(y|X)).dr
-00000ba0: 6966 745f 7369 7a65 203d 2069 6e74 2879  ift_size = int(y
-00000bb0: 5f74 6573 742e 7368 6170 655b 305d 202a  _test.shape[0] *
-00000bc0: 2030 2e32 290a 795f 7465 7374 5f64 7269   0.2).y_test_dri
-00000bd0: 6674 203d 2079 5f74 6573 745b 2d64 7269  ft = y_test[-dri
-00000be0: 6674 5f73 697a 653a 5d0a 6d6f 6469 6679  ft_size:].modify
-00000bf0: 5f69 6478 203d 206e 702e 7261 6e64 6f6d  _idx = np.random
-00000c00: 2e72 616e 6428 2a79 5f74 6573 745f 6472  .rand(*y_test_dr
-00000c10: 6966 742e 7368 6170 6529 203c 3d20 302e  ift.shape) <= 0.
-00000c20: 350a 795f 7465 7374 5f64 7269 6674 5b6d  5.y_test_drift[m
-00000c30: 6f64 6966 795f 6964 785d 203d 2028 795f  odify_idx] = (y_
-00000c40: 7465 7374 5f64 7269 6674 5b6d 6f64 6966  test_drift[modif
-00000c50: 795f 6964 785d 202b 2031 2920 2520 6c65  y_idx] + 1) % le
-00000c60: 6e28 6e70 2e75 6e69 7175 6528 795f 7465  n(np.unique(y_te
-00000c70: 7374 2929 0a79 5f74 6573 745b 2d64 7269  st)).y_test[-dri
-00000c80: 6674 5f73 697a 653a 5d20 3d20 795f 7465  ft_size:] = y_te
-00000c90: 7374 5f64 7269 6674 0a0a 2320 4465 6669  st_drift..# Defi
-00000ca0: 6e65 2061 6e64 2066 6974 206d 6f64 656c  ne and fit model
-00000cb0: 0a70 6970 656c 696e 6520 3d20 5069 7065  .pipeline = Pipe
-00000cc0: 6c69 6e65 280a 2020 2020 5b0a 2020 2020  line(.    [.    
-00000cd0: 2020 2020 2822 7363 616c 6572 222c 2053      ("scaler", S
-00000ce0: 7461 6e64 6172 6453 6361 6c65 7228 2929  tandardScaler())
-00000cf0: 2c0a 2020 2020 2020 2020 2822 6d6f 6465  ,.        ("mode
-00000d00: 6c22 2c20 4c6f 6769 7374 6963 5265 6772  l", LogisticRegr
-00000d10: 6573 7369 6f6e 2829 292c 0a20 2020 205d  ession()),.    ]
-00000d20: 0a29 0a70 6970 656c 696e 652e 6669 7428  .).pipeline.fit(
-00000d30: 583d 585f 7472 6169 6e2c 2079 3d79 5f74  X=X_train, y=y_t
-00000d40: 7261 696e 290a 0a23 2044 6574 6563 746f  rain)..# Detecto
-00000d50: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
-00000d60: 616e 6420 696e 7374 616e 7469 6174 696f  and instantiatio
-00000d70: 6e0a 636f 6e66 6967 203d 2044 444d 436f  n.config = DDMCo
-00000d80: 6e66 6967 2877 6172 6e69 6e67 5f6c 6576  nfig(warning_lev
-00000d90: 656c 3d32 2e30 2c0a 2020 2020 2020 2020  el=2.0,.        
-00000da0: 2020 2020 2020 2020 2020 2064 7269 6674             drift
-00000db0: 5f6c 6576 656c 3d33 2e30 2c0a 2020 2020  _level=3.0,.    
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00000dd0: 696e 5f6e 756d 5f69 6e73 7461 6e63 6573  in_num_instances
-00000de0: 3d33 302c 290a 6465 7465 6374 6f72 203d  =30,).detector =
-00000df0: 2044 444d 2863 6f6e 6669 673d 636f 6e66   DDM(config=conf
-00000e00: 6967 290a 0a23 2053 696d 756c 6174 6520  ig)..# Simulate 
-00000e10: 6461 7461 2073 7472 6561 6d20 2861 7373  data stream (ass
-00000e20: 756d 696e 6720 7465 7374 206c 6162 656c  uming test label
-00000e30: 2061 7661 696c 6162 6c65 2061 6674 6572   available after
-00000e40: 2070 7265 6469 6374 696f 6e29 0a66 6f72   prediction).for
-00000e50: 2069 2c20 2858 2c20 7929 2069 6e20 656e   i, (X, y) in en
-00000e60: 756d 6572 6174 6528 7a69 7028 585f 7465  umerate(zip(X_te
-00000e70: 7374 2c20 795f 7465 7374 2929 3a0a 2020  st, y_test)):.  
-00000e80: 2020 795f 7072 6564 203d 2070 6970 656c    y_pred = pipel
-00000e90: 696e 652e 7072 6564 6963 7428 582e 7265  ine.predict(X.re
-00000ea0: 7368 6170 6528 312c 202d 3129 290a 2020  shape(1, -1)).  
-00000eb0: 2020 6572 726f 7220 3d20 3120 2d20 696e    error = 1 - in
-00000ec0: 7428 795f 7072 6564 203d 3d20 7929 0a20  t(y_pred == y). 
-00000ed0: 2020 2064 6574 6563 746f 722e 7570 6461     detector.upda
-00000ee0: 7465 2876 616c 7565 3d65 7272 6f72 290a  te(value=error).
-00000ef0: 2020 2020 7374 6174 7573 203d 2064 6574      status = det
-00000f00: 6563 746f 722e 7374 6174 7573 0a20 2020  ector.status.   
-00000f10: 2069 6620 7374 6174 7573 5b22 6472 6966   if status["drif
-00000f20: 7422 5d3a 0a20 2020 2020 2020 2070 7269  t"]:.        pri
-00000f30: 6e74 2866 2244 7269 6674 2064 6574 6563  nt(f"Drift detec
-00000f40: 7465 6420 6174 2069 6e64 6578 207b 697d  ted at index {i}
-00000f50: 2229 0a20 2020 2020 2020 2062 7265 616b  ").        break
-00000f60: 0a0a 3e3e 2044 7269 6674 2064 6574 6563  ..>> Drift detec
-00000f70: 7465 6420 6174 2069 6e64 6578 2034 340a  ted at index 44.
-00000f80: 6060 600a 0a4d 6f72 6520 636f 6e63 6570  ```..More concep
-00000f90: 7420 6472 6966 7420 6578 616d 706c 6573  t drift examples
-00000fa0: 2063 616e 2062 6520 666f 756e 6420 5b68   can be found [h
-00000fb0: 6572 655d 2868 7474 7073 3a2f 2f66 726f  ere](https://fro
-00000fc0: 7572 6f73 2e72 6561 6474 6865 646f 6373  uros.readthedocs
-00000fd0: 2e69 6f2f 656e 2f6c 6174 6573 742f 6578  .io/en/latest/ex
-00000fe0: 616d 706c 6573 2e68 746d 6c23 6461 7461  amples.html#data
-00000ff0: 2d64 7269 6674 292e 0a0a 2323 2320 4461  -drift)...### Da
-00001000: 7461 2064 7269 6674 0a0a 4173 2061 2071  ta drift..As a q
-00001010: 7569 636b 2065 7861 6d70 6c65 2c20 7765  uick example, we
-00001020: 2063 616e 2075 7365 2074 6865 2069 7269   can use the iri
-00001030: 7320 6461 7461 7365 7420 746f 2077 6869  s dataset to whi
-00001040: 6368 2064 6174 6120 6472 6966 7420 696e  ch data drift in
-00001050: 206f 7264 6572 2074 6f20 7368 6f77 2074   order to show t
-00001060: 6865 2075 7365 206f 6620 6120 6461 7461  he use of a data
-00001070: 2064 7269 6674 2064 6574 6563 746f 7220   drift detector 
-00001080: 6c69 6b65 204b 6f6c 6d6f 676f 726f 762d  like Kolmogorov-
-00001090: 536d 6972 6e6f 7620 7465 7374 2e0a 0a60  Smirnov test...`
-000010a0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-000010b0: 6e75 6d70 7920 6173 206e 700a 6672 6f6d  numpy as np.from
-000010c0: 2073 6b6c 6561 726e 2e64 6174 6173 6574   sklearn.dataset
-000010d0: 7320 696d 706f 7274 206c 6f61 645f 6972  s import load_ir
-000010e0: 6973 0a66 726f 6d20 736b 6c65 6172 6e2e  is.from sklearn.
-000010f0: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e20  model_selection 
-00001100: 696d 706f 7274 2074 7261 696e 5f74 6573  import train_tes
-00001110: 745f 7370 6c69 740a 6672 6f6d 2073 6b6c  t_split.from skl
-00001120: 6561 726e 2e74 7265 6520 696d 706f 7274  earn.tree import
-00001130: 2044 6563 6973 696f 6e54 7265 6543 6c61   DecisionTreeCla
-00001140: 7373 6966 6965 720a 0a66 726f 6d20 6672  ssifier..from fr
-00001150: 6f75 726f 732e 6465 7465 6374 6f72 732e  ouros.detectors.
-00001160: 6461 7461 5f64 7269 6674 2069 6d70 6f72  data_drift impor
-00001170: 7420 4b53 5465 7374 0a0a 6e70 2e72 616e  t KSTest..np.ran
-00001180: 646f 6d2e 7365 6564 2873 6565 643d 3331  dom.seed(seed=31
-00001190: 290a 0a23 204c 6f61 6420 6972 6973 2064  )..# Load iris d
-000011a0: 6174 6173 6574 0a58 2c20 7920 3d20 6c6f  ataset.X, y = lo
-000011b0: 6164 5f69 7269 7328 7265 7475 726e 5f58  ad_iris(return_X
-000011c0: 5f79 3d54 7275 6529 0a0a 2320 5370 6c69  _y=True)..# Spli
-000011d0: 7420 7472 6169 6e20 2837 3025 2920 616e  t train (70%) an
-000011e0: 6420 7465 7374 2028 3330 2529 0a28 0a20  d test (30%).(. 
-000011f0: 2020 2058 5f74 7261 696e 2c0a 2020 2020     X_train,.    
-00001200: 585f 7465 7374 2c0a 2020 2020 795f 7472  X_test,.    y_tr
-00001210: 6169 6e2c 0a20 2020 2079 5f74 6573 742c  ain,.    y_test,
-00001220: 0a29 203d 2074 7261 696e 5f74 6573 745f  .) = train_test_
-00001230: 7370 6c69 7428 582c 2079 2c20 7472 6169  split(X, y, trai
-00001240: 6e5f 7369 7a65 3d30 2e37 2c20 7261 6e64  n_size=0.7, rand
-00001250: 6f6d 5f73 7461 7465 3d33 3129 0a0a 2320  om_state=31)..# 
-00001260: 5365 7420 7468 6520 6665 6174 7572 6520  Set the feature 
-00001270: 696e 6465 7820 746f 2077 6869 6368 2064  index to which d
-00001280: 6574 6563 746f 7220 6973 2061 7070 6c69  etector is appli
-00001290: 6564 0a64 696d 5f69 6478 203d 2030 0a0a  ed.dim_idx = 0..
-000012a0: 2320 494d 504f 5254 414e 543a 2049 6e64  # IMPORTANT: Ind
-000012b0: 7563 652f 7369 6d75 6c61 7465 2064 6174  uce/simulate dat
-000012c0: 6120 6472 6966 7420 696e 2074 6865 2073  a drift in the s
-000012d0: 656c 6563 7465 6420 6665 6174 7572 6520  elected feature 
-000012e0: 6f66 2079 5f74 6573 7420 6279 0a23 2061  of y_test by.# a
-000012f0: 7070 6c79 696e 6720 736f 6d65 2067 6175  pplying some gau
-00001300: 7373 6961 6e20 6e6f 6973 652e 2054 6865  ssian noise. The
-00001310: 7265 666f 7265 2c20 6368 616e 6769 6e67  refore, changing
-00001320: 2050 2858 2929 0a58 5f74 6573 745b 3a2c   P(X)).X_test[:,
-00001330: 2064 696d 5f69 6478 5d20 2b3d 206e 702e   dim_idx] += np.
-00001340: 7261 6e64 6f6d 2e6e 6f72 6d61 6c28 0a20  random.normal(. 
-00001350: 2020 206c 6f63 3d30 2e30 2c0a 2020 2020     loc=0.0,.    
-00001360: 7363 616c 653d 332e 302c 0a20 2020 2073  scale=3.0,.    s
-00001370: 697a 653d 585f 7465 7374 2e73 6861 7065  ize=X_test.shape
-00001380: 5b30 5d2c 0a29 0a0a 2320 4465 6669 6e65  [0],.)..# Define
-00001390: 2061 6e64 2066 6974 206d 6f64 656c 0a6d   and fit model.m
-000013a0: 6f64 656c 203d 2044 6563 6973 696f 6e54  odel = DecisionT
-000013b0: 7265 6543 6c61 7373 6966 6965 7228 7261  reeClassifier(ra
-000013c0: 6e64 6f6d 5f73 7461 7465 3d33 3129 0a6d  ndom_state=31).m
-000013d0: 6f64 656c 2e66 6974 2858 3d58 5f74 7261  odel.fit(X=X_tra
-000013e0: 696e 2c20 793d 795f 7472 6169 6e29 0a0a  in, y=y_train)..
-000013f0: 2320 5365 7420 7369 676e 6966 6963 616e  # Set significan
-00001400: 6365 206c 6576 656c 2066 6f72 2068 7970  ce level for hyp
-00001410: 6f74 6865 7369 7320 7465 7374 696e 670a  othesis testing.
-00001420: 616c 7068 6120 3d20 302e 3030 310a 2320  alpha = 0.001.# 
-00001430: 4465 6669 6e65 2061 6e64 2066 6974 2064  Define and fit d
-00001440: 6574 6563 746f 720a 6465 7465 6374 6f72  etector.detector
-00001450: 203d 204b 5354 6573 7428 290a 6465 7465   = KSTest().dete
-00001460: 6374 6f72 2e66 6974 2858 3d58 5f74 7261  ctor.fit(X=X_tra
-00001470: 696e 5b3a 2c20 6469 6d5f 6964 785d 290a  in[:, dim_idx]).
-00001480: 0a23 2041 7070 6c79 2064 6574 6563 746f  .# Apply detecto
-00001490: 7220 746f 2074 6865 2073 656c 6563 7465  r to the selecte
-000014a0: 6420 6665 6174 7572 6520 6f66 2058 5f74  d feature of X_t
-000014b0: 6573 740a 7265 7375 6c74 203d 2064 6574  est.result = det
-000014c0: 6563 746f 722e 636f 6d70 6172 6528 583d  ector.compare(X=
-000014d0: 585f 7465 7374 5b3a 2c20 6469 6d5f 6964  X_test[:, dim_id
-000014e0: 785d 290a 0a23 2043 6865 636b 2069 6620  x])..# Check if 
-000014f0: 6472 6966 7420 6973 2074 616b 696e 6720  drift is taking 
-00001500: 706c 6163 650a 7265 7375 6c74 5b30 5d2e  place.result[0].
-00001510: 705f 7661 6c75 6520 3c20 616c 7068 610a  p_value < alpha.
-00001520: 3e3e 2054 7275 6520 2320 4461 7461 2064  >> True # Data d
-00001530: 7269 6674 2064 6574 6563 7465 642e 0a23  rift detected..#
-00001540: 2054 6865 7265 666f 7265 2c20 7765 2063   Therefore, we c
-00001550: 616e 2072 656a 6563 7420 4830 2028 626f  an reject H0 (bo
-00001560: 7468 2073 616d 706c 6573 2063 6f6d 6520  th samples come 
-00001570: 6672 6f6d 2074 6865 2073 616d 6520 6469  from the same di
-00001580: 7374 7269 6275 7469 6f6e 292e 0a60 6060  stribution)..```
-00001590: 0a0a 4d6f 7265 2064 6174 6120 6472 6966  ..More data drif
-000015a0: 7420 6578 616d 706c 6573 2063 616e 2062  t examples can b
-000015b0: 6520 666f 756e 6420 5b68 6572 655d 2868  e found [here](h
-000015c0: 7474 7073 3a2f 2f66 726f 7572 6f73 2e72  ttps://frouros.r
-000015d0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000015e0: 2f6c 6174 6573 742f 6578 616d 706c 6573  /latest/examples
-000015f0: 2e68 746d 6c23 6461 7461 2d64 7269 6674  .html#data-drift
-00001600: 292e 0a0a 2323 20f0 9f9b a020 496e 7374  )...## .... Inst
-00001610: 616c 6c61 7469 6f6e 0a0a 4672 6f75 726f  allation..Frouro
-00001620: 7320 6361 6e20 6265 2069 6e73 7461 6c6c  s can be install
-00001630: 6564 2076 6961 2070 6970 3a0a 0a60 6060  ed via pip:..```
-00001640: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
-00001650: 2066 726f 7572 6f73 0a60 6060 0a0a 2323   frouros.```..##
-00001660: 20f0 9f95 b5f0 9f8f bbe2 808d e299 82ef   ...............
-00001670: b88f efb8 8f20 4472 6966 7420 6465 7465  ..... Drift dete
-00001680: 6374 696f 6e20 6d65 7468 6f64 730a 0a54  ction methods..T
-00001690: 6865 2063 7572 7265 6e74 6c79 2069 6d70  he currently imp
-000016a0: 6c65 6d65 6e74 6564 2064 6574 6563 746f  lemented detecto
-000016b0: 7273 2061 7265 206c 6973 7465 6420 696e  rs are listed in
-000016c0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2074   the following t
-000016d0: 6162 6c65 2e0a 0a3c 7461 626c 6520 7374  able...<table st
-000016e0: 796c 653d 2277 6964 7468 3a20 3130 3025  yle="width: 100%
-000016f0: 3b20 7465 7874 2d61 6c69 676e 3a20 6365  ; text-align: ce
-00001700: 6e74 6572 3b20 626f 7264 6572 2d63 6f6c  nter; border-col
-00001710: 6c61 7073 653a 2063 6f6c 6c61 7073 653b  lapse: collapse;
-00001720: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00001730: 6964 2067 7265 793b 223e 0a20 203c 7468  id grey;">.  <th
-00001740: 6561 643e 0a20 2020 203c 7472 3e0a 2020  ead>.    <tr>.  
-00001750: 2020 3c74 6820 7374 796c 653d 2274 6578    <th style="tex
-00001760: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00001770: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00001780: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00001790: 3a20 3470 783b 223e 4472 6966 7420 6465  : 4px;">Drift de
-000017a0: 7465 6374 6f72 3c2f 7468 3e0a 2020 2020  tector</th>.    
-000017b0: 3c74 6820 7374 796c 653d 2274 6578 742d  <th style="text-
-000017c0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000017d0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000017e0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-000017f0: 3470 783b 223e 5479 7065 3c2f 7468 3e0a  4px;">Type</th>.
-00001800: 2020 2020 3c74 6820 7374 796c 653d 2274      <th style="t
-00001810: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00001820: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00001830: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00001840: 6e67 3a20 3470 783b 223e 4661 6d69 6c79  ng: 4px;">Family
-00001850: 3c2f 7468 3e0a 2020 2020 3c74 6820 7374  </th>.    <th st
-00001860: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00001870: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00001880: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00001890: 2070 6164 6469 6e67 3a20 3470 783b 223e   padding: 4px;">
-000018a0: 556e 6976 6172 6961 7465 2028 5529 202f  Univariate (U) /
-000018b0: 204d 756c 7469 7661 7269 6174 6520 284d   Multivariate (M
-000018c0: 293c 2f74 683e 0a20 2020 203c 7468 2073  )</th>.    <th s
-000018d0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-000018e0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-000018f0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00001900: 3b20 7061 6464 696e 673a 2034 7078 3b22  ; padding: 4px;"
-00001910: 3e4e 756d 6572 6963 616c 2028 4e29 202f  >Numerical (N) /
-00001920: 2043 6174 6567 6f72 6963 616c 2028 4329   Categorical (C)
-00001930: 3c2f 7468 3e0a 2020 2020 3c74 6820 7374  </th>.    <th st
-00001940: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00001950: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00001960: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00001970: 2070 6164 6469 6e67 3a20 3470 783b 223e   padding: 4px;">
-00001980: 4d65 7468 6f64 3c2f 7468 3e0a 2020 2020  Method</th>.    
-00001990: 3c74 6820 7374 796c 653d 2274 6578 742d  <th style="text-
-000019a0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000019b0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000019c0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-000019d0: 3470 783b 223e 5265 6665 7265 6e63 653c  4px;">Reference<
-000019e0: 2f74 683e 0a20 2020 203c 2f74 723e 0a20  /th>.    </tr>. 
-000019f0: 203c 2f74 6865 6164 3e0a 2020 3c74 626f   </thead>.  <tbo
-00001a00: 6479 3e0a 2020 3c74 723e 0a20 2020 203c  dy>.  <tr>.    <
-00001a10: 7464 2072 6f77 7370 616e 3d22 3133 2220  td rowspan="13" 
-00001a20: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00001a30: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00001a40: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00001a50: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00001a60: 223e 436f 6e63 6570 7420 6472 6966 743c  ">Concept drift<
-00001a70: 2f74 643e 0a20 2020 203c 7464 2072 6f77  /td>.    <td row
-00001a80: 7370 616e 3d22 3133 2220 7374 796c 653d  span="13" style=
-00001a90: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00001aa0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00001ab0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00001ac0: 6469 6e67 3a20 3870 783b 223e 5374 7265  ding: 8px;">Stre
-00001ad0: 616d 696e 673c 2f74 643e 0a20 2020 203c  aming</td>.    <
-00001ae0: 7464 2072 6f77 7370 616e 3d22 3422 2073  td rowspan="4" s
-00001af0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00001b00: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00001b10: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00001b20: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00001b30: 3e43 6861 6e67 6520 6465 7465 6374 696f  >Change detectio
-00001b40: 6e3c 2f74 643e 0a20 2020 203c 7464 2073  n</td>.    <td s
-00001b50: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00001b60: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00001b70: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00001b80: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00001b90: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-00001ba0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00001bb0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00001bc0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00001bd0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00001be0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-00001bf0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00001c00: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00001c10: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00001c20: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00001c30: 3b22 3e42 4f43 443c 2f74 643e 0a20 2020  ;">BOCD</td>.   
-00001c40: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00001c50: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00001c60: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00001c70: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00001c80: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
-00001c90: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
-00001ca0: 3130 2e34 3835 3530 2f61 7258 6976 2e30  10.48550/arXiv.0
-00001cb0: 3731 302e 3337 3432 223e 4164 616d 7320  710.3742">Adams 
-00001cc0: 616e 6420 4d61 634b 6179 2028 3230 3037  and MacKay (2007
-00001cd0: 293c 2f61 3e3c 2f74 643e 0a20 203c 2f74  )</a></td>.  </t
-00001ce0: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
-00001cf0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00001d00: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00001d10: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00001d20: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00001d30: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
-00001d40: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00001d50: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00001d60: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00001d70: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00001d80: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
-00001d90: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00001da0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00001db0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00001dc0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00001dd0: 3870 783b 223e 4355 5355 4d3c 2f74 643e  8px;">CUSUM</td>
-00001de0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00001df0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00001e00: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00001e10: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00001e20: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
-00001e30: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
-00001e40: 6f72 672f 3130 2e32 3330 372f 3233 3333  org/10.2307/2333
-00001e50: 3030 3922 3e50 6167 6520 2831 3935 3429  009">Page (1954)
-00001e60: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
-00001e70: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
-00001e80: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00001e90: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00001ea0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00001eb0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00001ec0: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
-00001ed0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00001ee0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00001ef0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00001f00: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00001f10: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
-00001f20: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00001f30: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00001f40: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00001f50: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00001f60: 7078 3b22 3e47 656f 6d65 7472 6963 206d  px;">Geometric m
-00001f70: 6f76 696e 6720 6176 6572 6167 653c 2f74  oving average</t
-00001f80: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00001f90: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00001fa0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00001fb0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00001fc0: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
-00001fd0: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-00001fe0: 692e 6f72 672f 3130 2e32 3330 372f 3132  i.org/10.2307/12
-00001ff0: 3636 3434 3322 3e52 6f62 6572 7473 2028  66443">Roberts (
-00002000: 3139 3539 293c 2f61 3e3c 2f74 643e 0a20  1959)</a></td>. 
-00002010: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
-00002020: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00002030: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00002040: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00002050: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00002060: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
-00002070: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00002080: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002090: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000020a0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000020b0: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
-000020c0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-000020d0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-000020e0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-000020f0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002100: 6e67 3a20 3870 783b 223e 5061 6765 2048  ng: 8px;">Page H
-00002110: 696e 6b6c 6579 3c2f 7464 3e0a 2020 2020  inkley</td>.    
-00002120: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00002130: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00002140: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002150: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002160: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-00002170: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00002180: 302e 3233 3037 2f32 3333 3330 3039 223e  0.2307/2333009">
-00002190: 5061 6765 2028 3139 3534 293c 2f61 3e3c  Page (1954)</a><
-000021a0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-000021b0: 7472 3e0a 2020 2020 3c74 6420 726f 7773  tr>.    <td rows
-000021c0: 7061 6e3d 2236 2220 7374 796c 653d 2274  pan="6" style="t
-000021d0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-000021e0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-000021f0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002200: 6e67 3a20 3870 783b 223e 5374 6174 6973  ng: 8px;">Statis
-00002210: 7469 6361 6c20 7072 6f63 6573 7320 636f  tical process co
-00002220: 6e74 726f 6c3c 2f74 643e 0a20 2020 203c  ntrol</td>.    <
-00002230: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00002240: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002250: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00002260: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00002270: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
-00002280: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00002290: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000022a0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000022b0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-000022c0: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
-000022d0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-000022e0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-000022f0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00002300: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00002310: 2038 7078 3b22 3e44 444d 3c2f 7464 3e0a   8px;">DDM</td>.
-00002320: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00002330: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00002340: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00002350: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002360: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
-00002370: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
-00002380: 7267 2f31 302e 3130 3037 2f39 3738 2d33  rg/10.1007/978-3
-00002390: 2d35 3430 2d32 3836 3435 2d35 5f32 3922  -540-28645-5_29"
-000023a0: 3e47 616d 6120 6574 2061 6c2e 2028 3230  >Gama et al. (20
-000023b0: 3034 293c 2f61 3e3c 2f74 643e 0a20 203c  04)</a></td>.  <
-000023c0: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
-000023d0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000023e0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000023f0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002400: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002410: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
-00002420: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002430: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00002440: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00002450: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00002460: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
-00002470: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00002480: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00002490: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000024a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000024b0: 3a20 3870 783b 223e 4543 4444 2d57 543c  : 8px;">ECDD-WT<
-000024c0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-000024d0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-000024e0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-000024f0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00002500: 7061 6464 696e 673a 2038 7078 3b22 3e3c  padding: 8px;"><
-00002510: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002520: 646f 692e 6f72 672f 3130 2e31 3031 362f  doi.org/10.1016/
-00002530: 6a2e 7061 7472 6563 2e32 3031 312e 3038  j.patrec.2011.08
-00002540: 2e30 3139 223e 526f 7373 2065 7420 616c  .019">Ross et al
-00002550: 2e20 2832 3031 3229 3c2f 613e 3c2f 7464  . (2012)</a></td
-00002560: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
-00002570: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00002580: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00002590: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-000025a0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-000025b0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
-000025c0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000025d0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000025e0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000025f0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002600: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
-00002610: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002620: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002630: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002640: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002650: 6464 696e 673a 2038 7078 3b22 3e45 4444  dding: 8px;">EDD
-00002660: 4d3c 2f74 643e 0a20 2020 203c 7464 2073  M</td>.    <td s
-00002670: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00002680: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00002690: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-000026a0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-000026b0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-000026c0: 2f2f 7777 772e 7265 7365 6172 6368 6761  //www.researchga
-000026d0: 7465 2e6e 6574 2f70 7562 6c69 6361 7469  te.net/publicati
-000026e0: 6f6e 2f32 3435 3939 3937 3034 5f45 6172  on/245999704_Ear
-000026f0: 6c79 5f44 7269 6674 5f44 6574 6563 7469  ly_Drift_Detecti
-00002700: 6f6e 5f4d 6574 686f 6422 3e42 6165 6e61  on_Method">Baena
-00002710: 2d47 6172 63c4 b161 2065 7420 616c 2e20  -Garc..a et al. 
-00002720: 2832 3030 3629 3c2f 613e 3c2f 7464 3e0a  (2006)</a></td>.
-00002730: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
-00002740: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00002750: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002760: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002770: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002780: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
-00002790: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-000027a0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-000027b0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-000027c0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-000027d0: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
-000027e0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-000027f0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00002800: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00002810: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00002820: 696e 673a 2038 7078 3b22 3e48 4444 4d2d  ing: 8px;">HDDM-
-00002830: 413c 2f74 643e 0a20 2020 203c 7464 2073  A</td>.    <td s
-00002840: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00002850: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00002860: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00002870: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00002880: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00002890: 2f2f 646f 692e 6f72 672f 3130 2e31 3130  //doi.org/10.110
-000028a0: 392f 544b 4445 2e32 3031 342e 3233 3435  9/TKDE.2014.2345
-000028b0: 3338 3222 3e46 7269 6173 2d42 6c61 6e63  382">Frias-Blanc
-000028c0: 6f20 6574 2061 6c2e 2028 3230 3134 293c  o et al. (2014)<
-000028d0: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
-000028e0: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
-000028f0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00002900: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00002910: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00002920: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00002930: 223e 553c 2f74 643e 0a20 2020 203c 7464  ">U</td>.    <td
-00002940: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00002950: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00002960: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00002970: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00002980: 3b22 3e4e 3c2f 7464 3e0a 2020 2020 3c74  ;">N</td>.    <t
-00002990: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000029a0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-000029b0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-000029c0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-000029d0: 783b 223e 4844 444d 2d57 3c2f 7464 3e0a  x;">HDDM-W</td>.
-000029e0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-000029f0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00002a00: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00002a10: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002a20: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
-00002a30: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
-00002a40: 7267 2f31 302e 3131 3039 2f54 4b44 452e  rg/10.1109/TKDE.
-00002a50: 3230 3134 2e32 3334 3533 3832 223e 4672  2014.2345382">Fr
-00002a60: 6961 732d 426c 616e 636f 2065 7420 616c  ias-Blanco et al
-00002a70: 2e20 2832 3031 3429 3c2f 613e 3c2f 7464  . (2014)</a></td
-00002a80: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
-00002a90: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00002aa0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00002ab0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00002ac0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00002ad0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
-00002ae0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00002af0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00002b00: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00002b10: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002b20: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
-00002b30: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002b40: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002b50: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002b60: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002b70: 6464 696e 673a 2038 7078 3b22 3e52 4444  dding: 8px;">RDD
-00002b80: 4d3c 2f74 643e 0a20 2020 203c 7464 2073  M</td>.    <td s
-00002b90: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00002ba0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00002bb0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00002bc0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00002bd0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00002be0: 2f2f 646f 692e 6f72 672f 3130 2e31 3031  //doi.org/10.101
-00002bf0: 362f 6a2e 6573 7761 2e32 3031 372e 3038  6/j.eswa.2017.08
-00002c00: 2e30 3233 223e 4261 7272 6f73 2065 7420  .023">Barros et 
-00002c10: 616c 2e20 2832 3031 3729 3c2f 613e 3c2f  al. (2017)</a></
-00002c20: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
-00002c30: 723e 0a20 2020 203c 7464 2072 6f77 7370  r>.    <td rowsp
-00002c40: 616e 3d22 3322 2073 7479 6c65 3d22 7465  an="3" style="te
-00002c50: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002c60: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002c70: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002c80: 673a 2038 7078 3b22 3e57 696e 646f 7720  g: 8px;">Window 
-00002c90: 6261 7365 643c 2f74 643e 0a20 2020 203c  based</td>.    <
-00002ca0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00002cb0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002cc0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00002cd0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00002ce0: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
-00002cf0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00002d00: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00002d10: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002d20: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002d30: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
-00002d40: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002d50: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00002d60: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00002d70: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00002d80: 2038 7078 3b22 3e41 4457 494e 3c2f 7464   8px;">ADWIN</td
-00002d90: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00002da0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00002db0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00002dc0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002dd0: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
-00002de0: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
-00002df0: 2e6f 7267 2f31 302e 3131 3337 2f31 2e39  .org/10.1137/1.9
-00002e00: 3738 3136 3131 3937 3237 3731 2e34 3222  781611972771.42"
-00002e10: 3e42 6966 6574 2061 6e64 2047 6176 616c  >Bifet and Gaval
-00002e20: 6461 2028 3230 3037 293c 2f61 3e3c 2f74  da (2007)</a></t
-00002e30: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-00002e40: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00002e50: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00002e60: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00002e70: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002e80: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
-00002e90: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002ea0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002eb0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002ec0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002ed0: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
-00002ee0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00002ef0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00002f00: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00002f10: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00002f20: 6164 6469 6e67 3a20 3870 783b 223e 4b53  adding: 8px;">KS
-00002f30: 5749 4e3c 2f74 643e 0a20 2020 203c 7464  WIN</td>.    <td
-00002f40: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00002f50: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00002f60: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00002f70: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00002f80: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
-00002f90: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
-00002fa0: 3031 362f 6a2e 6e65 7563 6f6d 2e32 3031  016/j.neucom.201
-00002fb0: 392e 3131 2e31 3131 223e 5261 6162 2065  9.11.111">Raab e
-00002fc0: 7420 616c 2e20 2832 3032 3029 3c2f 613e  t al. (2020)</a>
-00002fd0: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00002fe0: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
-00002ff0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003000: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003010: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003020: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
-00003030: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003040: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003050: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003060: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003070: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003080: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
-00003090: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-000030a0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-000030b0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-000030c0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-000030d0: 3e53 5445 5044 3c2f 7464 3e0a 2020 2020  >STEPD</td>.    
-000030e0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000030f0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00003100: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00003110: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00003120: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-00003130: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00003140: 302e 3130 3037 2f39 3738 2d33 2d35 3430  0.1007/978-3-540
-00003150: 2d37 3534 3838 2d36 5f32 3722 3e4e 6973  -75488-6_27">Nis
-00003160: 6869 6461 2061 6e64 2059 616d 6175 6368  hida and Yamauch
-00003170: 6920 2832 3030 3729 3c2f 613e 3c2f 7464  i (2007)</a></td
-00003180: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
-00003190: 0a20 2020 203c 7464 2072 6f77 7370 616e  .    <td rowspan
-000031a0: 3d22 3136 2220 7374 796c 653d 2274 6578  ="16" style="tex
-000031b0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-000031c0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000031d0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000031e0: 3a20 3870 783b 223e 4461 7461 2064 7269  : 8px;">Data dri
-000031f0: 6674 3c2f 7464 3e0a 2020 2020 3c74 6420  ft</td>.    <td 
-00003200: 726f 7773 7061 6e3d 2231 3422 2073 7479  rowspan="14" sty
-00003210: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003220: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003230: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003240: 7061 6464 696e 673a 2038 7078 3b22 3e42  padding: 8px;">B
-00003250: 6174 6368 3c2f 7464 3e0a 2020 2020 3c74  atch</td>.    <t
-00003260: 6420 726f 7773 7061 6e3d 2239 2220 7374  d rowspan="9" st
-00003270: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003280: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003290: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000032a0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000032b0: 4469 7374 616e 6365 2062 6173 6564 3c2f  Distance based</
-000032c0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-000032d0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-000032e0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-000032f0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003300: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00003310: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00003320: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003330: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003340: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003350: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00003360: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003370: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003380: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003390: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000033a0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000033b0: 416e 6465 7273 6f6e 2d44 6172 6c69 6e67  Anderson-Darling
-000033c0: 2074 6573 743c 2f74 643e 0a20 2020 203c   test</td>.    <
-000033d0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-000033e0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-000033f0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00003400: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00003410: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
-00003420: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
-00003430: 2e32 3330 372f 3232 3838 3830 3522 3e53  .2307/2288805">S
-00003440: 6368 6f6c 7a20 616e 6420 5374 6570 6865  cholz and Stephe
-00003450: 6e73 2028 3139 3837 293c 2f61 3e3c 2f74  ns (1987)</a></t
-00003460: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-00003470: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00003480: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00003490: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000034a0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000034b0: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
-000034c0: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-000034d0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-000034e0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-000034f0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00003500: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
-00003510: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00003520: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003530: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00003540: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003550: 6164 6469 6e67 3a20 3870 783b 223e 4268  adding: 8px;">Bh
-00003560: 6174 7461 6368 6172 7979 6120 6469 7374  attacharyya dist
-00003570: 616e 6365 3c2f 7464 3e0a 2020 2020 3c74  ance</td>.    <t
-00003580: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00003590: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-000035a0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-000035b0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-000035c0: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
-000035d0: 7073 3a2f 2f77 7777 2e6a 7374 6f72 2e6f  ps://www.jstor.o
-000035e0: 7267 2f73 7461 626c 652f 3235 3034 3738  rg/stable/250478
-000035f0: 3832 223e 4268 6174 7461 6368 6172 7979  82">Bhattacharyy
-00003600: 6120 2831 3934 3629 3c2f 613e 3c2f 7464  a (1946)</a></td
-00003610: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
-00003620: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00003630: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00003640: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00003650: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00003660: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
-00003670: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00003680: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00003690: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000036a0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000036b0: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
-000036c0: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-000036d0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-000036e0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-000036f0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00003700: 6464 696e 673a 2038 7078 3b22 3e45 6172  dding: 8px;">Ear
-00003710: 7468 204d 6f76 6572 2773 2064 6973 7461  th Mover's dista
-00003720: 6e63 653c 2f74 643e 0a20 2020 203c 7464  nce</td>.    <td
-00003730: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00003740: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00003750: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00003760: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00003770: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
-00003780: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
-00003790: 3032 332f 413a 3130 3236 3534 3339 3030  023/A:1026543900
-000037a0: 3035 3422 3e52 7562 6e65 7220 6574 2061  054">Rubner et a
-000037b0: 6c2e 2028 3230 3030 293c 2f61 3e3c 2f74  l. (2000)</a></t
-000037c0: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-000037d0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000037e0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000037f0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00003800: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00003810: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
-00003820: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00003830: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00003840: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00003850: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00003860: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
-00003870: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00003880: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003890: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-000038a0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-000038b0: 6164 6469 6e67 3a20 3870 783b 223e 4865  adding: 8px;">He
-000038c0: 6c6c 696e 6765 7220 6469 7374 616e 6365  llinger distance
-000038d0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-000038e0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000038f0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003900: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003910: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003920: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00003930: 2f64 6f69 2e6f 7267 2f31 302e 3135 3135  /doi.org/10.1515
-00003940: 2f43 524c 4c2e 3139 3039 2e31 3336 2e32  /CRLL.1909.136.2
-00003950: 3130 223e 4865 6c6c 696e 6765 7220 2831  10">Hellinger (1
-00003960: 3930 3929 3c2f 613e 3c2f 7464 3e0a 2020  909)</a></td>.  
-00003970: 3c2f 7472 3e0a 2020 3c74 723e 0a20 2020  </tr>.  <tr>.   
-00003980: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00003990: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-000039a0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-000039b0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-000039c0: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
-000039d0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-000039e0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-000039f0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00003a00: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00003a10: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
-00003a20: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00003a30: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00003a40: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00003a50: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00003a60: 673a 2038 7078 3b22 3e48 6973 746f 6772  g: 8px;">Histogr
-00003a70: 616d 2069 6e74 6572 7365 6374 696f 6e20  am intersection 
-00003a80: 6e6f 726d 616c 697a 6564 2063 6f6d 706c  normalized compl
-00003a90: 656d 656e 743c 2f74 643e 0a20 2020 203c  ement</td>.    <
-00003aa0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00003ab0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00003ac0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00003ad0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00003ae0: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
-00003af0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
-00003b00: 2e31 3030 372f 4246 3030 3133 3034 3837  .1007/BF00130487
-00003b10: 223e 5377 6169 6e20 616e 6420 4261 6c6c  ">Swain and Ball
-00003b20: 6172 6420 2831 3939 3129 3c2f 613e 3c2f  ard (1991)</a></
-00003b30: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
-00003b40: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
-00003b50: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00003b60: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00003b70: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00003b80: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
-00003b90: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00003ba0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003bb0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00003bc0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003bd0: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
-00003be0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00003bf0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003c00: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003c10: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003c20: 7061 6464 696e 673a 2038 7078 3b22 3e4a  padding: 8px;">J
-00003c30: 656e 7365 6e2d 5368 616e 6e6f 6e20 6469  ensen-Shannon di
-00003c40: 7374 616e 6365 3c2f 7464 3e0a 2020 2020  stance</td>.    
-00003c50: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00003c60: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00003c70: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00003c80: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00003c90: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-00003ca0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00003cb0: 302e 3131 3039 2f31 382e 3631 3131 3522  0.1109/18.61115"
-00003cc0: 3e4c 696e 2028 3139 3931 293c 2f61 3e3c  >Lin (1991)</a><
-00003cd0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-00003ce0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-00003cf0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003d00: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00003d10: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003d20: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00003d30: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00003d40: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003d50: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003d60: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003d70: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00003d80: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003d90: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003da0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003db0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003dc0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003dd0: 4b75 6c6c 6261 636b 2d4c 6569 626c 6572  Kullback-Leibler
-00003de0: 2064 6976 6572 6765 6e63 653c 2f74 643e   divergence</td>
-00003df0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00003e00: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00003e10: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00003e20: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00003e30: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
-00003e40: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
-00003e50: 6f72 672f 3130 2e31 3231 342f 616f 6d73  org/10.1214/aoms
-00003e60: 2f31 3137 3737 3239 3639 3422 3e4b 756c  /1177729694">Kul
-00003e70: 6c62 6163 6b20 616e 6420 4c65 6962 6c65  lback and Leible
-00003e80: 7220 2831 3935 3129 3c2f 613e 3c2f 7464  r (1951)</a></td
-00003e90: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
-00003ea0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00003eb0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00003ec0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00003ed0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00003ee0: 696e 673a 2038 7078 3b22 3e4d 3c2f 7464  ing: 8px;">M</td
-00003ef0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00003f00: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00003f10: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00003f20: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00003f30: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
-00003f40: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00003f50: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00003f60: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00003f70: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00003f80: 6464 696e 673a 2038 7078 3b22 3e4d 4d44  dding: 8px;">MMD
-00003f90: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003fa0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003fb0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003fc0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003fd0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003fe0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00003ff0: 2f64 6c2e 6163 6d2e 6f72 672f 646f 692f  /dl.acm.org/doi/
-00004000: 3130 2e35 3535 352f 3231 3838 3338 352e  10.5555/2188385.
-00004010: 3231 3838 3431 3022 3e47 7265 7474 6f6e  2188410">Gretton
-00004020: 2065 7420 616c 2e20 2832 3031 3229 3c2f   et al. (2012)</
-00004030: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
-00004040: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
-00004050: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004060: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004070: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004080: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004090: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-000040a0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-000040b0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-000040c0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-000040d0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-000040e0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-000040f0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004100: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004110: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004120: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004130: 3b22 3e50 5349 3c2f 7464 3e0a 2020 2020  ;">PSI</td>.    
-00004140: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00004150: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00004160: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00004170: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00004180: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-00004190: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-000041a0: 302e 3130 3537 2f6a 6f72 732e 3230 3038  0.1057/jors.2008
-000041b0: 2e31 3434 223e 5775 2061 6e64 204f 6c73  .144">Wu and Ols
-000041c0: 6f6e 2028 3230 3130 293c 2f61 3e3c 2f74  on (2010)</a></t
-000041d0: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-000041e0: 3e0a 2020 2020 3c74 6420 726f 7773 7061  >.    <td rowspa
-000041f0: 6e3d 2235 2220 7374 796c 653d 2274 6578  n="5" style="tex
-00004200: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00004210: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00004220: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00004230: 3a20 3870 783b 223e 5374 6174 6973 7469  : 8px;">Statisti
-00004240: 6361 6c20 7465 7374 3c2f 7464 3e0a 2020  cal test</td>.  
-00004250: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00004260: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00004270: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00004280: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00004290: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
-000042a0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000042b0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000042c0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000042d0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000042e0: 673a 2038 7078 3b22 3e43 3c2f 7464 3e0a  g: 8px;">C</td>.
-000042f0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00004300: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00004310: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004320: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004330: 6e67 3a20 3870 783b 223e 4368 692d 7371  ng: 8px;">Chi-sq
-00004340: 7561 7265 2074 6573 743c 2f74 643e 0a20  uare test</td>. 
-00004350: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00004360: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00004370: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00004380: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00004390: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-000043a0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-000043b0: 672f 3130 2e31 3038 302f 3134 3738 3634  g/10.1080/147864
-000043c0: 3430 3030 3934 3633 3839 3722 3e50 6561  40009463897">Pea
-000043d0: 7273 6f6e 2028 3139 3030 293c 2f61 3e3c  rson (1900)</a><
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6672 6f75  : 2.1.Name: frou
+00000020: 726f 730a 5665 7273 696f 6e3a 2030 2e36  ros.Version: 0.6
+00000030: 2e30 0a53 756d 6d61 7279 3a20 416e 206f  .0.Summary: An o
+00000040: 7065 6e2d 736f 7572 6365 2050 7974 686f  pen-source Pytho
+00000050: 6e20 6c69 6272 6172 7920 666f 7220 6472  n library for dr
+00000060: 6966 7420 6465 7465 6374 696f 6e20 696e  ift detection in
+00000070: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+00000080: 6720 7379 7374 656d 730a 486f 6d65 2d70  g systems.Home-p
+00000090: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
+000000a0: 6875 622e 636f 6d2f 4946 4341 2f66 726f  hub.com/IFCA/fro
+000000b0: 7572 6f73 0a41 7574 686f 723a 204a 6169  uros.Author: Jai
+000000c0: 6d65 2043 c3a9 7370 6564 6573 2053 6973  me C..spedes Sis
+000000d0: 6e69 6567 610a 4175 7468 6f72 2d65 6d61  niega.Author-ema
+000000e0: 696c 3a20 6365 7370 6564 6573 4069 6663  il: cespedes@ifc
+000000f0: 612e 756e 6963 616e 2e65 730a 4d61 696e  a.unican.es.Main
+00000100: 7461 696e 6572 3a20 4a61 696d 6520 43c3  tainer: Jaime C.
+00000110: a973 7065 6465 7320 5369 736e 6965 6761  .spedes Sisniega
+00000120: 0a4d 6169 6e74 6169 6e65 722d 656d 6169  .Maintainer-emai
+00000130: 6c3a 2063 6573 7065 6465 7340 6966 6361  l: cespedes@ifca
+00000140: 2e75 6e69 6361 6e2e 6573 0a4c 6963 656e  .unican.es.Licen
+00000150: 7365 3a20 4253 442d 332d 436c 6175 7365  se: BSD-3-Clause
+00000160: 0a50 726f 6a65 6374 2d55 524c 3a20 686f  .Project-URL: ho
+00000170: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
+00000180: 6672 6f75 726f 732e 7265 6164 7468 6564  frouros.readthed
+00000190: 6f63 732e 696f 0a50 726f 6a65 6374 2d55  ocs.io.Project-U
+000001a0: 524c 3a20 7265 706f 7369 746f 7279 2c20  RL: repository, 
+000001b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000001c0: 6f6d 2f49 4643 412f 6672 6f75 726f 730a  om/IFCA/frouros.
+000001d0: 5072 6f6a 6563 742d 5552 4c3a 2064 6f63  Project-URL: doc
+000001e0: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
+000001f0: 733a 2f2f 6672 6f75 726f 732e 7265 6164  s://frouros.read
+00000200: 7468 6564 6f63 732e 696f 0a50 726f 6a65  thedocs.io.Proje
+00000210: 6374 2d55 524c 3a20 646f 776e 6c6f 6164  ct-URL: download
+00000220: 2c20 6874 7470 733a 2f2f 7079 7069 2e6f  , https://pypi.o
+00000230: 7267 2f70 726f 6a65 6374 2f66 726f 7572  rg/project/frour
+00000240: 6f73 2f0a 4b65 7977 6f72 6473 3a20 6472  os/.Keywords: dr
+00000250: 6966 742d 6465 7465 6374 696f 6e2c 636f  ift-detection,co
+00000260: 6e63 6570 742d 6472 6966 742c 6461 7461  ncept-drift,data
+00000270: 2d64 7269 6674 2c6d 6163 6869 6e65 2d6c  -drift,machine-l
+00000280: 6561 726e 696e 672c 6461 7461 2d73 6369  earning,data-sci
+00000290: 656e 6365 2c6d 6163 6869 6e65 2d6c 6561  ence,machine-lea
+000002a0: 726e 696e 672d 6f70 6572 6174 696f 6e73  rning-operations
+000002b0: 2c6d 6163 6869 6e65 2d6c 6561 726e 696e  ,machine-learnin
+000002c0: 672d 7379 7374 656d 730a 506c 6174 666f  g-systems.Platfo
+000002d0: 726d 3a20 554e 4b4e 4f57 4e0a 436c 6173  rm: UNKNOWN.Clas
+000002e0: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
+000002f0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
+00000300: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
+00000310: 626c 650a 436c 6173 7369 6669 6572 3a20  ble.Classifier: 
+00000320: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000330: 6520 3a3a 2044 6576 656c 6f70 6572 730a  e :: Developers.
+00000340: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000350: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000360: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
+00000370: 680a 436c 6173 7369 6669 6572 3a20 4c69  h.Classifier: Li
+00000380: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000390: 726f 7665 6420 3a3a 2042 5344 204c 6963  roved :: BSD Lic
+000003a0: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+000003b0: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
+000003c0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+000003d0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+000003e0: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
+000003f0: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
+00000400: 4172 7469 6669 6369 616c 2049 6e74 656c  Artificial Intel
+00000410: 6c69 6765 6e63 650a 436c 6173 7369 6669  ligence.Classifi
+00000420: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
+00000430: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000440: 696e 6720 3a3a 204d 6174 6865 6d61 7469  ing :: Mathemati
+00000450: 6373 0a43 6c61 7373 6966 6965 723a 2054  cs.Classifier: T
+00000460: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000470: 2044 6576 656c 6f70 6d65 6e74 0a43 6c61   Development.Cla
+00000480: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
+00000490: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+000004a0: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
+000004b0: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
+000004c0: 6475 6c65 730a 436c 6173 7369 6669 6572  dules.Classifier
+000004d0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000004e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000004f0: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+00000500: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000510: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000520: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
+00000530: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000540: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000550: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
+00000560: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000570: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000580: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
+00000590: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000005a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000005b0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+000005c0: 3a3a 204f 6e6c 790a 5265 7175 6972 6573  :: Only.Requires
+000005d0: 2d50 7974 686f 6e3a 203e 3d33 2e38 2c3c  -Python: >=3.8,<
+000005e0: 332e 3132 0a44 6573 6372 6970 7469 6f6e  3.12.Description
+000005f0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000600: 6578 742f 6d61 726b 646f 776e 0a50 726f  ext/markdown.Pro
+00000610: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
+00000620: 730a 5072 6f76 6964 6573 2d45 7874 7261  s.Provides-Extra
+00000630: 3a20 6e6f 7465 626f 6f6b 730a 4c69 6365  : notebooks.Lice
+00000640: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
+00000650: 450a 0a3c 7020 616c 6967 6e3d 2263 656e  E..<p align="cen
+00000660: 7465 7222 3e0a 2020 3c69 6d67 2068 6569  ter">.  <img hei
+00000670: 6768 743d 2231 3135 7078 2220 7372 633d  ght="115px" src=
+00000680: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000690: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000006a0: 6f6d 2f49 4643 412f 6672 6f75 726f 732f  om/IFCA/frouros/
+000006b0: 6d61 696e 2f69 6d61 6765 732f 6c6f 676f  main/images/logo
+000006c0: 2e70 6e67 2220 616c 743d 226c 6f67 6f22  .png" alt="logo"
+000006d0: 3e0a 3c2f 703e 0a0a 2d2d 2d0a 0a3c 7020  >.</p>..---..<p 
+000006e0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+000006f0: 2020 3c21 2d2d 2043 4920 2d2d 3e0a 2020    <!-- CI -->.  
+00000700: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000710: 2f67 6974 6875 622e 636f 6d2f 4946 4341  /github.com/IFCA
+00000720: 2f66 726f 7572 6f73 2f61 6374 696f 6e73  /frouros/actions
+00000730: 2f77 6f72 6b66 6c6f 7773 2f63 692e 796d  /workflows/ci.ym
+00000740: 6c22 3e0a 2020 2020 3c69 6d67 2073 7263  l">.    <img src
+00000750: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000760: 2e63 6f6d 2f49 4643 412f 6672 6f75 726f  .com/IFCA/frouro
+00000770: 732f 6163 7469 6f6e 732f 776f 726b 666c  s/actions/workfl
+00000780: 6f77 732f 6369 2e79 6d6c 2f62 6164 6765  ows/ci.yml/badge
+00000790: 2e73 7667 3f73 7479 6c65 3d66 6c61 742d  .svg?style=flat-
+000007a0: 7371 7561 7265 2220 616c 743d 2263 6922  square" alt="ci"
+000007b0: 2f3e 0a20 203c 2f61 3e0a 2020 3c21 2d2d  />.  </a>.  <!--
+000007c0: 2043 6f64 6520 636f 7665 7261 6765 202d   Code coverage -
+000007d0: 2d3e 0a20 203c 6120 6872 6566 3d22 6874  ->.  <a href="ht
+000007e0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000007f0: 2f67 682f 4946 4341 2f66 726f 7572 6f73  /gh/IFCA/frouros
+00000800: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000810: 2268 7474 7073 3a2f 2f63 6f64 6563 6f76  "https://codecov
+00000820: 2e69 6f2f 6768 2f49 4643 412f 6672 6f75  .io/gh/IFCA/frou
+00000830: 726f 732f 6272 616e 6368 2f6d 6169 6e2f  ros/branch/main/
+00000840: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00000850: 746f 6b65 6e3d 444c 4b51 5357 5954 594d  token=DLKQSWYTYM
+00000860: 2220 616c 743d 2263 6f76 6572 6167 6522  " alt="coverage"
+00000870: 2f3e 0a20 203c 2f61 3e0a 2020 3c21 2d2d  />.  </a>.  <!--
+00000880: 2044 6f63 756d 656e 7461 7469 6f6e 202d   Documentation -
+00000890: 2d3e 0a20 203c 6120 6872 6566 3d22 6874  ->.  <a href="ht
+000008a0: 7470 733a 2f2f 6672 6f75 726f 732e 7265  tps://frouros.re
+000008b0: 6164 7468 6564 6f63 732e 696f 2f22 3e0a  adthedocs.io/">.
+000008c0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000008d0: 7470 733a 2f2f 7265 6164 7468 6564 6f63  tps://readthedoc
+000008e0: 732e 6f72 672f 7072 6f6a 6563 7473 2f66  s.org/projects/f
+000008f0: 726f 7572 6f73 2f62 6164 6765 2f3f 7665  rouros/badge/?ve
+00000900: 7273 696f 6e3d 6c61 7465 7374 2220 616c  rsion=latest" al
+00000910: 743d 2264 6f63 756d 656e 7461 7469 6f6e  t="documentation
+00000920: 222f 3e0a 2020 3c2f 613e 0a20 203c 212d  "/>.  </a>.  <!-
+00000930: 2d20 446f 776e 6c6f 6164 7320 2d2d 3e0a  - Downloads -->.
+00000940: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000950: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
+00000960: 6a65 6374 2f66 726f 7572 6f73 223e 0a20  ject/frouros">. 
+00000970: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000980: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+00000990: 2e74 6563 682f 6261 6467 652f 6672 6f75  .tech/badge/frou
+000009a0: 726f 7322 2061 6c74 3d22 646f 776e 6c6f  ros" alt="downlo
+000009b0: 6164 7322 2f3e 0a20 203c 2f61 3e0a 2020  ads"/>.  </a>.  
+000009c0: 3c21 2d2d 2050 7950 4920 2d2d 3e0a 2020  <!-- PyPI -->.  
+000009d0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000009e0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000009f0: 742f 6672 6f75 726f 7322 3e0a 2020 2020  t/frouros">.    
+00000a00: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000a10: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000a20: 2f70 7970 692f 762f 6672 6f75 726f 732e  /pypi/v/frouros.
+00000a30: 7376 673f 6c61 6265 6c3d 7265 6c65 6173  svg?label=releas
+00000a40: 6526 636f 6c6f 723d 626c 7565 2220 616c  e&color=blue" al
+00000a50: 743d 2270 7970 6922 3e0a 2020 3c2f 613e  t="pypi">.  </a>
+00000a60: 0a20 203c 212d 2d20 5079 7468 6f6e 202d  .  <!-- Python -
+00000a70: 2d3e 0a20 203c 6120 6872 6566 3d22 6874  ->.  <a href="ht
+00000a80: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000a90: 726f 6a65 6374 2f66 726f 7572 6f73 223e  roject/frouros">
+00000aa0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000ab0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000ac0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+00000ad0: 7369 6f6e 732f 6672 6f75 726f 7322 2061  sions/frouros" a
+00000ae0: 6c74 3d22 7079 7468 6f6e 223e 0a20 203c  lt="python">.  <
+00000af0: 2f61 3e0a 2020 3c21 2d2d 204c 6963 656e  /a>.  <!-- Licen
+00000b00: 7365 202d 2d3e 0a20 203c 6120 6872 6566  se -->.  <a href
+00000b10: 3d22 6874 7470 733a 2f2f 6f70 656e 736f  ="https://openso
+00000b20: 7572 6365 2e6f 7267 2f6c 6963 656e 7365  urce.org/license
+00000b30: 732f 4253 442d 332d 436c 6175 7365 223e  s/BSD-3-Clause">
+00000b40: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000b50: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000b60: 6473 2e69 6f2f 6261 6467 652f 6c69 6365  ds.io/badge/lice
+00000b70: 6e73 652d 4253 4425 3230 332d 2d43 6c61  nse-BSD%203--Cla
+00000b80: 7573 652d 626c 7565 2e73 7667 2220 616c  use-blue.svg" al
+00000b90: 743d 2262 7364 5f33 5f6c 6963 656e 7365  t="bsd_3_license
+00000ba0: 223e 0a20 203c 2f61 3e0a 2020 3c21 2d2d  ">.  </a>.  <!--
+00000bb0: 2061 7258 6976 202d 2d3e 0a20 203c 6120   arXiv -->.  <a 
+00000bc0: 6872 6566 3d22 6874 7470 733a 2f2f 6172  href="https://ar
+00000bd0: 7869 762e 6f72 672f 6162 732f 3232 3038  xiv.org/abs/2208
+00000be0: 2e30 3638 3638 223e 0a20 2020 203c 696d  .06868">.    <im
+00000bf0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000c00: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000c10: 6467 652f 6172 5869 762d 3232 3038 2e30  dge/arXiv-2208.0
+00000c20: 3638 3638 2d62 6c75 652e 7376 6722 2061  6868-blue.svg" a
+00000c30: 6c74 3d22 6172 7869 7622 3e0a 2020 3c2f  lt="arxiv">.  </
+00000c40: 613e 0a3c 2f70 3e0a 0a46 726f 7572 6f73  a>.</p>..Frouros
+00000c50: 2069 7320 6120 5079 7468 6f6e 206c 6962   is a Python lib
+00000c60: 7261 7279 2066 6f72 2064 7269 6674 2064  rary for drift d
+00000c70: 6574 6563 7469 6f6e 2069 6e20 6d61 6368  etection in mach
+00000c80: 696e 6520 6c65 6172 6e69 6e67 2073 7973  ine learning sys
+00000c90: 7465 6d73 2074 6861 7420 7072 6f76 6964  tems that provid
+00000ca0: 6573 2061 2063 6f6d 6269 6e61 7469 6f6e  es a combination
+00000cb0: 206f 6620 636c 6173 7369 6361 6c20 616e   of classical an
+00000cc0: 6420 6d6f 7265 2072 6563 656e 7420 616c  d more recent al
+00000cd0: 676f 7269 7468 6d73 2066 6f72 2062 6f74  gorithms for bot
+00000ce0: 6820 636f 6e63 6570 7420 616e 6420 6461  h concept and da
+00000cf0: 7461 2064 7269 6674 2064 6574 6563 7469  ta drift detecti
+00000d00: 6f6e 2e0a 0a3c 7020 616c 6967 6e3d 2263  on...<p align="c
+00000d10: 656e 7465 7222 3e0a 2020 2020 3c69 3e0a  enter">.    <i>.
+00000d20: 2020 2020 2020 2020 2245 7665 7279 7468          "Everyth
+00000d30: 696e 6720 6368 616e 6765 7320 616e 6420  ing changes and 
+00000d40: 6e6f 7468 696e 6720 7374 616e 6473 2073  nothing stands s
+00000d50: 7469 6c6c 220a 2020 2020 3c2f 693e 0a3c  till".    </i>.<
+00000d60: 2f70 3e0a 3c70 2061 6c69 676e 3d22 6365  /p>.<p align="ce
+00000d70: 6e74 6572 223e 0a20 2020 203c 693e 0a20  nter">.    <i>. 
+00000d80: 2020 2020 2020 2022 596f 7520 636f 756c         "You coul
+00000d90: 6420 6e6f 7420 7374 6570 2074 7769 6365  d not step twice
+00000da0: 2069 6e74 6f20 7468 6520 7361 6d65 2072   into the same r
+00000db0: 6976 6572 220a 2020 2020 3c2f 693e 0a3c  iver".    </i>.<
+00000dc0: 2f70 3e0a 3c64 6976 2061 6c69 676e 3d22  /p>.<div align="
+00000dd0: 6365 6e74 6572 2220 7374 796c 653d 2277  center" style="w
+00000de0: 6964 7468 3a20 3730 253b 223e 0a20 2020  idth: 70%;">.   
+00000df0: 203c 7020 616c 6967 6e3d 2272 6967 6874   <p align="right
+00000e00: 223e 0a20 2020 2020 2020 203c 693e 0a20  ">.        <i>. 
+00000e10: 2020 2020 2020 2020 2020 2048 6572 6163             Herac
+00000e20: 6c69 7475 7320 6f66 2045 7068 6573 7573  litus of Ephesus
+00000e30: 2028 3533 352d 3437 3520 4243 452e 290a   (535-475 BCE.).
+00000e40: 2020 2020 2020 2020 3c2f 693e 0a20 2020          </i>.   
+00000e50: 203c 2f70 3e0a 3c2f 6469 763e 0a0a 2d2d   </p>.</div>..--
+00000e60: 2d2d 0a0a 2323 20e2 9aa1 efb8 8f20 5175  --..## ...... Qu
+00000e70: 6963 6b73 7461 7274 0a0a 2323 2320 436f  ickstart..### Co
+00000e80: 6e63 6570 7420 6472 6966 740a 0a41 7320  ncept drift..As 
+00000e90: 6120 7175 6963 6b20 6578 616d 706c 652c  a quick example,
+00000ea0: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
+00000eb0: 6272 6561 7374 2063 616e 6365 7220 6461  breast cancer da
+00000ec0: 7461 7365 7420 746f 2077 6869 6368 2063  taset to which c
+00000ed0: 6f6e 6365 7074 2064 7269 6674 2069 7420  oncept drift it 
+00000ee0: 6973 2069 6e64 7563 6564 2061 6e64 2073  is induced and s
+00000ef0: 686f 7720 7468 6520 7573 6520 6f66 2061  how the use of a
+00000f00: 2063 6f6e 6365 7074 2064 7269 6674 2064   concept drift d
+00000f10: 6574 6563 746f 7220 6c69 6b65 2044 444d  etector like DDM
+00000f20: 2028 4472 6966 7420 4465 7465 6374 696f   (Drift Detectio
+00000f30: 6e20 4d65 7468 6f64 292e 2057 6520 6361  n Method). We ca
+00000f40: 6e20 7365 6520 686f 7720 636f 6e63 6570  n see how concep
+00000f50: 7420 6472 6966 7420 6166 6665 6374 7320  t drift affects 
+00000f60: 7468 6520 7065 7266 6f72 6d61 6e63 6520  the performance 
+00000f70: 696e 2074 6572 6d73 206f 6620 6163 6375  in terms of accu
+00000f80: 7261 6379 2e0a 0a60 6060 7079 7468 6f6e  racy...```python
+00000f90: 0a69 6d70 6f72 7420 6e75 6d70 7920 6173  .import numpy as
+00000fa0: 206e 700a 6672 6f6d 2073 6b6c 6561 726e   np.from sklearn
+00000fb0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00000fc0: 206c 6f61 645f 6272 6561 7374 5f63 616e   load_breast_can
+00000fd0: 6365 720a 6672 6f6d 2073 6b6c 6561 726e  cer.from sklearn
+00000fe0: 2e6c 696e 6561 725f 6d6f 6465 6c20 696d  .linear_model im
+00000ff0: 706f 7274 204c 6f67 6973 7469 6352 6567  port LogisticReg
+00001000: 7265 7373 696f 6e0a 6672 6f6d 2073 6b6c  ression.from skl
+00001010: 6561 726e 2e6d 6f64 656c 5f73 656c 6563  earn.model_selec
+00001020: 7469 6f6e 2069 6d70 6f72 7420 7472 6169  tion import trai
+00001030: 6e5f 7465 7374 5f73 706c 6974 0a66 726f  n_test_split.fro
+00001040: 6d20 736b 6c65 6172 6e2e 7069 7065 6c69  m sklearn.pipeli
+00001050: 6e65 2069 6d70 6f72 7420 5069 7065 6c69  ne import Pipeli
+00001060: 6e65 0a66 726f 6d20 736b 6c65 6172 6e2e  ne.from sklearn.
+00001070: 7072 6570 726f 6365 7373 696e 6720 696d  preprocessing im
+00001080: 706f 7274 2053 7461 6e64 6172 6453 6361  port StandardSca
+00001090: 6c65 720a 0a66 726f 6d20 6672 6f75 726f  ler..from frouro
+000010a0: 732e 6465 7465 6374 6f72 732e 636f 6e63  s.detectors.conc
+000010b0: 6570 745f 6472 6966 7420 696d 706f 7274  ept_drift import
+000010c0: 2044 444d 2c20 4444 4d43 6f6e 6669 670a   DDM, DDMConfig.
+000010d0: 6672 6f6d 2066 726f 7572 6f73 2e6d 6574  from frouros.met
+000010e0: 7269 6373 2069 6d70 6f72 7420 5072 6571  rics import Preq
+000010f0: 7565 6e74 6961 6c45 7272 6f72 0a0a 6e70  uentialError..np
+00001100: 2e72 616e 646f 6d2e 7365 6564 2873 6565  .random.seed(see
+00001110: 643d 3331 290a 0a23 204c 6f61 6420 6272  d=31)..# Load br
+00001120: 6561 7374 2063 616e 6365 7220 6461 7461  east cancer data
+00001130: 7365 740a 582c 2079 203d 206c 6f61 645f  set.X, y = load_
+00001140: 6272 6561 7374 5f63 616e 6365 7228 7265  breast_cancer(re
+00001150: 7475 726e 5f58 5f79 3d54 7275 6529 0a0a  turn_X_y=True)..
+00001160: 2320 5370 6c69 7420 7472 6169 6e20 2837  # Split train (7
+00001170: 3025 2920 616e 6420 7465 7374 2028 3330  0%) and test (30
+00001180: 2529 0a28 0a20 2020 2058 5f74 7261 696e  %).(.    X_train
+00001190: 2c0a 2020 2020 585f 7465 7374 2c0a 2020  ,.    X_test,.  
+000011a0: 2020 795f 7472 6169 6e2c 0a20 2020 2079    y_train,.    y
+000011b0: 5f74 6573 742c 0a29 203d 2074 7261 696e  _test,.) = train
+000011c0: 5f74 6573 745f 7370 6c69 7428 582c 2079  _test_split(X, y
+000011d0: 2c20 7472 6169 6e5f 7369 7a65 3d30 2e37  , train_size=0.7
+000011e0: 2c20 7261 6e64 6f6d 5f73 7461 7465 3d33  , random_state=3
+000011f0: 3129 0a0a 2320 4465 6669 6e65 2061 6e64  1)..# Define and
+00001200: 2066 6974 206d 6f64 656c 0a70 6970 656c   fit model.pipel
+00001210: 696e 6520 3d20 5069 7065 6c69 6e65 280a  ine = Pipeline(.
+00001220: 2020 2020 5b0a 2020 2020 2020 2020 2822      [.        ("
+00001230: 7363 616c 6572 222c 2053 7461 6e64 6172  scaler", Standar
+00001240: 6453 6361 6c65 7228 2929 2c0a 2020 2020  dScaler()),.    
+00001250: 2020 2020 2822 6d6f 6465 6c22 2c20 4c6f      ("model", Lo
+00001260: 6769 7374 6963 5265 6772 6573 7369 6f6e  gisticRegression
+00001270: 2829 292c 0a20 2020 205d 0a29 0a70 6970  ()),.    ].).pip
+00001280: 656c 696e 652e 6669 7428 583d 585f 7472  eline.fit(X=X_tr
+00001290: 6169 6e2c 2079 3d79 5f74 7261 696e 290a  ain, y=y_train).
+000012a0: 0a23 2044 6574 6563 746f 7220 636f 6e66  .# Detector conf
+000012b0: 6967 7572 6174 696f 6e20 616e 6420 696e  iguration and in
+000012c0: 7374 616e 7469 6174 696f 6e0a 636f 6e66  stantiation.conf
+000012d0: 6967 203d 2044 444d 436f 6e66 6967 280a  ig = DDMConfig(.
+000012e0: 2020 2020 7761 726e 696e 675f 6c65 7665      warning_leve
+000012f0: 6c3d 322e 302c 0a20 2020 2064 7269 6674  l=2.0,.    drift
+00001300: 5f6c 6576 656c 3d33 2e30 2c0a 2020 2020  _level=3.0,.    
+00001310: 6d69 6e5f 6e75 6d5f 696e 7374 616e 6365  min_num_instance
+00001320: 733d 3235 2c20 2023 206d 696e 696d 756d  s=25,  # minimum
+00001330: 206e 756d 6265 7220 6f66 2069 6e73 7461   number of insta
+00001340: 6e63 6573 2062 6566 6f72 6520 6368 6563  nces before chec
+00001350: 6b69 6e67 2066 6f72 2063 6f6e 6365 7074  king for concept
+00001360: 2064 7269 6674 0a29 0a64 6574 6563 746f   drift.).detecto
+00001370: 7220 3d20 4444 4d28 636f 6e66 6967 3d63  r = DDM(config=c
+00001380: 6f6e 6669 6729 0a0a 2320 4d65 7472 6963  onfig)..# Metric
+00001390: 2074 6f20 636f 6d70 7574 6520 6163 6375   to compute accu
+000013a0: 7261 6379 0a6d 6574 7269 6320 3d20 5072  racy.metric = Pr
+000013b0: 6571 7565 6e74 6961 6c45 7272 6f72 2861  equentialError(a
+000013c0: 6c70 6861 3d31 2e30 2920 2023 2061 6c70  lpha=1.0)  # alp
+000013d0: 6861 3d31 2e30 2069 7320 6571 7569 7661  ha=1.0 is equiva
+000013e0: 6c65 6e74 2074 6f20 6e6f 726d 616c 2061  lent to normal a
+000013f0: 6363 7572 6163 790a 0a64 6566 2073 7472  ccuracy..def str
+00001400: 6561 6d5f 7465 7374 2858 5f74 6573 742c  eam_test(X_test,
+00001410: 2079 5f74 6573 742c 2079 2c20 6d65 7472   y_test, y, metr
+00001420: 6963 2c20 6465 7465 6374 6f72 293a 0a20  ic, detector):. 
+00001430: 2020 2022 2222 5369 6d75 6c61 7465 2064     """Simulate d
+00001440: 6174 6120 7374 7265 616d 206f 7665 7220  ata stream over 
+00001450: 585f 7465 7374 2061 6e64 2079 5f74 6573  X_test and y_tes
+00001460: 742e 2079 2069 7320 7468 6520 7472 7565  t. y is the true
+00001470: 206c 6162 656c 2e22 2222 0a20 2020 2064   label.""".    d
+00001480: 7269 6674 5f66 6c61 6720 3d20 4661 6c73  rift_flag = Fals
+00001490: 650a 2020 2020 666f 7220 692c 2028 582c  e.    for i, (X,
+000014a0: 2079 2920 696e 2065 6e75 6d65 7261 7465   y) in enumerate
+000014b0: 287a 6970 2858 5f74 6573 742c 2079 5f74  (zip(X_test, y_t
+000014c0: 6573 7429 293a 0a20 2020 2020 2020 2079  est)):.        y
+000014d0: 5f70 7265 6420 3d20 7069 7065 6c69 6e65  _pred = pipeline
+000014e0: 2e70 7265 6469 6374 2858 2e72 6573 6861  .predict(X.resha
+000014f0: 7065 2831 2c20 2d31 2929 0a20 2020 2020  pe(1, -1)).     
+00001500: 2020 2065 7272 6f72 203d 2031 202d 2028     error = 1 - (
+00001510: 795f 7072 6564 2e69 7465 6d28 2920 3d3d  y_pred.item() ==
+00001520: 2079 2e69 7465 6d28 2929 0a20 2020 2020   y.item()).     
+00001530: 2020 206d 6574 7269 635f 6572 726f 7220     metric_error 
+00001540: 3d20 6d65 7472 6963 2865 7272 6f72 5f76  = metric(error_v
+00001550: 616c 7565 3d65 7272 6f72 290a 2020 2020  alue=error).    
+00001560: 2020 2020 5f20 3d20 6465 7465 6374 6f72      _ = detector
+00001570: 2e75 7064 6174 6528 7661 6c75 653d 6572  .update(value=er
+00001580: 726f 7229 0a20 2020 2020 2020 2073 7461  ror).        sta
+00001590: 7475 7320 3d20 6465 7465 6374 6f72 2e73  tus = detector.s
+000015a0: 7461 7475 730a 2020 2020 2020 2020 6966  tatus.        if
+000015b0: 2073 7461 7475 735b 2264 7269 6674 225d   status["drift"]
+000015c0: 2061 6e64 206e 6f74 2064 7269 6674 5f66   and not drift_f
+000015d0: 6c61 673a 0a20 2020 2020 2020 2020 2020  lag:.           
+000015e0: 2064 7269 6674 5f66 6c61 6720 3d20 5472   drift_flag = Tr
+000015f0: 7565 0a20 2020 2020 2020 2020 2020 2070  ue.            p
+00001600: 7269 6e74 2866 2243 6f6e 6365 7074 2064  rint(f"Concept d
+00001610: 7269 6674 2064 6574 6563 7465 6420 6174  rift detected at
+00001620: 2073 7465 7020 7b69 7d2e 2041 6363 7572   step {i}. Accur
+00001630: 6163 793a 207b 3120 2d20 6d65 7472 6963  acy: {1 - metric
+00001640: 5f65 7272 6f72 3a2e 3466 7d22 290a 2020  _error:.4f}").  
+00001650: 2020 6966 206e 6f74 2064 7269 6674 5f66    if not drift_f
+00001660: 6c61 673a 0a20 2020 2020 2020 2070 7269  lag:.        pri
+00001670: 6e74 2822 4e6f 2063 6f6e 6365 7074 2064  nt("No concept d
+00001680: 7269 6674 2064 6574 6563 7465 6422 290a  rift detected").
+00001690: 2020 2020 7072 696e 7428 6622 4669 6e61      print(f"Fina
+000016a0: 6c20 6163 6375 7261 6379 3a20 7b31 202d  l accuracy: {1 -
+000016b0: 206d 6574 7269 635f 6572 726f 723a 2e34   metric_error:.4
+000016c0: 667d 5c6e 2229 0a0a 2320 5369 6d75 6c61  f}\n")..# Simula
+000016d0: 7465 2064 6174 6120 7374 7265 616d 2028  te data stream (
+000016e0: 6173 7375 6d69 6e67 2074 6573 7420 6c61  assuming test la
+000016f0: 6265 6c20 6176 6169 6c61 626c 6520 6166  bel available af
+00001700: 7465 7220 6561 6368 2070 7265 6469 6374  ter each predict
+00001710: 696f 6e29 0a23 204e 6f20 636f 6e63 6570  ion).# No concep
+00001720: 7420 6472 6966 7420 6973 2065 7870 6563  t drift is expec
+00001730: 7465 6420 746f 206f 6363 7572 0a73 7472  ted to occur.str
+00001740: 6561 6d5f 7465 7374 280a 2020 2020 585f  eam_test(.    X_
+00001750: 7465 7374 3d58 5f74 6573 742c 0a20 2020  test=X_test,.   
+00001760: 2079 5f74 6573 743d 795f 7465 7374 2c0a   y_test=y_test,.
+00001770: 2020 2020 793d 792c 0a20 2020 206d 6574      y=y,.    met
+00001780: 7269 633d 6d65 7472 6963 2c0a 2020 2020  ric=metric,.    
+00001790: 6465 7465 6374 6f72 3d64 6574 6563 746f  detector=detecto
+000017a0: 722c 0a29 0a23 203e 3e20 4e6f 2063 6f6e  r,.).# >> No con
+000017b0: 6365 7074 2064 7269 6674 2064 6574 6563  cept drift detec
+000017c0: 7465 640a 2320 3e3e 2046 696e 616c 2061  ted.# >> Final a
+000017d0: 6363 7572 6163 793a 2030 2e39 3736 360a  ccuracy: 0.9766.
+000017e0: 0a23 2049 4d50 4f52 5441 4e54 3a20 496e  .# IMPORTANT: In
+000017f0: 6475 6365 2f73 696d 756c 6174 6520 636f  duce/simulate co
+00001800: 6e63 6570 7420 6472 6966 7420 696e 2074  ncept drift in t
+00001810: 6865 206c 6173 7420 7061 7274 2028 3230  he last part (20
+00001820: 2529 0a23 206f 6620 795f 7465 7374 2062  %).# of y_test b
+00001830: 7920 6d6f 6469 6679 696e 6720 736f 6d65  y modifying some
+00001840: 206c 6162 656c 7320 2835 3025 2061 7070   labels (50% app
+00001850: 726f 7829 2e20 5468 6572 6566 6f72 652c  rox). Therefore,
+00001860: 2063 6861 6e67 696e 6720 5028 797c 5829   changing P(y|X)
+00001870: 290a 6472 6966 745f 7369 7a65 203d 2069  ).drift_size = i
+00001880: 6e74 2879 5f74 6573 742e 7368 6170 655b  nt(y_test.shape[
+00001890: 305d 202a 2030 2e32 290a 795f 7465 7374  0] * 0.2).y_test
+000018a0: 5f64 7269 6674 203d 2079 5f74 6573 745b  _drift = y_test[
+000018b0: 2d64 7269 6674 5f73 697a 653a 5d0a 6d6f  -drift_size:].mo
+000018c0: 6469 6679 5f69 6478 203d 206e 702e 7261  dify_idx = np.ra
+000018d0: 6e64 6f6d 2e72 616e 6428 2a79 5f74 6573  ndom.rand(*y_tes
+000018e0: 745f 6472 6966 742e 7368 6170 6529 203c  t_drift.shape) <
+000018f0: 3d20 302e 350a 795f 7465 7374 5f64 7269  = 0.5.y_test_dri
+00001900: 6674 5b6d 6f64 6966 795f 6964 785d 203d  ft[modify_idx] =
+00001910: 2028 795f 7465 7374 5f64 7269 6674 5b6d   (y_test_drift[m
+00001920: 6f64 6966 795f 6964 785d 202b 2031 2920  odify_idx] + 1) 
+00001930: 2520 6c65 6e28 6e70 2e75 6e69 7175 6528  % len(np.unique(
+00001940: 795f 7465 7374 2929 0a79 5f74 6573 745b  y_test)).y_test[
+00001950: 2d64 7269 6674 5f73 697a 653a 5d20 3d20  -drift_size:] = 
+00001960: 795f 7465 7374 5f64 7269 6674 0a0a 2320  y_test_drift..# 
+00001970: 5265 7365 7420 6465 7465 6374 6f72 2061  Reset detector a
+00001980: 6e64 206d 6574 7269 630a 6465 7465 6374  nd metric.detect
+00001990: 6f72 2e72 6573 6574 2829 0a6d 6574 7269  or.reset().metri
+000019a0: 632e 7265 7365 7428 290a 0a23 2053 696d  c.reset()..# Sim
+000019b0: 756c 6174 6520 6461 7461 2073 7472 6561  ulate data strea
+000019c0: 6d20 2861 7373 756d 696e 6720 7465 7374  m (assuming test
+000019d0: 206c 6162 656c 2061 7661 696c 6162 6c65   label available
+000019e0: 2061 6674 6572 2065 6163 6820 7072 6564   after each pred
+000019f0: 6963 7469 6f6e 290a 2320 436f 6e63 6570  iction).# Concep
+00001a00: 7420 6472 6966 7420 6973 2065 7870 6563  t drift is expec
+00001a10: 7465 6420 746f 206f 6363 7572 2062 6563  ted to occur bec
+00001a20: 6175 7365 206f 6620 7468 6520 6c61 6265  ause of the labe
+00001a30: 6c20 6d6f 6469 6669 6361 7469 6f6e 0a73  l modification.s
+00001a40: 7472 6561 6d5f 7465 7374 280a 2020 2020  tream_test(.    
+00001a50: 585f 7465 7374 3d58 5f74 6573 742c 0a20  X_test=X_test,. 
+00001a60: 2020 2079 5f74 6573 743d 795f 7465 7374     y_test=y_test
+00001a70: 2c0a 2020 2020 793d 792c 0a20 2020 206d  ,.    y=y,.    m
+00001a80: 6574 7269 633d 6d65 7472 6963 2c0a 2020  etric=metric,.  
+00001a90: 2020 6465 7465 6374 6f72 3d64 6574 6563    detector=detec
+00001aa0: 746f 722c 0a29 0a23 203e 3e20 436f 6e63  tor,.).# >> Conc
+00001ab0: 6570 7420 6472 6966 7420 6465 7465 6374  ept drift detect
+00001ac0: 6564 2061 7420 7374 6570 2031 3432 2e20  ed at step 142. 
+00001ad0: 4163 6375 7261 6379 3a20 302e 3935 3130  Accuracy: 0.9510
+00001ae0: 0a23 203e 3e20 4669 6e61 6c20 6163 6375  .# >> Final accu
+00001af0: 7261 6379 3a20 302e 3834 3830 0a60 6060  racy: 0.8480.```
+00001b00: 0a0a 4d6f 7265 2063 6f6e 6365 7074 2064  ..More concept d
+00001b10: 7269 6674 2065 7861 6d70 6c65 7320 6361  rift examples ca
+00001b20: 6e20 6265 2066 6f75 6e64 205b 6865 7265  n be found [here
+00001b30: 5d28 6874 7470 733a 2f2f 6672 6f75 726f  ](https://frouro
+00001b40: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
+00001b50: 2f65 6e2f 6c61 7465 7374 2f65 7861 6d70  /en/latest/examp
+00001b60: 6c65 732f 636f 6e63 6570 745f 6472 6966  les/concept_drif
+00001b70: 742e 6874 6d6c 292e 0a0a 2323 2320 4461  t.html)...### Da
+00001b80: 7461 2064 7269 6674 0a0a 4173 2061 2071  ta drift..As a q
+00001b90: 7569 636b 2065 7861 6d70 6c65 2c20 7765  uick example, we
+00001ba0: 2063 616e 2075 7365 2074 6865 2069 7269   can use the iri
+00001bb0: 7320 6461 7461 7365 7420 746f 2077 6869  s dataset to whi
+00001bc0: 6368 2064 6174 6120 6472 6966 7420 6973  ch data drift is
+00001bd0: 2069 6e64 7563 6564 2061 6e64 2073 686f   induced and sho
+00001be0: 7720 7468 6520 7573 6520 6f66 2061 2064  w the use of a d
+00001bf0: 6174 6120 6472 6966 7420 6465 7465 6374  ata drift detect
+00001c00: 6f72 206c 696b 6520 4b6f 6c6d 6f67 6f72  or like Kolmogor
+00001c10: 6f76 2d53 6d69 726e 6f76 2074 6573 742e  ov-Smirnov test.
+00001c20: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00001c30: 7274 206e 756d 7079 2061 7320 6e70 0a66  rt numpy as np.f
+00001c40: 726f 6d20 736b 6c65 6172 6e2e 6461 7461  rom sklearn.data
+00001c50: 7365 7473 2069 6d70 6f72 7420 6c6f 6164  sets import load
+00001c60: 5f69 7269 730a 6672 6f6d 2073 6b6c 6561  _iris.from sklea
+00001c70: 726e 2e6d 6f64 656c 5f73 656c 6563 7469  rn.model_selecti
+00001c80: 6f6e 2069 6d70 6f72 7420 7472 6169 6e5f  on import train_
+00001c90: 7465 7374 5f73 706c 6974 0a66 726f 6d20  test_split.from 
+00001ca0: 736b 6c65 6172 6e2e 7472 6565 2069 6d70  sklearn.tree imp
+00001cb0: 6f72 7420 4465 6369 7369 6f6e 5472 6565  ort DecisionTree
+00001cc0: 436c 6173 7369 6669 6572 0a0a 6672 6f6d  Classifier..from
+00001cd0: 2066 726f 7572 6f73 2e64 6574 6563 746f   frouros.detecto
+00001ce0: 7273 2e64 6174 615f 6472 6966 7420 696d  rs.data_drift im
+00001cf0: 706f 7274 204b 5354 6573 740a 0a6e 702e  port KSTest..np.
+00001d00: 7261 6e64 6f6d 2e73 6565 6428 7365 6564  random.seed(seed
+00001d10: 3d33 3129 0a0a 2320 4c6f 6164 2069 7269  =31)..# Load iri
+00001d20: 7320 6461 7461 7365 740a 582c 2079 203d  s dataset.X, y =
+00001d30: 206c 6f61 645f 6972 6973 2872 6574 7572   load_iris(retur
+00001d40: 6e5f 585f 793d 5472 7565 290a 0a23 2053  n_X_y=True)..# S
+00001d50: 706c 6974 2074 7261 696e 2028 3730 2529  plit train (70%)
+00001d60: 2061 6e64 2074 6573 7420 2833 3025 290a   and test (30%).
+00001d70: 280a 2020 2020 585f 7472 6169 6e2c 0a20  (.    X_train,. 
+00001d80: 2020 2058 5f74 6573 742c 0a20 2020 2079     X_test,.    y
+00001d90: 5f74 7261 696e 2c0a 2020 2020 795f 7465  _train,.    y_te
+00001da0: 7374 2c0a 2920 3d20 7472 6169 6e5f 7465  st,.) = train_te
+00001db0: 7374 5f73 706c 6974 2858 2c20 792c 2074  st_split(X, y, t
+00001dc0: 7261 696e 5f73 697a 653d 302e 372c 2072  rain_size=0.7, r
+00001dd0: 616e 646f 6d5f 7374 6174 653d 3331 290a  andom_state=31).
+00001de0: 0a23 2053 6574 2074 6865 2066 6561 7475  .# Set the featu
+00001df0: 7265 2069 6e64 6578 2074 6f20 7768 6963  re index to whic
+00001e00: 6820 6465 7465 6374 6f72 2069 7320 6170  h detector is ap
+00001e10: 706c 6965 640a 6665 6174 7572 655f 6964  plied.feature_id
+00001e20: 7820 3d20 300a 0a23 2049 4d50 4f52 5441  x = 0..# IMPORTA
+00001e30: 4e54 3a20 496e 6475 6365 2f73 696d 756c  NT: Induce/simul
+00001e40: 6174 6520 6461 7461 2064 7269 6674 2069  ate data drift i
+00001e50: 6e20 7468 6520 7365 6c65 6374 6564 2066  n the selected f
+00001e60: 6561 7475 7265 206f 6620 795f 7465 7374  eature of y_test
+00001e70: 2062 790a 2320 6170 706c 7969 6e67 2073   by.# applying s
+00001e80: 6f6d 6520 6761 7573 7369 616e 206e 6f69  ome gaussian noi
+00001e90: 7365 2e20 5468 6572 6566 6f72 652c 2063  se. Therefore, c
+00001ea0: 6861 6e67 696e 6720 5028 5829 290a 585f  hanging P(X)).X_
+00001eb0: 7465 7374 5b3a 2c20 6665 6174 7572 655f  test[:, feature_
+00001ec0: 6964 785d 202b 3d20 6e70 2e72 616e 646f  idx] += np.rando
+00001ed0: 6d2e 6e6f 726d 616c 280a 2020 2020 6c6f  m.normal(.    lo
+00001ee0: 633d 302e 302c 0a20 2020 2073 6361 6c65  c=0.0,.    scale
+00001ef0: 3d33 2e30 2c0a 2020 2020 7369 7a65 3d58  =3.0,.    size=X
+00001f00: 5f74 6573 742e 7368 6170 655b 305d 2c0a  _test.shape[0],.
+00001f10: 290a 0a23 2044 6566 696e 6520 616e 6420  )..# Define and 
+00001f20: 6669 7420 6d6f 6465 6c0a 6d6f 6465 6c20  fit model.model 
+00001f30: 3d20 4465 6369 7369 6f6e 5472 6565 436c  = DecisionTreeCl
+00001f40: 6173 7369 6669 6572 2872 616e 646f 6d5f  assifier(random_
+00001f50: 7374 6174 653d 3331 290a 6d6f 6465 6c2e  state=31).model.
+00001f60: 6669 7428 583d 585f 7472 6169 6e2c 2079  fit(X=X_train, y
+00001f70: 3d79 5f74 7261 696e 290a 0a23 2053 6574  =y_train)..# Set
+00001f80: 2073 6967 6e69 6669 6361 6e63 6520 6c65   significance le
+00001f90: 7665 6c20 666f 7220 6879 706f 7468 6573  vel for hypothes
+00001fa0: 6973 2074 6573 7469 6e67 0a61 6c70 6861  is testing.alpha
+00001fb0: 203d 2030 2e30 3031 0a23 2044 6566 696e   = 0.001.# Defin
+00001fc0: 6520 616e 6420 6669 7420 6465 7465 6374  e and fit detect
+00001fd0: 6f72 0a64 6574 6563 746f 7220 3d20 4b53  or.detector = KS
+00001fe0: 5465 7374 2829 0a5f 203d 2064 6574 6563  Test()._ = detec
+00001ff0: 746f 722e 6669 7428 583d 585f 7472 6169  tor.fit(X=X_trai
+00002000: 6e5b 3a2c 2066 6561 7475 7265 5f69 6478  n[:, feature_idx
+00002010: 5d29 0a0a 2320 4170 706c 7920 6465 7465  ])..# Apply dete
+00002020: 6374 6f72 2074 6f20 7468 6520 7365 6c65  ctor to the sele
+00002030: 6374 6564 2066 6561 7475 7265 206f 6620  cted feature of 
+00002040: 585f 7465 7374 0a72 6573 756c 742c 205f  X_test.result, _
+00002050: 203d 2064 6574 6563 746f 722e 636f 6d70   = detector.comp
+00002060: 6172 6528 583d 585f 7465 7374 5b3a 2c20  are(X=X_test[:, 
+00002070: 6665 6174 7572 655f 6964 785d 290a 0a23  feature_idx])..#
+00002080: 2043 6865 636b 2069 6620 6472 6966 7420   Check if drift 
+00002090: 6973 2074 616b 696e 6720 706c 6163 650a  is taking place.
+000020a0: 6966 2072 6573 756c 742e 705f 7661 6c75  if result.p_valu
+000020b0: 6520 3c3d 2061 6c70 6861 3a0a 2020 2020  e <= alpha:.    
+000020c0: 7072 696e 7428 6622 4461 7461 2064 7269  print(f"Data dri
+000020d0: 6674 2064 6574 6563 7465 6420 6174 2066  ft detected at f
+000020e0: 6561 7475 7265 207b 6665 6174 7572 655f  eature {feature_
+000020f0: 6964 787d 2229 0a65 6c73 653a 0a20 2020  idx}").else:.   
+00002100: 2070 7269 6e74 2866 224e 6f20 6461 7461   print(f"No data
+00002110: 2064 7269 6674 2064 6574 6563 7465 6420   drift detected 
+00002120: 6174 2066 6561 7475 7265 207b 6665 6174  at feature {feat
+00002130: 7572 655f 6964 787d 2229 0a23 203e 3e20  ure_idx}").# >> 
+00002140: 4461 7461 2064 7269 6674 2064 6574 6563  Data drift detec
+00002150: 7465 6420 6174 2066 6561 7475 7265 2030  ted at feature 0
+00002160: 0a23 2054 6865 7265 666f 7265 2c20 7765  .# Therefore, we
+00002170: 2063 616e 2072 656a 6563 7420 4830 2028   can reject H0 (
+00002180: 626f 7468 2073 616d 706c 6573 2063 6f6d  both samples com
+00002190: 6520 6672 6f6d 2074 6865 2073 616d 6520  e from the same 
+000021a0: 6469 7374 7269 6275 7469 6f6e 292e 0a60  distribution)..`
+000021b0: 6060 0a0a 4d6f 7265 2064 6174 6120 6472  ``..More data dr
+000021c0: 6966 7420 6578 616d 706c 6573 2063 616e  ift examples can
+000021d0: 2062 6520 666f 756e 6420 5b68 6572 655d   be found [here]
+000021e0: 2868 7474 7073 3a2f 2f66 726f 7572 6f73  (https://frouros
+000021f0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002200: 656e 2f6c 6174 6573 742f 6578 616d 706c  en/latest/exampl
+00002210: 6573 2f64 6174 615f 6472 6966 742e 6874  es/data_drift.ht
+00002220: 6d6c 292e 0a0a 2323 20f0 9f9b a020 496e  ml)...## .... In
+00002230: 7374 616c 6c61 7469 6f6e 0a0a 4672 6f75  stallation..Frou
+00002240: 726f 7320 6361 6e20 6265 2069 6e73 7461  ros can be insta
+00002250: 6c6c 6564 2076 6961 2070 6970 3a0a 0a60  lled via pip:..`
+00002260: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00002270: 6c6c 2066 726f 7572 6f73 0a60 6060 0a0a  ll frouros.```..
+00002280: 2323 20f0 9f95 b5f0 9f8f bbe2 808d e299  ## .............
+00002290: 82ef b88f efb8 8f20 4472 6966 7420 6465  ....... Drift de
+000022a0: 7465 6374 696f 6e20 6d65 7468 6f64 730a  tection methods.
+000022b0: 0a54 6865 2063 7572 7265 6e74 6c79 2069  .The currently i
+000022c0: 6d70 6c65 6d65 6e74 6564 2064 6574 6563  mplemented detec
+000022d0: 746f 7273 2061 7265 206c 6973 7465 6420  tors are listed 
+000022e0: 696e 2074 6865 2066 6f6c 6c6f 7769 6e67  in the following
+000022f0: 2074 6162 6c65 2e0a 0a3c 7461 626c 6520   table...<table 
+00002300: 7374 796c 653d 2277 6964 7468 3a20 3130  style="width: 10
+00002310: 3025 3b20 7465 7874 2d61 6c69 676e 3a20  0%; text-align: 
+00002320: 6365 6e74 6572 3b20 626f 7264 6572 2d63  center; border-c
+00002330: 6f6c 6c61 7073 653a 2063 6f6c 6c61 7073  ollapse: collaps
+00002340: 653b 2062 6f72 6465 723a 2031 7078 2073  e; border: 1px s
+00002350: 6f6c 6964 2067 7265 793b 223e 0a20 203c  olid grey;">.  <
+00002360: 7468 6561 643e 0a20 2020 203c 7472 3e0a  thead>.    <tr>.
+00002370: 2020 2020 3c74 6820 7374 796c 653d 2274      <th style="t
+00002380: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00002390: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000023a0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000023b0: 6e67 3a20 3470 783b 223e 4472 6966 7420  ng: 4px;">Drift 
+000023c0: 6465 7465 6374 6f72 3c2f 7468 3e0a 2020  detector</th>.  
+000023d0: 2020 3c74 6820 7374 796c 653d 2274 6578    <th style="tex
+000023e0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000023f0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002400: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002410: 3a20 3470 783b 223e 5479 7065 3c2f 7468  : 4px;">Type</th
+00002420: 3e0a 2020 2020 3c74 6820 7374 796c 653d  >.    <th style=
+00002430: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002440: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002450: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002460: 6469 6e67 3a20 3470 783b 223e 4661 6d69  ding: 4px;">Fami
+00002470: 6c79 3c2f 7468 3e0a 2020 2020 3c74 6820  ly</th>.    <th 
+00002480: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00002490: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000024a0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000024b0: 793b 2070 6164 6469 6e67 3a20 3470 783b  y; padding: 4px;
+000024c0: 223e 556e 6976 6172 6961 7465 2028 5529  ">Univariate (U)
+000024d0: 202f 204d 756c 7469 7661 7269 6174 6520   / Multivariate 
+000024e0: 284d 293c 2f74 683e 0a20 2020 203c 7468  (M)</th>.    <th
+000024f0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00002500: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00002510: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00002520: 6579 3b20 7061 6464 696e 673a 2034 7078  ey; padding: 4px
+00002530: 3b22 3e4e 756d 6572 6963 616c 2028 4e29  ;">Numerical (N)
+00002540: 202f 2043 6174 6567 6f72 6963 616c 2028   / Categorical (
+00002550: 4329 3c2f 7468 3e0a 2020 2020 3c74 6820  C)</th>.    <th 
+00002560: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00002570: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00002580: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00002590: 793b 2070 6164 6469 6e67 3a20 3470 783b  y; padding: 4px;
+000025a0: 223e 4d65 7468 6f64 3c2f 7468 3e0a 2020  ">Method</th>.  
+000025b0: 2020 3c74 6820 7374 796c 653d 2274 6578    <th style="tex
+000025c0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000025d0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000025e0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000025f0: 3a20 3470 783b 223e 5265 6665 7265 6e63  : 4px;">Referenc
+00002600: 653c 2f74 683e 0a20 2020 203c 2f74 723e  e</th>.    </tr>
+00002610: 0a20 203c 2f74 6865 6164 3e0a 2020 3c74  .  </thead>.  <t
+00002620: 626f 6479 3e0a 2020 3c74 723e 0a20 2020  body>.  <tr>.   
+00002630: 203c 7464 2072 6f77 7370 616e 3d22 3133   <td rowspan="13
+00002640: 2220 7374 796c 653d 2274 6578 742d 616c  " style="text-al
+00002650: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00002660: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00002670: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00002680: 783b 223e 436f 6e63 6570 7420 6472 6966  x;">Concept drif
+00002690: 743c 2f74 643e 0a20 2020 203c 7464 2072  t</td>.    <td r
+000026a0: 6f77 7370 616e 3d22 3133 2220 7374 796c  owspan="13" styl
+000026b0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000026c0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000026d0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000026e0: 6164 6469 6e67 3a20 3870 783b 223e 5374  adding: 8px;">St
+000026f0: 7265 616d 696e 673c 2f74 643e 0a20 2020  reaming</td>.   
+00002700: 203c 7464 2072 6f77 7370 616e 3d22 3422   <td rowspan="4"
+00002710: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00002720: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00002730: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00002740: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00002750: 3b22 3e43 6861 6e67 6520 6465 7465 6374  ;">Change detect
+00002760: 696f 6e3c 2f74 643e 0a20 2020 203c 7464  ion</td>.    <td
+00002770: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00002780: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00002790: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000027a0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000027b0: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
+000027c0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+000027d0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+000027e0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+000027f0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00002800: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
+00002810: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00002820: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00002830: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00002840: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00002850: 7078 3b22 3e42 4f43 443c 2f74 643e 0a20  px;">BOCD</td>. 
+00002860: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00002870: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00002880: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00002890: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000028a0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
+000028b0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+000028c0: 672f 3130 2e34 3835 3530 2f61 7258 6976  g/10.48550/arXiv
+000028d0: 2e30 3731 302e 3337 3432 223e 4164 616d  .0710.3742">Adam
+000028e0: 7320 616e 6420 4d61 634b 6179 2028 3230  s and MacKay (20
+000028f0: 3037 293c 2f61 3e3c 2f74 643e 0a20 203c  07)</a></td>.  <
+00002900: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
+00002910: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00002920: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00002930: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00002940: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00002950: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
+00002960: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002970: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002980: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002990: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+000029a0: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
+000029b0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+000029c0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000029d0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000029e0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000029f0: 3a20 3870 783b 223e 4355 5355 4d3c 2f74  : 8px;">CUSUM</t
+00002a00: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00002a10: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00002a20: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00002a30: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00002a40: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
+00002a50: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+00002a60: 692e 6f72 672f 3130 2e32 3330 372f 3233  i.org/10.2307/23
+00002a70: 3333 3030 3922 3e50 6167 6520 2831 3935  33009">Page (195
+00002a80: 3429 3c2f 613e 3c2f 7464 3e0a 2020 3c2f  4)</a></td>.  </
+00002a90: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
+00002aa0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00002ab0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00002ac0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00002ad0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00002ae0: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
+00002af0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00002b00: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00002b10: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00002b20: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00002b30: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
+00002b40: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002b50: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002b60: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002b70: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00002b80: 2038 7078 3b22 3e47 656f 6d65 7472 6963   8px;">Geometric
+00002b90: 206d 6f76 696e 6720 6176 6572 6167 653c   moving average<
+00002ba0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00002bb0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00002bc0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00002bd0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00002be0: 7061 6464 696e 673a 2038 7078 3b22 3e3c  padding: 8px;"><
+00002bf0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002c00: 646f 692e 6f72 672f 3130 2e32 3330 372f  doi.org/10.2307/
+00002c10: 3132 3636 3434 3322 3e52 6f62 6572 7473  1266443">Roberts
+00002c20: 2028 3139 3539 293c 2f61 3e3c 2f74 643e   (1959)</a></td>
+00002c30: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+00002c40: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00002c50: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00002c60: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00002c70: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00002c80: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
+00002c90: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00002ca0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00002cb0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00002cc0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00002cd0: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
+00002ce0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00002cf0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002d00: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002d10: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002d20: 6469 6e67 3a20 3870 783b 223e 5061 6765  ding: 8px;">Page
+00002d30: 2048 696e 6b6c 6579 3c2f 7464 3e0a 2020   Hinkley</td>.  
+00002d40: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00002d50: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00002d60: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002d70: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002d80: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00002d90: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00002da0: 2f31 302e 3233 3037 2f32 3333 3330 3039  /10.2307/2333009
+00002db0: 223e 5061 6765 2028 3139 3534 293c 2f61  ">Page (1954)</a
+00002dc0: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+00002dd0: 203c 7472 3e0a 2020 2020 3c74 6420 726f   <tr>.    <td ro
+00002de0: 7773 7061 6e3d 2236 2220 7374 796c 653d  wspan="6" style=
+00002df0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002e00: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002e10: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002e20: 6469 6e67 3a20 3870 783b 223e 5374 6174  ding: 8px;">Stat
+00002e30: 6973 7469 6361 6c20 7072 6f63 6573 7320  istical process 
+00002e40: 636f 6e74 726f 6c3c 2f74 643e 0a20 2020  control</td>.   
+00002e50: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002e60: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002e70: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002e80: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00002e90: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
+00002ea0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00002eb0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00002ec0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002ed0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002ee0: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
+00002ef0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00002f00: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00002f10: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00002f20: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00002f30: 673a 2038 7078 3b22 3e44 444d 3c2f 7464  g: 8px;">DDM</td
+00002f40: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00002f50: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002f60: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002f70: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002f80: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
+00002f90: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
+00002fa0: 2e6f 7267 2f31 302e 3130 3037 2f39 3738  .org/10.1007/978
+00002fb0: 2d33 2d35 3430 2d32 3836 3435 2d35 5f32  -3-540-28645-5_2
+00002fc0: 3922 3e47 616d 6120 6574 2061 6c2e 2028  9">Gama et al. (
+00002fd0: 3230 3034 293c 2f61 3e3c 2f74 643e 0a20  2004)</a></td>. 
+00002fe0: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
+00002ff0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00003000: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00003010: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00003020: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00003030: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
+00003040: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00003050: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00003060: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00003070: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00003080: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
+00003090: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+000030a0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+000030b0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000030c0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000030d0: 6e67 3a20 3870 783b 223e 4543 4444 2d57  ng: 8px;">ECDD-W
+000030e0: 543c 2f74 643e 0a20 2020 203c 7464 2073  T</td>.    <td s
+000030f0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003100: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003110: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003120: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003130: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00003140: 2f2f 646f 692e 6f72 672f 3130 2e31 3031  //doi.org/10.101
+00003150: 362f 6a2e 7061 7472 6563 2e32 3031 312e  6/j.patrec.2011.
+00003160: 3038 2e30 3139 223e 526f 7373 2065 7420  08.019">Ross et 
+00003170: 616c 2e20 2832 3031 3229 3c2f 613e 3c2f  al. (2012)</a></
+00003180: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00003190: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+000031a0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000031b0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000031c0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000031d0: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+000031e0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000031f0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00003200: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003210: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003220: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00003230: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003240: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003250: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003260: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003270: 7061 6464 696e 673a 2038 7078 3b22 3e45  padding: 8px;">E
+00003280: 4444 4d3c 2f74 643e 0a20 2020 203c 7464  DDM</td>.    <td
+00003290: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+000032a0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+000032b0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000032c0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000032d0: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
+000032e0: 733a 2f2f 7777 772e 7265 7365 6172 6368  s://www.research
+000032f0: 6761 7465 2e6e 6574 2f70 7562 6c69 6361  gate.net/publica
+00003300: 7469 6f6e 2f32 3435 3939 3937 3034 5f45  tion/245999704_E
+00003310: 6172 6c79 5f44 7269 6674 5f44 6574 6563  arly_Drift_Detec
+00003320: 7469 6f6e 5f4d 6574 686f 6422 3e42 6165  tion_Method">Bae
+00003330: 6e61 2d47 6172 63c4 b161 2065 7420 616c  na-Garc..a et al
+00003340: 2e20 2832 3030 3629 3c2f 613e 3c2f 7464  . (2006)</a></td
+00003350: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+00003360: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00003370: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003380: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003390: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000033a0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
+000033b0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+000033c0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+000033d0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+000033e0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+000033f0: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
+00003400: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00003410: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00003420: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00003430: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00003440: 6464 696e 673a 2038 7078 3b22 3e48 4444  dding: 8px;">HDD
+00003450: 4d2d 413c 2f74 643e 0a20 2020 203c 7464  M-A</td>.    <td
+00003460: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00003470: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00003480: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00003490: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000034a0: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
+000034b0: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
+000034c0: 3130 392f 544b 4445 2e32 3031 342e 3233  109/TKDE.2014.23
+000034d0: 3435 3338 3222 3e46 7269 6173 2d42 6c61  45382">Frias-Bla
+000034e0: 6e63 6f20 6574 2061 6c2e 2028 3230 3134  nco et al. (2014
+000034f0: 293c 2f61 3e3c 2f74 643e 0a20 203c 2f74  )</a></td>.  </t
+00003500: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
+00003510: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00003520: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00003530: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00003540: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00003550: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
+00003560: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00003570: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00003580: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00003590: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+000035a0: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
+000035b0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+000035c0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+000035d0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+000035e0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+000035f0: 3870 783b 223e 4844 444d 2d57 3c2f 7464  8px;">HDDM-W</td
+00003600: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00003610: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00003620: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00003630: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00003640: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
+00003650: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
+00003660: 2e6f 7267 2f31 302e 3131 3039 2f54 4b44  .org/10.1109/TKD
+00003670: 452e 3230 3134 2e32 3334 3533 3832 223e  E.2014.2345382">
+00003680: 4672 6961 732d 426c 616e 636f 2065 7420  Frias-Blanco et 
+00003690: 616c 2e20 2832 3031 3429 3c2f 613e 3c2f  al. (2014)</a></
+000036a0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+000036b0: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+000036c0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000036d0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000036e0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000036f0: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+00003700: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+00003710: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00003720: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003730: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003740: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00003750: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003760: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003770: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003780: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003790: 7061 6464 696e 673a 2038 7078 3b22 3e52  padding: 8px;">R
+000037a0: 4444 4d3c 2f74 643e 0a20 2020 203c 7464  DDM</td>.    <td
+000037b0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+000037c0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+000037d0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000037e0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000037f0: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
+00003800: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
+00003810: 3031 362f 6a2e 6573 7761 2e32 3031 372e  016/j.eswa.2017.
+00003820: 3038 2e30 3233 223e 4261 7272 6f73 2065  08.023">Barros e
+00003830: 7420 616c 2e20 2832 3031 3729 3c2f 613e  t al. (2017)</a>
+00003840: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
+00003850: 3c74 723e 0a20 2020 203c 7464 2072 6f77  <tr>.    <td row
+00003860: 7370 616e 3d22 3322 2073 7479 6c65 3d22  span="3" style="
+00003870: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003880: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003890: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000038a0: 696e 673a 2038 7078 3b22 3e57 696e 646f  ing: 8px;">Windo
+000038b0: 7720 6261 7365 643c 2f74 643e 0a20 2020  w based</td>.   
+000038c0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+000038d0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+000038e0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+000038f0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00003900: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
+00003910: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00003920: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00003930: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00003940: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00003950: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
+00003960: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00003970: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00003980: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00003990: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000039a0: 673a 2038 7078 3b22 3e41 4457 494e 3c2f  g: 8px;">ADWIN</
+000039b0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000039c0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000039d0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000039e0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000039f0: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
+00003a00: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00003a10: 6f69 2e6f 7267 2f31 302e 3131 3337 2f31  oi.org/10.1137/1
+00003a20: 2e39 3738 3136 3131 3937 3237 3731 2e34  .9781611972771.4
+00003a30: 3222 3e42 6966 6574 2061 6e64 2047 6176  2">Bifet and Gav
+00003a40: 616c 6461 2028 3230 3037 293c 2f61 3e3c  alda (2007)</a><
+00003a50: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00003a60: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
+00003a70: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00003a80: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003a90: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003aa0: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
+00003ab0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003ac0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003ad0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003ae0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003af0: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
+00003b00: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00003b10: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00003b20: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00003b30: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00003b40: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00003b50: 4b53 5749 4e3c 2f74 643e 0a20 2020 203c  KSWIN</td>.    <
+00003b60: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00003b70: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00003b80: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00003b90: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00003ba0: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+00003bb0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00003bc0: 2e31 3031 362f 6a2e 6e65 7563 6f6d 2e32  .1016/j.neucom.2
+00003bd0: 3031 392e 3131 2e31 3131 223e 5261 6162  019.11.111">Raab
+00003be0: 2065 7420 616c 2e20 2832 3032 3029 3c2f   et al. (2020)</
+00003bf0: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
+00003c00: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
+00003c10: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003c20: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003c30: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003c40: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003c50: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
+00003c60: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003c70: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003c80: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003c90: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003ca0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
+00003cb0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00003cc0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00003cd0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00003ce0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00003cf0: 3b22 3e53 5445 5044 3c2f 7464 3e0a 2020  ;">STEPD</td>.  
+00003d00: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00003d10: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00003d20: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00003d30: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00003d40: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00003d50: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00003d60: 2f31 302e 3130 3037 2f39 3738 2d33 2d35  /10.1007/978-3-5
+00003d70: 3430 2d37 3534 3838 2d36 5f32 3722 3e4e  40-75488-6_27">N
+00003d80: 6973 6869 6461 2061 6e64 2059 616d 6175  ishida and Yamau
+00003d90: 6368 6920 2832 3030 3729 3c2f 613e 3c2f  chi (2007)</a></
+00003da0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00003db0: 723e 0a20 2020 203c 7464 2072 6f77 7370  r>.    <td rowsp
+00003dc0: 616e 3d22 3136 2220 7374 796c 653d 2274  an="16" style="t
+00003dd0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00003de0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00003df0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00003e00: 6e67 3a20 3870 783b 223e 4461 7461 2064  ng: 8px;">Data d
+00003e10: 7269 6674 3c2f 7464 3e0a 2020 2020 3c74  rift</td>.    <t
+00003e20: 6420 726f 7773 7061 6e3d 2231 3422 2073  d rowspan="14" s
+00003e30: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003e40: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003e50: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003e60: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003e70: 3e42 6174 6368 3c2f 7464 3e0a 2020 2020  >Batch</td>.    
+00003e80: 3c74 6420 726f 7773 7061 6e3d 2239 2220  <td rowspan="9" 
+00003e90: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003ea0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003eb0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003ec0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003ed0: 223e 4469 7374 616e 6365 2062 6173 6564  ">Distance based
+00003ee0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00003ef0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00003f00: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00003f10: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00003f20: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00003f30: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00003f40: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003f50: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003f60: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003f70: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003f80: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+00003f90: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003fa0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003fb0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003fc0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003fd0: 223e 416e 6465 7273 6f6e 2d44 6172 6c69  ">Anderson-Darli
+00003fe0: 6e67 2074 6573 743c 2f74 643e 0a20 2020  ng test</td>.   
+00003ff0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00004000: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00004010: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00004020: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004030: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
+00004040: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00004050: 3130 2e32 3330 372f 3232 3838 3830 3522  10.2307/2288805"
+00004060: 3e53 6368 6f6c 7a20 616e 6420 5374 6570  >Scholz and Step
+00004070: 6865 6e73 2028 3139 3837 293c 2f61 3e3c  hens (1987)</a><
+00004080: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00004090: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
+000040a0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000040b0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000040c0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000040d0: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
+000040e0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+000040f0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004100: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004110: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004120: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
+00004130: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00004140: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00004150: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00004160: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00004170: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004180: 4268 6174 7461 6368 6172 7979 6120 6469  Bhattacharyya di
+00004190: 7374 616e 6365 3c2f 7464 3e0a 2020 2020  stance</td>.    
+000041a0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+000041b0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+000041c0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+000041d0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+000041e0: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
+000041f0: 7474 7073 3a2f 2f77 7777 2e6a 7374 6f72  ttps://www.jstor
+00004200: 2e6f 7267 2f73 7461 626c 652f 3235 3034  .org/stable/2504
+00004210: 3738 3832 223e 4268 6174 7461 6368 6172  7882">Bhattachar
+00004220: 7979 6120 2831 3934 3629 3c2f 613e 3c2f  yya (1946)</a></
+00004230: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00004240: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+00004250: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00004260: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00004270: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00004280: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+00004290: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000042a0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000042b0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000042c0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000042d0: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+000042e0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+000042f0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004300: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004310: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004320: 7061 6464 696e 673a 2038 7078 3b22 3e45  padding: 8px;">E
+00004330: 6172 7468 204d 6f76 6572 2773 2064 6973  arth Mover's dis
+00004340: 7461 6e63 653c 2f74 643e 0a20 2020 203c  tance</td>.    <
+00004350: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004360: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004370: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004380: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004390: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+000043a0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+000043b0: 2e31 3032 332f 413a 3130 3236 3534 3339  .1023/A:10265439
+000043c0: 3030 3035 3422 3e52 7562 6e65 7220 6574  00054">Rubner et
+000043d0: 2061 6c2e 2028 3230 3030 293c 2f61 3e3c   al. (2000)</a><
 000043e0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
 000043f0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
 00004400: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
 00004410: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
 00004420: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
 00004430: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
 00004440: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
@@ -1096,284 +1096,478 @@
 00004470: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
 00004480: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
 00004490: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
 000044a0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
 000044b0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
 000044c0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
 000044d0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000044e0: 4372 616d c3a9 722d 766f 6e20 4d69 7365  Cram..r-von Mise
-000044f0: 7320 7465 7374 3c2f 7464 3e0a 2020 2020  s test</td>.    
-00004500: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00004510: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00004520: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00004530: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00004540: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-00004550: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00004560: 302e 3130 3830 2f30 3334 3631 3233 382e  0.1080/03461238.
-00004570: 3139 3238 2e31 3034 3136 3836 3222 3e43  1928.10416862">C
-00004580: 7261 6dc3 a972 2028 3139 3032 293c 2f61  ram..r (1902)</a
-00004590: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
-000045a0: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
-000045b0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000045c0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-000045d0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000045e0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000045f0: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
-00004600: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004610: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004620: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004630: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004640: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
-00004650: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00004660: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00004670: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00004680: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00004690: 223e 4b6f 6c6d 6f67 6f72 6f76 2d53 6d69  ">Kolmogorov-Smi
-000046a0: 726e 6f76 2074 6573 743c 2f74 643e 0a20  rnov test</td>. 
-000046b0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000046c0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000046d0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000046e0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000046f0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-00004700: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-00004710: 672f 3130 2e32 3330 372f 3232 3830 3039  g/10.2307/228009
-00004720: 3522 3e4d 6173 7365 7920 4a72 2028 3139  5">Massey Jr (19
-00004730: 3531 293c 2f61 3e3c 2f74 643e 0a20 203c  51)</a></td>.  <
-00004740: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
-00004750: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00004760: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00004770: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00004780: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00004790: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
-000047a0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-000047b0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-000047c0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-000047d0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-000047e0: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
-000047f0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00004800: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00004810: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00004820: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00004830: 3a20 3870 783b 223e 4d61 6e6e 2d57 6869  : 8px;">Mann-Whi
-00004840: 746e 6579 2055 2074 6573 743c 2f74 643e  tney U test</td>
-00004850: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004860: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004870: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004880: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004890: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
-000048a0: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
-000048b0: 6f72 672f 3130 2e31 3231 342f 616f 6d73  org/10.1214/aoms
-000048c0: 2f31 3137 3737 3330 3439 3122 3e4d 616e  /1177730491">Man
-000048d0: 6e20 616e 6420 5768 6974 6e65 7920 2831  n and Whitney (1
-000048e0: 3934 3729 3c2f 613e 3c2f 7464 3e0a 2020  947)</a></td>.  
-000048f0: 3c2f 7472 3e0a 2020 3c74 723e 0a20 2020  </tr>.  <tr>.   
-00004900: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00004910: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00004920: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00004930: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00004940: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
-00004950: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00004960: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00004970: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00004980: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00004990: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
-000049a0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000049b0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000049c0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000049d0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000049e0: 673a 2038 7078 3b22 3e57 656c 6368 2773  g: 8px;">Welch's
-000049f0: 2074 2d74 6573 743c 2f74 643e 0a20 2020   t-test</td>.   
-00004a00: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00004a10: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00004a20: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00004a30: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00004a40: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
-00004a50: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
-00004a60: 3130 2e32 3330 372f 3233 3332 3531 3022  10.2307/2332510"
-00004a70: 3e57 656c 6368 2028 3139 3437 293c 2f61  >Welch (1947)</a
-00004a80: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
-00004a90: 203c 7472 3e0a 2020 2020 3c74 6420 726f   <tr>.    <td ro
-00004aa0: 7773 7061 6e3d 2232 2220 7374 796c 653d  wspan="2" style=
-00004ab0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00004ac0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00004ad0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00004ae0: 6469 6e67 3a20 3870 783b 223e 5374 7265  ding: 8px;">Stre
-00004af0: 616d 696e 673c 2f74 643e 0a20 2020 203c  aming</td>.    <
-00004b00: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00004b10: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00004b20: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00004b30: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00004b40: 7078 3b22 3e44 6973 7461 6e63 6520 6261  px;">Distance ba
-00004b50: 7365 643c 2f74 643e 0a20 2020 203c 7464  sed</td>.    <td
-00004b60: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004b70: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004b80: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004b90: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004ba0: 3b22 3e4d 3c2f 7464 3e0a 2020 2020 3c74  ;">M</td>.    <t
-00004bb0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00004bc0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00004bd0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00004be0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00004bf0: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
-00004c00: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00004c10: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00004c20: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00004c30: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00004c40: 7078 3b22 3e4d 4d44 3c2f 7464 3e0a 2020  px;">MMD</td>.  
-00004c50: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00004c60: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00004c70: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00004c80: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00004c90: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
-00004ca0: 2268 7474 7073 3a2f 2f64 6c2e 6163 6d2e  "https://dl.acm.
-00004cb0: 6f72 672f 646f 692f 3130 2e35 3535 352f  org/doi/10.5555/
-00004cc0: 3231 3838 3338 352e 3231 3838 3431 3022  2188385.2188410"
-00004cd0: 3e47 7265 7474 6f6e 2065 7420 616c 2e20  >Gretton et al. 
-00004ce0: 2832 3031 3229 3c2f 613e 3c2f 7464 3e0a  (2012)</a></td>.
-00004cf0: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
-00004d00: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00004d10: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00004d20: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00004d30: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00004d40: 673a 2038 7078 3b22 3e53 7461 7469 7374  g: 8px;">Statist
-00004d50: 6963 616c 2074 6573 743c 2f74 643e 0a20  ical test</td>. 
-00004d60: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00004d70: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00004d80: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00004d90: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00004da0: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
-00004db0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00004dc0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00004dd0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004de0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004df0: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
-00004e00: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004e10: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004e20: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004e30: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004e40: 696e 673a 2038 7078 3b22 3e49 6e63 7265  ing: 8px;">Incre
-00004e50: 6d65 6e74 616c 204b 6f6c 6d6f 676f 726f  mental Kolmogoro
-00004e60: 762d 536d 6972 6e6f 7620 7465 7374 3c2f  v-Smirnov test</
-00004e70: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00004e80: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00004e90: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00004ea0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00004eb0: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
-00004ec0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-00004ed0: 6f69 2e6f 7267 2f31 302e 3131 3435 2f32  oi.org/10.1145/2
-00004ee0: 3933 3936 3732 2e32 3933 3938 3336 223e  939672.2939836">
-00004ef0: 646f 7320 5265 6973 2065 7420 616c 2e20  dos Reis et al. 
-00004f00: 2832 3031 3629 3c2f 613e 3c2f 7464 3e0a  (2016)</a></td>.
-00004f10: 2020 3c2f 7472 3e0a 3c2f 7462 6f64 793e    </tr>.</tbody>
-00004f20: 0a3c 2f74 6162 6c65 3e0a 0a23 2320 e29d  .</table>..## ..
-00004f30: 9720 5768 6174 2069 7320 616e 6420 7768  . What is and wh
-00004f40: 6174 2069 7320 6e6f 7420 4672 6f75 726f  at is not Frouro
-00004f50: 733f 0a0a 556e 6c69 6b65 206f 7468 6572  s?..Unlike other
-00004f60: 206c 6962 7261 7269 6573 2074 6861 7420   libraries that 
-00004f70: 696e 2061 6464 6974 696f 6e20 746f 2070  in addition to p
-00004f80: 726f 7669 6465 2064 7269 6674 2064 6574  rovide drift det
-00004f90: 6563 7469 6f6e 2061 6c67 6f72 6974 686d  ection algorithm
-00004fa0: 732c 2069 6e63 6c75 6465 206f 7468 6572  s, include other
-00004fb0: 2066 756e 6374 696f 6e61 6c69 7469 6573   functionalities
-00004fc0: 2073 7563 6820 6173 2061 6e6f 6d61 6c79   such as anomaly
-00004fd0: 2f6f 7574 6c69 6572 2064 6574 6563 7469  /outlier detecti
-00004fe0: 6f6e 2c20 6164 7665 7273 6172 6961 6c20  on, adversarial 
-00004ff0: 6465 7465 6374 696f 6e2c 2069 6d62 616c  detection, imbal
-00005000: 616e 6365 206c 6561 726e 696e 672c 2061  ance learning, a
-00005010: 6d6f 6e67 206f 7468 6572 732c 2046 726f  mong others, Fro
-00005020: 7572 6f73 2068 6173 2061 6e64 2077 696c  uros has and wil
-00005030: 6c20 2a2a 4f4e 4c59 2a2a 2068 6176 6520  l **ONLY** have 
-00005040: 6f6e 6520 7075 7270 6f73 653a 202a 2a64  one purpose: **d
-00005050: 7269 6674 2064 6574 6563 7469 6f6e 2a2a  rift detection**
-00005060: 2e0a 0a57 6520 6669 726d 6c79 2062 656c  ...We firmly bel
-00005070: 6965 7665 2074 6861 7420 6d61 6368 696e  ieve that machin
-00005080: 6520 6c65 6172 6e69 6e67 2072 656c 6174  e learning relat
-00005090: 6564 206c 6962 7261 7269 6573 206f 7220  ed libraries or 
-000050a0: 6672 616d 6577 6f72 6b73 2073 686f 756c  frameworks shoul
-000050b0: 6420 6e6f 7420 666f 6c6c 6f77 205b 4a61  d not follow [Ja
-000050c0: 636b 206f 6620 616c 6c20 7472 6164 6573  ck of all trades
-000050d0: 2c20 6d61 7374 6572 206f 6620 6e6f 6e65  , master of none
-000050e0: 5d28 6874 7470 733a 2f2f 656e 2e77 696b  ](https://en.wik
-000050f0: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00005100: 4a61 636b 5f6f 665f 616c 6c5f 7472 6164  Jack_of_all_trad
-00005110: 6573 2c5f 6d61 7374 6572 5f6f 665f 6e6f  es,_master_of_no
-00005120: 6e65 2920 7072 696e 6369 706c 652e 2049  ne) principle. I
-00005130: 6e73 7465 6164 2c20 7468 6579 2073 686f  nstead, they sho
-00005140: 756c 6420 6265 2066 6f63 7573 6564 206f  uld be focused o
-00005150: 6e20 6120 7369 6e67 6c65 2074 6173 6b20  n a single task 
-00005160: 616e 6420 646f 2069 7420 7765 6c6c 2e0a  and do it well..
-00005170: 0a23 2320 e29c 8520 5768 6f20 6973 2075  .## ... Who is u
-00005180: 7369 6e67 2046 726f 7572 6f73 3f0a 0a46  sing Frouros?..F
-00005190: 726f 7572 6f73 2069 7320 6163 7469 7665  rouros is active
-000051a0: 6c79 2062 6569 6e67 2075 7365 6420 6279  ly being used by
-000051b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-000051c0: 726f 6a65 6374 7320 746f 2069 6d70 6c65  rojects to imple
-000051d0: 6d65 6e74 2064 7269 6674 0a64 6574 6563  ment drift.detec
-000051e0: 7469 6f6e 2069 6e20 6d61 6368 696e 6520  tion in machine 
-000051f0: 6c65 6172 6e69 6e67 2070 6970 656c 696e  learning pipelin
-00005200: 6573 3a0a 0a20 2a20 5b41 4934 454f 5343  es:.. * [AI4EOSC
-00005210: 5d28 6874 7470 733a 2f2f 6169 3465 6f73  ](https://ai4eos
-00005220: 632e 6575 292e 0a20 2a20 5b69 4d61 6769  c.eu).. * [iMagi
-00005230: 6e65 5d28 6874 7470 733a 2f2f 696d 6167  ne](https://imag
-00005240: 696e 652d 6169 2e65 7529 2e0a 0a49 6620  ine-ai.eu)...If 
-00005250: 796f 7520 7761 6e74 2079 6f75 7220 7072  you want your pr
-00005260: 6f6a 6563 7420 6c69 7374 6564 2068 6572  oject listed her
-00005270: 652c 2064 6f20 6e6f 7420 6865 7369 7461  e, do not hesita
-00005280: 7465 2074 6f20 7365 6e64 2075 7320 6120  te to send us a 
-00005290: 7075 6c6c 2072 6571 7565 7374 2e0a 0a23  pull request...#
-000052a0: 2320 f09f 918d 2043 6f6e 7472 6962 7574  # .... Contribut
-000052b0: 696e 670a 0a43 6865 636b 206f 7574 2074  ing..Check out t
-000052c0: 6865 205b 636f 6e74 7269 6275 7469 6f6e  he [contribution
-000052d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000052e0: 2e63 6f6d 2f49 4643 412f 6672 6f75 726f  .com/IFCA/frouro
-000052f0: 732f 626c 6f62 2f6d 6169 6e2f 434f 4e54  s/blob/main/CONT
-00005300: 5249 4255 5449 4e47 2e6d 6429 2073 6563  RIBUTING.md) sec
-00005310: 7469 6f6e 2e0a 0a23 2320 f09f 92ac 2043  tion...## .... C
-00005320: 6974 6174 696f 6e0a 0a41 6c74 686f 7567  itation..Althoug
-00005330: 6820 4672 6f75 726f 7320 7061 7065 7220  h Frouros paper 
-00005340: 6973 2073 7469 6c6c 2069 6e20 7072 6570  is still in prep
-00005350: 7269 6e74 2c20 6966 2079 6f75 2077 616e  rint, if you wan
-00005360: 7420 746f 2063 6974 6520 6974 2079 6f75  t to cite it you
-00005370: 2063 616e 2075 7365 2074 6865 205b 7072   can use the [pr
-00005380: 6570 7269 6e74 5d28 6874 7470 733a 2f2f  eprint](https://
-00005390: 6172 7869 762e 6f72 672f 6162 732f 3232  arxiv.org/abs/22
-000053a0: 3038 2e30 3638 3638 2920 7665 7273 696f  08.06868) versio
-000053b0: 6e20 2874 6f20 6265 2072 6570 6c61 6365  n (to be replace
-000053c0: 6420 6279 2074 6865 2070 6170 6572 206f  d by the paper o
-000053d0: 6e63 6520 6973 2070 7562 6c69 7368 6564  nce is published
-000053e0: 292e 0a0a 6060 6062 6962 7465 780a 4061  )...```bibtex.@a
-000053f0: 7274 6963 6c65 7b63 6573 7065 6465 7332  rticle{cespedes2
-00005400: 3032 3266 726f 7572 6f73 2c0a 2020 7469  022frouros,.  ti
-00005410: 746c 653d 7b46 726f 7572 6f73 3a20 4120  tle={Frouros: A 
-00005420: 5079 7468 6f6e 206c 6962 7261 7279 2066  Python library f
-00005430: 6f72 2064 7269 6674 2064 6574 6563 7469  or drift detecti
-00005440: 6f6e 2069 6e20 6d61 6368 696e 6520 6c65  on in machine le
-00005450: 6172 6e69 6e67 2073 7973 7465 6d73 7d2c  arning systems},
-00005460: 0a20 2061 7574 686f 723d 7b43 7b5c 2765  .  author={C{\'e
-00005470: 7d73 7065 6465 732d 5369 736e 6965 6761  }spedes-Sisniega
-00005480: 2c20 4a61 696d 6520 616e 6420 4c7b 5c27  , Jaime and L{\'
-00005490: 6f7d 7065 7a2d 4761 7263 7b5c 275c 697d  o}pez-Garc{\'\i}
-000054a0: 612c 207b 5c27 417d 6c76 6172 6f20 7d2c  a, {\'A}lvaro },
-000054b0: 0a20 206a 6f75 726e 616c 3d7b 6172 5869  .  journal={arXi
-000054c0: 7620 7072 6570 7269 6e74 2061 7258 6976  v preprint arXiv
-000054d0: 3a32 3230 382e 3036 3836 387d 2c0a 2020  :2208.06868},.  
-000054e0: 7965 6172 3d7b 3230 3232 7d0a 7d0a 6060  year={2022}.}.``
-000054f0: 600a 0a23 2320 f09f 939d 204c 6963 656e  `..## .... Licen
-00005500: 7365 0a0a 4672 6f75 726f 7320 6973 2061  se..Frouros is a
-00005510: 6e20 6f70 656e 2d73 6f75 7263 6520 736f  n open-source so
-00005520: 6674 7761 7265 206c 6963 656e 7365 6420  ftware licensed 
-00005530: 756e 6465 7220 7468 6520 5b42 5344 2d33  under the [BSD-3
-00005540: 2d43 6c61 7573 6520 6c69 6365 6e73 655d  -Clause license]
-00005550: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00005560: 636f 6d2f 4946 4341 2f66 726f 7572 6f73  com/IFCA/frouros
-00005570: 2f62 6c6f 622f 6d61 696e 2f4c 4943 454e  /blob/main/LICEN
-00005580: 5345 292e 0a0a 2323 20f0 9f99 8f20 4163  SE)...## .... Ac
-00005590: 6b6e 6f77 6c65 6467 656d 656e 7473 0a0a  knowledgements..
-000055a0: 4672 6f75 726f 7320 6861 7320 7265 6365  Frouros has rece
-000055b0: 6976 6564 2066 756e 6469 6e67 2066 726f  ived funding fro
-000055c0: 6d20 7468 6520 4167 656e 6369 6120 4573  m the Agencia Es
-000055d0: 7461 7461 6c20 6465 2049 6e76 6573 7469  tatal de Investi
-000055e0: 6761 6369 c3b3 6e2c 2055 6e69 6461 6420  gaci..n, Unidad 
-000055f0: 6465 2045 7863 656c 656e 6369 6120 4d61  de Excelencia Ma
-00005600: 72c3 ad61 2064 6520 4d61 657a 7475 2c20  r..a de Maeztu, 
-00005610: 7265 662e 204d 444d 2d32 3031 372d 3037  ref. MDM-2017-07
-00005620: 3635 2e0a                                65..
+000044e0: 4865 6c6c 696e 6765 7220 6469 7374 616e  Hellinger distan
+000044f0: 6365 3c2f 7464 3e0a 2020 2020 3c74 6420  ce</td>.    <td 
+00004500: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00004510: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00004520: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00004530: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00004540: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00004550: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3135  ://doi.org/10.15
+00004560: 3135 2f43 524c 4c2e 3139 3039 2e31 3336  15/CRLL.1909.136
+00004570: 2e32 3130 223e 4865 6c6c 696e 6765 7220  .210">Hellinger 
+00004580: 2831 3930 3929 3c2f 613e 3c2f 7464 3e0a  (1909)</a></td>.
+00004590: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
+000045a0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+000045b0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000045c0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000045d0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000045e0: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
+000045f0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00004600: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004610: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00004620: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004630: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
+00004640: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00004650: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00004660: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00004670: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00004680: 696e 673a 2038 7078 3b22 3e48 6973 746f  ing: 8px;">Histo
+00004690: 6772 616d 2069 6e74 6572 7365 6374 696f  gram intersectio
+000046a0: 6e20 6e6f 726d 616c 697a 6564 2063 6f6d  n normalized com
+000046b0: 706c 656d 656e 743c 2f74 643e 0a20 2020  plement</td>.   
+000046c0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+000046d0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+000046e0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+000046f0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004700: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
+00004710: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00004720: 3130 2e31 3030 372f 4246 3030 3133 3034  10.1007/BF001304
+00004730: 3837 223e 5377 6169 6e20 616e 6420 4261  87">Swain and Ba
+00004740: 6c6c 6172 6420 2831 3939 3129 3c2f 613e  llard (1991)</a>
+00004750: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
+00004760: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
+00004770: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004780: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004790: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+000047a0: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
+000047b0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+000047c0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+000047d0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+000047e0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+000047f0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004800: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
+00004810: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00004820: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00004830: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00004840: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00004850: 3e4a 656e 7365 6e2d 5368 616e 6e6f 6e20  >Jensen-Shannon 
+00004860: 6469 7374 616e 6365 3c2f 7464 3e0a 2020  distance</td>.  
+00004870: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004880: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004890: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000048a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000048b0: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+000048c0: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+000048d0: 2f31 302e 3131 3039 2f31 382e 3631 3131  /10.1109/18.6111
+000048e0: 3522 3e4c 696e 2028 3139 3931 293c 2f61  5">Lin (1991)</a
+000048f0: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+00004900: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
+00004910: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00004920: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00004930: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00004940: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004950: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00004960: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00004970: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00004980: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00004990: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+000049a0: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+000049b0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000049c0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000049d0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000049e0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+000049f0: 223e 4b75 6c6c 6261 636b 2d4c 6569 626c  ">Kullback-Leibl
+00004a00: 6572 2064 6976 6572 6765 6e63 653c 2f74  er divergence</t
+00004a10: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00004a20: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00004a30: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00004a40: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00004a50: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
+00004a60: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+00004a70: 692e 6f72 672f 3130 2e31 3231 342f 616f  i.org/10.1214/ao
+00004a80: 6d73 2f31 3137 3737 3239 3639 3422 3e4b  ms/1177729694">K
+00004a90: 756c 6c62 6163 6b20 616e 6420 4c65 6962  ullback and Leib
+00004aa0: 6c65 7220 2831 3935 3129 3c2f 613e 3c2f  ler (1951)</a></
+00004ab0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00004ac0: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+00004ad0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00004ae0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00004af0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00004b00: 6464 696e 673a 2038 7078 3b22 3e4d 3c2f  dding: 8px;">M</
+00004b10: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+00004b20: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00004b30: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00004b40: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00004b50: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00004b60: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00004b70: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004b80: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004b90: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004ba0: 7061 6464 696e 673a 2038 7078 3b22 3e4d  padding: 8px;">M
+00004bb0: 4d44 3c2f 7464 3e0a 2020 2020 3c74 6420  MD</td>.    <td 
+00004bc0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00004bd0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00004be0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00004bf0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00004c00: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00004c10: 3a2f 2f64 6c2e 6163 6d2e 6f72 672f 646f  ://dl.acm.org/do
+00004c20: 692f 3130 2e35 3535 352f 3231 3838 3338  i/10.5555/218838
+00004c30: 352e 3231 3838 3431 3022 3e47 7265 7474  5.2188410">Grett
+00004c40: 6f6e 2065 7420 616c 2e20 2832 3031 3229  on et al. (2012)
+00004c50: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
+00004c60: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
+00004c70: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00004c80: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00004c90: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00004ca0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00004cb0: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
+00004cc0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00004cd0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00004ce0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00004cf0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00004d00: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
+00004d10: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004d20: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004d30: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004d40: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004d50: 7078 3b22 3e50 5349 3c2f 7464 3e0a 2020  px;">PSI</td>.  
+00004d60: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004d70: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004d80: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00004d90: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00004da0: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00004db0: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00004dc0: 2f31 302e 3130 3537 2f6a 6f72 732e 3230  /10.1057/jors.20
+00004dd0: 3038 2e31 3434 223e 5775 2061 6e64 204f  08.144">Wu and O
+00004de0: 6c73 6f6e 2028 3230 3130 293c 2f61 3e3c  lson (2010)</a><
+00004df0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00004e00: 7472 3e0a 2020 2020 3c74 6420 726f 7773  tr>.    <td rows
+00004e10: 7061 6e3d 2235 2220 7374 796c 653d 2274  pan="5" style="t
+00004e20: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004e30: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00004e40: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004e50: 6e67 3a20 3870 783b 223e 5374 6174 6973  ng: 8px;">Statis
+00004e60: 7469 6361 6c20 7465 7374 3c2f 7464 3e0a  tical test</td>.
+00004e70: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00004e80: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004e90: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00004ea0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004eb0: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
+00004ec0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00004ed0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00004ee0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00004ef0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00004f00: 696e 673a 2038 7078 3b22 3e43 3c2f 7464  ing: 8px;">C</td
+00004f10: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00004f20: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00004f30: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00004f40: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00004f50: 6469 6e67 3a20 3870 783b 223e 4368 692d  ding: 8px;">Chi-
+00004f60: 7371 7561 7265 2074 6573 743c 2f74 643e  square test</td>
+00004f70: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00004f80: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00004f90: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00004fa0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00004fb0: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
+00004fc0: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
+00004fd0: 6f72 672f 3130 2e31 3038 302f 3134 3738  org/10.1080/1478
+00004fe0: 3634 3430 3030 3934 3633 3839 3722 3e50  6440009463897">P
+00004ff0: 6561 7273 6f6e 2028 3139 3030 293c 2f61  earson (1900)</a
+00005000: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+00005010: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
+00005020: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00005030: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00005040: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00005050: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00005060: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00005070: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00005080: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00005090: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+000050a0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+000050b0: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+000050c0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000050d0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000050e0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000050f0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00005100: 223e 4372 616d c3a9 722d 766f 6e20 4d69  ">Cram..r-von Mi
+00005110: 7365 7320 7465 7374 3c2f 7464 3e0a 2020  ses test</td>.  
+00005120: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00005130: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00005140: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00005150: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00005160: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00005170: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00005180: 2f31 302e 3130 3830 2f30 3334 3631 3233  /10.1080/0346123
+00005190: 382e 3139 3238 2e31 3034 3136 3836 3222  8.1928.10416862"
+000051a0: 3e43 7261 6dc3 a972 2028 3139 3032 293c  >Cram..r (1902)<
+000051b0: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
+000051c0: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
+000051d0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000051e0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000051f0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00005200: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00005210: 223e 553c 2f74 643e 0a20 2020 203c 7464  ">U</td>.    <td
+00005220: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00005230: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00005240: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00005250: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00005260: 3b22 3e4e 3c2f 7464 3e0a 2020 2020 3c74  ;">N</td>.    <t
+00005270: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00005280: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00005290: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+000052a0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+000052b0: 783b 223e 4b6f 6c6d 6f67 6f72 6f76 2d53  x;">Kolmogorov-S
+000052c0: 6d69 726e 6f76 2074 6573 743c 2f74 643e  mirnov test</td>
+000052d0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+000052e0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000052f0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00005300: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00005310: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
+00005320: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
+00005330: 6f72 672f 3130 2e32 3330 372f 3232 3830  org/10.2307/2280
+00005340: 3039 3522 3e4d 6173 7365 7920 4a72 2028  095">Massey Jr (
+00005350: 3139 3531 293c 2f61 3e3c 2f74 643e 0a20  1951)</a></td>. 
+00005360: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
+00005370: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00005380: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00005390: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000053a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000053b0: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
+000053c0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+000053d0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000053e0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000053f0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00005400: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
+00005410: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00005420: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00005430: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00005440: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00005450: 6e67 3a20 3870 783b 223e 4d61 6e6e 2d57  ng: 8px;">Mann-W
+00005460: 6869 746e 6579 2055 2074 6573 743c 2f74  hitney U test</t
+00005470: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00005480: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00005490: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000054a0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000054b0: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
+000054c0: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+000054d0: 692e 6f72 672f 3130 2e31 3231 342f 616f  i.org/10.1214/ao
+000054e0: 6d73 2f31 3137 3737 3330 3439 3122 3e4d  ms/1177730491">M
+000054f0: 616e 6e20 616e 6420 5768 6974 6e65 7920  ann and Whitney 
+00005500: 2831 3934 3729 3c2f 613e 3c2f 7464 3e0a  (1947)</a></td>.
+00005510: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
+00005520: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00005530: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00005540: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00005550: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00005560: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
+00005570: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00005580: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00005590: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000055a0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000055b0: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
+000055c0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+000055d0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000055e0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+000055f0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00005600: 696e 673a 2038 7078 3b22 3e57 656c 6368  ing: 8px;">Welch
+00005610: 2773 2074 2d74 6573 743c 2f74 643e 0a20  's t-test</td>. 
+00005620: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00005630: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00005640: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00005650: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00005660: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
+00005670: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+00005680: 672f 3130 2e32 3330 372f 3233 3332 3531  g/10.2307/233251
+00005690: 3022 3e57 656c 6368 2028 3139 3437 293c  0">Welch (1947)<
+000056a0: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
+000056b0: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
+000056c0: 726f 7773 7061 6e3d 2232 2220 7374 796c  rowspan="2" styl
+000056d0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000056e0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000056f0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00005700: 6164 6469 6e67 3a20 3870 783b 223e 5374  adding: 8px;">St
+00005710: 7265 616d 696e 673c 2f74 643e 0a20 2020  reaming</td>.   
+00005720: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00005730: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00005740: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00005750: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00005760: 2038 7078 3b22 3e44 6973 7461 6e63 6520   8px;">Distance 
+00005770: 6261 7365 643c 2f74 643e 0a20 2020 203c  based</td>.    <
+00005780: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00005790: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+000057a0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+000057b0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+000057c0: 7078 3b22 3e4d 3c2f 7464 3e0a 2020 2020  px;">M</td>.    
+000057d0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+000057e0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+000057f0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00005800: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00005810: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
+00005820: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00005830: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00005840: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00005850: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00005860: 2038 7078 3b22 3e4d 4d44 3c2f 7464 3e0a   8px;">MMD</td>.
+00005870: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00005880: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00005890: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000058a0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000058b0: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
+000058c0: 663d 2268 7474 7073 3a2f 2f64 6c2e 6163  f="https://dl.ac
+000058d0: 6d2e 6f72 672f 646f 692f 3130 2e35 3535  m.org/doi/10.555
+000058e0: 352f 3231 3838 3338 352e 3231 3838 3431  5/2188385.218841
+000058f0: 3022 3e47 7265 7474 6f6e 2065 7420 616c  0">Gretton et al
+00005900: 2e20 2832 3031 3229 3c2f 613e 3c2f 7464  . (2012)</a></td
+00005910: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+00005920: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00005930: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00005940: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00005950: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00005960: 696e 673a 2038 7078 3b22 3e53 7461 7469  ing: 8px;">Stati
+00005970: 7374 6963 616c 2074 6573 743c 2f74 643e  stical test</td>
+00005980: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00005990: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000059a0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+000059b0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000059c0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
+000059d0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+000059e0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+000059f0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00005a00: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00005a10: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
+00005a20: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00005a30: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00005a40: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00005a50: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00005a60: 6464 696e 673a 2038 7078 3b22 3e49 6e63  dding: 8px;">Inc
+00005a70: 7265 6d65 6e74 616c 204b 6f6c 6d6f 676f  remental Kolmogo
+00005a80: 726f 762d 536d 6972 6e6f 7620 7465 7374  rov-Smirnov test
+00005a90: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00005aa0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00005ab0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00005ac0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00005ad0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00005ae0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00005af0: 2f64 6f69 2e6f 7267 2f31 302e 3131 3435  /doi.org/10.1145
+00005b00: 2f32 3933 3936 3732 2e32 3933 3938 3336  /2939672.2939836
+00005b10: 223e 646f 7320 5265 6973 2065 7420 616c  ">dos Reis et al
+00005b20: 2e20 2832 3031 3629 3c2f 613e 3c2f 7464  . (2016)</a></td
+00005b30: 3e0a 2020 3c2f 7472 3e0a 3c2f 7462 6f64  >.  </tr>.</tbod
+00005b40: 793e 0a3c 2f74 6162 6c65 3e0a 0a23 2320  y>.</table>..## 
+00005b50: e29d 9720 5768 6174 2069 7320 616e 6420  ... What is and 
+00005b60: 7768 6174 2069 7320 6e6f 7420 4672 6f75  what is not Frou
+00005b70: 726f 733f 0a0a 556e 6c69 6b65 206f 7468  ros?..Unlike oth
+00005b80: 6572 206c 6962 7261 7269 6573 2074 6861  er libraries tha
+00005b90: 7420 696e 2061 6464 6974 696f 6e20 746f  t in addition to
+00005ba0: 2070 726f 7669 6465 2064 7269 6674 2064   provide drift d
+00005bb0: 6574 6563 7469 6f6e 2061 6c67 6f72 6974  etection algorit
+00005bc0: 686d 732c 2069 6e63 6c75 6465 206f 7468  hms, include oth
+00005bd0: 6572 2066 756e 6374 696f 6e61 6c69 7469  er functionaliti
+00005be0: 6573 2073 7563 6820 6173 2061 6e6f 6d61  es such as anoma
+00005bf0: 6c79 2f6f 7574 6c69 6572 2064 6574 6563  ly/outlier detec
+00005c00: 7469 6f6e 2c20 6164 7665 7273 6172 6961  tion, adversaria
+00005c10: 6c20 6465 7465 6374 696f 6e2c 2069 6d62  l detection, imb
+00005c20: 616c 616e 6365 206c 6561 726e 696e 672c  alance learning,
+00005c30: 2061 6d6f 6e67 206f 7468 6572 732c 2046   among others, F
+00005c40: 726f 7572 6f73 2068 6173 2061 6e64 2077  rouros has and w
+00005c50: 696c 6c20 2a2a 4f4e 4c59 2a2a 2068 6176  ill **ONLY** hav
+00005c60: 6520 6f6e 6520 7075 7270 6f73 653a 202a  e one purpose: *
+00005c70: 2a64 7269 6674 2064 6574 6563 7469 6f6e  *drift detection
+00005c80: 2a2a 2e0a 0a57 6520 6669 726d 6c79 2062  **...We firmly b
+00005c90: 656c 6965 7665 2074 6861 7420 6d61 6368  elieve that mach
+00005ca0: 696e 6520 6c65 6172 6e69 6e67 2072 656c  ine learning rel
+00005cb0: 6174 6564 206c 6962 7261 7269 6573 206f  ated libraries o
+00005cc0: 7220 6672 616d 6577 6f72 6b73 2073 686f  r frameworks sho
+00005cd0: 756c 6420 6e6f 7420 666f 6c6c 6f77 205b  uld not follow [
+00005ce0: 4a61 636b 206f 6620 616c 6c20 7472 6164  Jack of all trad
+00005cf0: 6573 2c20 6d61 7374 6572 206f 6620 6e6f  es, master of no
+00005d00: 6e65 5d28 6874 7470 733a 2f2f 656e 2e77  ne](https://en.w
+00005d10: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00005d20: 692f 4a61 636b 5f6f 665f 616c 6c5f 7472  i/Jack_of_all_tr
+00005d30: 6164 6573 2c5f 6d61 7374 6572 5f6f 665f  ades,_master_of_
+00005d40: 6e6f 6e65 2920 7072 696e 6369 706c 652e  none) principle.
+00005d50: 2049 6e73 7465 6164 2c20 7468 6579 2073   Instead, they s
+00005d60: 686f 756c 6420 6265 2066 6f63 7573 6564  hould be focused
+00005d70: 206f 6e20 6120 7369 6e67 6c65 2074 6173   on a single tas
+00005d80: 6b20 616e 6420 646f 2069 7420 7765 6c6c  k and do it well
+00005d90: 2e0a 0a23 2320 e29c 8520 5768 6f20 6973  ...## ... Who is
+00005da0: 2075 7369 6e67 2046 726f 7572 6f73 3f0a   using Frouros?.
+00005db0: 0a46 726f 7572 6f73 2069 7320 6163 7469  .Frouros is acti
+00005dc0: 7665 6c79 2062 6569 6e67 2075 7365 6420  vely being used 
+00005dd0: 6279 2074 6865 2066 6f6c 6c6f 7769 6e67  by the following
+00005de0: 2070 726f 6a65 6374 7320 746f 2069 6d70   projects to imp
+00005df0: 6c65 6d65 6e74 2064 7269 6674 0a64 6574  lement drift.det
+00005e00: 6563 7469 6f6e 2069 6e20 6d61 6368 696e  ection in machin
+00005e10: 6520 6c65 6172 6e69 6e67 2070 6970 656c  e learning pipel
+00005e20: 696e 6573 3a0a 0a20 2a20 5b41 4934 454f  ines:.. * [AI4EO
+00005e30: 5343 5d28 6874 7470 733a 2f2f 6169 3465  SC](https://ai4e
+00005e40: 6f73 632e 6575 292e 0a20 2a20 5b69 4d61  osc.eu).. * [iMa
+00005e50: 6769 6e65 5d28 6874 7470 733a 2f2f 696d  gine](https://im
+00005e60: 6167 696e 652d 6169 2e65 7529 2e0a 0a49  agine-ai.eu)...I
+00005e70: 6620 796f 7520 7761 6e74 2079 6f75 7220  f you want your 
+00005e80: 7072 6f6a 6563 7420 6c69 7374 6564 2068  project listed h
+00005e90: 6572 652c 2064 6f20 6e6f 7420 6865 7369  ere, do not hesi
+00005ea0: 7461 7465 2074 6f20 7365 6e64 2075 7320  tate to send us 
+00005eb0: 6120 7075 6c6c 2072 6571 7565 7374 2e0a  a pull request..
+00005ec0: 0a23 2320 f09f 918d 2043 6f6e 7472 6962  .## .... Contrib
+00005ed0: 7574 696e 670a 0a43 6865 636b 206f 7574  uting..Check out
+00005ee0: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
+00005ef0: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
+00005f00: 7562 2e63 6f6d 2f49 4643 412f 6672 6f75  ub.com/IFCA/frou
+00005f10: 726f 732f 626c 6f62 2f6d 6169 6e2f 434f  ros/blob/main/CO
+00005f20: 4e54 5249 4255 5449 4e47 2e6d 6429 2073  NTRIBUTING.md) s
+00005f30: 6563 7469 6f6e 2e0a 0a23 2320 f09f 92ac  ection...## ....
+00005f40: 2043 6974 6174 696f 6e0a 0a41 6c74 686f   Citation..Altho
+00005f50: 7567 6820 4672 6f75 726f 7320 7061 7065  ugh Frouros pape
+00005f60: 7220 6973 2073 7469 6c6c 2069 6e20 7072  r is still in pr
+00005f70: 6570 7269 6e74 2c20 6966 2079 6f75 2077  eprint, if you w
+00005f80: 616e 7420 746f 2063 6974 6520 6974 2079  ant to cite it y
+00005f90: 6f75 2063 616e 2075 7365 2074 6865 205b  ou can use the [
+00005fa0: 7072 6570 7269 6e74 5d28 6874 7470 733a  preprint](https:
+00005fb0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00005fc0: 3232 3038 2e30 3638 3638 2920 7665 7273  2208.06868) vers
+00005fd0: 696f 6e20 2874 6f20 6265 2072 6570 6c61  ion (to be repla
+00005fe0: 6365 6420 6279 2074 6865 2070 6170 6572  ced by the paper
+00005ff0: 206f 6e63 6520 6973 2070 7562 6c69 7368   once is publish
+00006000: 6564 292e 0a0a 6060 6062 6962 7465 780a  ed)...```bibtex.
+00006010: 4061 7274 6963 6c65 7b63 6573 7065 6465  @article{cespede
+00006020: 7332 3032 3266 726f 7572 6f73 2c0a 2020  s2022frouros,.  
+00006030: 7469 746c 653d 7b46 726f 7572 6f73 3a20  title={Frouros: 
+00006040: 4120 5079 7468 6f6e 206c 6962 7261 7279  A Python library
+00006050: 2066 6f72 2064 7269 6674 2064 6574 6563   for drift detec
+00006060: 7469 6f6e 2069 6e20 6d61 6368 696e 6520  tion in machine 
+00006070: 6c65 6172 6e69 6e67 2073 7973 7465 6d73  learning systems
+00006080: 7d2c 0a20 2061 7574 686f 723d 7b43 7b5c  },.  author={C{\
+00006090: 2765 7d73 7065 6465 732d 5369 736e 6965  'e}spedes-Sisnie
+000060a0: 6761 2c20 4a61 696d 6520 616e 6420 4c7b  ga, Jaime and L{
+000060b0: 5c27 6f7d 7065 7a2d 4761 7263 7b5c 275c  \'o}pez-Garc{\'\
+000060c0: 697d 612c 207b 5c27 417d 6c76 6172 6f20  i}a, {\'A}lvaro 
+000060d0: 7d2c 0a20 206a 6f75 726e 616c 3d7b 6172  },.  journal={ar
+000060e0: 5869 7620 7072 6570 7269 6e74 2061 7258  Xiv preprint arX
+000060f0: 6976 3a32 3230 382e 3036 3836 387d 2c0a  iv:2208.06868},.
+00006100: 2020 7965 6172 3d7b 3230 3232 7d0a 7d0a    year={2022}.}.
+00006110: 6060 600a 0a23 2320 f09f 939d 204c 6963  ```..## .... Lic
+00006120: 656e 7365 0a0a 4672 6f75 726f 7320 6973  ense..Frouros is
+00006130: 2061 6e20 6f70 656e 2d73 6f75 7263 6520   an open-source 
+00006140: 736f 6674 7761 7265 206c 6963 656e 7365  software license
+00006150: 6420 756e 6465 7220 7468 6520 5b42 5344  d under the [BSD
+00006160: 2d33 2d43 6c61 7573 6520 6c69 6365 6e73  -3-Clause licens
+00006170: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00006180: 622e 636f 6d2f 4946 4341 2f66 726f 7572  b.com/IFCA/frour
+00006190: 6f73 2f62 6c6f 622f 6d61 696e 2f4c 4943  os/blob/main/LIC
+000061a0: 454e 5345 292e 0a0a 2323 20f0 9f99 8f20  ENSE)...## .... 
+000061b0: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
+000061c0: 0a0a 4672 6f75 726f 7320 6861 7320 7265  ..Frouros has re
+000061d0: 6365 6976 6564 2066 756e 6469 6e67 2066  ceived funding f
+000061e0: 726f 6d20 7468 6520 4167 656e 6369 6120  rom the Agencia 
+000061f0: 4573 7461 7461 6c20 6465 2049 6e76 6573  Estatal de Inves
+00006200: 7469 6761 6369 c3b3 6e2c 2055 6e69 6461  tigaci..n, Unida
+00006210: 6420 6465 2045 7863 656c 656e 6369 6120  d de Excelencia 
+00006220: 4d61 72c3 ad61 2064 6520 4d61 657a 7475  Mar..a de Maeztu
+00006230: 2c20 7265 662e 204d 444d 2d32 3031 372d  , ref. MDM-2017-
+00006240: 3037 3635 2e0a 0a0a                      0765....
```

### Comparing `frouros-0.5.1/frouros/callbacks/base.py` & `frouros-0.6.0/frouros/callbacks/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Base callback module."""
 
 import abc
 from typing import Optional
 
+import numpy as np  # type: ignore
+
 
 class BaseCallback(abc.ABC):
     """Abstract class representing a callback."""
 
     def __init__(self, name: Optional[str] = None) -> None:
         """Init method.
 
@@ -51,19 +53,27 @@
     #     if not isinstance(
     #             value, (BaseConceptDrift, BaseDataDriftBatch)):
     #         raise TypeError(
     #             "value must be of type BaseConceptDrift or BaseDataDriftBatch."
     #         )
     #     self._detector = value
 
-    def on_fit_start(self, **kwargs) -> None:
-        """On fit start method."""
+    def on_fit_start(self, X: np.ndarray) -> None:  # noqa: N803
+        """On fit start method.
+
+        :param X: reference data
+        :type X: numpy.ndarray
+        """
 
-    def on_fit_end(self, **kwargs) -> None:
-        """On fit end method."""
+    def on_fit_end(self, X: np.ndarray) -> None:  # noqa: N803
+        """On fit end method.
+
+        :param X: reference data
+        :type X: numpy.ndarray
+        """
 
     @abc.abstractmethod
     def reset(self) -> None:
         """Reset method."""
 
     def __repr__(self) -> str:
         """Repr method.
```

### Comparing `frouros-0.5.1/frouros/callbacks/batch/base.py` & `frouros-0.6.0/frouros/callbacks/streaming/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-"""Base callback batch module."""
+"""Base callback streaming module."""
 
 import abc
+from typing import Union
 
 from frouros.callbacks.base import BaseCallback
 
 
-class BaseCallbackBatch(BaseCallback):
-    """Callback batch class."""
+class BaseCallbackStreaming(BaseCallback):
+    """Callback streaming class."""
 
-    def on_compare_start(self, **kwargs) -> None:
-        """On compare start method."""
+    def on_update_start(self, value: Union[int, float]) -> None:
+        """On update start method.
 
-    def on_compare_end(self, **kwargs) -> None:
-        """On compare end method."""
+        :param value: value used to update the detector
+        :type value: Union[int, float]
+        """
+
+    def on_update_end(self, value: Union[int, float]) -> None:
+        """On update end method.
+
+        :param value: value used to update the detector
+        :type value: Union[int, float]
+        """
 
     # FIXME: set_detector method as a workaround to  # pylint: disable=fixme
     #  avoid circular import problem. Make it an abstract method and
     #  uncomment commented code when it is solved
 
     # @abc.abstractmethod
     # def set_detector(self, detector) -> None:
```

### Comparing `frouros-0.5.1/frouros/callbacks/batch/permutation_test.py` & `frouros-0.6.0/frouros/callbacks/batch/permutation_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,33 +6,57 @@
 import numpy as np  # type: ignore
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.utils.stats import permutation
 
 
 class PermutationTestDistanceBased(BaseCallbackBatch):
-    """Permutation test on distance based batch callback class."""
+    """Permutation test callback class that can be applied to :mod:`data_drift.batch.distance_based <frouros.detectors.data_drift.batch.distance_based>` detectors.
 
-    def __init__(
+    :param num_permutations: number of permutations to obtain the p-value
+    :type num_permutations: int
+    :param num_jobs: number of jobs, defaults to -1
+    :type num_jobs: int
+    :param verbose: verbose flag, defaults to False
+    :type verbose: bool
+    :param name: name value, defaults to None. If None, the name will be set to `PermutationTestDistanceBased`.
+    :type name: Optional[str]
+
+    :Note:
+    Callbacks logs are updated with the following variables:
+
+    - `observed_statistic`: observed statistic obtained from the distance-based detector. Same distance value returned by the `compare` method
+    - `permutation_statistic`: list of statistics obtained from the permutations
+    - `p_value`: p-value obtained from the permutation test
+
+    :Example:
+
+    >>> from frouros.callbacks import PermutationTestDistanceBased
+    >>> from frouros.detectors.data_drift import MMD
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.multivariate_normal(mean=[1, 1], cov=[[2, 0], [0, 2]], size=100)
+    >>> Y = np.random.multivariate_normal(mean=[0, 0], cov=[[2, 1], [1, 2]], size=100)
+    >>> detector = MMD(callbacks=PermutationTestDistanceBased(num_permutations=1000, random_state=31))
+    >>> _ = detector.fit(X=X)
+    >>> distance, callbacks_log = detector.compare(X=Y)
+    >>> distance
+    DistanceResult(distance=0.05643613752975596)
+    >>> callbacks_log["PermutationTestDistanceBased"]["p_value"]
+    0.0
+    """  # noqa: E501  # pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
         self,
         num_permutations: int,
         num_jobs: int = -1,
-        name: Optional[str] = None,
         verbose: bool = False,
+        name: Optional[str] = None,
         **kwargs,
     ) -> None:
-        """Init method.
-
-        :param num_permutations: number of permutations
-        :type num_permutations: int
-        :param num_jobs: number of jobs
-        :type num_jobs: int
-        :param name: name to be use
-        :type name: Optional[str]
-        """
         super().__init__(name=name)
         self.num_permutations = num_permutations
         self.num_jobs = num_jobs
         self.verbose = verbose
         self.permutation_kwargs = kwargs
 
     @property
@@ -120,18 +144,30 @@
             random_state=random_state,
             verbose=verbose,
         )
         permuted_statistic = np.array(permuted_statistic)
         p_value = (permuted_statistic >= observed_statistic).mean()  # type: ignore
         return permuted_statistic, p_value
 
-    def on_compare_end(self, **kwargs) -> None:
-        """On compare end method."""
-        X_ref, X_test = kwargs["X_ref"], kwargs["X_test"]  # noqa: N806
-        observed_statistic = kwargs["result"][0]
+    def on_compare_end(
+        self,
+        result: Any,
+        X_ref: np.ndarray,  # noqa: N803
+        X_test: np.ndarray,
+    ) -> None:
+        """On compare end method.
+
+        :param result: result obtained from the `compare` method
+        :type result: Any
+        :param X_ref: reference data
+        :type X_ref: numpy.ndarray
+        :param X_test: test data
+        :type X_test: numpy.ndarray
+        """
+        observed_statistic = result.distance
         permuted_statistics, p_value = self._calculate_p_value(
             X_ref=X_ref,
             X_test=X_test,
             statistic=self.detector.statistical_method,  # type: ignore
             statistic_args=self.detector.statistical_kwargs,  # type: ignore
             observed_statistic=observed_statistic,
             num_permutations=self.num_permutations,
```

### Comparing `frouros-0.5.1/frouros/callbacks/streaming/msprt.py` & `frouros-0.6.0/frouros/datasets/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,202 +1,198 @@
-"""mSPRT (Mixing Sequentially Probability Ratio Test) callback module."""
+"""Base dataset module."""
 
-from typing import Union, Tuple, Optional
+import abc
+import tempfile
+import urllib.parse
+from pathlib import Path
+from typing import Any, List, Optional, Union
 
 import numpy as np  # type: ignore
+import requests
 
-from frouros.callbacks.streaming.base import BaseCallbackStreaming
-from frouros.utils.stats import CircularMean
+from frouros.datasets.exceptions import (
+    DownloadError,
+    InvalidURLError,
+    ReadFileError,
+)
+from frouros.utils.logger import logger
 
 
-class mSPRT(BaseCallbackStreaming):  # noqa: N801 # pylint: disable=invalid-name
-    """mSPRT (mixing Sequentially Probability Ratio Test) callback class.
-
-    :References:
-
-    .. [johari2022always] Ramesh, Johari, et al.
-        "Always valid inference: Continuous monitoring of a/b tests"
-        Operations Research 70.3 (2022): 1806-1821.
-    """
+class BaseDatasetDownload(abc.ABC):
+    """Abstract class representing a downloadable dataset."""
 
     def __init__(
         self,
-        alpha: float,
-        sigma: Union[int, float] = 1.0,
-        tau: Union[int, float] = 1.0,
-        lambda_: Union[int, float] = 1.0,
-        name: Optional[str] = None,
+        url: Union[str, List[str]],
+        file_path: Optional[str] = None,
     ) -> None:
         """Init method.
 
-        :param alpha: alpha value
-        :type alpha: float
-        :param sigma: sigma value
-        :type sigma: Union[int, float]
-        :param tau: tau value
-        :type tau: Union[int, float]
-        :param lambda_: lambda value
-        :type lambda_: Union[int, float]
-        :param name: name value
-        :type name: Optional[str]
-        """
-        super().__init__(name=name)
-        self.alpha = alpha
-        self.sigma = sigma
-        self.sigma_squared = self.sigma**2
-        self.two_sigma_squared = 2 * self.sigma_squared
-        self.tau = tau
-        self.tau_squared = self.tau**2
-        self.lambda_ = lambda_
-        self.mean = None
-        self.theta = None
-        self.p_value = 1.0
+        :param url: url or url mirrors from where dataset will be downloaded
+        :type url: Union[str, List[str]]
+        :param file_path: file path for the downloaded file
+        :type file_path: str
+        """
+        self.url = url  # type: ignore
+        self.file_path: Optional[Path] = (
+            Path(file_path)
+            if file_path
+            else Path(tempfile.NamedTemporaryFile(delete=False).name)
+        )
 
     @property
-    def alpha(self) -> float:
-        """Alpha property.
+    def file_path(self) -> Optional[Path]:
+        """File path property.
 
-        :return: alpha value
-        :rtype: float
+        :return: file path for the downloaded dataset
+        :rtype: Optional[Path]
         """
-        return self._alpha
+        return self._file_path
 
-    @alpha.setter
-    def alpha(self, value: float) -> None:
-        """Alpha setter.
+    @file_path.setter
+    def file_path(self, value: Optional[Path]) -> None:
+        """File path setter.
 
         :param value: value to be set
-        :type value: float
+        :type value: Optional[Path]
         """
-        if not isinstance(value, float):
-            raise TypeError("alpha must be a float")
-        if not 0.0 < value < 1.0:
-            raise ValueError("alpha must be in the range (0, 1)")
-        self._alpha = value
+        self._file_path = value
 
     @property
-    def sigma(self) -> Optional[Union[int, float]]:
-        """Sigma property.
+    def url(self) -> Union[str, List[str]]:
+        """URL property.
 
-        :return: sigma value
-        :rtype: Optional[Union[int, float]]
+        :return: URL from where dataset will be downloaded
+        :rtype: Union[str, List[str]]
         """
-        return self._sigma
+        return self._url
 
-    @sigma.setter
-    def sigma(self, value: Optional[Union[int, float]]) -> None:
-        """Sigma setter.
+    @url.setter
+    def url(self, value: Union[str, List[str]]) -> None:
+        """URL setter.
 
         :param value: value to be set
-        :type value: Optional[float]
+        :type value: Union[str, List[str]]
+        :raises InvalidURLError: Invalid URL exception
         """
-        if value is not None and not isinstance(value, (int, float)):
-            raise TypeError("sigma must be int, float or None")
-        self._sigma = value
+        urls = [value] if isinstance(value, str) else value
+        for url in urls:
+            if not self._check_valid_url(url=url):
+                raise InvalidURLError(f"{value} is not a valid URL.")
+        self._url = urls
 
-    @property
-    def tau(self) -> Optional[Union[int, float]]:
-        """Tau property.
+    @staticmethod
+    def _check_valid_url(url: str) -> bool:
+        final_url = urllib.parse.urlparse(url=urllib.parse.urljoin(base=url, url="/"))
+        is_valid = (
+            all([final_url.scheme, final_url.netloc, final_url.path])
+            and len(final_url.netloc.split(".")) > 1
+        )
+        return is_valid
 
-        :return: tau squared value
-        :rtype: Optional[Union[int, float]]
-        """
-        return self._tau
+    def _get_file(self, url: str) -> None:
+        response = self._request_file(url=url)
+        self._save_file(response=response)
+
+    def _remove_temporal_file(self) -> None:
+        self.file_path.unlink()  # type: ignore
+        self.file_path = None
+
+    def _request_file(self, url: str) -> requests.models.Response:
+        logger.info("Trying to download data from %s to %s", url, self._file_path)
+        request_head = requests.head(url=url)
+        if not request_head.ok:
+            raise requests.exceptions.RequestException()
+        request_response = requests.get(url=url, stream=True)
+        request_response.raise_for_status()
+        return request_response
+
+    def _save_file(self, response: requests.models.Response) -> None:
+        try:
+            self._write_file(content=response.content)
+        except IOError as e:
+            raise e
+
+    def _write_file(self, content: bytes) -> None:
+        with open(file=self.file_path, mode="ab") as f:  # type: ignore
+            f.write(content)
+
+    def download(self) -> None:
+        """Download dataset.
+
+        :raises DownloadError: Download exception
+        """
+        for url in self.url:
+            try:
+                self._get_file(url=url)
+                break
+            except requests.exceptions.RequestException:
+                logger.warning("File cannot be downloaded from %s", url)
+        else:
+            raise DownloadError("File cannot be downloaded from any of the urls.")
+
+    def load(self, **kwargs) -> Any:
+        """Load dataset.
+
+        :param kwargs: dict of kwargs
+        :type kwargs: dict
+        :raises FileNotFoundError: File not found exception
+        :raises ReadFileError: Read file exception
+        :return: loaded dataset
+        :rtype: Any
+        """
+        if not self.file_path:
+            raise FileNotFoundError(
+                "Missing file to be loaded. "
+                "Try using download() before "
+                "load () method."
+            )
+        try:
+            dataset = self.read_file(**kwargs)
+        except IndexError as e:
+            raise ReadFileError(e) from e
+        self._remove_temporal_file()
+        return dataset
+
+    @abc.abstractmethod
+    def read_file(self, **kwargs) -> Any:
+        """Read file abstract method.
+
+        :param kwargs: dict of kwargs
+        :type kwargs: dict
+        :return: read file
+        :rtype: Any
+        """
+
+    def __repr__(self) -> str:
+        """Repr method.
+
+        :return: repr value
+        :rtype: str
+        """
+        return (
+            f"{self.__class__.__name__}"
+            f"(url={self.url}, file_path='{self.file_path}')"
+        )
 
-    @tau.setter
-    def tau(self, value: Union[int, float]) -> None:
-        """Tau setter.
 
-        :param value: value to be set
-        :type value: Union[int, float]
-        """
-        if not isinstance(value, (int, float)):
-            raise TypeError("tau must be int, float or None")
-        self._tau = value
+class BaseDatasetGenerator(abc.ABC):
+    """Abstract class representing a dataset generator."""
 
-    @property
-    def lambda_(self) -> Optional[Union[int, float]]:
-        """Lambda property.
+    def __init__(self, seed: Optional[int] = None) -> None:
+        """Init method.
 
-        :return: lambda value
-        :rtype: Optional[Union[int, float]]
+        :param seed: seed value
+        :type seed: Optional[int]
         """
-        return self._lambda_
+        try:
+            np.random.seed(seed=seed)
+        except (TypeError, ValueError) as e:
+            raise e
 
-    @lambda_.setter
-    def lambda_(self, value: Union[int, float]) -> None:
-        """Lambda setter.
+    def __repr__(self) -> str:
+        """Repr method.
 
-        :param value: value to be set
-        :type value: Union[int, float]
+        :return: repr value
+        :rtype: str
         """
-        if not isinstance(value, (int, float)):
-            if value <= 0.0:
-                raise ValueError("lambda_ must be greater than 0")
-        self._lambda_ = value
-
-    def on_fit_end(self, **kwargs) -> None:
-        """On fit end method."""
-        self.mean = CircularMean(size=self.detector.window_size)  # type: ignore
-        self.theta = self.detector.compare(X=kwargs["X"])[0].distance  # type: ignore
-
-    def on_update_end(self, **kwargs) -> None:
-        """On update end method."""
-        self.mean.update(value=kwargs["value"])  # type: ignore
-        self.p_value, likelihood = self._calculate_p_value()
-
-        self.logs.update(
-            {
-                "distance_mean": self.mean.get(),  # type: ignore
-                "likelihood": likelihood,
-                "p_value": self.p_value,
-            },
-        )
-
-    def reset(self) -> None:
-        """Reset method."""
-        super().reset()
-        self.mean = None
-        self.p_value = 1.0
-
-    def _calculate_p_value(self) -> Tuple[float, float]:
-        likelihood = self._likelihood_normal_mixing_distribution(
-            mean=self.mean.get(),  # type: ignore
-            sigma=self.sigma,  # type: ignore
-            sigma_squared=self.sigma_squared,
-            tau_squared=self.tau_squared,
-            two_sigma_squared=self.two_sigma_squared,
-            n=self.detector.window_size,  # type: ignore
-            theta=self.theta,  # type: ignore
-            lambda_=self.lambda_,  # type: ignore
-        )
-        p_value = min(
-            self.p_value,
-            1 / likelihood,
-        )
-        return p_value, likelihood
-
-    @staticmethod
-    def _likelihood_normal_mixing_distribution(  # pylint: disable=too-many-arguments
-        mean: float,
-        sigma: float,
-        sigma_squared: float,
-        tau_squared: float,
-        two_sigma_squared: float,
-        n: int,
-        theta: float,
-        lambda_: float,
-    ) -> float:
-        # FIXME: Explore lambda_ influence   # pylint: disable=fixme
-        #  and redesign the likelihood formula
-        n_tau_squared = n * tau_squared
-        sigma_squared_plus_n_tau_squared = sigma_squared + n_tau_squared
-        likelihood = (sigma / np.sqrt(sigma_squared_plus_n_tau_squared)) * np.exp(
-            n
-            * n_tau_squared
-            * lambda_  # Not present in mSPRT, added as a hyperparameter to control
-            # the influence of the distance difference
-            * (mean - theta)
-            ** 2  # (mean-theta) ** 2, theta=detector statistic (H_0 value, no distance)
-            / (two_sigma_squared * sigma_squared_plus_n_tau_squared)
-        )
-        return likelihood
+        return f"{self.__class__.__name__}()"
```

### Comparing `frouros-0.5.1/frouros/datasets/synthetic.py` & `frouros-0.6.0/frouros/datasets/synthetic.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,52 @@
 """Synthetic datasets module."""
 
-from typing import Tuple, Iterator
+from typing import Tuple, Iterator, Optional
 
 import numpy as np  # type: ignore
 
 from frouros.datasets.base import BaseDatasetGenerator
 from frouros.datasets.exceptions import InvalidBlockError
 
 
 class SEA(BaseDatasetGenerator):
     """SEA generator [street2001streaming]_.
 
+    :param seed: seed value, defaults to None
+    :type seed: Optional[int]
+
     :References:
 
     .. [street2001streaming] Street, W. Nick, and YongSeog Kim.
         "A streaming ensemble algorithm (SEA) for large-scale classification."
         Proceedings of the seventh ACM SIGKDD international conference on Knowledge
         discovery and data mining. 2001.
+
+    :Example:
+
+    >>> from frouros.datasets.synthetic import SEA
+    >>> sea = SEA(seed=31)
+    >>> dataset = sea.generate_dataset(block=1, noise=0.1, num_samples=5)
+    >>> for X, y in dataset:
+    ...     print(X, y)
+    [2.86053822 9.58105567 7.70312932] 0
+    [2.08165462 1.36917049 9.08373802] 0
+    [8.36483632 1.12172604 8.3489916 ] 0
+    [2.44680795 1.36231348 7.22094455] 1
+    [1.28477715 2.20364007 5.19211202] 1
     """
 
-    block_map = {1: 8.0, 2: 9.0, 3: 7.0, 4: 9.5}
+    def __init__(  # noqa: D107
+        self,
+        seed: Optional[int] = None,
+    ) -> None:
+        super().__init__(
+            seed=seed,
+        )
+        self._block_map = {1: 8.0, 2: 9.0, 3: 7.0, 4: 9.5}
 
     @staticmethod
     def _generate_sample(threshold: float, noise: float) -> Tuple[np.ndarray, int]:
         X = np.random.uniform(low=0.0, high=10.0, size=(3,))  # noqa: N806
         if np.random.random() < noise:
             y = np.random.randint(2)
         else:
@@ -31,25 +54,25 @@
         return X, y
 
     def generate_dataset(
         self, block: int, noise: float = 0.1, num_samples: int = 12500
     ) -> Iterator[Tuple[np.ndarray, int]]:
         """Generate dataset.
 
-        :param block: block to generate samples from
+        :param block: block to generate samples from, must be 1, 2, 3 or 4
         :type block: int
-        :param noise: ratio of samples with a noisy class
+        :param noise: ratio of samples with a noisy class, defaults to 0.1
         :type noise: float
-        :param num_samples: number of samples to generate
+        :param num_samples: number of samples to generate, defaults to 12500
         :type num_samples: int
         :return: generator with the samples
         :rtype: Iterator[Tuple[np.ndarray, int]]
         """
         try:
-            threshold = self.block_map[block]
+            threshold = self._block_map[block]
         except KeyError as e:
             raise InvalidBlockError("block must be 1, 2, 3 or 4.") from e
         if num_samples < 1:
             raise ValueError("num_samples must be greater than 0.")
         if not 0 <= noise <= 1:
             raise ValueError("noise must be in the range [0, 1].")
         dataset = (
```

### Comparing `frouros-0.5.1/frouros/detectors/base.py` & `frouros-0.6.0/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/__init__.py` & `frouros-0.6.0/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/base.py` & `frouros-0.6.0/frouros/detectors/concept_drift/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,25 +180,25 @@
         return {"drift": self.drift}
 
     def update(self, value: Union[int, float], **kwargs) -> Dict[str, Any]:
         """Update method.
 
         :param value: value to update detector
         :type value: Union[int, float]
+        :return: callbacks logs
+        :rtype: Dict[str, Any]]
         """
         for callback in self.callbacks:  # type: ignore
             callback.on_update_start(  # type: ignore
                 value=value,
-                **kwargs,
             )
         self._update(value=value, **kwargs)
         for callback in self.callbacks:  # type: ignore
             callback.on_update_end(  # type: ignore
                 value=value,
-                **kwargs,
             )
 
         callbacks_logs = self._get_callbacks_logs()
         return callbacks_logs
 
     def _get_callbacks_logs(self) -> Dict[str, Any]:
         logs = {
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/base.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,29 +22,27 @@
 
     @abc.abstractmethod
     def _update(self, value: Union[int, float], **kwargs) -> None:
         pass
 
 
 class BaseCUSUMConfig(BaseChangeDetectionConfig):
-    """Class representing a CUSUM based configuration class."""
+    """Class representing a CUSUM based configuration class.
 
-    def __init__(
+    :param lambda_: lambda value, defaults to 50.0
+    :type lambda_: float
+    :param min_num_instances: minimum numbers of instances to start looking for changes, defaults to 30
+    :type min_num_instances: int
+    """  # noqa: E501  # pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
         self,
         lambda_: float = 50.0,
         min_num_instances: int = 30,
     ) -> None:
-        """Init method.
-
-        :param lambda_: lambda value
-        :type lambda_: float
-        :param min_num_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_instances: int
-        """
         super().__init__(min_num_instances=min_num_instances)
         self.lambda_ = lambda_
 
     @property
     def lambda_(self) -> float:
         """Threshold property.
 
@@ -135,33 +133,31 @@
         """
         if not 0.0 <= value <= 1.0:
             raise ValueError("alpha must be in the range [0, 1].")
         self._alpha = value
 
 
 class BaseCUSUM(BaseChangeDetection):
-    """CUSUM based algorithm class."""
+    """CUSUM based algorithm class.
+
+    :param config: configuration parameters, defaults to None
+    :type config: Optional[BaseCUSUMConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+    """  # noqa: E501
 
     config_type = BaseCUSUMConfig
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         config: Optional[BaseCUSUMConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[BaseCUSUMConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "mean_error_rate": Mean(),
             "sum_": 0.0,
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """BOCD (Bayesian Online Change Detection) module."""
 
 import abc
 import copy
-from typing import Union, Optional
+from typing import List, Union, Optional
 
 import numpy as np  # type: ignore
 from scipy.special import logsumexp  # type: ignore
 from scipy.stats import norm  # type: ignore
 
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.change_detection.base import (
     BaseChangeDetection,
     BaseChangeDetectionConfig,
 )
 
 
 class BaseBOCDModel(abc.ABC):
@@ -37,15 +38,16 @@
         :type value: Union[int, float]
         """
 
 
 class GaussianUnknownMean(BaseBOCDModel):
     """Gaussian unknown mean model.
 
-    (adapted from the implementation in https://github.com/gwgundersen/bocd)
+    :Note:
+     Adapted from the implementation in https://github.com/gwgundersen/bocd.
     """
 
     def __init__(
         self,
         prior_mean: float = 0,
         prior_var: float = 1,
         data_var: float = 1,
@@ -117,41 +119,40 @@
         """Helper function for computing the posterior variance."""
         return 1 / self.precision_params + self.data_var
 
 
 class BOCDConfig(BaseChangeDetectionConfig):
     """BOCD (Bayesian Online Change Detection) [adams2007bayesian]_ configuration.
 
+    :param model: BOCD model, defaults to None. If None, :class:`frouros.detectors.concept_drift.streaming.change_detection.bocd.GaussianUnknownMean` is used.
+    :type model: Optional[BaseBOCDModel]
+    :param hazard: hazard value, defaults to 0.01
+    :type hazard: float
+    :param min_num_instances: minimum numbers of instances to start looking for changes, defaults to 30
+    :type min_num_instances: int
+
     :References:
 
     .. [adams2007bayesian] Adams, Ryan Prescott, and David JC MacKay.
         "Bayesian online changepoint detection."
         arXiv preprint arXiv:0710.3742 (2007).
-    """
+    """  # noqa: E501  pylint: disable=line-too-long
 
-    def __init__(
+    model_type = GaussianUnknownMean
+
+    def __init__(  # noqa: D107
         self,
-        model: BaseBOCDModel = GaussianUnknownMean,  # type: ignore
+        model: Optional[BaseBOCDModel] = None,  # type: ignore
         hazard: float = 0.01,
         min_num_instances: int = 30,
     ) -> None:
-        """Init method.
-
-        :param model: BOCD model
-        :type model: BaseBOCDModel
-        :param hazard: hazard value
-        :type hazard: float
-        :param min_num_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_instances: int
-        """
         super().__init__(
             min_num_instances=min_num_instances,
         )
-        self.model = model
+        self.model = model  # type: ignore
         self.log_hazard = np.log(hazard)
         self.log_1_minus_hazard = np.log(1 - hazard)
 
     @property
     def model(self) -> BaseBOCDModel:
         """Get model.
 
@@ -164,43 +165,67 @@
     def model(self, model: BaseBOCDModel) -> None:
         """Set model.
 
         :param model: model
         :type model: BaseBOCDModel
         :raises TypeError: if model is not an instance of BaseModel
         """
-        if not isinstance(model, BaseBOCDModel):
-            raise TypeError(
-                f"model must be an instance of BaseModel, not {type(model)}"
-            )
-        self._model = model
+        if model is not None:
+            if not isinstance(model, BaseBOCDModel):
+                raise TypeError(
+                    f"model must be an instance of BaseModel, not {type(model)}"
+                )
+            self._model = model
+        else:
+            self._model = self.model_type()
 
 
 class BOCD(BaseChangeDetection):
     """BOCD (Bayesian Online Change Detection) [adams2007bayesian]_ detector.
 
-     (adapted from the implementation in https://github.com/gwgundersen/bocd)
+    :param config: configuration object of the detector, defaults to None. If None, the default configuration of :class:`BOCDConfig` is used.
+    :type config: Optional[BOCDConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
+    :Note:
+     Adapted from the implementation in https://github.com/gwgundersen/bocd.
 
     :References:
 
     .. [adams2007bayesian] Adams, Ryan Prescott, and David JC MacKay.
         "Bayesian online changepoint detection."
         arXiv preprint arXiv:0710.3742 (2007).
-    """
 
-    config_type = BOCDConfig  # type: ignore
+    :Example:
 
-    def __init__(self, config: BOCDConfig, callbacks: list = None) -> None:
-        """Init method.
+    >>> from frouros.detectors.concept_drift import BOCD
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> dist_a = np.random.normal(loc=0.2, scale=0.01, size=1000)
+    >>> dist_b = np.random.normal(loc=0.8, scale=0.04, size=1000)
+    >>> stream = np.concatenate((dist_a, dist_b))
+    >>> detector = BOCD()
+    >>> for i, value in enumerate(stream):
+    ...     _ = detector.update(value=value)
+    ...     if detector.drift:
+    ...         print(f"Change detected at step {i}")
+    ...         break
+    Change detected at step 1031
+    """  # noqa: E501  # pylint: disable=line-too-long
 
-        :param config: configuration object of the detector
-        :type config: BOCDConfig
-        :param callbacks: list of callbacks, defaults to None
-        :type callbacks: list, optional
-        """
+    config_type = BOCDConfig  # type: ignore
+
+    def __init__(  # noqa: D107
+        self,
+        config: Optional[BOCDConfig] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
+    ) -> None:
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "log_r": np.array([[0.0]]),
             "predicted_mean": None,
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,16 @@
     ) -> None:
         """Init method.
 
         :param average_run_length: expected time between false positive detections
         :type average_run_length: int
         :param lambda_: weight given to recent data compared to older data
         :type lambda_: float
+        :param warning_level: warning level value
+        :type warning_level: float
         :param min_num_instances: minimum numbers of instances
         to start looking for changes
         :type min_num_instances: int
         :raises InvalidAverageRunLengthError: Invalid average run length error exception
         """
         super().__init__(min_num_instances=min_num_instances)
         try:
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.6.0/frouros/metrics/prequential_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,159 +1,135 @@
-"""ECDD (EWMA for Concept Drift Detection) module."""
+"""Prequential error using fading factor metric module."""
 
-from typing import List, Optional, Union
+from typing import Optional, Union
 
-import numpy as np  # type: ignore
+from frouros.metrics.base import BaseMetric
 
-from frouros.callbacks.streaming.base import BaseCallbackStreaming
-from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    BaseSPC,
-    BaseECDDConfig,
-)
-from frouros.utils.stats import EWMA, Mean
 
+class PrequentialError(BaseMetric):
+    """Prequential error [dawid1984present]_ using fading factor [gama2009issues]_ metric.
 
-class ECDDWTConfig(BaseECDDConfig):
-    """ECDDWT (EWMA Concept Drift Detection Warning) [ross2012exponentially]_ configuration.
+    :param alpha: fading factor value, defaults to 1.0
+    :type alpha: Union[int, float]
+    :param name: name value, defaults to None. If None, the name will be set to `PrequentialError`.
+    :type name: Optional[str]
 
     :References:
 
-    .. [ross2012exponentially] Ross, Gordon J., et al.
-        "Exponentially weighted moving average charts for detecting concept drift."
-        Pattern recognition letters 33.2 (2012): 191-198.
-    """
+    .. [dawid1984present] Dawid, A. Philip.
+        "Present position and potential developments:
+        Some personal views statistical theory the prequential approach."
+        Journal of the Royal Statistical Society:
+        Series A (General) 147.2 (1984): 278-290.
+    .. [gama2009issues] Gama, Joao, Raquel Sebastiao, and Pedro Pereira Rodrigues.
+        "Issues in evaluation of stream learning algorithms."
+        Proceedings of the 15th ACM SIGKDD international conference on Knowledge
+        discovery and data mining. 2009.
+
+    :Example:
+
+    >>> from frouros.metrics import PrequentialError
+    >>> metric = PrequentialError(alpha=0.9)
+    >>> X = [1, 1, 0, 1, 0, 0]
+    >>> Y = [1, 0, 0, 0, 1, 1]
+    >>> for i, (X_sample, Y_sample) in enumerate(zip(X, Y)):
+    ...     error_value = 1 - (X_sample == Y_sample)
+    ...     prequential_error = metric(error_value=error_value)
+    ...     print(f"Metric={prequential_error:.5f} at step {i}")
+    Metric=0.00000 at step 0
+    Metric=0.52632 at step 1
+    Metric=0.33210 at step 2
+    Metric=0.52632 at step 3
+    Metric=0.64199 at step 4
+    Metric=0.71839 at step 5
+    """  # noqa: E501  # pylint: disable=line-too-long
 
-
-class ECDDWT(BaseSPC):
-    """ECDDWT (EWMA Concept Drift Detection Warning) [ross2012exponentially]_ detector.
-
-    :References:
-
-    .. [ross2012exponentially] Ross, Gordon J., et al.
-        "Exponentially weighted moving average charts for detecting concept drift."
-        Pattern recognition letters 33.2 (2012): 191-198.
-    """
-
-    config_type = ECDDWTConfig  # type: ignore
-
-    def __init__(
+    def __init__(  # noqa: D107
         self,
-        config: Optional[ECDDWTConfig] = None,
-        callbacks: Optional[
-            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
-        ] = None,
+        alpha: Union[int, float] = 1.0,
+        name: Optional[str] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[ECDDWTConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
-        super().__init__(
-            config=config,  # type: ignore
-            callbacks=callbacks,
-        )
-        self.additional_vars = {
-            "p": Mean(),
-            "z": EWMA(alpha=self.config.lambda_),  # type: ignore
-            **self.additional_vars,  # type: ignore
-        }
-        self._set_additional_vars_callback()
-        self._lambda_div_two_minus_lambda = self.config.lambda_ / (  # type: ignore
-            2 - self.config.lambda_  # type: ignore
-        )
+        super().__init__(name=name)
+        self.alpha = alpha
+        self.cumulative_error = 0.0
+        self.cumulative_instances = 0.0
+        self.num_instances = 0
 
     @property
-    def p(self) -> Mean:
-        """P property.
+    def alpha(self) -> Union[int, float]:
+        """Fading factor property.
 
-        :return: p value
-        :rtype: Mean
+        :return: fading factor value
+        :rtype: Union[int, float]
         """
-        return self._additional_vars["p"]
+        return self._alpha
 
-    @p.setter
-    def p(self, value: Mean) -> None:
-        """P setter.
+    @alpha.setter
+    def alpha(self, value: Union[int, float]) -> None:
+        """Fading factor setter.
 
         :param value: value to be set
-        :type value: Mean
-        :raises TypeError: Type error exception
+        :type value: Union[int, float]
         """
-        if not isinstance(value, Mean):
-            raise TypeError("value must be of type Mean.")
-        self._additional_vars["p"] = value
+        if not isinstance(value, (int, float)):
+            raise TypeError("value must be of type int or float.")
+        if not 0.0 < value <= 1.0:
+            raise ValueError("value must be in the range (0, 1].")
+        self._alpha = value
 
     @property
-    def z(self) -> EWMA:
-        """Z property.
+    def cumulative_instances(self) -> Union[int, float]:
+        """Cumulative instances' property.
 
-        :return: z value
-        :rtype: Mean
+        :return: fading factor value
+        :rtype: Union[int, float]
         """
-        return self._additional_vars["z"]
+        return self._cumulative_instances
 
-    @z.setter
-    def z(self, value: EWMA) -> None:
-        """Z setter.
+    @cumulative_instances.setter
+    def cumulative_instances(self, value: Union[int, float]) -> None:
+        """Cumulative instances' setter.
 
         :param value: value to be set
-        :type value: EWMA
-        :raises TypeError: Type error exception
+        :type value: Union[int, float]
         """
-        if not isinstance(value, EWMA):
-            raise TypeError("value must be of type EWMA.")
-        self._additional_vars["z"] = value
-
-    def _check_threshold(
-        self, control_limit: float, z_variance: float, warning_level: float = 1.0
-    ) -> bool:
-        return self.z.mean > self.p.mean + warning_level * control_limit * z_variance
+        if not isinstance(value, (int, float)):
+            raise TypeError("value must be of type int or float.")
+        self._cumulative_instances = value
+
+    @property
+    def cumulative_fading_error(self) -> Union[int, float]:
+        """Cumulative fading error property.
+
+        :return: cumulative facing error value
+        :rtype: Union[int, float]
+        """
+        return self.cumulative_error / self.cumulative_instances
+
+    def __call__(
+        self,
+        error_value: float,
+    ) -> Union[int, float]:
+        """__call__ method that updates the prequential error using fading factor.
+
+        :param error_value error value
+        :type error_value: float
+        :return: cumulative facing error
+        :rtype: Union[int, float]
+        """
+        self.cumulative_error = self.cumulative_error * self.alpha + error_value
+        self.cumulative_instances = self.cumulative_instances * self.alpha + 1
+        return self.cumulative_fading_error
 
     def reset(self) -> None:
         """Reset method."""
-        super().reset()
-        self.p = Mean()
-        self.z = EWMA(alpha=self.config.lambda_)  # type: ignore
-
-    def _update(self, value: Union[int, float], **kwargs) -> None:
-        self.num_instances += 1
-
-        self.p.update(value=value)
-        self.z.update(value=value)
-
-        if self.num_instances >= self.config.min_num_instances:
-            error_rate_variance = self.p.mean * (1 - self.p.mean)
-            z_variance = np.sqrt(
-                self._lambda_div_two_minus_lambda
-                * (1 - self.z.one_minus_alpha ** (2 * self.num_instances))
-                * error_rate_variance
-            )
-            control_limit = self.config.control_limit_func(  # type: ignore
-                p=self.p.mean
-            )
-
-            drift_flag = self._check_threshold(
-                control_limit=control_limit, z_variance=z_variance
-            )
-
-            if drift_flag:
-                # Out-of-Control
-                self.drift = True
-                self.warning = False
-            else:
-                warning_flag = self._check_threshold(
-                    control_limit=control_limit,
-                    z_variance=z_variance,
-                    warning_level=self.config.warning_level,  # type: ignore
-                )
-                if warning_flag:
-                    # Warning
-                    self.warning = True
-                else:
-                    # In-Control
-                    self.warning = False
-                self.drift = False
-        else:
-            self.drift, self.warning = False, False
+        self.cumulative_error = 0.0
+        self.cumulative_instances = 0.0
+        self.num_instances = 0
+
+    def __repr__(self) -> str:
+        """Repr method.
+
+        :return: repr value
+        :rtype: str
+        """
+        return f"{super().__repr__()[:-1]}, alpha={self.alpha})"
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,40 +11,37 @@
     BaseSPC,
 )
 
 
 class EDDMConfig(BaseSPCConfig):
     """EDDM (Early drift detection method) [baena2006early]_ configuration.
 
+    :param alpha: warning zone value, defaults to 0.95
+    :type alpha: float
+    :param beta: change zone value, defaults to 0.9
+    :type beta: float
+    :param level: level factor, defaults to 2.0
+    :type level: float
+    :param min_num_misclassified_instances: minimum numbers of instances to start looking for changes, defaults to 30
+    :type min_num_misclassified_instances: int
+
     :References:
 
     .. [baena2006early] Baena-Garcıa, Manuel, et al. "Early drift detection method."
         Fourth international workshop on knowledge discovery from data streams.
         Vol. 6. 2006.
-    """
+    """  # noqa: E501  # pylint: disable=line-too-long
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         alpha: float = 0.95,
         beta: float = 0.9,
         level: float = 2.0,
         min_num_misclassified_instances: int = 30,
     ) -> None:
-        """Init method.
-
-        :param alpha: warning zone value
-        :type alpha: float
-        :param beta: change zone value
-        :type beta: float
-        :param level: level factor
-        :type level: float
-        :param min_num_misclassified_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_misclassified_instances: int
-        """
         super().__init__()
         self.alpha = alpha
         self.beta = beta
         self.level = level
         self.min_num_misclassified_instances = min_num_misclassified_instances
 
     @property
@@ -132,38 +129,59 @@
             )
         self._min_num_misclassified_instances = value
 
 
 class EDDM(BaseSPC):
     """EDDM (Early drift detection method) [baena2006early]_ detector.
 
+    :param config: configuration object of the detector, defaults to None. If None, the default configuration of :class:`EDDMConfig` is used.
+    :type config: Optional[EDDMConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
+    :Note:
+    :func:`update` method expects to receive a value of 0 if the instance is correctly classified (no error) and 1 otherwise (error).
+
     :References:
 
     .. [baena2006early] Baena-Garcıa, Manuel, et al. "Early drift detection method."
         Fourth international workshop on knowledge discovery from data streams.
         Vol. 6. 2006.
-    """
+
+    :Example:
+
+    >>> from frouros.detectors.concept_drift import EDDM
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> dist_a = np.random.binomial(n=1, p=0.6, size=1000)
+    >>> dist_b = np.random.binomial(n=1, p=0.8, size=1000)
+    >>> stream = np.concatenate((dist_a, dist_b))
+    >>> detector = EDDM()
+    >>> warning_flag = False
+    >>> for i, value in enumerate(stream):
+    ...     _ = detector.update(value=value)
+    ...     if detector.drift:
+    ...         print(f"Change detected at step {i}")
+    ...         break
+    ...     if not warning_flag and detector.warning:
+    ...         print(f"Warning detected at step {i}")
+    ...         warning_flag = True
+    Warning detected at step 39
+    Change detected at step 1294
+    """  # noqa: E501  # pylint: disable=line-too-long
 
     config_type = EDDMConfig  # type: ignore
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         config: Optional[EDDMConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[EDDMConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         # mean_distance_error = 0.0
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         mean_distance_error = 0.0
         self.additional_vars = {
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """Init method.
 
         :param alpha_d: significance value for drift
         :type alpha_d: float
         :param alpha_w: significance value for warning
         :type alpha_w: float
         :param two_sided_test: flag that indicates if a two-sided test is performed
-        :param two_sided_test: bool
+        :type two_sided_test: bool
         :param min_num_instances: minimum numbers of instances
         to start looking for changes
         :type min_num_instances: int
         """
         super().__init__(min_num_instances=min_num_instances)
         self.alpha_d = alpha_d
         self.alpha_w = alpha_w
@@ -112,56 +112,76 @@
             raise ValueError("two_sided_test must be of type bool.")
         self._two_sided_test = value
 
 
 class HDDMAConfig(BaseHDDMConfig):
     """HDDM-A (Hoeffding's drift detection method A-Test) [frias2014online]_ configuration.
 
+    :param alpha_d: significance value for drift, defaults to 0.001
+    :type alpha_d: float
+    :param alpha_w: significance value for warning, defaults to 0.005
+    :type alpha_w: float
+    :param two_sided_test: flag that indicates if a two-sided test is performed, defaults to False
+    :type two_sided_test: bool
+    :param min_num_instances: minimum numbers of instances to start looking for changes, defaults to 30
+    :type min_num_instances: int
+
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
         810-823.
-    """
+    """  # noqa: E501  pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
+        self,
+        alpha_d: float = 0.001,
+        alpha_w: float = 0.005,
+        two_sided_test: bool = False,
+        min_num_instances: int = 30,
+    ) -> None:
+        super().__init__(
+            alpha_d=alpha_d,
+            alpha_w=alpha_w,
+            two_sided_test=two_sided_test,
+            min_num_instances=min_num_instances,
+        )
 
 
 class HDDMWConfig(BaseHDDMConfig):
     """HDDM-W (Hoeffding's drift detection method W-Test) [frias2014online]_ configuration.
 
+    :param alpha_d: significance value for drift, defaults to 0.001
+    :type alpha_d: float
+    :param alpha_w: significance value for warning, defaults to 0.005
+    :type alpha_w: float
+    :param two_sided_test: flag that indicates if a two-sided test is performed, defaults to False
+    :type two_sided_test: bool
+    :param lambda_: weight given to recent data compared to older data, defaults to 0.05
+    :type lambda_: float
+    :param min_num_instances: minimum numbers of instances to start looking for changes, defaults to 30
+    :type min_num_instances: int
+
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
         810-823.
-    """
+    """  # noqa: E501  # pylint: disable=line-too-long
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         alpha_d: float = 0.001,
         alpha_w: float = 0.005,
         two_sided_test: bool = False,
         lambda_: float = 0.05,
         min_num_instances: int = 30,
     ) -> None:
-        """Init method.
-
-        :param alpha_d: significance value for drift
-        :type alpha_d: float
-        :param alpha_w: significance value for warning
-        :type alpha_w: float
-        :param two_sided_test: flag that indicates if a two-sided test is performed
-        :param two_sided_test: bool
-        :param lambda_: weight given to recent data compared to older data
-        :type lambda_: float
-        :param min_num_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_instances: int
-        """
         super().__init__(
             alpha_d=alpha_d,
             alpha_w=alpha_w,
             two_sided_test=two_sided_test,
             min_num_instances=min_num_instances,
         )
         self.lambda_ = lambda_
@@ -317,39 +337,60 @@
         if self.y.mean - epsilon_y <= self.z.mean - epsilon_z:
             self.y = copy.deepcopy(self.z)
 
 
 class HDDMA(BaseSPC):
     """HDDM-A (Hoeffding's drift detection method with A-Test) [frias2014online]_ detector.
 
+    :param config: configuration object of the detector, defaults to None. If None, the default configuration of :class:`HDDMAConfig` is used.
+    :type config: Optional[HDDMAConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
+    :Note:
+    :func:`update` method expects to receive a value of 0 if the instance is correctly classified (no error) and 1 otherwise (error).
+
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
         810-823.
-    """
+
+    :Example:
+
+    >>> from frouros.detectors.concept_drift import HDDMA
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> dist_a = np.random.binomial(n=1, p=0.6, size=1000)
+    >>> dist_b = np.random.binomial(n=1, p=0.8, size=1000)
+    >>> stream = np.concatenate((dist_a, dist_b))
+    >>> detector = HDDMA()
+    >>> warning_flag = False
+    >>> for i, value in enumerate(stream):
+    ...     _ = detector.update(value=value)
+    ...     if detector.drift:
+    ...         print(f"Change detected at step {i}")
+    ...         break
+    ...     if not warning_flag and detector.warning:
+    ...         print(f"Warning detected at step {i}")
+    ...         warning_flag = True
+    Warning detected at step 1043
+    Change detected at step 1054
+    """  # noqa: E501  # pylint: disable=line-too-long
 
     config_type = HDDMAConfig  # type: ignore
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         config: Optional[HDDMAConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[HDDMAConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "test_type": (
                 HoeffdingTwoSidedTest(
@@ -616,39 +657,60 @@
         else:
             self.sample_decrease_2.update(value=value)
 
 
 class HDDMW(BaseSPC):
     """HDDM-W (Hoeffding's drift detection method with W-Test) [frias2014online]_ detector.
 
+    :param config: configuration object of the detector, defaults to None. If None, the default configuration of :class:`HDDMWConfig` is used.
+    :type config: Optional[HDDMWConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
+    :Note:
+    :func:`update` method expects to receive a value of 0 if the instance is correctly classified (no error) and 1 otherwise (error).
+
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
         810-823.
-    """
+
+    :Example:
+
+    >>> from frouros.detectors.concept_drift import HDDMW
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> dist_a = np.random.binomial(n=1, p=0.6, size=1000)
+    >>> dist_b = np.random.binomial(n=1, p=0.8, size=1000)
+    >>> stream = np.concatenate((dist_a, dist_b))
+    >>> detector = HDDMW()
+    >>> warning_flag = False
+    >>> for i, value in enumerate(stream):
+    ...     _ = detector.update(value=value)
+    ...     if detector.drift:
+    ...         print(f"Change detected at step {i}")
+    ...         break
+    ...     if not warning_flag and detector.warning:
+    ...         print(f"Warning detected at step {i}")
+    ...         warning_flag = True
+    Warning detected at step 1017
+    Change detected at step 1029
+    """  # noqa: E501  # pylint: disable=line-too-long
 
     config_type = HDDMWConfig  # type: ignore
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         config: Optional[HDDMWConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[HDDMWConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "test_type": (
                 McDiarmidTwoSidedTest(
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,46 +10,43 @@
 from frouros.utils.data_structures import CircularQueue
 from frouros.utils.stats import Mean
 
 
 class RDDMConfig(BaseSPCConfig):
     """RDDM (Reactive Drift detection method) [barros2017rddm]_ configuration.
 
+    :param warning_level: warning level factor, defaults to 1.773
+    :type warning_level: float
+    :param drift_level: drift level factor, defaults to 2.258
+    :type drift_level: float
+    :param max_concept_size: maximum size of a concept, defaults to 40000
+    :type max_concept_size: int
+    :param min_concept_size: reduced size of a concept, defaults to 7000
+    :type min_concept_size: int
+    :param max_num_instances_warning: maximum number of instances at warning level, defaults to 1400
+    :type max_num_instances_warning: int
+    :param min_num_instances: minimum numbers of instances to start looking for changes, defaults to 129
+    :type min_num_instances: int
+
     :References:
 
     .. [barros2017rddm] Barros, Roberto SM, et al.
         "RDDM: Reactive drift detection method."
         Expert Systems with Applications 90 (2017): 344-355.
-    """
+    """  # noqa: E501  # pylint: disable=line-too-long
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         warning_level: float = 1.773,
         drift_level: float = 2.258,
         max_concept_size: int = 40000,
         min_concept_size: int = 7000,
         max_num_instances_warning: int = 1400,
         min_num_instances: int = 129,
     ) -> None:
-        """Init method.
-
-        :param warning_level: warning level factor
-        :type warning_level: float
-        :param drift_level: drift level factor
-        :type drift_level: float
-        :param max_concept_size: maximum size of a concept
-        :type max_concept_size: int
-        :param min_concept_size: reduced size of a concept
-        :type min_concept_size: int
-        :param max_num_instances_warning: maximum number of instances at warning level
-        :type max_num_instances_warning: int
-        :param min_num_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_instances: int
-        """
         super().__init__(
             drift_level=drift_level,
             warning_level=warning_level,
             min_num_instances=min_num_instances,
         )
         self.max_concept_size = max_concept_size
         self.min_concept_size = min_concept_size
@@ -109,38 +106,59 @@
         """
         self._max_num_instances_warning = value
 
 
 class RDDM(BaseSPCError):
     """RDDM (Reactive Drift detection method) [barros2017rddm]_ detector.
 
+    :param config: configuration object of the detector, defaults to None. If None, the default configuration of :class:`RDDMConfig` is used.
+    :type config: Optional[RDDMConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
+    :Note:
+    :func:`update` method expects to receive a value of 0 if the instance is correctly classified (no error) and 1 otherwise (error).
+
     :References:
 
     .. [barros2017rddm] Barros, Roberto SM, et al.
         "RDDM: Reactive drift detection method."
         Expert Systems with Applications 90 (2017): 344-355.
-    """
+
+    :Example:
+
+    >>> from frouros.detectors.concept_drift import RDDM
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> dist_a = np.random.binomial(n=1, p=0.6, size=1000)
+    >>> dist_b = np.random.binomial(n=1, p=0.8, size=1000)
+    >>> stream = np.concatenate((dist_a, dist_b))
+    >>> detector = RDDM()
+    >>> warning_flag = False
+    >>> for i, value in enumerate(stream):
+    ...     _ = detector.update(value=value)
+    ...     if detector.drift:
+    ...         print(f"Change detected at step {i}")
+    ...         break
+    ...     if not warning_flag and detector.warning:
+    ...         print(f"Warning detected at step {i}")
+    ...         warning_flag = True
+    Warning detected at step 1036
+    Change detected at step 1066
+    """  # noqa: E501  # pylint: disable=line-too-long
 
     config_type = RDDMConfig  # type: ignore
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         config: Optional[RDDMConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[RDDMConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "num_warnings": 0,
             "rddm_drift": False,
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,46 +151,41 @@
 
         self.idx -= num_items_deleted
 
 
 class ADWINConfig(BaseWindowConfig):
     """ADWIN (ADaptive WINdowing) [bifet2007learning]_ configuration.
 
+    :param clock: clock value, default to 32
+    :type clock: int
+    :param delta: confidence value, default to 0.002
+    :type delta: float
+    :param m: controls the amount of memory used and the closeness of the cutpoints checked, default to 5
+    :type m: int
+    :param min_window_size: minimum numbers of instances per window to start looking for changes, default to 5
+    :type min_window_size: int
+    :param min_num_instances: minimum numbers of instances to start looking for changes, default to 10
+    :type min_num_instances: int
+
     :References:
 
     .. [bifet2007learning] Bifet, Albert, and Ricard Gavalda.
         "Learning from time-changing data with adaptive windowing."
         Proceedings of the 2007 SIAM international conference on data mining.
         Society for Industrial and Applied Mathematics, 2007.
-    """
+    """  # noqa: E501  # pylint: disable=line-too-long
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         clock: int = 32,
         delta: float = 0.002,
         m: int = 5,
         min_window_size: int = 5,
         min_num_instances: int = 10,
     ) -> None:
-        """Init method.
-
-        :param clock: clock value
-        :type clock: int
-        :param delta: confidence value
-        :type delta: float
-        :param m: controls the amount of memory used and
-        the closeness of the cutpoints checked
-        :type m: int
-        :param min_window_size: minimum numbers of instances
-        per window to start looking for changes
-        :type min_window_size: int
-        :param min_num_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_instances: int
-        """
         super().__init__(min_num_instances=min_num_instances)
         self.clock = clock
         self.delta = delta
         self.m = m
         self.min_window_size = min_window_size
 
     @property
@@ -278,39 +273,52 @@
             raise ValueError("min_window_size value must be greater than 0.")
         self._min_window_size = value
 
 
 class ADWIN(BaseWindow):
     """ADWIN (ADaptive WINdowing) [bifet2007learning]_ detector.
 
+    :param config: configuration object of the detector, defaults to None. If None, the default configuration of :class:`ADWINConfig` is used.
+    :type config: Optional[ADWINConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
     :References:
 
     .. [bifet2007learning] Bifet, Albert, and Ricard Gavalda.
         "Learning from time-changing data with adaptive windowing."
         Proceedings of the 2007 SIAM international conference on data mining.
         Society for Industrial and Applied Mathematics, 2007.
-    """
+
+    :Example:
+
+    >>> from frouros.detectors.concept_drift import ADWIN
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> dist_a = np.random.normal(loc=0.2, scale=0.01, size=1000)
+    >>> dist_b = np.random.normal(loc=0.8, scale=0.04, size=1000)
+    >>> stream = np.concatenate((dist_a, dist_b))
+    >>> detector = ADWIN()
+    >>> for i, value in enumerate(stream):
+    ...     _ = detector.update(value=value)
+    ...     if detector.drift:
+    ...         print(f"Change detected at step {i}")
+    ...         break
+    Change detected at step 1055
+    """  # noqa: E501  # pylint: disable=line-too-long
 
     config_type = ADWINConfig
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         config: Optional[ADWINConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[ADWINConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         num_buckets = 0
         self.additional_vars = {
             "buckets": deque([Bucket(m=self.config.m)]),  # type: ignore
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.6.0/frouros/detectors/data_drift/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,197 +1,233 @@
-"""KSWIN (Kolmogorov-Smirnov Windowing) module."""
+"""Base data drift module."""
 
-import itertools
-from collections import deque
-from typing import List, Optional, Union
+
+import abc
+import operator
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np  # type: ignore
-from scipy.stats import ks_2samp  # type: ignore
 
-from frouros.callbacks.streaming.base import BaseCallbackStreaming
-from frouros.detectors.concept_drift.streaming.window_based.base import (
-    BaseWindowConfig,
-    BaseWindow,
-)
+from frouros.callbacks.base import BaseCallback
+from frouros.detectors.base import BaseDetector
+from frouros.detectors.data_drift.exceptions import DimensionError, MissingFitError
 
 
-class KSWINConfig(BaseWindowConfig):
-    """KSWIN (Kolmogorov-Smirnov Windowing) [raab2020reactive]_ configuration.
+class BaseResult(abc.ABC):
+    """Abstract class representing a result."""
 
-    :References:
 
-    .. [raab2020reactive] Raab, Christoph, Moritz Heusinger, and Frank-Michael Schleif.
-        "Reactive soft prototype computing for concept drift streams."
-        Neurocomputing 416 (2020): 340-351.
-    """
+class BaseDataType(abc.ABC):
+    """Abstract class representing a data type."""
 
-    def __init__(
-        self,
-        alpha: float = 0.0001,
-        seed: Optional[int] = None,
-        min_num_instances: int = 100,
-        num_test_instances: int = 30,
-    ) -> None:
-        """Init method.
+    @abc.abstractmethod
+    def __init__(self) -> None:
+        """Init method."""
+
+    def __repr__(self) -> str:
+        """Repr method.
 
-        :param alpha: significance value
-        :type alpha: float
-        :param seed: seed value
-        :type seed: Optional[int]
-        :param min_num_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_instances: int
-        :param num_test_instances: numbers of instances
-        to be used by the statistical test
-        :type num_test_instances: int
-        :raises ValueError: Value error exception
+        :return: repr value
+        :rtype: str
         """
-        try:
-            np.random.seed(seed=seed)
-        except ValueError as e:
-            raise e
-        super().__init__(min_num_instances=min_num_instances)
-        self.alpha = alpha
-        self.num_test_instances = num_test_instances
+        return (
+            f"{self.__class__.__name__}"
+            f"({', '.join(f'{k}={v}' for k, v in self.__dict__.items())})"
+        )
 
-    @property
-    def alpha(self) -> float:
-        """Significance value property.
 
-        :return: significance value
-        :rtype: float
-        """
-        return self._alpha
+class CategoricalData(BaseDataType):
+    """Class representing categorical data."""
 
-    @alpha.setter
-    def alpha(self, value: int) -> None:
-        """Significance value setter.
+    def __init__(self) -> None:
+        """Init method."""
+        super().__init__()
+        self.output_type = None
 
-        :param value: value to be set
-        :type value: int
-        :raises ValueError: Value error exception
-        """
-        if value <= 0:
-            raise ValueError("alpha value must be greater than 0.")
-        self._alpha = value
 
-    @property
-    def num_test_instances(self) -> int:
-        """Number of tests instances property.
+class NumericalData(BaseDataType):
+    """Class representing numerical data."""
 
-        :return: number of tests instances to be used by the statistical test
-        :rtype: int
-        """
-        return self._num_test_instances
+    def __init__(self) -> None:
+        """Init method."""
+        super().__init__()
+        self.output_type = np.float32
 
-    @num_test_instances.setter
-    def num_test_instances(self, value: int) -> None:
-        """Number of tests instances value setter.
 
-        :param value: value to be set
-        :type value: int
-        :raises ValueError: Value error exception
+class BaseStatisticalType(abc.ABC):
+    """Abstract class representing a statistical data type."""
+
+    @abc.abstractmethod
+    def __init__(self) -> None:
+        """Init method."""
+
+    def __repr__(self) -> str:
+        """Repr method.
+
+        :return: repr value
+        :rtype: str
         """
-        if value > self.min_num_instances:
-            raise ValueError(
-                "num_test_instances value must be smaller or equal than "
-                "min_num_instances."
-            )
-        if value < 1:
-            raise ValueError("num_test_instances value must be greater than 0.")
-        self._num_test_instances = value
+        return (
+            f"{self.__class__.__name__}"
+            f"({', '.join(f'{k[1:]}={v}' for k, v in self.__dict__.items())})"
+        )
+
+
+class UnivariateData(BaseStatisticalType):
+    """Class representing a univariate data type."""
 
+    def __init__(self) -> None:
+        """Init method."""
+        super().__init__()
+        self.dim_check = operator.eq
 
-class KSWIN(BaseWindow):
-    """KSWIN (Kolmogorov-Smirnov Windowing) [raab2020reactive]_ detector.
 
-    :References:
+class MultivariateData(BaseStatisticalType):
+    """Class representing a multivariate data type."""
 
-    .. [raab2020reactive] Raab, Christoph, Moritz Heusinger, and Frank-Michael Schleif.
-        "Reactive soft prototype computing for concept drift streams."
-        Neurocomputing 416 (2020): 340-351.
-    """
+    def __init__(self) -> None:
+        """Init method."""
+        super().__init__()
+        self.dim_check = operator.ge
 
-    config_type = KSWINConfig
+
+class BaseDataDrift(BaseDetector):
+    """Abstract class representing a data drift detector."""
 
     def __init__(
         self,
-        config: Optional[KSWINConfig] = None,
-        callbacks: Optional[
-            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
-        ] = None,
+        data_type: BaseDataType,
+        statistical_type: BaseStatisticalType,
+        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
-        :param config: configuration parameters
-        :type config: Optional[KSWINConfig]
+        :param data_type: data type
+        :type data_type: BaseDataType
+        :param statistical_type: statistical type
+        :type statistical_type: BaseStatisticalType
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
+        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
         """
-        super().__init__(
-            config=config,
-            callbacks=callbacks,
-        )
-        self.additional_vars = {
-            "window": deque(maxlen=self.config.min_num_instances),
-        }
-        self._set_additional_vars_callback()
+        super().__init__(callbacks=callbacks)
+        self.data_type = data_type
+        self.statistical_type = statistical_type
+        self.X_ref = None  # type: ignore
+
+    @property
+    def data_type(self) -> BaseDataType:
+        """Data type property.
+
+        :return: data type
+        :rtype: BaseDataType
+        """
+        return self._data_type
+
+    @data_type.setter
+    def data_type(self, value: BaseDataType) -> None:
+        """Data type setter.
+
+        :param value: value to be set
+        :type value: BaseDataType
+        :raises TypeError: Type error exception
+        """
+        if not isinstance(value, BaseDataType):
+            raise TypeError("value must be of type BaseDataType.")
+        self._data_type = value
 
     @property
-    def window(self) -> deque:
-        """Window queue property.
+    def statistical_type(self) -> BaseStatisticalType:
+        """Statistical type property.
 
-        :return: window queue
-        :rtype: deque
+        :return: statistical type
+        :rtype: BaseStatisticalType
         """
-        return self._additional_vars["window"]
+        return self._statistical_type
 
-    @window.setter
-    def window(self, value: deque) -> None:
-        """Window queue setter.
+    @statistical_type.setter
+    def statistical_type(self, value: BaseStatisticalType) -> None:
+        """Statistical type setter.
 
         :param value: value to be set
-        :type value: deque
+        :type value: BaseStatisticalType
         :raises TypeError: Type error exception
         """
-        if not isinstance(value, deque):
-            raise TypeError("value must be of type deque.")
-        self._additional_vars["window"] = value
-
-    def _update(self, value: Union[int, float], **kwargs) -> None:
-        self.num_instances += 1
-
-        self.window.append(value)
-
-        window_size = len(self.window)
-        if window_size >= self.config.min_num_instances:
-            # fmt: off
-            num_first_samples = window_size - self.config.num_test_instances  # type: ignore # noqa: E501 pylint: disable=line-too-long
-            r_samples = [*itertools.islice(self.window,
-                                           num_first_samples,
-                                           window_size)]
-            w_samples = np.random.choice(
-                a=[*itertools.islice(self.window, 0, num_first_samples)],
-                size=self.config.num_test_instances,  # type: ignore
-                replace=False,
+        if not isinstance(value, BaseStatisticalType):
+            raise TypeError("value must be of type BaseStatisticalType.")
+        self._statistical_type = value
+
+    @property
+    def X_ref(self) -> Optional[np.ndarray]:  # noqa: N802
+        """Reference data property.
+
+        :return: reference data
+        :rtype: Optional[numpy.ndarray]
+        """
+        return self._X_ref  # type: ignore # pylint: disable=E1101
+
+    @X_ref.setter  # type: ignore
+    def X_ref(self, value: Optional[np.ndarray]) -> None:  # noqa: N802
+        """Reference data setter.
+
+        :param value: value to be set
+        :type value: Optional[numpy.ndarray]
+        """
+        if value is not None:
+            self._check_array(X=value)
+        self._X_ref = value
+
+    def fit(self, X: np.ndarray, **kwargs) -> Dict[str, Any]:  # noqa: N803
+        """Fit detector.
+
+        :param X: feature data
+        :type X: numpy.ndarray
+        :return: callbacks logs
+        :rtype: Dict[str, Any]
+        """
+        self._check_fit_dimensions(X=X)
+        for callback in self.callbacks:  # type: ignore
+            callback.on_fit_start(
+                X=X,
             )
-            # fmt: on
-            _, p_value = ks_2samp(
-                data1=w_samples,
-                data2=r_samples,
-                alternative="two-sided",
-                method="auto",
+        self._fit(X=X, **kwargs)
+        for callback in self.callbacks:  # type: ignore
+            callback.on_fit_end(
+                X=X,
             )
 
-            if p_value <= self.config.alpha:  # type: ignore
-                # Drift detected
-                self.drift = True
-            else:
-                self.drift = False
-        else:
-            self.drift = False
+        callbacks_logs = self._get_callbacks_logs()
+        return callbacks_logs
 
     def reset(self) -> None:
         """Reset method."""
-        super().reset()
-        self.window.clear()
+        self.X_ref = None
+
+    def _check_fit_dimensions(self, X: np.ndarray) -> None:  # noqa: N803
+        try:
+            if not self.statistical_type.dim_check(X.shape[1], 1):  # type: ignore
+                raise DimensionError(f"Dimensions of X ({X.shape[-1]})")
+        except IndexError as e:
+            if not self.statistical_type.dim_check(X.ndim, 1):  # type: ignore
+                raise DimensionError(f"Dimensions of X ({X.ndim})") from e
+
+    def _check_is_fitted(self):
+        if self.X_ref is None:
+            raise MissingFitError("fit method has not been called")
+
+    def _common_checks(self) -> None:  # noqa: N803
+        self._check_is_fitted()
+
+    @abc.abstractmethod
+    def _fit(self, X: np.ndarray) -> None:  # noqa: N803
+        pass
+
+    def __repr__(self) -> str:
+        """Repr method.
+
+        :return: repr value
+        :rtype: str
+        """
+        return (
+            f"{super().__repr__()[:-1]}, "
+            f"data_type={self.data_type}, "
+            f"statistical_type={self.statistical_type})"
+        )
```

### Comparing `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.6.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,37 +12,34 @@
 )
 from frouros.utils.data_structures import AccuracyQueue
 
 
 class STEPDConfig(BaseWindowConfig):
     """STEPD (Statistical test of equal proportions) [nishida2007detecting]_ configuration.
 
+    :param alpha_d: significance value for overall, defaults to 0.003
+    :type alpha_d: float
+    :param alpha_w: significance value for last, defaults to 0.05
+    :type alpha_w: float
+    :param min_num_instances: minimum numbers of instances to start looking for changes, defaults to 30
+    :type min_num_instances: int
+
     :References:
 
     .. [nishida2007detecting] Nishida, Kyosuke, and Koichiro Yamauchi.
         "Detecting concept drift using statistical testing." Discovery science.
         Vol. 4755. 2007.
-    """
+    """  # noqa: E501  # pylint: disable=line-too-long
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         alpha_d: float = 0.003,
         alpha_w: float = 0.05,
         min_num_instances: int = 30,
     ) -> None:
-        """Init method.
-
-        :param alpha_d: significance value for overall
-        :type alpha_d: float
-        :param alpha_w: significance value for last
-        :type alpha_w: float
-        :param min_num_instances: minimum numbers of instances
-        to start looking for changes
-        :type min_num_instances: int
-        """
         super().__init__(min_num_instances=min_num_instances)
         self.alpha_d = alpha_d
         self.alpha_w = alpha_w
 
     @property
     def alpha_d(self) -> float:
         """Significance level d property.
@@ -87,38 +84,56 @@
             raise ValueError("alpha_w must be greater than alpha_d.")
         self._alpha_w = value
 
 
 class STEPD(BaseWindow):
     """STEPD (Statistical test of equal proportions) [nishida2007detecting]_ detector.
 
+    :param config: configuration object of the detector, defaults to None. If None, the default configuration of :class:`STEPDConfig` is used.
+    :type config: Optional[STEPDConfig]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
     :References:
 
     .. [nishida2007detecting] Nishida, Kyosuke, and Koichiro Yamauchi.
         "Detecting concept drift using statistical testing." Discovery science.
         Vol. 4755. 2007.
-    """
+
+    :Example:
+
+    >>> from frouros.detectors.concept_drift import STEPD, STEPDConfig
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> dist_a = np.random.binomial(n=1, p=0.8, size=1000)
+    >>> dist_b = np.random.binomial(n=1, p=0.5, size=1000)
+    >>> stream = np.concatenate((dist_a, dist_b))
+    >>> detector = STEPD(config=STEPDConfig(alpha_d=0.001, alpha_w=0.005))
+    >>> for i, value in enumerate(stream):
+    ...     _ = detector.update(value=value)
+    ...     if detector.drift:
+    ...         print(f"Change detected at step {i}")
+    ...         break
+    ...     if detector.warning:
+    ...         print(f"Warning detected at step {i}")
+    Warning detected at step 640
+    Warning detected at step 641
+    Warning detected at step 1023
+    Change detected at step 1024
+    """  # noqa: E501  # pylint: disable=line-too-long
 
     config_type = STEPDConfig  # type: ignore
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         config: Optional[STEPDConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param config: configuration parameters
-        :type config: Optional[STEPDConfig]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "correct_total": 0,
             # FIXME include get method in AccuracyQueue  # pylint: disable=fixme
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/__init__.py` & `frouros-0.6.0/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/base.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def compare(
         self,
         X: np.ndarray,  # noqa: N803
         **kwargs,
     ) -> Tuple[np.ndarray, Dict[str, Any]]:
         """Compare values.
 
-        :param X: feature data
+        :param X: test data
         :type X: numpy.ndarray
         :return: compare result and callbacks logs
         :rtype: Tuple[numpy.ndarray, Dict[str, Any]]
         """
         for callback in self.callbacks:  # type: ignore
             callback.on_compare_start(  # type: ignore
                 X_ref=self.X_ref,
@@ -93,26 +93,33 @@
                 raise MismatchDimensionError(f"Dimensions of X ({X.ndim})") from e
 
     def _specific_checks(self, X: np.ndarray) -> None:  # noqa: N803
         self._check_compare_dimensions(X=X)
 
     @abc.abstractmethod
     def _apply_method(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        self,
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs,
     ) -> Any:
         pass
 
     @abc.abstractmethod
     def _compare(
         self,
         X: np.ndarray,  # noqa: N803
         **kwargs,
     ) -> np.ndarray:
         pass
 
     def _get_result(
-        self, X: np.ndarray, **kwargs  # noqa: N803
+        self,
+        X: np.ndarray,  # noqa: N803
+        **kwargs,
     ) -> Union[List[float], List[Tuple[float, float]], Tuple[float, float]]:
         result = self._apply_method(  # type: ignore # pylint: disable=not-callable
-            X_ref=self.X_ref, X=X, **kwargs
+            X_ref=self.X_ref,
+            X=X,
+            **kwargs,
         )
         return result
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,33 +9,43 @@
     BaseDistanceBasedBins,
 )
 
 
 class BhattacharyyaDistance(BaseDistanceBasedBins):
     """Bhattacharyya distance [bhattacharyya1946measure]_ detector.
 
+    :param num_bins: number of bins in which to divide probabilities, defaults to 10
+    :type num_bins: int
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+
     :References:
 
     .. [bhattacharyya1946measure] Bhattacharyya, Anil.
         "On a measure of divergence between two multinomial populations."
         Sankhyā: the indian journal of statistics (1946): 401-406.
+
+    :Example:
+
+    >>> from frouros.detectors.data_drift import BhattacharyyaDistance
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = BhattacharyyaDistance(num_bins=20)
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)
+    DistanceResult(distance=0.2182101059622703)
     """
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param num_bins: number of bins in which to divide probabilities
-        :type num_bins: int
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
-        """
         super().__init__(
             statistical_method=self._bhattacharyya,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,31 +12,43 @@
     DistanceResult,
 )
 
 
 class EMD(BaseDistanceBased):
     """EMD (Earth Mover's Distance) [rubner2000earth]_ detector.
 
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+    :param kwargs: additional keyword arguments to pass to scipy.stats.wasserstein_distance
+    :type kwargs: Dict[str, Any]
+
     :References:
 
     .. [rubner2000earth] Rubner, Yossi, Carlo Tomasi, and Leonidas J. Guibas.
         "The earth mover's distance as a metric for image retrieval."
         International journal of computer vision 40.2 (2000): 99.
-    """
 
-    def __init__(
+    :Example:
+
+    >>> from frouros.detectors.data_drift import EMD
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = EMD()
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    DistanceResult(distance=1.0686078744674332)
+    """  # noqa: E501
+
+    def __init__(  # noqa: D107
         self,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         **kwargs,
     ) -> None:
-        """Init method.
-
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=self._emd,
             statistical_kwargs=kwargs,
             callbacks=callbacks,
         )
         self.kwargs = kwargs
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,34 +9,44 @@
     BaseDistanceBasedBins,
 )
 
 
 class HellingerDistance(BaseDistanceBasedBins):
     """Hellinger distance [hellinger1909neue]_ detector.
 
+    :param num_bins: number of bins in which to divide probabilities, defaults to 10
+    :type num_bins: int
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+
     :References:
 
     .. [hellinger1909neue] Hellinger, Ernst.
         "Neue begründung der theorie quadratischer formen von unendlichvielen
         veränderlichen."
         Journal für die reine und angewandte Mathematik 1909.136 (1909): 210-271.
+
+    :Example:
+
+    >>> from frouros.detectors.data_drift import HellingerDistance
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = HellingerDistance(num_bins=20)
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    DistanceResult(distance=0.467129645775421)
     """
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param num_bins: number of bins in which to divide probabilities
-        :type num_bins: int
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         sqrt_div = np.sqrt(2)
         super().__init__(
             statistical_method=self._hellinger,
             statistical_kwargs={
                 "num_bins": num_bins,
                 "sqrt_div": sqrt_div,
             },
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,43 @@
     BaseDistanceBasedBins,
 )
 
 
 class HINormalizedComplement(BaseDistanceBasedBins):
     """HI (Histogram intersection) normalized complement [swain1991color]_ detector.
 
+    :param num_bins: number of bins in which to divide probabilities, defaults to 10
+    :type num_bins: int
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+
     :References:
 
     .. [swain1991color] Swain, M. J., and D. H. Ballard.
         "Color Indexing International Journal of Computer
         Vision 7." (1991): 11-32.
+
+    :Example:
+
+    >>> from frouros.detectors.data_drift import HINormalizedComplement
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = HINormalizedComplement(num_bins=20)
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    DistanceResult(distance=0.53)
     """
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param num_bins: number of bins in which to divide probabilities
-        :type num_bins: int
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             statistical_method=self._hi_normalized_complement,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,34 +11,46 @@
     DistanceResult,
 )
 
 
 class JS(BaseDistanceBasedProbability):
     """JS (Jensen-Shannon distance) [lin1991divergence]_ detector.
 
+    :param num_bins: number of bins in which to divide probabilities, defaults to 10
+    :type num_bins: int
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+    :param kwargs: additional keyword arguments to pass to scipy.spatial.distance.jensenshannon
+    :type kwargs: Dict[str, Any]
+
     :References:
 
     .. [lin1991divergence] Lin, Jianhua.
         "Divergence measures based on the Shannon entropy."
         IEEE Transactions on Information theory 37.1 (1991): 145-151.
-    """
 
-    def __init__(
+    :Example:
+
+    >>> from frouros.detectors.data_drift import JS
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = JS(num_bins=20)
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    DistanceResult(distance=0.41702877367162156)
+    """  # noqa: E501
+
+    def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         **kwargs,
     ) -> None:
-        """Init method.
-
-        :param num_bins: number of bins in which to divide probabilities
-        :type num_bins: int
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             statistical_method=self._js,
             statistical_kwargs={
                 "num_bins": num_bins,
                 **kwargs,
             },
             callbacks=callbacks,
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,34 +11,46 @@
     DistanceResult,
 )
 
 
 class KL(BaseDistanceBasedProbability):
     """KL (Kullback-Leibler divergence) [kullback1951information]_ detector.
 
+    :param num_bins: number of bins in which to divide probabilities, defaults to 10
+    :type num_bins: int
+    :param callbacks: number of bins in which to divide probabilities, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+    :param kwargs: additional keyword arguments to pass to scipy.special.rel_entr
+    :type kwargs: Dict[str, Any]
+
     :References:
 
     .. [kullback1951information] Kullback, Solomon, and Richard A. Leibler.
         "On information and sufficiency."
         The annals of mathematical statistics 22.1 (1951): 79-86.
+
+    :Example:
+
+    >>> from frouros.detectors.data_drift import KL
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = KL(num_bins=20)
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    DistanceResult(distance=inf)
     """
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         **kwargs,
     ) -> None:
-        """Init method.
-
-        :param num_bins: number of bins in which to divide probabilities
-        :type num_bins: int
-        :param callbacks: number of bins in which to divide probabilities
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             statistical_method=self._kl,
             statistical_kwargs={**kwargs, "num_bins": num_bins},
             callbacks=callbacks,
         )
         self.num_bins = num_bins
         self.kwargs = kwargs
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,36 +15,48 @@
 )
 from frouros.utils.kernels import rbf_kernel
 
 
 class MMD(BaseDistanceBased):
     """MMD (Maximum Mean Discrepancy) [gretton2012kernel]_ detector.
 
+    :param kernel: kernel function, defaults to :func:`rbf_kernel() <frouros.utils.kernels.rbf_kernel>`
+    :type kernel: Callable
+    :param chunk_size: chunk size value, defaults to None
+    :type chunk_size: Optional[int]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+
     :References:
 
     .. [gretton2012kernel] Gretton, Arthur, et al.
         "A kernel two-sample test."
         The Journal of Machine Learning Research 13.1 (2012): 723-773.
-    """
 
-    def __init__(
+    :Example:
+
+    >>> from functools import partial
+    >>> from frouros.detectors.data_drift import MMD
+    >>> from frouros.utils.kernels import rbf_kernel
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.multivariate_normal(mean=[1, 1], cov=[[2, 0], [0, 2]], size=100)
+    >>> Y = np.random.multivariate_normal(mean=[0, 0], cov=[[2, 1], [1, 2]], size=100)
+    >>> detector = MMD(kernel=partial(rbf_kernel, sigma=0.5))
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    DistanceResult(distance=0.02146955300299802)
+    """  # noqa: E501  # pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
         self,
         kernel: Callable = rbf_kernel,
         chunk_size: Optional[int] = None,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param kernel: kernel function
-        :type kernel: Callable
-        :param chunk_size: chunk size value
-        :type chunk_size: Optional[int]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             statistical_type=MultivariateData(),
             statistical_method=self._mmd,
             statistical_kwargs={
                 "kernel": kernel,
             },
             callbacks=callbacks,
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,33 +11,43 @@
     DistanceResult,
 )
 
 
 class PSI(BaseDistanceBasedBins):
     """PSI (Population Stability Index) [wu2010enterprise]_ detector.
 
+    :param num_bins: number of bins in which to divide probabilities, defaults to 10
+    :type num_bins: int
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+
     :References:
 
     .. [wu2010enterprise] Wu, Desheng, and David L. Olson.
         "Enterprise risk management: coping with model risk in a large bank."
         Journal of the Operational Research Society 61.2 (2010): 179-190.
+
+    :Example:
+
+    >>> from frouros.detectors.data_drift import PSI
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = PSI(num_bins=20)
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    DistanceResult(distance=134.95409065116183)
     """
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param num_bins: number of bins in which to divide probabilities
-        :type num_bins: int
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             statistical_method=self._psi,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,42 +12,55 @@
     StatisticalResult,
 )
 
 
 class AndersonDarlingTest(BaseStatisticalTest):
     """Anderson-Darling test [scholz1987k]_ detector.
 
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+
     :Note:
-     p-values are bounded between 0.001 and 0.25 according to scipy documentation [1]_.
+    - Passing additional arguments to `scipy.stats.anderson_ksamp <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.anderson_ksamp.html>`__ can be done using :func:`compare` kwargs.
+    - p-values are bounded between 0.001 and 0.25 according to `scipy.stats.anderson_ksamp <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.anderson_ksamp.html>`__.
 
     :References:
 
     .. [scholz1987k] Scholz, Fritz W., and Michael A. Stephens.
         "K-sample Anderson–Darling tests."
         Journal of the American Statistical Association 82.399 (1987): 918-924.
-       [1] https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.anderson_ksamp.html  # noqa: E501 # pylint: disable=line-too-long
-    """
 
-    def __init__(
+    :Example:
+
+    >>> from frouros.detectors.data_drift import AndersonDarlingTest
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = AndersonDarlingTest()
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    StatisticalResult(statistic=32.40316586267425, p_value=0.001)
+    """  # noqa: E501  # pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
         self,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
 
+    @staticmethod
     def _statistical_test(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs,
     ) -> StatisticalResult:
         test = anderson_ksamp(
             samples=[
                 X_ref,
                 X,
             ],
             **kwargs,
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,27 +11,37 @@
 StatisticalResult = namedtuple("StatisticalResult", ["statistic", "p_value"])
 
 
 class BaseStatisticalTest(BaseDataDriftBatch):
     """Abstract class representing a statistical test."""
 
     def _apply_method(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        self,
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs,
     ) -> Tuple[float, float]:
-        statistical_test = self._statistical_test(X_ref=X_ref, X=X, **kwargs)
+        statistical_test = self._statistical_test(
+            X_ref=X_ref,
+            X=X,
+            **kwargs,
+        )
         return statistical_test
 
     def _compare(
         self,
         X: np.ndarray,  # noqa: N803
         **kwargs,
     ) -> StatisticalResult:
         self._common_checks()  # noqa: N806
         self._specific_checks(X=X)  # noqa: N806
         result = self._get_result(X=X, **kwargs)
         return result  # type: ignore
 
+    @staticmethod
     @abc.abstractmethod
     def _statistical_test(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
-    ) -> Tuple[float, float]:
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs,
+    ) -> StatisticalResult:
         pass
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,53 +13,77 @@
     StatisticalResult,
 )
 
 
 class ChiSquareTest(BaseStatisticalTest):
     """ChiSquareTest (Chi-square test) [pearson1900x]_ detector.
 
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+
+    :Note:
+    - Passing additional arguments to `scipy.stats.chi2_contingency <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.chi2_contingency.html>`__ can be done using :func:`compare` kwargs.
+
     :References:
 
     .. [pearson1900x] Pearson, Karl.
         "X. On the criterion that a given system of deviations from the probable in the
         case of a correlated system of variables is such that it can be reasonably
         supposed to have arisen from random sampling."
         The London, Edinburgh, and Dublin Philosophical Magazine and Journal of
         Science 50.302 (1900): 157-175.
-    """
 
-    def __init__(
+    :Example:
+
+    >>> from frouros.detectors.data_drift import ChiSquareTest
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.choice(a=[0, 1], size=100, p=[0.5, 0.5])
+    >>> Y = np.random.choice(a=[0, 1], size=100, p=[0.8, 0.2])
+    >>> detector = ChiSquareTest()
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    StatisticalResult(statistic=9.81474665685192, p_value=0.0017311812135839511)
+    """  # noqa: E501  # pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
         self,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             data_type=CategoricalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
 
+    @staticmethod
     def _statistical_test(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs,
     ) -> StatisticalResult:
-        f_exp, f_obs = self._calculate_frequencies(X_ref=X_ref, X=X)
+        f_exp, f_obs = ChiSquareTest._calculate_frequencies(
+            X_ref=X_ref,
+            X=X,
+        )
         statistic, p_value, _, _ = chi2_contingency(
-            observed=np.array([f_obs, f_exp]), **kwargs
+            observed=np.array([f_obs, f_exp]),
+            **kwargs,
         )
 
-        test = StatisticalResult(statistic=statistic, p_value=p_value)
+        test = StatisticalResult(
+            statistic=statistic,
+            p_value=p_value,
+        )
         return test
 
     @staticmethod
     def _calculate_frequencies(
-        X_ref: np.ndarray, X: np.ndarray  # noqa: N803
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
     ) -> Tuple[List[int], List[int]]:
         X_ref_counter, X_counter = [  # noqa: N806
             *map(collections.Counter, [X_ref, X])  # noqa: N806
         ]
         possible_values = set([*X_ref_counter.keys()] + [*X_counter.keys()])
         f_exp, f_obs = {}, {}
         for value in possible_values:
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.6.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,30 +13,43 @@
 )
 from frouros.detectors.data_drift.exceptions import InsufficientSamplesError
 
 
 class CVMTest(BaseStatisticalTest):
     """CVMTest (Cramér-von Mises test) [cramer1928composition]_ detector.
 
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
+
+    :Note:
+    - Passing additional arguments to `scipy.stats.cramervonmises_2samp <https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.cramervonmises_2samp.html>`__ can be done using :func:`compare` kwargs.
+
     :References:
 
     .. [cramer1928composition] Cramér, Harald.
         "On the composition of elementary errors: First paper: Mathematical deductions."
         Scandinavian Actuarial Journal 1928.1 (1928): 13-74.
-    """
 
-    def __init__(
+    :Example:
+
+    >>> from frouros.detectors.data_drift import CVMTest
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = CVMTest()
+    >>> _ = detector.fit(X=X)
+    >>> detector.compare(X=Y)[0]
+    StatisticalResult(statistic=5.331699999999998, p_value=1.7705426014202885e-10)
+    """  # noqa: E501  # pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
         self,
         callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
-        """Init method.
-
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
-        """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
 
     @BaseStatisticalTest.X_ref.setter  # type: ignore[attr-defined]
@@ -57,17 +70,23 @@
         self._check_sufficient_samples(X=X)
 
     @staticmethod
     def _check_sufficient_samples(X: np.ndarray) -> None:  # noqa: N803
         if X.shape[0] < 2:
             raise InsufficientSamplesError("Number of samples must be at least 2.")
 
+    @staticmethod
     def _statistical_test(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs,
     ) -> StatisticalResult:
         test = cramervonmises_2samp(
             x=X_ref,
             y=X,
-            method=kwargs.get("method", "auto"),
+            **kwargs,
+        )
+        test = StatisticalResult(
+            statistic=test.statistic,
+            p_value=test.pvalue,
         )
-        test = StatisticalResult(statistic=test.statistic, p_value=test.pvalue)
         return test
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.6.0/frouros/detectors/data_drift/streaming/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,35 +52,37 @@
     def reset(self) -> None:
         """Reset method."""
         super().reset()
         self.num_instances = 0
         self._reset()
 
     def update(
-        self, value: Union[int, float]
+        self,
+        value: Union[int, float],
     ) -> Tuple[Optional[BaseResult], Dict[str, Any]]:
         """Update detector.
 
         :param value: value to use to update the detector
         :type value: Union[int, float]
-        :return: update result
-        :rtype: Optional[BaseResult]
+        :return: update result and callbacks logs
+        :rtype: Tuple[Optional[BaseResult], Dict[str, Any]]
         """
         self._common_checks()  # noqa: N806
         self._specific_checks(X=value)  # noqa: N806
         self.num_instances += 1
 
         for callback in self.callbacks:  # type: ignore
-            callback.on_update_start(value=value)  # type: ignore
+            callback.on_update_start(  # type: ignore
+                value=value,  # type: ignore
+            )
         result = self._update(value=value)
-        if result is not None:
-            for callback in self.callbacks:  # type: ignore
-                callback.on_update_end(  # type: ignore
-                    value=result.distance,  # type: ignore
-                )
+        for callback in self.callbacks:  # type: ignore
+            callback.on_update_end(  # type: ignore
+                value=result,  # type: ignore
+            )
 
         callbacks_logs = self._get_callbacks_logs()
         return result, callbacks_logs
 
     def _specific_checks(self, X: np.ndarray) -> None:  # noqa: N803
         pass
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.6.0/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.6.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,42 +14,56 @@
 )
 from frouros.utils.data_structures import CircularQueue
 
 
 class MMD(BaseDistanceBased):
     """MMD (Maximum Mean Discrepancy) [gretton2012kernel]_ detector.
 
+    :param window_size: window size value
+    :type window_size: int
+    :param kernel: kernel function, defaults to :func:`rbf_kernel() <frouros.utils.kernels.rbf_kernel>`
+    :type kernel: Callable
+    :param chunk_size: chunk size value, defaults to None
+    :type chunk_size: Optional[int]
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming,
+    List[BaseCallbackStreaming]]]
+
     :References:
 
     .. [gretton2012kernel] Gretton, Arthur, et al.
         "A kernel two-sample test."
         The Journal of Machine Learning Research 13.1 (2012): 723-773.
-    """
 
-    def __init__(
+    :Example:
+
+    >>> from functools import partial
+    >>> from frouros.detectors.data_drift import MMDStreaming
+    >>> from frouros.utils.kernels import rbf_kernel
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.multivariate_normal(mean=[1, 1], cov=[[2, 0], [0, 2]], size=100)
+    >>> Y = np.random.multivariate_normal(mean=[0, 0], cov=[[2, 1], [1, 2]], size=100)
+    >>> detector = MMDStreaming(window_size=10, kernel=partial(rbf_kernel, sigma=0.5))
+    >>> _ = detector.fit(X=X)
+    >>> for sample in Y:
+    ...     distance, _ = detector.update(value=sample)
+    ...     if distance is not None:
+    ...         print(distance)
+    """  # noqa: E501  # pylint: disable=line-too-long
+
+    def __init__(  # noqa: D107
         self,
         window_size: int,
         kernel: Callable = rbf_kernel,
         chunk_size: Optional[int] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
-        """Init method.
-
-        :param window_size: window size
-        :type window_size: int
-        :param kernel: kernel function
-        :type kernel: Callable
-        :param chunk_size: chunk size value
-        :type chunk_size: Optional[int]
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=MultivariateData(),
             callbacks=callbacks,
         )
         self.mmd = MMDBatch(
             kernel=kernel,
```

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.6.0/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.6.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,38 +26,49 @@
 # Value used in scipy
 MAX_AUTO_N = 10000
 
 
 class IncrementalKSTest(BaseStatisticalTest):
     """IncrementalKSTest (Incremental Kolmogorov-Smirnov test) [dos2016fast]_ detector.
 
+    :param window_size: window size value
+    :type window_size: int
+    :param callbacks: callbacks, defaults to None
+    :type callbacks: Optional[Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]]
+
     :References:
 
     .. [dos2016fast] dos Reis, Denis Moreira, et al.
         "Fast unsupervised online drift detection using incremental kolmogorov-smirnov
         test."
         Proceedings of the 22nd ACM SIGKDD international conference on knowledge
         discovery and data mining. 2016.
+
+    :Example:
+
+    >>> from frouros.detectors.data_drift import IncrementalKSTest
+    >>> import numpy as np
+    >>> np.random.seed(seed=31)
+    >>> X = np.random.normal(loc=0, scale=1, size=100)
+    >>> Y = np.random.normal(loc=1, scale=1, size=100)
+    >>> detector = IncrementalKSTest(window_size=10)
+    >>> _ = detector.fit(X=X)
+    >>> for sample in Y:
+    ...     test, _ = detector.update(value=sample)
+    ...     if test is not None:
+    ...         print(test.statistic, test.p_value)
     """
 
-    def __init__(
+    def __init__(  # noqa: D107
         self,
+        window_size: int,
         callbacks: Optional[
             Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
         ] = None,
-        window_size: int = 10,
     ) -> None:
-        """Init method.
-
-        :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallbackStreaming,
-        List[BaseCallbackStreaming]]]
-        :param window_size: window size
-        :type window_size: int
-        """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
         self.window_size = window_size
         self.gcd = None
```

### Comparing `frouros-0.5.1/frouros/metrics/base.py` & `frouros-0.6.0/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/tests/conftest.py` & `frouros-0.6.0/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/tests/integration/test_concept_drift.py` & `frouros-0.6.0/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/tests/integration/test_data_drift.py` & `frouros-0.6.0/frouros/tests/integration/test_data_drift.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     with pytest.raises(expected_exception):
         _ = MMD(chunk_size=chunk_size)  # type: ignore
 
 
 @pytest.mark.parametrize(
     "detector, expected_statistic, expected_p_value",
     [
-        (IncrementalKSTest(), 0.27, 0.46046910),
+        (IncrementalKSTest(window_size=10), 0.27, 0.46046910),
     ],
 )
 def test_streaming_statistical_univariate_same_distribution(
     univariate_distribution_p: Tuple[float, float],
     detector: BaseDataDriftBatch,
     expected_statistic: float,
     expected_p_value: float,
@@ -336,15 +336,15 @@
     assert np.isclose(test.statistic, expected_statistic)
     assert np.isclose(test.p_value, expected_p_value)
 
 
 @pytest.mark.parametrize(
     "detector, expected_statistic, expected_p_value",
     [
-        (IncrementalKSTest(), 1.0, 0.0),
+        (IncrementalKSTest(window_size=10), 1.0, 0.0),
     ],
 )
 def test_streaming_statistical_univariate_different_distribution(
     univariate_distribution_p: Tuple[float, float],
     univariate_distribution_q: Tuple[float, float],
     detector: BaseDataDriftBatch,
     expected_statistic: float,
```

### Comparing `frouros-0.5.1/frouros/tests/integration/test_real.py` & `frouros-0.6.0/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/tests/integration/test_synthetic.py` & `frouros-0.6.0/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.6.0/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/utils/checks.py` & `frouros-0.6.0/frouros/utils/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Checks module."""
 
 from typing import Any
 
 from frouros.callbacks.base import BaseCallback
 
 
-def check_callbacks(callbacks: Any, expected_cls: BaseCallback) -> None:
+def check_callbacks(
+    callbacks: Any,
+    expected_cls: BaseCallback,
+) -> None:
     """Check callbacks.
 
     :param callbacks: callbacks
     :type callbacks: Any
     :param expected_cls: expected callback class
     :type expected_cls: BaseCallback
     :raises TypeError: Type error exception
```

### Comparing `frouros-0.5.1/frouros/utils/data_structures.py` & `frouros-0.6.0/frouros/utils/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 """Data structures module."""
 
-from typing import Any, Optional, List, Union
+from typing import Any, Optional, List, Union, Dict, Tuple
 
 import numpy as np  # type: ignore
 
 
 class EmptyQueueError(Exception):
-    """Empty queue exception."""
+    """Empty queue exception.
 
-    def __init__(self, *args, msg="Queue is empty.", **kwargs) -> None:
-        """Init method.
-
-        :param msg: exception message
-        :type msg: str
-        """
-        super().__init__(msg, *args, **kwargs)
+    :param args: exception arguments
+    :type args: Tuple[Any, ...]
+    :param msg: exception message, defaults to "Queue is empty."
+    :type msg: str
+    :param kwargs: exception keyword arguments
+    :type kwargs: Dict[str, Dict[str, Any]]
+    """
+
+    def __init__(  # noqa: D107
+        self,
+        *args: Tuple[Any, ...],
+        msg: str = "Queue is empty.",
+        **kwargs: Dict[str, Dict[str, Any]],
+    ) -> None:
+        super().__init__(
+            msg,
+            *args,
+            **kwargs,
+        )
 
 
 class CircularQueue:
-    """Class representing a circular queue."""
-
-    def __init__(self, max_len: int) -> None:
-        """Init method.
+    """Class representing a circular queue.
 
-        :param max_len: maximum capacity
-        :type max_len: int
-        """
+    :param max_len: maximum capacity
+    :type max_len: int
+    """
+
+    def __init__(  # noqa: D107
+        self,
+        max_len: int,
+    ) -> None:
         self.count = 0
         self.first = 0
         self.last = -1
         self.max_len = max_len
         self.queue = [None] * self.max_len
 
     @property
@@ -214,22 +228,24 @@
         :return: queue item
         :rtype: Any
         """
         return self.queue[idx]  # type: ignore
 
 
 class AccuracyQueue(CircularQueue):
-    """Class representing an accuracy queue."""
-
-    def __init__(self, max_len: int) -> None:
-        """Init method.
+    """Class representing an accuracy queue.
 
-        :param max_len: maximum capacity
-        :type max_len: int
-        """
+    :param max_len: maximum capacity
+    :type max_len: int
+    """
+
+    def __init__(  # noqa: D107
+        self,
+        max_len: int,
+    ) -> None:
         super().__init__(max_len=max_len)
         self.num_true = 0
 
     @property
     def num_false(self):
         """Number of false label property.
```

### Comparing `frouros-0.5.1/frouros/utils/kernels.py` & `frouros-0.6.0/frouros/utils/kernels.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.1/frouros/utils/stats.py` & `frouros-0.6.0/frouros/utils/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,16 +32,17 @@
     def get(self) -> float:
         """Get method."""
 
 
 class Mean(IncrementalStat):
     """Incremental mean class."""
 
-    def __init__(self) -> None:
-        """Init method."""
+    def __init__(  # noqa: D107
+        self,
+    ) -> None:
         self.mean = 0.0
         self.num_values = 0
 
     @property
     def mean(self) -> float:
         """Mean property.
 
@@ -83,16 +84,16 @@
     def update(self, value: Union[int, float]) -> None:
         """Update the mean value sequentially.
 
         :param value: value to use to update the mean
         :type value: int
         :raises TypeError: Type error exception
         """
-        if not isinstance(value, (int, float)):
-            raise TypeError("value must be of type int or float.")
+        if not isinstance(value, (int, float, np.number)):
+            raise TypeError("value must be of type int, float or numpy number.")
         self.num_values += 1
         self.mean += self.incremental_op(
             value=value,
             element=self.mean,
             size=self.num_values,
         )
 
@@ -107,48 +108,56 @@
 
     def get(self) -> float:
         """Get method."""
         return self.mean
 
 
 class CircularMean(Mean):
-    """Circular mean class."""
+    """Circular mean class.
 
-    def __init__(self, size: int) -> None:
-        """Init method."""
+    :param size: size of the circular mean
+    :type size: int
+    """
+
+    def __init__(  # noqa: D107
+        self,
+        size: int,
+    ) -> None:
         super().__init__()
         self.queue = CircularQueue(max_len=size)
 
     def update(self, value: Union[int, float]) -> None:
         """Update the mean value sequentially.
 
         :param value: value to use to update the mean
         :type value: int
         :raises TypeError: Type error exception
         """
-        if not isinstance(value, (int, float)):
-            raise TypeError("value must be of type int or float.")
+        if not isinstance(value, (int, float, np.number)):
+            raise TypeError("value must be of type int, float or numpy number.")
         element = self.queue.enqueue(value=value)
         self.num_values = len(self.queue)
         self.mean += self.incremental_op(
             value=value,
             element=self.mean if element is None else element,
             size=self.num_values,
         )
 
 
 class EWMA(IncrementalStat):
-    """EWMA (Exponential Weighted Moving Average) class."""
+    """EWMA (Exponential Weighted Moving Average) class.
 
-    def __init__(self, alpha: float) -> None:
-        """Init method.
+    :param alpha: alpha value
+    :type alpha: float
+    """
 
-        :param alpha:
-        :type alpha: float
-        """
+    def __init__(  # noqa: D107
+        self,
+        alpha: float,
+    ) -> None:
         self.alpha = alpha
         self.one_minus_alpha = 1.0 - self.alpha
         self.mean = 0
 
     @property
     def alpha(self) -> float:
         """Alpha property.
@@ -191,16 +200,16 @@
     def update(self, value: Union[int, float]) -> None:
         """Update the mean value sequentially.
 
         :param value: value to use to update the mean
         :type value: int
         :raises TypeError: Type error exception
         """
-        if not isinstance(value, (int, float)):
-            raise TypeError("value must be of type int or float.")
+        if not isinstance(value, (int, float, np.number)):
+            raise TypeError("value must be of type int, float or numpy number.")
         self.mean = self.alpha * value + self.one_minus_alpha * self.mean
 
     def get(self) -> float:
         """Get method."""
         return self.mean
 
 
@@ -224,17 +233,17 @@
     :type statistic: Callable
     :param statistical_args: args to pass to statistic method
     :type statistical_args: Dict[str, Any]
     :param num_permutations: number of permutations to use
     :type num_permutations: int
     :param num_jobs: number of jobs to use
     :type num_jobs: int
-    :param random_state: random state value
+    :param random_state: random state value, defaults to None
     :type random_state: Optional[int]
-    :param verbose: verbose flag
+    :param verbose: verbose flag, defaults to False
     :type verbose: bool
     :return: permuted statistics
     :rtype: List[float]
     """
     np.random.seed(seed=random_state)
     X_num_samples, Y_num_samples = X.shape[0], Y.shape[0]  # noqa: N806
     data = np.concatenate([X, Y])
```

### Comparing `frouros-0.5.1/frouros.egg-info/PKG-INFO` & `frouros-0.6.0/frouros.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6672 6f75  : 2.1.Name: frou
-00000020: 726f 730a 5665 7273 696f 6e3a 2030 2e35  ros.Version: 0.5
-00000030: 2e31 0a53 756d 6d61 7279 3a20 416e 206f  .1.Summary: An o
+00000020: 726f 730a 5665 7273 696f 6e3a 2030 2e36  ros.Version: 0.6
+00000030: 2e30 0a53 756d 6d61 7279 3a20 416e 206f  .0.Summary: An o
 00000040: 7065 6e2d 736f 7572 6365 2050 7974 686f  pen-source Pytho
 00000050: 6e20 6c69 6272 6172 7920 666f 7220 6472  n library for dr
 00000060: 6966 7420 6465 7465 6374 696f 6e20 696e  ift detection in
 00000070: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
 00000080: 6720 7379 7374 656d 730a 486f 6d65 2d70  g systems.Home-p
 00000090: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 000000a0: 6875 622e 636f 6d2f 4946 4341 2f66 726f  hub.com/IFCA/fro
@@ -229,1252 +229,1345 @@
 00000e40: 2020 2020 2020 2020 3c2f 693e 0a20 2020          </i>.   
 00000e50: 203c 2f70 3e0a 3c2f 6469 763e 0a0a 2d2d   </p>.</div>..--
 00000e60: 2d2d 0a0a 2323 20e2 9aa1 efb8 8f20 5175  --..## ...... Qu
 00000e70: 6963 6b73 7461 7274 0a0a 2323 2320 436f  ickstart..### Co
 00000e80: 6e63 6570 7420 6472 6966 740a 0a41 7320  ncept drift..As 
 00000e90: 6120 7175 6963 6b20 6578 616d 706c 652c  a quick example,
 00000ea0: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
-00000eb0: 7769 6e65 2064 6174 6173 6574 2074 6f20  wine dataset to 
-00000ec0: 7768 6963 6820 636f 6e63 6570 7420 6472  which concept dr
-00000ed0: 6966 7420 6974 2069 7320 696e 6475 6365  ift it is induce
-00000ee0: 6420 696e 206f 7264 6572 2074 6f20 7368  d in order to sh
-00000ef0: 6f77 2074 6865 2075 7365 206f 6620 6120  ow the use of a 
-00000f00: 636f 6e63 6570 7420 6472 6966 7420 6465  concept drift de
-00000f10: 7465 6374 6f72 206c 696b 6520 4444 4d20  tector like DDM 
-00000f20: 2844 7269 6674 2044 6574 6563 7469 6f6e  (Drift Detection
-00000f30: 204d 6574 686f 6429 2e0a 0a60 6060 7079   Method)...```py
-00000f40: 7468 6f6e 0a69 6d70 6f72 7420 6e75 6d70  thon.import nump
-00000f50: 7920 6173 206e 700a 6672 6f6d 2073 6b6c  y as np.from skl
-00000f60: 6561 726e 2e64 6174 6173 6574 7320 696d  earn.datasets im
-00000f70: 706f 7274 206c 6f61 645f 7769 6e65 0a66  port load_wine.f
-00000f80: 726f 6d20 736b 6c65 6172 6e2e 6c69 6e65  rom sklearn.line
-00000f90: 6172 5f6d 6f64 656c 2069 6d70 6f72 7420  ar_model import 
-00000fa0: 4c6f 6769 7374 6963 5265 6772 6573 7369  LogisticRegressi
-00000fb0: 6f6e 0a66 726f 6d20 736b 6c65 6172 6e2e  on.from sklearn.
-00000fc0: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e20  model_selection 
-00000fd0: 696d 706f 7274 2074 7261 696e 5f74 6573  import train_tes
-00000fe0: 745f 7370 6c69 740a 6672 6f6d 2073 6b6c  t_split.from skl
-00000ff0: 6561 726e 2e70 6970 656c 696e 6520 696d  earn.pipeline im
-00001000: 706f 7274 2050 6970 656c 696e 650a 6672  port Pipeline.fr
-00001010: 6f6d 2073 6b6c 6561 726e 2e70 7265 7072  om sklearn.prepr
-00001020: 6f63 6573 7369 6e67 2069 6d70 6f72 7420  ocessing import 
-00001030: 5374 616e 6461 7264 5363 616c 6572 0a0a  StandardScaler..
-00001040: 6672 6f6d 2066 726f 7572 6f73 2e64 6574  from frouros.det
-00001050: 6563 746f 7273 2e63 6f6e 6365 7074 5f64  ectors.concept_d
-00001060: 7269 6674 2069 6d70 6f72 7420 4444 4d2c  rift import DDM,
-00001070: 2044 444d 436f 6e66 6967 0a0a 6e70 2e72   DDMConfig..np.r
-00001080: 616e 646f 6d2e 7365 6564 2873 6565 643d  andom.seed(seed=
-00001090: 3331 290a 0a23 204c 6f61 6420 7769 6e65  31)..# Load wine
-000010a0: 2064 6174 6173 6574 0a58 2c20 7920 3d20   dataset.X, y = 
-000010b0: 6c6f 6164 5f77 696e 6528 7265 7475 726e  load_wine(return
-000010c0: 5f58 5f79 3d54 7275 6529 0a0a 2320 5370  _X_y=True)..# Sp
-000010d0: 6c69 7420 7472 6169 6e20 2837 3025 2920  lit train (70%) 
-000010e0: 616e 6420 7465 7374 2028 3330 2529 0a28  and test (30%).(
-000010f0: 0a20 2020 2058 5f74 7261 696e 2c0a 2020  .    X_train,.  
-00001100: 2020 585f 7465 7374 2c0a 2020 2020 795f    X_test,.    y_
-00001110: 7472 6169 6e2c 0a20 2020 2079 5f74 6573  train,.    y_tes
-00001120: 742c 0a29 203d 2074 7261 696e 5f74 6573  t,.) = train_tes
-00001130: 745f 7370 6c69 7428 582c 2079 2c20 7472  t_split(X, y, tr
-00001140: 6169 6e5f 7369 7a65 3d30 2e37 2c20 7261  ain_size=0.7, ra
-00001150: 6e64 6f6d 5f73 7461 7465 3d33 3129 0a0a  ndom_state=31)..
-00001160: 2320 494d 504f 5254 414e 543a 2049 6e64  # IMPORTANT: Ind
-00001170: 7563 652f 7369 6d75 6c61 7465 2063 6f6e  uce/simulate con
-00001180: 6365 7074 2064 7269 6674 2069 6e20 7468  cept drift in th
-00001190: 6520 6c61 7374 2070 6172 7420 2832 3025  e last part (20%
-000011a0: 290a 2320 6f66 2079 5f74 6573 7420 6279  ).# of y_test by
-000011b0: 206d 6f64 6966 7969 6e67 2073 6f6d 6520   modifying some 
-000011c0: 6c61 6265 6c73 2028 3530 2520 6170 7072  labels (50% appr
-000011d0: 6f78 292e 2054 6865 7265 666f 7265 2c20  ox). Therefore, 
-000011e0: 6368 616e 6769 6e67 2050 2879 7c58 2929  changing P(y|X))
-000011f0: 0a64 7269 6674 5f73 697a 6520 3d20 696e  .drift_size = in
-00001200: 7428 795f 7465 7374 2e73 6861 7065 5b30  t(y_test.shape[0
-00001210: 5d20 2a20 302e 3229 0a79 5f74 6573 745f  ] * 0.2).y_test_
-00001220: 6472 6966 7420 3d20 795f 7465 7374 5b2d  drift = y_test[-
-00001230: 6472 6966 745f 7369 7a65 3a5d 0a6d 6f64  drift_size:].mod
-00001240: 6966 795f 6964 7820 3d20 6e70 2e72 616e  ify_idx = np.ran
-00001250: 646f 6d2e 7261 6e64 282a 795f 7465 7374  dom.rand(*y_test
-00001260: 5f64 7269 6674 2e73 6861 7065 2920 3c3d  _drift.shape) <=
-00001270: 2030 2e35 0a79 5f74 6573 745f 6472 6966   0.5.y_test_drif
-00001280: 745b 6d6f 6469 6679 5f69 6478 5d20 3d20  t[modify_idx] = 
-00001290: 2879 5f74 6573 745f 6472 6966 745b 6d6f  (y_test_drift[mo
-000012a0: 6469 6679 5f69 6478 5d20 2b20 3129 2025  dify_idx] + 1) %
-000012b0: 206c 656e 286e 702e 756e 6971 7565 2879   len(np.unique(y
-000012c0: 5f74 6573 7429 290a 795f 7465 7374 5b2d  _test)).y_test[-
-000012d0: 6472 6966 745f 7369 7a65 3a5d 203d 2079  drift_size:] = y
-000012e0: 5f74 6573 745f 6472 6966 740a 0a23 2044  _test_drift..# D
-000012f0: 6566 696e 6520 616e 6420 6669 7420 6d6f  efine and fit mo
-00001300: 6465 6c0a 7069 7065 6c69 6e65 203d 2050  del.pipeline = P
-00001310: 6970 656c 696e 6528 0a20 2020 205b 0a20  ipeline(.    [. 
-00001320: 2020 2020 2020 2028 2273 6361 6c65 7222         ("scaler"
-00001330: 2c20 5374 616e 6461 7264 5363 616c 6572  , StandardScaler
-00001340: 2829 292c 0a20 2020 2020 2020 2028 226d  ()),.        ("m
-00001350: 6f64 656c 222c 204c 6f67 6973 7469 6352  odel", LogisticR
-00001360: 6567 7265 7373 696f 6e28 2929 2c0a 2020  egression()),.  
-00001370: 2020 5d0a 290a 7069 7065 6c69 6e65 2e66    ].).pipeline.f
-00001380: 6974 2858 3d58 5f74 7261 696e 2c20 793d  it(X=X_train, y=
-00001390: 795f 7472 6169 6e29 0a0a 2320 4465 7465  y_train)..# Dete
-000013a0: 6374 6f72 2063 6f6e 6669 6775 7261 7469  ctor configurati
-000013b0: 6f6e 2061 6e64 2069 6e73 7461 6e74 6961  on and instantia
-000013c0: 7469 6f6e 0a63 6f6e 6669 6720 3d20 4444  tion.config = DD
-000013d0: 4d43 6f6e 6669 6728 7761 726e 696e 675f  MConfig(warning_
-000013e0: 6c65 7665 6c3d 322e 302c 0a20 2020 2020  level=2.0,.     
-000013f0: 2020 2020 2020 2020 2020 2020 2020 6472                dr
-00001400: 6966 745f 6c65 7665 6c3d 332e 302c 0a20  ift_level=3.0,. 
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 2020 6d69 6e5f 6e75 6d5f 696e 7374 616e    min_num_instan
-00001430: 6365 733d 3330 2c29 0a64 6574 6563 746f  ces=30,).detecto
-00001440: 7220 3d20 4444 4d28 636f 6e66 6967 3d63  r = DDM(config=c
-00001450: 6f6e 6669 6729 0a0a 2320 5369 6d75 6c61  onfig)..# Simula
-00001460: 7465 2064 6174 6120 7374 7265 616d 2028  te data stream (
-00001470: 6173 7375 6d69 6e67 2074 6573 7420 6c61  assuming test la
-00001480: 6265 6c20 6176 6169 6c61 626c 6520 6166  bel available af
-00001490: 7465 7220 7072 6564 6963 7469 6f6e 290a  ter prediction).
-000014a0: 666f 7220 692c 2028 582c 2079 2920 696e  for i, (X, y) in
-000014b0: 2065 6e75 6d65 7261 7465 287a 6970 2858   enumerate(zip(X
-000014c0: 5f74 6573 742c 2079 5f74 6573 7429 293a  _test, y_test)):
-000014d0: 0a20 2020 2079 5f70 7265 6420 3d20 7069  .    y_pred = pi
-000014e0: 7065 6c69 6e65 2e70 7265 6469 6374 2858  peline.predict(X
-000014f0: 2e72 6573 6861 7065 2831 2c20 2d31 2929  .reshape(1, -1))
-00001500: 0a20 2020 2065 7272 6f72 203d 2031 202d  .    error = 1 -
-00001510: 2069 6e74 2879 5f70 7265 6420 3d3d 2079   int(y_pred == y
-00001520: 290a 2020 2020 6465 7465 6374 6f72 2e75  ).    detector.u
-00001530: 7064 6174 6528 7661 6c75 653d 6572 726f  pdate(value=erro
-00001540: 7229 0a20 2020 2073 7461 7475 7320 3d20  r).    status = 
-00001550: 6465 7465 6374 6f72 2e73 7461 7475 730a  detector.status.
-00001560: 2020 2020 6966 2073 7461 7475 735b 2264      if status["d
-00001570: 7269 6674 225d 3a0a 2020 2020 2020 2020  rift"]:.        
-00001580: 7072 696e 7428 6622 4472 6966 7420 6465  print(f"Drift de
-00001590: 7465 6374 6564 2061 7420 696e 6465 7820  tected at index 
-000015a0: 7b69 7d22 290a 2020 2020 2020 2020 6272  {i}").        br
-000015b0: 6561 6b0a 0a3e 3e20 4472 6966 7420 6465  eak..>> Drift de
-000015c0: 7465 6374 6564 2061 7420 696e 6465 7820  tected at index 
-000015d0: 3434 0a60 6060 0a0a 4d6f 7265 2063 6f6e  44.```..More con
-000015e0: 6365 7074 2064 7269 6674 2065 7861 6d70  cept drift examp
-000015f0: 6c65 7320 6361 6e20 6265 2066 6f75 6e64  les can be found
-00001600: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-00001610: 6672 6f75 726f 732e 7265 6164 7468 6564  frouros.readthed
-00001620: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00001630: 2f65 7861 6d70 6c65 732e 6874 6d6c 2364  /examples.html#d
-00001640: 6174 612d 6472 6966 7429 2e0a 0a23 2323  ata-drift)...###
-00001650: 2044 6174 6120 6472 6966 740a 0a41 7320   Data drift..As 
-00001660: 6120 7175 6963 6b20 6578 616d 706c 652c  a quick example,
-00001670: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
-00001680: 6972 6973 2064 6174 6173 6574 2074 6f20  iris dataset to 
-00001690: 7768 6963 6820 6461 7461 2064 7269 6674  which data drift
-000016a0: 2069 6e20 6f72 6465 7220 746f 2073 686f   in order to sho
-000016b0: 7720 7468 6520 7573 6520 6f66 2061 2064  w the use of a d
-000016c0: 6174 6120 6472 6966 7420 6465 7465 6374  ata drift detect
-000016d0: 6f72 206c 696b 6520 4b6f 6c6d 6f67 6f72  or like Kolmogor
-000016e0: 6f76 2d53 6d69 726e 6f76 2074 6573 742e  ov-Smirnov test.
-000016f0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-00001700: 7274 206e 756d 7079 2061 7320 6e70 0a66  rt numpy as np.f
-00001710: 726f 6d20 736b 6c65 6172 6e2e 6461 7461  rom sklearn.data
-00001720: 7365 7473 2069 6d70 6f72 7420 6c6f 6164  sets import load
-00001730: 5f69 7269 730a 6672 6f6d 2073 6b6c 6561  _iris.from sklea
-00001740: 726e 2e6d 6f64 656c 5f73 656c 6563 7469  rn.model_selecti
-00001750: 6f6e 2069 6d70 6f72 7420 7472 6169 6e5f  on import train_
-00001760: 7465 7374 5f73 706c 6974 0a66 726f 6d20  test_split.from 
-00001770: 736b 6c65 6172 6e2e 7472 6565 2069 6d70  sklearn.tree imp
-00001780: 6f72 7420 4465 6369 7369 6f6e 5472 6565  ort DecisionTree
-00001790: 436c 6173 7369 6669 6572 0a0a 6672 6f6d  Classifier..from
-000017a0: 2066 726f 7572 6f73 2e64 6574 6563 746f   frouros.detecto
-000017b0: 7273 2e64 6174 615f 6472 6966 7420 696d  rs.data_drift im
-000017c0: 706f 7274 204b 5354 6573 740a 0a6e 702e  port KSTest..np.
-000017d0: 7261 6e64 6f6d 2e73 6565 6428 7365 6564  random.seed(seed
-000017e0: 3d33 3129 0a0a 2320 4c6f 6164 2069 7269  =31)..# Load iri
-000017f0: 7320 6461 7461 7365 740a 582c 2079 203d  s dataset.X, y =
-00001800: 206c 6f61 645f 6972 6973 2872 6574 7572   load_iris(retur
-00001810: 6e5f 585f 793d 5472 7565 290a 0a23 2053  n_X_y=True)..# S
-00001820: 706c 6974 2074 7261 696e 2028 3730 2529  plit train (70%)
-00001830: 2061 6e64 2074 6573 7420 2833 3025 290a   and test (30%).
-00001840: 280a 2020 2020 585f 7472 6169 6e2c 0a20  (.    X_train,. 
-00001850: 2020 2058 5f74 6573 742c 0a20 2020 2079     X_test,.    y
-00001860: 5f74 7261 696e 2c0a 2020 2020 795f 7465  _train,.    y_te
-00001870: 7374 2c0a 2920 3d20 7472 6169 6e5f 7465  st,.) = train_te
-00001880: 7374 5f73 706c 6974 2858 2c20 792c 2074  st_split(X, y, t
-00001890: 7261 696e 5f73 697a 653d 302e 372c 2072  rain_size=0.7, r
-000018a0: 616e 646f 6d5f 7374 6174 653d 3331 290a  andom_state=31).
-000018b0: 0a23 2053 6574 2074 6865 2066 6561 7475  .# Set the featu
-000018c0: 7265 2069 6e64 6578 2074 6f20 7768 6963  re index to whic
-000018d0: 6820 6465 7465 6374 6f72 2069 7320 6170  h detector is ap
-000018e0: 706c 6965 640a 6469 6d5f 6964 7820 3d20  plied.dim_idx = 
-000018f0: 300a 0a23 2049 4d50 4f52 5441 4e54 3a20  0..# IMPORTANT: 
-00001900: 496e 6475 6365 2f73 696d 756c 6174 6520  Induce/simulate 
-00001910: 6461 7461 2064 7269 6674 2069 6e20 7468  data drift in th
-00001920: 6520 7365 6c65 6374 6564 2066 6561 7475  e selected featu
-00001930: 7265 206f 6620 795f 7465 7374 2062 790a  re of y_test by.
-00001940: 2320 6170 706c 7969 6e67 2073 6f6d 6520  # applying some 
-00001950: 6761 7573 7369 616e 206e 6f69 7365 2e20  gaussian noise. 
-00001960: 5468 6572 6566 6f72 652c 2063 6861 6e67  Therefore, chang
-00001970: 696e 6720 5028 5829 290a 585f 7465 7374  ing P(X)).X_test
-00001980: 5b3a 2c20 6469 6d5f 6964 785d 202b 3d20  [:, dim_idx] += 
-00001990: 6e70 2e72 616e 646f 6d2e 6e6f 726d 616c  np.random.normal
-000019a0: 280a 2020 2020 6c6f 633d 302e 302c 0a20  (.    loc=0.0,. 
-000019b0: 2020 2073 6361 6c65 3d33 2e30 2c0a 2020     scale=3.0,.  
-000019c0: 2020 7369 7a65 3d58 5f74 6573 742e 7368    size=X_test.sh
-000019d0: 6170 655b 305d 2c0a 290a 0a23 2044 6566  ape[0],.)..# Def
-000019e0: 696e 6520 616e 6420 6669 7420 6d6f 6465  ine and fit mode
-000019f0: 6c0a 6d6f 6465 6c20 3d20 4465 6369 7369  l.model = Decisi
-00001a00: 6f6e 5472 6565 436c 6173 7369 6669 6572  onTreeClassifier
-00001a10: 2872 616e 646f 6d5f 7374 6174 653d 3331  (random_state=31
-00001a20: 290a 6d6f 6465 6c2e 6669 7428 583d 585f  ).model.fit(X=X_
-00001a30: 7472 6169 6e2c 2079 3d79 5f74 7261 696e  train, y=y_train
-00001a40: 290a 0a23 2053 6574 2073 6967 6e69 6669  )..# Set signifi
-00001a50: 6361 6e63 6520 6c65 7665 6c20 666f 7220  cance level for 
-00001a60: 6879 706f 7468 6573 6973 2074 6573 7469  hypothesis testi
-00001a70: 6e67 0a61 6c70 6861 203d 2030 2e30 3031  ng.alpha = 0.001
-00001a80: 0a23 2044 6566 696e 6520 616e 6420 6669  .# Define and fi
-00001a90: 7420 6465 7465 6374 6f72 0a64 6574 6563  t detector.detec
-00001aa0: 746f 7220 3d20 4b53 5465 7374 2829 0a64  tor = KSTest().d
-00001ab0: 6574 6563 746f 722e 6669 7428 583d 585f  etector.fit(X=X_
-00001ac0: 7472 6169 6e5b 3a2c 2064 696d 5f69 6478  train[:, dim_idx
-00001ad0: 5d29 0a0a 2320 4170 706c 7920 6465 7465  ])..# Apply dete
-00001ae0: 6374 6f72 2074 6f20 7468 6520 7365 6c65  ctor to the sele
-00001af0: 6374 6564 2066 6561 7475 7265 206f 6620  cted feature of 
-00001b00: 585f 7465 7374 0a72 6573 756c 7420 3d20  X_test.result = 
-00001b10: 6465 7465 6374 6f72 2e63 6f6d 7061 7265  detector.compare
-00001b20: 2858 3d58 5f74 6573 745b 3a2c 2064 696d  (X=X_test[:, dim
-00001b30: 5f69 6478 5d29 0a0a 2320 4368 6563 6b20  _idx])..# Check 
-00001b40: 6966 2064 7269 6674 2069 7320 7461 6b69  if drift is taki
-00001b50: 6e67 2070 6c61 6365 0a72 6573 756c 745b  ng place.result[
-00001b60: 305d 2e70 5f76 616c 7565 203c 2061 6c70  0].p_value < alp
-00001b70: 6861 0a3e 3e20 5472 7565 2023 2044 6174  ha.>> True # Dat
-00001b80: 6120 6472 6966 7420 6465 7465 6374 6564  a drift detected
-00001b90: 2e0a 2320 5468 6572 6566 6f72 652c 2077  ..# Therefore, w
-00001ba0: 6520 6361 6e20 7265 6a65 6374 2048 3020  e can reject H0 
-00001bb0: 2862 6f74 6820 7361 6d70 6c65 7320 636f  (both samples co
-00001bc0: 6d65 2066 726f 6d20 7468 6520 7361 6d65  me from the same
-00001bd0: 2064 6973 7472 6962 7574 696f 6e29 2e0a   distribution)..
-00001be0: 6060 600a 0a4d 6f72 6520 6461 7461 2064  ```..More data d
-00001bf0: 7269 6674 2065 7861 6d70 6c65 7320 6361  rift examples ca
-00001c00: 6e20 6265 2066 6f75 6e64 205b 6865 7265  n be found [here
-00001c10: 5d28 6874 7470 733a 2f2f 6672 6f75 726f  ](https://frouro
-00001c20: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
-00001c30: 2f65 6e2f 6c61 7465 7374 2f65 7861 6d70  /en/latest/examp
-00001c40: 6c65 732e 6874 6d6c 2364 6174 612d 6472  les.html#data-dr
-00001c50: 6966 7429 2e0a 0a23 2320 f09f 9ba0 2049  ift)...## .... I
-00001c60: 6e73 7461 6c6c 6174 696f 6e0a 0a46 726f  nstallation..Fro
-00001c70: 7572 6f73 2063 616e 2062 6520 696e 7374  uros can be inst
-00001c80: 616c 6c65 6420 7669 6120 7069 703a 0a0a  alled via pip:..
-00001c90: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
-00001ca0: 616c 6c20 6672 6f75 726f 730a 6060 600a  all frouros.```.
-00001cb0: 0a23 2320 f09f 95b5 f09f 8fbb e280 8de2  .## ............
-00001cc0: 9982 efb8 8fef b88f 2044 7269 6674 2064  ........ Drift d
-00001cd0: 6574 6563 7469 6f6e 206d 6574 686f 6473  etection methods
-00001ce0: 0a0a 5468 6520 6375 7272 656e 746c 7920  ..The currently 
-00001cf0: 696d 706c 656d 656e 7465 6420 6465 7465  implemented dete
-00001d00: 6374 6f72 7320 6172 6520 6c69 7374 6564  ctors are listed
-00001d10: 2069 6e20 7468 6520 666f 6c6c 6f77 696e   in the followin
-00001d20: 6720 7461 626c 652e 0a0a 3c74 6162 6c65  g table...<table
-00001d30: 2073 7479 6c65 3d22 7769 6474 683a 2031   style="width: 1
-00001d40: 3030 253b 2074 6578 742d 616c 6967 6e3a  00%; text-align:
-00001d50: 2063 656e 7465 723b 2062 6f72 6465 722d   center; border-
-00001d60: 636f 6c6c 6170 7365 3a20 636f 6c6c 6170  collapse: collap
-00001d70: 7365 3b20 626f 7264 6572 3a20 3170 7820  se; border: 1px 
-00001d80: 736f 6c69 6420 6772 6579 3b22 3e0a 2020  solid grey;">.  
-00001d90: 3c74 6865 6164 3e0a 2020 2020 3c74 723e  <thead>.    <tr>
-00001da0: 0a20 2020 203c 7468 2073 7479 6c65 3d22  .    <th style="
-00001db0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00001dc0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00001dd0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00001de0: 696e 673a 2034 7078 3b22 3e44 7269 6674  ing: 4px;">Drift
-00001df0: 2064 6574 6563 746f 723c 2f74 683e 0a20   detector</th>. 
-00001e00: 2020 203c 7468 2073 7479 6c65 3d22 7465     <th style="te
-00001e10: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00001e20: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00001e30: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00001e40: 673a 2034 7078 3b22 3e54 7970 653c 2f74  g: 4px;">Type</t
-00001e50: 683e 0a20 2020 203c 7468 2073 7479 6c65  h>.    <th style
-00001e60: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00001e70: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00001e80: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00001e90: 6464 696e 673a 2034 7078 3b22 3e46 616d  dding: 4px;">Fam
-00001ea0: 696c 793c 2f74 683e 0a20 2020 203c 7468  ily</th>.    <th
-00001eb0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00001ec0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00001ed0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00001ee0: 6579 3b20 7061 6464 696e 673a 2034 7078  ey; padding: 4px
-00001ef0: 3b22 3e55 6e69 7661 7269 6174 6520 2855  ;">Univariate (U
-00001f00: 2920 2f20 4d75 6c74 6976 6172 6961 7465  ) / Multivariate
-00001f10: 2028 4d29 3c2f 7468 3e0a 2020 2020 3c74   (M)</th>.    <t
-00001f20: 6820 7374 796c 653d 2274 6578 742d 616c  h style="text-al
-00001f30: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00001f40: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00001f50: 7265 793b 2070 6164 6469 6e67 3a20 3470  rey; padding: 4p
-00001f60: 783b 223e 4e75 6d65 7269 6361 6c20 284e  x;">Numerical (N
-00001f70: 2920 2f20 4361 7465 676f 7269 6361 6c20  ) / Categorical 
-00001f80: 2843 293c 2f74 683e 0a20 2020 203c 7468  (C)</th>.    <th
-00001f90: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00001fa0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00001fb0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00001fc0: 6579 3b20 7061 6464 696e 673a 2034 7078  ey; padding: 4px
-00001fd0: 3b22 3e4d 6574 686f 643c 2f74 683e 0a20  ;">Method</th>. 
-00001fe0: 2020 203c 7468 2073 7479 6c65 3d22 7465     <th style="te
-00001ff0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002000: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002010: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002020: 673a 2034 7078 3b22 3e52 6566 6572 656e  g: 4px;">Referen
-00002030: 6365 3c2f 7468 3e0a 2020 2020 3c2f 7472  ce</th>.    </tr
-00002040: 3e0a 2020 3c2f 7468 6561 643e 0a20 203c  >.  </thead>.  <
-00002050: 7462 6f64 793e 0a20 203c 7472 3e0a 2020  tbody>.  <tr>.  
-00002060: 2020 3c74 6420 726f 7773 7061 6e3d 2231    <td rowspan="1
-00002070: 3322 2073 7479 6c65 3d22 7465 7874 2d61  3" style="text-a
-00002080: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002090: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-000020a0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-000020b0: 7078 3b22 3e43 6f6e 6365 7074 2064 7269  px;">Concept dri
-000020c0: 6674 3c2f 7464 3e0a 2020 2020 3c74 6420  ft</td>.    <td 
-000020d0: 726f 7773 7061 6e3d 2231 3322 2073 7479  rowspan="13" sty
-000020e0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-000020f0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00002100: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00002110: 7061 6464 696e 673a 2038 7078 3b22 3e53  padding: 8px;">S
-00002120: 7472 6561 6d69 6e67 3c2f 7464 3e0a 2020  treaming</td>.  
-00002130: 2020 3c74 6420 726f 7773 7061 6e3d 2234    <td rowspan="4
-00002140: 2220 7374 796c 653d 2274 6578 742d 616c  " style="text-al
-00002150: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00002160: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00002170: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00002180: 783b 223e 4368 616e 6765 2064 6574 6563  x;">Change detec
-00002190: 7469 6f6e 3c2f 7464 3e0a 2020 2020 3c74  tion</td>.    <t
-000021a0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000021b0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-000021c0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-000021d0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-000021e0: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
-000021f0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00002200: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002210: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00002220: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00002230: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
-00002240: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00002250: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00002260: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002270: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002280: 3870 783b 223e 424f 4344 3c2f 7464 3e0a  8px;">BOCD</td>.
-00002290: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-000022a0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-000022b0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-000022c0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-000022d0: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
-000022e0: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
-000022f0: 7267 2f31 302e 3438 3535 302f 6172 5869  rg/10.48550/arXi
-00002300: 762e 3037 3130 2e33 3734 3222 3e41 6461  v.0710.3742">Ada
-00002310: 6d73 2061 6e64 204d 6163 4b61 7920 2832  ms and MacKay (2
-00002320: 3030 3729 3c2f 613e 3c2f 7464 3e0a 2020  007)</a></td>.  
-00002330: 3c2f 7472 3e0a 2020 3c74 723e 0a20 2020  </tr>.  <tr>.   
-00002340: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002350: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00002360: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00002370: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00002380: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
-00002390: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-000023a0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-000023b0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000023c0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000023d0: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
-000023e0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000023f0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002400: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002410: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002420: 673a 2038 7078 3b22 3e43 5553 554d 3c2f  g: 8px;">CUSUM</
-00002430: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00002440: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00002450: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00002460: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00002470: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
-00002480: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-00002490: 6f69 2e6f 7267 2f31 302e 3233 3037 2f32  oi.org/10.2307/2
-000024a0: 3333 3330 3039 223e 5061 6765 2028 3139  333009">Page (19
-000024b0: 3534 293c 2f61 3e3c 2f74 643e 0a20 203c  54)</a></td>.  <
-000024c0: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
-000024d0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000024e0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000024f0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002500: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002510: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
-00002520: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002530: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00002540: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00002550: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00002560: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
-00002570: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00002580: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00002590: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000025a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000025b0: 3a20 3870 783b 223e 4765 6f6d 6574 7269  : 8px;">Geometri
-000025c0: 6320 6d6f 7669 6e67 2061 7665 7261 6765  c moving average
-000025d0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-000025e0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000025f0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00002600: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00002610: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00002620: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00002630: 2f64 6f69 2e6f 7267 2f31 302e 3233 3037  /doi.org/10.2307
-00002640: 2f31 3236 3634 3433 223e 526f 6265 7274  /1266443">Robert
-00002650: 7320 2831 3935 3929 3c2f 613e 3c2f 7464  s (1959)</a></td
-00002660: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
-00002670: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00002680: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00002690: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-000026a0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-000026b0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
-000026c0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000026d0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000026e0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000026f0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002700: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
-00002710: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002720: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002730: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002740: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002750: 6464 696e 673a 2038 7078 3b22 3e50 6167  dding: 8px;">Pag
-00002760: 6520 4869 6e6b 6c65 793c 2f74 643e 0a20  e Hinkley</td>. 
-00002770: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00002780: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002790: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000027a0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000027b0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-000027c0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-000027d0: 672f 3130 2e32 3330 372f 3233 3333 3030  g/10.2307/233300
-000027e0: 3922 3e50 6167 6520 2831 3935 3429 3c2f  9">Page (1954)</
-000027f0: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
-00002800: 2020 3c74 723e 0a20 2020 203c 7464 2072    <tr>.    <td r
-00002810: 6f77 7370 616e 3d22 3622 2073 7479 6c65  owspan="6" style
-00002820: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002830: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002840: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002850: 6464 696e 673a 2038 7078 3b22 3e53 7461  dding: 8px;">Sta
-00002860: 7469 7374 6963 616c 2070 726f 6365 7373  tistical process
-00002870: 2063 6f6e 7472 6f6c 3c2f 7464 3e0a 2020   control</td>.  
-00002880: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00002890: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-000028a0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-000028b0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-000028c0: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
-000028d0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000028e0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000028f0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002900: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002910: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
-00002920: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00002930: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00002940: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00002950: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002960: 6e67 3a20 3870 783b 223e 4444 4d3c 2f74  ng: 8px;">DDM</t
-00002970: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002980: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002990: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-000029a0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-000029b0: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
-000029c0: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-000029d0: 692e 6f72 672f 3130 2e31 3030 372f 3937  i.org/10.1007/97
-000029e0: 382d 332d 3534 302d 3238 3634 352d 355f  8-3-540-28645-5_
-000029f0: 3239 223e 4761 6d61 2065 7420 616c 2e20  29">Gama et al. 
-00002a00: 2832 3030 3429 3c2f 613e 3c2f 7464 3e0a  (2004)</a></td>.
-00002a10: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
-00002a20: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00002a30: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00002a40: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00002a50: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00002a60: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
-00002a70: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00002a80: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00002a90: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00002aa0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00002ab0: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
-00002ac0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00002ad0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00002ae0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00002af0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00002b00: 696e 673a 2038 7078 3b22 3e45 4344 442d  ing: 8px;">ECDD-
-00002b10: 5754 3c2f 7464 3e0a 2020 2020 3c74 6420  WT</td>.    <td 
-00002b20: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00002b30: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00002b40: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00002b50: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00002b60: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
-00002b70: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
-00002b80: 3136 2f6a 2e70 6174 7265 632e 3230 3131  16/j.patrec.2011
-00002b90: 2e30 382e 3031 3922 3e52 6f73 7320 6574  .08.019">Ross et
-00002ba0: 2061 6c2e 2028 3230 3132 293c 2f61 3e3c   al. (2012)</a><
-00002bb0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-00002bc0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-00002bd0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00002be0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00002bf0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00002c00: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00002c10: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00002c20: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00002c30: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00002c40: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00002c50: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00002c60: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00002c70: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00002c80: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00002c90: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00002ca0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00002cb0: 4544 444d 3c2f 7464 3e0a 2020 2020 3c74  EDDM</td>.    <t
-00002cc0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00002cd0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00002ce0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00002cf0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00002d00: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
-00002d10: 7073 3a2f 2f77 7777 2e72 6573 6561 7263  ps://www.researc
-00002d20: 6867 6174 652e 6e65 742f 7075 626c 6963  hgate.net/public
-00002d30: 6174 696f 6e2f 3234 3539 3939 3730 345f  ation/245999704_
-00002d40: 4561 726c 795f 4472 6966 745f 4465 7465  Early_Drift_Dete
-00002d50: 6374 696f 6e5f 4d65 7468 6f64 223e 4261  ction_Method">Ba
-00002d60: 656e 612d 4761 7263 c4b1 6120 6574 2061  ena-Garc..a et a
-00002d70: 6c2e 2028 3230 3036 293c 2f61 3e3c 2f74  l. (2006)</a></t
-00002d80: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-00002d90: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00002da0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00002db0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00002dc0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00002dd0: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
-00002de0: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00002df0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00002e00: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00002e10: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00002e20: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
-00002e30: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00002e40: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00002e50: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00002e60: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00002e70: 6164 6469 6e67 3a20 3870 783b 223e 4844  adding: 8px;">HD
-00002e80: 444d 2d41 3c2f 7464 3e0a 2020 2020 3c74  DM-A</td>.    <t
-00002e90: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00002ea0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00002eb0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00002ec0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00002ed0: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
-00002ee0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00002ef0: 3131 3039 2f54 4b44 452e 3230 3134 2e32  1109/TKDE.2014.2
-00002f00: 3334 3533 3832 223e 4672 6961 732d 426c  345382">Frias-Bl
-00002f10: 616e 636f 2065 7420 616c 2e20 2832 3031  anco et al. (201
-00002f20: 3429 3c2f 613e 3c2f 7464 3e0a 2020 3c2f  4)</a></td>.  </
-00002f30: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
-00002f40: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00002f50: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00002f60: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00002f70: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00002f80: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
-00002f90: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00002fa0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00002fb0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00002fc0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00002fd0: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
-00002fe0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00002ff0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00003000: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00003010: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00003020: 2038 7078 3b22 3e48 4444 4d2d 573c 2f74   8px;">HDDM-W</t
-00003030: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00003040: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00003050: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00003060: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00003070: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
-00003080: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
-00003090: 692e 6f72 672f 3130 2e31 3130 392f 544b  i.org/10.1109/TK
-000030a0: 4445 2e32 3031 342e 3233 3435 3338 3222  DE.2014.2345382"
-000030b0: 3e46 7269 6173 2d42 6c61 6e63 6f20 6574  >Frias-Blanco et
-000030c0: 2061 6c2e 2028 3230 3134 293c 2f61 3e3c   al. (2014)</a><
-000030d0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-000030e0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-000030f0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003100: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00003110: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003120: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00003130: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00003140: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003150: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003160: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003170: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00003180: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003190: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000031a0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-000031b0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000031c0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000031d0: 5244 444d 3c2f 7464 3e0a 2020 2020 3c74  RDDM</td>.    <t
-000031e0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000031f0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00003200: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00003210: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00003220: 783b 223e 3c61 2068 7265 663d 2268 7474  x;"><a href="htt
-00003230: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00003240: 3130 3136 2f6a 2e65 7377 612e 3230 3137  1016/j.eswa.2017
-00003250: 2e30 382e 3032 3322 3e42 6172 726f 7320  .08.023">Barros 
-00003260: 6574 2061 6c2e 2028 3230 3137 293c 2f61  et al. (2017)</a
-00003270: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
-00003280: 203c 7472 3e0a 2020 2020 3c74 6420 726f   <tr>.    <td ro
-00003290: 7773 7061 6e3d 2233 2220 7374 796c 653d  wspan="3" style=
-000032a0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000032b0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000032c0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000032d0: 6469 6e67 3a20 3870 783b 223e 5769 6e64  ding: 8px;">Wind
-000032e0: 6f77 2062 6173 6564 3c2f 7464 3e0a 2020  ow based</td>.  
-000032f0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00003300: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00003310: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00003320: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00003330: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
-00003340: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00003350: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00003360: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00003370: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00003380: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
-00003390: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-000033a0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-000033b0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-000033c0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-000033d0: 6e67 3a20 3870 783b 223e 4144 5749 4e3c  ng: 8px;">ADWIN<
-000033e0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-000033f0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003400: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003410: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003420: 7061 6464 696e 673a 2038 7078 3b22 3e3c  padding: 8px;"><
-00003430: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00003440: 646f 692e 6f72 672f 3130 2e31 3133 372f  doi.org/10.1137/
-00003450: 312e 3937 3831 3631 3139 3732 3737 312e  1.9781611972771.
-00003460: 3432 223e 4269 6665 7420 616e 6420 4761  42">Bifet and Ga
-00003470: 7661 6c64 6120 2832 3030 3729 3c2f 613e  valda (2007)</a>
-00003480: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00003490: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
-000034a0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-000034b0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-000034c0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-000034d0: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
-000034e0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-000034f0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003500: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003510: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003520: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003530: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
-00003540: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003550: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003560: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003570: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003580: 3e4b 5357 494e 3c2f 7464 3e0a 2020 2020  >KSWIN</td>.    
-00003590: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000035a0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000035b0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000035c0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-000035d0: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-000035e0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-000035f0: 302e 3130 3136 2f6a 2e6e 6575 636f 6d2e  0.1016/j.neucom.
-00003600: 3230 3139 2e31 312e 3131 3122 3e52 6161  2019.11.111">Raa
-00003610: 6220 6574 2061 6c2e 2028 3230 3230 293c  b et al. (2020)<
-00003620: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
-00003630: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
-00003640: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00003650: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00003660: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00003670: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00003680: 223e 553c 2f74 643e 0a20 2020 203c 7464  ">U</td>.    <td
-00003690: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000036a0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-000036b0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-000036c0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-000036d0: 3b22 3e4e 3c2f 7464 3e0a 2020 2020 3c74  ;">N</td>.    <t
-000036e0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000036f0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00003700: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00003710: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00003720: 783b 223e 5354 4550 443c 2f74 643e 0a20  x;">STEPD</td>. 
-00003730: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00003740: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00003750: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00003760: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00003770: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-00003780: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-00003790: 672f 3130 2e31 3030 372f 3937 382d 332d  g/10.1007/978-3-
-000037a0: 3534 302d 3735 3438 382d 365f 3237 223e  540-75488-6_27">
-000037b0: 4e69 7368 6964 6120 616e 6420 5961 6d61  Nishida and Yama
-000037c0: 7563 6869 2028 3230 3037 293c 2f61 3e3c  uchi (2007)</a><
-000037d0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-000037e0: 7472 3e0a 2020 2020 3c74 6420 726f 7773  tr>.    <td rows
-000037f0: 7061 6e3d 2231 3622 2073 7479 6c65 3d22  pan="16" style="
-00003800: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00003810: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00003820: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00003830: 696e 673a 2038 7078 3b22 3e44 6174 6120  ing: 8px;">Data 
-00003840: 6472 6966 743c 2f74 643e 0a20 2020 203c  drift</td>.    <
-00003850: 7464 2072 6f77 7370 616e 3d22 3134 2220  td rowspan="14" 
-00003860: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00003870: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00003880: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00003890: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-000038a0: 223e 4261 7463 683c 2f74 643e 0a20 2020  ">Batch</td>.   
-000038b0: 203c 7464 2072 6f77 7370 616e 3d22 3922   <td rowspan="9"
-000038c0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000038d0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-000038e0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-000038f0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00003900: 3b22 3e44 6973 7461 6e63 6520 6261 7365  ;">Distance base
-00003910: 643c 2f74 643e 0a20 2020 203c 7464 2073  d</td>.    <td s
-00003920: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003930: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003940: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003950: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003960: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-00003970: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00003980: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00003990: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-000039a0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-000039b0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-000039c0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000039d0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-000039e0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-000039f0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00003a00: 3b22 3e41 6e64 6572 736f 6e2d 4461 726c  ;">Anderson-Darl
-00003a10: 696e 6720 7465 7374 3c2f 7464 3e0a 2020  ing test</td>.  
-00003a20: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00003a30: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00003a40: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00003a50: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00003a60: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
-00003a70: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
-00003a80: 2f31 302e 3233 3037 2f32 3238 3838 3035  /10.2307/2288805
-00003a90: 223e 5363 686f 6c7a 2061 6e64 2053 7465  ">Scholz and Ste
-00003aa0: 7068 656e 7320 2831 3938 3729 3c2f 613e  phens (1987)</a>
-00003ab0: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00003ac0: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
-00003ad0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003ae0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003af0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003b00: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
-00003b10: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003b20: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003b30: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003b40: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003b50: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003b60: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
-00003b70: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003b80: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003b90: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003ba0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003bb0: 3e42 6861 7474 6163 6861 7279 7961 2064  >Bhattacharyya d
-00003bc0: 6973 7461 6e63 653c 2f74 643e 0a20 2020  istance</td>.   
-00003bd0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00003be0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00003bf0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00003c00: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00003c10: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
-00003c20: 6874 7470 733a 2f2f 7777 772e 6a73 746f  https://www.jsto
-00003c30: 722e 6f72 672f 7374 6162 6c65 2f32 3530  r.org/stable/250
-00003c40: 3437 3838 3222 3e42 6861 7474 6163 6861  47882">Bhattacha
-00003c50: 7279 7961 2028 3139 3436 293c 2f61 3e3c  ryya (1946)</a><
-00003c60: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-00003c70: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-00003c80: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00003c90: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00003ca0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00003cb0: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
-00003cc0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00003cd0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003ce0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003cf0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003d00: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00003d10: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003d20: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003d30: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003d40: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003d50: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003d60: 4561 7274 6820 4d6f 7665 7227 7320 6469  Earth Mover's di
-00003d70: 7374 616e 6365 3c2f 7464 3e0a 2020 2020  stance</td>.    
-00003d80: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00003d90: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00003da0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00003db0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00003dc0: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
-00003dd0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00003de0: 302e 3130 3233 2f41 3a31 3032 3635 3433  0.1023/A:1026543
-00003df0: 3930 3030 3534 223e 5275 626e 6572 2065  900054">Rubner e
-00003e00: 7420 616c 2e20 2832 3030 3029 3c2f 613e  t al. (2000)</a>
-00003e10: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00003e20: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
-00003e30: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00003e40: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00003e50: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00003e60: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
-00003e70: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-00003e80: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003e90: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-00003ea0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-00003eb0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-00003ec0: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
-00003ed0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00003ee0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00003ef0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00003f00: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00003f10: 3e48 656c 6c69 6e67 6572 2064 6973 7461  >Hellinger dista
-00003f20: 6e63 653c 2f74 643e 0a20 2020 203c 7464  nce</td>.    <td
-00003f30: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00003f40: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00003f50: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00003f60: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00003f70: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
-00003f80: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
-00003f90: 3531 352f 4352 4c4c 2e31 3930 392e 3133  515/CRLL.1909.13
-00003fa0: 362e 3231 3022 3e48 656c 6c69 6e67 6572  6.210">Hellinger
-00003fb0: 2028 3139 3039 293c 2f61 3e3c 2f74 643e   (1909)</a></td>
-00003fc0: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
-00003fd0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00003fe0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00003ff0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004000: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004010: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
-00004020: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004030: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004040: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004050: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004060: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
-00004070: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00004080: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00004090: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000040a0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000040b0: 6469 6e67 3a20 3870 783b 223e 4869 7374  ding: 8px;">Hist
-000040c0: 6f67 7261 6d20 696e 7465 7273 6563 7469  ogram intersecti
-000040d0: 6f6e 206e 6f72 6d61 6c69 7a65 6420 636f  on normalized co
-000040e0: 6d70 6c65 6d65 6e74 3c2f 7464 3e0a 2020  mplement</td>.  
-000040f0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00004100: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00004110: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00004120: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00004130: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
-00004140: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
-00004150: 2f31 302e 3130 3037 2f42 4630 3031 3330  /10.1007/BF00130
-00004160: 3438 3722 3e53 7761 696e 2061 6e64 2042  487">Swain and B
-00004170: 616c 6c61 7264 2028 3139 3931 293c 2f61  allard (1991)</a
-00004180: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
-00004190: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
-000041a0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000041b0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-000041c0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000041d0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000041e0: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
-000041f0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004200: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004210: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004220: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004230: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
-00004240: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00004250: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00004260: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00004270: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00004280: 223e 4a65 6e73 656e 2d53 6861 6e6e 6f6e  ">Jensen-Shannon
-00004290: 2064 6973 7461 6e63 653c 2f74 643e 0a20   distance</td>. 
-000042a0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000042b0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000042c0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000042d0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000042e0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-000042f0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-00004300: 672f 3130 2e31 3130 392f 3138 2e36 3131  g/10.1109/18.611
-00004310: 3135 223e 4c69 6e20 2831 3939 3129 3c2f  15">Lin (1991)</
-00004320: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
-00004330: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
-00004340: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004350: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004360: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004370: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004380: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-00004390: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-000043a0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-000043b0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-000043c0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-000043d0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-000043e0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000043f0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004400: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004410: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004420: 3b22 3e4b 756c 6c62 6163 6b2d 4c65 6962  ;">Kullback-Leib
-00004430: 6c65 7220 6469 7665 7267 656e 6365 3c2f  ler divergence</
-00004440: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00004450: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00004460: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00004470: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00004480: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
-00004490: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-000044a0: 6f69 2e6f 7267 2f31 302e 3132 3134 2f61  oi.org/10.1214/a
-000044b0: 6f6d 732f 3131 3737 3732 3936 3934 223e  oms/1177729694">
-000044c0: 4b75 6c6c 6261 636b 2061 6e64 204c 6569  Kullback and Lei
-000044d0: 626c 6572 2028 3139 3531 293c 2f61 3e3c  bler (1951)</a><
-000044e0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
-000044f0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
-00004500: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00004510: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00004520: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00004530: 6164 6469 6e67 3a20 3870 783b 223e 4d3c  adding: 8px;">M<
-00004540: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
-00004550: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00004560: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00004570: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00004580: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
-00004590: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
-000045a0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-000045b0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
-000045c0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
-000045d0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
-000045e0: 4d4d 443c 2f74 643e 0a20 2020 203c 7464  MMD</td>.    <td
-000045f0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004600: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004610: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004620: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004630: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
-00004640: 733a 2f2f 646c 2e61 636d 2e6f 7267 2f64  s://dl.acm.org/d
-00004650: 6f69 2f31 302e 3535 3535 2f32 3138 3833  oi/10.5555/21883
-00004660: 3835 2e32 3138 3834 3130 223e 4772 6574  85.2188410">Gret
-00004670: 746f 6e20 6574 2061 6c2e 2028 3230 3132  ton et al. (2012
-00004680: 293c 2f61 3e3c 2f74 643e 0a20 203c 2f74  )</a></td>.  </t
-00004690: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
-000046a0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-000046b0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-000046c0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-000046d0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-000046e0: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
-000046f0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00004700: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00004710: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00004720: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00004730: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
-00004740: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-00004750: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-00004760: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-00004770: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-00004780: 3870 783b 223e 5053 493c 2f74 643e 0a20  8px;">PSI</td>. 
-00004790: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-000047a0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000047b0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-000047c0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-000047d0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-000047e0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-000047f0: 672f 3130 2e31 3035 372f 6a6f 7273 2e32  g/10.1057/jors.2
-00004800: 3030 382e 3134 3422 3e57 7520 616e 6420  008.144">Wu and 
-00004810: 4f6c 736f 6e20 2832 3031 3029 3c2f 613e  Olson (2010)</a>
-00004820: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
-00004830: 3c74 723e 0a20 2020 203c 7464 2072 6f77  <tr>.    <td row
-00004840: 7370 616e 3d22 3522 2073 7479 6c65 3d22  span="5" style="
-00004850: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004860: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004870: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004880: 696e 673a 2038 7078 3b22 3e53 7461 7469  ing: 8px;">Stati
-00004890: 7374 6963 616c 2074 6573 743c 2f74 643e  stical test</td>
-000048a0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-000048b0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-000048c0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-000048d0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-000048e0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
-000048f0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00004900: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00004910: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00004920: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00004930: 6469 6e67 3a20 3870 783b 223e 433c 2f74  ding: 8px;">C</t
-00004940: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00004950: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00004960: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00004970: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00004980: 6464 696e 673a 2038 7078 3b22 3e43 6869  dding: 8px;">Chi
-00004990: 2d73 7175 6172 6520 7465 7374 3c2f 7464  -square test</td
-000049a0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000049b0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000049c0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000049d0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000049e0: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
-000049f0: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
-00004a00: 2e6f 7267 2f31 302e 3130 3830 2f31 3437  .org/10.1080/147
-00004a10: 3836 3434 3030 3039 3436 3338 3937 223e  86440009463897">
-00004a20: 5065 6172 736f 6e20 2831 3930 3029 3c2f  Pearson (1900)</
-00004a30: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
-00004a40: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
-00004a50: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00004a60: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-00004a70: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00004a80: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00004a90: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
-00004aa0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
-00004ab0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
-00004ac0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
-00004ad0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
-00004ae0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
-00004af0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004b00: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004b10: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004b20: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004b30: 3b22 3e43 7261 6dc3 a972 2d76 6f6e 204d  ;">Cram..r-von M
-00004b40: 6973 6573 2074 6573 743c 2f74 643e 0a20  ises test</td>. 
-00004b50: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00004b60: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00004b70: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00004b80: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00004b90: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
-00004ba0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
-00004bb0: 672f 3130 2e31 3038 302f 3033 3436 3132  g/10.1080/034612
-00004bc0: 3338 2e31 3932 382e 3130 3431 3638 3632  38.1928.10416862
-00004bd0: 223e 4372 616d c3a9 7220 2831 3930 3229  ">Cram..r (1902)
-00004be0: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
-00004bf0: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
-00004c00: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00004c10: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
-00004c20: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
-00004c30: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
-00004c40: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
-00004c50: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
-00004c60: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
-00004c70: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
-00004c80: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
-00004c90: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
-00004ca0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
-00004cb0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
-00004cc0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00004cd0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
-00004ce0: 7078 3b22 3e4b 6f6c 6d6f 676f 726f 762d  px;">Kolmogorov-
-00004cf0: 536d 6972 6e6f 7620 7465 7374 3c2f 7464  Smirnov test</td
-00004d00: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00004d10: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00004d20: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00004d30: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00004d40: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
-00004d50: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
-00004d60: 2e6f 7267 2f31 302e 3233 3037 2f32 3238  .org/10.2307/228
-00004d70: 3030 3935 223e 4d61 7373 6579 204a 7220  0095">Massey Jr 
-00004d80: 2831 3935 3129 3c2f 613e 3c2f 7464 3e0a  (1951)</a></td>.
-00004d90: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
-00004da0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
-00004db0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-00004dc0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
-00004dd0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
-00004de0: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
-00004df0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00004e00: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00004e10: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004e20: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004e30: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
-00004e40: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004e50: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004e60: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004e70: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004e80: 696e 673a 2038 7078 3b22 3e4d 616e 6e2d  ing: 8px;">Mann-
-00004e90: 5768 6974 6e65 7920 5520 7465 7374 3c2f  Whitney U test</
-00004ea0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00004eb0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00004ec0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00004ed0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00004ee0: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
-00004ef0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-00004f00: 6f69 2e6f 7267 2f31 302e 3132 3134 2f61  oi.org/10.1214/a
-00004f10: 6f6d 732f 3131 3737 3733 3034 3931 223e  oms/1177730491">
-00004f20: 4d61 6e6e 2061 6e64 2057 6869 746e 6579  Mann and Whitney
-00004f30: 2028 3139 3437 293c 2f61 3e3c 2f74 643e   (1947)</a></td>
-00004f40: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
-00004f50: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00004f60: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00004f70: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00004f80: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00004f90: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
-00004fa0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-00004fb0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00004fc0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-00004fd0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-00004fe0: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
-00004ff0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00005000: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00005010: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00005020: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00005030: 6469 6e67 3a20 3870 783b 223e 5765 6c63  ding: 8px;">Welc
-00005040: 6827 7320 742d 7465 7374 3c2f 7464 3e0a  h's t-test</td>.
-00005050: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
-00005060: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
-00005070: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
-00005080: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
-00005090: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
-000050a0: 663d 2268 7474 7073 3a2f 2f64 6f69 2e6f  f="https://doi.o
-000050b0: 7267 2f31 302e 3233 3037 2f32 3333 3235  rg/10.2307/23325
-000050c0: 3130 223e 5765 6c63 6820 2831 3934 3729  10">Welch (1947)
-000050d0: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
-000050e0: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
-000050f0: 2072 6f77 7370 616e 3d22 3222 2073 7479   rowspan="2" sty
-00005100: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00005110: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
-00005120: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
-00005130: 7061 6464 696e 673a 2038 7078 3b22 3e53  padding: 8px;">S
-00005140: 7472 6561 6d69 6e67 3c2f 7464 3e0a 2020  treaming</td>.  
-00005150: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00005160: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00005170: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00005180: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00005190: 3a20 3870 783b 223e 4469 7374 616e 6365  : 8px;">Distance
-000051a0: 2062 6173 6564 3c2f 7464 3e0a 2020 2020   based</td>.    
-000051b0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
-000051c0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
-000051d0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-000051e0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
-000051f0: 3870 783b 223e 4d3c 2f74 643e 0a20 2020  8px;">M</td>.   
-00005200: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
-00005210: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-00005220: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
-00005230: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
-00005240: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
-00005250: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
-00005260: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
-00005270: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-00005280: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
-00005290: 3a20 3870 783b 223e 4d4d 443c 2f74 643e  : 8px;">MMD</td>
-000052a0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
-000052b0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-000052c0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
-000052d0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
-000052e0: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
-000052f0: 6566 3d22 6874 7470 733a 2f2f 646c 2e61  ef="https://dl.a
-00005300: 636d 2e6f 7267 2f64 6f69 2f31 302e 3535  cm.org/doi/10.55
-00005310: 3535 2f32 3138 3833 3835 2e32 3138 3834  55/2188385.21884
-00005320: 3130 223e 4772 6574 746f 6e20 6574 2061  10">Gretton et a
-00005330: 6c2e 2028 3230 3132 293c 2f61 3e3c 2f74  l. (2012)</a></t
-00005340: 643e 0a20 203c 2f74 723e 0a20 203c 7472  d>.  </tr>.  <tr
-00005350: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-00005360: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00005370: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-00005380: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-00005390: 6469 6e67 3a20 3870 783b 223e 5374 6174  ding: 8px;">Stat
-000053a0: 6973 7469 6361 6c20 7465 7374 3c2f 7464  istical test</td
-000053b0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
-000053c0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-000053d0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
-000053e0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
-000053f0: 6469 6e67 3a20 3870 783b 223e 553c 2f74  ding: 8px;">U</t
-00005400: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
-00005410: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
-00005420: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
-00005430: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
-00005440: 6464 696e 673a 2038 7078 3b22 3e4e 3c2f  dding: 8px;">N</
-00005450: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
-00005460: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
-00005470: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
-00005480: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
-00005490: 6164 6469 6e67 3a20 3870 783b 223e 496e  adding: 8px;">In
-000054a0: 6372 656d 656e 7461 6c20 4b6f 6c6d 6f67  cremental Kolmog
-000054b0: 6f72 6f76 2d53 6d69 726e 6f76 2074 6573  orov-Smirnov tes
-000054c0: 743c 2f74 643e 0a20 2020 203c 7464 2073  t</td>.    <td s
-000054d0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-000054e0: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
-000054f0: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
-00005500: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
-00005510: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00005520: 2f2f 646f 692e 6f72 672f 3130 2e31 3134  //doi.org/10.114
-00005530: 352f 3239 3339 3637 322e 3239 3339 3833  5/2939672.293983
-00005540: 3622 3e64 6f73 2052 6569 7320 6574 2061  6">dos Reis et a
-00005550: 6c2e 2028 3230 3136 293c 2f61 3e3c 2f74  l. (2016)</a></t
-00005560: 643e 0a20 203c 2f74 723e 0a3c 2f74 626f  d>.  </tr>.</tbo
-00005570: 6479 3e0a 3c2f 7461 626c 653e 0a0a 2323  dy>.</table>..##
-00005580: 20e2 9d97 2057 6861 7420 6973 2061 6e64   ... What is and
-00005590: 2077 6861 7420 6973 206e 6f74 2046 726f   what is not Fro
-000055a0: 7572 6f73 3f0a 0a55 6e6c 696b 6520 6f74  uros?..Unlike ot
-000055b0: 6865 7220 6c69 6272 6172 6965 7320 7468  her libraries th
-000055c0: 6174 2069 6e20 6164 6469 7469 6f6e 2074  at in addition t
-000055d0: 6f20 7072 6f76 6964 6520 6472 6966 7420  o provide drift 
-000055e0: 6465 7465 6374 696f 6e20 616c 676f 7269  detection algori
-000055f0: 7468 6d73 2c20 696e 636c 7564 6520 6f74  thms, include ot
-00005600: 6865 7220 6675 6e63 7469 6f6e 616c 6974  her functionalit
-00005610: 6965 7320 7375 6368 2061 7320 616e 6f6d  ies such as anom
-00005620: 616c 792f 6f75 746c 6965 7220 6465 7465  aly/outlier dete
-00005630: 6374 696f 6e2c 2061 6476 6572 7361 7269  ction, adversari
-00005640: 616c 2064 6574 6563 7469 6f6e 2c20 696d  al detection, im
-00005650: 6261 6c61 6e63 6520 6c65 6172 6e69 6e67  balance learning
-00005660: 2c20 616d 6f6e 6720 6f74 6865 7273 2c20  , among others, 
-00005670: 4672 6f75 726f 7320 6861 7320 616e 6420  Frouros has and 
-00005680: 7769 6c6c 202a 2a4f 4e4c 592a 2a20 6861  will **ONLY** ha
-00005690: 7665 206f 6e65 2070 7572 706f 7365 3a20  ve one purpose: 
-000056a0: 2a2a 6472 6966 7420 6465 7465 6374 696f  **drift detectio
-000056b0: 6e2a 2a2e 0a0a 5765 2066 6972 6d6c 7920  n**...We firmly 
-000056c0: 6265 6c69 6576 6520 7468 6174 206d 6163  believe that mac
-000056d0: 6869 6e65 206c 6561 726e 696e 6720 7265  hine learning re
-000056e0: 6c61 7465 6420 6c69 6272 6172 6965 7320  lated libraries 
-000056f0: 6f72 2066 7261 6d65 776f 726b 7320 7368  or frameworks sh
-00005700: 6f75 6c64 206e 6f74 2066 6f6c 6c6f 7720  ould not follow 
-00005710: 5b4a 6163 6b20 6f66 2061 6c6c 2074 7261  [Jack of all tra
-00005720: 6465 732c 206d 6173 7465 7220 6f66 206e  des, master of n
-00005730: 6f6e 655d 2868 7474 7073 3a2f 2f65 6e2e  one](https://en.
-00005740: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-00005750: 6b69 2f4a 6163 6b5f 6f66 5f61 6c6c 5f74  ki/Jack_of_all_t
-00005760: 7261 6465 732c 5f6d 6173 7465 725f 6f66  rades,_master_of
-00005770: 5f6e 6f6e 6529 2070 7269 6e63 6970 6c65  _none) principle
-00005780: 2e20 496e 7374 6561 642c 2074 6865 7920  . Instead, they 
-00005790: 7368 6f75 6c64 2062 6520 666f 6375 7365  should be focuse
-000057a0: 6420 6f6e 2061 2073 696e 676c 6520 7461  d on a single ta
-000057b0: 736b 2061 6e64 2064 6f20 6974 2077 656c  sk and do it wel
-000057c0: 6c2e 0a0a 2323 20e2 9c85 2057 686f 2069  l...## ... Who i
-000057d0: 7320 7573 696e 6720 4672 6f75 726f 733f  s using Frouros?
-000057e0: 0a0a 4672 6f75 726f 7320 6973 2061 6374  ..Frouros is act
-000057f0: 6976 656c 7920 6265 696e 6720 7573 6564  ively being used
-00005800: 2062 7920 7468 6520 666f 6c6c 6f77 696e   by the followin
-00005810: 6720 7072 6f6a 6563 7473 2074 6f20 696d  g projects to im
-00005820: 706c 656d 656e 7420 6472 6966 740a 6465  plement drift.de
-00005830: 7465 6374 696f 6e20 696e 206d 6163 6869  tection in machi
-00005840: 6e65 206c 6561 726e 696e 6720 7069 7065  ne learning pipe
-00005850: 6c69 6e65 733a 0a0a 202a 205b 4149 3445  lines:.. * [AI4E
-00005860: 4f53 435d 2868 7474 7073 3a2f 2f61 6934  OSC](https://ai4
-00005870: 656f 7363 2e65 7529 2e0a 202a 205b 694d  eosc.eu).. * [iM
-00005880: 6167 696e 655d 2868 7474 7073 3a2f 2f69  agine](https://i
-00005890: 6d61 6769 6e65 2d61 692e 6575 292e 0a0a  magine-ai.eu)...
-000058a0: 4966 2079 6f75 2077 616e 7420 796f 7572  If you want your
-000058b0: 2070 726f 6a65 6374 206c 6973 7465 6420   project listed 
-000058c0: 6865 7265 2c20 646f 206e 6f74 2068 6573  here, do not hes
-000058d0: 6974 6174 6520 746f 2073 656e 6420 7573  itate to send us
-000058e0: 2061 2070 756c 6c20 7265 7175 6573 742e   a pull request.
-000058f0: 0a0a 2323 20f0 9f91 8d20 436f 6e74 7269  ..## .... Contri
-00005900: 6275 7469 6e67 0a0a 4368 6563 6b20 6f75  buting..Check ou
-00005910: 7420 7468 6520 5b63 6f6e 7472 6962 7574  t the [contribut
-00005920: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
-00005930: 6875 622e 636f 6d2f 4946 4341 2f66 726f  hub.com/IFCA/fro
-00005940: 7572 6f73 2f62 6c6f 622f 6d61 696e 2f43  uros/blob/main/C
-00005950: 4f4e 5452 4942 5554 494e 472e 6d64 2920  ONTRIBUTING.md) 
-00005960: 7365 6374 696f 6e2e 0a0a 2323 20f0 9f92  section...## ...
-00005970: ac20 4369 7461 7469 6f6e 0a0a 416c 7468  . Citation..Alth
-00005980: 6f75 6768 2046 726f 7572 6f73 2070 6170  ough Frouros pap
-00005990: 6572 2069 7320 7374 696c 6c20 696e 2070  er is still in p
-000059a0: 7265 7072 696e 742c 2069 6620 796f 7520  reprint, if you 
-000059b0: 7761 6e74 2074 6f20 6369 7465 2069 7420  want to cite it 
-000059c0: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-000059d0: 5b70 7265 7072 696e 745d 2868 7474 7073  [preprint](https
-000059e0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-000059f0: 2f32 3230 382e 3036 3836 3829 2076 6572  /2208.06868) ver
-00005a00: 7369 6f6e 2028 746f 2062 6520 7265 706c  sion (to be repl
-00005a10: 6163 6564 2062 7920 7468 6520 7061 7065  aced by the pape
-00005a20: 7220 6f6e 6365 2069 7320 7075 626c 6973  r once is publis
-00005a30: 6865 6429 2e0a 0a60 6060 6269 6274 6578  hed)...```bibtex
-00005a40: 0a40 6172 7469 636c 657b 6365 7370 6564  .@article{cesped
-00005a50: 6573 3230 3232 6672 6f75 726f 732c 0a20  es2022frouros,. 
-00005a60: 2074 6974 6c65 3d7b 4672 6f75 726f 733a   title={Frouros:
-00005a70: 2041 2050 7974 686f 6e20 6c69 6272 6172   A Python librar
-00005a80: 7920 666f 7220 6472 6966 7420 6465 7465  y for drift dete
-00005a90: 6374 696f 6e20 696e 206d 6163 6869 6e65  ction in machine
-00005aa0: 206c 6561 726e 696e 6720 7379 7374 656d   learning system
-00005ab0: 737d 2c0a 2020 6175 7468 6f72 3d7b 437b  s},.  author={C{
-00005ac0: 5c27 657d 7370 6564 6573 2d53 6973 6e69  \'e}spedes-Sisni
-00005ad0: 6567 612c 204a 6169 6d65 2061 6e64 204c  ega, Jaime and L
-00005ae0: 7b5c 276f 7d70 657a 2d47 6172 637b 5c27  {\'o}pez-Garc{\'
-00005af0: 5c69 7d61 2c20 7b5c 2741 7d6c 7661 726f  \i}a, {\'A}lvaro
-00005b00: 207d 2c0a 2020 6a6f 7572 6e61 6c3d 7b61   },.  journal={a
-00005b10: 7258 6976 2070 7265 7072 696e 7420 6172  rXiv preprint ar
-00005b20: 5869 763a 3232 3038 2e30 3638 3638 7d2c  Xiv:2208.06868},
-00005b30: 0a20 2079 6561 723d 7b32 3032 327d 0a7d  .  year={2022}.}
-00005b40: 0a60 6060 0a0a 2323 20f0 9f93 9d20 4c69  .```..## .... Li
-00005b50: 6365 6e73 650a 0a46 726f 7572 6f73 2069  cense..Frouros i
-00005b60: 7320 616e 206f 7065 6e2d 736f 7572 6365  s an open-source
-00005b70: 2073 6f66 7477 6172 6520 6c69 6365 6e73   software licens
-00005b80: 6564 2075 6e64 6572 2074 6865 205b 4253  ed under the [BS
-00005b90: 442d 332d 436c 6175 7365 206c 6963 656e  D-3-Clause licen
-00005ba0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-00005bb0: 7562 2e63 6f6d 2f49 4643 412f 6672 6f75  ub.com/IFCA/frou
-00005bc0: 726f 732f 626c 6f62 2f6d 6169 6e2f 4c49  ros/blob/main/LI
-00005bd0: 4345 4e53 4529 2e0a 0a23 2320 f09f 998f  CENSE)...## ....
-00005be0: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
-00005bf0: 730a 0a46 726f 7572 6f73 2068 6173 2072  s..Frouros has r
-00005c00: 6563 6569 7665 6420 6675 6e64 696e 6720  eceived funding 
-00005c10: 6672 6f6d 2074 6865 2041 6765 6e63 6961  from the Agencia
-00005c20: 2045 7374 6174 616c 2064 6520 496e 7665   Estatal de Inve
-00005c30: 7374 6967 6163 69c3 b36e 2c20 556e 6964  stigaci..n, Unid
-00005c40: 6164 2064 6520 4578 6365 6c65 6e63 6961  ad de Excelencia
-00005c50: 204d 6172 c3ad 6120 6465 204d 6165 7a74   Mar..a de Maezt
-00005c60: 752c 2072 6566 2e20 4d44 4d2d 3230 3137  u, ref. MDM-2017
-00005c70: 2d30 3736 352e 0a0a 0a                   -0765....
+00000eb0: 6272 6561 7374 2063 616e 6365 7220 6461  breast cancer da
+00000ec0: 7461 7365 7420 746f 2077 6869 6368 2063  taset to which c
+00000ed0: 6f6e 6365 7074 2064 7269 6674 2069 7420  oncept drift it 
+00000ee0: 6973 2069 6e64 7563 6564 2061 6e64 2073  is induced and s
+00000ef0: 686f 7720 7468 6520 7573 6520 6f66 2061  how the use of a
+00000f00: 2063 6f6e 6365 7074 2064 7269 6674 2064   concept drift d
+00000f10: 6574 6563 746f 7220 6c69 6b65 2044 444d  etector like DDM
+00000f20: 2028 4472 6966 7420 4465 7465 6374 696f   (Drift Detectio
+00000f30: 6e20 4d65 7468 6f64 292e 2057 6520 6361  n Method). We ca
+00000f40: 6e20 7365 6520 686f 7720 636f 6e63 6570  n see how concep
+00000f50: 7420 6472 6966 7420 6166 6665 6374 7320  t drift affects 
+00000f60: 7468 6520 7065 7266 6f72 6d61 6e63 6520  the performance 
+00000f70: 696e 2074 6572 6d73 206f 6620 6163 6375  in terms of accu
+00000f80: 7261 6379 2e0a 0a60 6060 7079 7468 6f6e  racy...```python
+00000f90: 0a69 6d70 6f72 7420 6e75 6d70 7920 6173  .import numpy as
+00000fa0: 206e 700a 6672 6f6d 2073 6b6c 6561 726e   np.from sklearn
+00000fb0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00000fc0: 206c 6f61 645f 6272 6561 7374 5f63 616e   load_breast_can
+00000fd0: 6365 720a 6672 6f6d 2073 6b6c 6561 726e  cer.from sklearn
+00000fe0: 2e6c 696e 6561 725f 6d6f 6465 6c20 696d  .linear_model im
+00000ff0: 706f 7274 204c 6f67 6973 7469 6352 6567  port LogisticReg
+00001000: 7265 7373 696f 6e0a 6672 6f6d 2073 6b6c  ression.from skl
+00001010: 6561 726e 2e6d 6f64 656c 5f73 656c 6563  earn.model_selec
+00001020: 7469 6f6e 2069 6d70 6f72 7420 7472 6169  tion import trai
+00001030: 6e5f 7465 7374 5f73 706c 6974 0a66 726f  n_test_split.fro
+00001040: 6d20 736b 6c65 6172 6e2e 7069 7065 6c69  m sklearn.pipeli
+00001050: 6e65 2069 6d70 6f72 7420 5069 7065 6c69  ne import Pipeli
+00001060: 6e65 0a66 726f 6d20 736b 6c65 6172 6e2e  ne.from sklearn.
+00001070: 7072 6570 726f 6365 7373 696e 6720 696d  preprocessing im
+00001080: 706f 7274 2053 7461 6e64 6172 6453 6361  port StandardSca
+00001090: 6c65 720a 0a66 726f 6d20 6672 6f75 726f  ler..from frouro
+000010a0: 732e 6465 7465 6374 6f72 732e 636f 6e63  s.detectors.conc
+000010b0: 6570 745f 6472 6966 7420 696d 706f 7274  ept_drift import
+000010c0: 2044 444d 2c20 4444 4d43 6f6e 6669 670a   DDM, DDMConfig.
+000010d0: 6672 6f6d 2066 726f 7572 6f73 2e6d 6574  from frouros.met
+000010e0: 7269 6373 2069 6d70 6f72 7420 5072 6571  rics import Preq
+000010f0: 7565 6e74 6961 6c45 7272 6f72 0a0a 6e70  uentialError..np
+00001100: 2e72 616e 646f 6d2e 7365 6564 2873 6565  .random.seed(see
+00001110: 643d 3331 290a 0a23 204c 6f61 6420 6272  d=31)..# Load br
+00001120: 6561 7374 2063 616e 6365 7220 6461 7461  east cancer data
+00001130: 7365 740a 582c 2079 203d 206c 6f61 645f  set.X, y = load_
+00001140: 6272 6561 7374 5f63 616e 6365 7228 7265  breast_cancer(re
+00001150: 7475 726e 5f58 5f79 3d54 7275 6529 0a0a  turn_X_y=True)..
+00001160: 2320 5370 6c69 7420 7472 6169 6e20 2837  # Split train (7
+00001170: 3025 2920 616e 6420 7465 7374 2028 3330  0%) and test (30
+00001180: 2529 0a28 0a20 2020 2058 5f74 7261 696e  %).(.    X_train
+00001190: 2c0a 2020 2020 585f 7465 7374 2c0a 2020  ,.    X_test,.  
+000011a0: 2020 795f 7472 6169 6e2c 0a20 2020 2079    y_train,.    y
+000011b0: 5f74 6573 742c 0a29 203d 2074 7261 696e  _test,.) = train
+000011c0: 5f74 6573 745f 7370 6c69 7428 582c 2079  _test_split(X, y
+000011d0: 2c20 7472 6169 6e5f 7369 7a65 3d30 2e37  , train_size=0.7
+000011e0: 2c20 7261 6e64 6f6d 5f73 7461 7465 3d33  , random_state=3
+000011f0: 3129 0a0a 2320 4465 6669 6e65 2061 6e64  1)..# Define and
+00001200: 2066 6974 206d 6f64 656c 0a70 6970 656c   fit model.pipel
+00001210: 696e 6520 3d20 5069 7065 6c69 6e65 280a  ine = Pipeline(.
+00001220: 2020 2020 5b0a 2020 2020 2020 2020 2822      [.        ("
+00001230: 7363 616c 6572 222c 2053 7461 6e64 6172  scaler", Standar
+00001240: 6453 6361 6c65 7228 2929 2c0a 2020 2020  dScaler()),.    
+00001250: 2020 2020 2822 6d6f 6465 6c22 2c20 4c6f      ("model", Lo
+00001260: 6769 7374 6963 5265 6772 6573 7369 6f6e  gisticRegression
+00001270: 2829 292c 0a20 2020 205d 0a29 0a70 6970  ()),.    ].).pip
+00001280: 656c 696e 652e 6669 7428 583d 585f 7472  eline.fit(X=X_tr
+00001290: 6169 6e2c 2079 3d79 5f74 7261 696e 290a  ain, y=y_train).
+000012a0: 0a23 2044 6574 6563 746f 7220 636f 6e66  .# Detector conf
+000012b0: 6967 7572 6174 696f 6e20 616e 6420 696e  iguration and in
+000012c0: 7374 616e 7469 6174 696f 6e0a 636f 6e66  stantiation.conf
+000012d0: 6967 203d 2044 444d 436f 6e66 6967 280a  ig = DDMConfig(.
+000012e0: 2020 2020 7761 726e 696e 675f 6c65 7665      warning_leve
+000012f0: 6c3d 322e 302c 0a20 2020 2064 7269 6674  l=2.0,.    drift
+00001300: 5f6c 6576 656c 3d33 2e30 2c0a 2020 2020  _level=3.0,.    
+00001310: 6d69 6e5f 6e75 6d5f 696e 7374 616e 6365  min_num_instance
+00001320: 733d 3235 2c20 2023 206d 696e 696d 756d  s=25,  # minimum
+00001330: 206e 756d 6265 7220 6f66 2069 6e73 7461   number of insta
+00001340: 6e63 6573 2062 6566 6f72 6520 6368 6563  nces before chec
+00001350: 6b69 6e67 2066 6f72 2063 6f6e 6365 7074  king for concept
+00001360: 2064 7269 6674 0a29 0a64 6574 6563 746f   drift.).detecto
+00001370: 7220 3d20 4444 4d28 636f 6e66 6967 3d63  r = DDM(config=c
+00001380: 6f6e 6669 6729 0a0a 2320 4d65 7472 6963  onfig)..# Metric
+00001390: 2074 6f20 636f 6d70 7574 6520 6163 6375   to compute accu
+000013a0: 7261 6379 0a6d 6574 7269 6320 3d20 5072  racy.metric = Pr
+000013b0: 6571 7565 6e74 6961 6c45 7272 6f72 2861  equentialError(a
+000013c0: 6c70 6861 3d31 2e30 2920 2023 2061 6c70  lpha=1.0)  # alp
+000013d0: 6861 3d31 2e30 2069 7320 6571 7569 7661  ha=1.0 is equiva
+000013e0: 6c65 6e74 2074 6f20 6e6f 726d 616c 2061  lent to normal a
+000013f0: 6363 7572 6163 790a 0a64 6566 2073 7472  ccuracy..def str
+00001400: 6561 6d5f 7465 7374 2858 5f74 6573 742c  eam_test(X_test,
+00001410: 2079 5f74 6573 742c 2079 2c20 6d65 7472   y_test, y, metr
+00001420: 6963 2c20 6465 7465 6374 6f72 293a 0a20  ic, detector):. 
+00001430: 2020 2022 2222 5369 6d75 6c61 7465 2064     """Simulate d
+00001440: 6174 6120 7374 7265 616d 206f 7665 7220  ata stream over 
+00001450: 585f 7465 7374 2061 6e64 2079 5f74 6573  X_test and y_tes
+00001460: 742e 2079 2069 7320 7468 6520 7472 7565  t. y is the true
+00001470: 206c 6162 656c 2e22 2222 0a20 2020 2064   label.""".    d
+00001480: 7269 6674 5f66 6c61 6720 3d20 4661 6c73  rift_flag = Fals
+00001490: 650a 2020 2020 666f 7220 692c 2028 582c  e.    for i, (X,
+000014a0: 2079 2920 696e 2065 6e75 6d65 7261 7465   y) in enumerate
+000014b0: 287a 6970 2858 5f74 6573 742c 2079 5f74  (zip(X_test, y_t
+000014c0: 6573 7429 293a 0a20 2020 2020 2020 2079  est)):.        y
+000014d0: 5f70 7265 6420 3d20 7069 7065 6c69 6e65  _pred = pipeline
+000014e0: 2e70 7265 6469 6374 2858 2e72 6573 6861  .predict(X.resha
+000014f0: 7065 2831 2c20 2d31 2929 0a20 2020 2020  pe(1, -1)).     
+00001500: 2020 2065 7272 6f72 203d 2031 202d 2028     error = 1 - (
+00001510: 795f 7072 6564 2e69 7465 6d28 2920 3d3d  y_pred.item() ==
+00001520: 2079 2e69 7465 6d28 2929 0a20 2020 2020   y.item()).     
+00001530: 2020 206d 6574 7269 635f 6572 726f 7220     metric_error 
+00001540: 3d20 6d65 7472 6963 2865 7272 6f72 5f76  = metric(error_v
+00001550: 616c 7565 3d65 7272 6f72 290a 2020 2020  alue=error).    
+00001560: 2020 2020 5f20 3d20 6465 7465 6374 6f72      _ = detector
+00001570: 2e75 7064 6174 6528 7661 6c75 653d 6572  .update(value=er
+00001580: 726f 7229 0a20 2020 2020 2020 2073 7461  ror).        sta
+00001590: 7475 7320 3d20 6465 7465 6374 6f72 2e73  tus = detector.s
+000015a0: 7461 7475 730a 2020 2020 2020 2020 6966  tatus.        if
+000015b0: 2073 7461 7475 735b 2264 7269 6674 225d   status["drift"]
+000015c0: 2061 6e64 206e 6f74 2064 7269 6674 5f66   and not drift_f
+000015d0: 6c61 673a 0a20 2020 2020 2020 2020 2020  lag:.           
+000015e0: 2064 7269 6674 5f66 6c61 6720 3d20 5472   drift_flag = Tr
+000015f0: 7565 0a20 2020 2020 2020 2020 2020 2070  ue.            p
+00001600: 7269 6e74 2866 2243 6f6e 6365 7074 2064  rint(f"Concept d
+00001610: 7269 6674 2064 6574 6563 7465 6420 6174  rift detected at
+00001620: 2073 7465 7020 7b69 7d2e 2041 6363 7572   step {i}. Accur
+00001630: 6163 793a 207b 3120 2d20 6d65 7472 6963  acy: {1 - metric
+00001640: 5f65 7272 6f72 3a2e 3466 7d22 290a 2020  _error:.4f}").  
+00001650: 2020 6966 206e 6f74 2064 7269 6674 5f66    if not drift_f
+00001660: 6c61 673a 0a20 2020 2020 2020 2070 7269  lag:.        pri
+00001670: 6e74 2822 4e6f 2063 6f6e 6365 7074 2064  nt("No concept d
+00001680: 7269 6674 2064 6574 6563 7465 6422 290a  rift detected").
+00001690: 2020 2020 7072 696e 7428 6622 4669 6e61      print(f"Fina
+000016a0: 6c20 6163 6375 7261 6379 3a20 7b31 202d  l accuracy: {1 -
+000016b0: 206d 6574 7269 635f 6572 726f 723a 2e34   metric_error:.4
+000016c0: 667d 5c6e 2229 0a0a 2320 5369 6d75 6c61  f}\n")..# Simula
+000016d0: 7465 2064 6174 6120 7374 7265 616d 2028  te data stream (
+000016e0: 6173 7375 6d69 6e67 2074 6573 7420 6c61  assuming test la
+000016f0: 6265 6c20 6176 6169 6c61 626c 6520 6166  bel available af
+00001700: 7465 7220 6561 6368 2070 7265 6469 6374  ter each predict
+00001710: 696f 6e29 0a23 204e 6f20 636f 6e63 6570  ion).# No concep
+00001720: 7420 6472 6966 7420 6973 2065 7870 6563  t drift is expec
+00001730: 7465 6420 746f 206f 6363 7572 0a73 7472  ted to occur.str
+00001740: 6561 6d5f 7465 7374 280a 2020 2020 585f  eam_test(.    X_
+00001750: 7465 7374 3d58 5f74 6573 742c 0a20 2020  test=X_test,.   
+00001760: 2079 5f74 6573 743d 795f 7465 7374 2c0a   y_test=y_test,.
+00001770: 2020 2020 793d 792c 0a20 2020 206d 6574      y=y,.    met
+00001780: 7269 633d 6d65 7472 6963 2c0a 2020 2020  ric=metric,.    
+00001790: 6465 7465 6374 6f72 3d64 6574 6563 746f  detector=detecto
+000017a0: 722c 0a29 0a23 203e 3e20 4e6f 2063 6f6e  r,.).# >> No con
+000017b0: 6365 7074 2064 7269 6674 2064 6574 6563  cept drift detec
+000017c0: 7465 640a 2320 3e3e 2046 696e 616c 2061  ted.# >> Final a
+000017d0: 6363 7572 6163 793a 2030 2e39 3736 360a  ccuracy: 0.9766.
+000017e0: 0a23 2049 4d50 4f52 5441 4e54 3a20 496e  .# IMPORTANT: In
+000017f0: 6475 6365 2f73 696d 756c 6174 6520 636f  duce/simulate co
+00001800: 6e63 6570 7420 6472 6966 7420 696e 2074  ncept drift in t
+00001810: 6865 206c 6173 7420 7061 7274 2028 3230  he last part (20
+00001820: 2529 0a23 206f 6620 795f 7465 7374 2062  %).# of y_test b
+00001830: 7920 6d6f 6469 6679 696e 6720 736f 6d65  y modifying some
+00001840: 206c 6162 656c 7320 2835 3025 2061 7070   labels (50% app
+00001850: 726f 7829 2e20 5468 6572 6566 6f72 652c  rox). Therefore,
+00001860: 2063 6861 6e67 696e 6720 5028 797c 5829   changing P(y|X)
+00001870: 290a 6472 6966 745f 7369 7a65 203d 2069  ).drift_size = i
+00001880: 6e74 2879 5f74 6573 742e 7368 6170 655b  nt(y_test.shape[
+00001890: 305d 202a 2030 2e32 290a 795f 7465 7374  0] * 0.2).y_test
+000018a0: 5f64 7269 6674 203d 2079 5f74 6573 745b  _drift = y_test[
+000018b0: 2d64 7269 6674 5f73 697a 653a 5d0a 6d6f  -drift_size:].mo
+000018c0: 6469 6679 5f69 6478 203d 206e 702e 7261  dify_idx = np.ra
+000018d0: 6e64 6f6d 2e72 616e 6428 2a79 5f74 6573  ndom.rand(*y_tes
+000018e0: 745f 6472 6966 742e 7368 6170 6529 203c  t_drift.shape) <
+000018f0: 3d20 302e 350a 795f 7465 7374 5f64 7269  = 0.5.y_test_dri
+00001900: 6674 5b6d 6f64 6966 795f 6964 785d 203d  ft[modify_idx] =
+00001910: 2028 795f 7465 7374 5f64 7269 6674 5b6d   (y_test_drift[m
+00001920: 6f64 6966 795f 6964 785d 202b 2031 2920  odify_idx] + 1) 
+00001930: 2520 6c65 6e28 6e70 2e75 6e69 7175 6528  % len(np.unique(
+00001940: 795f 7465 7374 2929 0a79 5f74 6573 745b  y_test)).y_test[
+00001950: 2d64 7269 6674 5f73 697a 653a 5d20 3d20  -drift_size:] = 
+00001960: 795f 7465 7374 5f64 7269 6674 0a0a 2320  y_test_drift..# 
+00001970: 5265 7365 7420 6465 7465 6374 6f72 2061  Reset detector a
+00001980: 6e64 206d 6574 7269 630a 6465 7465 6374  nd metric.detect
+00001990: 6f72 2e72 6573 6574 2829 0a6d 6574 7269  or.reset().metri
+000019a0: 632e 7265 7365 7428 290a 0a23 2053 696d  c.reset()..# Sim
+000019b0: 756c 6174 6520 6461 7461 2073 7472 6561  ulate data strea
+000019c0: 6d20 2861 7373 756d 696e 6720 7465 7374  m (assuming test
+000019d0: 206c 6162 656c 2061 7661 696c 6162 6c65   label available
+000019e0: 2061 6674 6572 2065 6163 6820 7072 6564   after each pred
+000019f0: 6963 7469 6f6e 290a 2320 436f 6e63 6570  iction).# Concep
+00001a00: 7420 6472 6966 7420 6973 2065 7870 6563  t drift is expec
+00001a10: 7465 6420 746f 206f 6363 7572 2062 6563  ted to occur bec
+00001a20: 6175 7365 206f 6620 7468 6520 6c61 6265  ause of the labe
+00001a30: 6c20 6d6f 6469 6669 6361 7469 6f6e 0a73  l modification.s
+00001a40: 7472 6561 6d5f 7465 7374 280a 2020 2020  tream_test(.    
+00001a50: 585f 7465 7374 3d58 5f74 6573 742c 0a20  X_test=X_test,. 
+00001a60: 2020 2079 5f74 6573 743d 795f 7465 7374     y_test=y_test
+00001a70: 2c0a 2020 2020 793d 792c 0a20 2020 206d  ,.    y=y,.    m
+00001a80: 6574 7269 633d 6d65 7472 6963 2c0a 2020  etric=metric,.  
+00001a90: 2020 6465 7465 6374 6f72 3d64 6574 6563    detector=detec
+00001aa0: 746f 722c 0a29 0a23 203e 3e20 436f 6e63  tor,.).# >> Conc
+00001ab0: 6570 7420 6472 6966 7420 6465 7465 6374  ept drift detect
+00001ac0: 6564 2061 7420 7374 6570 2031 3432 2e20  ed at step 142. 
+00001ad0: 4163 6375 7261 6379 3a20 302e 3935 3130  Accuracy: 0.9510
+00001ae0: 0a23 203e 3e20 4669 6e61 6c20 6163 6375  .# >> Final accu
+00001af0: 7261 6379 3a20 302e 3834 3830 0a60 6060  racy: 0.8480.```
+00001b00: 0a0a 4d6f 7265 2063 6f6e 6365 7074 2064  ..More concept d
+00001b10: 7269 6674 2065 7861 6d70 6c65 7320 6361  rift examples ca
+00001b20: 6e20 6265 2066 6f75 6e64 205b 6865 7265  n be found [here
+00001b30: 5d28 6874 7470 733a 2f2f 6672 6f75 726f  ](https://frouro
+00001b40: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
+00001b50: 2f65 6e2f 6c61 7465 7374 2f65 7861 6d70  /en/latest/examp
+00001b60: 6c65 732f 636f 6e63 6570 745f 6472 6966  les/concept_drif
+00001b70: 742e 6874 6d6c 292e 0a0a 2323 2320 4461  t.html)...### Da
+00001b80: 7461 2064 7269 6674 0a0a 4173 2061 2071  ta drift..As a q
+00001b90: 7569 636b 2065 7861 6d70 6c65 2c20 7765  uick example, we
+00001ba0: 2063 616e 2075 7365 2074 6865 2069 7269   can use the iri
+00001bb0: 7320 6461 7461 7365 7420 746f 2077 6869  s dataset to whi
+00001bc0: 6368 2064 6174 6120 6472 6966 7420 6973  ch data drift is
+00001bd0: 2069 6e64 7563 6564 2061 6e64 2073 686f   induced and sho
+00001be0: 7720 7468 6520 7573 6520 6f66 2061 2064  w the use of a d
+00001bf0: 6174 6120 6472 6966 7420 6465 7465 6374  ata drift detect
+00001c00: 6f72 206c 696b 6520 4b6f 6c6d 6f67 6f72  or like Kolmogor
+00001c10: 6f76 2d53 6d69 726e 6f76 2074 6573 742e  ov-Smirnov test.
+00001c20: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00001c30: 7274 206e 756d 7079 2061 7320 6e70 0a66  rt numpy as np.f
+00001c40: 726f 6d20 736b 6c65 6172 6e2e 6461 7461  rom sklearn.data
+00001c50: 7365 7473 2069 6d70 6f72 7420 6c6f 6164  sets import load
+00001c60: 5f69 7269 730a 6672 6f6d 2073 6b6c 6561  _iris.from sklea
+00001c70: 726e 2e6d 6f64 656c 5f73 656c 6563 7469  rn.model_selecti
+00001c80: 6f6e 2069 6d70 6f72 7420 7472 6169 6e5f  on import train_
+00001c90: 7465 7374 5f73 706c 6974 0a66 726f 6d20  test_split.from 
+00001ca0: 736b 6c65 6172 6e2e 7472 6565 2069 6d70  sklearn.tree imp
+00001cb0: 6f72 7420 4465 6369 7369 6f6e 5472 6565  ort DecisionTree
+00001cc0: 436c 6173 7369 6669 6572 0a0a 6672 6f6d  Classifier..from
+00001cd0: 2066 726f 7572 6f73 2e64 6574 6563 746f   frouros.detecto
+00001ce0: 7273 2e64 6174 615f 6472 6966 7420 696d  rs.data_drift im
+00001cf0: 706f 7274 204b 5354 6573 740a 0a6e 702e  port KSTest..np.
+00001d00: 7261 6e64 6f6d 2e73 6565 6428 7365 6564  random.seed(seed
+00001d10: 3d33 3129 0a0a 2320 4c6f 6164 2069 7269  =31)..# Load iri
+00001d20: 7320 6461 7461 7365 740a 582c 2079 203d  s dataset.X, y =
+00001d30: 206c 6f61 645f 6972 6973 2872 6574 7572   load_iris(retur
+00001d40: 6e5f 585f 793d 5472 7565 290a 0a23 2053  n_X_y=True)..# S
+00001d50: 706c 6974 2074 7261 696e 2028 3730 2529  plit train (70%)
+00001d60: 2061 6e64 2074 6573 7420 2833 3025 290a   and test (30%).
+00001d70: 280a 2020 2020 585f 7472 6169 6e2c 0a20  (.    X_train,. 
+00001d80: 2020 2058 5f74 6573 742c 0a20 2020 2079     X_test,.    y
+00001d90: 5f74 7261 696e 2c0a 2020 2020 795f 7465  _train,.    y_te
+00001da0: 7374 2c0a 2920 3d20 7472 6169 6e5f 7465  st,.) = train_te
+00001db0: 7374 5f73 706c 6974 2858 2c20 792c 2074  st_split(X, y, t
+00001dc0: 7261 696e 5f73 697a 653d 302e 372c 2072  rain_size=0.7, r
+00001dd0: 616e 646f 6d5f 7374 6174 653d 3331 290a  andom_state=31).
+00001de0: 0a23 2053 6574 2074 6865 2066 6561 7475  .# Set the featu
+00001df0: 7265 2069 6e64 6578 2074 6f20 7768 6963  re index to whic
+00001e00: 6820 6465 7465 6374 6f72 2069 7320 6170  h detector is ap
+00001e10: 706c 6965 640a 6665 6174 7572 655f 6964  plied.feature_id
+00001e20: 7820 3d20 300a 0a23 2049 4d50 4f52 5441  x = 0..# IMPORTA
+00001e30: 4e54 3a20 496e 6475 6365 2f73 696d 756c  NT: Induce/simul
+00001e40: 6174 6520 6461 7461 2064 7269 6674 2069  ate data drift i
+00001e50: 6e20 7468 6520 7365 6c65 6374 6564 2066  n the selected f
+00001e60: 6561 7475 7265 206f 6620 795f 7465 7374  eature of y_test
+00001e70: 2062 790a 2320 6170 706c 7969 6e67 2073   by.# applying s
+00001e80: 6f6d 6520 6761 7573 7369 616e 206e 6f69  ome gaussian noi
+00001e90: 7365 2e20 5468 6572 6566 6f72 652c 2063  se. Therefore, c
+00001ea0: 6861 6e67 696e 6720 5028 5829 290a 585f  hanging P(X)).X_
+00001eb0: 7465 7374 5b3a 2c20 6665 6174 7572 655f  test[:, feature_
+00001ec0: 6964 785d 202b 3d20 6e70 2e72 616e 646f  idx] += np.rando
+00001ed0: 6d2e 6e6f 726d 616c 280a 2020 2020 6c6f  m.normal(.    lo
+00001ee0: 633d 302e 302c 0a20 2020 2073 6361 6c65  c=0.0,.    scale
+00001ef0: 3d33 2e30 2c0a 2020 2020 7369 7a65 3d58  =3.0,.    size=X
+00001f00: 5f74 6573 742e 7368 6170 655b 305d 2c0a  _test.shape[0],.
+00001f10: 290a 0a23 2044 6566 696e 6520 616e 6420  )..# Define and 
+00001f20: 6669 7420 6d6f 6465 6c0a 6d6f 6465 6c20  fit model.model 
+00001f30: 3d20 4465 6369 7369 6f6e 5472 6565 436c  = DecisionTreeCl
+00001f40: 6173 7369 6669 6572 2872 616e 646f 6d5f  assifier(random_
+00001f50: 7374 6174 653d 3331 290a 6d6f 6465 6c2e  state=31).model.
+00001f60: 6669 7428 583d 585f 7472 6169 6e2c 2079  fit(X=X_train, y
+00001f70: 3d79 5f74 7261 696e 290a 0a23 2053 6574  =y_train)..# Set
+00001f80: 2073 6967 6e69 6669 6361 6e63 6520 6c65   significance le
+00001f90: 7665 6c20 666f 7220 6879 706f 7468 6573  vel for hypothes
+00001fa0: 6973 2074 6573 7469 6e67 0a61 6c70 6861  is testing.alpha
+00001fb0: 203d 2030 2e30 3031 0a23 2044 6566 696e   = 0.001.# Defin
+00001fc0: 6520 616e 6420 6669 7420 6465 7465 6374  e and fit detect
+00001fd0: 6f72 0a64 6574 6563 746f 7220 3d20 4b53  or.detector = KS
+00001fe0: 5465 7374 2829 0a5f 203d 2064 6574 6563  Test()._ = detec
+00001ff0: 746f 722e 6669 7428 583d 585f 7472 6169  tor.fit(X=X_trai
+00002000: 6e5b 3a2c 2066 6561 7475 7265 5f69 6478  n[:, feature_idx
+00002010: 5d29 0a0a 2320 4170 706c 7920 6465 7465  ])..# Apply dete
+00002020: 6374 6f72 2074 6f20 7468 6520 7365 6c65  ctor to the sele
+00002030: 6374 6564 2066 6561 7475 7265 206f 6620  cted feature of 
+00002040: 585f 7465 7374 0a72 6573 756c 742c 205f  X_test.result, _
+00002050: 203d 2064 6574 6563 746f 722e 636f 6d70   = detector.comp
+00002060: 6172 6528 583d 585f 7465 7374 5b3a 2c20  are(X=X_test[:, 
+00002070: 6665 6174 7572 655f 6964 785d 290a 0a23  feature_idx])..#
+00002080: 2043 6865 636b 2069 6620 6472 6966 7420   Check if drift 
+00002090: 6973 2074 616b 696e 6720 706c 6163 650a  is taking place.
+000020a0: 6966 2072 6573 756c 742e 705f 7661 6c75  if result.p_valu
+000020b0: 6520 3c3d 2061 6c70 6861 3a0a 2020 2020  e <= alpha:.    
+000020c0: 7072 696e 7428 6622 4461 7461 2064 7269  print(f"Data dri
+000020d0: 6674 2064 6574 6563 7465 6420 6174 2066  ft detected at f
+000020e0: 6561 7475 7265 207b 6665 6174 7572 655f  eature {feature_
+000020f0: 6964 787d 2229 0a65 6c73 653a 0a20 2020  idx}").else:.   
+00002100: 2070 7269 6e74 2866 224e 6f20 6461 7461   print(f"No data
+00002110: 2064 7269 6674 2064 6574 6563 7465 6420   drift detected 
+00002120: 6174 2066 6561 7475 7265 207b 6665 6174  at feature {feat
+00002130: 7572 655f 6964 787d 2229 0a23 203e 3e20  ure_idx}").# >> 
+00002140: 4461 7461 2064 7269 6674 2064 6574 6563  Data drift detec
+00002150: 7465 6420 6174 2066 6561 7475 7265 2030  ted at feature 0
+00002160: 0a23 2054 6865 7265 666f 7265 2c20 7765  .# Therefore, we
+00002170: 2063 616e 2072 656a 6563 7420 4830 2028   can reject H0 (
+00002180: 626f 7468 2073 616d 706c 6573 2063 6f6d  both samples com
+00002190: 6520 6672 6f6d 2074 6865 2073 616d 6520  e from the same 
+000021a0: 6469 7374 7269 6275 7469 6f6e 292e 0a60  distribution)..`
+000021b0: 6060 0a0a 4d6f 7265 2064 6174 6120 6472  ``..More data dr
+000021c0: 6966 7420 6578 616d 706c 6573 2063 616e  ift examples can
+000021d0: 2062 6520 666f 756e 6420 5b68 6572 655d   be found [here]
+000021e0: 2868 7474 7073 3a2f 2f66 726f 7572 6f73  (https://frouros
+000021f0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002200: 656e 2f6c 6174 6573 742f 6578 616d 706c  en/latest/exampl
+00002210: 6573 2f64 6174 615f 6472 6966 742e 6874  es/data_drift.ht
+00002220: 6d6c 292e 0a0a 2323 20f0 9f9b a020 496e  ml)...## .... In
+00002230: 7374 616c 6c61 7469 6f6e 0a0a 4672 6f75  stallation..Frou
+00002240: 726f 7320 6361 6e20 6265 2069 6e73 7461  ros can be insta
+00002250: 6c6c 6564 2076 6961 2070 6970 3a0a 0a60  lled via pip:..`
+00002260: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00002270: 6c6c 2066 726f 7572 6f73 0a60 6060 0a0a  ll frouros.```..
+00002280: 2323 20f0 9f95 b5f0 9f8f bbe2 808d e299  ## .............
+00002290: 82ef b88f efb8 8f20 4472 6966 7420 6465  ....... Drift de
+000022a0: 7465 6374 696f 6e20 6d65 7468 6f64 730a  tection methods.
+000022b0: 0a54 6865 2063 7572 7265 6e74 6c79 2069  .The currently i
+000022c0: 6d70 6c65 6d65 6e74 6564 2064 6574 6563  mplemented detec
+000022d0: 746f 7273 2061 7265 206c 6973 7465 6420  tors are listed 
+000022e0: 696e 2074 6865 2066 6f6c 6c6f 7769 6e67  in the following
+000022f0: 2074 6162 6c65 2e0a 0a3c 7461 626c 6520   table...<table 
+00002300: 7374 796c 653d 2277 6964 7468 3a20 3130  style="width: 10
+00002310: 3025 3b20 7465 7874 2d61 6c69 676e 3a20  0%; text-align: 
+00002320: 6365 6e74 6572 3b20 626f 7264 6572 2d63  center; border-c
+00002330: 6f6c 6c61 7073 653a 2063 6f6c 6c61 7073  ollapse: collaps
+00002340: 653b 2062 6f72 6465 723a 2031 7078 2073  e; border: 1px s
+00002350: 6f6c 6964 2067 7265 793b 223e 0a20 203c  olid grey;">.  <
+00002360: 7468 6561 643e 0a20 2020 203c 7472 3e0a  thead>.    <tr>.
+00002370: 2020 2020 3c74 6820 7374 796c 653d 2274      <th style="t
+00002380: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00002390: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000023a0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000023b0: 6e67 3a20 3470 783b 223e 4472 6966 7420  ng: 4px;">Drift 
+000023c0: 6465 7465 6374 6f72 3c2f 7468 3e0a 2020  detector</th>.  
+000023d0: 2020 3c74 6820 7374 796c 653d 2274 6578    <th style="tex
+000023e0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000023f0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002400: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002410: 3a20 3470 783b 223e 5479 7065 3c2f 7468  : 4px;">Type</th
+00002420: 3e0a 2020 2020 3c74 6820 7374 796c 653d  >.    <th style=
+00002430: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002440: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002450: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002460: 6469 6e67 3a20 3470 783b 223e 4661 6d69  ding: 4px;">Fami
+00002470: 6c79 3c2f 7468 3e0a 2020 2020 3c74 6820  ly</th>.    <th 
+00002480: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00002490: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000024a0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000024b0: 793b 2070 6164 6469 6e67 3a20 3470 783b  y; padding: 4px;
+000024c0: 223e 556e 6976 6172 6961 7465 2028 5529  ">Univariate (U)
+000024d0: 202f 204d 756c 7469 7661 7269 6174 6520   / Multivariate 
+000024e0: 284d 293c 2f74 683e 0a20 2020 203c 7468  (M)</th>.    <th
+000024f0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00002500: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00002510: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00002520: 6579 3b20 7061 6464 696e 673a 2034 7078  ey; padding: 4px
+00002530: 3b22 3e4e 756d 6572 6963 616c 2028 4e29  ;">Numerical (N)
+00002540: 202f 2043 6174 6567 6f72 6963 616c 2028   / Categorical (
+00002550: 4329 3c2f 7468 3e0a 2020 2020 3c74 6820  C)</th>.    <th 
+00002560: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00002570: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00002580: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00002590: 793b 2070 6164 6469 6e67 3a20 3470 783b  y; padding: 4px;
+000025a0: 223e 4d65 7468 6f64 3c2f 7468 3e0a 2020  ">Method</th>.  
+000025b0: 2020 3c74 6820 7374 796c 653d 2274 6578    <th style="tex
+000025c0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000025d0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000025e0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000025f0: 3a20 3470 783b 223e 5265 6665 7265 6e63  : 4px;">Referenc
+00002600: 653c 2f74 683e 0a20 2020 203c 2f74 723e  e</th>.    </tr>
+00002610: 0a20 203c 2f74 6865 6164 3e0a 2020 3c74  .  </thead>.  <t
+00002620: 626f 6479 3e0a 2020 3c74 723e 0a20 2020  body>.  <tr>.   
+00002630: 203c 7464 2072 6f77 7370 616e 3d22 3133   <td rowspan="13
+00002640: 2220 7374 796c 653d 2274 6578 742d 616c  " style="text-al
+00002650: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00002660: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00002670: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00002680: 783b 223e 436f 6e63 6570 7420 6472 6966  x;">Concept drif
+00002690: 743c 2f74 643e 0a20 2020 203c 7464 2072  t</td>.    <td r
+000026a0: 6f77 7370 616e 3d22 3133 2220 7374 796c  owspan="13" styl
+000026b0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000026c0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000026d0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000026e0: 6164 6469 6e67 3a20 3870 783b 223e 5374  adding: 8px;">St
+000026f0: 7265 616d 696e 673c 2f74 643e 0a20 2020  reaming</td>.   
+00002700: 203c 7464 2072 6f77 7370 616e 3d22 3422   <td rowspan="4"
+00002710: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00002720: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00002730: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00002740: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00002750: 3b22 3e43 6861 6e67 6520 6465 7465 6374  ;">Change detect
+00002760: 696f 6e3c 2f74 643e 0a20 2020 203c 7464  ion</td>.    <td
+00002770: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00002780: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00002790: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000027a0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000027b0: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
+000027c0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+000027d0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+000027e0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+000027f0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00002800: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
+00002810: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00002820: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00002830: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00002840: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00002850: 7078 3b22 3e42 4f43 443c 2f74 643e 0a20  px;">BOCD</td>. 
+00002860: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00002870: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00002880: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00002890: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000028a0: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
+000028b0: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+000028c0: 672f 3130 2e34 3835 3530 2f61 7258 6976  g/10.48550/arXiv
+000028d0: 2e30 3731 302e 3337 3432 223e 4164 616d  .0710.3742">Adam
+000028e0: 7320 616e 6420 4d61 634b 6179 2028 3230  s and MacKay (20
+000028f0: 3037 293c 2f61 3e3c 2f74 643e 0a20 203c  07)</a></td>.  <
+00002900: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
+00002910: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00002920: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00002930: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00002940: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00002950: 3870 783b 223e 553c 2f74 643e 0a20 2020  8px;">U</td>.   
+00002960: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002970: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002980: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002990: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+000029a0: 2038 7078 3b22 3e4e 3c2f 7464 3e0a 2020   8px;">N</td>.  
+000029b0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+000029c0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+000029d0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000029e0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000029f0: 3a20 3870 783b 223e 4355 5355 4d3c 2f74  : 8px;">CUSUM</t
+00002a00: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00002a10: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00002a20: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00002a30: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00002a40: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
+00002a50: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+00002a60: 692e 6f72 672f 3130 2e32 3330 372f 3233  i.org/10.2307/23
+00002a70: 3333 3030 3922 3e50 6167 6520 2831 3935  33009">Page (195
+00002a80: 3429 3c2f 613e 3c2f 7464 3e0a 2020 3c2f  4)</a></td>.  </
+00002a90: 7472 3e0a 2020 3c74 723e 0a20 2020 203c  tr>.  <tr>.    <
+00002aa0: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00002ab0: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00002ac0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00002ad0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00002ae0: 7078 3b22 3e55 3c2f 7464 3e0a 2020 2020  px;">U</td>.    
+00002af0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+00002b00: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00002b10: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00002b20: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00002b30: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
+00002b40: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002b50: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002b60: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002b70: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00002b80: 2038 7078 3b22 3e47 656f 6d65 7472 6963   8px;">Geometric
+00002b90: 206d 6f76 696e 6720 6176 6572 6167 653c   moving average<
+00002ba0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00002bb0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00002bc0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00002bd0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00002be0: 7061 6464 696e 673a 2038 7078 3b22 3e3c  padding: 8px;"><
+00002bf0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002c00: 646f 692e 6f72 672f 3130 2e32 3330 372f  doi.org/10.2307/
+00002c10: 3132 3636 3434 3322 3e52 6f62 6572 7473  1266443">Roberts
+00002c20: 2028 3139 3539 293c 2f61 3e3c 2f74 643e   (1959)</a></td>
+00002c30: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+00002c40: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00002c50: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00002c60: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00002c70: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00002c80: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
+00002c90: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00002ca0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00002cb0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00002cc0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00002cd0: 696e 673a 2038 7078 3b22 3e4e 3c2f 7464  ing: 8px;">N</td
+00002ce0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00002cf0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002d00: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002d10: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002d20: 6469 6e67 3a20 3870 783b 223e 5061 6765  ding: 8px;">Page
+00002d30: 2048 696e 6b6c 6579 3c2f 7464 3e0a 2020   Hinkley</td>.  
+00002d40: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00002d50: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00002d60: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002d70: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002d80: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00002d90: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00002da0: 2f31 302e 3233 3037 2f32 3333 3330 3039  /10.2307/2333009
+00002db0: 223e 5061 6765 2028 3139 3534 293c 2f61  ">Page (1954)</a
+00002dc0: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+00002dd0: 203c 7472 3e0a 2020 2020 3c74 6420 726f   <tr>.    <td ro
+00002de0: 7773 7061 6e3d 2236 2220 7374 796c 653d  wspan="6" style=
+00002df0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002e00: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002e10: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002e20: 6469 6e67 3a20 3870 783b 223e 5374 6174  ding: 8px;">Stat
+00002e30: 6973 7469 6361 6c20 7072 6f63 6573 7320  istical process 
+00002e40: 636f 6e74 726f 6c3c 2f74 643e 0a20 2020  control</td>.   
+00002e50: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00002e60: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00002e70: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00002e80: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00002e90: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
+00002ea0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00002eb0: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00002ec0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00002ed0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00002ee0: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
+00002ef0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00002f00: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00002f10: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00002f20: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00002f30: 673a 2038 7078 3b22 3e44 444d 3c2f 7464  g: 8px;">DDM</td
+00002f40: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00002f50: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00002f60: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00002f70: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00002f80: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
+00002f90: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
+00002fa0: 2e6f 7267 2f31 302e 3130 3037 2f39 3738  .org/10.1007/978
+00002fb0: 2d33 2d35 3430 2d32 3836 3435 2d35 5f32  -3-540-28645-5_2
+00002fc0: 3922 3e47 616d 6120 6574 2061 6c2e 2028  9">Gama et al. (
+00002fd0: 3230 3034 293c 2f61 3e3c 2f74 643e 0a20  2004)</a></td>. 
+00002fe0: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
+00002ff0: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00003000: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00003010: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00003020: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00003030: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
+00003040: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00003050: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00003060: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00003070: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00003080: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
+00003090: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+000030a0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+000030b0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000030c0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000030d0: 6e67 3a20 3870 783b 223e 4543 4444 2d57  ng: 8px;">ECDD-W
+000030e0: 543c 2f74 643e 0a20 2020 203c 7464 2073  T</td>.    <td s
+000030f0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003100: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003110: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003120: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003130: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00003140: 2f2f 646f 692e 6f72 672f 3130 2e31 3031  //doi.org/10.101
+00003150: 362f 6a2e 7061 7472 6563 2e32 3031 312e  6/j.patrec.2011.
+00003160: 3038 2e30 3139 223e 526f 7373 2065 7420  08.019">Ross et 
+00003170: 616c 2e20 2832 3031 3229 3c2f 613e 3c2f  al. (2012)</a></
+00003180: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00003190: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+000031a0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000031b0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000031c0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000031d0: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+000031e0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000031f0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00003200: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003210: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003220: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00003230: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003240: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003250: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003260: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003270: 7061 6464 696e 673a 2038 7078 3b22 3e45  padding: 8px;">E
+00003280: 4444 4d3c 2f74 643e 0a20 2020 203c 7464  DDM</td>.    <td
+00003290: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+000032a0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+000032b0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000032c0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000032d0: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
+000032e0: 733a 2f2f 7777 772e 7265 7365 6172 6368  s://www.research
+000032f0: 6761 7465 2e6e 6574 2f70 7562 6c69 6361  gate.net/publica
+00003300: 7469 6f6e 2f32 3435 3939 3937 3034 5f45  tion/245999704_E
+00003310: 6172 6c79 5f44 7269 6674 5f44 6574 6563  arly_Drift_Detec
+00003320: 7469 6f6e 5f4d 6574 686f 6422 3e42 6165  tion_Method">Bae
+00003330: 6e61 2d47 6172 63c4 b161 2065 7420 616c  na-Garc..a et al
+00003340: 2e20 2832 3030 3629 3c2f 613e 3c2f 7464  . (2006)</a></td
+00003350: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+00003360: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00003370: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003380: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003390: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000033a0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
+000033b0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+000033c0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+000033d0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+000033e0: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+000033f0: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
+00003400: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00003410: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00003420: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00003430: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00003440: 6464 696e 673a 2038 7078 3b22 3e48 4444  dding: 8px;">HDD
+00003450: 4d2d 413c 2f74 643e 0a20 2020 203c 7464  M-A</td>.    <td
+00003460: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00003470: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00003480: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00003490: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000034a0: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
+000034b0: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
+000034c0: 3130 392f 544b 4445 2e32 3031 342e 3233  109/TKDE.2014.23
+000034d0: 3435 3338 3222 3e46 7269 6173 2d42 6c61  45382">Frias-Bla
+000034e0: 6e63 6f20 6574 2061 6c2e 2028 3230 3134  nco et al. (2014
+000034f0: 293c 2f61 3e3c 2f74 643e 0a20 203c 2f74  )</a></td>.  </t
+00003500: 723e 0a20 203c 7472 3e0a 2020 2020 3c74  r>.  <tr>.    <t
+00003510: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00003520: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00003530: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00003540: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00003550: 783b 223e 553c 2f74 643e 0a20 2020 203c  x;">U</td>.    <
+00003560: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00003570: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00003580: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00003590: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+000035a0: 7078 3b22 3e4e 3c2f 7464 3e0a 2020 2020  px;">N</td>.    
+000035b0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+000035c0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+000035d0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+000035e0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+000035f0: 3870 783b 223e 4844 444d 2d57 3c2f 7464  8px;">HDDM-W</td
+00003600: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00003610: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00003620: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00003630: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00003640: 6469 6e67 3a20 3870 783b 223e 3c61 2068  ding: 8px;"><a h
+00003650: 7265 663d 2268 7474 7073 3a2f 2f64 6f69  ref="https://doi
+00003660: 2e6f 7267 2f31 302e 3131 3039 2f54 4b44  .org/10.1109/TKD
+00003670: 452e 3230 3134 2e32 3334 3533 3832 223e  E.2014.2345382">
+00003680: 4672 6961 732d 426c 616e 636f 2065 7420  Frias-Blanco et 
+00003690: 616c 2e20 2832 3031 3429 3c2f 613e 3c2f  al. (2014)</a></
+000036a0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+000036b0: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+000036c0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+000036d0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000036e0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000036f0: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+00003700: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+00003710: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00003720: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003730: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003740: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00003750: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003760: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003770: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003780: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003790: 7061 6464 696e 673a 2038 7078 3b22 3e52  padding: 8px;">R
+000037a0: 4444 4d3c 2f74 643e 0a20 2020 203c 7464  DDM</td>.    <td
+000037b0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+000037c0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+000037d0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+000037e0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+000037f0: 3b22 3e3c 6120 6872 6566 3d22 6874 7470  ;"><a href="http
+00003800: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
+00003810: 3031 362f 6a2e 6573 7761 2e32 3031 372e  016/j.eswa.2017.
+00003820: 3038 2e30 3233 223e 4261 7272 6f73 2065  08.023">Barros e
+00003830: 7420 616c 2e20 2832 3031 3729 3c2f 613e  t al. (2017)</a>
+00003840: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
+00003850: 3c74 723e 0a20 2020 203c 7464 2072 6f77  <tr>.    <td row
+00003860: 7370 616e 3d22 3322 2073 7479 6c65 3d22  span="3" style="
+00003870: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00003880: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00003890: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000038a0: 696e 673a 2038 7078 3b22 3e57 696e 646f  ing: 8px;">Windo
+000038b0: 7720 6261 7365 643c 2f74 643e 0a20 2020  w based</td>.   
+000038c0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+000038d0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+000038e0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+000038f0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00003900: 2038 7078 3b22 3e55 3c2f 7464 3e0a 2020   8px;">U</td>.  
+00003910: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00003920: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00003930: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00003940: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00003950: 3a20 3870 783b 223e 4e3c 2f74 643e 0a20  : 8px;">N</td>. 
+00003960: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00003970: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00003980: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00003990: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000039a0: 673a 2038 7078 3b22 3e41 4457 494e 3c2f  g: 8px;">ADWIN</
+000039b0: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000039c0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000039d0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000039e0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000039f0: 6164 6469 6e67 3a20 3870 783b 223e 3c61  adding: 8px;"><a
+00003a00: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00003a10: 6f69 2e6f 7267 2f31 302e 3131 3337 2f31  oi.org/10.1137/1
+00003a20: 2e39 3738 3136 3131 3937 3237 3731 2e34  .9781611972771.4
+00003a30: 3222 3e42 6966 6574 2061 6e64 2047 6176  2">Bifet and Gav
+00003a40: 616c 6461 2028 3230 3037 293c 2f61 3e3c  alda (2007)</a><
+00003a50: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00003a60: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
+00003a70: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00003a80: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00003a90: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00003aa0: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
+00003ab0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00003ac0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00003ad0: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00003ae0: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00003af0: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
+00003b00: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00003b10: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00003b20: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00003b30: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00003b40: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00003b50: 4b53 5749 4e3c 2f74 643e 0a20 2020 203c  KSWIN</td>.    <
+00003b60: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00003b70: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00003b80: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00003b90: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00003ba0: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+00003bb0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00003bc0: 2e31 3031 362f 6a2e 6e65 7563 6f6d 2e32  .1016/j.neucom.2
+00003bd0: 3031 392e 3131 2e31 3131 223e 5261 6162  019.11.111">Raab
+00003be0: 2065 7420 616c 2e20 2832 3032 3029 3c2f   et al. (2020)</
+00003bf0: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
+00003c00: 2020 3c74 723e 0a20 2020 203c 7464 2073    <tr>.    <td s
+00003c10: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003c20: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003c30: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003c40: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003c50: 3e55 3c2f 7464 3e0a 2020 2020 3c74 6420  >U</td>.    <td 
+00003c60: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003c70: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003c80: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003c90: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003ca0: 223e 4e3c 2f74 643e 0a20 2020 203c 7464  ">N</td>.    <td
+00003cb0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00003cc0: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00003cd0: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00003ce0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00003cf0: 3b22 3e53 5445 5044 3c2f 7464 3e0a 2020  ;">STEPD</td>.  
+00003d00: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00003d10: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00003d20: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00003d30: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00003d40: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00003d50: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00003d60: 2f31 302e 3130 3037 2f39 3738 2d33 2d35  /10.1007/978-3-5
+00003d70: 3430 2d37 3534 3838 2d36 5f32 3722 3e4e  40-75488-6_27">N
+00003d80: 6973 6869 6461 2061 6e64 2059 616d 6175  ishida and Yamau
+00003d90: 6368 6920 2832 3030 3729 3c2f 613e 3c2f  chi (2007)</a></
+00003da0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00003db0: 723e 0a20 2020 203c 7464 2072 6f77 7370  r>.    <td rowsp
+00003dc0: 616e 3d22 3136 2220 7374 796c 653d 2274  an="16" style="t
+00003dd0: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00003de0: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00003df0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00003e00: 6e67 3a20 3870 783b 223e 4461 7461 2064  ng: 8px;">Data d
+00003e10: 7269 6674 3c2f 7464 3e0a 2020 2020 3c74  rift</td>.    <t
+00003e20: 6420 726f 7773 7061 6e3d 2231 3422 2073  d rowspan="14" s
+00003e30: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003e40: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003e50: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003e60: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003e70: 3e42 6174 6368 3c2f 7464 3e0a 2020 2020  >Batch</td>.    
+00003e80: 3c74 6420 726f 7773 7061 6e3d 2239 2220  <td rowspan="9" 
+00003e90: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003ea0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003eb0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003ec0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003ed0: 223e 4469 7374 616e 6365 2062 6173 6564  ">Distance based
+00003ee0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00003ef0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00003f00: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00003f10: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00003f20: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00003f30: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00003f40: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00003f50: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00003f60: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00003f70: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00003f80: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+00003f90: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00003fa0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00003fb0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00003fc0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00003fd0: 223e 416e 6465 7273 6f6e 2d44 6172 6c69  ">Anderson-Darli
+00003fe0: 6e67 2074 6573 743c 2f74 643e 0a20 2020  ng test</td>.   
+00003ff0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00004000: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00004010: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00004020: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004030: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
+00004040: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00004050: 3130 2e32 3330 372f 3232 3838 3830 3522  10.2307/2288805"
+00004060: 3e53 6368 6f6c 7a20 616e 6420 5374 6570  >Scholz and Step
+00004070: 6865 6e73 2028 3139 3837 293c 2f61 3e3c  hens (1987)</a><
+00004080: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00004090: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
+000040a0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000040b0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000040c0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000040d0: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
+000040e0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+000040f0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004100: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004110: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004120: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
+00004130: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00004140: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00004150: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00004160: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00004170: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004180: 4268 6174 7461 6368 6172 7979 6120 6469  Bhattacharyya di
+00004190: 7374 616e 6365 3c2f 7464 3e0a 2020 2020  stance</td>.    
+000041a0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+000041b0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+000041c0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+000041d0: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+000041e0: 3870 783b 223e 3c61 2068 7265 663d 2268  8px;"><a href="h
+000041f0: 7474 7073 3a2f 2f77 7777 2e6a 7374 6f72  ttps://www.jstor
+00004200: 2e6f 7267 2f73 7461 626c 652f 3235 3034  .org/stable/2504
+00004210: 3738 3832 223e 4268 6174 7461 6368 6172  7882">Bhattachar
+00004220: 7979 6120 2831 3934 3629 3c2f 613e 3c2f  yya (1946)</a></
+00004230: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00004240: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+00004250: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00004260: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00004270: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00004280: 6464 696e 673a 2038 7078 3b22 3e55 3c2f  dding: 8px;">U</
+00004290: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+000042a0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000042b0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000042c0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+000042d0: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+000042e0: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+000042f0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004300: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004310: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004320: 7061 6464 696e 673a 2038 7078 3b22 3e45  padding: 8px;">E
+00004330: 6172 7468 204d 6f76 6572 2773 2064 6973  arth Mover's dis
+00004340: 7461 6e63 653c 2f74 643e 0a20 2020 203c  tance</td>.    <
+00004350: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004360: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004370: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004380: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004390: 7078 3b22 3e3c 6120 6872 6566 3d22 6874  px;"><a href="ht
+000043a0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+000043b0: 2e31 3032 332f 413a 3130 3236 3534 3339  .1023/A:10265439
+000043c0: 3030 3035 3422 3e52 7562 6e65 7220 6574  00054">Rubner et
+000043d0: 2061 6c2e 2028 3230 3030 293c 2f61 3e3c   al. (2000)</a><
+000043e0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+000043f0: 7472 3e0a 2020 2020 3c74 6420 7374 796c  tr>.    <td styl
+00004400: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00004410: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00004420: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00004430: 6164 6469 6e67 3a20 3870 783b 223e 553c  adding: 8px;">U<
+00004440: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00004450: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004460: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004470: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004480: 7061 6464 696e 673a 2038 7078 3b22 3e4e  padding: 8px;">N
+00004490: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+000044a0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+000044b0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+000044c0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+000044d0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+000044e0: 4865 6c6c 696e 6765 7220 6469 7374 616e  Hellinger distan
+000044f0: 6365 3c2f 7464 3e0a 2020 2020 3c74 6420  ce</td>.    <td 
+00004500: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00004510: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00004520: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00004530: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00004540: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00004550: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3135  ://doi.org/10.15
+00004560: 3135 2f43 524c 4c2e 3139 3039 2e31 3336  15/CRLL.1909.136
+00004570: 2e32 3130 223e 4865 6c6c 696e 6765 7220  .210">Hellinger 
+00004580: 2831 3930 3929 3c2f 613e 3c2f 7464 3e0a  (1909)</a></td>.
+00004590: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
+000045a0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+000045b0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000045c0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000045d0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+000045e0: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
+000045f0: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00004600: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004610: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00004620: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004630: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
+00004640: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00004650: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00004660: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00004670: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00004680: 696e 673a 2038 7078 3b22 3e48 6973 746f  ing: 8px;">Histo
+00004690: 6772 616d 2069 6e74 6572 7365 6374 696f  gram intersectio
+000046a0: 6e20 6e6f 726d 616c 697a 6564 2063 6f6d  n normalized com
+000046b0: 706c 656d 656e 743c 2f74 643e 0a20 2020  plement</td>.   
+000046c0: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+000046d0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+000046e0: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+000046f0: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00004700: 2038 7078 3b22 3e3c 6120 6872 6566 3d22   8px;"><a href="
+00004710: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00004720: 3130 2e31 3030 372f 4246 3030 3133 3034  10.1007/BF001304
+00004730: 3837 223e 5377 6169 6e20 616e 6420 4261  87">Swain and Ba
+00004740: 6c6c 6172 6420 2831 3939 3129 3c2f 613e  llard (1991)</a>
+00004750: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 2020  </td>.  </tr>.  
+00004760: 3c74 723e 0a20 2020 203c 7464 2073 7479  <tr>.    <td sty
+00004770: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004780: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004790: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+000047a0: 7061 6464 696e 673a 2038 7078 3b22 3e55  padding: 8px;">U
+000047b0: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+000047c0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+000047d0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+000047e0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+000047f0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004800: 4e3c 2f74 643e 0a20 2020 203c 7464 2073  N</td>.    <td s
+00004810: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00004820: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00004830: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00004840: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+00004850: 3e4a 656e 7365 6e2d 5368 616e 6e6f 6e20  >Jensen-Shannon 
+00004860: 6469 7374 616e 6365 3c2f 7464 3e0a 2020  distance</td>.  
+00004870: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004880: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004890: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000048a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000048b0: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+000048c0: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+000048d0: 2f31 302e 3131 3039 2f31 382e 3631 3131  /10.1109/18.6111
+000048e0: 3522 3e4c 696e 2028 3139 3931 293c 2f61  5">Lin (1991)</a
+000048f0: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+00004900: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
+00004910: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00004920: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00004930: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00004940: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00004950: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00004960: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00004970: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00004980: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+00004990: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+000049a0: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+000049b0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000049c0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000049d0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000049e0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+000049f0: 223e 4b75 6c6c 6261 636b 2d4c 6569 626c  ">Kullback-Leibl
+00004a00: 6572 2064 6976 6572 6765 6e63 653c 2f74  er divergence</t
+00004a10: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00004a20: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00004a30: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00004a40: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00004a50: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
+00004a60: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+00004a70: 692e 6f72 672f 3130 2e31 3231 342f 616f  i.org/10.1214/ao
+00004a80: 6d73 2f31 3137 3737 3239 3639 3422 3e4b  ms/1177729694">K
+00004a90: 756c 6c62 6163 6b20 616e 6420 4c65 6962  ullback and Leib
+00004aa0: 6c65 7220 2831 3935 3129 3c2f 613e 3c2f  ler (1951)</a></
+00004ab0: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00004ac0: 723e 0a20 2020 203c 7464 2073 7479 6c65  r>.    <td style
+00004ad0: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00004ae0: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00004af0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00004b00: 6464 696e 673a 2038 7078 3b22 3e4d 3c2f  dding: 8px;">M</
+00004b10: 7464 3e0a 2020 2020 3c74 6420 7374 796c  td>.    <td styl
+00004b20: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+00004b30: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+00004b40: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00004b50: 6164 6469 6e67 3a20 3870 783b 223e 4e3c  adding: 8px;">N<
+00004b60: 2f74 643e 0a20 2020 203c 7464 2073 7479  /td>.    <td sty
+00004b70: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004b80: 6365 6e74 6572 3b20 626f 7264 6572 3a20  center; border: 
+00004b90: 3170 7820 736f 6c69 6420 6772 6579 3b20  1px solid grey; 
+00004ba0: 7061 6464 696e 673a 2038 7078 3b22 3e4d  padding: 8px;">M
+00004bb0: 4d44 3c2f 7464 3e0a 2020 2020 3c74 6420  MD</td>.    <td 
+00004bc0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00004bd0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+00004be0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00004bf0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00004c00: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00004c10: 3a2f 2f64 6c2e 6163 6d2e 6f72 672f 646f  ://dl.acm.org/do
+00004c20: 692f 3130 2e35 3535 352f 3231 3838 3338  i/10.5555/218838
+00004c30: 352e 3231 3838 3431 3022 3e47 7265 7474  5.2188410">Grett
+00004c40: 6f6e 2065 7420 616c 2e20 2832 3031 3229  on et al. (2012)
+00004c50: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
+00004c60: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
+00004c70: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00004c80: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00004c90: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00004ca0: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00004cb0: 3b22 3e55 3c2f 7464 3e0a 2020 2020 3c74  ;">U</td>.    <t
+00004cc0: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00004cd0: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00004ce0: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+00004cf0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+00004d00: 783b 223e 4e3c 2f74 643e 0a20 2020 203c  x;">N</td>.    <
+00004d10: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00004d20: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+00004d30: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+00004d40: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+00004d50: 7078 3b22 3e50 5349 3c2f 7464 3e0a 2020  px;">PSI</td>.  
+00004d60: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00004d70: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00004d80: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00004d90: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00004da0: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00004db0: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00004dc0: 2f31 302e 3130 3537 2f6a 6f72 732e 3230  /10.1057/jors.20
+00004dd0: 3038 2e31 3434 223e 5775 2061 6e64 204f  08.144">Wu and O
+00004de0: 6c73 6f6e 2028 3230 3130 293c 2f61 3e3c  lson (2010)</a><
+00004df0: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00004e00: 7472 3e0a 2020 2020 3c74 6420 726f 7773  tr>.    <td rows
+00004e10: 7061 6e3d 2235 2220 7374 796c 653d 2274  pan="5" style="t
+00004e20: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004e30: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00004e40: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004e50: 6e67 3a20 3870 783b 223e 5374 6174 6973  ng: 8px;">Statis
+00004e60: 7469 6361 6c20 7465 7374 3c2f 7464 3e0a  tical test</td>.
+00004e70: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00004e80: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00004e90: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00004ea0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00004eb0: 6e67 3a20 3870 783b 223e 553c 2f74 643e  ng: 8px;">U</td>
+00004ec0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00004ed0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00004ee0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00004ef0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00004f00: 696e 673a 2038 7078 3b22 3e43 3c2f 7464  ing: 8px;">C</td
+00004f10: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+00004f20: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00004f30: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00004f40: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00004f50: 6469 6e67 3a20 3870 783b 223e 4368 692d  ding: 8px;">Chi-
+00004f60: 7371 7561 7265 2074 6573 743c 2f74 643e  square test</td>
+00004f70: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00004f80: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00004f90: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00004fa0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00004fb0: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
+00004fc0: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
+00004fd0: 6f72 672f 3130 2e31 3038 302f 3134 3738  org/10.1080/1478
+00004fe0: 3634 3430 3030 3934 3633 3839 3722 3e50  6440009463897">P
+00004ff0: 6561 7273 6f6e 2028 3139 3030 293c 2f61  earson (1900)</a
+00005000: 3e3c 2f74 643e 0a20 203c 2f74 723e 0a20  ></td>.  </tr>. 
+00005010: 203c 7472 3e0a 2020 2020 3c74 6420 7374   <tr>.    <td st
+00005020: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00005030: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00005040: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00005050: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00005060: 553c 2f74 643e 0a20 2020 203c 7464 2073  U</td>.    <td s
+00005070: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00005080: 3a20 6365 6e74 6572 3b20 626f 7264 6572  : center; border
+00005090: 3a20 3170 7820 736f 6c69 6420 6772 6579  : 1px solid grey
+000050a0: 3b20 7061 6464 696e 673a 2038 7078 3b22  ; padding: 8px;"
+000050b0: 3e4e 3c2f 7464 3e0a 2020 2020 3c74 6420  >N</td>.    <td 
+000050c0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000050d0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000050e0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+000050f0: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00005100: 223e 4372 616d c3a9 722d 766f 6e20 4d69  ">Cram..r-von Mi
+00005110: 7365 7320 7465 7374 3c2f 7464 3e0a 2020  ses test</td>.  
+00005120: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00005130: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00005140: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+00005150: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+00005160: 3a20 3870 783b 223e 3c61 2068 7265 663d  : 8px;"><a href=
+00005170: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00005180: 2f31 302e 3130 3830 2f30 3334 3631 3233  /10.1080/0346123
+00005190: 382e 3139 3238 2e31 3034 3136 3836 3222  8.1928.10416862"
+000051a0: 3e43 7261 6dc3 a972 2028 3139 3032 293c  >Cram..r (1902)<
+000051b0: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
+000051c0: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
+000051d0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000051e0: 6e3a 2063 656e 7465 723b 2062 6f72 6465  n: center; borde
+000051f0: 723a 2031 7078 2073 6f6c 6964 2067 7265  r: 1px solid gre
+00005200: 793b 2070 6164 6469 6e67 3a20 3870 783b  y; padding: 8px;
+00005210: 223e 553c 2f74 643e 0a20 2020 203c 7464  ">U</td>.    <td
+00005220: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
+00005230: 676e 3a20 6365 6e74 6572 3b20 626f 7264  gn: center; bord
+00005240: 6572 3a20 3170 7820 736f 6c69 6420 6772  er: 1px solid gr
+00005250: 6579 3b20 7061 6464 696e 673a 2038 7078  ey; padding: 8px
+00005260: 3b22 3e4e 3c2f 7464 3e0a 2020 2020 3c74  ;">N</td>.    <t
+00005270: 6420 7374 796c 653d 2274 6578 742d 616c  d style="text-al
+00005280: 6967 6e3a 2063 656e 7465 723b 2062 6f72  ign: center; bor
+00005290: 6465 723a 2031 7078 2073 6f6c 6964 2067  der: 1px solid g
+000052a0: 7265 793b 2070 6164 6469 6e67 3a20 3870  rey; padding: 8p
+000052b0: 783b 223e 4b6f 6c6d 6f67 6f72 6f76 2d53  x;">Kolmogorov-S
+000052c0: 6d69 726e 6f76 2074 6573 743c 2f74 643e  mirnov test</td>
+000052d0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+000052e0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000052f0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00005300: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00005310: 696e 673a 2038 7078 3b22 3e3c 6120 6872  ing: 8px;"><a hr
+00005320: 6566 3d22 6874 7470 733a 2f2f 646f 692e  ef="https://doi.
+00005330: 6f72 672f 3130 2e32 3330 372f 3232 3830  org/10.2307/2280
+00005340: 3039 3522 3e4d 6173 7365 7920 4a72 2028  095">Massey Jr (
+00005350: 3139 3531 293c 2f61 3e3c 2f74 643e 0a20  1951)</a></td>. 
+00005360: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
+00005370: 2020 3c74 6420 7374 796c 653d 2274 6578    <td style="tex
+00005380: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00005390: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+000053a0: 6964 2067 7265 793b 2070 6164 6469 6e67  id grey; padding
+000053b0: 3a20 3870 783b 223e 553c 2f74 643e 0a20  : 8px;">U</td>. 
+000053c0: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+000053d0: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+000053e0: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+000053f0: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00005400: 673a 2038 7078 3b22 3e4e 3c2f 7464 3e0a  g: 8px;">N</td>.
+00005410: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00005420: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00005430: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+00005440: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+00005450: 6e67 3a20 3870 783b 223e 4d61 6e6e 2d57  ng: 8px;">Mann-W
+00005460: 6869 746e 6579 2055 2074 6573 743c 2f74  hitney U test</t
+00005470: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00005480: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00005490: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+000054a0: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+000054b0: 6464 696e 673a 2038 7078 3b22 3e3c 6120  dding: 8px;"><a 
+000054c0: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+000054d0: 692e 6f72 672f 3130 2e31 3231 342f 616f  i.org/10.1214/ao
+000054e0: 6d73 2f31 3137 3737 3330 3439 3122 3e4d  ms/1177730491">M
+000054f0: 616e 6e20 616e 6420 5768 6974 6e65 7920  ann and Whitney 
+00005500: 2831 3934 3729 3c2f 613e 3c2f 7464 3e0a  (1947)</a></td>.
+00005510: 2020 3c2f 7472 3e0a 2020 3c74 723e 0a20    </tr>.  <tr>. 
+00005520: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00005530: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00005540: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00005550: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00005560: 673a 2038 7078 3b22 3e55 3c2f 7464 3e0a  g: 8px;">U</td>.
+00005570: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00005580: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00005590: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000055a0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000055b0: 6e67 3a20 3870 783b 223e 4e3c 2f74 643e  ng: 8px;">N</td>
+000055c0: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+000055d0: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000055e0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+000055f0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00005600: 696e 673a 2038 7078 3b22 3e57 656c 6368  ing: 8px;">Welch
+00005610: 2773 2074 2d74 6573 743c 2f74 643e 0a20  's t-test</td>. 
+00005620: 2020 203c 7464 2073 7479 6c65 3d22 7465     <td style="te
+00005630: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00005640: 3b20 626f 7264 6572 3a20 3170 7820 736f  ; border: 1px so
+00005650: 6c69 6420 6772 6579 3b20 7061 6464 696e  lid grey; paddin
+00005660: 673a 2038 7078 3b22 3e3c 6120 6872 6566  g: 8px;"><a href
+00005670: 3d22 6874 7470 733a 2f2f 646f 692e 6f72  ="https://doi.or
+00005680: 672f 3130 2e32 3330 372f 3233 3332 3531  g/10.2307/233251
+00005690: 3022 3e57 656c 6368 2028 3139 3437 293c  0">Welch (1947)<
+000056a0: 2f61 3e3c 2f74 643e 0a20 203c 2f74 723e  /a></td>.  </tr>
+000056b0: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
+000056c0: 726f 7773 7061 6e3d 2232 2220 7374 796c  rowspan="2" styl
+000056d0: 653d 2274 6578 742d 616c 6967 6e3a 2063  e="text-align: c
+000056e0: 656e 7465 723b 2062 6f72 6465 723a 2031  enter; border: 1
+000056f0: 7078 2073 6f6c 6964 2067 7265 793b 2070  px solid grey; p
+00005700: 6164 6469 6e67 3a20 3870 783b 223e 5374  adding: 8px;">St
+00005710: 7265 616d 696e 673c 2f74 643e 0a20 2020  reaming</td>.   
+00005720: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00005730: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00005740: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00005750: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00005760: 2038 7078 3b22 3e44 6973 7461 6e63 6520   8px;">Distance 
+00005770: 6261 7365 643c 2f74 643e 0a20 2020 203c  based</td>.    <
+00005780: 7464 2073 7479 6c65 3d22 7465 7874 2d61  td style="text-a
+00005790: 6c69 676e 3a20 6365 6e74 6572 3b20 626f  lign: center; bo
+000057a0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+000057b0: 6772 6579 3b20 7061 6464 696e 673a 2038  grey; padding: 8
+000057c0: 7078 3b22 3e4d 3c2f 7464 3e0a 2020 2020  px;">M</td>.    
+000057d0: 3c74 6420 7374 796c 653d 2274 6578 742d  <td style="text-
+000057e0: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+000057f0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+00005800: 2067 7265 793b 2070 6164 6469 6e67 3a20   grey; padding: 
+00005810: 3870 783b 223e 4e3c 2f74 643e 0a20 2020  8px;">N</td>.   
+00005820: 203c 7464 2073 7479 6c65 3d22 7465 7874   <td style="text
+00005830: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
+00005840: 626f 7264 6572 3a20 3170 7820 736f 6c69  border: 1px soli
+00005850: 6420 6772 6579 3b20 7061 6464 696e 673a  d grey; padding:
+00005860: 2038 7078 3b22 3e4d 4d44 3c2f 7464 3e0a   8px;">MMD</td>.
+00005870: 2020 2020 3c74 6420 7374 796c 653d 2274      <td style="t
+00005880: 6578 742d 616c 6967 6e3a 2063 656e 7465  ext-align: cente
+00005890: 723b 2062 6f72 6465 723a 2031 7078 2073  r; border: 1px s
+000058a0: 6f6c 6964 2067 7265 793b 2070 6164 6469  olid grey; paddi
+000058b0: 6e67 3a20 3870 783b 223e 3c61 2068 7265  ng: 8px;"><a hre
+000058c0: 663d 2268 7474 7073 3a2f 2f64 6c2e 6163  f="https://dl.ac
+000058d0: 6d2e 6f72 672f 646f 692f 3130 2e35 3535  m.org/doi/10.555
+000058e0: 352f 3231 3838 3338 352e 3231 3838 3431  5/2188385.218841
+000058f0: 3022 3e47 7265 7474 6f6e 2065 7420 616c  0">Gretton et al
+00005900: 2e20 2832 3031 3229 3c2f 613e 3c2f 7464  . (2012)</a></td
+00005910: 3e0a 2020 3c2f 7472 3e0a 2020 3c74 723e  >.  </tr>.  <tr>
+00005920: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00005930: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00005940: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+00005950: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+00005960: 696e 673a 2038 7078 3b22 3e53 7461 7469  ing: 8px;">Stati
+00005970: 7374 6963 616c 2074 6573 743c 2f74 643e  stical test</td>
+00005980: 0a20 2020 203c 7464 2073 7479 6c65 3d22  .    <td style="
+00005990: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+000059a0: 6572 3b20 626f 7264 6572 3a20 3170 7820  er; border: 1px 
+000059b0: 736f 6c69 6420 6772 6579 3b20 7061 6464  solid grey; padd
+000059c0: 696e 673a 2038 7078 3b22 3e55 3c2f 7464  ing: 8px;">U</td
+000059d0: 3e0a 2020 2020 3c74 6420 7374 796c 653d  >.    <td style=
+000059e0: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+000059f0: 7465 723b 2062 6f72 6465 723a 2031 7078  ter; border: 1px
+00005a00: 2073 6f6c 6964 2067 7265 793b 2070 6164   solid grey; pad
+00005a10: 6469 6e67 3a20 3870 783b 223e 4e3c 2f74  ding: 8px;">N</t
+00005a20: 643e 0a20 2020 203c 7464 2073 7479 6c65  d>.    <td style
+00005a30: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00005a40: 6e74 6572 3b20 626f 7264 6572 3a20 3170  nter; border: 1p
+00005a50: 7820 736f 6c69 6420 6772 6579 3b20 7061  x solid grey; pa
+00005a60: 6464 696e 673a 2038 7078 3b22 3e49 6e63  dding: 8px;">Inc
+00005a70: 7265 6d65 6e74 616c 204b 6f6c 6d6f 676f  remental Kolmogo
+00005a80: 726f 762d 536d 6972 6e6f 7620 7465 7374  rov-Smirnov test
+00005a90: 3c2f 7464 3e0a 2020 2020 3c74 6420 7374  </td>.    <td st
+00005aa0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00005ab0: 2063 656e 7465 723b 2062 6f72 6465 723a   center; border:
+00005ac0: 2031 7078 2073 6f6c 6964 2067 7265 793b   1px solid grey;
+00005ad0: 2070 6164 6469 6e67 3a20 3870 783b 223e   padding: 8px;">
+00005ae0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00005af0: 2f64 6f69 2e6f 7267 2f31 302e 3131 3435  /doi.org/10.1145
+00005b00: 2f32 3933 3936 3732 2e32 3933 3938 3336  /2939672.2939836
+00005b10: 223e 646f 7320 5265 6973 2065 7420 616c  ">dos Reis et al
+00005b20: 2e20 2832 3031 3629 3c2f 613e 3c2f 7464  . (2016)</a></td
+00005b30: 3e0a 2020 3c2f 7472 3e0a 3c2f 7462 6f64  >.  </tr>.</tbod
+00005b40: 793e 0a3c 2f74 6162 6c65 3e0a 0a23 2320  y>.</table>..## 
+00005b50: e29d 9720 5768 6174 2069 7320 616e 6420  ... What is and 
+00005b60: 7768 6174 2069 7320 6e6f 7420 4672 6f75  what is not Frou
+00005b70: 726f 733f 0a0a 556e 6c69 6b65 206f 7468  ros?..Unlike oth
+00005b80: 6572 206c 6962 7261 7269 6573 2074 6861  er libraries tha
+00005b90: 7420 696e 2061 6464 6974 696f 6e20 746f  t in addition to
+00005ba0: 2070 726f 7669 6465 2064 7269 6674 2064   provide drift d
+00005bb0: 6574 6563 7469 6f6e 2061 6c67 6f72 6974  etection algorit
+00005bc0: 686d 732c 2069 6e63 6c75 6465 206f 7468  hms, include oth
+00005bd0: 6572 2066 756e 6374 696f 6e61 6c69 7469  er functionaliti
+00005be0: 6573 2073 7563 6820 6173 2061 6e6f 6d61  es such as anoma
+00005bf0: 6c79 2f6f 7574 6c69 6572 2064 6574 6563  ly/outlier detec
+00005c00: 7469 6f6e 2c20 6164 7665 7273 6172 6961  tion, adversaria
+00005c10: 6c20 6465 7465 6374 696f 6e2c 2069 6d62  l detection, imb
+00005c20: 616c 616e 6365 206c 6561 726e 696e 672c  alance learning,
+00005c30: 2061 6d6f 6e67 206f 7468 6572 732c 2046   among others, F
+00005c40: 726f 7572 6f73 2068 6173 2061 6e64 2077  rouros has and w
+00005c50: 696c 6c20 2a2a 4f4e 4c59 2a2a 2068 6176  ill **ONLY** hav
+00005c60: 6520 6f6e 6520 7075 7270 6f73 653a 202a  e one purpose: *
+00005c70: 2a64 7269 6674 2064 6574 6563 7469 6f6e  *drift detection
+00005c80: 2a2a 2e0a 0a57 6520 6669 726d 6c79 2062  **...We firmly b
+00005c90: 656c 6965 7665 2074 6861 7420 6d61 6368  elieve that mach
+00005ca0: 696e 6520 6c65 6172 6e69 6e67 2072 656c  ine learning rel
+00005cb0: 6174 6564 206c 6962 7261 7269 6573 206f  ated libraries o
+00005cc0: 7220 6672 616d 6577 6f72 6b73 2073 686f  r frameworks sho
+00005cd0: 756c 6420 6e6f 7420 666f 6c6c 6f77 205b  uld not follow [
+00005ce0: 4a61 636b 206f 6620 616c 6c20 7472 6164  Jack of all trad
+00005cf0: 6573 2c20 6d61 7374 6572 206f 6620 6e6f  es, master of no
+00005d00: 6e65 5d28 6874 7470 733a 2f2f 656e 2e77  ne](https://en.w
+00005d10: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00005d20: 692f 4a61 636b 5f6f 665f 616c 6c5f 7472  i/Jack_of_all_tr
+00005d30: 6164 6573 2c5f 6d61 7374 6572 5f6f 665f  ades,_master_of_
+00005d40: 6e6f 6e65 2920 7072 696e 6369 706c 652e  none) principle.
+00005d50: 2049 6e73 7465 6164 2c20 7468 6579 2073   Instead, they s
+00005d60: 686f 756c 6420 6265 2066 6f63 7573 6564  hould be focused
+00005d70: 206f 6e20 6120 7369 6e67 6c65 2074 6173   on a single tas
+00005d80: 6b20 616e 6420 646f 2069 7420 7765 6c6c  k and do it well
+00005d90: 2e0a 0a23 2320 e29c 8520 5768 6f20 6973  ...## ... Who is
+00005da0: 2075 7369 6e67 2046 726f 7572 6f73 3f0a   using Frouros?.
+00005db0: 0a46 726f 7572 6f73 2069 7320 6163 7469  .Frouros is acti
+00005dc0: 7665 6c79 2062 6569 6e67 2075 7365 6420  vely being used 
+00005dd0: 6279 2074 6865 2066 6f6c 6c6f 7769 6e67  by the following
+00005de0: 2070 726f 6a65 6374 7320 746f 2069 6d70   projects to imp
+00005df0: 6c65 6d65 6e74 2064 7269 6674 0a64 6574  lement drift.det
+00005e00: 6563 7469 6f6e 2069 6e20 6d61 6368 696e  ection in machin
+00005e10: 6520 6c65 6172 6e69 6e67 2070 6970 656c  e learning pipel
+00005e20: 696e 6573 3a0a 0a20 2a20 5b41 4934 454f  ines:.. * [AI4EO
+00005e30: 5343 5d28 6874 7470 733a 2f2f 6169 3465  SC](https://ai4e
+00005e40: 6f73 632e 6575 292e 0a20 2a20 5b69 4d61  osc.eu).. * [iMa
+00005e50: 6769 6e65 5d28 6874 7470 733a 2f2f 696d  gine](https://im
+00005e60: 6167 696e 652d 6169 2e65 7529 2e0a 0a49  agine-ai.eu)...I
+00005e70: 6620 796f 7520 7761 6e74 2079 6f75 7220  f you want your 
+00005e80: 7072 6f6a 6563 7420 6c69 7374 6564 2068  project listed h
+00005e90: 6572 652c 2064 6f20 6e6f 7420 6865 7369  ere, do not hesi
+00005ea0: 7461 7465 2074 6f20 7365 6e64 2075 7320  tate to send us 
+00005eb0: 6120 7075 6c6c 2072 6571 7565 7374 2e0a  a pull request..
+00005ec0: 0a23 2320 f09f 918d 2043 6f6e 7472 6962  .## .... Contrib
+00005ed0: 7574 696e 670a 0a43 6865 636b 206f 7574  uting..Check out
+00005ee0: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
+00005ef0: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
+00005f00: 7562 2e63 6f6d 2f49 4643 412f 6672 6f75  ub.com/IFCA/frou
+00005f10: 726f 732f 626c 6f62 2f6d 6169 6e2f 434f  ros/blob/main/CO
+00005f20: 4e54 5249 4255 5449 4e47 2e6d 6429 2073  NTRIBUTING.md) s
+00005f30: 6563 7469 6f6e 2e0a 0a23 2320 f09f 92ac  ection...## ....
+00005f40: 2043 6974 6174 696f 6e0a 0a41 6c74 686f   Citation..Altho
+00005f50: 7567 6820 4672 6f75 726f 7320 7061 7065  ugh Frouros pape
+00005f60: 7220 6973 2073 7469 6c6c 2069 6e20 7072  r is still in pr
+00005f70: 6570 7269 6e74 2c20 6966 2079 6f75 2077  eprint, if you w
+00005f80: 616e 7420 746f 2063 6974 6520 6974 2079  ant to cite it y
+00005f90: 6f75 2063 616e 2075 7365 2074 6865 205b  ou can use the [
+00005fa0: 7072 6570 7269 6e74 5d28 6874 7470 733a  preprint](https:
+00005fb0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00005fc0: 3232 3038 2e30 3638 3638 2920 7665 7273  2208.06868) vers
+00005fd0: 696f 6e20 2874 6f20 6265 2072 6570 6c61  ion (to be repla
+00005fe0: 6365 6420 6279 2074 6865 2070 6170 6572  ced by the paper
+00005ff0: 206f 6e63 6520 6973 2070 7562 6c69 7368   once is publish
+00006000: 6564 292e 0a0a 6060 6062 6962 7465 780a  ed)...```bibtex.
+00006010: 4061 7274 6963 6c65 7b63 6573 7065 6465  @article{cespede
+00006020: 7332 3032 3266 726f 7572 6f73 2c0a 2020  s2022frouros,.  
+00006030: 7469 746c 653d 7b46 726f 7572 6f73 3a20  title={Frouros: 
+00006040: 4120 5079 7468 6f6e 206c 6962 7261 7279  A Python library
+00006050: 2066 6f72 2064 7269 6674 2064 6574 6563   for drift detec
+00006060: 7469 6f6e 2069 6e20 6d61 6368 696e 6520  tion in machine 
+00006070: 6c65 6172 6e69 6e67 2073 7973 7465 6d73  learning systems
+00006080: 7d2c 0a20 2061 7574 686f 723d 7b43 7b5c  },.  author={C{\
+00006090: 2765 7d73 7065 6465 732d 5369 736e 6965  'e}spedes-Sisnie
+000060a0: 6761 2c20 4a61 696d 6520 616e 6420 4c7b  ga, Jaime and L{
+000060b0: 5c27 6f7d 7065 7a2d 4761 7263 7b5c 275c  \'o}pez-Garc{\'\
+000060c0: 697d 612c 207b 5c27 417d 6c76 6172 6f20  i}a, {\'A}lvaro 
+000060d0: 7d2c 0a20 206a 6f75 726e 616c 3d7b 6172  },.  journal={ar
+000060e0: 5869 7620 7072 6570 7269 6e74 2061 7258  Xiv preprint arX
+000060f0: 6976 3a32 3230 382e 3036 3836 387d 2c0a  iv:2208.06868},.
+00006100: 2020 7965 6172 3d7b 3230 3232 7d0a 7d0a    year={2022}.}.
+00006110: 6060 600a 0a23 2320 f09f 939d 204c 6963  ```..## .... Lic
+00006120: 656e 7365 0a0a 4672 6f75 726f 7320 6973  ense..Frouros is
+00006130: 2061 6e20 6f70 656e 2d73 6f75 7263 6520   an open-source 
+00006140: 736f 6674 7761 7265 206c 6963 656e 7365  software license
+00006150: 6420 756e 6465 7220 7468 6520 5b42 5344  d under the [BSD
+00006160: 2d33 2d43 6c61 7573 6520 6c69 6365 6e73  -3-Clause licens
+00006170: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00006180: 622e 636f 6d2f 4946 4341 2f66 726f 7572  b.com/IFCA/frour
+00006190: 6f73 2f62 6c6f 622f 6d61 696e 2f4c 4943  os/blob/main/LIC
+000061a0: 454e 5345 292e 0a0a 2323 20f0 9f99 8f20  ENSE)...## .... 
+000061b0: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
+000061c0: 0a0a 4672 6f75 726f 7320 6861 7320 7265  ..Frouros has re
+000061d0: 6365 6976 6564 2066 756e 6469 6e67 2066  ceived funding f
+000061e0: 726f 6d20 7468 6520 4167 656e 6369 6120  rom the Agencia 
+000061f0: 4573 7461 7461 6c20 6465 2049 6e76 6573  Estatal de Inves
+00006200: 7469 6761 6369 c3b3 6e2c 2055 6e69 6461  tigaci..n, Unida
+00006210: 6420 6465 2045 7863 656c 656e 6369 6120  d de Excelencia 
+00006220: 4d61 72c3 ad61 2064 6520 4d61 657a 7475  Mar..a de Maeztu
+00006230: 2c20 7265 662e 204d 444d 2d32 3031 372d  , ref. MDM-2017-
+00006240: 3037 3635 2e0a 0a0a                      0765....
```

### Comparing `frouros-0.5.1/frouros.egg-info/SOURCES.txt` & `frouros-0.6.0/frouros.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,14 @@
 frouros/callbacks/batch/__init__.py
 frouros/callbacks/batch/base.py
 frouros/callbacks/batch/permutation_test.py
 frouros/callbacks/batch/reset.py
 frouros/callbacks/streaming/__init__.py
 frouros/callbacks/streaming/base.py
 frouros/callbacks/streaming/history.py
-frouros/callbacks/streaming/msprt.py
-frouros/callbacks/streaming/warning_samples.py
-frouros/common/__init__.py
-frouros/common/exceptions.py
 frouros/datasets/__init__.py
 frouros/datasets/base.py
 frouros/datasets/exceptions.py
 frouros/datasets/real.py
 frouros/datasets/synthetic.py
 frouros/detectors/__init__.py
 frouros/detectors/base.py
```

### Comparing `frouros-0.5.1/pyproject.toml` & `frouros-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.5.1"
+version = "0.6.0"
 description = "An open-source Python library for drift detection in machine learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
@@ -41,25 +41,25 @@
     "requests>=2.31.0,<2.32",
     "scipy>=1.10.0,<1.11",
     "tqdm>=4.65,<5",
 ]
 
 [project.optional-dependencies]
 docs = [
-    "sphinx>=5.3.0,<7.1",
+    "sphinx>=5.3.0,<7.2",
     "sphinx-book-theme>=1.0.0,<1.1",
     "sphinxcontrib-bibtex>=2.5.0,<2.6",
     "myst-parser>=0.18.0,<2.1",
     "myst-nb>=0.17.0,<0.18",
 ]
 notebooks = [
     "scikit-learn>=1.2.0,<1.4",
     "torch>=1.13.0,<2.1",
     "torchvision>=0.14.0,<0.16",
-    "ipywidgets>=8.0.0,<8.1",
+    "ipywidgets>=8.0.0,<8.2",
 ]
 
 [project.urls]
 homepage = "https://frouros.readthedocs.io"
 repository = "https://github.com/IFCA/frouros"
 documentation = "https://frouros.readthedocs.io"
 download = "https://pypi.org/project/frouros/"
```

### Comparing `frouros-0.5.1/setup.py` & `frouros-0.6.0/setup.py`

 * *Files identical despite different names*

