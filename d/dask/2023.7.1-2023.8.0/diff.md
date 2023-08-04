# Comparing `tmp/dask-2023.7.1.tar.gz` & `tmp/dask-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-2023.7.1.tar", last modified: Thu Jul 20 21:06:45 2023, max compression
+gzip compressed data, was "dask-2023.8.0.tar", last modified: Fri Aug  4 18:09:12 2023, max compression
```

## Comparing `dask-2023.7.1.tar` & `dask-2023.8.0.tar`

### file list

```diff
@@ -1,487 +1,488 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:45.218559 dask-2023.7.1/
--rw-r--r--   0 james      (501) staff       (20)     1531 2022-10-24 20:44:15.000000 dask-2023.7.1/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      325 2022-11-09 22:20:24.000000 dask-2023.7.1/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     2532 2023-07-20 21:06:45.217983 dask-2023.7.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1291 2022-11-09 22:20:24.000000 dask-2023.7.1/README.rst
--rw-r--r--   0 james      (501) staff       (20)     2505 2023-07-20 20:35:59.000000 dask-2023.7.1/conftest.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:45.219183 dask-2023.7.1/dask/
--rw-r--r--   0 james      (501) staff       (20)      485 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      133 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/__main__.py
--rw-r--r--   0 james      (501) staff       (20)      643 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/_compatibility.py
--rw-r--r--   0 james      (501) staff       (20)      500 2023-07-20 21:06:45.219343 dask-2023.7.1/dask/_version.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.686655 dask-2023.7.1/dask/array/
--rw-r--r--   0 james      (501) staff       (20)     1543 2021-06-08 02:50:30.000000 dask-2023.7.1/dask/array/NUMPY_LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)     5413 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12600 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/backends.py
--rw-r--r--   0 james      (501) staff       (20)     9983 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/blockwise.py
--rw-r--r--   0 james      (501) staff       (20)    12304 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/chunk.py
--rw-r--r--   0 james      (501) staff       (20)     5066 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/chunk_types.py
--rw-r--r--   0 james      (501) staff       (20)   190831 2023-06-26 19:07:05.000000 dask-2023.7.1/dask/array/core.py
--rw-r--r--   0 james      (501) staff       (20)    40564 2023-05-03 18:02:08.000000 dask-2023.7.1/dask/array/creation.py
--rw-r--r--   0 james      (501) staff       (20)     2114 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/cupy_entry_point.py
--rw-r--r--   0 james      (501) staff       (20)      526 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/dispatch.py
--rw-r--r--   0 james      (501) staff       (20)     9146 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/array/einsumfuncs.py
--rw-r--r--   0 james      (501) staff       (20)     7252 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/fft.py
--rw-r--r--   0 james      (501) staff       (20)    32656 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/gufunc.py
--rw-r--r--   0 james      (501) staff       (20)     1996 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/image.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.691353 dask-2023.7.1/dask/array/lib/
--rw-r--r--   0 james      (501) staff       (20)       77 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/lib/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      101 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/lib/stride_tricks.py
--rw-r--r--   0 james      (501) staff       (20)    53335 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/linalg.py
--rw-r--r--   0 james      (501) staff       (20)     6363 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/ma.py
--rw-r--r--   0 james      (501) staff       (20)     5699 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/numpy_compat.py
--rw-r--r--   0 james      (501) staff       (20)    12838 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/optimization.py
--rw-r--r--   0 james      (501) staff       (20)    28480 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/overlap.py
--rw-r--r--   0 james      (501) staff       (20)    10652 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/percentile.py
--rw-r--r--   0 james      (501) staff       (20)    40604 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/random.py
--rw-r--r--   0 james      (501) staff       (20)    28324 2023-06-20 19:59:21.000000 dask-2023.7.1/dask/array/rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    57287 2023-06-01 20:02:33.000000 dask-2023.7.1/dask/array/reductions.py
--rw-r--r--   0 james      (501) staff       (20)    10765 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/reshape.py
--rw-r--r--   0 james      (501) staff       (20)    81977 2023-06-20 20:00:03.000000 dask-2023.7.1/dask/array/routines.py
--rw-r--r--   0 james      (501) staff       (20)    72631 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/slicing.py
--rw-r--r--   0 james      (501) staff       (20)    16184 2023-07-07 00:51:47.000000 dask-2023.7.1/dask/array/stats.py
--rw-r--r--   0 james      (501) staff       (20)     8048 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/svg.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.730127 dask-2023.7.1/dask/array/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.7.1/dask/array/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)   161461 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_array_core.py
--rw-r--r--   0 james      (501) staff       (20)     6689 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_array_function.py
--rw-r--r--   0 james      (501) staff       (20)     3159 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_array_utils.py
--rw-r--r--   0 james      (501) staff       (20)    23222 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_atop.py
--rw-r--r--   0 james      (501) staff       (20)     3304 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_chunk.py
--rw-r--r--   0 james      (501) staff       (20)    31150 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_creation.py
--rw-r--r--   0 james      (501) staff       (20)    19888 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_core.py
--rw-r--r--   0 james      (501) staff       (20)     6456 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_creation.py
--rw-r--r--   0 james      (501) staff       (20)      594 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_gufunc.py
--rw-r--r--   0 james      (501) staff       (20)    13412 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_linalg.py
--rw-r--r--   0 james      (501) staff       (20)     4303 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_overlap.py
--rw-r--r--   0 james      (501) staff       (20)     2862 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_percentile.py
--rw-r--r--   0 james      (501) staff       (20)     9219 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_random.py
--rw-r--r--   0 james      (501) staff       (20)     2224 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_reductions.py
--rw-r--r--   0 james      (501) staff       (20)     7437 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_routines.py
--rw-r--r--   0 james      (501) staff       (20)     4877 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_slicing.py
--rw-r--r--   0 james      (501) staff       (20)     2982 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_cupy_sparse.py
--rw-r--r--   0 james      (501) staff       (20)     8865 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_dispatch.py
--rw-r--r--   0 james      (501) staff       (20)     8437 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_fft.py
--rw-r--r--   0 james      (501) staff       (20)    21013 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_gufunc.py
--rw-r--r--   0 james      (501) staff       (20)     1482 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_image.py
--rw-r--r--   0 james      (501) staff       (20)    36448 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_linalg.py
--rw-r--r--   0 james      (501) staff       (20)    15635 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_masked.py
--rw-r--r--   0 james      (501) staff       (20)     1087 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_numpy_compat.py
--rw-r--r--   0 james      (501) staff       (20)    17446 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_optimization.py
--rw-r--r--   0 james      (501) staff       (20)    26718 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_overlap.py
--rw-r--r--   0 james      (501) staff       (20)     3443 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_percentiles.py
--rw-r--r--   0 james      (501) staff       (20)    15353 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_random.py
--rw-r--r--   0 james      (501) staff       (20)    36262 2023-06-20 19:59:21.000000 dask-2023.7.1/dask/array/tests/test_rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    32756 2023-06-01 20:02:33.000000 dask-2023.7.1/dask/array/tests/test_reductions.py
--rw-r--r--   0 james      (501) staff       (20)     7289 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_reshape.py
--rw-r--r--   0 james      (501) staff       (20)    83849 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_routines.py
--rw-r--r--   0 james      (501) staff       (20)    32302 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_slicing.py
--rw-r--r--   0 james      (501) staff       (20)     6592 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_sparse.py
--rw-r--r--   0 james      (501) staff       (20)     5489 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_stats.py
--rw-r--r--   0 james      (501) staff       (20)     2740 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_svg.py
--rw-r--r--   0 james      (501) staff       (20)      525 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_testing.py
--rw-r--r--   0 james      (501) staff       (20)    17390 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_ufunc.py
--rw-r--r--   0 james      (501) staff       (20)     2706 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_wrap.py
--rw-r--r--   0 james      (501) staff       (20)     1317 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tests/test_xarray.py
--rw-r--r--   0 james      (501) staff       (20)     4737 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/tiledb_io.py
--rw-r--r--   0 james      (501) staff       (20)     9943 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/ufunc.py
--rw-r--r--   0 james      (501) staff       (20)    18674 2023-06-26 19:11:47.000000 dask-2023.7.1/dask/array/utils.py
--rw-r--r--   0 james      (501) staff       (20)     6906 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/array/wrap.py
--rw-r--r--   0 james      (501) staff       (20)     4936 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/backends.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.734026 dask-2023.7.1/dask/bag/
--rw-r--r--   0 james      (501) staff       (20)      903 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     9111 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/avro.py
--rw-r--r--   0 james      (501) staff       (20)      763 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/chunk.py
--rw-r--r--   0 james      (501) staff       (20)    85425 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/bag/core.py
--rw-r--r--   0 james      (501) staff       (20)     5464 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/random.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.736400 dask-2023.7.1/dask/bag/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.7.1/dask/bag/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3808 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/tests/test_avro.py
--rw-r--r--   0 james      (501) staff       (20)    51087 2023-06-20 19:59:21.000000 dask-2023.7.1/dask/bag/tests/test_bag.py
--rw-r--r--   0 james      (501) staff       (20)     6528 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/tests/test_random.py
--rw-r--r--   0 james      (501) staff       (20)     5049 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/tests/test_text.py
--rw-r--r--   0 james      (501) staff       (20)     6765 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/text.py
--rw-r--r--   0 james      (501) staff       (20)      241 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bag/utils.py
--rw-r--r--   0 james      (501) staff       (20)    53616 2023-07-07 00:51:47.000000 dask-2023.7.1/dask/base.py
--rw-r--r--   0 james      (501) staff       (20)    53252 2023-05-19 15:53:47.000000 dask-2023.7.1/dask/blockwise.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.738081 dask-2023.7.1/dask/bytes/
--rw-r--r--   0 james      (501) staff       (20)       75 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bytes/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6933 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bytes/core.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.741555 dask-2023.7.1/dask/bytes/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.7.1/dask/bytes/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5158 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bytes/tests/test_bytes_utils.py
--rw-r--r--   0 james      (501) staff       (20)      530 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bytes/tests/test_compression.py
--rw-r--r--   0 james      (501) staff       (20)     6563 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/bytes/tests/test_http.py
--rw-r--r--   0 james      (501) staff       (20)    11476 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bytes/tests/test_local.py
--rw-r--r--   0 james      (501) staff       (20)    19385 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/bytes/tests/test_s3.py
--rw-r--r--   0 james      (501) staff       (20)      500 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/bytes/utils.py
--rw-r--r--   0 james      (501) staff       (20)     2001 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/cache.py
--rw-r--r--   0 james      (501) staff       (20)     4067 2022-10-24 20:44:15.000000 dask-2023.7.1/dask/callbacks.py
--rw-r--r--   0 james      (501) staff       (20)     3272 2023-07-07 00:51:47.000000 dask-2023.7.1/dask/cli.py
--rw-r--r--   0 james      (501) staff       (20)      523 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/compatibility.py
--rw-r--r--   0 james      (501) staff       (20)    21703 2023-06-20 19:59:21.000000 dask-2023.7.1/dask/config.py
--rw-r--r--   0 james      (501) staff       (20)     1756 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/context.py
--rw-r--r--   0 james      (501) staff       (20)    14833 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/core.py
--rw-r--r--   0 james      (501) staff       (20)     8060 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dask-schema.yaml
--rw-r--r--   0 james      (501) staff       (20)     2122 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dask.yaml
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.756948 dask-2023.7.1/dask/dataframe/
--rw-r--r--   0 james      (501) staff       (20)     1812 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7496 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/_compat.py
--rw-r--r--   0 james      (501) staff       (20)     2171 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/_dtypes.py
--rw-r--r--   0 james      (501) staff       (20)     3959 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/_pyarrow.py
--rw-r--r--   0 james      (501) staff       (20)     1936 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/_pyarrow_compat.py
--rw-r--r--   0 james      (501) staff       (20)    12101 2023-05-03 18:02:08.000000 dask-2023.7.1/dask/dataframe/accessor.py
--rw-r--r--   0 james      (501) staff       (20)    24817 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/dataframe/backends.py
--rw-r--r--   0 james      (501) staff       (20)     9507 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/categorical.py
--rw-r--r--   0 james      (501) staff       (20)   301737 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/core.py
--rw-r--r--   0 james      (501) staff       (20)     4609 2023-06-20 19:59:21.000000 dask-2023.7.1/dask/dataframe/dispatch.py
--rw-r--r--   0 james      (501) staff       (20)      552 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/extensions.py
--rw-r--r--   0 james      (501) staff       (20)   115448 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/groupby.py
--rw-r--r--   0 james      (501) staff       (20)     2463 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/hyperloglog.py
--rw-r--r--   0 james      (501) staff       (20)    13412 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/indexing.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.762985 dask-2023.7.1/dask/dataframe/io/
--rw-r--r--   0 james      (501) staff       (20)      706 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    33854 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/dataframe/io/csv.py
--rw-r--r--   0 james      (501) staff       (20)    17953 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/io/demo.py
--rw-r--r--   0 james      (501) staff       (20)    18275 2023-06-20 19:59:21.000000 dask-2023.7.1/dask/dataframe/io/hdf.py
--rw-r--r--   0 james      (501) staff       (20)    38599 2023-07-07 00:51:47.000000 dask-2023.7.1/dask/dataframe/io/io.py
--rw-r--r--   0 james      (501) staff       (20)    11163 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/json.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.764842 dask-2023.7.1/dask/dataframe/io/orc/
--rw-r--r--   0 james      (501) staff       (20)       92 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/orc/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     4487 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/orc/arrow.py
--rw-r--r--   0 james      (501) staff       (20)     7098 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/orc/core.py
--rw-r--r--   0 james      (501) staff       (20)      510 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/orc/utils.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.768170 dask-2023.7.1/dask/dataframe/io/parquet/
--rw-r--r--   0 james      (501) staff       (20)      166 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/parquet/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    71794 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/io/parquet/arrow.py
--rw-r--r--   0 james      (501) staff       (20)    67270 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/io/parquet/core.py
--rw-r--r--   0 james      (501) staff       (20)    52312 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/io/parquet/fastparquet.py
--rw-r--r--   0 james      (501) staff       (20)    32896 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/parquet/utils.py
--rw-r--r--   0 james      (501) staff       (20)    21108 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/sql.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.774199 dask-2023.7.1/dask/dataframe/io/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-03-07 20:03:52.000000 dask-2023.7.1/dask/dataframe/io/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    59293 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/dataframe/io/tests/test_csv.py
--rw-r--r--   0 james      (501) staff       (20)    11113 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/io/tests/test_demo.py
--rw-r--r--   0 james      (501) staff       (20)    27232 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/tests/test_hdf.py
--rw-r--r--   0 james      (501) staff       (20)    34779 2023-07-07 00:51:47.000000 dask-2023.7.1/dask/dataframe/io/tests/test_io.py
--rw-r--r--   0 james      (501) staff       (20)     8625 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/tests/test_json.py
--rw-r--r--   0 james      (501) staff       (20)     5238 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/tests/test_orc.py
--rw-r--r--   0 james      (501) staff       (20)   166740 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/io/tests/test_parquet.py
--rw-r--r--   0 james      (501) staff       (20)    17632 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/io/tests/test_sql.py
--rw-r--r--   0 james      (501) staff       (20)     8041 2023-06-20 19:59:21.000000 dask-2023.7.1/dask/dataframe/io/utils.py
--rw-r--r--   0 james      (501) staff       (20)    14071 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/dataframe/methods.py
--rw-r--r--   0 james      (501) staff       (20)    54050 2023-07-20 20:35:55.000000 dask-2023.7.1/dask/dataframe/multi.py
--rw-r--r--   0 james      (501) staff       (20)     1600 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/numeric.py
--rw-r--r--   0 james      (501) staff       (20)     8778 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/optimize.py
--rw-r--r--   0 james      (501) staff       (20)    20104 2023-07-07 00:51:47.000000 dask-2023.7.1/dask/dataframe/partitionquantiles.py
--rw-r--r--   0 james      (501) staff       (20)    11825 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/reshape.py
--rw-r--r--   0 james      (501) staff       (20)    22185 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/rolling.py
--rw-r--r--   0 james      (501) staff       (20)    38106 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/shuffle.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.791552 dask-2023.7.1/dask/dataframe/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.7.1/dask/dataframe/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    10633 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_accessors.py
--rw-r--r--   0 james      (501) staff       (20)    67628 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_arithmetics_reduction.py
--rw-r--r--   0 james      (501) staff       (20)      942 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_boolean.py
--rw-r--r--   0 james      (501) staff       (20)    16678 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_categorical.py
--rw-r--r--   0 james      (501) staff       (20)   194008 2023-07-20 20:35:55.000000 dask-2023.7.1/dask/dataframe/tests/test_dataframe.py
--rw-r--r--   0 james      (501) staff       (20)     1456 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_extensions.py
--rw-r--r--   0 james      (501) staff       (20)    14743 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_format.py
--rw-r--r--   0 james      (501) staff       (20)   121782 2023-07-20 20:35:55.000000 dask-2023.7.1/dask/dataframe/tests/test_groupby.py
--rw-r--r--   0 james      (501) staff       (20)     2702 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_hashing.py
--rw-r--r--   0 james      (501) staff       (20)     2897 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_hyperloglog.py
--rw-r--r--   0 james      (501) staff       (20)    22382 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_indexing.py
--rw-r--r--   0 james      (501) staff       (20)     7034 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_merge_column_and_index.py
--rw-r--r--   0 james      (501) staff       (20)      463 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_methods.py
--rw-r--r--   0 james      (501) staff       (20)    91084 2023-07-20 20:35:55.000000 dask-2023.7.1/dask/dataframe/tests/test_multi.py
--rw-r--r--   0 james      (501) staff       (20)     2120 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_numeric.py
--rw-r--r--   0 james      (501) staff       (20)     1067 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_optimize_dataframe.py
--rw-r--r--   0 james      (501) staff       (20)     6662 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_pyarrow.py
--rw-r--r--   0 james      (501) staff       (20)     4550 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_pyarrow_compat.py
--rw-r--r--   0 james      (501) staff       (20)    11571 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_reshape.py
--rw-r--r--   0 james      (501) staff       (20)    17510 2023-07-20 20:35:55.000000 dask-2023.7.1/dask/dataframe/tests/test_rolling.py
--rw-r--r--   0 james      (501) staff       (20)    54512 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/dataframe/tests/test_shuffle.py
--rw-r--r--   0 james      (501) staff       (20)    16595 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tests/test_ufunc.py
--rw-r--r--   0 james      (501) staff       (20)    22156 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/tests/test_utils_dataframe.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.792815 dask-2023.7.1/dask/dataframe/tseries/
--rw-r--r--   0 james      (501) staff       (20)        0 2021-06-08 02:50:30.000000 dask-2023.7.1/dask/dataframe/tseries/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7664 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tseries/resample.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.793993 dask-2023.7.1/dask/dataframe/tseries/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.7.1/dask/dataframe/tseries/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6866 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/dataframe/tseries/tests/test_resample.py
--rw-r--r--   0 james      (501) staff       (20)    27606 2023-07-20 20:35:59.000000 dask-2023.7.1/dask/dataframe/utils.py
--rw-r--r--   0 james      (501) staff       (20)     5314 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/datasets.py
--rw-r--r--   0 james      (501) staff       (20)    24389 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/delayed.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.796567 dask-2023.7.1/dask/diagnostics/
--rw-r--r--   0 james      (501) staff       (20)      258 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/diagnostics/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12136 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/diagnostics/profile.py
--rw-r--r--   0 james      (501) staff       (20)    16332 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/diagnostics/profile_visualize.py
--rw-r--r--   0 james      (501) staff       (20)     5001 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/diagnostics/progress.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.798034 dask-2023.7.1/dask/diagnostics/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.7.1/dask/diagnostics/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12045 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/diagnostics/tests/test_profiler.py
--rw-r--r--   0 james      (501) staff       (20)     3388 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/diagnostics/tests/test_progress.py
--rw-r--r--   0 james      (501) staff       (20)      715 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/distributed.py
--rw-r--r--   0 james      (501) staff       (20)    16587 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/dot.py
--rw-r--r--   0 james      (501) staff       (20)    19595 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/graph_manipulation.py
--rw-r--r--   0 james      (501) staff       (20)     2492 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/hashing.py
--rw-r--r--   0 james      (501) staff       (20)    34778 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/highlevelgraph.py
--rw-r--r--   0 james      (501) staff       (20)    46007 2023-05-03 18:02:08.000000 dask-2023.7.1/dask/layers.py
--rw-r--r--   0 james      (501) staff       (20)    18888 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/local.py
--rw-r--r--   0 james      (501) staff       (20)      487 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/ml.py
--rw-r--r--   0 james      (501) staff       (20)     8466 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/multiprocessing.py
--rw-r--r--   0 james      (501) staff       (20)    35638 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/optimization.py
--rw-r--r--   0 james      (501) staff       (20)    45768 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/order.py
--rw-r--r--   0 james      (501) staff       (20)        0 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/py.typed
--rw-r--r--   0 james      (501) staff       (20)    12597 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/rewrite.py
--rw-r--r--   0 james      (501) staff       (20)     7298 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/sizeof.py
--rw-r--r--   0 james      (501) staff       (20)     1510 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/system.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.820755 dask-2023.7.1/dask/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-03-07 20:04:31.000000 dask-2023.7.1/dask/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      742 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_backends.py
--rw-r--r--   0 james      (501) staff       (20)    51124 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_base.py
--rw-r--r--   0 james      (501) staff       (20)     1613 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_cache.py
--rw-r--r--   0 james      (501) staff       (20)     2570 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_callbacks.py
--rw-r--r--   0 james      (501) staff       (20)     1199 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_ci.py
--rw-r--r--   0 james      (501) staff       (20)     3550 2023-07-07 00:51:47.000000 dask-2023.7.1/dask/tests/test_cli.py
--rw-r--r--   0 james      (501) staff       (20)      379 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_compatibility.py
--rw-r--r--   0 james      (501) staff       (20)    17846 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_config.py
--rw-r--r--   0 james      (501) staff       (20)     1137 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_context.py
--rw-r--r--   0 james      (501) staff       (20)     7422 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_core.py
--rw-r--r--   0 james      (501) staff       (20)     1112 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_datasets.py
--rw-r--r--   0 james      (501) staff       (20)    22989 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_delayed.py
--rw-r--r--   0 james      (501) staff       (20)    35741 2023-06-20 20:00:03.000000 dask-2023.7.1/dask/tests/test_distributed.py
--rw-r--r--   0 james      (501) staff       (20)      925 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_docs.py
--rw-r--r--   0 james      (501) staff       (20)    12271 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_dot.py
--rw-r--r--   0 james      (501) staff       (20)    15070 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_graph_manipulation.py
--rw-r--r--   0 james      (501) staff       (20)     1095 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_hashing.py
--rw-r--r--   0 james      (501) staff       (20)     8860 2023-06-26 19:01:25.000000 dask-2023.7.1/dask/tests/test_highgraph.py
--rw-r--r--   0 james      (501) staff       (20)     9341 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_layers.py
--rw-r--r--   0 james      (501) staff       (20)     5008 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_local.py
--rw-r--r--   0 james      (501) staff       (20)      419 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_ml.py
--rw-r--r--   0 james      (501) staff       (20)     8457 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_multiprocessing.py
--rw-r--r--   0 james      (501) staff       (20)    45227 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_optimization.py
--rw-r--r--   0 james      (501) staff       (20)    28229 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_order.py
--rw-r--r--   0 james      (501) staff       (20)     4684 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_rewrite.py
--rw-r--r--   0 james      (501) staff       (20)     7518 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_sizeof.py
--rw-r--r--   0 james      (501) staff       (20)     7154 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_spark_compat.py
--rw-r--r--   0 james      (501) staff       (20)     1397 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_system.py
--rw-r--r--   0 james      (501) staff       (20)     4749 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_threaded.py
--rw-r--r--   0 james      (501) staff       (20)     5670 2023-04-25 18:34:46.000000 dask-2023.7.1/dask/tests/test_typing.py
--rw-r--r--   0 james      (501) staff       (20)    23923 2023-07-20 20:35:55.000000 dask-2023.7.1/dask/tests/test_utils.py
--rw-r--r--   0 james      (501) staff       (20)     1598 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/test_utils_test.py
--rw-r--r--   0 james      (501) staff       (20)      211 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/tests/warning_aliases.py
--rw-r--r--   0 james      (501) staff       (20)     2993 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/threaded.py
--rw-r--r--   0 james      (501) staff       (20)    14538 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/typing.py
--rw-r--r--   0 james      (501) staff       (20)    58037 2023-07-20 20:35:55.000000 dask-2023.7.1/dask/utils.py
--rw-r--r--   0 james      (501) staff       (20)     4825 2023-04-11 17:13:14.000000 dask-2023.7.1/dask/utils_test.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.822059 dask-2023.7.1/dask/widgets/
--rw-r--r--   0 james      (501) staff       (20)      792 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/widgets/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.827928 dask-2023.7.1/dask/widgets/templates/
--rw-r--r--   0 james      (501) staff       (20)     1295 2023-03-13 17:40:25.000000 dask-2023.7.1/dask/widgets/templates/array.html.j2
--rw-r--r--   0 james      (501) staff       (20)      124 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/widgets/templates/dataframe.html.j2
--rw-r--r--   0 james      (501) staff       (20)     2579 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/widgets/templates/highlevelgraph.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1981 2022-11-09 22:20:24.000000 dask-2023.7.1/dask/widgets/templates/highlevelgraph_layer.html.j2
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.828943 dask-2023.7.1/dask/widgets/tests/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.831739 dask-2023.7.1/dask/widgets/tests/templates/
--rw-r--r--   0 james      (501) staff       (20)       38 2022-10-24 20:44:15.000000 dask-2023.7.1/dask/widgets/tests/templates/bytes.html.j2
--rw-r--r--   0 james      (501) staff       (20)       39 2022-10-24 20:44:15.000000 dask-2023.7.1/dask/widgets/tests/templates/custom_filter.html.j2
--rw-r--r--   0 james      (501) staff       (20)       30 2022-10-24 20:44:15.000000 dask-2023.7.1/dask/widgets/tests/templates/example.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1401 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/widgets/tests/test_widgets.py
--rw-r--r--   0 james      (501) staff       (20)     1120 2023-05-31 15:34:32.000000 dask-2023.7.1/dask/widgets/widgets.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.645095 dask-2023.7.1/dask.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2532 2023-07-20 21:06:44.000000 dask-2023.7.1/dask.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)    13939 2023-07-20 21:06:44.000000 dask-2023.7.1/dask.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-20 21:06:44.000000 dask-2023.7.1/dask.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      124 2023-07-20 21:06:44.000000 dask-2023.7.1/dask.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-20 21:06:43.000000 dask-2023.7.1/dask.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)      454 2023-07-20 21:06:44.000000 dask-2023.7.1/dask.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        5 2023-07-20 21:06:44.000000 dask-2023.7.1/dask.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.833984 dask-2023.7.1/docs/
--rw-r--r--   0 james      (501) staff       (20)     5741 2023-03-22 19:03:53.000000 dask-2023.7.1/docs/Makefile
--rw-r--r--   0 james      (501) staff       (20)     5186 2022-08-08 20:45:08.000000 dask-2023.7.1/docs/make.bat
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.945646 dask-2023.7.1/docs/source/
--rw-r--r--   0 james      (501) staff       (20)    17598 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/10-minutes-to-dask.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.959982 dask-2023.7.1/docs/source/_static/
--rw-r--r--   0 james      (501) staff       (20)    10187 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/_static/config_converter.js
--rw-r--r--   0 james      (501) staff       (20)    11021 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/_static/dask-simple.png
--rw-r--r--   0 james      (501) staff       (20)     2375 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/_static/main-page.css
--rw-r--r--   0 james      (501) staff       (20)    15598 2022-08-08 20:45:08.000000 dask-2023.7.1/docs/source/_static/profile.html
--rw-r--r--   0 james      (501) staff       (20)    65304 2022-08-08 20:45:08.000000 dask-2023.7.1/docs/source/_static/stacked_profile.html
--rw-r--r--   0 james      (501) staff       (20)      523 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/_static/style.css
--rw-r--r--   0 james      (501) staff       (20)      365 2021-06-16 20:41:28.000000 dask-2023.7.1/docs/source/_static/theme_overrides.css
--rw-r--r--   0 james      (501) staff       (20)   292662 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/_static/transpose_cyto.html
--rw-r--r--   0 james      (501) staff       (20)    49423 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/_static/yaml.min.js
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.963069 dask-2023.7.1/docs/source/_templates/
--rw-r--r--   0 james      (501) staff       (20)      180 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/_templates/layout.html
--rw-r--r--   0 james      (501) staff       (20)     3109 2023-07-20 20:35:59.000000 dask-2023.7.1/docs/source/api.rst
--rw-r--r--   0 james      (501) staff       (20)     6968 2023-05-24 15:39:04.000000 dask-2023.7.1/docs/source/array-api.rst
--rw-r--r--   0 james      (501) staff       (20)     2943 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/array-assignment.rst
--rw-r--r--   0 james      (501) staff       (20)     4740 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/array-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)    13262 2023-07-07 00:51:47.000000 dask-2023.7.1/docs/source/array-chunks.rst
--rw-r--r--   0 james      (501) staff       (20)    18437 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/array-creation.rst
--rw-r--r--   0 james      (501) staff       (20)     5885 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/array-design.rst
--rw-r--r--   0 james      (501) staff       (20)     2857 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/array-gufunc.rst
--rw-r--r--   0 james      (501) staff       (20)     6069 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/array-overlap.rst
--rw-r--r--   0 james      (501) staff       (20)     3924 2023-05-19 15:53:47.000000 dask-2023.7.1/docs/source/array-random.rst
--rw-r--r--   0 james      (501) staff       (20)     4137 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/array-slicing.rst
--rw-r--r--   0 james      (501) staff       (20)     3291 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/array-sparse.rst
--rw-r--r--   0 james      (501) staff       (20)     2018 2022-10-07 21:37:36.000000 dask-2023.7.1/docs/source/array-stack.rst
--rw-r--r--   0 james      (501) staff       (20)     1140 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/array-stats.rst
--rw-r--r--   0 james      (501) staff       (20)     4121 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/array.rst
--rw-r--r--   0 james      (501) staff       (20)     1574 2022-08-08 20:45:08.000000 dask-2023.7.1/docs/source/bag-api.rst
--rw-r--r--   0 james      (501) staff       (20)     4557 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/bag-creation.rst
--rw-r--r--   0 james      (501) staff       (20)     4068 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/bag.rst
--rw-r--r--   0 james      (501) staff       (20)    14050 2023-05-22 17:52:26.000000 dask-2023.7.1/docs/source/best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     5553 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/caching.rst
--rw-r--r--   0 james      (501) staff       (20)   310479 2023-07-20 21:00:24.000000 dask-2023.7.1/docs/source/changelog.rst
--rw-r--r--   0 james      (501) staff       (20)      211 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/cheatsheet.rst
--rw-r--r--   0 james      (501) staff       (20)     4047 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/cli.rst
--rw-r--r--   0 james      (501) staff       (20)    15465 2023-03-13 20:41:19.000000 dask-2023.7.1/docs/source/conf.py
--rw-r--r--   0 james      (501) staff       (20)    16654 2023-04-06 21:35:01.000000 dask-2023.7.1/docs/source/configuration.rst
--rw-r--r--   0 james      (501) staff       (20)    18651 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/custom-collections.rst
--rw-r--r--   0 james      (501) staff       (20)     3604 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/custom-graphs.rst
--rw-r--r--   0 james      (501) staff       (20)      932 2023-05-31 15:34:32.000000 dask-2023.7.1/docs/source/dashboard-progress-script.py
--rw-r--r--   0 james      (501) staff       (20)    15045 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/dashboard.rst
--rw-r--r--   0 james      (501) staff       (20)   203552 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/daskcheatsheet.pdf
--rw-r--r--   0 james      (501) staff       (20)    13611 2023-06-26 19:01:25.000000 dask-2023.7.1/docs/source/dataframe-api.rst
--rw-r--r--   0 james      (501) staff       (20)     9611 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/dataframe-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     3951 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/dataframe-categoricals.rst
--rw-r--r--   0 james      (501) staff       (20)     5967 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/dataframe-create.rst
--rw-r--r--   0 james      (501) staff       (20)     5002 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/dataframe-design.rst
--rw-r--r--   0 james      (501) staff       (20)     6224 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/dataframe-extend.rst
--rw-r--r--   0 james      (501) staff       (20)     8050 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/dataframe-groupby.rst
--rw-r--r--   0 james      (501) staff       (20)     6115 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/dataframe-indexing.rst
--rw-r--r--   0 james      (501) staff       (20)     3454 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/dataframe-joins.rst
--rw-r--r--   0 james      (501) staff       (20)    10952 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/dataframe-parquet.rst
--rw-r--r--   0 james      (501) staff       (20)    12661 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/dataframe-sql.rst
--rw-r--r--   0 james      (501) staff       (20)     7772 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/dataframe.rst
--rw-r--r--   0 james      (501) staff       (20)      363 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/debugging-performance.rst
--rw-r--r--   0 james      (501) staff       (20)     1696 2022-08-08 20:45:08.000000 dask-2023.7.1/docs/source/delayed-api.rst
--rw-r--r--   0 james      (501) staff       (20)    17616 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/delayed-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     1497 2022-10-07 21:37:36.000000 dask-2023.7.1/docs/source/delayed-collections.rst
--rw-r--r--   0 james      (501) staff       (20)     6357 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/delayed.rst
--rw-r--r--   0 james      (501) staff       (20)     3620 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/deploying-cli.rst
--rw-r--r--   0 james      (501) staff       (20)     3012 2023-05-22 17:52:26.000000 dask-2023.7.1/docs/source/deploying-cloud.rst
--rw-r--r--   0 james      (501) staff       (20)     2868 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/deploying-docker.rst
--rw-r--r--   0 james      (501) staff       (20)     9939 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/deploying-hpc.rst
--rw-r--r--   0 james      (501) staff       (20)     4001 2023-05-19 15:53:47.000000 dask-2023.7.1/docs/source/deploying-kubernetes.rst
--rw-r--r--   0 james      (501) staff       (20)     5823 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/deploying-python-advanced.rst
--rw-r--r--   0 james      (501) staff       (20)     2839 2023-04-25 18:34:46.000000 dask-2023.7.1/docs/source/deploying-python.rst
--rw-r--r--   0 james      (501) staff       (20)     1619 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/deploying-ssh.rst
--rw-r--r--   0 james      (501) staff       (20)     7356 2023-06-12 20:31:35.000000 dask-2023.7.1/docs/source/deploying.rst
--rw-r--r--   0 james      (501) staff       (20)    10873 2023-05-22 17:52:26.000000 dask-2023.7.1/docs/source/deployment-considerations.rst
--rw-r--r--   0 james      (501) staff       (20)    13144 2023-05-31 15:34:32.000000 dask-2023.7.1/docs/source/develop.rst
--rw-r--r--   0 james      (501) staff       (20)     4442 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/diagnostics-distributed.rst
--rw-r--r--   0 james      (501) staff       (20)    10407 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/diagnostics-local.rst
--rw-r--r--   0 james      (501) staff       (20)     4364 2023-05-22 17:52:26.000000 dask-2023.7.1/docs/source/ecosystem.rst
--rw-r--r--   0 james      (501) staff       (20)    19999 2023-05-22 17:52:26.000000 dask-2023.7.1/docs/source/faq.rst
--rw-r--r--   0 james      (501) staff       (20)    25569 2023-05-19 15:53:47.000000 dask-2023.7.1/docs/source/futures.rst
--rw-r--r--   0 james      (501) staff       (20)     5820 2022-10-07 21:37:14.000000 dask-2023.7.1/docs/source/gpu.rst
--rw-r--r--   0 james      (501) staff       (20)     2541 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/graph_manipulation.rst
--rw-r--r--   0 james      (501) staff       (20)     5433 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/graphs.rst
--rw-r--r--   0 james      (501) staff       (20)     5399 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/graphviz.rst
--rw-r--r--   0 james      (501) staff       (20)     6946 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/high-level-graphs.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:44.973411 dask-2023.7.1/docs/source/how-to/
--rw-r--r--   0 james      (501) staff       (20)     4364 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/how-to/adaptive.rst
--rw-r--r--   0 james      (501) staff       (20)    15360 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/how-to/connect-to-remote-data.rst
--rw-r--r--   0 james      (501) staff       (20)     4209 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/how-to/customize-initialization.rst
--rw-r--r--   0 james      (501) staff       (20)    10859 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/how-to/debug.rst
--rw-r--r--   0 james      (501) staff       (20)     1722 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/how-to/extend-sizeof.rst
--rw-r--r--   0 james      (501) staff       (20)      433 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/how-to/index.rst
--rw-r--r--   0 james      (501) staff       (20)     4562 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/how-to/manage-environments.rst
--rw-r--r--   0 james      (501) staff       (20)     6680 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/how-to/selecting-the-collection-backend.rst
--rw-r--r--   0 james      (501) staff       (20)      902 2023-04-25 18:34:46.000000 dask-2023.7.1/docs/source/how-to/setup-prometheus.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:45.216322 dask-2023.7.1/docs/source/images/
--rw-r--r--   0 james      (501) staff       (20)    99565 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/10_minutes_array_graph.png
--rw-r--r--   0 james      (501) staff       (20)    22442 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/10_minutes_bag_graph.png
--rw-r--r--   0 james      (501) staff       (20)    56229 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/10_minutes_dataframe_graph.png
--rw-r--r--   0 james      (501) staff       (20)     4059 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/HHMI_Janelia_Color.png
--rw-r--r--   0 james      (501) staff       (20)    18406 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/images/array.svg
--rw-r--r--   0 james      (501) staff       (20)  1620104 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/async-embarrassing.gif
--rw-r--r--   0 james      (501) staff       (20)    10752 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/concurrent-futures-threaded.webp
--rw-r--r--   0 james      (501) staff       (20)   135129 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/crosstalk.svg
--rw-r--r--   0 james      (501) staff       (20)  2367087 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dashboard_jupyterlab.png
--rw-r--r--   0 james      (501) staff       (20)    37971 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dashboard_link.png
--rw-r--r--   0 james      (501) staff       (20)    68712 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dashboard_memory.png
--rw-r--r--   0 james      (501) staff       (20)   281018 2023-04-25 18:34:46.000000 dask-2023.7.1/docs/source/images/dashboard_memory_new.gif
--rw-r--r--   0 james      (501) staff       (20)    25435 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/images/dashboard_progress.png
--rw-r--r--   0 james      (501) staff       (20)   276928 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/images/dashboard_status.png
--rw-r--r--   0 james      (501) staff       (20)    12009 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/images/dashboard_task_processing.png
--rw-r--r--   0 james      (501) staff       (20)    58238 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dashboard_task_stream_unhealthy.png
--rw-r--r--   0 james      (501) staff       (20)   103654 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dashboard_taskstream_healthy.png
--rw-r--r--   0 james      (501) staff       (20)   112822 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/dask-adaptive.svg
--rw-r--r--   0 james      (501) staff       (20)    14645 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/dask-array.svg
--rw-r--r--   0 james      (501) staff       (20)   222084 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/dask-cluster-manager.svg
--rw-r--r--   0 james      (501) staff       (20)    18782 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/dask-dataframe.svg
--rw-r--r--   0 james      (501) staff       (20)   381903 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask-overview-distributed-callout.svg
--rw-r--r--   0 james      (501) staff       (20)   357643 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask-overview-schedulers.svg
--rw-r--r--   0 james      (501) staff       (20)    97471 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/dask-overview.svg
--rw-r--r--   0 james      (501) staff       (20)     3022 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_horizontal.svg
--rw-r--r--   0 james      (501) staff       (20)     3651 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_horizontal_black.svg
--rw-r--r--   0 james      (501) staff       (20)     3767 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_horizontal_on_blue.svg
--rw-r--r--   0 james      (501) staff       (20)     3738 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_horizontal_on_pink.svg
--rw-r--r--   0 james      (501) staff       (20)     3738 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_horizontal_white.svg
--rw-r--r--   0 james      (501) staff       (20)     1607 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_icon.svg
--rw-r--r--   0 james      (501) staff       (20)     1571 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_icon_black.svg
--rw-r--r--   0 james      (501) staff       (20)     1607 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_icon_on_pink.svg
--rw-r--r--   0 james      (501) staff       (20)     1609 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/dask_icon_white.svg
--rw-r--r--   0 james      (501) staff       (20)    20216 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/delayed-inc-double-add.svg
--rw-r--r--   0 james      (501) staff       (20)   104628 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/distributed-overview.svg
--rw-r--r--   0 james      (501) staff       (20)    18297 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/images/frame-shuffle.svg
--rw-r--r--   0 james      (501) staff       (20)    22979 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/images/frame-sort.svg
--rw-r--r--   0 james      (501) staff       (20)    12181 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/images/frame.svg
--rw-r--r--   0 james      (501) staff       (20)    41828 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/gputester-msg.png
--rw-r--r--   0 james      (501) staff       (20)   210392 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/images/growth_of_languages.png
--rw-r--r--   0 james      (501) staff       (20)   167834 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/images/growth_of_libraries.png
--rw-r--r--   0 james      (501) staff       (20)     4097 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/inc-add.svg
--rw-r--r--   0 james      (501) staff       (20)   123010 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/map-reduce-task-scheduling.svg
--rw-r--r--   0 james      (501) staff       (20)   482302 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/map_blocks_drop_axis.png
--rw-r--r--   0 james      (501) staff       (20)   113067 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/images/merge_chunks.png
--rw-r--r--   0 james      (501) staff       (20)    63244 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/images/merge_chunks_false.png
--rw-r--r--   0 james      (501) staff       (20)    13024 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/images/optimize_dask1.svg
--rw-r--r--   0 james      (501) staff       (20)     8803 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/images/optimize_dask2.svg
--rw-r--r--   0 james      (501) staff       (20)     5198 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/images/optimize_dask3.svg
--rw-r--r--   0 james      (501) staff       (20)     4104 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/images/optimize_dask4.svg
--rw-r--r--   0 james      (501) staff       (20)     2738 2021-11-11 17:33:01.000000 dask-2023.7.1/docs/source/images/optimize_dask5.svg
--rw-r--r--   0 james      (501) staff       (20)   292827 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/images/order-failure.png
--rw-r--r--   0 james      (501) staff       (20)   239828 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/images/order-success.png
--rw-r--r--   0 james      (501) staff       (20)    40833 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/overlap.svg
--rw-r--r--   0 james      (501) staff       (20)    18785 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/overlapping-blocks.svg
--rw-r--r--   0 james      (501) staff       (20)     4537 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/overlapping-neighbors.svg
--rw-r--r--   0 james      (501) staff       (20)    20533 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/pipeline.svg
--rw-r--r--   0 james      (501) staff       (20)    31576 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/images/reshape.png
--rw-r--r--   0 james      (501) staff       (20)    31410 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/images/reshape_problem.png
--rw-r--r--   0 james      (501) staff       (20)    33288 2021-11-11 20:27:17.000000 dask-2023.7.1/docs/source/images/reshape_rechunked.png
--rw-r--r--   0 james      (501) staff       (20)    50209 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/images/scaling-edges.png
--rw-r--r--   0 james      (501) staff       (20)    68476 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/images/scaling-nodes.png
--rw-r--r--   0 james      (501) staff       (20)    21294 2021-06-08 02:50:31.000000 dask-2023.7.1/docs/source/images/simple-dask.png
--rw-r--r--   0 james      (501) staff       (20)    27572 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/transpose-hlg-hovertooltip.png
--rw-r--r--   0 james      (501) staff       (20)    84492 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/images/transpose-hlg-html-repr.png
--rw-r--r--   0 james      (501) staff       (20)    39365 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/transpose.svg
--rw-r--r--   0 james      (501) staff       (20)    22446 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/transpose_opt.svg
--rw-r--r--   0 james      (501) staff       (20)   115022 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/images/trivial.svg
--rw-r--r--   0 james      (501) staff       (20)     2451 2021-06-08 02:51:08.000000 dask-2023.7.1/docs/source/images/unoverlapping-neighbors.svg
--rw-r--r--   0 james      (501) staff       (20)     6237 2023-03-13 17:40:25.000000 dask-2023.7.1/docs/source/index.rst
--rw-r--r--   0 james      (501) staff       (20)    15235 2023-05-31 15:34:32.000000 dask-2023.7.1/docs/source/install.rst
--rw-r--r--   0 james      (501) staff       (20)      341 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/internals.rst
--rw-r--r--   0 james      (501) staff       (20)      868 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/logos.rst
--rw-r--r--   0 james      (501) staff       (20)     3573 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/maintainers.rst
--rw-r--r--   0 james      (501) staff       (20)    12200 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/optimize.rst
--rw-r--r--   0 james      (501) staff       (20)     7119 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/order.rst
--rw-r--r--   0 james      (501) staff       (20)     4810 2022-10-07 21:37:14.000000 dask-2023.7.1/docs/source/phases-of-computation.rst
--rw-r--r--   0 james      (501) staff       (20)     5089 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/presentations.rst
--rw-r--r--   0 james      (501) staff       (20)     6010 2022-10-07 21:37:14.000000 dask-2023.7.1/docs/source/scheduler-overview.rst
--rw-r--r--   0 james      (501) staff       (20)     4493 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/scheduling-policy.rst
--rw-r--r--   0 james      (501) staff       (20)    11015 2023-05-31 15:34:32.000000 dask-2023.7.1/docs/source/scheduling.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-20 21:06:45.217250 dask-2023.7.1/docs/source/scripts/
--rw-r--r--   0 james      (501) staff       (20)     3294 2023-05-31 15:34:32.000000 dask-2023.7.1/docs/source/scripts/scheduling.py
--rw-r--r--   0 james      (501) staff       (20)     6104 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/shared.rst
--rw-r--r--   0 james      (501) staff       (20)     9342 2022-11-09 22:20:24.000000 dask-2023.7.1/docs/source/spark.rst
--rw-r--r--   0 james      (501) staff       (20)     3966 2022-10-07 21:37:14.000000 dask-2023.7.1/docs/source/spec.rst
--rw-r--r--   0 james      (501) staff       (20)     4754 2023-05-22 17:52:26.000000 dask-2023.7.1/docs/source/support.rst
--rw-r--r--   0 james      (501) staff       (20)     1831 2021-06-16 20:41:28.000000 dask-2023.7.1/docs/source/understanding-performance.rst
--rw-r--r--   0 james      (501) staff       (20)    12205 2023-05-03 18:02:08.000000 dask-2023.7.1/docs/source/user-interfaces.rst
--rw-r--r--   0 james      (501) staff       (20)    11744 2022-10-24 20:44:15.000000 dask-2023.7.1/docs/source/why.rst
--rw-r--r--   0 james      (501) staff       (20)     5526 2023-07-20 20:46:10.000000 dask-2023.7.1/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-20 21:06:45.218715 dask-2023.7.1/setup.cfg
--rwxr-xr-x   0 james      (501) staff       (20)      194 2023-05-03 18:02:08.000000 dask-2023.7.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.094173 dask-2023.8.0/
+-rw-r--r--   0 james      (501) staff       (20)     1531 2023-07-17 19:15:27.000000 dask-2023.8.0/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      325 2023-07-17 19:15:27.000000 dask-2023.8.0/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     2541 2023-08-04 18:09:12.093986 dask-2023.8.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1291 2023-07-17 19:15:27.000000 dask-2023.8.0/README.rst
+-rw-r--r--   0 james      (501) staff       (20)     2505 2023-08-02 15:27:02.000000 dask-2023.8.0/conftest.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.094359 dask-2023.8.0/dask/
+-rw-r--r--   0 james      (501) staff       (20)      485 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      133 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/__main__.py
+-rw-r--r--   0 james      (501) staff       (20)      643 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/_compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)      500 2023-08-04 18:09:12.094401 dask-2023.8.0/dask/_version.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.002150 dask-2023.8.0/dask/array/
+-rw-r--r--   0 james      (501) staff       (20)     1543 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/array/NUMPY_LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)     5413 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12600 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/backends.py
+-rw-r--r--   0 james      (501) staff       (20)     9983 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/blockwise.py
+-rw-r--r--   0 james      (501) staff       (20)    12304 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/chunk.py
+-rw-r--r--   0 james      (501) staff       (20)     5066 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/chunk_types.py
+-rw-r--r--   0 james      (501) staff       (20)   190831 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/core.py
+-rw-r--r--   0 james      (501) staff       (20)    40564 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/creation.py
+-rw-r--r--   0 james      (501) staff       (20)     2114 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/cupy_entry_point.py
+-rw-r--r--   0 james      (501) staff       (20)      526 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)     9146 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/einsumfuncs.py
+-rw-r--r--   0 james      (501) staff       (20)     7252 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/fft.py
+-rw-r--r--   0 james      (501) staff       (20)    32656 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     1996 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/image.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.002426 dask-2023.8.0/dask/array/lib/
+-rw-r--r--   0 james      (501) staff       (20)       77 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/lib/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      101 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/lib/stride_tricks.py
+-rw-r--r--   0 james      (501) staff       (20)    53335 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/linalg.py
+-rw-r--r--   0 james      (501) staff       (20)     6363 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/ma.py
+-rw-r--r--   0 james      (501) staff       (20)     5699 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/numpy_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    12838 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    28480 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/overlap.py
+-rw-r--r--   0 james      (501) staff       (20)    10652 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/percentile.py
+-rw-r--r--   0 james      (501) staff       (20)    40604 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/random.py
+-rw-r--r--   0 james      (501) staff       (20)    28324 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/rechunk.py
+-rw-r--r--   0 james      (501) staff       (20)    57287 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/reductions.py
+-rw-r--r--   0 james      (501) staff       (20)    10765 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    81977 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/routines.py
+-rw-r--r--   0 james      (501) staff       (20)    72631 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/slicing.py
+-rw-r--r--   0 james      (501) staff       (20)    16184 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/stats.py
+-rw-r--r--   0 james      (501) staff       (20)     8048 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/svg.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.008391 dask-2023.8.0/dask/array/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/array/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)   161461 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/array/tests/test_array_core.py
+-rw-r--r--   0 james      (501) staff       (20)     6689 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_array_function.py
+-rw-r--r--   0 james      (501) staff       (20)     3159 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_array_utils.py
+-rw-r--r--   0 james      (501) staff       (20)    23222 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_atop.py
+-rw-r--r--   0 james      (501) staff       (20)     3304 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_chunk.py
+-rw-r--r--   0 james      (501) staff       (20)    31150 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_creation.py
+-rw-r--r--   0 james      (501) staff       (20)    19888 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_core.py
+-rw-r--r--   0 james      (501) staff       (20)     6456 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_creation.py
+-rw-r--r--   0 james      (501) staff       (20)      594 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    13412 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_linalg.py
+-rw-r--r--   0 james      (501) staff       (20)     4303 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_overlap.py
+-rw-r--r--   0 james      (501) staff       (20)     2862 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_percentile.py
+-rw-r--r--   0 james      (501) staff       (20)     9219 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_random.py
+-rw-r--r--   0 james      (501) staff       (20)     2224 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_reductions.py
+-rw-r--r--   0 james      (501) staff       (20)     7437 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_routines.py
+-rw-r--r--   0 james      (501) staff       (20)     4877 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_slicing.py
+-rw-r--r--   0 james      (501) staff       (20)     2982 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_cupy_sparse.py
+-rw-r--r--   0 james      (501) staff       (20)     8865 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)     8437 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_fft.py
+-rw-r--r--   0 james      (501) staff       (20)    21013 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     1482 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_image.py
+-rw-r--r--   0 james      (501) staff       (20)    36448 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_linalg.py
+-rw-r--r--   0 james      (501) staff       (20)    15635 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_masked.py
+-rw-r--r--   0 james      (501) staff       (20)     1087 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_numpy_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    17446 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    26718 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_overlap.py
+-rw-r--r--   0 james      (501) staff       (20)     3443 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_percentiles.py
+-rw-r--r--   0 james      (501) staff       (20)    15353 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_random.py
+-rw-r--r--   0 james      (501) staff       (20)    36262 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_rechunk.py
+-rw-r--r--   0 james      (501) staff       (20)    32756 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_reductions.py
+-rw-r--r--   0 james      (501) staff       (20)     7289 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    83849 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_routines.py
+-rw-r--r--   0 james      (501) staff       (20)    32302 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_slicing.py
+-rw-r--r--   0 james      (501) staff       (20)     6592 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_sparse.py
+-rw-r--r--   0 james      (501) staff       (20)     5489 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_stats.py
+-rw-r--r--   0 james      (501) staff       (20)     2740 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_svg.py
+-rw-r--r--   0 james      (501) staff       (20)      525 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_testing.py
+-rw-r--r--   0 james      (501) staff       (20)    17390 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     2706 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_wrap.py
+-rw-r--r--   0 james      (501) staff       (20)     1317 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tests/test_xarray.py
+-rw-r--r--   0 james      (501) staff       (20)     4737 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/tiledb_io.py
+-rw-r--r--   0 james      (501) staff       (20)     9943 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    18674 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     6906 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/array/wrap.py
+-rw-r--r--   0 james      (501) staff       (20)     4936 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/backends.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.009531 dask-2023.8.0/dask/bag/
+-rw-r--r--   0 james      (501) staff       (20)      903 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     9111 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/avro.py
+-rw-r--r--   0 james      (501) staff       (20)      763 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/chunk.py
+-rw-r--r--   0 james      (501) staff       (20)    85425 2023-08-02 15:26:59.000000 dask-2023.8.0/dask/bag/core.py
+-rw-r--r--   0 james      (501) staff       (20)     5464 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/random.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.010370 dask-2023.8.0/dask/bag/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/bag/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3808 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/tests/test_avro.py
+-rw-r--r--   0 james      (501) staff       (20)    51087 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/tests/test_bag.py
+-rw-r--r--   0 james      (501) staff       (20)     6528 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/tests/test_random.py
+-rw-r--r--   0 james      (501) staff       (20)     5049 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/tests/test_text.py
+-rw-r--r--   0 james      (501) staff       (20)     6765 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/text.py
+-rw-r--r--   0 james      (501) staff       (20)      241 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bag/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    53616 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/base.py
+-rw-r--r--   0 james      (501) staff       (20)    53252 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/blockwise.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.010938 dask-2023.8.0/dask/bytes/
+-rw-r--r--   0 james      (501) staff       (20)       75 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bytes/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6933 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bytes/core.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.011899 dask-2023.8.0/dask/bytes/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/bytes/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     5158 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bytes/tests/test_bytes_utils.py
+-rw-r--r--   0 james      (501) staff       (20)      530 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bytes/tests/test_compression.py
+-rw-r--r--   0 james      (501) staff       (20)     6563 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/bytes/tests/test_http.py
+-rw-r--r--   0 james      (501) staff       (20)    11476 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bytes/tests/test_local.py
+-rw-r--r--   0 james      (501) staff       (20)    19385 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/bytes/tests/test_s3.py
+-rw-r--r--   0 james      (501) staff       (20)      500 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/bytes/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     2001 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/cache.py
+-rw-r--r--   0 james      (501) staff       (20)     4067 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/callbacks.py
+-rw-r--r--   0 james      (501) staff       (20)     3272 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/cli.py
+-rw-r--r--   0 james      (501) staff       (20)      523 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)    21703 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/config.py
+-rw-r--r--   0 james      (501) staff       (20)     1756 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/context.py
+-rw-r--r--   0 james      (501) staff       (20)    14833 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/core.py
+-rw-r--r--   0 james      (501) staff       (20)     8060 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dask-schema.yaml
+-rw-r--r--   0 james      (501) staff       (20)     2122 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dask.yaml
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.016162 dask-2023.8.0/dask/dataframe/
+-rw-r--r--   0 james      (501) staff       (20)     1812 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7496 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/_compat.py
+-rw-r--r--   0 james      (501) staff       (20)     2171 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/_dtypes.py
+-rw-r--r--   0 james      (501) staff       (20)     3959 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/_pyarrow.py
+-rw-r--r--   0 james      (501) staff       (20)     1936 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/_pyarrow_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    12101 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/accessor.py
+-rw-r--r--   0 james      (501) staff       (20)    24817 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/backends.py
+-rw-r--r--   0 james      (501) staff       (20)     9507 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/categorical.py
+-rw-r--r--   0 james      (501) staff       (20)   301737 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/core.py
+-rw-r--r--   0 james      (501) staff       (20)     4609 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)      552 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/extensions.py
+-rw-r--r--   0 james      (501) staff       (20)   115448 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/groupby.py
+-rw-r--r--   0 james      (501) staff       (20)     2463 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/hyperloglog.py
+-rw-r--r--   0 james      (501) staff       (20)    13412 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/indexing.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.017469 dask-2023.8.0/dask/dataframe/io/
+-rw-r--r--   0 james      (501) staff       (20)      706 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    33854 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/csv.py
+-rw-r--r--   0 james      (501) staff       (20)    18318 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/demo.py
+-rw-r--r--   0 james      (501) staff       (20)    18275 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/hdf.py
+-rw-r--r--   0 james      (501) staff       (20)    38599 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/io.py
+-rw-r--r--   0 james      (501) staff       (20)    11163 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/json.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.018038 dask-2023.8.0/dask/dataframe/io/orc/
+-rw-r--r--   0 james      (501) staff       (20)       92 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/orc/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4487 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/orc/arrow.py
+-rw-r--r--   0 james      (501) staff       (20)     7098 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/orc/core.py
+-rw-r--r--   0 james      (501) staff       (20)      510 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/orc/utils.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.018850 dask-2023.8.0/dask/dataframe/io/parquet/
+-rw-r--r--   0 james      (501) staff       (20)      166 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/parquet/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    71794 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/parquet/arrow.py
+-rw-r--r--   0 james      (501) staff       (20)    67270 2023-08-02 15:26:59.000000 dask-2023.8.0/dask/dataframe/io/parquet/core.py
+-rw-r--r--   0 james      (501) staff       (20)    52312 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/parquet/fastparquet.py
+-rw-r--r--   0 james      (501) staff       (20)    32896 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/parquet/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    21108 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/sql.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.020311 dask-2023.8.0/dask/dataframe/io/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/dataframe/io/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    59293 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/tests/test_csv.py
+-rw-r--r--   0 james      (501) staff       (20)    11113 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/tests/test_demo.py
+-rw-r--r--   0 james      (501) staff       (20)    27232 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/tests/test_hdf.py
+-rw-r--r--   0 james      (501) staff       (20)    34779 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/tests/test_io.py
+-rw-r--r--   0 james      (501) staff       (20)     8625 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/tests/test_json.py
+-rw-r--r--   0 james      (501) staff       (20)     5238 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/tests/test_orc.py
+-rw-r--r--   0 james      (501) staff       (20)   167023 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/io/tests/test_parquet.py
+-rw-r--r--   0 james      (501) staff       (20)    17632 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/tests/test_sql.py
+-rw-r--r--   0 james      (501) staff       (20)     8041 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/io/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    14071 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/methods.py
+-rw-r--r--   0 james      (501) staff       (20)    54050 2023-08-02 15:26:59.000000 dask-2023.8.0/dask/dataframe/multi.py
+-rw-r--r--   0 james      (501) staff       (20)     1600 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/numeric.py
+-rw-r--r--   0 james      (501) staff       (20)     8778 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/optimize.py
+-rw-r--r--   0 james      (501) staff       (20)    20104 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/partitionquantiles.py
+-rw-r--r--   0 james      (501) staff       (20)    11825 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    21893 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/rolling.py
+-rw-r--r--   0 james      (501) staff       (20)    38106 2023-08-02 15:26:59.000000 dask-2023.8.0/dask/dataframe/shuffle.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.024356 dask-2023.8.0/dask/dataframe/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/dataframe/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    10633 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_accessors.py
+-rw-r--r--   0 james      (501) staff       (20)    67628 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_arithmetics_reduction.py
+-rw-r--r--   0 james      (501) staff       (20)      942 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_boolean.py
+-rw-r--r--   0 james      (501) staff       (20)    16678 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_categorical.py
+-rw-r--r--   0 james      (501) staff       (20)   194019 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_dataframe.py
+-rw-r--r--   0 james      (501) staff       (20)     1456 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_extensions.py
+-rw-r--r--   0 james      (501) staff       (20)    14743 2023-07-19 20:27:22.000000 dask-2023.8.0/dask/dataframe/tests/test_format.py
+-rw-r--r--   0 james      (501) staff       (20)   121815 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_groupby.py
+-rw-r--r--   0 james      (501) staff       (20)     2702 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_hashing.py
+-rw-r--r--   0 james      (501) staff       (20)     2897 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_hyperloglog.py
+-rw-r--r--   0 james      (501) staff       (20)    22382 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_indexing.py
+-rw-r--r--   0 james      (501) staff       (20)     7034 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_merge_column_and_index.py
+-rw-r--r--   0 james      (501) staff       (20)      463 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_methods.py
+-rw-r--r--   0 james      (501) staff       (20)    91084 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_multi.py
+-rw-r--r--   0 james      (501) staff       (20)     2120 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_numeric.py
+-rw-r--r--   0 james      (501) staff       (20)     1067 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_optimize_dataframe.py
+-rw-r--r--   0 james      (501) staff       (20)     6662 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_pyarrow.py
+-rw-r--r--   0 james      (501) staff       (20)     4550 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_pyarrow_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    11571 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    17510 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_rolling.py
+-rw-r--r--   0 james      (501) staff       (20)    54512 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_shuffle.py
+-rw-r--r--   0 james      (501) staff       (20)    16595 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tests/test_ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    22156 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tests/test_utils_dataframe.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.024675 dask-2023.8.0/dask/dataframe/tseries/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/dataframe/tseries/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7664 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/tseries/resample.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.024990 dask-2023.8.0/dask/dataframe/tseries/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/dataframe/tseries/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6866 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dataframe/tseries/tests/test_resample.py
+-rw-r--r--   0 james      (501) staff       (20)    27606 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/dataframe/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     5314 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/datasets.py
+-rw-r--r--   0 james      (501) staff       (20)    24389 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/delayed.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.025586 dask-2023.8.0/dask/diagnostics/
+-rw-r--r--   0 james      (501) staff       (20)      258 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/diagnostics/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12136 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/diagnostics/profile.py
+-rw-r--r--   0 james      (501) staff       (20)    16332 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/diagnostics/profile_visualize.py
+-rw-r--r--   0 james      (501) staff       (20)     5001 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/diagnostics/progress.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.025976 dask-2023.8.0/dask/diagnostics/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/diagnostics/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12045 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/diagnostics/tests/test_profiler.py
+-rw-r--r--   0 james      (501) staff       (20)     3388 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/diagnostics/tests/test_progress.py
+-rw-r--r--   0 james      (501) staff       (20)      715 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/distributed.py
+-rw-r--r--   0 james      (501) staff       (20)    16587 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/dot.py
+-rw-r--r--   0 james      (501) staff       (20)    19595 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/graph_manipulation.py
+-rw-r--r--   0 james      (501) staff       (20)     2492 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/hashing.py
+-rw-r--r--   0 james      (501) staff       (20)    34778 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/highlevelgraph.py
+-rw-r--r--   0 james      (501) staff       (20)    46007 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/layers.py
+-rw-r--r--   0 james      (501) staff       (20)    18888 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/local.py
+-rw-r--r--   0 james      (501) staff       (20)      487 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/ml.py
+-rw-r--r--   0 james      (501) staff       (20)     8466 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/multiprocessing.py
+-rw-r--r--   0 james      (501) staff       (20)    35638 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    45768 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/order.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/py.typed
+-rw-r--r--   0 james      (501) staff       (20)    12597 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/rewrite.py
+-rw-r--r--   0 james      (501) staff       (20)     7298 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/sizeof.py
+-rw-r--r--   0 james      (501) staff       (20)     1510 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/system.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.031169 dask-2023.8.0/dask/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2023.8.0/dask/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      742 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_backends.py
+-rw-r--r--   0 james      (501) staff       (20)    51124 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_base.py
+-rw-r--r--   0 james      (501) staff       (20)     1613 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_cache.py
+-rw-r--r--   0 james      (501) staff       (20)     2570 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_callbacks.py
+-rw-r--r--   0 james      (501) staff       (20)     1199 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_ci.py
+-rw-r--r--   0 james      (501) staff       (20)     3550 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_cli.py
+-rw-r--r--   0 james      (501) staff       (20)      379 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)    17846 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_config.py
+-rw-r--r--   0 james      (501) staff       (20)     1137 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_context.py
+-rw-r--r--   0 james      (501) staff       (20)     7422 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_core.py
+-rw-r--r--   0 james      (501) staff       (20)     1112 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_datasets.py
+-rw-r--r--   0 james      (501) staff       (20)    22989 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_delayed.py
+-rw-r--r--   0 james      (501) staff       (20)    35741 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_distributed.py
+-rw-r--r--   0 james      (501) staff       (20)      925 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_docs.py
+-rw-r--r--   0 james      (501) staff       (20)    12271 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_dot.py
+-rw-r--r--   0 james      (501) staff       (20)    15070 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_graph_manipulation.py
+-rw-r--r--   0 james      (501) staff       (20)     1095 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_hashing.py
+-rw-r--r--   0 james      (501) staff       (20)     8860 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_highgraph.py
+-rw-r--r--   0 james      (501) staff       (20)     9341 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_layers.py
+-rw-r--r--   0 james      (501) staff       (20)     5008 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_local.py
+-rw-r--r--   0 james      (501) staff       (20)      419 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_ml.py
+-rw-r--r--   0 james      (501) staff       (20)     8457 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_multiprocessing.py
+-rw-r--r--   0 james      (501) staff       (20)    45227 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    28229 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_order.py
+-rw-r--r--   0 james      (501) staff       (20)     4684 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_rewrite.py
+-rw-r--r--   0 james      (501) staff       (20)     7518 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_sizeof.py
+-rw-r--r--   0 james      (501) staff       (20)     7154 2023-08-02 15:27:02.000000 dask-2023.8.0/dask/tests/test_spark_compat.py
+-rw-r--r--   0 james      (501) staff       (20)     1397 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_system.py
+-rw-r--r--   0 james      (501) staff       (20)     4749 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_threaded.py
+-rw-r--r--   0 james      (501) staff       (20)     5670 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_typing.py
+-rw-r--r--   0 james      (501) staff       (20)    23923 2023-08-02 15:26:59.000000 dask-2023.8.0/dask/tests/test_utils.py
+-rw-r--r--   0 james      (501) staff       (20)     1598 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/test_utils_test.py
+-rw-r--r--   0 james      (501) staff       (20)      211 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/tests/warning_aliases.py
+-rw-r--r--   0 james      (501) staff       (20)     2993 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/threaded.py
+-rw-r--r--   0 james      (501) staff       (20)    14538 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/typing.py
+-rw-r--r--   0 james      (501) staff       (20)    58037 2023-08-02 15:26:59.000000 dask-2023.8.0/dask/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     4825 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/utils_test.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.031525 dask-2023.8.0/dask/widgets/
+-rw-r--r--   0 james      (501) staff       (20)      792 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.032558 dask-2023.8.0/dask/widgets/templates/
+-rw-r--r--   0 james      (501) staff       (20)     1295 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/templates/array.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      124 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/templates/dataframe.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     2579 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/templates/highlevelgraph.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1981 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/templates/highlevelgraph_layer.html.j2
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.032729 dask-2023.8.0/dask/widgets/tests/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.033249 dask-2023.8.0/dask/widgets/tests/templates/
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/tests/templates/bytes.html.j2
+-rw-r--r--   0 james      (501) staff       (20)       39 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/tests/templates/custom_filter.html.j2
+-rw-r--r--   0 james      (501) staff       (20)       30 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/tests/templates/example.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1401 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/tests/test_widgets.py
+-rw-r--r--   0 james      (501) staff       (20)     1120 2023-07-17 19:15:27.000000 dask-2023.8.0/dask/widgets/widgets.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:11.997306 dask-2023.8.0/dask.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2541 2023-08-04 18:09:11.000000 dask-2023.8.0/dask.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)    13981 2023-08-04 18:09:11.000000 dask-2023.8.0/dask.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-04 18:09:11.000000 dask-2023.8.0/dask.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      124 2023-08-04 18:09:11.000000 dask-2023.8.0/dask.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-04 18:09:11.000000 dask-2023.8.0/dask.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)      454 2023-08-04 18:09:11.000000 dask-2023.8.0/dask.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        5 2023-08-04 18:09:11.000000 dask-2023.8.0/dask.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.033619 dask-2023.8.0/docs/
+-rw-r--r--   0 james      (501) staff       (20)     5741 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     5186 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/make.bat
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.056918 dask-2023.8.0/docs/source/
+-rw-r--r--   0 james      (501) staff       (20)    17598 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/10-minutes-to-dask.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.059280 dask-2023.8.0/docs/source/_static/
+-rw-r--r--   0 james      (501) staff       (20)    10187 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/config_converter.js
+-rw-r--r--   0 james      (501) staff       (20)    11021 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/_static/dask-simple.png
+-rw-r--r--   0 james      (501) staff       (20)     2375 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/main-page.css
+-rw-r--r--   0 james      (501) staff       (20)    15598 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/profile.html
+-rw-r--r--   0 james      (501) staff       (20)    65304 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/stacked_profile.html
+-rw-r--r--   0 james      (501) staff       (20)      523 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/style.css
+-rw-r--r--   0 james      (501) staff       (20)      365 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 james      (501) staff       (20)   292662 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/transpose_cyto.html
+-rw-r--r--   0 james      (501) staff       (20)    49423 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_static/yaml.min.js
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.059884 dask-2023.8.0/docs/source/_templates/
+-rw-r--r--   0 james      (501) staff       (20)      180 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/_templates/layout.html
+-rw-r--r--   0 james      (501) staff       (20)     3109 2023-08-02 15:26:59.000000 dask-2023.8.0/docs/source/api.rst
+-rw-r--r--   0 james      (501) staff       (20)     7189 2023-08-02 15:27:02.000000 dask-2023.8.0/docs/source/array-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     2943 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-assignment.rst
+-rw-r--r--   0 james      (501) staff       (20)     4740 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)    13262 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-chunks.rst
+-rw-r--r--   0 james      (501) staff       (20)    18437 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-creation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5885 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-design.rst
+-rw-r--r--   0 james      (501) staff       (20)     2857 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-gufunc.rst
+-rw-r--r--   0 james      (501) staff       (20)    21469 2023-08-02 15:27:02.000000 dask-2023.8.0/docs/source/array-numpy-compatibility.rst
+-rw-r--r--   0 james      (501) staff       (20)     6069 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-overlap.rst
+-rw-r--r--   0 james      (501) staff       (20)     3924 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-random.rst
+-rw-r--r--   0 james      (501) staff       (20)     4137 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-slicing.rst
+-rw-r--r--   0 james      (501) staff       (20)     3291 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-sparse.rst
+-rw-r--r--   0 james      (501) staff       (20)     2018 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-stack.rst
+-rw-r--r--   0 james      (501) staff       (20)     1140 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/array-stats.rst
+-rw-r--r--   0 james      (501) staff       (20)     4154 2023-08-02 15:27:02.000000 dask-2023.8.0/docs/source/array.rst
+-rw-r--r--   0 james      (501) staff       (20)     1574 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/bag-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     4557 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/bag-creation.rst
+-rw-r--r--   0 james      (501) staff       (20)     4068 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/bag.rst
+-rw-r--r--   0 james      (501) staff       (20)    14050 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     5553 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/caching.rst
+-rw-r--r--   0 james      (501) staff       (20)   311306 2023-08-04 18:00:45.000000 dask-2023.8.0/docs/source/changelog.rst
+-rw-r--r--   0 james      (501) staff       (20)      211 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/cheatsheet.rst
+-rw-r--r--   0 james      (501) staff       (20)     4047 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/cli.rst
+-rw-r--r--   0 james      (501) staff       (20)    15465 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/conf.py
+-rw-r--r--   0 james      (501) staff       (20)    16654 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/configuration.rst
+-rw-r--r--   0 james      (501) staff       (20)    18651 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/custom-collections.rst
+-rw-r--r--   0 james      (501) staff       (20)     3604 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/custom-graphs.rst
+-rw-r--r--   0 james      (501) staff       (20)      932 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dashboard-progress-script.py
+-rw-r--r--   0 james      (501) staff       (20)    15045 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dashboard.rst
+-rw-r--r--   0 james      (501) staff       (20)   203552 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/daskcheatsheet.pdf
+-rw-r--r--   0 james      (501) staff       (20)    13611 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     9611 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     3951 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-categoricals.rst
+-rw-r--r--   0 james      (501) staff       (20)     5967 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-create.rst
+-rw-r--r--   0 james      (501) staff       (20)     5002 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-design.rst
+-rw-r--r--   0 james      (501) staff       (20)     6224 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-extend.rst
+-rw-r--r--   0 james      (501) staff       (20)     8050 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-groupby.rst
+-rw-r--r--   0 james      (501) staff       (20)     6115 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-indexing.rst
+-rw-r--r--   0 james      (501) staff       (20)     3454 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-joins.rst
+-rw-r--r--   0 james      (501) staff       (20)    10952 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-parquet.rst
+-rw-r--r--   0 james      (501) staff       (20)    12661 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe-sql.rst
+-rw-r--r--   0 james      (501) staff       (20)     7772 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/dataframe.rst
+-rw-r--r--   0 james      (501) staff       (20)      363 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/debugging-performance.rst
+-rw-r--r--   0 james      (501) staff       (20)     1696 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/delayed-api.rst
+-rw-r--r--   0 james      (501) staff       (20)    17616 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/delayed-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     1497 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/delayed-collections.rst
+-rw-r--r--   0 james      (501) staff       (20)     6357 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/delayed.rst
+-rw-r--r--   0 james      (501) staff       (20)     3620 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-cli.rst
+-rw-r--r--   0 james      (501) staff       (20)     3012 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-cloud.rst
+-rw-r--r--   0 james      (501) staff       (20)     2868 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-docker.rst
+-rw-r--r--   0 james      (501) staff       (20)     9939 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-hpc.rst
+-rw-r--r--   0 james      (501) staff       (20)     4001 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-kubernetes.rst
+-rw-r--r--   0 james      (501) staff       (20)     5823 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-python-advanced.rst
+-rw-r--r--   0 james      (501) staff       (20)     2839 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-python.rst
+-rw-r--r--   0 james      (501) staff       (20)     1619 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying-ssh.rst
+-rw-r--r--   0 james      (501) staff       (20)     7356 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deploying.rst
+-rw-r--r--   0 james      (501) staff       (20)    10873 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/deployment-considerations.rst
+-rw-r--r--   0 james      (501) staff       (20)    13144 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/develop.rst
+-rw-r--r--   0 james      (501) staff       (20)     4442 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/diagnostics-distributed.rst
+-rw-r--r--   0 james      (501) staff       (20)    10407 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/diagnostics-local.rst
+-rw-r--r--   0 james      (501) staff       (20)     4364 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/ecosystem.rst
+-rw-r--r--   0 james      (501) staff       (20)    19999 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/faq.rst
+-rw-r--r--   0 james      (501) staff       (20)    25569 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/futures.rst
+-rw-r--r--   0 james      (501) staff       (20)     5820 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/gpu.rst
+-rw-r--r--   0 james      (501) staff       (20)     2541 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/graph_manipulation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5433 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/graphs.rst
+-rw-r--r--   0 james      (501) staff       (20)     5399 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/graphviz.rst
+-rw-r--r--   0 james      (501) staff       (20)     6946 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/high-level-graphs.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.061435 dask-2023.8.0/docs/source/how-to/
+-rw-r--r--   0 james      (501) staff       (20)     4364 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/adaptive.rst
+-rw-r--r--   0 james      (501) staff       (20)    15360 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/connect-to-remote-data.rst
+-rw-r--r--   0 james      (501) staff       (20)     4209 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/customize-initialization.rst
+-rw-r--r--   0 james      (501) staff       (20)    11477 2023-08-04 17:53:09.000000 dask-2023.8.0/docs/source/how-to/debug.rst
+-rw-r--r--   0 james      (501) staff       (20)     1722 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/extend-sizeof.rst
+-rw-r--r--   0 james      (501) staff       (20)      433 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/index.rst
+-rw-r--r--   0 james      (501) staff       (20)     4562 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/manage-environments.rst
+-rw-r--r--   0 james      (501) staff       (20)     6680 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/selecting-the-collection-backend.rst
+-rw-r--r--   0 james      (501) staff       (20)      902 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/how-to/setup-prometheus.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.093547 dask-2023.8.0/docs/source/images/
+-rw-r--r--   0 james      (501) staff       (20)    99565 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/10_minutes_array_graph.png
+-rw-r--r--   0 james      (501) staff       (20)    22442 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/10_minutes_bag_graph.png
+-rw-r--r--   0 james      (501) staff       (20)    56229 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/10_minutes_dataframe_graph.png
+-rw-r--r--   0 james      (501) staff       (20)     4059 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/HHMI_Janelia_Color.png
+-rw-r--r--   0 james      (501) staff       (20)    18406 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/images/array.svg
+-rw-r--r--   0 james      (501) staff       (20)  1620104 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/async-embarrassing.gif
+-rw-r--r--   0 james      (501) staff       (20)    10752 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/concurrent-futures-threaded.webp
+-rw-r--r--   0 james      (501) staff       (20)   135129 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/crosstalk.svg
+-rw-r--r--   0 james      (501) staff       (20)  2367087 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_jupyterlab.png
+-rw-r--r--   0 james      (501) staff       (20)    37971 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_link.png
+-rw-r--r--   0 james      (501) staff       (20)    68712 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_memory.png
+-rw-r--r--   0 james      (501) staff       (20)   281018 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_memory_new.gif
+-rw-r--r--   0 james      (501) staff       (20)    25435 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_progress.png
+-rw-r--r--   0 james      (501) staff       (20)   276928 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_status.png
+-rw-r--r--   0 james      (501) staff       (20)    12009 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_task_processing.png
+-rw-r--r--   0 james      (501) staff       (20)    58238 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_task_stream_unhealthy.png
+-rw-r--r--   0 james      (501) staff       (20)   103654 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dashboard_taskstream_healthy.png
+-rw-r--r--   0 james      (501) staff       (20)   112822 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask-adaptive.svg
+-rw-r--r--   0 james      (501) staff       (20)    14645 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask-array.svg
+-rw-r--r--   0 james      (501) staff       (20)   222084 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask-cluster-manager.svg
+-rw-r--r--   0 james      (501) staff       (20)    18782 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask-dataframe.svg
+-rw-r--r--   0 james      (501) staff       (20)   381903 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask-overview-distributed-callout.svg
+-rw-r--r--   0 james      (501) staff       (20)   357643 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask-overview-schedulers.svg
+-rw-r--r--   0 james      (501) staff       (20)    97471 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask-overview.svg
+-rw-r--r--   0 james      (501) staff       (20)     3022 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_horizontal.svg
+-rw-r--r--   0 james      (501) staff       (20)     3651 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_horizontal_black.svg
+-rw-r--r--   0 james      (501) staff       (20)     3767 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_horizontal_on_blue.svg
+-rw-r--r--   0 james      (501) staff       (20)     3738 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_horizontal_on_pink.svg
+-rw-r--r--   0 james      (501) staff       (20)     3738 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_horizontal_white.svg
+-rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_icon.svg
+-rw-r--r--   0 james      (501) staff       (20)     1571 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_icon_black.svg
+-rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_icon_on_pink.svg
+-rw-r--r--   0 james      (501) staff       (20)     1609 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/dask_icon_white.svg
+-rw-r--r--   0 james      (501) staff       (20)    20216 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/delayed-inc-double-add.svg
+-rw-r--r--   0 james      (501) staff       (20)   104628 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/distributed-overview.svg
+-rw-r--r--   0 james      (501) staff       (20)    18297 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/images/frame-shuffle.svg
+-rw-r--r--   0 james      (501) staff       (20)    22979 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/images/frame-sort.svg
+-rw-r--r--   0 james      (501) staff       (20)    12181 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/images/frame.svg
+-rw-r--r--   0 james      (501) staff       (20)    41828 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/gputester-msg.png
+-rw-r--r--   0 james      (501) staff       (20)   210392 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/growth_of_languages.png
+-rw-r--r--   0 james      (501) staff       (20)   167834 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/growth_of_libraries.png
+-rw-r--r--   0 james      (501) staff       (20)     4097 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/inc-add.svg
+-rw-r--r--   0 james      (501) staff       (20)   123010 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/map-reduce-task-scheduling.svg
+-rw-r--r--   0 james      (501) staff       (20)   482302 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/map_blocks_drop_axis.png
+-rw-r--r--   0 james      (501) staff       (20)   113067 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/merge_chunks.png
+-rw-r--r--   0 james      (501) staff       (20)    63244 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/merge_chunks_false.png
+-rw-r--r--   0 james      (501) staff       (20)    13024 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/optimize_dask1.svg
+-rw-r--r--   0 james      (501) staff       (20)     8803 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/optimize_dask2.svg
+-rw-r--r--   0 james      (501) staff       (20)     5198 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/optimize_dask3.svg
+-rw-r--r--   0 james      (501) staff       (20)     4104 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/optimize_dask4.svg
+-rw-r--r--   0 james      (501) staff       (20)     2738 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/optimize_dask5.svg
+-rw-r--r--   0 james      (501) staff       (20)   292827 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/order-failure.png
+-rw-r--r--   0 james      (501) staff       (20)   239828 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/order-success.png
+-rw-r--r--   0 james      (501) staff       (20)    40833 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/overlap.svg
+-rw-r--r--   0 james      (501) staff       (20)    18785 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/overlapping-blocks.svg
+-rw-r--r--   0 james      (501) staff       (20)     4537 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/overlapping-neighbors.svg
+-rw-r--r--   0 james      (501) staff       (20)    20533 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/pipeline.svg
+-rw-r--r--   0 james      (501) staff       (20)    31576 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/reshape.png
+-rw-r--r--   0 james      (501) staff       (20)    31410 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/reshape_problem.png
+-rw-r--r--   0 james      (501) staff       (20)    33288 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/reshape_rechunked.png
+-rw-r--r--   0 james      (501) staff       (20)    50209 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/images/scaling-edges.png
+-rw-r--r--   0 james      (501) staff       (20)    68476 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/images/scaling-nodes.png
+-rw-r--r--   0 james      (501) staff       (20)    21294 2023-07-17 19:15:13.000000 dask-2023.8.0/docs/source/images/simple-dask.png
+-rw-r--r--   0 james      (501) staff       (20)    27572 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/transpose-hlg-hovertooltip.png
+-rw-r--r--   0 james      (501) staff       (20)    84492 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/transpose-hlg-html-repr.png
+-rw-r--r--   0 james      (501) staff       (20)    39365 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/transpose.svg
+-rw-r--r--   0 james      (501) staff       (20)    22446 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/transpose_opt.svg
+-rw-r--r--   0 james      (501) staff       (20)   115022 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/trivial.svg
+-rw-r--r--   0 james      (501) staff       (20)     2451 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/images/unoverlapping-neighbors.svg
+-rw-r--r--   0 james      (501) staff       (20)     6237 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/index.rst
+-rw-r--r--   0 james      (501) staff       (20)    15235 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/install.rst
+-rw-r--r--   0 james      (501) staff       (20)      341 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/internals.rst
+-rw-r--r--   0 james      (501) staff       (20)      868 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/logos.rst
+-rw-r--r--   0 james      (501) staff       (20)     3573 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/maintainers.rst
+-rw-r--r--   0 james      (501) staff       (20)    12200 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/optimize.rst
+-rw-r--r--   0 james      (501) staff       (20)     7119 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/order.rst
+-rw-r--r--   0 james      (501) staff       (20)     4810 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/phases-of-computation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5089 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/presentations.rst
+-rw-r--r--   0 james      (501) staff       (20)     6010 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/scheduler-overview.rst
+-rw-r--r--   0 james      (501) staff       (20)     4493 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/scheduling-policy.rst
+-rw-r--r--   0 james      (501) staff       (20)    11015 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/scheduling.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-04 18:09:12.093751 dask-2023.8.0/docs/source/scripts/
+-rw-r--r--   0 james      (501) staff       (20)     3294 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/scripts/scheduling.py
+-rw-r--r--   0 james      (501) staff       (20)     6104 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/shared.rst
+-rw-r--r--   0 james      (501) staff       (20)     9342 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/spark.rst
+-rw-r--r--   0 james      (501) staff       (20)     3966 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/spec.rst
+-rw-r--r--   0 james      (501) staff       (20)     4754 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/support.rst
+-rw-r--r--   0 james      (501) staff       (20)     1831 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/understanding-performance.rst
+-rw-r--r--   0 james      (501) staff       (20)    12205 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/user-interfaces.rst
+-rw-r--r--   0 james      (501) staff       (20)    11744 2023-07-17 19:15:27.000000 dask-2023.8.0/docs/source/why.rst
+-rw-r--r--   0 james      (501) staff       (20)     5533 2023-08-04 18:05:51.000000 dask-2023.8.0/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-08-04 18:09:12.094228 dask-2023.8.0/setup.cfg
+-rwxr-xr-x   0 james      (501) staff       (20)      194 2023-07-17 19:15:27.000000 dask-2023.8.0/setup.py
```

### Comparing `dask-2023.7.1/LICENSE.txt` & `dask-2023.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/PKG-INFO` & `dask-2023.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dask
-Version: 2023.7.1
+Version: 2023.8.0
 Summary: Parallel PyData with Task Scheduling
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
-License: BSD
+License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/dask/dask/
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `dask-2023.7.1/README.rst` & `dask-2023.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/conftest.py` & `dask-2023.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/_compatibility.py` & `dask-2023.8.0/dask/_compatibility.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/NUMPY_LICENSE.txt` & `dask-2023.8.0/dask/array/NUMPY_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/__init__.py` & `dask-2023.8.0/dask/array/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/backends.py` & `dask-2023.8.0/dask/array/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/blockwise.py` & `dask-2023.8.0/dask/array/blockwise.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/chunk.py` & `dask-2023.8.0/dask/array/chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/chunk_types.py` & `dask-2023.8.0/dask/array/chunk_types.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/core.py` & `dask-2023.8.0/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/creation.py` & `dask-2023.8.0/dask/array/creation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/cupy_entry_point.py` & `dask-2023.8.0/dask/array/cupy_entry_point.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/dispatch.py` & `dask-2023.8.0/dask/array/dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/einsumfuncs.py` & `dask-2023.8.0/dask/array/einsumfuncs.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/fft.py` & `dask-2023.8.0/dask/array/fft.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/gufunc.py` & `dask-2023.8.0/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/image.py` & `dask-2023.8.0/dask/array/image.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/linalg.py` & `dask-2023.8.0/dask/array/linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/ma.py` & `dask-2023.8.0/dask/array/ma.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/numpy_compat.py` & `dask-2023.8.0/dask/array/numpy_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/optimization.py` & `dask-2023.8.0/dask/array/optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/overlap.py` & `dask-2023.8.0/dask/array/overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/percentile.py` & `dask-2023.8.0/dask/array/percentile.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/random.py` & `dask-2023.8.0/dask/array/random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/rechunk.py` & `dask-2023.8.0/dask/array/rechunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/reductions.py` & `dask-2023.8.0/dask/array/reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/reshape.py` & `dask-2023.8.0/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/routines.py` & `dask-2023.8.0/dask/array/routines.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/slicing.py` & `dask-2023.8.0/dask/array/slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/stats.py` & `dask-2023.8.0/dask/array/stats.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/svg.py` & `dask-2023.8.0/dask/array/svg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_array_core.py` & `dask-2023.8.0/dask/array/tests/test_array_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -4531,20 +4531,20 @@
     with pytest.raises(ValueError) as info:
         normalize_chunks(((np.nan, np.nan), "auto"), (10, 10), limit=10, dtype=np.uint8)
     assert "auto" in str(info.value)
 
 
 def test_pandas_from_dask_array():
     pd = pytest.importorskip("pandas")
-    from dask.dataframe._compat import PANDAS_GT_131
+    from dask.dataframe._compat import PANDAS_GE_131
 
     a = da.ones((12,), chunks=4)
     s = pd.Series(a, index=range(12))
 
-    if not PANDAS_GT_131:
+    if not PANDAS_GE_131:
         # https://github.com/pandas-dev/pandas/issues/38645
         assert s.dtype != a.dtype
     else:
         assert s.dtype == a.dtype
         assert_eq(s.values, a)
```

### Comparing `dask-2023.7.1/dask/array/tests/test_array_function.py` & `dask-2023.8.0/dask/array/tests/test_array_function.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_array_utils.py` & `dask-2023.8.0/dask/array/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_atop.py` & `dask-2023.8.0/dask/array/tests/test_atop.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_chunk.py` & `dask-2023.8.0/dask/array/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_creation.py` & `dask-2023.8.0/dask/array/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_core.py` & `dask-2023.8.0/dask/array/tests/test_cupy_core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_creation.py` & `dask-2023.8.0/dask/array/tests/test_cupy_creation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_gufunc.py` & `dask-2023.8.0/dask/array/tests/test_cupy_gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_linalg.py` & `dask-2023.8.0/dask/array/tests/test_cupy_linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_overlap.py` & `dask-2023.8.0/dask/array/tests/test_cupy_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_percentile.py` & `dask-2023.8.0/dask/array/tests/test_cupy_percentile.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_random.py` & `dask-2023.8.0/dask/array/tests/test_cupy_random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_reductions.py` & `dask-2023.8.0/dask/array/tests/test_cupy_reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_routines.py` & `dask-2023.8.0/dask/array/tests/test_cupy_routines.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_slicing.py` & `dask-2023.8.0/dask/array/tests/test_cupy_slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_cupy_sparse.py` & `dask-2023.8.0/dask/array/tests/test_cupy_sparse.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_dispatch.py` & `dask-2023.8.0/dask/array/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_fft.py` & `dask-2023.8.0/dask/array/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_gufunc.py` & `dask-2023.8.0/dask/array/tests/test_gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_image.py` & `dask-2023.8.0/dask/array/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_linalg.py` & `dask-2023.8.0/dask/array/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_masked.py` & `dask-2023.8.0/dask/array/tests/test_masked.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_numpy_compat.py` & `dask-2023.8.0/dask/array/tests/test_numpy_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_optimization.py` & `dask-2023.8.0/dask/array/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_overlap.py` & `dask-2023.8.0/dask/array/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_percentiles.py` & `dask-2023.8.0/dask/array/tests/test_percentiles.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_random.py` & `dask-2023.8.0/dask/array/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_rechunk.py` & `dask-2023.8.0/dask/array/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_reductions.py` & `dask-2023.8.0/dask/array/tests/test_reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_reshape.py` & `dask-2023.8.0/dask/array/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_routines.py` & `dask-2023.8.0/dask/array/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_slicing.py` & `dask-2023.8.0/dask/array/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_sparse.py` & `dask-2023.8.0/dask/array/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_stats.py` & `dask-2023.8.0/dask/array/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_svg.py` & `dask-2023.8.0/dask/array/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_testing.py` & `dask-2023.8.0/dask/array/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_ufunc.py` & `dask-2023.8.0/dask/array/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_wrap.py` & `dask-2023.8.0/dask/array/tests/test_wrap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tests/test_xarray.py` & `dask-2023.8.0/dask/array/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/tiledb_io.py` & `dask-2023.8.0/dask/array/tiledb_io.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/ufunc.py` & `dask-2023.8.0/dask/array/ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/utils.py` & `dask-2023.8.0/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/array/wrap.py` & `dask-2023.8.0/dask/array/wrap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/backends.py` & `dask-2023.8.0/dask/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/__init__.py` & `dask-2023.8.0/dask/bag/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/avro.py` & `dask-2023.8.0/dask/bag/avro.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/chunk.py` & `dask-2023.8.0/dask/bag/chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/core.py` & `dask-2023.8.0/dask/bag/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/random.py` & `dask-2023.8.0/dask/bag/random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/tests/test_avro.py` & `dask-2023.8.0/dask/bag/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/tests/test_bag.py` & `dask-2023.8.0/dask/bag/tests/test_bag.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/tests/test_random.py` & `dask-2023.8.0/dask/bag/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/tests/test_text.py` & `dask-2023.8.0/dask/bag/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bag/text.py` & `dask-2023.8.0/dask/bag/text.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/base.py` & `dask-2023.8.0/dask/base.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/blockwise.py` & `dask-2023.8.0/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bytes/core.py` & `dask-2023.8.0/dask/bytes/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bytes/tests/test_bytes_utils.py` & `dask-2023.8.0/dask/bytes/tests/test_bytes_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bytes/tests/test_compression.py` & `dask-2023.8.0/dask/bytes/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bytes/tests/test_http.py` & `dask-2023.8.0/dask/bytes/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bytes/tests/test_local.py` & `dask-2023.8.0/dask/bytes/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/bytes/tests/test_s3.py` & `dask-2023.8.0/dask/bytes/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/cache.py` & `dask-2023.8.0/dask/cache.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/callbacks.py` & `dask-2023.8.0/dask/callbacks.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/cli.py` & `dask-2023.8.0/dask/cli.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/compatibility.py` & `dask-2023.8.0/dask/compatibility.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/config.py` & `dask-2023.8.0/dask/config.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/context.py` & `dask-2023.8.0/dask/context.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/core.py` & `dask-2023.8.0/dask/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dask-schema.yaml` & `dask-2023.8.0/dask/dask-schema.yaml`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dask.yaml` & `dask-2023.8.0/dask/dask.yaml`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/__init__.py` & `dask-2023.8.0/dask/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/_compat.py` & `dask-2023.8.0/dask/dataframe/_compat.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import warnings
 
 import numpy as np
 import pandas as pd
 from packaging.version import Version
 
 PANDAS_VERSION = Version(pd.__version__)
-PANDAS_GT_131 = PANDAS_VERSION >= Version("1.3.1")
-PANDAS_GT_133 = PANDAS_VERSION >= Version("1.3.3")
-PANDAS_GT_140 = PANDAS_VERSION >= Version("1.4.0")
-PANDAS_GT_150 = PANDAS_VERSION >= Version("1.5.0")
-PANDAS_GT_200 = PANDAS_VERSION.major >= 2
-PANDAS_GT_201 = PANDAS_VERSION.release >= (2, 0, 1)
-PANDAS_GT_202 = PANDAS_VERSION.release >= (2, 0, 2)
-PANDAS_GT_210 = PANDAS_VERSION.release >= (2, 1, 0)
+PANDAS_GE_131 = PANDAS_VERSION >= Version("1.3.1")
+PANDAS_GE_133 = PANDAS_VERSION >= Version("1.3.3")
+PANDAS_GE_140 = PANDAS_VERSION >= Version("1.4.0")
+PANDAS_GE_150 = PANDAS_VERSION >= Version("1.5.0")
+PANDAS_GE_200 = PANDAS_VERSION.major >= 2
+PANDAS_GE_201 = PANDAS_VERSION.release >= (2, 0, 1)
+PANDAS_GE_202 = PANDAS_VERSION.release >= (2, 0, 2)
+PANDAS_GE_210 = PANDAS_VERSION.release >= (2, 1, 0)
 
 import pandas.testing as tm
 
 
 def assert_categorical_equal(left, right, *args, **kwargs):
     tm.assert_extension_array_equal(left, right, *args, **kwargs)
     assert isinstance(
@@ -83,169 +83,169 @@
     )
     return df
 
 
 @contextlib.contextmanager
 def check_numeric_only_deprecation(name=None, show_nuisance_warning: bool = False):
     supported_funcs = ["sum", "median", "prod", "min", "max", "std", "var", "quantile"]
-    if name not in supported_funcs and PANDAS_GT_150 and not PANDAS_GT_200:
+    if name not in supported_funcs and PANDAS_GE_150 and not PANDAS_GE_200:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="The default value of numeric_only",
                 category=FutureWarning,
             )
             yield
     elif (
-        not show_nuisance_warning and name not in supported_funcs and not PANDAS_GT_150
+        not show_nuisance_warning and name not in supported_funcs and not PANDAS_GE_150
     ):
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="Dropping of nuisance columns in DataFrame",
                 category=FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_nuisance_columns_warning():
-    if not PANDAS_GT_150:
+    if not PANDAS_GE_150:
         with warnings.catch_warnings(record=True):
             warnings.filterwarnings(
                 "ignore", "Dropping of nuisance columns", FutureWarning
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_groupby_axis_deprecation():
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 ".*Call without passing 'axis' instead|.*Operate on the un-grouped DataFrame instead",
                 FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_observed_deprecation():
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="The default of observed=False",
                 category=FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_axis_keyword_deprecation():
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="The 'axis' keyword|Support for axis",
                 category=FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_convert_dtype_deprecation():
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="the convert_dtype parameter",
                 category=FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_to_pydatetime_deprecation(catch_deprecation_warnings: bool):
-    if PANDAS_GT_210 and catch_deprecation_warnings:
+    if PANDAS_GE_210 and catch_deprecation_warnings:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message=".*DatetimeProperties.to_pydatetime is deprecated",
                 category=FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_apply_dataframe_deprecation():
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="Returning a DataFrame",
                 category=FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_applymap_dataframe_deprecation():
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="DataFrame.applymap has been deprecated",
                 category=FutureWarning,
             )
             yield
     else:
         yield
 
 
 @contextlib.contextmanager
 def check_reductions_runtime_warning():
-    if PANDAS_GT_200 and not PANDAS_GT_201:
+    if PANDAS_GE_200 and not PANDAS_GE_201:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 message="invalid value encountered in double_scalars|Degrees of freedom <= 0 for slice",
                 category=RuntimeWarning,
             )
             yield
     else:
         yield
 
 
-if PANDAS_GT_150:
+if PANDAS_GE_150:
     IndexingError = pd.errors.IndexingError
 else:
     IndexingError = pd.core.indexing.IndexingError
 
 
 def is_any_real_numeric_dtype(arr_or_dtype) -> bool:
     try:
-        # `is_any_real_numeric_dtype` was added in PANDAS_GT_200.
+        # `is_any_real_numeric_dtype` was added in PANDAS_GE_200.
         # We can remove this compatibility utility once we only support `pandas>=2.0`
         return pd.api.types.is_any_real_numeric_dtype(arr_or_dtype)
     except AttributeError:
         from pandas.api.types import is_bool_dtype, is_complex_dtype, is_numeric_dtype
 
         return (
             is_numeric_dtype(arr_or_dtype)
@@ -258,10 +258,10 @@
     # is_string_dtype did not recognize pyarrow strings before 2.0
     # Can remove once 2.0 is minimum version for us
     if hasattr(arr_or_dtype, "dtype"):
         dtype = arr_or_dtype.dtype
     else:
         dtype = arr_or_dtype
 
-    if not PANDAS_GT_200:
+    if not PANDAS_GE_200:
         return pd.api.types.is_dtype_equal(dtype, "string")
     return pd.api.types.is_string_dtype(dtype)
```

### Comparing `dask-2023.7.1/dask/dataframe/_dtypes.py` & `dask-2023.8.0/dask/dataframe/_dtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from datetime import date, time
 from decimal import Decimal
 
 import pandas as pd
 
-from dask.dataframe._compat import PANDAS_GT_150
+from dask.dataframe._compat import PANDAS_GE_150
 from dask.dataframe.extensions import make_array_nonempty, make_scalar
 
 
 @make_array_nonempty.register(pd.DatetimeTZDtype)
 def _(dtype):
     return pd.array([pd.Timestamp(1), pd.NaT], dtype=dtype)
 
@@ -20,15 +20,15 @@
 
 
 @make_array_nonempty.register(pd.StringDtype)
 def _(dtype):
     return pd.array(["a", pd.NA], dtype=dtype)
 
 
-if PANDAS_GT_150:
+if PANDAS_GE_150:
 
     @make_array_nonempty.register(pd.ArrowDtype)
     def _make_array_nonempty_pyarrow_dtype(dtype):
         import pyarrow as pa
 
         if pa.types.is_integer(dtype.pyarrow_dtype):
             data = [1, 2]
```

### Comparing `dask-2023.7.1/dask/dataframe/_pyarrow.py` & `dask-2023.8.0/dask/dataframe/_pyarrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 from functools import partial
 
 import pandas as pd
 from packaging.version import Version
 
-from dask.dataframe._compat import PANDAS_GT_150, PANDAS_GT_200
+from dask.dataframe._compat import PANDAS_GE_150, PANDAS_GE_200
 from dask.dataframe.utils import is_dataframe_like, is_index_like, is_series_like
 
 try:
     import pyarrow as pa
 except ImportError:
     pa = None
 
 
 def is_pyarrow_string_dtype(dtype):
     """Is the input dtype a pyarrow string?"""
     if pa is None:
         return False
 
-    if PANDAS_GT_150:
+    if PANDAS_GE_150:
         pa_string_types = [pd.StringDtype("pyarrow"), pd.ArrowDtype(pa.string())]
     else:
         pa_string_types = [pd.StringDtype("pyarrow")]
     return dtype in pa_string_types
 
 
 def is_object_string_dtype(dtype):
@@ -110,15 +110,15 @@
     index_check=is_pyarrow_string_index,
     string_dtype=object,
 )
 
 
 def check_pyarrow_string_supported():
     """Make sure we have all the required versions"""
-    if not PANDAS_GT_200:
+    if not PANDAS_GE_200:
         raise RuntimeError(
             "Using dask's `dataframe.convert-string` configuration "
             "option requires `pandas>=2.0` to be installed."
         )
     if pa is None or Version(pa.__version__) < Version("12.0.0"):
         raise RuntimeError(
             "Using dask's `dataframe.convert-string` configuration "
```

### Comparing `dask-2023.7.1/dask/dataframe/_pyarrow_compat.py` & `dask-2023.8.0/dask/dataframe/_pyarrow_compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 
 try:
     import pyarrow as pa
 except ImportError:
     pa = None
 
-from dask.dataframe._compat import PANDAS_GT_150, PANDAS_GT_200
+from dask.dataframe._compat import PANDAS_GE_150, PANDAS_GE_200
 
 # Pickling of pyarrow arrays is effectively broken - pickling a slice of an
 # array ends up pickling the entire backing array.
 #
 # See https://issues.apache.org/jira/browse/ARROW-10739
 #
 # This comes up when using pandas `string[pyarrow]` dtypes, which are backed by
@@ -35,15 +35,15 @@
 def reduce_arrowextensionarray(x):
     return (rebuild_arrowextensionarray, (type(x), x._data.combine_chunks()))
 
 
 # `pandas=2` includes efficient serialization of `pyarrow`-backed extension arrays.
 # See https://github.com/pandas-dev/pandas/pull/49078 for details.
 # We only need to backport efficient serialization for `pandas<2`.
-if pa is not None and not PANDAS_GT_200:
-    if PANDAS_GT_150:
+if pa is not None and not PANDAS_GE_200:
+    if PANDAS_GE_150:
         # Applies to all `pyarrow`-backed extension arrays (e.g. `string[pyarrow]`, `int64[pyarrow]`)
         for type_ in [pd.arrays.ArrowExtensionArray, pd.arrays.ArrowStringArray]:
             copyreg.dispatch_table[type_] = reduce_arrowextensionarray
     else:
         # Only `string[pyarrow]` is implemented, so just patch that
         copyreg.dispatch_table[pd.arrays.ArrowStringArray] = reduce_arrowextensionarray
```

### Comparing `dask-2023.7.1/dask/dataframe/accessor.py` & `dask-2023.8.0/dask/dataframe/accessor.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/backends.py` & `dask-2023.8.0/dask/dataframe/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/categorical.py` & `dask-2023.8.0/dask/dataframe/categorical.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/core.py` & `dask-2023.8.0/dask/dataframe/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,18 +60,18 @@
 000003b0: 6b2e 636f 6e74 6578 7420 696d 706f 7274  k.context import
 000003c0: 2067 6c6f 6261 6c6d 6574 686f 640a 6672   globalmethod.fr
 000003d0: 6f6d 2064 6173 6b2e 6461 7461 6672 616d  om dask.datafram
 000003e0: 6520 696d 706f 7274 206d 6574 686f 6473  e import methods
 000003f0: 0a66 726f 6d20 6461 736b 2e64 6174 6166  .from dask.dataf
 00000400: 7261 6d65 2e5f 636f 6d70 6174 2069 6d70  rame._compat imp
 00000410: 6f72 7420 280a 2020 2020 5041 4e44 4153  ort (.    PANDAS
-00000420: 5f47 545f 3134 302c 0a20 2020 2050 414e  _GT_140,.    PAN
-00000430: 4441 535f 4754 5f31 3530 2c0a 2020 2020  DAS_GT_150,.    
-00000440: 5041 4e44 4153 5f47 545f 3230 302c 0a20  PANDAS_GT_200,. 
-00000450: 2020 2050 414e 4441 535f 4754 5f32 3130     PANDAS_GT_210
+00000420: 5f47 455f 3134 302c 0a20 2020 2050 414e  _GE_140,.    PAN
+00000430: 4441 535f 4745 5f31 3530 2c0a 2020 2020  DAS_GE_150,.    
+00000440: 5041 4e44 4153 5f47 455f 3230 302c 0a20  PANDAS_GE_200,. 
+00000450: 2020 2050 414e 4441 535f 4745 5f32 3130     PANDAS_GE_210
 00000460: 2c0a 2020 2020 5041 4e44 4153 5f56 4552  ,.    PANDAS_VER
 00000470: 5349 4f4e 2c0a 2020 2020 6368 6563 6b5f  SION,.    check_
 00000480: 636f 6e76 6572 745f 6474 7970 655f 6465  convert_dtype_de
 00000490: 7072 6563 6174 696f 6e2c 0a20 2020 2063  precation,.    c
 000004a0: 6865 636b 5f6e 7569 7361 6e63 655f 636f  heck_nuisance_co
 000004b0: 6c75 6d6e 735f 7761 726e 696e 672c 0a20  lumns_warning,. 
 000004c0: 2020 2063 6865 636b 5f6e 756d 6572 6963     check_numeric
@@ -173,16 +173,16 @@
 00000ac0: 2274 6872 6561 6473 222c 206e 616d 6564  "threads", named
 00000ad0: 5f73 6368 6564 756c 6572 735b 2273 796e  _schedulers["syn
 00000ae0: 6322 5d29 0a0a 6e6f 5f64 6566 6175 6c74  c"])..no_default
 00000af0: 203d 2022 5f5f 6e6f 5f64 6566 6175 6c74   = "__no_default
 00000b00: 5f5f 220a 0a47 524f 5550 5f4b 4559 535f  __"..GROUP_KEYS_
 00000b10: 4445 4641 554c 543a 2062 6f6f 6c20 7c20  DEFAULT: bool | 
 00000b20: 4e6f 6e65 203d 2054 7275 650a 6966 2050  None = True.if P
-00000b30: 414e 4441 535f 4754 5f31 3530 2061 6e64  ANDAS_GT_150 and
-00000b40: 206e 6f74 2050 414e 4441 535f 4754 5f32   not PANDAS_GT_2
+00000b30: 414e 4441 535f 4745 5f31 3530 2061 6e64  ANDAS_GE_150 and
+00000b40: 206e 6f74 2050 414e 4441 535f 4745 5f32   not PANDAS_GE_2
 00000b50: 3030 3a0a 2020 2020 4752 4f55 505f 4b45  00:.    GROUP_KE
 00000b60: 5953 5f44 4546 4155 4c54 203d 204e 6f6e  YS_DEFAULT = Non
 00000b70: 650a 0a70 642e 7365 745f 6f70 7469 6f6e  e..pd.set_option
 00000b80: 2822 636f 6d70 7574 652e 7573 655f 6e75  ("compute.use_nu
 00000b90: 6d65 7870 7222 2c20 4661 6c73 6529 0a0a  mexpr", False)..
 00000ba0: 0a64 6566 205f 6e75 6d65 7269 635f 6f6e  .def _numeric_on
 00000bb0: 6c79 2866 756e 6329 3a0a 2020 2020 2222  ly(func):.    ""
@@ -269,15 +269,15 @@
 000010c0: 6620 6973 5f64 6174 6166 7261 6d65 5f6c  f is_dataframe_l
 000010d0: 696b 6528 6466 293a 0a20 2020 2020 2020  ike(df):.       
 000010e0: 2077 6172 6e5f 6e75 6d65 7269 635f 6f6e   warn_numeric_on
 000010f0: 6c79 203d 2046 616c 7365 0a20 2020 2020  ly = False.     
 00001100: 2020 2069 6620 6e75 6d65 7269 635f 6f6e     if numeric_on
 00001110: 6c79 2069 7320 6e6f 5f64 6566 6175 6c74  ly is no_default
 00001120: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00001130: 2050 414e 4441 535f 4754 5f32 3030 3a0a   PANDAS_GT_200:.
+00001130: 2050 414e 4441 535f 4745 5f32 3030 3a0a   PANDAS_GE_200:.
 00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001150: 6e75 6d65 7269 635f 6f6e 6c79 203d 2046  numeric_only = F
 00001160: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
 00001170: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
 00001180: 2020 2020 2020 2077 6172 6e5f 6e75 6d65         warn_nume
 00001190: 7269 635f 6f6e 6c79 203d 2054 7275 650a  ric_only = True.
 000011a0: 0a20 2020 2020 2020 206e 756d 6572 6963  .        numeric
@@ -850,15 +850,15 @@
 00003510: 6374 7320 746f 2070 7961 7272 6f77 2073  cts to pyarrow s
 00003520: 7472 696e 6773 2077 6865 7265 206f 6e6c  trings where onl
 00003530: 7920 7468 6520 696e 6465 780a 2020 2020  y the index.    
 00003540: 2020 2020 2020 2020 2020 2020 2320 636f              # co
 00003550: 6e74 6169 6e73 206e 6f6e 2d70 7961 7272  ntains non-pyarr
 00003560: 6f77 2073 7472 696e 6720 6461 7461 2e0a  ow string data..
 00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 6966 206e 6f74 2050 414e 4441 535f 4754  if not PANDAS_GT
+00003580: 6966 206e 6f74 2050 414e 4441 535f 4745  if not PANDAS_GE
 00003590: 5f31 3430 2061 6e64 2028 0a20 2020 2020  _140 and (.     
 000035a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
 000035b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000035c0: 2020 2020 2020 2020 2069 735f 6f62 6a65           is_obje
 000035d0: 6374 5f73 7472 696e 675f 6461 7461 6672  ct_string_datafr
 000035e0: 616d 6528 6d65 7461 290a 2020 2020 2020  ame(meta).      
 000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -4108,15 +4108,15 @@
 000100b0: 7329 0a0a 2020 2020 4064 6572 6976 6564  s)..    @derived
 000100c0: 5f66 726f 6d28 7064 2e44 6174 6146 7261  _from(pd.DataFra
 000100d0: 6d65 290a 2020 2020 6465 6620 7265 706c  me).    def repl
 000100e0: 6163 6528 7365 6c66 2c20 746f 5f72 6570  ace(self, to_rep
 000100f0: 6c61 6365 3d4e 6f6e 652c 2076 616c 7565  lace=None, value
 00010100: 3d4e 6f6e 652c 2072 6567 6578 3d46 616c  =None, regex=Fal
 00010110: 7365 293a 0a20 2020 2020 2020 2023 2049  se):.        # I
-00010120: 6e20 5041 4e44 4153 5f47 545f 3134 3020  n PANDAS_GT_140 
+00010120: 6e20 5041 4e44 4153 5f47 455f 3134 3020  n PANDAS_GE_140 
 00010130: 7061 6e64 6173 2073 7461 7274 7320 7573  pandas starts us
 00010140: 696e 6720 6e6f 5f64 6566 6175 6c74 2069  ing no_default i
 00010150: 6e73 7465 6164 206f 6620 4e6f 6e65 0a20  nstead of None. 
 00010160: 2020 2020 2020 2076 616c 7565 5f6b 7761         value_kwa
 00010170: 7267 203d 207b 2276 616c 7565 223a 2076  rg = {"value": v
 00010180: 616c 7565 7d20 6966 2076 616c 7565 2069  alue} if value i
 00010190: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
@@ -4948,17 +4948,17 @@
 00013530: 6620 6d61 7828 7365 6c66 2c20 6178 6973  f max(self, axis
 00013540: 3d30 2c20 736b 6970 6e61 3d54 7275 652c  =0, skipna=True,
 00013550: 2073 706c 6974 5f65 7665 7279 3d46 616c   split_every=Fal
 00013560: 7365 2c20 6f75 743d 4e6f 6e65 2c20 6e75  se, out=None, nu
 00013570: 6d65 7269 635f 6f6e 6c79 3d4e 6f6e 6529  meric_only=None)
 00013580: 3a0a 2020 2020 2020 2020 6966 2028 0a20  :.        if (. 
 00013590: 2020 2020 2020 2020 2020 2050 414e 4441             PANDA
-000135a0: 535f 4754 5f31 3430 0a20 2020 2020 2020  S_GT_140.       
+000135a0: 535f 4745 5f31 3430 0a20 2020 2020 2020  S_GE_140.       
 000135b0: 2020 2020 2061 6e64 206e 6f74 2050 414e       and not PAN
-000135c0: 4441 535f 4754 5f32 3030 0a20 2020 2020  DAS_GT_200.     
+000135c0: 4441 535f 4745 5f32 3030 0a20 2020 2020  DAS_GE_200.     
 000135d0: 2020 2020 2020 2061 6e64 2061 7869 7320         and axis 
 000135e0: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
 000135f0: 2020 2020 616e 6420 6973 696e 7374 616e      and isinstan
 00013600: 6365 2873 656c 662c 2044 6174 6146 7261  ce(self, DataFra
 00013610: 6d65 290a 2020 2020 2020 2020 293a 0a20  me).        ):. 
 00013620: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
 00013630: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
@@ -4993,30 +4993,30 @@
 00013800: 5374 6172 7469 6e67 2069 6e20 7061 6e64  Starting in pand
 00013810: 6173 2032 2e30 2c20 6061 7869 733d 4e6f  as 2.0, `axis=No
 00013820: 6e65 6020 646f 6573 2061 2066 756c 6c20  ne` does a full 
 00013830: 6167 6772 6567 6174 696f 6e20 6163 726f  aggregation acro
 00013840: 7373 2062 6f74 6820 6178 6573 0a20 2020  ss both axes.   
 00013850: 2020 2020 2020 2020 206e 6f6e 655f 6973           none_is
 00013860: 5f7a 6572 6f3d 6e6f 7420 5041 4e44 4153  _zero=not PANDAS
-00013870: 5f47 545f 3230 302c 0a20 2020 2020 2020  _GT_200,.       
+00013870: 5f47 455f 3230 302c 0a20 2020 2020 2020  _GE_200,.       
 00013880: 2020 2020 206e 756d 6572 6963 5f6f 6e6c       numeric_onl
 00013890: 793d 6e75 6d65 7269 635f 6f6e 6c79 2c0a  y=numeric_only,.
 000138a0: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
 000138b0: 6465 7269 7665 645f 6672 6f6d 2870 642e  derived_from(pd.
 000138c0: 4461 7461 4672 616d 6529 0a20 2020 2064  DataFrame).    d
 000138d0: 6566 206d 696e 2873 656c 662c 2061 7869  ef min(self, axi
 000138e0: 733d 302c 2073 6b69 706e 613d 5472 7565  s=0, skipna=True
 000138f0: 2c20 7370 6c69 745f 6576 6572 793d 4661  , split_every=Fa
 00013900: 6c73 652c 206f 7574 3d4e 6f6e 652c 206e  lse, out=None, n
 00013910: 756d 6572 6963 5f6f 6e6c 793d 4e6f 6e65  umeric_only=None
 00013920: 293a 0a20 2020 2020 2020 2069 6620 280a  ):.        if (.
 00013930: 2020 2020 2020 2020 2020 2020 5041 4e44              PAND
-00013940: 4153 5f47 545f 3134 300a 2020 2020 2020  AS_GT_140.      
+00013940: 4153 5f47 455f 3134 300a 2020 2020 2020  AS_GE_140.      
 00013950: 2020 2020 2020 616e 6420 6e6f 7420 5041        and not PA
-00013960: 4e44 4153 5f47 545f 3230 300a 2020 2020  NDAS_GT_200.    
+00013960: 4e44 4153 5f47 455f 3230 300a 2020 2020  NDAS_GE_200.    
 00013970: 2020 2020 2020 2020 616e 6420 6178 6973          and axis
 00013980: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
 00013990: 2020 2020 2061 6e64 2069 7369 6e73 7461       and isinsta
 000139a0: 6e63 6528 7365 6c66 2c20 4461 7461 4672  nce(self, DataFr
 000139b0: 616d 6529 0a20 2020 2020 2020 2029 3a0a  ame).        ):.
 000139c0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
 000139d0: 696e 6773 2e77 6172 6e28 0a20 2020 2020  ings.warn(.     
@@ -5051,15 +5051,15 @@
 00013ba0: 2053 7461 7274 696e 6720 696e 2070 616e   Starting in pan
 00013bb0: 6461 7320 322e 302c 2060 6178 6973 3d4e  das 2.0, `axis=N
 00013bc0: 6f6e 6560 2064 6f65 7320 6120 6675 6c6c  one` does a full
 00013bd0: 2061 6767 7265 6761 7469 6f6e 2061 6372   aggregation acr
 00013be0: 6f73 7320 626f 7468 2061 7865 730a 2020  oss both axes.  
 00013bf0: 2020 2020 2020 2020 2020 6e6f 6e65 5f69            none_i
 00013c00: 735f 7a65 726f 3d6e 6f74 2050 414e 4441  s_zero=not PANDA
-00013c10: 535f 4754 5f32 3030 2c0a 2020 2020 2020  S_GT_200,.      
+00013c10: 535f 4745 5f32 3030 2c0a 2020 2020 2020  S_GE_200,.      
 00013c20: 2020 2020 2020 6e75 6d65 7269 635f 6f6e        numeric_on
 00013c30: 6c79 3d6e 756d 6572 6963 5f6f 6e6c 792c  ly=numeric_only,
 00013c40: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
 00013c50: 4064 6572 6976 6564 5f66 726f 6d28 7064  @derived_from(pd
 00013c60: 2e44 6174 6146 7261 6d65 290a 2020 2020  .DataFrame).    
 00013c70: 6465 6620 6964 786d 6178 280a 2020 2020  def idxmax(.    
 00013c80: 2020 2020 7365 6c66 2c20 6178 6973 3d4e      self, axis=N
@@ -5354,17 +5354,17 @@
 00014e90: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
 00014ea0: 6474 7970 653d 4e6f 6e65 2c0a 2020 2020  dtype=None,.    
 00014eb0: 2020 2020 6f75 743d 4e6f 6e65 2c0a 2020      out=None,.  
 00014ec0: 2020 2020 2020 6e75 6d65 7269 635f 6f6e        numeric_on
 00014ed0: 6c79 3d4e 6f6e 652c 0a20 2020 2029 3a0a  ly=None,.    ):.
 00014ee0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
 00014ef0: 2020 2020 2020 2020 2050 414e 4441 535f           PANDAS_
-00014f00: 4754 5f31 3430 0a20 2020 2020 2020 2020  GT_140.         
+00014f00: 4745 5f31 3430 0a20 2020 2020 2020 2020  GE_140.         
 00014f10: 2020 2061 6e64 206e 6f74 2050 414e 4441     and not PANDA
-00014f20: 535f 4754 5f32 3030 0a20 2020 2020 2020  S_GT_200.       
+00014f20: 535f 4745 5f32 3030 0a20 2020 2020 2020  S_GE_200.       
 00014f30: 2020 2020 2061 6e64 2061 7869 7320 6973       and axis is
 00014f40: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
 00014f50: 2020 616e 6420 6973 696e 7374 616e 6365    and isinstance
 00014f60: 2873 656c 662c 2044 6174 6146 7261 6d65  (self, DataFrame
 00014f70: 290a 2020 2020 2020 2020 293a 0a20 2020  ).        ):.   
 00014f80: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
 00014f90: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
@@ -5383,15 +5383,15 @@
 00015060: 616d 652e 6d65 616e 2829 2722 2c0a 2020  ame.mean()'",.  
 00015070: 2020 2020 2020 2020 2020 2020 2020 4675                Fu
 00015080: 7475 7265 5761 726e 696e 672c 0a20 2020  tureWarning,.   
 00015090: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 000150a0: 2020 2061 7869 7320 3d20 7365 6c66 2e5f     axis = self._
 000150b0: 7661 6c69 6461 7465 5f61 7869 7328 6178  validate_axis(ax
 000150c0: 6973 2c20 6e6f 6e65 5f69 735f 7a65 726f  is, none_is_zero
-000150d0: 3d6e 6f74 2050 414e 4441 535f 4754 5f32  =not PANDAS_GT_2
+000150d0: 3d6e 6f74 2050 414e 4441 535f 4745 5f32  =not PANDAS_GE_2
 000150e0: 3030 290a 2020 2020 2020 2020 5f72 6169  00).        _rai
 000150f0: 7365 5f69 665f 6f62 6a65 6374 5f73 6572  se_if_object_ser
 00015100: 6965 7328 7365 6c66 2c20 226d 6561 6e22  ies(self, "mean"
 00015110: 290a 2020 2020 2020 2020 2320 4e4f 5445  ).        # NOTE
 00015120: 3a20 446f 2077 6520 7761 6e74 2074 6f20  : Do we want to 
 00015130: 7761 726e 2068 6572 653f 0a20 2020 2020  warn here?.     
 00015140: 2020 2077 6974 6820 6368 6563 6b5f 6e75     with check_nu
@@ -5444,15 +5444,15 @@
 00015430: 7279 290a 2020 2020 2020 2020 2020 2020  ry).            
 00015440: 2320 5374 6172 7469 6e67 2069 6e20 7061  # Starting in pa
 00015450: 6e64 6173 2032 2e30 2c20 6061 7869 733d  ndas 2.0, `axis=
 00015460: 4e6f 6e65 6020 646f 6573 2061 2066 756c  None` does a ful
 00015470: 6c20 6167 6772 6567 6174 696f 6e20 6163  l aggregation ac
 00015480: 726f 7373 2062 6f74 6820 6178 6573 0a20  ross both axes. 
 00015490: 2020 2020 2020 2020 2020 2069 6620 5041             if PA
-000154a0: 4e44 4153 5f47 545f 3230 3020 616e 6420  NDAS_GT_200 and 
+000154a0: 4e44 4153 5f47 455f 3230 3020 616e 6420  NDAS_GE_200 and 
 000154b0: 6178 6973 2069 7320 4e6f 6e65 2061 6e64  axis is None and
 000154c0: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
 000154d0: 2c20 4461 7461 4672 616d 6529 3a0a 2020  , DataFrame):.  
 000154e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
 000154f0: 7375 6c74 203d 2073 2e73 756d 2829 202f  sult = s.sum() /
 00015500: 206e 2e73 756d 2829 0a20 2020 2020 2020   n.sum().       
 00015510: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
@@ -6108,15 +6108,15 @@
 00017db0: 7570 706f 7274 2066 696c 7465 7269 6e67  upport filtering
 00017dc0: 206f 7574 204e 614e 0a20 2020 2020 2020   out NaN.       
 00017dd0: 2020 2020 7661 6c75 6573 2c20 7768 6963      values, whic
 00017de0: 6820 6973 2061 6761 696e 2061 2064 6966  h is again a dif
 00017df0: 6665 7265 6e63 6520 746f 2050 616e 6461  ference to Panda
 00017e00: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
 00017e10: 2020 2020 2020 2069 6620 5041 4e44 4153         if PANDAS
-00017e20: 5f47 545f 3230 3020 616e 6420 6178 6973  _GT_200 and axis
+00017e20: 5f47 455f 3230 3020 616e 6420 6178 6973  _GE_200 and axis
 00017e30: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
 00017e40: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
 00017e50: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
 00017e60: 2020 2020 2020 2020 2260 6178 6973 3d4e          "`axis=N
 00017e70: 6f6e 6560 2069 736e 2774 2063 7572 7265  one` isn't curre
 00017e80: 6e74 6c79 2073 7570 706f 7274 6564 2066  ntly supported f
 00017e90: 6f72 2060 736b 6577 6020 7768 656e 2075  or `skew` when u
@@ -6383,15 +6383,15 @@
 00018ee0: 6573 206e 6f74 2073 7570 706f 7274 2066  es not support f
 00018ef0: 696c 7465 7269 6e67 206f 7574 204e 614e  iltering out NaN
 00018f00: 0a20 2020 2020 2020 2020 2020 7661 6c75  .           valu
 00018f10: 6573 2c20 7768 6963 6820 6973 2061 6761  es, which is aga
 00018f20: 696e 2061 2064 6966 6665 7265 6e63 6520  in a difference 
 00018f30: 746f 2050 616e 6461 732e 0a20 2020 2020  to Pandas..     
 00018f40: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00018f50: 6620 5041 4e44 4153 5f47 545f 3230 3020  f PANDAS_GT_200 
+00018f50: 6620 5041 4e44 4153 5f47 455f 3230 3020  f PANDAS_GE_200 
 00018f60: 616e 6420 6178 6973 2069 7320 4e6f 6e65  and axis is None
 00018f70: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
 00018f80: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
 00018f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018fa0: 2260 6178 6973 3d4e 6f6e 6560 2069 736e  "`axis=None` isn
 00018fb0: 2774 2063 7572 7265 6e74 6c79 2073 7570  't currently sup
 00018fc0: 706f 7274 6564 2066 6f72 2060 6b75 7274  ported for `kurt
@@ -6838,15 +6838,15 @@
 0001ab50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
 0001ab60: 656c 662e 5f67 6574 5f6e 756d 6572 6963  elf._get_numeric
 0001ab70: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
 0001ab80: 2020 2020 2020 2020 6966 206e 756d 6572          if numer
 0001ab90: 6963 5f6f 6e6c 7920 6973 2054 7275 650a  ic_only is True.
 0001aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001abb0: 6f72 2028 6e6f 7420 5041 4e44 4153 5f47  or (not PANDAS_G
-0001abc0: 545f 3230 3020 616e 6420 6e75 6d65 7269  T_200 and numeri
+0001abc0: 455f 3230 3020 616e 6420 6e75 6d65 7269  E_200 and numeri
 0001abd0: 635f 6f6e 6c79 2069 7320 6e6f 5f64 6566  c_only is no_def
 0001abe0: 6175 6c74 290a 2020 2020 2020 2020 2020  ault).          
 0001abf0: 2020 2020 2020 656c 7365 2073 656c 660a        else self.
 0001ac00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 0001ac10: 2020 2020 2020 2020 2020 7175 616e 7469            quanti
 0001ac20: 6c65 7320 3d20 7475 706c 6528 0a20 2020  les = tuple(.   
 0001ac30: 2020 2020 2020 2020 2020 2020 2071 7561               qua
@@ -6917,15 +6917,15 @@
 0001b040: 6f64 3d22 6465 6661 756c 7422 2c0a 2020  od="default",.  
 0001b050: 2020 2020 2020 696e 636c 7564 653d 4e6f        include=No
 0001b060: 6e65 2c0a 2020 2020 2020 2020 6578 636c  ne,.        excl
 0001b070: 7564 653d 4e6f 6e65 2c0a 2020 2020 2020  ude=None,.      
 0001b080: 2020 6461 7465 7469 6d65 5f69 735f 6e75    datetime_is_nu
 0001b090: 6d65 7269 633d 6e6f 5f64 6566 6175 6c74  meric=no_default
 0001b0a0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0001b0b0: 2069 6620 5041 4e44 4153 5f47 545f 3230   if PANDAS_GT_20
+0001b0b0: 2069 6620 5041 4e44 4153 5f47 455f 3230   if PANDAS_GE_20
 0001b0c0: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
 0001b0d0: 6620 6461 7465 7469 6d65 5f69 735f 6e75  f datetime_is_nu
 0001b0e0: 6d65 7269 6320 6973 206e 6f5f 6465 6661  meric is no_defa
 0001b0f0: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
 0001b100: 2020 2020 2064 6174 6574 696d 655f 6973       datetime_is
 0001b110: 5f6e 756d 6572 6963 203d 2054 7275 650a  _numeric = True.
 0001b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -7444,15 +7444,15 @@
 0001d130: 636f 6c6e 616d 6529 0a20 2020 2020 2020  colname).       
 0001d140: 207d 0a20 2020 2020 2020 2067 7261 7068   }.        graph
 0001d150: 203d 2048 6967 684c 6576 656c 4772 6170   = HighLevelGrap
 0001d160: 682e 6672 6f6d 5f63 6f6c 6c65 6374 696f  h.from_collectio
 0001d170: 6e73 286e 616d 652c 206c 6179 6572 2c20  ns(name, layer, 
 0001d180: 6465 7065 6e64 656e 6369 6573 3d73 7461  dependencies=sta
 0001d190: 7473 290a 0a20 2020 2020 2020 2069 6620  ts)..        if 
-0001d1a0: 6e6f 7420 5041 4e44 4153 5f47 545f 3230  not PANDAS_GT_20
+0001d1a0: 6e6f 7420 5041 4e44 4153 5f47 455f 3230  not PANDAS_GE_20
 0001d1b0: 303a 0a20 2020 2020 2020 2020 2020 2064  0:.            d
 0001d1c0: 6174 6574 696d 655f 6973 5f6e 756d 6572  atetime_is_numer
 0001d1d0: 6963 5f6b 7761 7267 203d 207b 2264 6174  ic_kwarg = {"dat
 0001d1e0: 6574 696d 655f 6973 5f6e 756d 6572 6963  etime_is_numeric
 0001d1f0: 223a 2064 6174 6574 696d 655f 6973 5f6e  ": datetime_is_n
 0001d200: 756d 6572 6963 7d0a 2020 2020 2020 2020  umeric}.        
 0001d210: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
@@ -7920,23 +7920,23 @@
 0001eef0: 6d61 705f 7061 7274 6974 696f 6e73 280a  map_partitions(.
 0001ef00: 2020 2020 2020 2020 2020 2020 4d2e 6173              M.as
 0001ef10: 7479 7065 2c20 6474 7970 653d 6474 7970  type, dtype=dtyp
 0001ef20: 652c 206d 6574 613d 6d65 7461 2c20 656e  e, meta=meta, en
 0001ef30: 666f 7263 655f 6d65 7461 6461 7461 3d46  force_metadata=F
 0001ef40: 616c 7365 0a20 2020 2020 2020 2029 0a0a  alse.        )..
 0001ef50: 2020 2020 6966 206e 6f74 2050 414e 4441      if not PANDA
-0001ef60: 535f 4754 5f32 3030 3a0a 0a20 2020 2020  S_GT_200:..     
+0001ef60: 535f 4745 5f32 3030 3a0a 0a20 2020 2020  S_GE_200:..     
 0001ef70: 2020 2040 6465 7269 7665 645f 6672 6f6d     @derived_from
 0001ef80: 2870 642e 5365 7269 6573 290a 2020 2020  (pd.Series).    
 0001ef90: 2020 2020 6465 6620 6170 7065 6e64 2873      def append(s
 0001efa0: 656c 662c 206f 7468 6572 2c20 696e 7465  elf, other, inte
 0001efb0: 726c 6561 7665 5f70 6172 7469 7469 6f6e  rleave_partition
 0001efc0: 733d 4661 6c73 6529 3a0a 2020 2020 2020  s=False):.      
 0001efd0: 2020 2020 2020 6966 2050 414e 4441 535f        if PANDAS_
-0001efe0: 4754 5f31 3430 3a0a 2020 2020 2020 2020  GT_140:.        
+0001efe0: 4745 5f31 3430 3a0a 2020 2020 2020 2020  GE_140:.        
 0001eff0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
 0001f000: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
 0001f010: 2020 2020 2020 2020 2020 2022 5468 6520             "The 
 0001f020: 6672 616d 652e 6170 7065 6e64 206d 6574  frame.append met
 0001f030: 686f 6420 6973 2064 6570 7265 6361 7465  hod is deprecate
 0001f040: 6420 616e 6420 7769 6c6c 2062 6520 7265  d and will be re
 0001f050: 6d6f 7665 6420 6672 6f6d 220a 2020 2020  moved from".    
@@ -9119,21 +9119,21 @@
 000239e0: 6672 6f6d 2870 642e 4461 7461 4672 616d  from(pd.DataFram
 000239f0: 6529 0a20 2020 2064 6566 205f 6765 745f  e).    def _get_
 00023a00: 6e75 6d65 7269 635f 6461 7461 2873 656c  numeric_data(sel
 00023a10: 662c 2068 6f77 3d22 616e 7922 2c20 7375  f, how="any", su
 00023a20: 6273 6574 3d4e 6f6e 6529 3a0a 2020 2020  bset=None):.    
 00023a30: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
 00023a40: 0a20 2020 2069 6620 6e6f 7420 5041 4e44  .    if not PAND
-00023a50: 4153 5f47 545f 3230 303a 0a0a 2020 2020  AS_GT_200:..    
+00023a50: 4153 5f47 455f 3230 303a 0a0a 2020 2020  AS_GE_200:..    
 00023a60: 2020 2020 4064 6572 6976 6564 5f66 726f      @derived_fro
 00023a70: 6d28 7064 2e53 6572 6965 7329 0a20 2020  m(pd.Series).   
 00023a80: 2020 2020 2064 6566 2069 7465 7269 7465       def iterite
 00023a90: 6d73 2873 656c 6629 3a0a 2020 2020 2020  ms(self):.      
 00023aa0: 2020 2020 2020 6966 2050 414e 4441 535f        if PANDAS_
-00023ab0: 4754 5f31 3530 3a0a 2020 2020 2020 2020  GT_150:.        
+00023ab0: 4745 5f31 3530 3a0a 2020 2020 2020 2020  GE_150:.        
 00023ac0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
 00023ad0: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
 00023ae0: 2020 2020 2020 2020 2020 2022 6974 6572             "iter
 00023af0: 6974 656d 7320 6973 2064 6570 7265 6361  items is depreca
 00023b00: 7465 6420 616e 6420 7769 6c6c 2062 6520  ted and will be 
 00023b10: 7265 6d6f 7665 6420 696e 2061 2066 7574  removed in a fut
 00023b20: 7572 6520 7665 7273 696f 6e2e 2022 0a20  ure version. ". 
@@ -9863,15 +9863,15 @@
 00026860: 756e 632c 2061 7267 733d 6172 6773 2c20  unc, args=args, 
 00026870: 7564 663d 5472 7565 2c20 2a2a 6b77 6473  udf=True, **kwds
 00026880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00026890: 2029 0a20 2020 2020 2020 2020 2020 2077   ).            w
 000268a0: 6172 6e69 6e67 732e 7761 726e 286d 6574  arnings.warn(met
 000268b0: 615f 7761 726e 696e 6728 6d65 7461 2929  a_warning(meta))
 000268c0: 0a20 2020 2020 2020 2065 6c69 6620 5041  .        elif PA
-000268d0: 4e44 4153 5f47 545f 3231 303a 0a20 2020  NDAS_GT_210:.   
+000268d0: 4e44 4153 5f47 455f 3231 303a 0a20 2020  NDAS_GE_210:.   
 000268e0: 2020 2020 2020 2020 2074 6573 745f 6d65           test_me
 000268f0: 7461 203d 206d 616b 655f 6d65 7461 286d  ta = make_meta(m
 00026900: 6574 6129 0a20 2020 2020 2020 2020 2020  eta).           
 00026910: 2069 6620 6973 5f64 6174 6166 7261 6d65   if is_dataframe
 00026920: 5f6c 696b 6528 7465 7374 5f6d 6574 6129  _like(test_meta)
 00026930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00026940: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
@@ -10011,22 +10011,22 @@
 000271a0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
 000271b0: 2072 6573 3120 3d20 6f74 6865 7220 2f2f   res1 = other //
 000271c0: 2073 656c 660a 2020 2020 2020 2020 7265   self.        re
 000271d0: 7332 203d 206f 7468 6572 2025 2073 656c  s2 = other % sel
 000271e0: 660a 2020 2020 2020 2020 7265 7475 726e  f.        return
 000271f0: 2072 6573 312c 2072 6573 320a 0a20 2020   res1, res2..   
 00027200: 2069 6620 6e6f 7420 5041 4e44 4153 5f47   if not PANDAS_G
-00027210: 545f 3230 303a 0a0a 2020 2020 2020 2020  T_200:..        
+00027210: 455f 3230 303a 0a0a 2020 2020 2020 2020  E_200:..        
 00027220: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
 00027230: 2020 4064 6572 6976 6564 5f66 726f 6d28    @derived_from(
 00027240: 7064 2e53 6572 6965 7329 0a20 2020 2020  pd.Series).     
 00027250: 2020 2064 6566 2069 735f 6d6f 6e6f 746f     def is_monoto
 00027260: 6e69 6328 7365 6c66 293a 0a20 2020 2020  nic(self):.     
 00027270: 2020 2020 2020 2069 6620 5041 4e44 4153         if PANDAS
-00027280: 5f47 545f 3135 303a 0a20 2020 2020 2020  _GT_150:.       
+00027280: 5f47 455f 3135 303a 0a20 2020 2020 2020  _GE_150:.       
 00027290: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
 000272a0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
 000272b0: 2020 2020 2020 2020 2020 2020 2269 735f              "is_
 000272c0: 6d6f 6e6f 746f 6e69 6320 6973 2064 6570  monotonic is dep
 000272d0: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
 000272e0: 2062 6520 7265 6d6f 7665 6420 696e 2061   be removed in a
 000272f0: 2066 7574 7572 6520 7665 7273 696f 6e2e   future version.
@@ -10437,22 +10437,22 @@
 00028c40: 6e29 0a20 2020 2020 2020 2020 2020 2029  n).            )
 00028c50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
 00028c60: 2020 2020 2020 2020 2020 2061 7070 6c69             appli
 00028c70: 6564 203d 2061 7070 6c69 6564 2e63 6c65  ed = applied.cle
 00028c80: 6172 5f64 6976 6973 696f 6e73 2829 0a20  ar_divisions(). 
 00028c90: 2020 2020 2020 2072 6574 7572 6e20 6170         return ap
 00028ca0: 706c 6965 640a 0a20 2020 2069 6620 6e6f  plied..    if no
-00028cb0: 7420 5041 4e44 4153 5f47 545f 3230 303a  t PANDAS_GT_200:
+00028cb0: 7420 5041 4e44 4153 5f47 455f 3230 303a  t PANDAS_GE_200:
 00028cc0: 0a0a 2020 2020 2020 2020 4070 726f 7065  ..        @prope
 00028cd0: 7274 790a 2020 2020 2020 2020 4064 6572  rty.        @der
 00028ce0: 6976 6564 5f66 726f 6d28 7064 2e49 6e64  ived_from(pd.Ind
 00028cf0: 6578 290a 2020 2020 2020 2020 6465 6620  ex).        def 
 00028d00: 6973 5f6d 6f6e 6f74 6f6e 6963 2873 656c  is_monotonic(sel
 00028d10: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-00028d20: 6966 2050 414e 4441 535f 4754 5f31 3530  if PANDAS_GT_150
+00028d20: 6966 2050 414e 4441 535f 4745 5f31 3530  if PANDAS_GE_150
 00028d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00028d40: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
 00028d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00028d60: 2020 2020 2022 6973 5f6d 6f6e 6f74 6f6e       "is_monoton
 00028d70: 6963 2069 7320 6465 7072 6563 6174 6564  ic is deprecated
 00028d80: 2061 6e64 2077 696c 6c20 6265 2072 656d   and will be rem
 00028d90: 6f76 6564 2069 6e20 6120 6675 7475 7265  oved in a future
@@ -13099,15 +13099,15 @@
 000332a0: 6666 6978 6573 3d28 6c73 7566 6669 782c  ffixes=(lsuffix,
 000332b0: 2072 7375 6666 6978 292c 0a20 2020 2020   rsuffix),.     
 000332c0: 2020 2020 2020 206e 7061 7274 6974 696f         npartitio
 000332d0: 6e73 3d6e 7061 7274 6974 696f 6e73 2c0a  ns=npartitions,.
 000332e0: 2020 2020 2020 2020 2020 2020 7368 7566              shuf
 000332f0: 666c 653d 7368 7566 666c 652c 0a20 2020  fle=shuffle,.   
 00033300: 2020 2020 2029 0a0a 2020 2020 6966 206e       )..    if n
-00033310: 6f74 2050 414e 4441 535f 4754 5f32 3030  ot PANDAS_GT_200
+00033310: 6f74 2050 414e 4441 535f 4745 5f32 3030  ot PANDAS_GE_200
 00033320: 3a0a 0a20 2020 2020 2020 2040 6465 7269  :..        @deri
 00033330: 7665 645f 6672 6f6d 2870 642e 4461 7461  ved_from(pd.Data
 00033340: 4672 616d 6529 0a20 2020 2020 2020 2064  Frame).        d
 00033350: 6566 2061 7070 656e 6428 7365 6c66 2c20  ef append(self, 
 00033360: 6f74 6865 722c 2069 6e74 6572 6c65 6176  other, interleav
 00033370: 655f 7061 7274 6974 696f 6e73 3d46 616c  e_partitions=Fal
 00033380: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
@@ -13555,15 +13555,15 @@
 00034f20: 6473 2e61 7070 6c79 6d61 702c 2073 656c  ds.applymap, sel
 00034f30: 662c 2066 756e 632c 206d 6574 613d 6d65  f, func, meta=me
 00034f40: 7461 290a 0a20 2020 2064 6566 206d 6170  ta)..    def map
 00034f50: 2873 656c 662c 2066 756e 632c 206d 6574  (self, func, met
 00034f60: 613d 6e6f 5f64 6566 6175 6c74 2c20 6e61  a=no_default, na
 00034f70: 5f61 6374 696f 6e3d 4e6f 6e65 293a 0a20  _action=None):. 
 00034f80: 2020 2020 2020 2069 6620 6e6f 7420 5041         if not PA
-00034f90: 4e44 4153 5f47 545f 3231 303a 0a20 2020  NDAS_GT_210:.   
+00034f90: 4e44 4153 5f47 455f 3231 303a 0a20 2020  NDAS_GE_210:.   
 00034fa0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
 00034fb0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
 00034fc0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
 00034fd0: 2020 2020 6622 4461 7461 4672 616d 652e      f"DataFrame.
 00034fe0: 6d61 7020 7265 7175 6972 6573 2070 616e  map requires pan
 00034ff0: 6461 733e 3d32 2e31 2e30 2c20 6275 7420  das>=2.1.0, but 
 00035000: 7061 6e64 6173 3d7b 5041 4e44 4153 5f56  pandas={PANDAS_V
@@ -13785,15 +13785,15 @@
 00035d80: 782e 5f6d 6574 6129 2e5f 5f6e 616d 655f  x._meta).__name_
 00035d90: 5f7d 3a20 3020 656e 7472 6965 7322 290a  _}: 0 entries").
 00035da0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
 00035db0: 732e 6170 7065 6e64 2866 2245 6d70 7479  s.append(f"Empty
 00035dc0: 207b 7479 7065 2873 656c 6629 2e5f 5f6e   {type(self).__n
 00035dd0: 616d 655f 5f7d 2229 0a20 2020 2020 2020  ame__}").       
 00035de0: 2020 2020 2069 6620 5041 4e44 4153 5f47       if PANDAS_G
-00035df0: 545f 3135 303a 0a20 2020 2020 2020 2020  T_150:.         
+00035df0: 455f 3135 303a 0a20 2020 2020 2020 2020  E_150:.         
 00035e00: 2020 2020 2020 2023 2070 616e 6461 7320         # pandas 
 00035e10: 6461 7461 6672 616d 6520 7374 6172 7465  dataframe starte
 00035e20: 6420 6164 6469 6e67 2061 206e 6577 6c69  d adding a newli
 00035e30: 6e65 2077 6865 6e20 696e 666f 2069 7320  ne when info is 
 00035e40: 6361 6c6c 6564 2e0a 2020 2020 2020 2020  called..        
 00035e50: 2020 2020 2020 2020 6c69 6e65 732e 6170          lines.ap
 00035e60: 7065 6e64 2822 2229 0a20 2020 2020 2020  pend("").       
@@ -16312,19 +16312,19 @@
 0003fb70: 7269 6320 6461 7461 2061 6e64 2061 7373  ric data and ass
 0003fb80: 6f63 6961 7465 6420 6465 7072 6563 6174  ociated deprecat
 0003fb90: 696f 6e20 7761 726e 696e 670a 2020 2020  ion warning.    
 0003fba0: 6d61 7962 655f 7761 726e 203d 2046 616c  maybe_warn = Fal
 0003fbb0: 7365 0a20 2020 2069 6620 6e75 6d65 7269  se.    if numeri
 0003fbc0: 635f 6f6e 6c79 2069 7320 6e6f 5f64 6566  c_only is no_def
 0003fbd0: 6175 6c74 3a0a 2020 2020 2020 2020 6966  ault:.        if
-0003fbe0: 2050 414e 4441 535f 4754 5f32 3030 3a0a   PANDAS_GT_200:.
+0003fbe0: 2050 414e 4441 535f 4745 5f32 3030 3a0a   PANDAS_GE_200:.
 0003fbf0: 2020 2020 2020 2020 2020 2020 6e75 6d65              nume
 0003fc00: 7269 635f 6f6e 6c79 203d 2046 616c 7365  ric_only = False
 0003fc10: 0a20 2020 2020 2020 2065 6c69 6620 5041  .        elif PA
-0003fc20: 4e44 4153 5f47 545f 3135 303a 0a20 2020  NDAS_GT_150:.   
+0003fc20: 4e44 4153 5f47 455f 3135 303a 0a20 2020  NDAS_GE_150:.   
 0003fc30: 2020 2020 2020 2020 206d 6179 6265 5f77           maybe_w
 0003fc40: 6172 6e20 3d20 5472 7565 0a20 2020 2020  arn = True.     
 0003fc50: 2020 2020 2020 206e 756d 6572 6963 5f6f         numeric_o
 0003fc60: 6e6c 7920 3d20 5472 7565 0a20 2020 2020  nly = True.     
 0003fc70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 0003fc80: 2020 2020 206e 756d 6572 6963 5f6f 6e6c       numeric_onl
 0003fc90: 7920 3d20 5472 7565 0a0a 2020 2020 616c  y = True..    al
@@ -17732,15 +17732,15 @@
 00045430: 6d61 786d 696e 5f63 6875 6e6b 2878 2c20  maxmin_chunk(x, 
 00045440: 666e 3d4e 6f6e 652c 2073 6b69 706e 613d  fn=None, skipna=
 00045450: 5472 7565 2c20 6e75 6d65 7269 635f 6f6e  True, numeric_on
 00045460: 6c79 3d46 616c 7365 293a 0a20 2020 206e  ly=False):.    n
 00045470: 756d 6572 6963 5f6f 6e6c 795f 6b77 6172  umeric_only_kwar
 00045480: 6773 203d 2028 0a20 2020 2020 2020 207b  gs = (.        {
 00045490: 7d20 6966 206e 6f74 2050 414e 4441 535f  } if not PANDAS_
-000454a0: 4754 5f31 3530 206f 7220 6973 5f73 6572  GT_150 or is_ser
+000454a0: 4745 5f31 3530 206f 7220 6973 5f73 6572  GE_150 or is_ser
 000454b0: 6965 735f 6c69 6b65 2878 2920 656c 7365  ies_like(x) else
 000454c0: 207b 226e 756d 6572 6963 5f6f 6e6c 7922   {"numeric_only"
 000454d0: 3a20 6e75 6d65 7269 635f 6f6e 6c79 7d0a  : numeric_only}.
 000454e0: 2020 2020 290a 2020 2020 6d69 6e6d 6178      ).    minmax
 000454f0: 203d 2022 6d61 7822 2069 6620 666e 203d   = "max" if fn =
 00045500: 3d20 2269 6478 6d61 7822 2065 6c73 6520  = "idxmax" else 
 00045510: 226d 696e 220a 2020 2020 6966 206c 656e  "min".    if len
@@ -18001,15 +18001,15 @@
 00046500: 2020 2020 2020 6d65 7461 2e69 6e64 6578        meta.index
 00046510: 203d 206d 6574 612e 696e 6465 782e 6173   = meta.index.as
 00046520: 7479 7065 2861 7267 2e69 6e64 6578 2e64  type(arg.index.d
 00046530: 7479 7065 290a 2020 2020 2020 2020 2020  type).          
 00046540: 2020 6d65 7461 2e69 6e64 6578 2e6e 616d    meta.index.nam
 00046550: 6520 3d20 6172 672e 696e 6465 782e 6e61  e = arg.index.na
 00046560: 6d65 0a20 2020 2069 6620 5041 4e44 4153  me.    if PANDAS
-00046570: 5f47 545f 3230 3020 616e 6420 2269 6e66  _GT_200 and "inf
+00046570: 5f47 455f 3230 3020 616e 6420 2269 6e66  _GE_200 and "inf
 00046580: 6572 5f64 6174 6574 696d 655f 666f 726d  er_datetime_form
 00046590: 6174 2220 696e 206b 7761 7267 733a 0a20  at" in kwargs:. 
 000465a0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
 000465b0: 7761 726e 280a 2020 2020 2020 2020 2020  warn(.          
 000465c0: 2020 2254 6865 2061 7267 756d 656e 7420    "The argument 
 000465d0: 2769 6e66 6572 5f64 6174 6574 696d 655f  'infer_datetime_
 000465e0: 666f 726d 6174 2720 6973 2064 6570 7265  format' is depre
```

### Comparing `dask-2023.7.1/dask/dataframe/dispatch.py` & `dask-2023.8.0/dask/dataframe/dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/extensions.py` & `dask-2023.8.0/dask/dataframe/extensions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/groupby.py` & `dask-2023.8.0/dask/dataframe/groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import numpy as np
 import pandas as pd
 
 from dask import config
 from dask.base import is_dask_collection, tokenize
 from dask.core import flatten
 from dask.dataframe._compat import (
-    PANDAS_GT_140,
-    PANDAS_GT_150,
-    PANDAS_GT_200,
-    PANDAS_GT_210,
+    PANDAS_GE_140,
+    PANDAS_GE_150,
+    PANDAS_GE_200,
+    PANDAS_GE_210,
     check_groupby_axis_deprecation,
     check_numeric_only_deprecation,
     check_observed_deprecation,
 )
 from dask.dataframe.core import (
     GROUP_KEYS_DEFAULT,
     DataFrame,
@@ -46,15 +46,15 @@
     is_series_like,
     make_meta,
     raise_on_meta_error,
 )
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import M, _deprecated, derived_from, funcname, itemgetter
 
-if PANDAS_GT_140:
+if PANDAS_GE_140:
     from pandas.core.apply import reconstruct_func, validate_func_kwargs
 
 # #############################################
 #
 # GroupBy implementation notes
 #
 # Dask groupby supports reductions, i.e., mean, sum and alike, and apply. The
@@ -301,19 +301,19 @@
 
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         if isinstance(self, DataFrameGroupBy):
             numeric_only = kwargs.get("numeric_only", no_default)
             # Prior to `pandas=1.5`, `numeric_only` support wasn't uniformly supported
             # in pandas. We don't support `numeric_only=False` in this case.
-            if not PANDAS_GT_150 and numeric_only is False:
+            if not PANDAS_GE_150 and numeric_only is False:
                 raise NotImplementedError(
                     "'numeric_only=False' is not implemented in Dask."
                 )
-            if PANDAS_GT_150 and not PANDAS_GT_200 and not self._all_numeric():
+            if PANDAS_GE_150 and not PANDAS_GE_200 and not self._all_numeric():
                 if numeric_only is no_default:
                     warnings.warn(
                         "The default value of numeric_only will be changed to False in "
                         "the future when using dask with pandas 2.0",
                         FutureWarning,
                     )
                 elif numeric_only is False and funcname(func) in ("sum", "prod"):
@@ -339,28 +339,28 @@
                 and len(args) > 0
                 and args[0] not in NUMERIC_ONLY_NOT_IMPLEMENTED
             )
             if maybe_raise:
                 numeric_only = kwargs.get("numeric_only", no_default)
                 # Prior to `pandas=1.5`, `numeric_only` support wasn't uniformly supported
                 # in pandas. We don't support `numeric_only=False` in this case.
-                if not PANDAS_GT_150 and numeric_only is False:
+                if not PANDAS_GE_150 and numeric_only is False:
                     raise NotImplementedError(
                         "'numeric_only=False' is not implemented in Dask."
                     )
                 if not self._all_numeric():
                     if numeric_only is False or (
-                        PANDAS_GT_200 and numeric_only is no_default
+                        PANDAS_GE_200 and numeric_only is no_default
                     ):
                         raise NotImplementedError(
                             "'numeric_only=False' is not implemented in Dask."
                         )
                     if (
-                        PANDAS_GT_150
-                        and not PANDAS_GT_200
+                        PANDAS_GE_150
+                        and not PANDAS_GE_200
                         and numeric_only is no_default
                     ):
                         warnings.warn(
                             "The default value of numeric_only will be changed to False "
                             "in the future when using dask with pandas 2.0",
                             FutureWarning,
                         )
@@ -2042,15 +2042,15 @@
             split_out=split_out,
             shuffle=shuffle,
         )
 
     @derived_from(pd.core.groupby.GroupBy)
     @numeric_only_not_implemented
     def var(self, ddof=1, split_every=None, split_out=1, numeric_only=no_default):
-        if not PANDAS_GT_150 and numeric_only is not no_default:
+        if not PANDAS_GE_150 and numeric_only is not no_default:
             raise TypeError("numeric_only not supported for pandas < 1.5")
 
         if self.sort is None and split_out > 1:
             warnings.warn(SORT_SPLIT_OUT_WARNING, FutureWarning)
 
         levels = _determine_levels(self.by)
         result = aca(
@@ -2082,15 +2082,15 @@
             result = result[self._slice]
 
         return result
 
     @derived_from(pd.core.groupby.GroupBy)
     @numeric_only_not_implemented
     def std(self, ddof=1, split_every=None, split_out=1, numeric_only=no_default):
-        if not PANDAS_GT_150 and numeric_only is not no_default:
+        if not PANDAS_GE_150 and numeric_only is not no_default:
             raise TypeError("numeric_only not supported for pandas < 1.5")
         # We sometimes emit this warning ourselves. We ignore it here so users only see it once.
         with check_numeric_only_deprecation():
             v = self.var(
                 ddof,
                 split_every=split_every,
                 split_out=split_out,
@@ -2100,15 +2100,15 @@
         return result
 
     @derived_from(pd.DataFrame)
     def corr(self, ddof=1, split_every=None, split_out=1, numeric_only=no_default):
         """Groupby correlation:
         corr(X, Y) = cov(X, Y) / (std_x * std_y)
         """
-        if not PANDAS_GT_150 and numeric_only is not no_default:
+        if not PANDAS_GE_150 and numeric_only is not no_default:
             raise TypeError("numeric_only not supported for pandas < 1.5")
         return self.cov(
             split_every=split_every,
             split_out=split_out,
             std=True,
             numeric_only=numeric_only,
         )
@@ -2123,15 +2123,15 @@
            all columns: a b c -> a*a, a*b, b*b, b*c, c*c.
 
         2. The values are then aggregated and the final covariance value is calculated:
            cov(X, Y) = X*Y - Xbar * Ybar
 
         When `std` is True calculate Correlation
         """
-        if not PANDAS_GT_150 and numeric_only is not no_default:
+        if not PANDAS_GE_150 and numeric_only is not no_default:
             raise TypeError("numeric_only not supported for pandas < 1.5")
         numeric_only_kwargs = get_numeric_only_kwargs(numeric_only)
         if self.sort is None and split_out > 1:
             warnings.warn(SORT_SPLIT_OUT_WARNING, FutureWarning)
 
         levels = _determine_levels(self.by)
 
@@ -2231,15 +2231,15 @@
             split_out = 1
         shuffle = _determine_shuffle(shuffle, split_out)
 
         relabeling = None
         columns = None
         order = None
         column_projection = None
-        if PANDAS_GT_140:
+        if PANDAS_GE_140:
             if isinstance(self, DataFrameGroupBy):
                 if arg is None:
                     relabeling, arg, columns, order = reconstruct_func(arg, **kwargs)
 
             elif isinstance(self, SeriesGroupBy):
                 relabeling = arg is None
                 if relabeling:
@@ -2771,15 +2771,15 @@
             min_periods=min_periods,
             center=center,
             win_type=win_type,
             axis=axis,
         )
 
     def _normalize_axis(self, axis, method: str):
-        if PANDAS_GT_210 and axis is not no_default:
+        if PANDAS_GE_210 and axis is not no_default:
             if axis in (0, "index"):
                 warnings.warn(
                     f"The 'axis' keyword in {type(self).__name__}.{method} is deprecated and will "
                     "be removed in a future version. Call without passing 'axis' instead.",
                     FutureWarning,
                 )
             else:
@@ -2844,40 +2844,40 @@
             value=value,
             method=method,
             limit=limit,
             axis=axis,
             meta=meta,
         )
 
-        if PANDAS_GT_150 and self.group_keys:
+        if PANDAS_GE_150 and self.group_keys:
             return result.map_partitions(M.droplevel, self.by)
 
         return result
 
     @derived_from(pd.core.groupby.GroupBy)
     def ffill(self, limit=None):
         meta = self._meta_nonempty.apply(
             _drop_apply, by=self.by, what="ffill", limit=limit
         )
         result = self.apply(
             _drop_apply, by=self.by, what="ffill", limit=limit, meta=meta
         )
-        if PANDAS_GT_150 and self.group_keys:
+        if PANDAS_GE_150 and self.group_keys:
             return result.map_partitions(M.droplevel, self.by)
         return result
 
     @derived_from(pd.core.groupby.GroupBy)
     def bfill(self, limit=None):
         meta = self._meta_nonempty.apply(
             _drop_apply, by=self.by, what="bfill", limit=limit
         )
         result = self.apply(
             _drop_apply, by=self.by, what="bfill", limit=limit, meta=meta
         )
-        if PANDAS_GT_150 and self.group_keys:
+        if PANDAS_GE_150 and self.group_keys:
             return result.map_partitions(M.droplevel, self.by)
         return result
 
 
 class DataFrameGroupBy(_GroupBy):
     _token_prefix = "dataframe-groupby-"
```

### Comparing `dask-2023.7.1/dask/dataframe/hyperloglog.py` & `dask-2023.8.0/dask/dataframe/hyperloglog.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/indexing.py` & `dask-2023.8.0/dask/dataframe/indexing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/__init__.py` & `dask-2023.8.0/dask/dataframe/io/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/csv.py` & `dask-2023.8.0/dask/dataframe/io/csv.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/demo.py` & `dask-2023.8.0/dask/dataframe/io/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import string
 from dataclasses import asdict, dataclass, field
 from typing import Any, Callable, cast
 
 import numpy as np
 import pandas as pd
 
+from dask.dataframe._pyarrow import is_object_string_dtype
 from dask.dataframe.core import tokenize
 from dask.dataframe.io.io import from_map
 from dask.dataframe.io.utils import DataFrameIOFunction
 from dask.utils import random_state_data
 
 __all__ = [
     "make_timeseries",
@@ -176,16 +177,14 @@
             # "poisson", "binomial", etc.
             handler_args, handler_kwargs = _with_defaults(method)
             handler = getattr(rstate, method)
             data = handler(*handler_args, size=n, **handler_kwargs)
         else:
             # method is a Callable
             data = method(*args, state=rstate, size=n, **kwargs)
-    if dtype is not None:
-        data = data.astype(dtype)
     return data
 
 
 names = [
     "Alice",
     "Bob",
     "Charlie",
@@ -317,14 +316,21 @@
         raise TypeError(f"Unhandled index dtype: {index_dtype}")
     df = make_partition(columns, dtypes, index, kwargs, state)
     while df.index[-1] >= end:
         df = df.iloc[:-1]
     return df
 
 
+def same_astype(a: str | type, b: str | type):
+    """Same as pandas.api.types.is_dtype_equal, but also returns True for str / object"""
+    return pd.api.types.is_dtype_equal(a, b) or (
+        is_object_string_dtype(a) and is_object_string_dtype(b)
+    )
+
+
 def make_partition(columns: list, dtypes: dict[str, type | str], index, kwargs, state):
     data = {}
     for k, dt in dtypes.items():
         kws = {
             kk.rsplit("_", 1)[1]: v
             for kk, v in kwargs.items()
             if kk.rsplit("_", 1)[0] == k
@@ -333,17 +339,21 @@
         # columns. This ensures the same output given the same state_data, regardless
         # of whether there is any column projection.
         # cf. https://github.com/dask/dask/pull/9538#issuecomment-1267461887
         result = make[dt](len(index), state, **kws)
         if k in columns:
             data[k] = result
     df = pd.DataFrame(data, index=index, columns=columns)
-    for k, dtype in dtypes.items():
-        if k in columns:
-            df[k] = df[k].astype(dtype)
+    update_dtypes = {
+        k: v
+        for k, v in dtypes.items()
+        if k in columns and not same_astype(v, df[k].dtype)
+    }
+    if update_dtypes:
+        df = df.astype(update_dtypes, copy=False)
     return df
 
 
 def make_timeseries(
     start="2000-01-01",
     end="2000-12-31",
     dtypes=None,
```

### Comparing `dask-2023.7.1/dask/dataframe/io/hdf.py` & `dask-2023.8.0/dask/dataframe/io/hdf.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/io.py` & `dask-2023.8.0/dask/dataframe/io/io.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/json.py` & `dask-2023.8.0/dask/dataframe/io/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pandas as pd
 from fsspec.core import open_files
 
 from dask.base import compute as dask_compute
 from dask.bytes import read_bytes
 from dask.core import flatten
-from dask.dataframe._compat import PANDAS_GT_200, PANDAS_VERSION
+from dask.dataframe._compat import PANDAS_GE_200, PANDAS_VERSION
 from dask.dataframe.backends import dataframe_creation_dispatch
 from dask.dataframe.io.io import from_delayed
 from dask.dataframe.utils import insert_meta_param_description, make_meta
 from dask.delayed import delayed
 
 
 def to_json(
@@ -213,15 +213,15 @@
         include_path_column = "path"
 
     if path_converter is None:
         path_converter = lambda x: x
 
     # Handle engine string (Pandas>=2.0)
     if isinstance(engine, str):
-        if not PANDAS_GT_200:
+        if not PANDAS_GE_200:
             raise ValueError(
                 f"Pandas>=2.0 is required to pass a string to the "
                 f"`engine` argument of `read_json` "
                 f"(pandas={str(PANDAS_VERSION)} is currently installed)."
             )
         engine = partial(pd.read_json, engine=engine)
```

### Comparing `dask-2023.7.1/dask/dataframe/io/orc/arrow.py` & `dask-2023.8.0/dask/dataframe/io/orc/arrow.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/orc/core.py` & `dask-2023.8.0/dask/dataframe/io/orc/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/parquet/arrow.py` & `dask-2023.8.0/dask/dataframe/io/parquet/arrow.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/parquet/core.py` & `dask-2023.8.0/dask/dataframe/io/parquet/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/parquet/fastparquet.py` & `dask-2023.8.0/dask/dataframe/io/parquet/fastparquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 import pandas as pd
 import tlz as toolz
 from packaging.version import parse as parse_version
 
 from dask.core import flatten
-from dask.dataframe._compat import PANDAS_GT_201
+from dask.dataframe._compat import PANDAS_GE_201
 
 try:
     import fastparquet
     from fastparquet import ParquetFile
     from fastparquet.util import ex_from_sep, get_file_scheme, groupby_types, val_to_num
     from fastparquet.writer import make_part_file, partition_on_columns
 except ImportError:
@@ -1111,15 +1111,15 @@
 
         # Extract row-groups and pre-allocate df
         rgs = pf.row_groups
         size = sum(rg.num_rows for rg in rgs)
         df, views = pf.pre_allocate(size, columns, categories, index)
         if (
             parse_version(fastparquet.__version__) <= parse_version("2023.02.0")
-            and PANDAS_GT_201
+            and PANDAS_GE_201
             and df.columns.empty
         ):
             df.columns = pd.Index([], dtype=object)
         start = 0
 
         # Get a map of file names -> row-groups
         fn_rg_map = defaultdict(list)
```

### Comparing `dask-2023.7.1/dask/dataframe/io/parquet/utils.py` & `dask-2023.8.0/dask/dataframe/io/parquet/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/sql.py` & `dask-2023.8.0/dask/dataframe/io/sql.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_csv.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from tlz import partition_all, valmap
 
 import dask
 from dask.base import compute_as_if_collection
 from dask.bytes.core import read_bytes
 from dask.bytes.utils import compress
 from dask.core import flatten
-from dask.dataframe._compat import PANDAS_GT_140, PANDAS_GT_200, tm
+from dask.dataframe._compat import PANDAS_GE_140, PANDAS_GE_200, tm
 from dask.dataframe.io.csv import (
     _infer_block_size,
     auto_blocksize,
     block_mask,
     pandas_read_text,
     text_blocks_to_pandas,
 )
@@ -374,15 +374,15 @@
         assert list(f.columns) == ["name", "amount"]
         # index may be different
         result = f.compute(scheduler="sync").reset_index(drop=True)
         assert_eq(result, pd_read(fn, sep=sep))
 
 
 @pytest.mark.skipif(
-    not PANDAS_GT_200, reason="dataframe.convert-string requires pandas>=2.0"
+    not PANDAS_GE_200, reason="dataframe.convert-string requires pandas>=2.0"
 )
 def test_read_csv_convert_string_config():
     pytest.importorskip("pyarrow", reason="Requires pyarrow strings")
     with filetext(csv_text) as fn:
         df = pd.read_csv(fn)
         with dask.config.set({"dataframe.convert-string": True}):
             ddf = dd.read_csv(fn)
@@ -1250,15 +1250,15 @@
 
 def test_read_csv_singleton_dtype():
     data = b"a,b\n1,2\n3,4\n5,6"
     with filetext(data, mode="wb") as fn:
         assert_eq(pd.read_csv(fn, dtype=float), dd.read_csv(fn, dtype=float))
 
 
-@pytest.mark.skipif(not PANDAS_GT_140, reason="arrow engine available from 1.4")
+@pytest.mark.skipif(not PANDAS_GE_140, reason="arrow engine available from 1.4")
 def test_read_csv_arrow_engine():
     pytest.importorskip("pyarrow")
     sep_text = normalize_text(
         """
     a,b
     1,2
     """
```

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_demo.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 import pytest
 
 import dask
 import dask.dataframe as dd
 from dask.blockwise import Blockwise, optimize_blockwise
-from dask.dataframe._compat import PANDAS_GT_200, tm
+from dask.dataframe._compat import PANDAS_GE_200, tm
 from dask.dataframe.optimize import optimize_dataframe_getitem
 from dask.dataframe.utils import assert_eq, get_string_dtype
 
 
 def test_make_timeseries():
     df = dd.demo.make_timeseries(
         "2000", "2015", {"A": float, "B": int, "C": str}, freq="2D", partition_freq="6M"
@@ -213,15 +213,15 @@
             ColumnSpec(prefix="c", dtype="category", choices=["apple", "banana"]),
             ColumnSpec(prefix="s", dtype=str, length=15, random=True),
         ],
     )
     ddf = with_spec(spec, seed=seed)
     assert isinstance(ddf, dd.DataFrame)
     assert ddf.columns.tolist() == ["i1", "f1", "c1", "s1"]
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         assert ddf.index.dtype == "int32"
     assert ddf["i1"].dtype == "int32"
     assert ddf["f1"].dtype == "float32"
     assert ddf["c1"].dtype.name == "category"
     assert ddf["s1"].dtype == get_string_dtype()
     res = ddf.compute().sort_index()
     assert len(res) == 10
```

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_hdf.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_hdf.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_io.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pytest
 
 import dask
 import dask.array as da
 import dask.dataframe as dd
 from dask import config
 from dask.blockwise import Blockwise
-from dask.dataframe._compat import PANDAS_GT_200, tm
+from dask.dataframe._compat import PANDAS_GE_200, tm
 from dask.dataframe.io.io import _meta_from_array
 from dask.dataframe.optimize import optimize
 from dask.dataframe.utils import assert_eq, get_string_dtype, pyarrow_strings_enabled
 from dask.delayed import Delayed, delayed
 from dask.utils_test import hlg_layer_topological
 
 ##########
@@ -276,15 +276,15 @@
 def test_from_pandas_npartitions_duplicates(index):
     df = pd.DataFrame({"a": range(8), "index": index}).set_index("index")
     ddf = dd.from_pandas(df, npartitions=3)
     assert ddf.divisions == ("A", "B", "C", "C")
 
 
 @pytest.mark.skipif(
-    not PANDAS_GT_200, reason="dataframe.convert-string requires pandas>=2.0"
+    not PANDAS_GE_200, reason="dataframe.convert-string requires pandas>=2.0"
 )
 def test_from_pandas_convert_string_config():
     pytest.importorskip("pyarrow", reason="Requires pyarrow strings")
 
     # With `dataframe.convert-string=False`, strings should remain objects
     with dask.config.set({"dataframe.convert-string": False}):
         s = pd.Series(["foo", "bar", "ricky", "bobby"], index=["a", "b", "c", "d"])
@@ -313,15 +313,15 @@
     s_pyarrow.index = s_pyarrow.index.astype("string[pyarrow]")
     df_pyarrow = df.astype({"z": "string[pyarrow]"})
     df_pyarrow.index = df_pyarrow.index.astype("string[pyarrow]")
     assert_eq(s_pyarrow, ds)
     assert_eq(df_pyarrow, ddf)
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="Requires pandas<2.0")
+@pytest.mark.skipif(PANDAS_GE_200, reason="Requires pandas<2.0")
 def test_from_pandas_convert_string_config_raises():
     pytest.importorskip("pyarrow", reason="Different error without pyarrow")
     df = pd.DataFrame(
         {
             "x": [1, 2, 3, 4],
             "y": [5.0, 6.0, 7.0, 8.0],
             "z": ["foo", "bar", "ricky", "bobby"],
```

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_json.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 import pandas as pd
 import pytest
 
 import dask
 import dask.dataframe as dd
-from dask.dataframe._compat import PANDAS_GT_200
+from dask.dataframe._compat import PANDAS_GE_200
 from dask.dataframe.utils import assert_eq
 from dask.utils import tmpdir, tmpfile
 
 df = pd.DataFrame({"x": ["a", "b", "c", "d"], "y": [1, 2, 3, 4]})
 ddf = dd.from_pandas(df, npartitions=2)
 
 
@@ -123,15 +123,15 @@
         assert_eq(actual, actual_pd)
 
 
 @pytest.mark.parametrize("engine", ["ujson", pd.read_json])
 def test_read_json_engine_str(engine):
     with tmpfile("json") as f:
         df.to_json(f, lines=False)
-        if isinstance(engine, str) and not PANDAS_GT_200:
+        if isinstance(engine, str) and not PANDAS_GE_200:
             with pytest.raises(ValueError, match="Pandas>=2.0 is required"):
                 dd.read_json(f, engine=engine, lines=False)
         else:
             got = dd.read_json(f, engine=engine, lines=False)
             assert_eq(got, df)
```

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_orc.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_orc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_parquet.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from packaging.version import parse as parse_version
 
 import dask
 import dask.dataframe as dd
 import dask.multiprocessing
 from dask.array.numpy_compat import _numpy_124
 from dask.blockwise import Blockwise, optimize_blockwise
-from dask.dataframe._compat import PANDAS_GT_150, PANDAS_GT_200, PANDAS_GT_202
+from dask.dataframe._compat import PANDAS_GE_150, PANDAS_GE_200, PANDAS_GE_202
 from dask.dataframe.io.parquet.core import get_engine
 from dask.dataframe.io.parquet.utils import _parse_pandas_metadata
 from dask.dataframe.optimize import optimize_dataframe_getitem
 from dask.dataframe.utils import assert_eq, pyarrow_strings_enabled
 from dask.layers import DataFrameIOLayer
 from dask.utils import natural_sort_key
 from dask.utils_test import hlg_layer
@@ -599,15 +599,15 @@
 @pytest.mark.parametrize(
     "dtype_backend",
     [
         "pandas",
         pytest.param(
             "pyarrow",
             marks=pytest.mark.skipif(
-                not PANDAS_GT_150, reason="Requires pyarrow-backed nullable dtypes"
+                not PANDAS_GE_150, reason="Requires pyarrow-backed nullable dtypes"
             ),
         ),
     ],
 )
 def test_use_nullable_dtypes(tmp_path, dtype_backend, engine):
     """
     Test reading a parquet file without pandas metadata,
@@ -1145,15 +1145,15 @@
         and df.x.dtype == "M8[ns]"
         and engine == "fastparquet"
         and fastparquet_version <= parse_version("0.6.3")
     ):
         pytest.xfail(reason="fastparquet doesn't support nanosecond precision yet")
     # non-ns times
     if (
-        PANDAS_GT_200
+        PANDAS_GE_200
         and "x" in df
         and (df.x.dtype == "M8[ms]" or df.x.dtype == "M8[us]")
     ):
         if engine == "pyarrow":
             pytest.xfail("https://github.com/apache/arrow/issues/15079")
         elif engine == "fastparquet" and fastparquet_version <= parse_version(
             "2022.12.0"
@@ -2420,21 +2420,23 @@
         pd.DataFrame({"x": list(map(pd.Timestamp, [3000000, 2000000, 1000000]))}),  # ms
         pd.DataFrame({"x": list(map(pd.Timestamp, [3000, 2000, 1000]))}),  # us
         pd.DataFrame({"x": [3000, 2000, 1000]}).astype("M8[ns]"),
         # pd.DataFrame({'x': [3, 2, 1]}).astype('M8[ns]'), # Casting errors
         pytest.param(
             pd.DataFrame({"x": [3, 2, 1]}).astype("M8[us]"),
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="https://github.com/apache/arrow/issues/15079"
+                PANDAS_GE_200 and pyarrow_version < parse_version("13.0.0.dev"),
+                reason="https://github.com/apache/arrow/issues/15079",
             ),
         ),
         pytest.param(
             pd.DataFrame({"x": [3, 2, 1]}).astype("M8[ms]"),
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="https://github.com/apache/arrow/issues/15079"
+                PANDAS_GE_200 and pyarrow_version < parse_version("13.0.0.dev"),
+                reason="https://github.com/apache/arrow/issues/15079",
             ),
         ),
         pd.DataFrame({"x": [3, 2, 1]}).astype("uint16"),
         pd.DataFrame({"x": [3, 2, 1]}).astype("float32"),
         pd.DataFrame({"x": [3, 1, 2]}, index=[3, 2, 1]),
         pd.DataFrame(
             {"x": [4, 5, 6, 1, 2, 3]}, index=pd.Index([1, 2, 3, 4, 5, 6], name="foo")
@@ -3367,18 +3369,21 @@
     arr_dates = arr_numeric.astype("datetime64[ms]")
 
     table = pa.Table.from_arrays([pa.array(arr_dates)], names=["ts"])
     pa.parquet.write_table(
         table, f"{tmpdir}/file.parquet", use_deprecated_int96_timestamps=False
     )
 
-    # This will raise by default due to overflow
-    with pytest.raises(pa.lib.ArrowInvalid) as e:
+    if pyarrow_version < parse_version("13.0.0.dev"):
+        # This will raise by default due to overflow
+        with pytest.raises(pa.lib.ArrowInvalid) as e:
+            dd.read_parquet(str(tmpdir), engine="pyarrow").compute()
+            assert "out of bounds" in str(e.value)
+    else:
         dd.read_parquet(str(tmpdir), engine="pyarrow").compute()
-    assert "out of bounds" in str(e.value)
 
     from dask.dataframe.io.parquet.arrow import ArrowDatasetEngine as ArrowEngine
 
     class ArrowEngineWithTimestampClamp(ArrowEngine):
         @classmethod
         def clamp_arrow_datetimes(cls, arrow_table: pa.Table) -> pa.Table:
             """Constrain datetimes to be valid for pandas
@@ -3565,15 +3570,15 @@
         }
     ).set_index("myindex")
     data.index.name = None
     df1 = dd.from_pandas(data, npartitions=npartitions)
     df1.to_parquet(tmp, partition_on="B", engine=write_engine)
 
     expect = data[data["B"] == 1]
-    if PANDAS_GT_200 and read_engine == "fastparquet":
+    if PANDAS_GE_200 and read_engine == "fastparquet":
         # fastparquet does not preserve dtype of cats
         expect = expect.copy()  # SettingWithCopyWarning
         expect["B"] = expect["B"].astype(
             pd.CategoricalDtype(expect["B"].dtype.categories.astype("int64"))
         )
     got = dd.read_parquet(tmp, engine=read_engine, filters=[("B", "==", 1)])
     assert_eq(expect, got)
@@ -4481,15 +4486,15 @@
     )
 
 
 @PYARROW_MARK
 def test_roundtrip_partitioned_pyarrow_dataset(tmpdir, engine):
     # See: https://github.com/dask/dask/issues/8650
 
-    if engine == "fastparquet" and PANDAS_GT_200:
+    if engine == "fastparquet" and PANDAS_GE_200:
         # https://github.com/dask/dask/issues/9966
         pytest.xfail("fastparquet reads as int64 while pyarrow does as int32")
 
     import pyarrow.parquet as pq
     from pyarrow.dataset import HivePartitioning, write_dataset
 
     # Sample data
@@ -4787,15 +4792,15 @@
 
     ddf = dd.read_parquet(path, engine=engine, filters=[("b", "is not", None)])
     assert_eq(df, ddf)
 
 
 @pytest.mark.parametrize("convert_string", [True, False])
 @pytest.mark.skipif(
-    not PANDAS_GT_200, reason="dataframe.convert-string requires pandas>=2.0"
+    not PANDAS_GE_200, reason="dataframe.convert-string requires pandas>=2.0"
 )
 def test_read_parquet_convert_string(tmp_path, convert_string, engine):
     df = pd.DataFrame(
         {"A": ["def", "abc", "ghi"], "B": [5, 2, 3], "C": ["x", "y", "z"]}
     ).set_index("C")
 
     outfile = tmp_path / "out.parquet"
@@ -4821,15 +4826,15 @@
         ddf2 = dd.read_parquet(outfile, engine="pyarrow")
 
     assert ddf1._name != ddf2._name
 
 
 @PYARROW_MARK
 @pytest.mark.skipif(
-    not PANDAS_GT_200, reason="dataframe.convert-string requires pandas>=2.0"
+    not PANDAS_GE_200, reason="dataframe.convert-string requires pandas>=2.0"
 )
 def test_read_parquet_convert_string_nullable_mapper(tmp_path, engine):
     """Make sure that when convert_string, dtype_backend and types_mapper are set,
     all three are used."""
     df = pd.DataFrame(
         {
             "A": pd.Series(["def", "abc", "ghi"], dtype="string"),
@@ -4864,15 +4869,15 @@
     expected.index = expected.index.astype("string[pyarrow]")
 
     assert_eq(ddf, expected)
 
 
 @PYARROW_MARK
 @pytest.mark.parametrize("dtype_backend", ["numpy_nullable", "pyarrow"])
-@pytest.mark.skipif(not PANDAS_GT_150, reason="Requires pyarrow-backed nullable dtypes")
+@pytest.mark.skipif(not PANDAS_GE_150, reason="Requires pyarrow-backed nullable dtypes")
 def test_dtype_backend(tmp_path, dtype_backend, engine):
     """
     Test reading a parquet file without pandas metadata,
     but forcing use of nullable dtypes where appropriate
     """
     dtype_extra = "" if dtype_backend == "numpy_nullable" else "[pyarrow]"
     df = pd.DataFrame(
@@ -4907,15 +4912,15 @@
     else:
         ddf2 = dd.read_parquet(tmp_path, engine=engine, dtype_backend=dtype_backend)
         assert_eq(df, ddf2, check_index=False)
 
 
 @PYARROW_MARK
 @pytest.mark.skipif(
-    not PANDAS_GT_200, reason="pd.Index does not support int32 before 2.0"
+    not PANDAS_GE_200, reason="pd.Index does not support int32 before 2.0"
 )
 def test_read_parquet_preserve_categorical_column_dtype(tmp_path):
     df = pd.DataFrame({"a": [1, 2], "b": ["x", "y"]})
 
     outdir = tmp_path / "out.parquet"
     df.to_parquet(outdir, engine="pyarrow", partition_cols=["a"])
     ddf = dd.read_parquet(outdir, engine="pyarrow")
@@ -4924,23 +4929,23 @@
         {"b": ["x", "y"], "a": pd.Categorical(pd.Index([1, 2], dtype="int32"))},
         index=[0, 0],
     )
     assert_eq(ddf, expected)
 
 
 @PYARROW_MARK
-@pytest.mark.skipif(not PANDAS_GT_200, reason="Requires pd.ArrowDtype")
+@pytest.mark.skipif(not PANDAS_GE_200, reason="Requires pd.ArrowDtype")
 def test_dtype_backend_categoricals(tmp_path):
     df = pd.DataFrame({"a": pd.Series(["x", "y"], dtype="category"), "b": [1, 2]})
     outdir = tmp_path / "out.parquet"
     df.to_parquet(outdir, engine="pyarrow")
     ddf = dd.read_parquet(outdir, engine="pyarrow", dtype_backend="pyarrow")
     pdf = pd.read_parquet(outdir, engine="pyarrow", dtype_backend="pyarrow")
     # Set sort_results=False because of pandas bug up to 2.0.1
-    assert_eq(ddf, pdf, sort_results=PANDAS_GT_202)
+    assert_eq(ddf, pdf, sort_results=PANDAS_GE_202)
 
 
 @PYARROW_MARK
 @pytest.mark.parametrize("filters", [None, [[("b", "==", "dog")]]])
 def test_non_categorical_partitioning_pyarrow(tmpdir, filters):
     from pyarrow.dataset import partitioning as pd_partitioning
```

### Comparing `dask-2023.7.1/dask/dataframe/io/tests/test_sql.py` & `dask-2023.8.0/dask/dataframe/io/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/io/utils.py` & `dask-2023.8.0/dask/dataframe/io/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/methods.py` & `dask-2023.8.0/dask/dataframe/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_extension_array_dtype
 from tlz import partition
 
 from dask.dataframe._compat import (
-    PANDAS_GT_131,
-    PANDAS_GT_140,
-    PANDAS_GT_200,
+    PANDAS_GE_131,
+    PANDAS_GE_140,
+    PANDAS_GE_200,
     check_apply_dataframe_deprecation,
     check_applymap_dataframe_deprecation,
     check_convert_dtype_deprecation,
     check_observed_deprecation,
 )
 
 #  preserve compatibility while moving dispatch objects
@@ -107,15 +107,15 @@
     Empty DataFrame
     Columns: []
     Index: []
     """
     if len(df.index) == 0:
         return df
 
-    if PANDAS_GT_131:
+    if PANDAS_GE_131:
         if kind is not None:
             warnings.warn(
                 "The `kind` argument is no longer used/supported. "
                 "It will be dropped in a future release.",
                 category=FutureWarning,
             )
         kind_opts = {}
@@ -347,15 +347,15 @@
 
 
 def assign(df, *pairs):
     # Only deep copy when updating an element
     # (to avoid modifying the original)
     # Setitem never modifies an array inplace with pandas 1.4 and up
     pairs = dict(partition(2, pairs))
-    deep = bool(set(pairs) & set(df.columns)) and not PANDAS_GT_140
+    deep = bool(set(pairs) & set(df.columns)) and not PANDAS_GE_140
     df = df.copy(deep=bool(deep))
     for name, val in pairs.items():
         df[name] = val
     return df
 
 
 def unique(x, series_name=None):
@@ -377,15 +377,15 @@
     x, sort=True, ascending=False, normalize=False, total_length=None, **groupby_kwargs
 ):
     out = value_counts_combine(x, **groupby_kwargs)
     if normalize:
         out /= total_length if total_length is not None else out.sum()
     if sort:
         out = out.sort_values(ascending=ascending)
-    if PANDAS_GT_200 and normalize:
+    if PANDAS_GE_200 and normalize:
         out.name = "proportion"
     return out
 
 
 def nbytes(x):
     return x.nbytes
```

### Comparing `dask-2023.7.1/dask/dataframe/multi.py` & `dask-2023.8.0/dask/dataframe/multi.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/numeric.py` & `dask-2023.8.0/dask/dataframe/numeric.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/optimize.py` & `dask-2023.8.0/dask/dataframe/optimize.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/partitionquantiles.py` & `dask-2023.8.0/dask/dataframe/partitionquantiles.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/reshape.py` & `dask-2023.8.0/dask/dataframe/reshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_list_like, is_scalar
 
 import dask
 from dask.dataframe import methods
-from dask.dataframe._compat import PANDAS_GT_200
+from dask.dataframe._compat import PANDAS_GE_200
 from dask.dataframe.core import DataFrame, Series, apply_concat_apply, map_partitions
 from dask.dataframe.utils import has_known_categories
 from dask.utils import M, get_meta_library
 
 ###############################################################
 # Dummies
 ###############################################################
 
 
-_get_dummies_dtype_default = bool if PANDAS_GT_200 else np.uint8
+_get_dummies_dtype_default = bool if PANDAS_GE_200 else np.uint8
 
 
 def get_dummies(
     data,
     prefix=None,
     prefix_sep="_",
     dummy_na=False,
```

### Comparing `dask-2023.7.1/dask/dataframe/rolling.py` & `dask-2023.8.0/dask/dataframe/rolling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import datetime
-import inspect
 from numbers import Integral
 
 import pandas as pd
 from pandas.api.types import is_datetime64_any_dtype
 from pandas.core.window import Rolling as pd_Rolling
 
 from dask.array.core import normalize_arg
@@ -597,33 +596,30 @@
     def quantile(self, quantile):
         return self._call_method("quantile", quantile)
 
     @derived_from(pd_Rolling)
     def apply(
         self,
         func,
-        raw=None,
+        raw=False,
         engine="cython",
         engine_kwargs=None,
         args=None,
         kwargs=None,
     ):
-        compat_kwargs = {}
         kwargs = kwargs or {}
         args = args or ()
-        meta = self.obj._meta.rolling(0)
-        if has_keyword(meta.apply, "engine"):
-            # PANDAS_GT_100
-            compat_kwargs = dict(engine=engine, engine_kwargs=engine_kwargs)
-        if raw is None:
-            # PANDAS_GT_100: The default changed from None to False
-            raw = inspect.signature(meta.apply).parameters["raw"]
-
         return self._call_method(
-            "apply", func, raw=raw, args=args, kwargs=kwargs, **compat_kwargs
+            "apply",
+            func,
+            raw=raw,
+            engine=engine,
+            engine_kwargs=engine_kwargs,
+            args=args,
+            kwargs=kwargs,
         )
 
     @derived_from(pd_Rolling)
     def aggregate(self, func, *args, **kwargs):
         return self._call_method("agg", func, *args, **kwargs)
 
     agg = aggregate
```

### Comparing `dask-2023.7.1/dask/dataframe/shuffle.py` & `dask-2023.8.0/dask/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_accessors.py` & `dask-2023.8.0/dask/dataframe/tests/test_accessors.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import contextlib
 
 import numpy as np
 import pytest
 
 pd = pytest.importorskip("pandas")
 import dask.dataframe as dd
-from dask.dataframe._compat import PANDAS_GT_140, PANDAS_GT_210
+from dask.dataframe._compat import PANDAS_GE_140, PANDAS_GE_210
 from dask.dataframe._pyarrow import to_pyarrow_string
 from dask.dataframe.utils import assert_eq, pyarrow_strings_enabled
 
 
 @contextlib.contextmanager
 def ensure_removed(obj, attr):
     """Ensure that an attribute added to 'obj' during the test is
@@ -98,15 +98,15 @@
 
     assert "date" in dir(ddf.dt_col.dt)
 
     # pandas loses Series.name via datetime accessor
     # see https://github.com/pydata/pandas/issues/10712
     assert_eq(ddf.dt_col.dt.date, df.dt_col.dt.date, check_names=False)
 
-    warning = FutureWarning if PANDAS_GT_210 else None
+    warning = FutureWarning if PANDAS_GE_210 else None
     # to_pydatetime returns a numpy array in pandas, but a Series in dask
     # pandas will start returning a Series with 3.0 as well
     with pytest.warns(warning, match="will return a Series"):
         ddf_result = ddf.dt_col.dt.to_pydatetime()
     with pytest.warns(warning, match="will return a Series"):
         pd_result = pd.Series(
             df.dt_col.dt.to_pydatetime(), index=df.index, dtype=object
@@ -219,15 +219,15 @@
 def test_str_accessor_extractall(df_ddf):
     df, ddf = df_ddf
     assert_eq(
         ddf.str_col.str.extractall("(.*)b(.*)"), df.str_col.str.extractall("(.*)b(.*)")
     )
 
 
-@pytest.mark.skipif(not PANDAS_GT_140, reason="requires pandas >= 1.4.0")
+@pytest.mark.skipif(not PANDAS_GE_140, reason="requires pandas >= 1.4.0")
 @pytest.mark.parametrize("method", ["removeprefix", "removesuffix"])
 def test_str_accessor_removeprefix_removesuffix(df_ddf, method):
     df, ddf = df_ddf
     prefix = df.str_col.iloc[0][:2]
     suffix = df.str_col.iloc[0][-2:]
     missing = "definitely a missing prefix/suffix"
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_arithmetics_reduction.py` & `dask-2023.8.0/dask/dataframe/tests/test_arithmetics_reduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import pandas as pd
 import pytest
 from pandas.api.types import is_scalar
 
 import dask.dataframe as dd
 from dask.array.numpy_compat import _numpy_125
 from dask.dataframe._compat import (
-    PANDAS_GT_140,
-    PANDAS_GT_150,
-    PANDAS_GT_200,
+    PANDAS_GE_140,
+    PANDAS_GE_150,
+    PANDAS_GE_200,
     PANDAS_VERSION,
     check_numeric_only_deprecation,
 )
 from dask.dataframe.utils import (
     assert_dask_graph,
     assert_eq,
     make_meta,
@@ -743,15 +743,15 @@
 
         if scipy:
             # pandas uses unbiased skew, need to correct for that
             n = pds.shape[0]
             bias_factor = (n * (n - 1)) ** 0.5 / (n - 2)
             assert_eq(dds.skew(), pds.skew() / bias_factor)
 
-            if PANDAS_GT_200:
+            if PANDAS_GE_200:
                 # TODO: Remove this `if`-block once `axis=None` support is added.
                 # https://github.com/dask/dask/issues/9915
                 with pytest.raises(
                     ValueError, match="`axis=None` isn't currently supported"
                 ):
                     dds.skew(axis=None)
             else:
@@ -760,15 +760,15 @@
         if scipy:
             # pandas uses a bias factor for kurtosis, need to correct for that
             n = pds.shape[0]
             factor = ((n - 1) * (n + 1)) / ((n - 2) * (n - 3))
             offset = (6 * (n - 1)) / ((n - 2) * (n - 3))
             assert_eq(factor * dds.kurtosis() + offset, pds.kurtosis())
 
-            if PANDAS_GT_200:
+            if PANDAS_GE_200:
                 # TODO: Remove this `if`-block once `axis=None` support is added.
                 # https://github.com/dask/dask/issues/9915
                 with pytest.raises(
                     ValueError, match="`axis=None` isn't currently supported"
                 ):
                     dds.kurtosis(axis=None)
             else:
@@ -1147,15 +1147,15 @@
             pdf1.sem(axis=axis, ddof=0),
         )
         assert_eq(ddf1.mean(axis=axis, split_every=split_every), pdf1.mean(axis=axis))
 
     pytest.raises(ValueError, lambda: ddf1.sum(axis="incorrect").compute())
 
     # axis=None
-    if PANDAS_GT_140 and not PANDAS_GT_200:
+    if PANDAS_GE_140 and not PANDAS_GE_200:
         ctx = pytest.warns(FutureWarning, match="axis=None")
     else:
         ctx = contextlib.nullcontext()
     # min
     with ctx:
         result = ddf1.min(axis=None, split_every=split_every)
     with ctx:
@@ -1351,30 +1351,30 @@
         assert_eq(
             getattr(df, func)(numeric_only=False),
             getattr(ddf, func)(numeric_only=False),
         )
         warning = None
 
     # `numeric_only` default value
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         if func in numeric_only_false_raises:
             with pytest.raises(
                 errors,
                 match="'DatetimeArray' with dtype datetime64.*|"
                 "'DatetimeArray' does not implement reduction|could not convert|"
                 "'ArrowStringArray' with dtype string"
                 "|unsupported operand|no kernel",
             ):
                 getattr(ddf, func)()
         else:
             assert_eq(
                 getattr(df, func)(),
                 getattr(ddf, func)(),
             )
-    elif PANDAS_GT_150:
+    elif PANDAS_GE_150:
         with pytest.warns(warning, match="The default value of numeric_only"):
             pd_result = getattr(df, func)()
         with pytest.warns(warning, match="The default value of numeric_only"):
             dd_result = getattr(ddf, func)()
         assert_eq(pd_result, dd_result)
     else:
         if func in ["std", "var", "quantile"]:
@@ -1469,17 +1469,17 @@
     ctx = pytest.raises(TypeError, match="does not support|does not implement")
 
     with ctx:
         getattr(df, func)(numeric_only=False)
     with ctx:
         getattr(ddf, func)(numeric_only=False)
 
-    if PANDAS_GT_150 and not PANDAS_GT_200:
+    if PANDAS_GE_150 and not PANDAS_GE_200:
         ctx = pytest.warns(FutureWarning, match="default value")
-    elif not PANDAS_GT_150:
+    elif not PANDAS_GE_150:
         ctx = pytest.warns(FutureWarning, match="nuisance columns")
 
     with ctx:
         getattr(df, func)()
     with ctx:
         getattr(ddf, func)()
 
@@ -1786,15 +1786,15 @@
     ddf = dd.from_pandas(pdf, 3)
 
     kwargs = {} if numeric_only is None else {"numeric_only": numeric_only}
     kwargs["skipna"] = skipna
 
     ctx = contextlib.nullcontext()
     success = True
-    if numeric_only is False or (PANDAS_GT_200 and numeric_only is None):
+    if numeric_only is False or (PANDAS_GE_200 and numeric_only is None):
         ctx = pytest.raises(TypeError)
         success = False
     elif numeric_only is None:
         ctx = pytest.warns(FutureWarning, match="numeric_only")
 
     # Single column always results in NaT
     expected = pdf[["dt1"]].std(axis=1, **kwargs)
@@ -1837,36 +1837,36 @@
     with pytest.raises(
         NotImplementedError,
         match="`std` is only supported with objects that are Dataframes or Series",
     ):
         dd.from_pandas(pd.DataFrame({"test": [1, 2]}), npartitions=2).index.std()
 
 
-@pytest.mark.skipif(not PANDAS_GT_200, reason="ArrowDtype not supported")
+@pytest.mark.skipif(not PANDAS_GE_200, reason="ArrowDtype not supported")
 def test_std_raises_with_arrow_string_ea():
     pa = pytest.importorskip("pyarrow")
     ser = pd.Series(["a", "b", "c"], dtype=pd.ArrowDtype(pa.string()))
     ds = dd.from_pandas(ser, npartitions=2)
     with pytest.raises(ValueError, match="`std` not supported with string series"):
         ds.std()
 
 
 @pytest.mark.parametrize(
     "dtype",
     [
         pytest.param(
             "int64[pyarrow]",
             marks=pytest.mark.skipif(
-                pa is None or not PANDAS_GT_150, reason="requires pyarrow installed"
+                pa is None or not PANDAS_GE_150, reason="requires pyarrow installed"
             ),
         ),
         pytest.param(
             "float64[pyarrow]",
             marks=pytest.mark.skipif(
-                pa is None or not PANDAS_GT_150, reason="requires pyarrow installed"
+                pa is None or not PANDAS_GE_150, reason="requires pyarrow installed"
             ),
         ),
         "Int64",
         "Int32",
         "Float64",
         "UInt64",
     ],
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_boolean.py` & `dask-2023.8.0/dask/dataframe/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_categorical.py` & `dask-2023.8.0/dask/dataframe/tests/test_categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 import dask
 import dask.dataframe as dd
 from dask.dataframe import _compat
-from dask.dataframe._compat import PANDAS_GT_150, PANDAS_GT_200, PANDAS_GT_210, tm
+from dask.dataframe._compat import PANDAS_GE_150, PANDAS_GE_200, PANDAS_GE_210, tm
 from dask.dataframe._pyarrow import to_pyarrow_string
 from dask.dataframe.core import _concat
 from dask.dataframe.utils import (
     assert_eq,
     clear_known_categories,
     get_string_dtype,
     make_meta,
@@ -127,25 +127,25 @@
     "numeric_only",
     [
         True,
         pytest.param(
             False,
             marks=[
                 pytest.mark.xfail(
-                    PANDAS_GT_200, reason="numeric_only=False not implemented"
+                    PANDAS_GE_200, reason="numeric_only=False not implemented"
                 ),
                 pytest.mark.xfail(
-                    not PANDAS_GT_150, reason="`numeric_only` not implemented"
+                    not PANDAS_GE_150, reason="`numeric_only` not implemented"
                 ),
             ],
         ),
         pytest.param(
             None,
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="numeric_only=False not implemented"
+                PANDAS_GE_200, reason="numeric_only=False not implemented"
             ),
         ),
     ],
 )
 @pytest.mark.filterwarnings("ignore:The default value of numeric_only")
 @pytest.mark.filterwarnings("ignore:Dropping")
 def test_unknown_categoricals(shuffle_method, numeric_only):
@@ -162,15 +162,15 @@
     df = ddf.compute()
 
     assert_eq(ddf.w.value_counts(), df.w.value_counts())
     assert_eq(ddf.w.nunique(), df.w.nunique())
 
     ctx = (
         pytest.warns(FutureWarning, match="The default of observed=False")
-        if PANDAS_GT_210
+        if PANDAS_GE_210
         else contextlib.nullcontext()
     )
     numeric_kwargs = {} if numeric_only is None else {"numeric_only": numeric_only}
     with ctx:
         expected = df.groupby(df.w).sum(**numeric_kwargs)
     with ctx:
         result = ddf.groupby(ddf.w).sum(**numeric_kwargs)
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_dataframe.py` & `dask-2023.8.0/dask/dataframe/tests/test_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 import dask.dataframe as dd
 import dask.dataframe.groupby
 from dask import delayed
 from dask.base import compute_as_if_collection
 from dask.blockwise import fuse_roots
 from dask.dataframe import _compat, methods
 from dask.dataframe._compat import (
-    PANDAS_GT_140,
-    PANDAS_GT_150,
-    PANDAS_GT_200,
-    PANDAS_GT_210,
+    PANDAS_GE_133,
+    PANDAS_GE_140,
+    PANDAS_GE_150,
+    PANDAS_GE_200,
+    PANDAS_GE_210,
     tm,
 )
 from dask.dataframe._pyarrow import to_pyarrow_string
 from dask.dataframe.core import (
     Scalar,
     _concat,
     _map_freq_to_period_start,
@@ -500,15 +501,15 @@
     df["a"] = df["a"].astype(get_string_dtype())
 
     if subset is not None:
         df = df.loc[:, subset]
 
     ddf = dd.from_pandas(df, 2)
 
-    if not PANDAS_GT_200:
+    if not PANDAS_GE_200:
         datetime_is_numeric_kwarg = {"datetime_is_numeric": True}
     else:
         datetime_is_numeric_kwarg = {}
 
     # Act
     actual = ddf.describe(
         include=include,
@@ -519,26 +520,26 @@
     expected = df.describe(
         include=include,
         exclude=exclude,
         percentiles=percentiles,
         **datetime_is_numeric_kwarg,
     )
 
-    if "e" in expected and (datetime_is_numeric_kwarg or PANDAS_GT_200):
+    if "e" in expected and (datetime_is_numeric_kwarg or PANDAS_GE_200):
         expected = _drop_mean(expected, "e")
 
     assert_eq(actual, expected)
 
     # Check series
     if subset is None:
         for col in ["a", "c", "e", "g"]:
             expected = df[col].describe(
                 include=include, exclude=exclude, **datetime_is_numeric_kwarg
             )
-            if col == "e" and (datetime_is_numeric_kwarg or PANDAS_GT_200):
+            if col == "e" and (datetime_is_numeric_kwarg or PANDAS_GE_200):
                 expected = _drop_mean(expected)
             actual = ddf[col].describe(
                 include=include, exclude=exclude, **datetime_is_numeric_kwarg
             )
             assert_eq(expected, actual)
 
 
@@ -559,24 +560,24 @@
     }
     # Arrange
     df = pd.DataFrame(data)
     ddf = dd.from_pandas(df, 2)
 
     # Assert
     expected = df.describe()
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         expected = _drop_mean(expected, "e")
 
     assert_eq(ddf.describe(), expected)
 
     # Check series
     for col in ["a", "c"]:
         assert_eq(df[col].describe(), ddf[col].describe())
 
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         expected = _drop_mean(df.e.describe())
         assert_eq(expected, ddf.e.describe())
         with pytest.raises(
             TypeError,
             match="datetime_is_numeric is removed in pandas>=2.0.0",
         ):
             ddf.e.describe(datetime_is_numeric=True)
@@ -1494,17 +1495,17 @@
     assert result.name == "b"
     assert result.compute().name == "b"
     assert_eq(result, exp)
 
 
 @contextlib.contextmanager
 def assert_numeric_only_default_warning(numeric_only, func=None):
-    if func == "quantile" and not PANDAS_GT_150:
+    if func == "quantile" and not PANDAS_GE_150:
         ctx = contextlib.nullcontext()
-    elif numeric_only is None and not PANDAS_GT_200:
+    elif numeric_only is None and not PANDAS_GE_200:
         ctx = pytest.warns(FutureWarning, match="default value of numeric_only")
     else:
         ctx = contextlib.nullcontext()
 
     with ctx:
         yield
 
@@ -1555,15 +1556,15 @@
     )
     ddf = dd.from_pandas(df, 3)
 
     numeric_only_kwarg = {}
     if numeric_only is not None:
         numeric_only_kwarg = {"numeric_only": numeric_only}
 
-    if numeric_only is False or (PANDAS_GT_200 and numeric_only is None):
+    if numeric_only is False or (PANDAS_GE_200 and numeric_only is None):
         with pytest.raises(TypeError):
             df.quantile(**numeric_only_kwarg)
         with pytest.raises(
             (TypeError, ArrowNotImplementedError), match="unsupported operand|no kernel"
         ):
             ddf.quantile(**numeric_only_kwarg)
     else:
@@ -3214,15 +3215,15 @@
             ddf.apply(lambda xy: xy.iloc[0] + xy.iloc[1], axis=1),
             df.apply(lambda xy: xy.iloc[0] + xy.iloc[1], axis=1),
         )
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", UserWarning)
         assert_eq(ddf.apply(lambda xy: xy, axis=1), df.apply(lambda xy: xy, axis=1))
 
-    warning = FutureWarning if PANDAS_GT_210 else None
+    warning = FutureWarning if PANDAS_GE_210 else None
     # specify meta
     func = lambda x: pd.Series([x, x])
     with pytest.warns(warning, match="Returning a DataFrame"):
         ddf_result = ddf.x.apply(func, meta=[(0, int), (1, int)])
     with pytest.warns(warning, match="Returning a DataFrame"):
         pdf_result = df.x.apply(func)
     assert_eq(ddf_result, pdf_result)
@@ -3245,15 +3246,15 @@
 
 @pytest.mark.parametrize("convert_dtype", [None, True, False])
 def test_apply_convert_dtype(convert_dtype):
     """Make sure that explicit convert_dtype raises a warning with pandas>=2.1"""
     df = pd.DataFrame({"x": [2, 3, 4, 5], "y": [10, 20, 30, 40]})
     ddf = dd.from_pandas(df, npartitions=2)
     kwargs = {} if convert_dtype is None else {"convert_dtype": convert_dtype}
-    should_warn = PANDAS_GT_210 and convert_dtype is not None
+    should_warn = PANDAS_GE_210 and convert_dtype is not None
 
     meta_val = ddf.x._meta_nonempty.iloc[0]
 
     def func(x):
         # meta check is a regression test for https://github.com/dask/dask/issues/10209
         assert x != meta_val
         return x + 1
@@ -3292,39 +3293,39 @@
 
     func = lambda row: row["x"] + row["y"]
 
     with pytest.warns(FutureWarning, match="Meta is not valid"):
         ddf.apply(func, axis=1, meta=int)
 
 
-@pytest.mark.skipif(not PANDAS_GT_210, reason="Not available before")
+@pytest.mark.skipif(not PANDAS_GE_210, reason="Not available before")
 @pytest.mark.parametrize("na_action", [None, "ignore"])
 def test_dataframe_map(na_action):
     df = pd.DataFrame({"x": [1, 2, 3, np.nan], "y": [10, 20, 30, 40]})
     ddf = dd.from_pandas(df, npartitions=2)
     assert_eq(
         ddf.map(lambda x: x + 1, na_action=na_action),
         df.map(lambda x: x + 1, na_action=na_action),
     )
     assert_eq(ddf.map(lambda x: (x, x)), df.map(lambda x: (x, x)))
 
 
-@pytest.mark.skipif(PANDAS_GT_210, reason="Available at 2.1")
+@pytest.mark.skipif(PANDAS_GE_210, reason="Available at 2.1")
 def test_dataframe_map_raises():
     df = pd.DataFrame({"x": [1, 2, 3, 4], "y": [10, 20, 30, 40]})
     ddf = dd.from_pandas(df, npartitions=2)
     with pytest.raises(NotImplementedError, match="DataFrame.map requires pandas"):
         ddf.map(lambda x: x + 1)
 
 
 def test_applymap():
     df = pd.DataFrame({"x": [1, 2, 3, 4], "y": [10, 20, 30, 40]})
     ddf = dd.from_pandas(df, npartitions=2)
     msg = "DataFrame.applymap has been deprecated"
-    warning = FutureWarning if PANDAS_GT_210 else None
+    warning = FutureWarning if PANDAS_GE_210 else None
     with pytest.warns(warning, match=msg):
         ddf_result = ddf.applymap(lambda x: x + 1)
     with pytest.warns(warning, match=msg):
         pdf_result = df.applymap(lambda x: x + 1)
     assert_eq(ddf_result, pdf_result)
 
     with pytest.warns(warning, match=msg):
@@ -3374,21 +3375,21 @@
 @pytest.mark.parametrize(
     "numeric_only",
     [
         None,
         pytest.param(
             True,
             marks=pytest.mark.skipif(
-                not PANDAS_GT_150, reason="numeric_only not yet implemented"
+                not PANDAS_GE_150, reason="numeric_only not yet implemented"
             ),
         ),
         pytest.param(
             False,
             marks=pytest.mark.skipif(
-                not PANDAS_GT_150, reason="numeric_only not yet implemented"
+                not PANDAS_GE_150, reason="numeric_only not yet implemented"
             ),
         ),
     ],
 )
 def test_cov_dataframe(numeric_only):
     df = _compat.makeMissingDataframe()
     ddf = dd.from_pandas(df, npartitions=6)
@@ -3440,21 +3441,21 @@
 @pytest.mark.parametrize(
     "numeric_only",
     [
         None,
         pytest.param(
             True,
             marks=pytest.mark.skipif(
-                not PANDAS_GT_150, reason="numeric_only not yet implemented"
+                not PANDAS_GE_150, reason="numeric_only not yet implemented"
             ),
         ),
         pytest.param(
             False,
             marks=pytest.mark.skipif(
-                not PANDAS_GT_150, reason="numeric_only not yet implemented"
+                not PANDAS_GE_150, reason="numeric_only not yet implemented"
             ),
         ),
     ],
 )
 def test_cov_gpu(numeric_only):
     cudf = pytest.importorskip("cudf")
 
@@ -3581,30 +3582,30 @@
 
 @pytest.mark.parametrize(
     "numeric_only",
     [
         pytest.param(
             None,
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="fails with non-numeric data"
+                PANDAS_GE_200, reason="fails with non-numeric data"
             ),
         ),
         pytest.param(
             True,
             marks=pytest.mark.skipif(
-                not PANDAS_GT_150, reason="numeric_only not yet implemented"
+                not PANDAS_GE_150, reason="numeric_only not yet implemented"
             ),
         ),
         pytest.param(
             False,
             marks=[
                 pytest.mark.skipif(
-                    not PANDAS_GT_150, reason="numeric_only not yet implemented"
+                    not PANDAS_GE_150, reason="numeric_only not yet implemented"
                 ),
-                pytest.mark.xfail(PANDAS_GT_150, reason="fails with non-numeric data"),
+                pytest.mark.xfail(PANDAS_GE_150, reason="fails with non-numeric data"),
             ],
         ),
     ],
 )
 def test_cov_corr_mixed(numeric_only):
     size = 1000
     d = {
@@ -3627,15 +3628,15 @@
     df["unique_id"] = df["unique_id"].astype(str)
 
     ddf = dd.from_pandas(df, npartitions=20)
 
     numeric_only_kwarg = {}
     if numeric_only is not None:
         numeric_only_kwarg = {"numeric_only": numeric_only}
-    if not numeric_only_kwarg and PANDAS_GT_150 and not PANDAS_GT_200:
+    if not numeric_only_kwarg and PANDAS_GE_150 and not PANDAS_GE_200:
         ctx = pytest.warns(FutureWarning, match="default value of numeric_only")
     else:
         ctx = contextlib.nullcontext()
 
     # Corr
     with ctx:
         expected = df.corr(**numeric_only_kwarg)
@@ -3684,15 +3685,15 @@
     assert isinstance(result, dd.Series)
     assert result.name is None
     assert_eq(result, df.apply(lambda x: 1, axis=1))
 
     def return_df2(x):
         return pd.Series([x * 2, x * 3], index=["x2", "x3"])
 
-    warning = FutureWarning if PANDAS_GT_210 else None
+    warning = FutureWarning if PANDAS_GE_210 else None
     # Series to completely different DataFrame
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", UserWarning)
         with pytest.warns(warning, match="Returning a DataFrame"):
             result = ddf.x.apply(return_df2)
     assert isinstance(result, dd.DataFrame)
     tm.assert_index_equal(result.columns, pd.Index(["x2", "x3"]))
@@ -3809,25 +3810,25 @@
         FutureWarning,
         match="Using the ``in`` operator to test for membership in Series is deprecated",
     ):
         output = 0 in ds
     assert not output
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="iteritems has been removed")
+@pytest.mark.skipif(PANDAS_GE_200, reason="iteritems has been removed")
 def test_series_iteritems():
     df = pd.DataFrame({"x": [1, 2, 3, 4]})
     ddf = dd.from_pandas(df, npartitions=2)
     # `iteritems` was deprecated starting in `pandas=1.5.0`
     with _check_warning(
-        PANDAS_GT_150, FutureWarning, message="iteritems is deprecated"
+        PANDAS_GE_150, FutureWarning, message="iteritems is deprecated"
     ):
         pd_items = df["x"].iteritems()
     with _check_warning(
-        PANDAS_GT_150, FutureWarning, message="iteritems is deprecated"
+        PANDAS_GE_150, FutureWarning, message="iteritems is deprecated"
     ):
         dd_items = ddf["x"].iteritems()
     for a, b in zip(pd_items, dd_items):
         assert a == b
 
 
 def test_series_iter():
@@ -4251,15 +4252,15 @@
     df = pd.DataFrame(np.random.randn(100, 5), columns=list("abcde"), index=idx)
     df.iloc[31, 1] = np.nan
     df.iloc[78, 3] = np.nan
     ddf = dd.from_pandas(df, npartitions=3)
 
     # https://github.com/pandas-dev/pandas/issues/43587
     check_dtype = not all(
-        (_compat.PANDAS_GT_133, skipna is False, isinstance(idx, pd.DatetimeIndex))
+        (PANDAS_GE_133, skipna is False, isinstance(idx, pd.DatetimeIndex))
     )
 
     with warnings.catch_warnings(record=True):
         assert_eq(df.idxmax(axis=1, skipna=skipna), ddf.idxmax(axis=1, skipna=skipna))
         assert_eq(df.idxmin(axis=1, skipna=skipna), ddf.idxmin(axis=1, skipna=skipna))
 
         assert_eq(
@@ -4316,15 +4317,15 @@
             "dt": [pd.NaT] + [datetime(2010, i, 1) for i in range(1, 8)],
             "timedelta": pd.to_timedelta([1, 2, 3, 4, 5, 6, 7, np.nan]),
             "bool": [True, False] * 4,
         }
     )
     ddf = dd.from_pandas(df, npartitions=2)
 
-    if PANDAS_GT_150:
+    if PANDAS_GE_150:
         assert_eq(
             getattr(ddf, func)(numeric_only=False),
             getattr(df, func)(numeric_only=False).sort_index(),
         )
         assert_eq(
             getattr(ddf, func)(numeric_only=True),
             getattr(df, func)(numeric_only=True).sort_index(),
@@ -4564,23 +4565,23 @@
     for freq in freqs:
         index = pd.date_range("1/1/2000", "1/1/2001", freq=freq)[::4]
         df = pd.DataFrame(
             np.random.random((len(index), 4)), index=index, columns=["A", "B", "C", "D"]
         )
         ddf = dd.from_pandas(df, npartitions=10)
         for offset in offsets:
-            with _check_warning(PANDAS_GT_210, FutureWarning, method):
+            with _check_warning(PANDAS_GE_210, FutureWarning, method):
                 expected = f(df, offset)
-            with _check_warning(PANDAS_GT_210, FutureWarning, method):
+            with _check_warning(PANDAS_GE_210, FutureWarning, method):
                 actual = f(ddf, offset)
             assert_eq(actual, expected)
 
-            with _check_warning(PANDAS_GT_210, FutureWarning, method):
+            with _check_warning(PANDAS_GE_210, FutureWarning, method):
                 expected = f(df.A, offset)
-            with _check_warning(PANDAS_GT_210, FutureWarning, method):
+            with _check_warning(PANDAS_GE_210, FutureWarning, method):
                 actual = f(ddf.A, offset)
             assert_eq(actual, expected)
 
 
 @pytest.mark.parametrize("npartitions", [1, 4, 20])
 @pytest.mark.parametrize("split_every", [2, 5])
 @pytest.mark.parametrize("split_out", [None, 1, 5, 20])
@@ -4674,15 +4675,15 @@
 
     with pytest.warns(UserWarning, match="object dtype"):
         result = ddf.y.values
     assert_eq(result, df.y.values.astype(object))
 
     # Prior to pandas=1.4, `pd.Index` couldn't hold extension dtypes
     ctx = contextlib.nullcontext()
-    if PANDAS_GT_140:
+    if PANDAS_GE_140:
         ctx = pytest.warns(UserWarning, match="object dtype")
     with ctx:
         result = ddf.index.values
     assert_eq(result, df.index.values.astype(object))
 
 
 def test_copy():
@@ -4823,15 +4824,15 @@
     data = [["Tom", 10, 7], ["Farahn", 14, 7], ["Julie", 14, 5], ["Nick", 10, 10]]
 
     df = pd.DataFrame(data, columns=["Name", "Num", "Num"])
     ddf = dd.from_pandas(df, npartitions=3)
 
     assert_eq(ddf.mode(), df.mode())
     # name is not preserved in older pandas
-    assert_eq(ddf.Name.mode(), df.Name.mode(), check_names=PANDAS_GT_140)
+    assert_eq(ddf.Name.mode(), df.Name.mode(), check_names=PANDAS_GE_140)
 
     # test empty
     df = pd.DataFrame(columns=["a", "b"])
     ddf = dd.from_pandas(df, npartitions=1)
     # check_index=False should be removed once https://github.com/pandas-dev/pandas/issues/33321 is resolved.
     assert_eq(ddf.mode(), df.mode(), check_index=False)
 
@@ -4905,15 +4906,15 @@
 
     s = xd.Series(
         ["3/11/2000", "3/12/2000", "3/13/2000"] * 100,
         index=["3/11/2000", "3/12/2000", "3/13/2000"] * 100,
     )
     ds = dd.from_pandas(s, npartitions=10, sort=False)
 
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         ctx = pytest.warns(UserWarning, match="'infer_datetime_format' is deprecated")
     else:
         ctx = contextlib.nullcontext()
 
     with ctx:
         expected = xd.to_datetime(s, infer_datetime_format=True)
     with ctx:
@@ -5733,25 +5734,25 @@
 
     s_3 = pd.Series(list(range(0, 5)) + list(range(0, 20)))
     ds_3 = dd.from_pandas(s_3, npartitions=5)
     assert_eq(s_3.is_monotonic_increasing, ds_3.is_monotonic_increasing)
     assert_eq(s_3.is_monotonic_decreasing, ds_3.is_monotonic_decreasing)
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="pandas removed is_monotonic")
+@pytest.mark.skipif(PANDAS_GE_200, reason="pandas removed is_monotonic")
 def test_is_monotonic_deprecated():
     s = pd.Series(range(20))
     ds = dd.from_pandas(s, npartitions=5)
     # `is_monotonic` was deprecated starting in `pandas=1.5.0`
     with _check_warning(
-        PANDAS_GT_150, FutureWarning, message="is_monotonic is deprecated"
+        PANDAS_GE_150, FutureWarning, message="is_monotonic is deprecated"
     ):
         expected = s.is_monotonic
     with _check_warning(
-        PANDAS_GT_150, FutureWarning, message="is_monotonic is deprecated"
+        PANDAS_GE_150, FutureWarning, message="is_monotonic is deprecated"
     ):
         result = ds.is_monotonic
     assert_eq(expected, result)
 
 
 def test_is_monotonic_dt64():
     s = pd.Series(pd.date_range("20130101", periods=10))
@@ -5774,25 +5775,25 @@
 
     s_3 = pd.Series(1, index=list(range(0, 5)) + list(range(0, 20)))
     ds_3 = dd.from_pandas(s_3, npartitions=5, sort=False)
     assert_eq(s_3.index.is_monotonic_increasing, ds_3.index.is_monotonic_increasing)
     assert_eq(s_3.index.is_monotonic_decreasing, ds_3.index.is_monotonic_decreasing)
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="pandas removed is_monotonic")
+@pytest.mark.skipif(PANDAS_GE_200, reason="pandas removed is_monotonic")
 def test_index_is_monotonic_deprecated():
     s = pd.Series(1, index=range(20))
     ds = dd.from_pandas(s, npartitions=5, sort=False)
     # `is_monotonic` was deprecated starting in `pandas=1.5.0`
     with _check_warning(
-        PANDAS_GT_150, FutureWarning, message="is_monotonic is deprecated"
+        PANDAS_GE_150, FutureWarning, message="is_monotonic is deprecated"
     ):
         expected = s.index.is_monotonic
     with _check_warning(
-        PANDAS_GT_150, FutureWarning, message="is_monotonic is deprecated"
+        PANDAS_GE_150, FutureWarning, message="is_monotonic is deprecated"
     ):
         result = ds.index.is_monotonic
     assert_eq(expected, result)
 
 
 def test_index_is_monotonic_dt64():
     s = pd.Series(1, index=pd.date_range("20130101", periods=20))
@@ -5887,15 +5888,15 @@
     assert all([not l.is_materialized() for l in s.dask.layers.values()])
     s.__repr__()
     s.to_frame().__repr__()
     assert all([not l.is_materialized() for l in s.dask.layers.values()])
 
 
 @pytest.mark.skipif(
-    not PANDAS_GT_150, reason="Requires native PyArrow-backed ExtensionArrays"
+    not PANDAS_GE_150, reason="Requires native PyArrow-backed ExtensionArrays"
 )
 @pytest.mark.parametrize(
     "dtype",
     [
         "int64[pyarrow]",
         "int32[pyarrow]",
         "float64[pyarrow]",
@@ -5910,15 +5911,15 @@
     ddf = dd.from_pandas(df, npartitions=3)
     expected = (df.x + df.x) * 2
     result = (ddf.x + ddf.x) * 2
     assert_eq(expected, result)
 
 
 @pytest.mark.skipif(
-    not PANDAS_GT_150, reason="Requires native PyArrow-backed ExtensionArrays"
+    not PANDAS_GE_150, reason="Requires native PyArrow-backed ExtensionArrays"
 )
 def test_pyarrow_decimal_extension_dtype():
     # Similar to `test_pyarrow_extension_dtype` but for pyarrow decimal dtypes
     pa = pytest.importorskip("pyarrow")
     pa_dtype = pa.decimal128(precision=7, scale=3)
 
     data = pa.array(
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_extensions.py` & `dask-2023.8.0/dask/dataframe/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_format.py` & `dask-2023.8.0/dask/dataframe/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_groupby.py` & `dask-2023.8.0/dask/dataframe/tests/test_groupby.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 import pandas as pd
 import pytest
 
 import dask
 import dask.dataframe as dd
 from dask.dataframe import _compat
 from dask.dataframe._compat import (
-    PANDAS_GT_140,
-    PANDAS_GT_150,
-    PANDAS_GT_200,
-    PANDAS_GT_210,
+    PANDAS_GE_140,
+    PANDAS_GE_150,
+    PANDAS_GE_200,
+    PANDAS_GE_210,
     check_nuisance_columns_warning,
     check_numeric_only_deprecation,
     check_observed_deprecation,
     tm,
 )
 from dask.dataframe._pyarrow import to_pyarrow_string
 from dask.dataframe.backends import grouper_dispatch
@@ -38,52 +38,52 @@
 from dask.utils_test import _check_warning, hlg_layer
 
 AGG_FUNCS = [
     "sum",
     pytest.param(
         "mean",
         marks=pytest.mark.xfail(
-            condition=PANDAS_GT_200,
+            condition=PANDAS_GE_200,
             reason="numeric_only=False not implemented",
             strict=False,
         ),
     ),
     "median",
     "min",
     "max",
     "count",
     "size",
     pytest.param(
         "std",
         marks=pytest.mark.xfail(
-            condition=PANDAS_GT_200,
+            condition=PANDAS_GE_200,
             reason="numeric_only=False not implemented",
             strict=False,
         ),
     ),
     pytest.param(
         "var",
         marks=pytest.mark.xfail(
-            condition=PANDAS_GT_200,
+            condition=PANDAS_GE_200,
             reason="numeric_only=False not implemented",
             strict=False,
         ),
     ),
     pytest.param(
         "cov",
         marks=pytest.mark.xfail(
-            condition=PANDAS_GT_200,
+            condition=PANDAS_GE_200,
             reason="numeric_only=False not implemented",
             strict=False,
         ),
     ),
     pytest.param(
         "corr",
         marks=pytest.mark.xfail(
-            condition=PANDAS_GT_200,
+            condition=PANDAS_GE_200,
             reason="numeric_only=False not implemented",
             strict=False,
         ),
     ),
     "nunique",
     "first",
     "last",
@@ -105,15 +105,15 @@
 def auto_shuffle_method(shuffle_method):
     yield
 
 
 @contextlib.contextmanager
 def groupby_axis_deprecated():
     ctx = contextlib.nullcontext()
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         ctx = pytest.warns(FutureWarning, match="axis")
     with ctx:
         yield
 
 
 @pytest.mark.xfail(reason="uncertain how to handle. See issue #3481.")
 def test_groupby_internal_repr_xfail():
@@ -484,15 +484,15 @@
     }
     meta = dsk[("x", 0)]
     ddf = dd.DataFrame(dsk, "x", meta, [0, 4, 9, 9])
     if categoricals:
         ddf = ddf.categorize(columns=["b"])
     pdf = ddf.compute()
 
-    if PANDAS_GT_210 and categoricals:
+    if PANDAS_GE_210 and categoricals:
         ctx = pytest.warns(FutureWarning, match="The default of observed=False")
     else:
         ctx = contextlib.nullcontext()
 
     with ctx:
         ddgrouped = ddf.groupby(by(ddf))
     with ctx:
@@ -1527,15 +1527,15 @@
         lambda df: df["a"],
         lambda df: df["a"] > 2,
         lambda df: [df["a"], df["b"]],
         lambda df: [df["a"] > 2],
         pytest.param(
             lambda df: [df["a"] > 2, df["b"] > 1],
             marks=pytest.mark.xfail(
-                not PANDAS_GT_150,
+                not PANDAS_GE_150,
                 reason="index dtype does not coincide: boolean != empty",
             ),
         ),
     ],
 )
 @pytest.mark.parametrize(
     "group_and_slice",
@@ -2187,27 +2187,27 @@
 
 @pytest.mark.parametrize(
     "func",
     [
         pytest.param(
             "var",
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="numeric_only=False not implemented"
+                PANDAS_GE_200, reason="numeric_only=False not implemented"
             ),
         ),
         pytest.param(
             "std",
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="numeric_only=False not implemented"
+                PANDAS_GE_200, reason="numeric_only=False not implemented"
             ),
         ),
         pytest.param(
             "mean",
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="numeric_only=False not implemented"
+                PANDAS_GE_200, reason="numeric_only=False not implemented"
             ),
         ),
         pytest.param(
             "sum",
             marks=pytest.mark.xfail_with_pyarrow_strings,
         ),
     ],
@@ -2220,15 +2220,15 @@
     # TODO: add deprecation warnings to match pandas
     ctx = contextlib.nullcontext()
     if func != "sum":
         ctx = check_nuisance_columns_warning()
     with ctx, check_numeric_only_deprecation():
         expected = getattr(df, func)()
     with _check_warning(
-        func in ["std", "var"] and not PANDAS_GT_200,
+        func in ["std", "var"] and not PANDAS_GE_200,
         FutureWarning,
         message="numeric_only",
     ):
         result = getattr(ddf, func)()
     assert_eq(expected, result)
 
     # DataFrameGroupBy
@@ -2551,18 +2551,18 @@
 
 @contextlib.contextmanager
 def groupby_axis_and_meta():
     # Because we're checking for multiple warnings, we need to record
     # all warnings and inspect them after the fact
     with pytest.warns() as record:
         yield
-    assert len(record) == 2 if PANDAS_GT_210 else 1, [x.message for x in record.list]
+    assert len(record) == 2 if PANDAS_GE_210 else 1, [x.message for x in record.list]
     assert record[-1].category is UserWarning
     assert "`meta` is not specified" in str(record[-1].message)
-    if PANDAS_GT_210:
+    if PANDAS_GE_210:
         assert record[0].category is FutureWarning
         assert "axis" in str(record[0].message)
 
 
 @pytest.mark.parametrize("npartitions", [1, 2, 5])
 @pytest.mark.parametrize("period", [1, -1, 10])
 @pytest.mark.parametrize("axis", [0, 1])
@@ -2762,15 +2762,15 @@
 
     # DataFrameGroupBy
     with check_observed_deprecation():
         expected = agg(grouping(pdf))
 
     observed_ctx = (
         pytest.warns(FutureWarning, match="observed")
-        if PANDAS_GT_210
+        if PANDAS_GE_210
         else contextlib.nullcontext()
     )
     with observed_ctx:
         result = agg(grouping(ddf))
         assert_eq(result, expected)
 
     # SeriesGroupBy
@@ -2946,15 +2946,15 @@
 @pytest.mark.gpu
 @pytest.mark.parametrize(
     "group_keys",
     [
         pytest.param(
             True,
             marks=pytest.mark.skipif(
-                not PANDAS_GT_150,
+                not PANDAS_GE_150,
                 reason="cudf and pandas behave differently",
             ),
         ),
         False,
     ],
 )
 def test_groupby_apply_cudf(group_keys):
@@ -2983,15 +2983,15 @@
 
 @pytest.mark.parametrize("sort", [True, False])
 def test_groupby_dropna_with_agg(sort):
     # https://github.com/dask/dask/issues/6986
     df = pd.DataFrame(
         {"id1": ["a", None, "b"], "id2": [1, 2, None], "v1": [4.5, 5.5, None]}
     )
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         expected = df.groupby(["id1", "id2"], dropna=False, sort=sort).agg("sum")
     else:
         # before 2.0, sort=False appears to be disregarded, but only when
         # grouping on index columns, which is what we do in dask groupby.
         # So we should expect sorted index levels even with sort=False.
         # Fixed in 2.0, possibly by https://github.com/pandas-dev/pandas/pull/49613
         expected = df.groupby(["id1", "id2"], dropna=False, sort=True).agg("sum")
@@ -3036,15 +3036,15 @@
             "c": [0, 1] * 4,
             "d": ["dog", "cat", "cat", "dog", "dog", "dog", "cat", "bird"],
         }
     ).fillna(0)
     df["e"] = df["d"].astype("category")
     ddf = dd.from_pandas(df, npartitions=3)
 
-    if column == ["b", "e"] and PANDAS_GT_210:
+    if column == ["b", "e"] and PANDAS_GE_210:
         ctx = pytest.warns(FutureWarning, match="observed")
     else:
         ctx = contextlib.nullcontext()
 
     with ctx:
         result_so1 = (
             ddf.groupby(column, sort=False).a.mean(split_out=1).compute().dropna()
@@ -3092,21 +3092,21 @@
 @pytest.mark.parametrize(
     "agg",
     [
         "count",
         pytest.param(
             "mean",
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="numeric_only=False not implemented", strict=False
+                PANDAS_GE_200, reason="numeric_only=False not implemented", strict=False
             ),
         ),
         pytest.param(
             "std",
             marks=pytest.mark.xfail(
-                PANDAS_GT_200, reason="numeric_only=False not implemented", strict=False
+                PANDAS_GE_200, reason="numeric_only=False not implemented", strict=False
             ),
         ),
     ],
 )
 @pytest.mark.parametrize("sort", [True, False])
 def test_groupby_sort_argument(by, agg, sort):
     df = pd.DataFrame(
@@ -3225,15 +3225,15 @@
         pytest.skip("Not implemented for DataFrameGroupBy yet.")
     if agg_func == "median" and isinstance(groupby, str):
         pytest.skip("Can't calculate median over categorical")
     if agg_func in ["sum", "count", "prod"] and groupby != "cat_1":
         pytest.skip("Gives zeros rather than nans.")
     if agg_func in ["std", "var"] and observed:
         pytest.skip("Can't calculate observed with all nans")
-    if agg_func in ["sum", "prod"] and PANDAS_GT_200:
+    if agg_func in ["sum", "prod"] and PANDAS_GE_200:
         pytest.xfail("Not implemented for category type with pandas 2.0")
 
     pdf = pd.DataFrame(
         {
             "cat_1": pd.Categorical(
                 list("AB"), categories=list("ABCDE"), ordered=ordered_cats
             ),
@@ -3245,15 +3245,15 @@
 
     if not known_cats:
         ddf["cat_1"] = ddf["cat_1"].cat.as_unknown()
         ddf["cat_2"] = ddf["cat_2"].cat.as_unknown()
 
     def agg(grp, **kwargs):
         if isinstance(grp, pd.core.groupby.DataFrameGroupBy) or (
-            PANDAS_GT_150 and not PANDAS_GT_200
+            PANDAS_GE_150 and not PANDAS_GE_200
         ):
             # with pandas 1.5, dask also raises a warning on default numeric_only
             ctx = check_numeric_only_deprecation
         else:
             ctx = contextlib.nullcontext
         with ctx():
             return getattr(grp, agg_func)(**kwargs)
@@ -3283,23 +3283,23 @@
         }
     )
 
     ddf = dd.from_pandas(pdf, npartitions=2)
     assert_eq(ddf.groupby("b").cov(), pdf.groupby("b").cov())
 
 
-@pytest.mark.skipif(not PANDAS_GT_150, reason="requires pandas >= 1.5.0")
+@pytest.mark.skipif(not PANDAS_GE_150, reason="requires pandas >= 1.5.0")
 def test_groupby_numeric_only_None_column_name():
     df = pd.DataFrame({"a": [1, 2, 3], None: ["a", "b", "c"]})
     ddf = dd.from_pandas(df, npartitions=1)
     with pytest.raises(NotImplementedError):
         ddf.groupby(lambda x: x).mean(numeric_only=False)
 
 
-@pytest.mark.skipif(not PANDAS_GT_140, reason="requires pandas >= 1.4.0")
+@pytest.mark.skipif(not PANDAS_GE_140, reason="requires pandas >= 1.4.0")
 @pytest.mark.parametrize("shuffle", [True, False])
 def test_dataframe_named_agg(shuffle):
     df = pd.DataFrame(
         {
             "a": [1, 1, 2, 2],
             "b": [1, 2, 5, 6],
             "c": [6, 3, 6, 7],
@@ -3315,15 +3315,15 @@
         shuffle=shuffle,
         x=pd.NamedAgg("b", aggfunc="sum"),
         y=pd.NamedAgg("c", aggfunc=partial(np.std, ddof=1)),
     )
     assert_eq(expected, actual)
 
 
-@pytest.mark.skipif(not PANDAS_GT_140, reason="requires pandas >= 1.4.0")
+@pytest.mark.skipif(not PANDAS_GE_140, reason="requires pandas >= 1.4.0")
 @pytest.mark.parametrize("shuffle", [True, False])
 @pytest.mark.parametrize("agg", ["count", "mean", partial(np.var, ddof=1)])
 def test_series_named_agg(shuffle, agg):
     df = pd.DataFrame(
         {
             "a": [5, 4, 3, 5, 4, 2, 3, 2],
             "b": [1, 2, 5, 6, 9, 2, 6, 8],
@@ -3523,15 +3523,15 @@
     ],
 )
 @pytest.mark.parametrize(
     "numeric_only",
     [None, True, False],
 )
 @pytest.mark.skipif(
-    not PANDAS_GT_150, reason="numeric_only not implemented for pandas < 1.5"
+    not PANDAS_GE_150, reason="numeric_only not implemented for pandas < 1.5"
 )
 def test_groupby_numeric_only_supported(func, numeric_only):
     pdf = pd.DataFrame(
         {
             "ints": [4, 4, 5, 5, 5],
             "ints2": [1, 2, 3, 4, 1],
             "dates": pd.date_range("2015-01-01", periods=5, freq="1T"),
@@ -3542,15 +3542,15 @@
 
     kwargs = {} if numeric_only is None else {"numeric_only": numeric_only}
 
     # Some groupby methods will raise deprecation warnings or TypeErrors
     # depending on the version of pandas being used. Here we check that
     # dask and panadas have similar behavior
     ctx = contextlib.nullcontext()
-    if PANDAS_GT_150 and not PANDAS_GT_200:
+    if PANDAS_GE_150 and not PANDAS_GE_200:
         if func in ("sum", "prod", "median"):
             if numeric_only is None:
                 ctx = pytest.warns(
                     FutureWarning, match="The default value of numeric_only"
                 )
             elif numeric_only is False:
                 ctx = pytest.warns(FutureWarning, match="Dropping invalid columns")
@@ -3559,15 +3559,16 @@
         with ctx:
             expected = getattr(pdf.groupby("ints"), func)(**kwargs)
         successful_compute = True
     except TypeError:
         # Make sure dask and pandas raise the same error message
         # We raise the error on _meta_nonempty, actual element may differ
         ctx = pytest.raises(
-            TypeError, match="Cannot convert|could not convert|does not support"
+            TypeError,
+            match="Cannot convert|could not convert|does not support|agg function failed",
         )
         successful_compute = False
 
     # Here's where we check that dask behaves the same as pandas
     with ctx:
         result = getattr(ddf.groupby("ints"), func)(**kwargs)
         if successful_compute:
@@ -3584,18 +3585,18 @@
 
     ctx = contextlib.nullcontext()
     ctx_warn = pytest.warns(FutureWarning, match="The default value of numeric_only")
     ctx_error = pytest.raises(
         NotImplementedError, match="'numeric_only=False' is not implemented in Dask"
     )
     if numeric_only is None:
-        if PANDAS_GT_150 and not PANDAS_GT_200:
+        if PANDAS_GE_150 and not PANDAS_GE_200:
             # Start warning about upcoming change to `numeric_only` default value
             ctx = ctx_warn
-        elif PANDAS_GT_200:
+        elif PANDAS_GE_200:
             # Default was changed to `numeric_only=False` in pandas 2.0
             ctx = ctx_error
     else:
         # Always error when `numeric_only=False`
         ctx = ctx_error
 
     # Here `numeric_only=None` means "use default value for `numeric_only`"
@@ -3623,26 +3624,26 @@
         "var",
     ],
 )
 def test_groupby_numeric_only_true(func):
     df = pd.DataFrame({"A": [1, 1, 2, 2], "B": [3, 4, 3, 4], "C": ["a", "b", "c", "d"]})
     ddf = dd.from_pandas(df, npartitions=2)
 
-    if func in ["var", "std", "cov", "corr"] and not PANDAS_GT_150:
+    if func in ["var", "std", "cov", "corr"] and not PANDAS_GE_150:
         with pytest.raises(TypeError, match="numeric_only not supported"):
             getattr(ddf.groupby("A"), func)(numeric_only=True)
         with pytest.raises(TypeError, match="got an unexpected keyword"):
             getattr(df.groupby("A"), func)(numeric_only=True)
     else:
         ddf_result = getattr(ddf.groupby("A"), func)(numeric_only=True)
         pdf_result = getattr(df.groupby("A"), func)(numeric_only=True)
         assert_eq(ddf_result, pdf_result)
 
 
-@pytest.mark.skipif(not PANDAS_GT_150, reason="numeric_only not supported for <1.5")
+@pytest.mark.skipif(not PANDAS_GE_150, reason="numeric_only not supported for <1.5")
 @pytest.mark.parametrize("func", ["cov", "corr"])
 def test_groupby_numeric_only_false_cov_corr(func):
     df = pd.DataFrame(
         {
             "float": [1.0, 2.0, 3.0, 4.0, 5, 6.0, 7.0, 8.0],
             "int": [1, 2, 3, 4, 5, 6, 7, 8],
             "timedelta": pd.to_timedelta([1, 2, 3, 4, 5, 6, 7, 8]),
@@ -3667,15 +3668,15 @@
             "float": [1.0, 2.0, 3.0, 4.0, np.nan, 6.0, 7.0, 8.0],
             "dt": [pd.NaT] + [datetime(2010, i, 1) for i in range(1, 8)],
             "A": 1,
         }
     )
     ddf = dd.from_pandas(df, npartitions=2)
 
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         ctx = pytest.raises(TypeError, match="does not support")
 
         with ctx:
             getattr(ddf.groupby("A"), func)(numeric_only=False)
         with ctx:
             getattr(df.groupby("A"), func)(numeric_only=False)
 
@@ -3688,15 +3689,15 @@
 
         with ctx:
             dd_result = getattr(ddf.groupby("A"), func)(numeric_only=False)
         with ctx:
             pd_result = getattr(df.groupby("A"), func)(numeric_only=False)
         assert_eq(dd_result, pd_result)
 
-        if PANDAS_GT_150:
+        if PANDAS_GE_150:
             ctx = pytest.warns(FutureWarning, match="default value of numeric_only")
         else:
             ctx = contextlib.nullcontext()
 
         with ctx:
             dd_result = getattr(ddf.groupby("A"), func)()
         with ctx:
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_hashing.py` & `dask-2023.8.0/dask/dataframe/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_hyperloglog.py` & `dask-2023.8.0/dask/dataframe/tests/test_hyperloglog.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_indexing.py` & `dask-2023.8.0/dask/dataframe/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_merge_column_and_index.py` & `dask-2023.8.0/dask/dataframe/tests/test_merge_column_and_index.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_multi.py` & `dask-2023.8.0/dask/dataframe/tests/test_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.api.types import is_object_dtype
 
 import dask.dataframe as dd
 from dask.base import compute_as_if_collection
-from dask.dataframe._compat import PANDAS_GT_140, PANDAS_GT_150, PANDAS_GT_200, tm
+from dask.dataframe._compat import PANDAS_GE_140, PANDAS_GE_150, PANDAS_GE_200, tm
 from dask.dataframe.core import _Frame
 from dask.dataframe.methods import concat
 from dask.dataframe.multi import (
     _maybe_align_partitions,
     align_partitions,
     concat_indexed_dataframes,
     hash_join,
@@ -2237,28 +2237,28 @@
 
     result = dd.concat([db2, db3])
     expected = pd.concat([b2, b3])
     assert_eq(result, expected)
 
 
 def check_append_with_warning(dask_obj, dask_append, pandas_obj, pandas_append):
-    if PANDAS_GT_140:
+    if PANDAS_GE_140:
         with pytest.warns(FutureWarning, match="append method is deprecated"):
             expected = pandas_obj.append(pandas_append)
             result = dask_obj.append(dask_append)
             assert_eq(result, expected)
     else:
         expected = pandas_obj.append(pandas_append)
         result = dask_obj.append(dask_append)
         assert_eq(result, expected)
 
     return result
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="pandas removed append")
+@pytest.mark.skipif(PANDAS_GE_200, reason="pandas removed append")
 def test_append():
     df = pd.DataFrame({"a": [1, 2, 3, 4, 5, 6], "b": [1, 2, 3, 4, 5, 6]})
     df2 = pd.DataFrame(
         {"a": [1, 2, 3, 4, 5, 6], "b": [1, 2, 3, 4, 5, 6]}, index=[6, 7, 8, 9, 10, 11]
     )
     df3 = pd.DataFrame(
         {"b": [1, 2, 3, 4, 5, 6], "c": [1, 2, 3, 4, 5, 6]}, index=[6, 7, 8, 9, 10, 11]
@@ -2282,15 +2282,15 @@
     check_append_with_warning(ddf, df2, df, df2)
     check_append_with_warning(ddf.a, df2.a, df.a, df2.a)
 
     check_append_with_warning(ddf, df3, df, df3)
     check_append_with_warning(ddf.a, df3.b, df.a, df3.b)
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="pandas removed append")
+@pytest.mark.skipif(PANDAS_GE_200, reason="pandas removed append")
 def test_append2():
     dsk = {
         ("x", 0): pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]}),
         ("x", 1): pd.DataFrame({"a": [4, 5, 6], "b": [3, 2, 1]}),
         ("x", 2): pd.DataFrame({"a": [7, 8, 9], "b": [0, 0, 0]}),
     }
     meta = make_meta({"a": "i8", "b": "i8"}, parent_meta=pd.DataFrame())
@@ -2325,15 +2325,15 @@
     check_append_with_warning(ddf2, df1, df2, df1)
 
     # different columns
     check_append_with_warning(ddf1, df3, df1, df3)
     check_append_with_warning(ddf3, df1, df3, df1)
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="pandas removed append")
+@pytest.mark.skipif(PANDAS_GE_200, reason="pandas removed append")
 def test_append_categorical():
     frames = [
         pd.DataFrame(
             {
                 "x": np.arange(5, 10),
                 "y": list("abbba"),
                 "z": np.arange(5, 10, dtype="f8"),
@@ -2374,15 +2374,15 @@
         assert has_known_categories(res.index) == known
         assert has_known_categories(res) == known
 
         res = check_append_with_warning(ddf1.index, ddf2.index, df1.index, df2.index)
         assert has_known_categories(res) == known
 
 
-@pytest.mark.skipif(PANDAS_GT_200, reason="pandas removed append")
+@pytest.mark.skipif(PANDAS_GE_200, reason="pandas removed append")
 def test_append_lose_divisions():
     df = pd.DataFrame({"x": [1, 2, 3, 4]}, index=[1, 2, 3, 4])
     ddf = dd.from_pandas(df, npartitions=2)
 
     res = check_append_with_warning(ddf, ddf, df, df)
     assert res.known_divisions is False
 
@@ -2528,22 +2528,22 @@
     "dtype",
     [
         "Int64",
         "Float64",
         pytest.param(
             "int64[pyarrow]",
             marks=pytest.mark.skipif(
-                pa is None or not PANDAS_GT_150,
+                pa is None or not PANDAS_GE_150,
                 reason="Support for ArrowDtypes requires pyarrow and pandas>=1.5.0",
             ),
         ),
         pytest.param(
             "float64[pyarrow]",
             marks=pytest.mark.skipif(
-                pa is None or not PANDAS_GT_150,
+                pa is None or not PANDAS_GE_150,
                 reason="Support for ArrowDtypes requires pyarrow and pandas>=1.5.0",
             ),
         ),
     ],
 )
 def test_nullable_types_merge(dtype):
     df1 = pd.DataFrame({"a": [1, 2, 3], "b": [1, 1, 3], "c": list("aab")})
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_numeric.py` & `dask-2023.8.0/dask/dataframe/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_optimize_dataframe.py` & `dask-2023.8.0/dask/dataframe/tests/test_optimize_dataframe.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_pyarrow.py` & `dask-2023.8.0/dask/dataframe/tests/test_pyarrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.tests.extension.decimal.array import DecimalDtype
 
-from dask.dataframe._compat import PANDAS_GT_140, PANDAS_GT_150
+from dask.dataframe._compat import PANDAS_GE_140, PANDAS_GE_150
 from dask.dataframe._pyarrow import (
     is_object_string_dataframe,
     is_object_string_dtype,
     is_object_string_index,
     is_object_string_series,
     is_pyarrow_string_dtype,
 )
@@ -25,26 +25,26 @@
         (np.dtype(int), False),
         (np.dtype(float), False),
         (pd.StringDtype("python"), False),
         (DecimalDtype(), False),
         pytest.param(
             pa.int64(),
             False,
-            marks=pytest.mark.skipif(not PANDAS_GT_150, reason="Needs pd.ArrowDtype"),
+            marks=pytest.mark.skipif(not PANDAS_GE_150, reason="Needs pd.ArrowDtype"),
         ),
         pytest.param(
             pa.float64(),
             False,
-            marks=pytest.mark.skipif(not PANDAS_GT_150, reason="Needs pd.ArrowDtype"),
+            marks=pytest.mark.skipif(not PANDAS_GE_150, reason="Needs pd.ArrowDtype"),
         ),
         (pd.StringDtype("pyarrow"), True),
         pytest.param(
             pa.string(),
             True,
-            marks=pytest.mark.skipif(not PANDAS_GT_150, reason="Needs pd.ArrowDtype"),
+            marks=pytest.mark.skipif(not PANDAS_GE_150, reason="Needs pd.ArrowDtype"),
         ),
     ],
 )
 def test_is_pyarrow_string_dtype(dtype, expected):
     if isinstance(dtype, pa.DataType):
         dtype = pd.ArrowDtype(dtype)
     assert is_pyarrow_string_dtype(dtype) is expected
@@ -58,26 +58,26 @@
         (np.dtype(int), False),
         (np.dtype(float), False),
         (pd.StringDtype("python"), True),
         (DecimalDtype(), False),
         pytest.param(
             pa.int64(),
             False,
-            marks=pytest.mark.skipif(not PANDAS_GT_150, reason="Needs pd.ArrowDtype"),
+            marks=pytest.mark.skipif(not PANDAS_GE_150, reason="Needs pd.ArrowDtype"),
         ),
         pytest.param(
             pa.float64(),
             False,
-            marks=pytest.mark.skipif(not PANDAS_GT_150, reason="Needs pd.ArrowDtype"),
+            marks=pytest.mark.skipif(not PANDAS_GE_150, reason="Needs pd.ArrowDtype"),
         ),
         (pd.StringDtype("pyarrow"), False),
         pytest.param(
             pa.string(),
             False,
-            marks=pytest.mark.skipif(not PANDAS_GT_150, reason="Needs pd.ArrowDtype"),
+            marks=pytest.mark.skipif(not PANDAS_GE_150, reason="Needs pd.ArrowDtype"),
         ),
     ],
 )
 def test_is_object_string_dtype(dtype, expected):
     if isinstance(dtype, pa.DataType):
         dtype = pd.ArrowDtype(dtype)
     assert is_object_string_dtype(dtype) is expected
@@ -87,15 +87,15 @@
     "index,expected",
     [
         (pd.Index(["a", "b"], dtype=object), True),
         (pd.Index(["a", "b"], dtype="string[python]"), True),
         # Prior to pandas=1.4, Index couldn't contain extension dtypes
         (
             pd.Index(["a", "b"], dtype="string[pyarrow]"),
-            False if PANDAS_GT_140 else True,
+            False if PANDAS_GE_140 else True,
         ),
         (pd.Index([1, 2], dtype=int), False),
         (pd.Index([1, 2], dtype=float), False),
         (pd.Series(["a", "b"], dtype=object), False),
         (
             pd.MultiIndex.from_arrays(
                 [
@@ -109,15 +109,15 @@
         (
             pd.MultiIndex.from_arrays(
                 [
                     pd.Index(["a", "a"], dtype="string[pyarrow]"),
                     pd.Index(["a", "b"], dtype="string[pyarrow]"),
                 ]
             ),
-            False if PANDAS_GT_140 else True,
+            False if PANDAS_GE_140 else True,
         ),
         (
             pd.MultiIndex.from_arrays(
                 [pd.Index(["a", "a"], dtype=object), pd.Index([1, 2], dtype=int)]
             ),
             True,
         ),
@@ -146,15 +146,15 @@
             True,
         ),
         (
             pd.Series(
                 [1, 2], dtype=float, index=pd.Index(["a", "b"], dtype="string[pyarrow]")
             ),
             # Prior to pandas=1.4, Index couldn't contain extension dtypes
-            False if PANDAS_GT_140 else True,
+            False if PANDAS_GE_140 else True,
         ),
         (pd.Index(["a", "b"], dtype=object), False),
     ],
 )
 def test_is_object_string_series(series, expected):
     assert is_object_string_series(series) is expected
 
@@ -176,15 +176,15 @@
         (
             pd.DataFrame(
                 {"x": [1, 2]},
                 dtype=float,
                 index=pd.Index(["a", "b"], dtype="string[pyarrow]"),
             ),
             # Prior to pandas=1.4, Index couldn't contain extension dtypes
-            False if PANDAS_GT_140 else True,
+            False if PANDAS_GE_140 else True,
         ),
         (pd.Series({"x": ["a", "b"]}, dtype=object), False),
         (pd.Index({"x": ["a", "b"]}, dtype=object), False),
         (
             pd.MultiIndex.from_arrays(
                 [pd.Index(["a", "a"], dtype=object), pd.Index(["a", "b"], dtype=object)]
             ),
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_pyarrow_compat.py` & `dask-2023.8.0/dask/dataframe/tests/test_pyarrow_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 import pandas as pd
 import pandas._testing as tm
 import pytest
 
 pa = pytest.importorskip("pyarrow")
 
-from dask.dataframe._compat import PANDAS_GT_150
+from dask.dataframe._compat import PANDAS_GE_150
 
 # Tests are from https://github.com/pandas-dev/pandas/pull/49078
 
 
 @pytest.fixture
 def data(dtype):
-    if PANDAS_GT_150:
+    if PANDAS_GE_150:
         pa_dtype = dtype.pyarrow_dtype
     else:
         pa_dtype = pa.string()
     if pa.types.is_boolean(pa_dtype):
         data = [True, False] * 4 + [None] + [True, False] * 44 + [None] + [True, False]
     elif pa.types.is_floating(pa_dtype):
         data = [1.0, 0.0] * 4 + [None] + [-2.0, -1.0] * 44 + [None] + [0.5, 99.5]
@@ -74,20 +74,20 @@
     elif pa.types.is_binary(pa_dtype):
         data = [b"a", b"b"] * 4 + [None] + [b"1", b"2"] * 44 + [None] + [b"!", b">"]
     else:
         raise NotImplementedError
     return pd.array(data * 100, dtype=dtype)
 
 
-PYARROW_TYPES = tm.ALL_PYARROW_DTYPES if PANDAS_GT_150 else [pa.string()]
+PYARROW_TYPES = tm.ALL_PYARROW_DTYPES if PANDAS_GE_150 else [pa.string()]
 
 
 @pytest.fixture(params=PYARROW_TYPES, ids=str)
 def dtype(request):
-    if PANDAS_GT_150:
+    if PANDAS_GE_150:
         return pd.ArrowDtype(pyarrow_dtype=request.param)
     else:
         return pd.StringDtype("pyarrow")
 
 
 def test_pickle_roundtrip(data):
     expected = pd.Series(data)
@@ -107,15 +107,15 @@
 
 @pytest.mark.parametrize(
     "string_dtype",
     [
         "stringdtype",
         pytest.param(
             "arrowdtype",
-            marks=pytest.mark.skipif(not PANDAS_GT_150, reason="Requires ArrowDtype"),
+            marks=pytest.mark.skipif(not PANDAS_GE_150, reason="Requires ArrowDtype"),
         ),
     ],
 )
 def test_pickle_roundtrip_pyarrow_string_implementations(string_dtype):
     # There are two pyarrow string implementations in pandas.
     # This tests that both implementations have similar serialization performance.
     if string_dtype == "stringdtype":
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_reshape.py` & `dask-2023.8.0/dask/dataframe/tests/test_reshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     exp = pd.get_dummies(s, dummy_na=True)
     res = dd.get_dummies(ds, dummy_na=True)
     assert_eq(res, exp)
 
 
 def check_pandas_issue_45618_warning(test_func):
     # Check for FutureWarning raised in `pandas=1.4.0`-only.
-    # This can be removed when `pandas=1.4.0` is no longer supported (PANDAS_GT_140).
+    # This can be removed when `pandas=1.4.0` is no longer supported (PANDAS_GE_140).
     # See https://github.com/pandas-dev/pandas/issues/45618 for more details.
 
     def decorator():
         with warnings.catch_warnings(record=True) as record:
             test_func()
         if PANDAS_VERSION == parse_version("1.4.0"):
             assert all(
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_rolling.py` & `dask-2023.8.0/dask/dataframe/tests/test_rolling.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import dask.dataframe as dd
 import dask.dataframe.rolling
-from dask.dataframe._compat import PANDAS_GT_210
+from dask.dataframe._compat import PANDAS_GE_210
 from dask.dataframe.utils import assert_eq
 
 N = 40
 df = pd.DataFrame(
     {
         "a": np.random.randn(N).cumsum(),
         "b": np.random.randint(100, size=(N,)),
@@ -359,15 +359,15 @@
 )
 def test_rolling_axis(kwargs):
     df = pd.DataFrame(np.random.randn(20, 16))
     ddf = dd.from_pandas(df, npartitions=3)
 
     ctx = (
         pytest.warns(FutureWarning, match="The 'axis' keyword|Support for axis")
-        if PANDAS_GT_210
+        if PANDAS_GE_210
         else contextlib.nullcontext()
     )
     if kwargs["axis"] == "series":
         # Series
         with ctx:
             expected = df[3].rolling(5, axis=0).std()
         with ctx:
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_shuffle.py` & `dask-2023.8.0/dask/dataframe/tests/test_shuffle.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import pandas as pd
 import pytest
 
 import dask
 import dask.dataframe as dd
 from dask.base import compute_as_if_collection
 from dask.dataframe._compat import (
-    PANDAS_GT_140,
-    PANDAS_GT_150,
-    PANDAS_GT_200,
+    PANDAS_GE_140,
+    PANDAS_GE_150,
+    PANDAS_GE_200,
     assert_categorical_equal,
     tm,
 )
 from dask.dataframe.shuffle import (
     _calculate_divisions,
     _noop,
     maybe_buffered_partd,
@@ -198,15 +198,15 @@
             "z": np.random.choice(names, 100),
         },
         index=np.random.random(100),
     )
     # Ensure extension dtypes work
     # NOTE: Older version of pandas have known issues with extension dtypes.
     # We generally expect extension dtypes to work well when using `pandas>=1.4.0`.
-    if PANDAS_GT_140:
+    if PANDAS_GE_140:
         df = df.astype({"x": "Float64", "z": "string"})
 
     ddf = dd.from_pandas(df, npartitions=npartitions)
 
     assert_eq(df.set_index("x"), ddf.set_index("x", shuffle=shuffle_method))
     assert_eq(df.set_index("y"), ddf.set_index("y", shuffle=shuffle_method))
     assert_eq(df.set_index("z"), ddf.set_index("z", shuffle=shuffle_method))
@@ -214,15 +214,15 @@
     assert_eq(
         df.set_index(df.x + df.y), ddf.set_index(ddf.x + ddf.y, shuffle=shuffle_method)
     )
     assert_eq(df.set_index(df.x + 1), ddf.set_index(ddf.x + 1, shuffle=shuffle_method))
 
 
 @pytest.mark.skipif(
-    not PANDAS_GT_150, reason="Only test `string[pyarrow]` on recent versions of pandas"
+    not PANDAS_GE_150, reason="Only test `string[pyarrow]` on recent versions of pandas"
 )
 @pytest.mark.parametrize(
     "string_dtype", ["string[python]", "string[pyarrow]", "object"]
 )
 def test_set_index_string(shuffle_method, string_dtype):
     if string_dtype == "string[pyarrow]":
         pytest.importorskip("pyarrow")
@@ -1116,15 +1116,15 @@
         assert ts1.timetuple() == ts2.timetuple()
         assert ts1.tz == ts2.tz
 
     assert_eq(df2, ddf_new_div, check_freq=False)
     assert_eq(df2, ddf.set_index("A"), check_freq=False)
 
 
-@pytest.mark.skipif(not PANDAS_GT_140, reason="EA Indexes not supported before")
+@pytest.mark.skipif(not PANDAS_GE_140, reason="EA Indexes not supported before")
 def test_set_index_ea_dtype():
     pdf = pd.DataFrame({"a": 1, "b": pd.Series([1, 2], dtype="Int64")})
     ddf = dd.from_pandas(pdf, npartitions=2)
     pdf_result = pdf.set_index("b")
     ddf_result = ddf.set_index("b")
     assert_eq(ddf_result, pdf_result)
 
@@ -1585,15 +1585,15 @@
     assert divisions == expected[0]
     assert mins == expected[1]
     assert maxes == expected[2]
     assert presorted == expected[3]
 
 
 @pytest.mark.skipif(pa is None, reason="Need pyarrow")
-@pytest.mark.skipif(not PANDAS_GT_200, reason="dtype support not good before 2.0")
+@pytest.mark.skipif(not PANDAS_GE_200, reason="dtype support not good before 2.0")
 @pytest.mark.parametrize(
     "data, dtype",
     [
         (["a", "b"], "string[pyarrow]"),
         ([b"a", b"b"], "binary[pyarrow]"),
         # Should probably fix upstream, https://github.com/pandas-dev/pandas/issues/52590
         # (["a", "b"], pa.large_string()),
```

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_ufunc.py` & `dask-2023.8.0/dask/dataframe/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/tests/test_utils_dataframe.py` & `dask-2023.8.0/dask/dataframe/tests/test_utils_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 from packaging.version import Version
 
 import dask
 import dask.dataframe as dd
-from dask.dataframe._compat import PANDAS_GT_200, tm
+from dask.dataframe._compat import PANDAS_GE_200, tm
 from dask.dataframe.core import apply_and_enforce
 from dask.dataframe.utils import (
     UNKNOWN_CATEGORIES,
     assert_eq,
     check_matching_columns,
     check_meta,
     is_dataframe_like,
@@ -269,15 +269,15 @@
     res = meta_nonempty(idx)
     assert type(res) is pd.RangeIndex
     assert res.name == idx.name
 
     idx = pd.Index([1], name="foo", dtype="int")
     res = meta_nonempty(idx)
     assert type(res) is type(idx)
-    if PANDAS_GT_200:
+    if PANDAS_GE_200:
         assert res.dtype == np.int_
     else:
         # before pandas 2.0, index dtypes were only x64
         assert res.dtype == "int64"
     assert res.name == idx.name
 
     idx = pd.Index(["a"], name="foo")
@@ -679,15 +679,15 @@
     try:
         import pyarrow as pa
     except ImportError:
         pa = None
 
     # If `pandas>=2` and `pyarrow>=12` are installed, then default to using pyarrow strings
     if (
-        PANDAS_GT_200
+        PANDAS_GE_200
         and pa is not None
         and Version(pa.__version__) >= Version("12.0.0")
     ):
         assert pyarrow_strings_enabled() is True
     else:
         assert pyarrow_strings_enabled() is False
```

### Comparing `dask-2023.7.1/dask/dataframe/tseries/resample.py` & `dask-2023.8.0/dask/dataframe/tseries/resample.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pandas as pd
 from pandas.core.resample import Resampler as pd_Resampler
 
 from dask.base import tokenize
 from dask.dataframe import methods
-from dask.dataframe._compat import PANDAS_GT_140
+from dask.dataframe._compat import PANDAS_GE_140
 from dask.dataframe.core import DataFrame, Series
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import derived_from
 
 
 def _resample_series(
     series,
@@ -24,15 +24,15 @@
     how_args,
     how_kwargs,
 ):
     out = getattr(series.resample(rule, **resample_kwargs), how)(
         *how_args, **how_kwargs
     )
 
-    if PANDAS_GT_140:
+    if PANDAS_GE_140:
         if reindex_closed is None:
             inclusive = "both"
         else:
             inclusive = reindex_closed
         closed_kwargs = {"inclusive": inclusive}
     else:
         closed_kwargs = {"closed": reindex_closed}
```

### Comparing `dask-2023.7.1/dask/dataframe/tseries/tests/test_resample.py` & `dask-2023.8.0/dask/dataframe/tseries/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dataframe/utils.py` & `dask-2023.8.0/dask/dataframe/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import dask
 from dask.base import get_scheduler, is_dask_collection
 from dask.core import get_deps
 from dask.dataframe import (  # noqa: F401 register pandas extension types
     _dtypes,
     methods,
 )
-from dask.dataframe._compat import PANDAS_GT_150, tm  # noqa: F401
+from dask.dataframe._compat import PANDAS_GE_150, tm  # noqa: F401
 from dask.dataframe.dispatch import (  # noqa : F401
     make_meta,
     make_meta_obj,
     meta_nonempty,
 )
 from dask.dataframe.extensions import make_scalar
 from dask.utils import (
@@ -847,14 +847,14 @@
 
     return {} if numeric_only is no_default else {"numeric_only": numeric_only}
 
 
 def check_numeric_only_valid(numeric_only, name: str) -> dict:
     from dask.dataframe.core import no_default  # Avoid circular import
 
-    if PANDAS_GT_150 and numeric_only is not no_default:
+    if PANDAS_GE_150 and numeric_only is not no_default:
         return {"numeric_only": numeric_only}
     elif numeric_only is no_default:
         return {}
     raise NotImplementedError(
         f"numeric_only is not implemented for {name} for pandas < 1.5."
     )
```

### Comparing `dask-2023.7.1/dask/datasets.py` & `dask-2023.8.0/dask/datasets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/delayed.py` & `dask-2023.8.0/dask/delayed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/diagnostics/profile.py` & `dask-2023.8.0/dask/diagnostics/profile.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/diagnostics/profile_visualize.py` & `dask-2023.8.0/dask/diagnostics/profile_visualize.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/diagnostics/progress.py` & `dask-2023.8.0/dask/diagnostics/progress.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/diagnostics/tests/test_profiler.py` & `dask-2023.8.0/dask/diagnostics/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/diagnostics/tests/test_progress.py` & `dask-2023.8.0/dask/diagnostics/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/distributed.py` & `dask-2023.8.0/dask/distributed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/dot.py` & `dask-2023.8.0/dask/dot.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/graph_manipulation.py` & `dask-2023.8.0/dask/graph_manipulation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/hashing.py` & `dask-2023.8.0/dask/hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/highlevelgraph.py` & `dask-2023.8.0/dask/highlevelgraph.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/layers.py` & `dask-2023.8.0/dask/layers.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/local.py` & `dask-2023.8.0/dask/local.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/multiprocessing.py` & `dask-2023.8.0/dask/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/optimization.py` & `dask-2023.8.0/dask/optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/order.py` & `dask-2023.8.0/dask/order.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/rewrite.py` & `dask-2023.8.0/dask/rewrite.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/sizeof.py` & `dask-2023.8.0/dask/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/system.py` & `dask-2023.8.0/dask/system.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_backends.py` & `dask-2023.8.0/dask/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_base.py` & `dask-2023.8.0/dask/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_cache.py` & `dask-2023.8.0/dask/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_callbacks.py` & `dask-2023.8.0/dask/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_ci.py` & `dask-2023.8.0/dask/tests/test_ci.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_cli.py` & `dask-2023.8.0/dask/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_config.py` & `dask-2023.8.0/dask/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_context.py` & `dask-2023.8.0/dask/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_core.py` & `dask-2023.8.0/dask/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_datasets.py` & `dask-2023.8.0/dask/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_delayed.py` & `dask-2023.8.0/dask/tests/test_delayed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_distributed.py` & `dask-2023.8.0/dask/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_docs.py` & `dask-2023.8.0/dask/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_dot.py` & `dask-2023.8.0/dask/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_graph_manipulation.py` & `dask-2023.8.0/dask/tests/test_graph_manipulation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_hashing.py` & `dask-2023.8.0/dask/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_highgraph.py` & `dask-2023.8.0/dask/tests/test_highgraph.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_layers.py` & `dask-2023.8.0/dask/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_local.py` & `dask-2023.8.0/dask/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_multiprocessing.py` & `dask-2023.8.0/dask/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_optimization.py` & `dask-2023.8.0/dask/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_order.py` & `dask-2023.8.0/dask/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_rewrite.py` & `dask-2023.8.0/dask/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_sizeof.py` & `dask-2023.8.0/dask/tests/test_sizeof.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_spark_compat.py` & `dask-2023.8.0/dask/tests/test_spark_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 pyspark = pytest.importorskip("pyspark")
 pa = pytest.importorskip("pyarrow")
 pytest.importorskip("fastparquet")
 
 import numpy as np
 import pandas as pd
 
-from dask.dataframe._compat import PANDAS_GT_150, PANDAS_GT_200
+from dask.dataframe._compat import PANDAS_GE_150, PANDAS_GE_200
 from dask.dataframe.utils import assert_eq
 
 pytestmark = [
     pytest.mark.skipif(
         sys.platform != "linux",
         reason="Unnecessary, and hard to get spark working on non-linux platforms",
     ),
     pytest.mark.skipif(
-        PANDAS_GT_200,
+        PANDAS_GE_200,
         reason="pyspark doesn't yet have support for pandas 2.0",
     ),
     # we only test with pyarrow strings and pandas 2.0
     pytest.mark.skip_with_pyarrow_strings,  # pyspark doesn't support pandas 2.0
 ]
 
 # pyspark auto-converts timezones -- round-tripping timestamps is easier if
@@ -159,15 +159,15 @@
     ddf = dd.read_parquet(tmpdir, engine="pyarrow", dtype_backend="numpy_nullable")
     assert all(
         [pd.api.types.is_extension_array_dtype(dtype) for dtype in ddf.dtypes]
     ), ddf.dtypes
     assert_eq(ddf, pdf, check_index=False)
 
 
-@pytest.mark.skipif(not PANDAS_GT_150, reason="Requires pyarrow-backed nullable dtypes")
+@pytest.mark.skipif(not PANDAS_GE_150, reason="Requires pyarrow-backed nullable dtypes")
 def test_read_decimal_dtype_pyarrow(spark_session, tmpdir):
     tmpdir = str(tmpdir)
     npartitions = 3
     size = 6
 
     decimal_data = [
         decimal.Decimal("8093.234"),
```

### Comparing `dask-2023.7.1/dask/tests/test_system.py` & `dask-2023.8.0/dask/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_threaded.py` & `dask-2023.8.0/dask/tests/test_threaded.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_typing.py` & `dask-2023.8.0/dask/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_utils.py` & `dask-2023.8.0/dask/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/tests/test_utils_test.py` & `dask-2023.8.0/dask/tests/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/threaded.py` & `dask-2023.8.0/dask/threaded.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/typing.py` & `dask-2023.8.0/dask/typing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/utils.py` & `dask-2023.8.0/dask/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/utils_test.py` & `dask-2023.8.0/dask/utils_test.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/widgets/__init__.py` & `dask-2023.8.0/dask/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/widgets/templates/array.html.j2` & `dask-2023.8.0/dask/widgets/templates/array.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/widgets/templates/highlevelgraph.html.j2` & `dask-2023.8.0/dask/widgets/templates/highlevelgraph.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/widgets/templates/highlevelgraph_layer.html.j2` & `dask-2023.8.0/dask/widgets/templates/highlevelgraph_layer.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/widgets/tests/test_widgets.py` & `dask-2023.8.0/dask/widgets/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask/widgets/widgets.py` & `dask-2023.8.0/dask/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/dask.egg-info/PKG-INFO` & `dask-2023.8.0/dask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dask
-Version: 2023.7.1
+Version: 2023.8.0
 Summary: Parallel PyData with Task Scheduling
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
-License: BSD
+License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/dask/dask/
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `dask-2023.7.1/dask.egg-info/SOURCES.txt` & `dask-2023.8.0/dask.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,15 @@
 docs/source/array-api.rst
 docs/source/array-assignment.rst
 docs/source/array-best-practices.rst
 docs/source/array-chunks.rst
 docs/source/array-creation.rst
 docs/source/array-design.rst
 docs/source/array-gufunc.rst
+docs/source/array-numpy-compatibility.rst
 docs/source/array-overlap.rst
 docs/source/array-random.rst
 docs/source/array-slicing.rst
 docs/source/array-sparse.rst
 docs/source/array-stack.rst
 docs/source/array-stats.rst
 docs/source/array.rst
```

### Comparing `dask-2023.7.1/docs/Makefile` & `dask-2023.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/make.bat` & `dask-2023.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/10-minutes-to-dask.rst` & `dask-2023.8.0/docs/source/10-minutes-to-dask.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/config_converter.js` & `dask-2023.8.0/docs/source/_static/config_converter.js`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/dask-simple.png` & `dask-2023.8.0/docs/source/_static/dask-simple.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/main-page.css` & `dask-2023.8.0/docs/source/_static/main-page.css`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/profile.html` & `dask-2023.8.0/docs/source/_static/profile.html`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/stacked_profile.html` & `dask-2023.8.0/docs/source/_static/stacked_profile.html`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/style.css` & `dask-2023.8.0/docs/source/_static/style.css`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/transpose_cyto.html` & `dask-2023.8.0/docs/source/_static/transpose_cyto.html`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/_static/yaml.min.js` & `dask-2023.8.0/docs/source/_static/yaml.min.js`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/api.rst` & `dask-2023.8.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-api.rst` & `dask-2023.8.0/docs/source/array-api.rst`

 * *Files 8% similar despite different names*

```diff
@@ -62,29 +62,33 @@
    cosh
    count_nonzero
    cov
    cumprod
    cumsum
    deg2rad
    degrees
+   delete
    diag
    diagonal
    diff
+   divide
    divmod
    digitize
    dot
    dstack
    ediff1d
    einsum
    empty
    empty_like
    equal
    exp
    exp2
+   expand_dims
    expm1
+   extract
    eye
    fabs
    fix
    flatnonzero
    flip
    flipud
    fliplr
@@ -103,14 +107,15 @@
    greater
    greater_equal
    histogram
    histogram2d
    histogramdd
    hstack
    hypot
+   i0
    imag
    indices
    insert
    invert
    isclose
    iscomplex
    isfinite
@@ -120,14 +125,15 @@
    isnan
    isnull
    isposinf
    isreal
    ldexp
    left_shift
    less
+   less_equal
    linspace
    log
    log10
    log1p
    log2
    logaddexp
    logaddexp2
@@ -178,14 +184,15 @@
    positive
    power
    prod
    ptp
    rad2deg
    radians
    ravel
+   ravel_multi_index
    real
    reciprocal
    rechunk
    reduction
    register_chunk_type
    remainder
    repeat
@@ -194,38 +201,48 @@
    right_shift
    rint
    roll
    rollaxis
    rot90
    round
    searchsorted
+   select
+   shape
    sign
    signbit
    sin
    sinc
    sinh
+   spacing
    sqrt
    square
    squeeze
    stack
    std
    subtract
    sum
+   swapaxes
    take
    tan
    tanh
    tensordot
    tile
    topk
    trace
    transpose
-   true_divide
+   tri
    tril
+   tril_indices
+   tril_indices_from
    triu
+   triu_indices
+   triu_indices_from
+   true_divide
    trunc
+   union1d
    unique
    unravel_index
    var
    vdot
    vstack
    where
    zeros
```

### Comparing `dask-2023.7.1/docs/source/array-assignment.rst` & `dask-2023.8.0/docs/source/array-assignment.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-best-practices.rst` & `dask-2023.8.0/docs/source/array-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-chunks.rst` & `dask-2023.8.0/docs/source/array-chunks.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-creation.rst` & `dask-2023.8.0/docs/source/array-creation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-design.rst` & `dask-2023.8.0/docs/source/array-design.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-gufunc.rst` & `dask-2023.8.0/docs/source/array-gufunc.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-overlap.rst` & `dask-2023.8.0/docs/source/array-overlap.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-random.rst` & `dask-2023.8.0/docs/source/array-random.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-slicing.rst` & `dask-2023.8.0/docs/source/array-slicing.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-sparse.rst` & `dask-2023.8.0/docs/source/array-sparse.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-stack.rst` & `dask-2023.8.0/docs/source/array-stack.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array-stats.rst` & `dask-2023.8.0/docs/source/array-stats.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/array.rst` & `dask-2023.8.0/docs/source/array.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
    array-stats.rst
    array-slicing.rst
    array-assignment.rst
    array-stack.rst
    array-gufunc.rst
    array-random.rst
    array-api.rst
+   array-numpy-compatibility.rst
 
 Dask Array implements a subset of the NumPy ndarray interface using blocked
 algorithms, cutting up the large array into many small arrays. This lets us
 compute on arrays larger than memory using all of our cores.  We coordinate
 these blocked algorithms using Dask graphs.
 
 .. raw:: html
```

### Comparing `dask-2023.7.1/docs/source/bag-api.rst` & `dask-2023.8.0/docs/source/bag-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/bag-creation.rst` & `dask-2023.8.0/docs/source/bag-creation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/bag.rst` & `dask-2023.8.0/docs/source/bag.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/best-practices.rst` & `dask-2023.8.0/docs/source/best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/caching.rst` & `dask-2023.8.0/docs/source/caching.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/changelog.rst` & `dask-2023.8.0/docs/source/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 Changelog
 =========
 
+.. _v2023.8.0:
+
+2023.8.0
+--------
+
+Released on August 4, 2023
+
+Enhancements
+^^^^^^^^^^^^
+- Fix for ``make_timeseries`` performance regression (:pr:`10428`) `Irina Truong`_
+
+Documentation
+^^^^^^^^^^^^^
+- Add ``distributed.print`` to debugging docs (:pr:`10435`) `James Bourbeau`_
+- Documenting compatibility of NumPy functions with Dask functions (:pr:`9941`) `Chiara Marmo`_
+
+Maintenance
+^^^^^^^^^^^
+- Use SPDX in ``license`` metadata (:pr:`10437`) `John A Kirkham`_
+- Require ``dask[array]`` in ``dask[dataframe]`` (:pr:`10357`) `John A Kirkham`_
+- Update gpuCI ``RAPIDS_VER`` to ``23.10`` (:pr:`10427`)
+- Simplify compatibility code (:pr:`10426`) `Hendrik Makait`_
+- Fix compatibility variable naming (:pr:`10424`) `Hendrik Makait`_
+- Fix a few errors with upstream ``pandas`` and ``pyarrow`` (:pr:`10412`) `Irina Truong`_
+
+
 .. _v2023.7.1:
 
 2023.7.1
 --------
 
 Released on July 20, 2023
```

### Comparing `dask-2023.7.1/docs/source/cli.rst` & `dask-2023.8.0/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/conf.py` & `dask-2023.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/configuration.rst` & `dask-2023.8.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/custom-collections.rst` & `dask-2023.8.0/docs/source/custom-collections.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/custom-graphs.rst` & `dask-2023.8.0/docs/source/custom-graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dashboard-progress-script.py` & `dask-2023.8.0/docs/source/dashboard-progress-script.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dashboard.rst` & `dask-2023.8.0/docs/source/dashboard.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/daskcheatsheet.pdf` & `dask-2023.8.0/docs/source/daskcheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-api.rst` & `dask-2023.8.0/docs/source/dataframe-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-best-practices.rst` & `dask-2023.8.0/docs/source/dataframe-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-categoricals.rst` & `dask-2023.8.0/docs/source/dataframe-categoricals.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-create.rst` & `dask-2023.8.0/docs/source/dataframe-create.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-design.rst` & `dask-2023.8.0/docs/source/dataframe-design.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-extend.rst` & `dask-2023.8.0/docs/source/dataframe-extend.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-groupby.rst` & `dask-2023.8.0/docs/source/dataframe-groupby.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-indexing.rst` & `dask-2023.8.0/docs/source/dataframe-indexing.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-joins.rst` & `dask-2023.8.0/docs/source/dataframe-joins.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-parquet.rst` & `dask-2023.8.0/docs/source/dataframe-parquet.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe-sql.rst` & `dask-2023.8.0/docs/source/dataframe-sql.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/dataframe.rst` & `dask-2023.8.0/docs/source/dataframe.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/delayed-api.rst` & `dask-2023.8.0/docs/source/delayed-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/delayed-best-practices.rst` & `dask-2023.8.0/docs/source/delayed-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/delayed-collections.rst` & `dask-2023.8.0/docs/source/delayed-collections.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/delayed.rst` & `dask-2023.8.0/docs/source/delayed.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-cli.rst` & `dask-2023.8.0/docs/source/deploying-cli.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-cloud.rst` & `dask-2023.8.0/docs/source/deploying-cloud.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-docker.rst` & `dask-2023.8.0/docs/source/deploying-docker.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-hpc.rst` & `dask-2023.8.0/docs/source/deploying-hpc.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-kubernetes.rst` & `dask-2023.8.0/docs/source/deploying-kubernetes.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-python-advanced.rst` & `dask-2023.8.0/docs/source/deploying-python-advanced.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-python.rst` & `dask-2023.8.0/docs/source/deploying-python.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying-ssh.rst` & `dask-2023.8.0/docs/source/deploying-ssh.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deploying.rst` & `dask-2023.8.0/docs/source/deploying.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/deployment-considerations.rst` & `dask-2023.8.0/docs/source/deployment-considerations.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/develop.rst` & `dask-2023.8.0/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/diagnostics-distributed.rst` & `dask-2023.8.0/docs/source/diagnostics-distributed.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/diagnostics-local.rst` & `dask-2023.8.0/docs/source/diagnostics-local.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/ecosystem.rst` & `dask-2023.8.0/docs/source/ecosystem.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/faq.rst` & `dask-2023.8.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/futures.rst` & `dask-2023.8.0/docs/source/futures.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/gpu.rst` & `dask-2023.8.0/docs/source/gpu.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/graph_manipulation.rst` & `dask-2023.8.0/docs/source/graph_manipulation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/graphs.rst` & `dask-2023.8.0/docs/source/graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/graphviz.rst` & `dask-2023.8.0/docs/source/graphviz.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/high-level-graphs.rst` & `dask-2023.8.0/docs/source/high-level-graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/how-to/adaptive.rst` & `dask-2023.8.0/docs/source/how-to/adaptive.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/how-to/connect-to-remote-data.rst` & `dask-2023.8.0/docs/source/how-to/connect-to-remote-data.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/how-to/customize-initialization.rst` & `dask-2023.8.0/docs/source/how-to/customize-initialization.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/how-to/debug.rst` & `dask-2023.8.0/docs/source/how-to/debug.rst`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 
 Dask has a variety of mechanisms to make this process easier.  Depending on
 your situation, some of these approaches may be more appropriate than others.
 
 These approaches are ordered from lightweight or easy solutions to more
 involved solutions.
 
+Printing
+--------
+
+One of the most basic methods of debugging is to simply print values and inspect them.
+However, when using Python's built-in :func:`print` function with Dask, those prints
+often happen on remote machines instead of in the user's Python session, which typically
+isn't the experience developers want when debugging.
+
+Because of this, Dask offers a :func:`dask.distributed.print <distributed.print>` function which acts
+just like Python's built-in :func:`print` but also forwards the printed output to the
+client side Python session. This makes distributed debugging feel more like debugging
+locally.
+
 Exceptions
 ----------
 
 When a task in your computation fails, the standard way of understanding what
 went wrong is to look at the exception and traceback.  Often people do this
 with the ``pdb`` module, IPython ``%debug`` or ``%pdb`` magics, or by just
 looking at the traceback and investigating where in their code the exception
```

### Comparing `dask-2023.7.1/docs/source/how-to/extend-sizeof.rst` & `dask-2023.8.0/docs/source/how-to/extend-sizeof.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/how-to/manage-environments.rst` & `dask-2023.8.0/docs/source/how-to/manage-environments.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/how-to/selecting-the-collection-backend.rst` & `dask-2023.8.0/docs/source/how-to/selecting-the-collection-backend.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/how-to/setup-prometheus.rst` & `dask-2023.8.0/docs/source/how-to/setup-prometheus.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/10_minutes_array_graph.png` & `dask-2023.8.0/docs/source/images/10_minutes_array_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/10_minutes_bag_graph.png` & `dask-2023.8.0/docs/source/images/10_minutes_bag_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/10_minutes_dataframe_graph.png` & `dask-2023.8.0/docs/source/images/10_minutes_dataframe_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/HHMI_Janelia_Color.png` & `dask-2023.8.0/docs/source/images/HHMI_Janelia_Color.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/array.svg` & `dask-2023.8.0/docs/source/images/array.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/async-embarrassing.gif` & `dask-2023.8.0/docs/source/images/async-embarrassing.gif`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/concurrent-futures-threaded.webp` & `dask-2023.8.0/docs/source/images/concurrent-futures-threaded.webp`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/crosstalk.svg` & `dask-2023.8.0/docs/source/images/crosstalk.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_jupyterlab.png` & `dask-2023.8.0/docs/source/images/dashboard_jupyterlab.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_link.png` & `dask-2023.8.0/docs/source/images/dashboard_link.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_memory.png` & `dask-2023.8.0/docs/source/images/dashboard_memory.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_memory_new.gif` & `dask-2023.8.0/docs/source/images/dashboard_memory_new.gif`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_progress.png` & `dask-2023.8.0/docs/source/images/dashboard_progress.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_status.png` & `dask-2023.8.0/docs/source/images/dashboard_status.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_task_processing.png` & `dask-2023.8.0/docs/source/images/dashboard_task_processing.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_task_stream_unhealthy.png` & `dask-2023.8.0/docs/source/images/dashboard_task_stream_unhealthy.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dashboard_taskstream_healthy.png` & `dask-2023.8.0/docs/source/images/dashboard_taskstream_healthy.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask-adaptive.svg` & `dask-2023.8.0/docs/source/images/dask-adaptive.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask-array.svg` & `dask-2023.8.0/docs/source/images/dask-array.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask-cluster-manager.svg` & `dask-2023.8.0/docs/source/images/dask-cluster-manager.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask-dataframe.svg` & `dask-2023.8.0/docs/source/images/dask-dataframe.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask-overview-distributed-callout.svg` & `dask-2023.8.0/docs/source/images/dask-overview-distributed-callout.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask-overview-schedulers.svg` & `dask-2023.8.0/docs/source/images/dask-overview-schedulers.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask-overview.svg` & `dask-2023.8.0/docs/source/images/dask-overview.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_horizontal.svg` & `dask-2023.8.0/docs/source/images/dask_horizontal.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_horizontal_black.svg` & `dask-2023.8.0/docs/source/images/dask_horizontal_black.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_horizontal_on_blue.svg` & `dask-2023.8.0/docs/source/images/dask_horizontal_on_blue.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_horizontal_on_pink.svg` & `dask-2023.8.0/docs/source/images/dask_horizontal_on_pink.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_horizontal_white.svg` & `dask-2023.8.0/docs/source/images/dask_horizontal_white.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_icon.svg` & `dask-2023.8.0/docs/source/images/dask_icon.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_icon_black.svg` & `dask-2023.8.0/docs/source/images/dask_icon_black.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_icon_on_pink.svg` & `dask-2023.8.0/docs/source/images/dask_icon_on_pink.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/dask_icon_white.svg` & `dask-2023.8.0/docs/source/images/dask_icon_white.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/delayed-inc-double-add.svg` & `dask-2023.8.0/docs/source/images/delayed-inc-double-add.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/distributed-overview.svg` & `dask-2023.8.0/docs/source/images/distributed-overview.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/frame-shuffle.svg` & `dask-2023.8.0/docs/source/images/frame-shuffle.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/frame-sort.svg` & `dask-2023.8.0/docs/source/images/frame-sort.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/frame.svg` & `dask-2023.8.0/docs/source/images/frame.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/gputester-msg.png` & `dask-2023.8.0/docs/source/images/gputester-msg.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/growth_of_languages.png` & `dask-2023.8.0/docs/source/images/growth_of_languages.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/growth_of_libraries.png` & `dask-2023.8.0/docs/source/images/growth_of_libraries.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/inc-add.svg` & `dask-2023.8.0/docs/source/images/inc-add.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/map-reduce-task-scheduling.svg` & `dask-2023.8.0/docs/source/images/map-reduce-task-scheduling.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/map_blocks_drop_axis.png` & `dask-2023.8.0/docs/source/images/map_blocks_drop_axis.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/merge_chunks.png` & `dask-2023.8.0/docs/source/images/merge_chunks.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/merge_chunks_false.png` & `dask-2023.8.0/docs/source/images/merge_chunks_false.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/optimize_dask1.svg` & `dask-2023.8.0/docs/source/images/optimize_dask1.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/optimize_dask2.svg` & `dask-2023.8.0/docs/source/images/optimize_dask2.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/optimize_dask3.svg` & `dask-2023.8.0/docs/source/images/optimize_dask3.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/optimize_dask4.svg` & `dask-2023.8.0/docs/source/images/optimize_dask4.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/optimize_dask5.svg` & `dask-2023.8.0/docs/source/images/optimize_dask5.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/order-failure.png` & `dask-2023.8.0/docs/source/images/order-failure.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/order-success.png` & `dask-2023.8.0/docs/source/images/order-success.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/overlap.svg` & `dask-2023.8.0/docs/source/images/overlap.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/overlapping-blocks.svg` & `dask-2023.8.0/docs/source/images/overlapping-blocks.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/overlapping-neighbors.svg` & `dask-2023.8.0/docs/source/images/overlapping-neighbors.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/pipeline.svg` & `dask-2023.8.0/docs/source/images/pipeline.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/reshape.png` & `dask-2023.8.0/docs/source/images/reshape.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/reshape_problem.png` & `dask-2023.8.0/docs/source/images/reshape_problem.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/reshape_rechunked.png` & `dask-2023.8.0/docs/source/images/reshape_rechunked.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/scaling-edges.png` & `dask-2023.8.0/docs/source/images/scaling-edges.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/scaling-nodes.png` & `dask-2023.8.0/docs/source/images/scaling-nodes.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/simple-dask.png` & `dask-2023.8.0/docs/source/images/simple-dask.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/transpose-hlg-hovertooltip.png` & `dask-2023.8.0/docs/source/images/transpose-hlg-hovertooltip.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/transpose-hlg-html-repr.png` & `dask-2023.8.0/docs/source/images/transpose-hlg-html-repr.png`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/transpose.svg` & `dask-2023.8.0/docs/source/images/transpose.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/transpose_opt.svg` & `dask-2023.8.0/docs/source/images/transpose_opt.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/trivial.svg` & `dask-2023.8.0/docs/source/images/trivial.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/images/unoverlapping-neighbors.svg` & `dask-2023.8.0/docs/source/images/unoverlapping-neighbors.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/index.rst` & `dask-2023.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/install.rst` & `dask-2023.8.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/logos.rst` & `dask-2023.8.0/docs/source/logos.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/maintainers.rst` & `dask-2023.8.0/docs/source/maintainers.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/optimize.rst` & `dask-2023.8.0/docs/source/optimize.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/order.rst` & `dask-2023.8.0/docs/source/order.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/phases-of-computation.rst` & `dask-2023.8.0/docs/source/phases-of-computation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/presentations.rst` & `dask-2023.8.0/docs/source/presentations.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/scheduler-overview.rst` & `dask-2023.8.0/docs/source/scheduler-overview.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/scheduling-policy.rst` & `dask-2023.8.0/docs/source/scheduling-policy.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/scheduling.rst` & `dask-2023.8.0/docs/source/scheduling.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/scripts/scheduling.py` & `dask-2023.8.0/docs/source/scripts/scheduling.py`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/shared.rst` & `dask-2023.8.0/docs/source/shared.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/spark.rst` & `dask-2023.8.0/docs/source/spark.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/spec.rst` & `dask-2023.8.0/docs/source/spec.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/support.rst` & `dask-2023.8.0/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/understanding-performance.rst` & `dask-2023.8.0/docs/source/understanding-performance.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/user-interfaces.rst` & `dask-2023.8.0/docs/source/user-interfaces.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/docs/source/why.rst` & `dask-2023.8.0/docs/source/why.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.7.1/pyproject.toml` & `dask-2023.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=62.6", "versioneer[toml]==0.28"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dask"
 description = "Parallel PyData with Task Scheduling"
 maintainers = [{name = "Matthew Rocklin", email = "mrocklin@gmail.com"}]
-license = {text = "BSD"}
+license = {text = "BSD-3-Clause"}
 keywords = ["task-scheduling parallel numpy pandas pydata"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
@@ -48,18 +48,18 @@
 [project.optional-dependencies]
 # NOTE: These are tested in `continuous_integration/test_imports.sh` If
 # you modify these, make sure to change the corresponding line there.
 array = ["numpy >= 1.21"]
 # keeping for backwards compatibility
 bag = []
 dataframe = [
-    "numpy >= 1.21",
+    "dask[array]",
     "pandas >= 1.3",
 ]
-distributed = ["distributed == 2023.7.1"]
+distributed = ["distributed == 2023.8.0"]
 diagnostics = [
     "bokeh >= 2.4.2",
     "jinja2 >= 2.10.3",
 ]
 # keeping for backwards compatibility
 delayed = []
 complete = [
```

