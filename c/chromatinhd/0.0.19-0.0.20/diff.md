# Comparing `tmp/chromatinhd-0.0.19.tar.gz` & `tmp/chromatinhd-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromatinhd-0.0.19.tar", last modified: Thu Aug  3 08:46:52 2023, max compression
+gzip compressed data, was "chromatinhd-0.0.20.tar", last modified: Fri Aug  4 12:39:42 2023, max compression
```

## Comparing `chromatinhd-0.0.19.tar` & `chromatinhd-0.0.20.tar`

### file list

```diff
@@ -1,223 +1,237 @@
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/.github/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/.github/workflows/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      674 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/.github/workflows/ci.yml
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3298 2023-07-21 17:12:01.000000 chromatinhd-0.0.19/.gitignore
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      120 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/.pre-commit-config.yaml
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1070 2023-07-22 10:00:10.000000 chromatinhd-0.0.19/LICENSE.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      860 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/PKG-INFO
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      284 2023-07-22 10:00:10.000000 chromatinhd-0.0.19/README.md
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/docs/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/override/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      196 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/override/main.html
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2523 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/index.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      925 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/docs/source/index.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       28 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/jupytext.toml
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/quickstart/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1170 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/quickstart/0_install.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5643 2023-07-22 07:37:54.000000 chromatinhd-0.0.19/docs/source/quickstart/1_data.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5762 2023-07-22 07:37:54.000000 chromatinhd-0.0.19/docs/source/quickstart/2_pred.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3195 2023-07-22 07:37:54.000000 chromatinhd-0.0.19/docs/source/quickstart/3_diff.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/reference/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/reference/data/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       42 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/clustering.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       40 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/fragments.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       34 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/regions.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       34 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/transcriptome.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/reference/index.md
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/docs/source/reference/models/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/reference/models/pred/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/models/pred/plot.md
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   167512 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/favicon.ai
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2336 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/static/favicon.png
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   220360 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/static/logo.ai
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9528 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/static/logo.png
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/docs/source/static/models/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/diff/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/diff/1x/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7684 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/diff/1x/logo.png
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   973869 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/diff/logo.pdf
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/dime/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   221105 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/dime/logo.pdf
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4068 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/dime/logo.png
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/pred/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/pred/1x/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1621 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/pred/1x/logo.png
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   153226 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/pred/logo.pdf
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/time/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   219145 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/time/logo.pdf
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3954 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/time/logo.png
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/stylesheets/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      375 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/stylesheets/extra-reference.css
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      847 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/stylesheets/extra.css
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1270 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/mkdocs.yml
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1616 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/pyproject.toml
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/scripts/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      415 2023-08-03 08:46:41.000000 chromatinhd-0.0.19/scripts/build.sh
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16878 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/scripts/setup_data_tiny.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1186 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/scripts/test.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       38 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/setup.cfg
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/src/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      661 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/biomart/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      101 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       92 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/cache.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5785 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/dataset.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3611 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/tss.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/data/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      378 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/data/clustering/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/clustering/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1069 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/data/clustering/clustering.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/src/chromatinhd/data/examples/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2046327 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4403 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2614194 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/folds/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/folds/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3670 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/folds/folds.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/fragments/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       51 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/fragments/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7344 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/fragments/fragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/genotype/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       31 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/genotype/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      146 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/genotype/genotype.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       74 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2392 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motifscan.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      528 2023-01-31 18:45:51.000000 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motiftrack.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11269 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/peakcounts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2179 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/regions.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       40 2022-12-09 09:27:27.000000 chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4781 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/transcriptome.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      238 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/device.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2430 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/embedding.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9539 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/flow.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/grid/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       47 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/grid/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1729 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/grid/broken.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    14406 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/grid/grid.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/loaders/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      147 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4314 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/chunkfragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5044 2022-12-15 11:33:47.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/fragments.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18790 2023-01-10 08:03:37.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/motifs.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10212 2023-01-31 18:34:46.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/fragmentmotif.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10589 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/fragments.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3733 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/minibatching.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1930 2023-01-09 14:53:04.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/peakcounts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8390 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/pool.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      374 2022-12-02 07:47:23.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/setup.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1087 2022-12-13 10:48:55.000000 chromatinhd-0.0.19/src/chromatinhd/loss.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1291 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/models/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      132 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16611 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/differential.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18467 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/enrichment.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5245 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/genepositional.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      150 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      924 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1016 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering_cuts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4821 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/cuts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/fragments_helpers.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3231 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/minibatches.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       20 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    23535 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/cutnf.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    12040 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/spline.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       45 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9280 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/cubic.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3460 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/linear.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5788 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/quadratic.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    14633 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5598 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3183 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential_expression.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       29 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3588 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/trainer.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       84 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      147 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3261 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/censorers.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/filter.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8982 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genemultiwindow.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7202 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genepairwindow.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      182 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5133 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments_helpers.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3255 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/minibatches.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      571 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1087 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome_fragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       23 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    20929 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/across.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    21570 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/additive.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      338 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/loss.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      183 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1581 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/copredictivity.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1593 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/effect.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8120 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/predictivity.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       29 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4701 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/trainer.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1200 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/optim.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/plot/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      102 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/plot/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/plot/genome/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/genome/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11346 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/plot/genome/genes.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2400 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/matshow45.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1312 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/patch.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1925 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/quasirandom.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2297 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/plot/tickers.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6499 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/sparse.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4716 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/train.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/utils/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4452 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1395 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/ansi.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      966 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/ecdf.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      269 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/utils/numpy.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2341 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/testing.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1240 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/utils/torch.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd.egg-info/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      860 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/PKG-INFO
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6084 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/SOURCES.txt
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        1 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/dependency_links.txt
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      260 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/requires.txt
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       12 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/top_level.txt
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/biomart/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      165 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/tests/biomart/conftest.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      463 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/tests/biomart/tss_test.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2074 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/tests/conftest.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/tests/models/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/tests/models/diff/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/diff/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      508 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/tests/models/diff/loader/test_clustering_cuts.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/diff/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      307 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/tests/models/diff/model/test_cutnf.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/tests/models/pred/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/pred/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      533 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/tests/models/pred/loader/test_transcriptome_fragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/pred/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      310 2023-08-02 13:32:25.000000 chromatinhd-0.0.19/tests/models/pred/model/test_additive.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      480 2023-01-31 18:34:46.000000 chromatinhd-0.0.19/tests/test_loss.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/.github/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/.github/workflows/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      883 2023-08-04 12:35:53.000000 chromatinhd-0.0.20/.github/workflows/ci.yml
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3298 2023-07-21 17:12:01.000000 chromatinhd-0.0.20/.gitignore
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      120 2023-07-22 07:01:56.000000 chromatinhd-0.0.20/.pre-commit-config.yaml
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1070 2023-07-22 10:00:10.000000 chromatinhd-0.0.20/LICENSE.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      841 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/PKG-INFO
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      245 2023-08-04 07:26:21.000000 chromatinhd-0.0.20/README.md
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/docs/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/override/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      196 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/docs/override/main.html
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2523 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/index.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      925 2023-07-22 07:01:56.000000 chromatinhd-0.0.20/docs/source/index.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/javascripts/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      861 2023-08-03 13:21:44.000000 chromatinhd-0.0.20/docs/source/javascripts/reference.js
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       28 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/docs/source/jupytext.toml
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/quickstart/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1170 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/quickstart/0_install.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5643 2023-07-22 07:37:54.000000 chromatinhd-0.0.20/docs/source/quickstart/1_data.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5762 2023-07-22 07:37:54.000000 chromatinhd-0.0.20/docs/source/quickstart/2_pred.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3195 2023-07-22 07:37:54.000000 chromatinhd-0.0.20/docs/source/quickstart/3_diff.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/reference/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/reference/data/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       42 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/docs/source/reference/data/clustering.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       33 2023-08-04 06:10:04.000000 chromatinhd-0.0.20/docs/source/reference/data/folds.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       40 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/docs/source/reference/data/fragments.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       41 2023-08-03 13:21:44.000000 chromatinhd-0.0.20/docs/source/reference/data/motifscan.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       34 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/docs/source/reference/data/regions.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       34 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/docs/source/reference/data/transcriptome.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/docs/source/reference/index.md
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/docs/source/reference/models/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/reference/models/diff/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       53 2023-08-04 09:17:43.000000 chromatinhd-0.0.20/docs/source/reference/models/diff/interpret.md
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/reference/models/pred/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      107 2023-08-04 06:28:36.000000 chromatinhd-0.0.20/docs/source/reference/models/pred/interpret.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      190 2023-08-04 06:23:08.000000 chromatinhd-0.0.20/docs/source/reference/models/pred/model.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/docs/source/reference/models/pred/plot.md
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/static/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   167512 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/favicon.ai
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2336 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/docs/source/static/favicon.png
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   220360 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/docs/source/static/logo.ai
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9528 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/docs/source/static/logo.png
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/docs/source/static/models/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/static/models/diff/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/static/models/diff/1x/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7684 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/diff/1x/logo.png
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   973869 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/diff/logo.pdf
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/static/models/dime/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   221105 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/dime/logo.pdf
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4068 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/dime/logo.png
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/static/models/pred/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/static/models/pred/1x/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1621 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/pred/1x/logo.png
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   153226 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/pred/logo.pdf
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/static/models/time/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   219145 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/time/logo.pdf
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3954 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/docs/source/static/models/time/logo.png
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/docs/source/stylesheets/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1005 2023-08-04 12:38:09.000000 chromatinhd-0.0.20/docs/source/stylesheets/extra-reference.css
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1224 2023-08-04 07:24:14.000000 chromatinhd-0.0.20/docs/source/stylesheets/extra.css
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1340 2023-08-04 07:24:24.000000 chromatinhd-0.0.20/mkdocs.yml
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1802 2023-08-04 12:35:47.000000 chromatinhd-0.0.20/pyproject.toml
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.583486 chromatinhd-0.0.20/scripts/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      143 2023-08-04 11:52:55.000000 chromatinhd-0.0.20/scripts/cythonize.sh
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      440 2023-08-04 12:39:27.000000 chromatinhd-0.0.20/scripts/dist.sh
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      231 2023-08-04 11:40:03.000000 chromatinhd-0.0.20/scripts/install.sh
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16878 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/scripts/setup_data_tiny.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1186 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/scripts/test.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       38 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/setup.cfg
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      613 2023-08-04 11:56:56.000000 chromatinhd-0.0.20/setup.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/src/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.587486 chromatinhd-0.0.20/src/chromatinhd/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      593 2023-08-04 11:17:09.000000 chromatinhd-0.0.20/src/chromatinhd/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.587486 chromatinhd-0.0.20/src/chromatinhd/biomart/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      101 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/biomart/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       92 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/biomart/cache.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5785 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/biomart/dataset.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3611 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/biomart/tss.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.587486 chromatinhd-0.0.20/src/chromatinhd/data/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      409 2023-08-03 13:21:44.000000 chromatinhd-0.0.20/src/chromatinhd/data/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.587486 chromatinhd-0.0.20/src/chromatinhd/data/clustering/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/clustering/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1086 2023-08-03 13:21:44.000000 chromatinhd-0.0.20/src/chromatinhd/data/clustering/clustering.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/src/chromatinhd/data/examples/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.587486 chromatinhd-0.0.20/src/chromatinhd/data/examples/pbmc10ktiny/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2046327 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4403 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2614194 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/data/folds/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/folds/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4502 2023-08-04 07:23:42.000000 chromatinhd-0.0.20/src/chromatinhd/data/folds/folds.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/data/fragments/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       51 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/fragments/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8165 2023-08-04 09:12:39.000000 chromatinhd-0.0.20/src/chromatinhd/data/fragments/fragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/data/genotype/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       31 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/genotype/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      146 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/data/genotype/genotype.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/data/motifscan/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       68 2023-08-03 13:21:44.000000 chromatinhd-0.0.20/src/chromatinhd/data/motifscan/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1667 2023-08-03 13:21:44.000000 chromatinhd-0.0.20/src/chromatinhd/data/motifscan/gwas.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10109 2023-08-04 07:24:00.000000 chromatinhd-0.0.20/src/chromatinhd/data/motifscan/motifscan.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      528 2023-01-31 18:45:51.000000 chromatinhd-0.0.20/src/chromatinhd/data/motifscan/motiftrack.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/data/peakcounts/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/data/peakcounts/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11277 2023-08-04 10:07:43.000000 chromatinhd-0.0.20/src/chromatinhd/data/peakcounts/peakcounts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2177 2023-08-03 13:21:44.000000 chromatinhd-0.0.20/src/chromatinhd/data/regions.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/data/transcriptome/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       40 2022-12-09 09:27:27.000000 chromatinhd-0.0.20/src/chromatinhd/data/transcriptome/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4581 2023-08-04 10:07:21.000000 chromatinhd-0.0.20/src/chromatinhd/data/transcriptome/transcriptome.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      238 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/device.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2430 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/embedding.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9993 2023-08-04 07:24:24.000000 chromatinhd-0.0.20/src/chromatinhd/flow.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/grid/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       47 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/grid/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1729 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/grid/broken.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    14406 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/grid/grid.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/loaders/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      154 2023-08-04 11:59:34.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4314 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/chunkfragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/loaders/extraction/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5044 2022-12-15 11:33:47.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/extraction/fragments.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18790 2023-01-10 08:03:37.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/extraction/motifs.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10224 2023-08-04 11:59:54.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/fragmentmotif.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10592 2023-08-04 11:54:59.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/fragments.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3733 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/minibatching.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1930 2023-01-09 14:53:04.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/peakcounts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8390 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/pool.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      374 2022-12-02 07:47:23.000000 chromatinhd-0.0.20/src/chromatinhd/loaders/setup.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/models/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1291 2023-07-22 07:01:56.000000 chromatinhd-0.0.20/src/chromatinhd/models/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/models/diff/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      132 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16611 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/differential.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/models/diff/enrichment/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/enrichment/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18467 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/enrichment/enrichment.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/models/diff/interpret/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       43 2023-08-04 09:19:49.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/interpret/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6015 2023-08-04 09:16:35.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/interpret/genepositional.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      150 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      924 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/clustering.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1016 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/clustering_cuts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5042 2023-08-04 12:01:08.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/cuts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  1097970 2023-08-04 11:52:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/fragments_helpers.c
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/fragments_helpers.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3231 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/minibatches.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       20 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    23527 2023-08-04 09:12:39.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/cutnf.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    12138 2023-08-04 09:12:39.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/spline.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.591486 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       45 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9280 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/cubic.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3460 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/linear.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5788 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/quadratic.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/diff/plot/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    14633 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/plot/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5598 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/plot/differential.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3192 2023-08-04 10:08:03.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/plot/differential_expression.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/diff/trainer/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       29 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/trainer/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3635 2023-08-04 07:33:16.000000 chromatinhd-0.0.20/src/chromatinhd/models/diff/trainer/trainer.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/pred/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       84 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      147 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3261 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/censorers.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/filter.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9033 2023-08-04 09:13:24.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/genemultiwindow.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8048 2023-08-04 07:37:27.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/genepairwindow.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      182 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5347 2023-08-04 12:00:59.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/fragments.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  1097970 2023-08-04 11:52:56.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/fragments_helpers.c
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/fragments_helpers.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3466 2023-08-04 07:24:24.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/minibatches.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      760 2023-08-04 07:24:24.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/transcriptome.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1087 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/transcriptome_fragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/pred/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       23 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/model/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    22333 2023-08-04 07:41:30.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/model/across.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    22989 2023-08-04 07:40:45.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/model/additive.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      338 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/model/loss.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      183 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1581 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/copredictivity.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1593 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/effect.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8120 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/predictivity.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/models/pred/trainer/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       39 2023-08-04 07:24:24.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/trainer/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8071 2023-08-04 07:41:13.000000 chromatinhd-0.0.20/src/chromatinhd/models/pred/trainer/trainer.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1200 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/optim.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/plot/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      102 2023-07-22 07:01:56.000000 chromatinhd-0.0.20/src/chromatinhd/plot/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/plot/genome/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/plot/genome/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11346 2023-07-22 07:01:56.000000 chromatinhd-0.0.20/src/chromatinhd/plot/genome/genes.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2400 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/plot/matshow45.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1312 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/plot/patch.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1925 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/plot/quasirandom.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2297 2023-07-22 07:01:56.000000 chromatinhd-0.0.20/src/chromatinhd/plot/tickers.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6499 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/sparse.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4624 2023-08-04 10:03:04.000000 chromatinhd-0.0.20/src/chromatinhd/train.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/src/chromatinhd/utils/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4405 2023-08-04 10:03:09.000000 chromatinhd-0.0.20/src/chromatinhd/utils/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      966 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/utils/ecdf.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      269 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/utils/numpy.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2341 2023-07-21 17:11:57.000000 chromatinhd-0.0.20/src/chromatinhd/utils/testing.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1240 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/src/chromatinhd/utils/torch.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.587486 chromatinhd-0.0.20/src/chromatinhd.egg-info/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      841 2023-08-04 12:39:42.000000 chromatinhd-0.0.20/src/chromatinhd.egg-info/PKG-INFO
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6497 2023-08-04 12:39:42.000000 chromatinhd-0.0.20/src/chromatinhd.egg-info/SOURCES.txt
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        1 2023-08-04 12:39:42.000000 chromatinhd-0.0.20/src/chromatinhd.egg-info/dependency_links.txt
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      272 2023-08-04 12:39:42.000000 chromatinhd-0.0.20/src/chromatinhd.egg-info/requires.txt
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       12 2023-08-04 12:39:42.000000 chromatinhd-0.0.20/src/chromatinhd.egg-info/top_level.txt
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/tests/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/tests/biomart/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      165 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/tests/biomart/conftest.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      463 2023-08-03 08:46:11.000000 chromatinhd-0.0.20/tests/biomart/tss_test.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2328 2023-08-04 10:09:18.000000 chromatinhd-0.0.20/tests/conftest.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/tests/data/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/tests/data/motifscan/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5197 2023-08-03 18:22:40.000000 chromatinhd-0.0.20/tests/data/motifscan/test_motifscan.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/tests/models/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/tests/models/diff/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/tests/models/diff/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      508 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/tests/models/diff/loader/test_clustering_cuts.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/tests/models/diff/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      307 2023-07-22 07:01:56.000000 chromatinhd-0.0.20/tests/models/diff/model/test_cutnf.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.579486 chromatinhd-0.0.20/tests/models/pred/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/tests/models/pred/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      533 2023-07-22 09:14:17.000000 chromatinhd-0.0.20/tests/models/pred/loader/test_transcriptome_fragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-04 12:39:42.595486 chromatinhd-0.0.20/tests/models/pred/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      493 2023-08-04 07:23:55.000000 chromatinhd-0.0.20/tests/models/pred/model/test_additive.py
```

### Comparing `chromatinhd-0.0.19/.gitignore` & `chromatinhd-0.0.20/.gitignore`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/LICENSE.md` & `chromatinhd-0.0.20/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/PKG-INFO` & `chromatinhd-0.0.20/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: chromatinhd
-Version: 0.0.19
+Version: 0.0.20
 Summary: High-definition modeling of (single-cell) chromatin + transcriptomics data
 Author-email: Wouter Saelens <wouter.saelens@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/DeplanckeLab/ChromatinHD
 Project-URL: Bug Tracker, https://github.com/DeplanckeLab/ChromatinHD/issues
 Keywords: bioinformatics,chromatin accessibility,transcriptomics
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE.md
 
 <p align="center">
-  <a href="https://deplanckelab.github.io/ChromatinHD/">
+  <a href="https://chromatinhd.eu">
     <img src="https://raw.githubusercontent.com/DeplanckeLab/ChromatinHD/main/docs/source/static/logo.png" width="300" />
   </a>
 </p>
 
-Documentation is available at https://deplanckelab.github.io/ChromatinHD/
+Documentation is available at <https://chromatinhd.eu>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.19 Summary: High-
+Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.20 Summary: High-
 definition modeling of (single-cell) chromatin + transcriptomics data Author-
 email: Wouter Saelens
 saelens@gmail.com> License: MIT Project-URL: Homepage, https://github.com/
 DeplanckeLab/ChromatinHD Project-URL: Bug Tracker, https://github.com/
 DeplanckeLab/ChromatinHD/issues Keywords: bioinformatics,chromatin
 accessibility,transcriptomics Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE.md
+dev Provides-Extra: test License-File: LICENSE.md
  [https://raw.githubusercontent.com/DeplanckeLab/ChromatinHD/main/docs/source/
                                static/logo.png]
-Documentation is available at https://deplanckelab.github.io/ChromatinHD/
+Documentation is available at
+chromatinhd.eu>
```

### Comparing `chromatinhd-0.0.19/docs/source/index.md` & `chromatinhd-0.0.20/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/index.py` & `chromatinhd-0.0.20/docs/source/index.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/quickstart/0_install.py` & `chromatinhd-0.0.20/docs/source/quickstart/0_install.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/quickstart/1_data.py` & `chromatinhd-0.0.20/docs/source/quickstart/1_data.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/quickstart/2_pred.py` & `chromatinhd-0.0.20/docs/source/quickstart/2_pred.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/quickstart/3_diff.py` & `chromatinhd-0.0.20/docs/source/quickstart/3_diff.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/favicon.ai` & `chromatinhd-0.0.20/docs/source/static/favicon.ai`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/favicon.png` & `chromatinhd-0.0.20/docs/source/static/favicon.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/logo.ai` & `chromatinhd-0.0.20/docs/source/static/logo.ai`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/logo.png` & `chromatinhd-0.0.20/docs/source/static/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/diff/1x/logo.png` & `chromatinhd-0.0.20/docs/source/static/models/diff/1x/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/diff/logo.pdf` & `chromatinhd-0.0.20/docs/source/static/models/diff/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/dime/logo.pdf` & `chromatinhd-0.0.20/docs/source/static/models/dime/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/dime/logo.png` & `chromatinhd-0.0.20/docs/source/static/models/dime/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/pred/1x/logo.png` & `chromatinhd-0.0.20/docs/source/static/models/pred/1x/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/pred/logo.pdf` & `chromatinhd-0.0.20/docs/source/static/models/pred/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/time/logo.pdf` & `chromatinhd-0.0.20/docs/source/static/models/time/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/static/models/time/logo.png` & `chromatinhd-0.0.20/docs/source/static/models/time/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/docs/source/stylesheets/extra.css` & `chromatinhd-0.0.20/docs/source/stylesheets/extra.css`

 * *Files 22% similar despite different names*

```diff
@@ -46,7 +46,31 @@
     border-left: 2px green solid !important;
 }
 
 /* remove the cell toolbar with ugly tags */
 .jupyter-wrapper .celltoolbar {
     display: none !important;
 }
+
+/* nav bar */
+.md-tabs__item {
+    height: inherit;
+    padding-left: 0;
+    padding-right: 0;
+}
+
+.md-tabs__item>a {
+    padding-top: 0.8em;
+    padding-bottom: 0.8em;
+    padding-left: 0.8em;
+    padding-right: 0.8em;
+    margin-top: 0;
+    transition: 0.1s;
+}
+
+.md-tabs__item>a:hover {
+    background-color: #EEE;
+}
+
+.md-tabs__link--active {
+    background-color: #F8F8F8;
+}
```

### Comparing `chromatinhd-0.0.19/mkdocs.yml` & `chromatinhd-0.0.20/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -8,28 +8,29 @@
   favicon: static/favicon.png
   custom_dir: docs/override
   features:
     - navigation.tracking
     - navigation.tabs
     - navigation.footer
 
-site_url: "https://deplanckelab.github.io/ChromatinHD/"
+site_url: "https://chromatinhd.eu/"
 repo_url: https://github.com/DeplanckeLab/ChromatinHD
 
 plugins:
   - mkdocstrings:
       handlers:
         python:
           import:
           - https://docs.python-requests.org/en/master/objects.inv
           options:
             docstring_style: google
             heading_level: 2
             inheritance_diagram: True
             show_root_heading: True
+            show_symbol_type_heading: True
   - mike
   - search
   - mkdocs-jupyter:
       include: ["*.ipynb"] # Default: ["*.py", "*.ipynb"]
       remove_tag_config:
         remove_input_tags:
           - hide_code
@@ -47,8 +48,10 @@
   - pymdownx.details
   - pymdownx.superfences
   - attr_list
   - md_in_html
   - pymdownx.details
 extra_css:
   - stylesheets/extra.css
-  - stylesheets/extra-reference.css
+  - stylesheets/extra-reference.css
+extra_javascript:
+  - javascripts/reference.js
```

### Comparing `chromatinhd-0.0.19/pyproject.toml` & `chromatinhd-0.0.20/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = [ "setuptools>=41", "wheel", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=41", "wheel", "setuptools_scm[toml]>=6.2", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "chromatinhd"
@@ -19,20 +19,20 @@
 dependencies = [
     "torch",  # --extra-index-url https://download.pytorch.org/whl/cu113
     "torch-scatter", # --find-links https://data.pyg.org/whl/torch-1.12.1+cu113.html
     "scanpy",
     "matplotlib",
     "numpy",
     "seaborn",
-    "Cython",
     "fisher",
     "diskcache",
     "appdirs",
     "xarray",
     "pysam",
+    "requests",
 ]
 dynamic = ["version", "readme"]
 license = {text = "MIT"}
 
 [project.urls]
 "Homepage" = "https://github.com/DeplanckeLab/ChromatinHD"
 "Bug Tracker" = "https://github.com/DeplanckeLab/ChromatinHD/issues"
@@ -44,26 +44,37 @@
 dev = [
     "pre-commit",
     "pytest",
     "coverage",
     "black",
     "pylint",
     "jupytext",
-    "pytest",
-    "statsmodels",
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]",
     "mkdocs-jupyter",
     "mike",
     "cairosvg",  # for mkdocs social
     "pillow",  # for mkdocs social
-    "setuptools_scm"
+    "setuptools_scm",
     # "faiss-cpu",
+    "Cython",
+]
+test = [
+    "pytest",
 ]
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore",
+]
+
+[tool.pylint.'MESSAGES CONTROL']
+max-line-length = 120
+disable = [
+    "too-many-arguments",
+    "not-callable",
+    "redefined-builtin",
+    "redefined-outer-name",
 ]
```

### Comparing `chromatinhd-0.0.19/scripts/setup_data_tiny.py` & `chromatinhd-0.0.20/scripts/setup_data_tiny.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/scripts/test.py` & `chromatinhd-0.0.20/scripts/test.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/__init__.py` & `chromatinhd-0.0.20/src/chromatinhd/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from . import sparse
 from . import utils
 from . import flow
 from . import grid
 from . import plot
 from . import data
 from . import train
-from . import loaders
-from . import loss
 from . import embedding
 from . import optim
 from . import biomart
 from . import models
 
 __all__ = [
     "get_git_root",
@@ -22,16 +20,14 @@
     "Unpickler",
     "load",
     "sparse",
     "utils",
     "flow",
     "data",
     "train",
-    "loaders",
-    "loss",
     "embedding",
     "optim",
     "grid",
     "biomart",
     "models",
     "plot",
 ]
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/biomart/dataset.py` & `chromatinhd-0.0.20/src/chromatinhd/biomart/dataset.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/biomart/tss.py` & `chromatinhd-0.0.20/src/chromatinhd/biomart/tss.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/clustering/clustering.py` & `chromatinhd-0.0.20/src/chromatinhd/data/clustering/clustering.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import pandas as pd
 import pickle
 
-from chromatinhd.flow import Flow, Stored, StoredDict
+from chromatinhd.flow import Flow, Stored, StoredDict, StoredDataFrame
 from chromatinhd import sparse
 from chromatinhd.utils import Unpickler
 
 
 class Clustering(Flow):
     labels = Stored("labels")
-    """Labels for each cell."""
+    "Labels for each cell."
 
-    cluster_info = Stored("cluster_info")
-    """Dataframe containing information, such as a label, for each cluster."""
+    cluster_info = StoredDataFrame("cluster_info")
+    "Dataframe containing information for each cluster, such as a label."
 
     @classmethod
     def from_labels(cls, labels, path):
         clustering = cls(path)
         if not isinstance(labels, pd.Series):
             labels = pd.Series(labels).astype("category")
         clustering.labels = labels
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz` & `chromatinhd-0.0.20/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi` & `chromatinhd-0.0.20/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad` & `chromatinhd-0.0.20/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/fragments/fragments.py` & `chromatinhd-0.0.20/src/chromatinhd/data/fragments/fragments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,40 @@
+import math
+import pathlib
+from typing import Union
+
 import numpy as np
 import pandas as pd
+import torch
+import tqdm.auto as tqdm
 
+from chromatinhd.data.regions import Regions
 from chromatinhd.flow import (
+    TSV,
     Flow,
-    StoredTorchInt32,
+    Linked,
     Stored,
+    StoredTorchInt32,
     StoredTorchInt64,
-    TSV,
-    Linked,
 )
 
-from chromatinhd.data.regions import Regions
-
-import torch
-import math
-import pathlib
-import typing
-import tqdm.auto as tqdm
-
 
 class RawFragments:
     def __init__(self, file):
         self.file = file
 
 
 class Fragments(Flow):
     """Fragments centered around a gene window"""
 
     regions = Linked("regions")
-    """regions of the fragments"""
+    """Regions in which fragments are stored"""
 
     coordinates: torch.Tensor = StoredTorchInt64("coordinates")
-    """Coordinates of the fragments"""
+    """Coordinates of the two cut sites."""
 
     mapping: torch.Tensor = StoredTorchInt64("mapping")
     """Mapping of a fragment to a gene and a cell"""
 
     cellxgene_indptr: torch.Tensor = StoredTorchInt64("cellxgene_indptr")
     """Index pointers for each cellxgene combination"""
 
@@ -74,15 +73,18 @@
     @property
     def cellmapping(self):
         if self._cellmapping is None:
             self._cellmapping = self.mapping[:, 0].contiguous()
         return self._cellmapping
 
     var = TSV("var")
+    """DataFrame containing information about regions."""
+
     obs = TSV("obs")
+    """DataFrame containing information about cells."""
 
     _n_genes = None
 
     @property
     def n_genes(self):
         if self._n_genes is None:
             self._n_genes = self.var.shape[0]
@@ -99,83 +101,93 @@
     @property
     def local_cellxgene_ix(self):
         return self.cellmapping * self.n_genes + self.genemapping
 
     def estimate_fragment_per_cellxgene(self):
         return math.ceil(self.coordinates.shape[0] / self.n_cells / self.n_genes * 2)
 
-    def create_cut_data(self):
-        cut_coordinates = self.coordinates.flatten()
-        cut_coordinates = (cut_coordinates - self.window[0]) / (
-            self.window[1] - self.window[0]
-        )
-        keep_cuts = (cut_coordinates >= 0) & (cut_coordinates <= 1)
-        cut_coordinates = cut_coordinates[keep_cuts]
+    # def create_cut_data(self):
+    #     cut_coordinates = self.coordinates.flatten()
+    #     cut_coordinates = (cut_coordinates - self.window[0]) / (
+    #         self.window[1] - self.window[0]
+    #     )
+    #     keep_cuts = (cut_coordinates >= 0) & (cut_coordinates <= 1)
+    #     cut_coordinates = cut_coordinates[keep_cuts]
 
-        self.cut_coordinates = cut_coordinates
+    #     self.cut_coordinates = cut_coordinates
 
-        self.cut_local_gene_ix = self.genemapping.expand(2, -1).T.flatten()[keep_cuts]
-        self.cut_local_cell_ix = self.cellmapping.expand(2, -1).T.flatten()[keep_cuts]
+    #     self.cut_local_gene_ix = self.genemapping.expand(2, -1).T.flatten()[keep_cuts]
+    #     self.cut_local_cell_ix = self.cellmapping.expand(2, -1).T.flatten()[keep_cuts]
 
     @property
     def genes_oi_torch(self):
         return torch.from_numpy(self.genes_oi).to(self.coordinates.device)
 
     @property
     def cells_oi_torch(self):
         return torch.from_numpy(self.genes_oi).to(self.coordinates.device)
 
     @classmethod
     def from_fragments_tsv(
         cls,
-        fragments_file: typing.Union[pathlib.Path, str],
+        fragments_file: Union[pathlib.Path, str],
         regions: Regions,
         obs: pd.DataFrame,
-        path: typing.Union[pathlib.Path, str],
-        overwrite=True,
+        path: Union[pathlib.Path, str],
+        cell_column: str = None,
+        overwrite: bool = True,
     ):
         """
-        Create a Fragments object from a tsv file
+        Create a Fragments object from a fragments tsv file
 
         Parameters:
             fragments_file:
                 Location of the `fragments.tsv` file created by e.g. CellRanger or sinto
+            obs:
+                DataFrame containing information about cells. The index should be the cell names as present in the fragments file. If not, you can specify the column name using the `cell_column` argument.
             path:
                 Folder in which the fragments data will be stored
             regions:
                 Regions object
+            cell_column (optional):
+                Column name in the `obs` DataFrame containing the cell names. If not specified, the index of the `obs` DataFrame is used.
+            overwrite (optional):
+                Whether to overwrite the data if it already exists
         """
 
         if isinstance(fragments_file, str):
             fragments_file = pathlib.Path(fragments_file)
         if isinstance(path, str):
             path = pathlib.Path(path)
         if not fragments_file.exists():
             raise FileNotFoundError(f"File {fragments_file} does not exist")
         if not overwrite and path.exists():
             raise FileExistsError(f"Folder {path} already exists")
         path.mkdir(parents=True, exist_ok=True)
 
-        # region information
+        # regions information
         var = pd.DataFrame(index=regions.coordinates.index)
         var["ix"] = np.arange(var.shape[0])
 
         # cell information
         obs["ix"] = np.arange(obs.shape[0])
-        cell_to_cell_ix = obs["ix"].to_dict()
+        if cell_column is None:
+            cell_to_cell_ix = obs["ix"].to_dict()
+        else:
+            cell_to_cell_ix = obs.set_index(cell_column)["ix"].to_dict()
 
         # load fragments tabix
         import pysam
 
         fragments_tabix = pysam.TabixFile(str(fragments_file))
 
         coordinates_raw = []
         mapping_raw = []
 
-        for i, (gene, promoter_info) in tqdm.tqdm(
+        for _, (gene, promoter_info) in tqdm.tqdm(
             enumerate(regions.coordinates.iterrows()),
             total=regions.coordinates.shape[0],
             leave=False,
             desc="Processing fragments",
         ):
             gene_ix = var.loc[gene, "ix"]
             start = max(0, promoter_info["start"])
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motifscan.py` & `chromatinhd-0.0.20/src/chromatinhd/data/motifscan/gwas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-from chromatinhd.flow import Flow, CompressedNumpyInt64, CompressedNumpyFloat64, Stored
-from chromatinhd.utils import indptr_to_indices
-import pandas as pd
-
-
-class Motifscan(Flow):
-    indptr = CompressedNumpyInt64("indptr")
-    indices = CompressedNumpyInt64("indices")
-    data = CompressedNumpyFloat64("data")
-    shape = Stored("shape")
-    n_motifs = Stored("n_motifs")
-
-    _motifs = None
-
-    @property
-    def motifs(self):
-        if self._motifs is None:
-            self._motifs = pd.read_pickle(self.path / "motifs.pkl")
-        return self._motifs
-
-    @motifs.setter
-    def motifs(self, value):
-        value.index.name = "gene"
-        value.to_pickle(self.path / "motifs.pkl")
-        self._motifs = value
-
-
 class GWAS(Motifscan):
     association = Stored("association")
     window = Stored("window")
 
     def get_motifdata(self, promoter: pd.Series):
         assert "ix" in promoter.index
         gene_ix = promoter["ix"]
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motiftrack.py` & `chromatinhd-0.0.20/src/chromatinhd/data/motifscan/motiftrack.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/peakcounts.py` & `chromatinhd-0.0.20/src/chromatinhd/data/peakcounts/peakcounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import pandas as pd
 
-import scanpy as sc
-
 import collections
 import subprocess as sp
 import tqdm.auto as tqdm
 import pickle
 
 from chromatinhd.flow import Flow
 
 
 class PeakCounts(Flow):
     def create_adata(self, original_adata):
+        import scanpy as sc
+
         adata = sc.AnnData(self.counts, obs=self.obs, var=self.var)
         adata.obsm["X_umap"] = original_adata.obsm["X_umap"]
         self.adata = adata
 
     def count_peaks(self, fragments_location, cell_ids, tabix_location="tabix"):
         # extract unique peaks
         peaks = self.peaks
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/regions.py` & `chromatinhd-0.0.20/src/chromatinhd/data/regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         Parameters:
             canonical_transcripts:
                 Dataframe of canonical transcripts, with columns chrom, start, end, strand, ensembl_transcript_id
             window:
                 Window around each transcription start site. Should be a 2-element array, e.g. [-10000, 10000]
             path:
-                Folder in which the fragments data will be stored
+                Folder in which the regions data will be stored
         """
         regions = canonical_transcripts[
             ["chrom", "start", "end", "ensembl_transcript_id"]
         ].copy()
 
         regions["tss"] = [
             genes_row["start"] if genes_row["strand"] == +1 else genes_row["end"]
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/transcriptome.py` & `chromatinhd-0.0.20/src/chromatinhd/data/transcriptome/transcriptome.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 import numpy as np
 import pandas as pd
 import pickle
+import pathlib
+from typing import Union
 
-from chromatinhd.flow import Flow, Stored, StoredDict
+from chromatinhd.flow import Flow, Stored, StoredDict, TSV
 from chromatinhd import sparse
 from chromatinhd.utils import Unpickler
 
 
 class Transcriptome(Flow):
-    _var = None
+    """
+    A transcriptome containing counts for each gene in each cell.
+    """
 
-    @property
-    def var(self):
-        if self._var is None:
-            self._var = pd.read_table(self.path / "var.tsv", index_col=0)
-        return self._var
-
-    @var.setter
-    def var(self, value):
-        value.index.name = "gene"
-        value.to_csv(self.path / "var.tsv", sep="\t")
-        self._var = value
-
-    _obs = None
-
-    @property
-    def obs(self):
-        if self._obs is None:
-            self._obs = pd.read_table(self.path / "obs.tsv", index_col=0)
-        return self._obs
-
-    @obs.setter
-    def obs(self, value):
-        value.index.name = "cell"
-        value.to_csv(self.path / "obs.tsv", sep="\t")
-        self._obs = value
+    var = TSV("var", index_name="gene")
+    obs = TSV("obs", index_name="gene")
 
     adata = Stored("adata")
-    """
-    Anndata object containing the transcriptome data.
-    """
+    "Anndata object containing the transcriptome data."
 
-    def gene_id(self, symbol):
+    def gene_id(self, symbol, column="symbol"):
         """
         Get the gene id for a given gene symbol.
         """
-        assert all(pd.Series(symbol).isin(self.var["symbol"])), set(
-            pd.Series(symbol)[~pd.Series(symbol).isin(self.var["symbol"])]
+        assert all(pd.Series(symbol).isin(self.var[column])), set(
+            pd.Series(symbol)[~pd.Series(symbol).isin(self.var[column])]
         )
-        return self.var.reset_index("gene").set_index("symbol").loc[symbol]["gene"]
+        return self.var.reset_index("gene").set_index(column).loc[symbol]["gene"]
 
-    def symbol(self, gene_id):
+    def symbol(self, gene_id, column="symbol"):
         """
-        Get the gene symbol for a given gene ID (e.g. Ensembl ID)
+        Get the gene symbol for a given gene ID (e.g. Ensembl ID).
         """
         assert all(pd.Series(gene_id).isin(self.var.index)), set(
             pd.Series(gene_id)[~pd.Series(gene_id).isin(self.var.index)]
         )
-        return self.var.loc[gene_id]["symbol"]
+        return self.var.loc[gene_id][column]
 
     def gene_ix(self, symbol):
         """
         Get the gene index for a given gene symbol.
         """
         self.var["ix"] = np.arange(self.var.shape[0])
         assert all(pd.Series(symbol).isin(self.var["symbol"])), set(
@@ -77,31 +56,36 @@
             X_scipy = scipy.sparse.csr_matrix(X_scipy)
         X = sparse.COOMatrix.from_scipy_csr(X_scipy)
         X.populate_mapping()
 
         self.X = X
 
     X = Stored("X")
+    "Raw counts for each gene in each cell."
 
     @classmethod
-    def from_adata(cls, adata, path):
+    def from_adata(cls, adata, path: Union[pathlib.Path, str]):
         """
         Create a Transcriptome object from an AnnData object.
+
+        Parameters:
+            adata:
+                Anndata object containing the transcriptome data.
+            path:
+                Folder in which the transcriptome data will be stored.
         """
         transcriptome = cls(path=path)
         transcriptome.adata = adata
         transcriptome.layers["X"] = adata.X
         transcriptome.var = adata.var
         transcriptome.obs = adata.obs
         return transcriptome
 
     layers = StoredDict("layers", Stored)
-    """
-    Dictionary of layers, such as raw, normalized and imputed data.
-    """
+    "Dictionary of layers, such as raw, normalized and imputed data."
 
 
 class ClusterTranscriptome(Flow):
     var = Stored("var")
     obs = Stored("obs")
     adata = Stored("adata")
     X = Stored("X")
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/embedding.py` & `chromatinhd-0.0.20/src/chromatinhd/embedding.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/flow.py` & `chromatinhd-0.0.20/src/chromatinhd/flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     A folder on disk that can contain other folders or objects
     """
 
     path: pathlib.Path
     default_name = None
 
     def __init__(self, path=None, folder=None, name=None, reset=False):
+        if not isinstance(path, pathlib.Path):
+            path = pathlib.Path(path)
         if path is None:
             if folder is None:
                 raise ValueError("Either path or folder must be specified")
             if name is None:
                 if self.default_name is None:
                     raise ValueError(
                         "Cannot create Flow without name, and no default_name specified"
@@ -79,14 +81,17 @@
         """
         shutil.rmtree(self.path)
         self.path.mkdir(parents=True, exist_ok=True)
 
     def __getstate__(self):
         raise TypeError("This class cannot be pickled.")
 
+    def get(self, k):
+        return self.__class__.__dict__[k]
+
 
 class Linked:
     """
     A link to another flow on disk
     """
 
     def __init__(self, name):
@@ -148,14 +153,23 @@
             return getattr(obj, name)
 
     def __set__(self, obj, value):
         name = "_" + self.name
         pickle.dump(value, self.get_path(obj.path).open("wb"))
         setattr(obj, name, value)
 
+    def exists(self, obj):
+        return self.get_path(obj.path).exists()
+
+
+class StoredDataFrame(Stored):
+    """
+    A pandas dataframe stored on disk
+    """
+
 
 class StoredTorchInt64(Stored):
     """
     A pytorch int64 tensor stored on disk
     """
 
     def __get__(self, obj, type=None):
@@ -264,17 +278,18 @@
 
 
 class TSV(Stored):
     """
     A pandas object stored on disk in tsv format
     """
 
-    def __init__(self, name, columns=None):
+    def __init__(self, name, columns=None, index_name=None):
         super().__init__(name)
         self.columns = columns
+        self.index_name = index_name
 
     def get_path(self, folder):
         return folder / (self.name + ".tsv")
 
     def __get__(self, obj=None, type=None):
         if obj is not None:
             name = "_" + self.name
@@ -285,14 +300,16 @@
                 setattr(obj, name, x)
             return getattr(obj, name)
 
     def __set__(self, obj, value, folder=None):
         name = "_" + self.name
         if folder is None:
             folder = obj.path
+        if self.index_name is not None:
+            value.index.name = self.index_name
         value.to_csv(self.get_path(folder), sep="\t")
         setattr(obj, name, value)
 
 
 class StoredDict:
     def __init__(self, name, cls):
         self.name = name
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/grid/broken.py` & `chromatinhd-0.0.20/src/chromatinhd/grid/broken.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/grid/grid.py` & `chromatinhd-0.0.20/src/chromatinhd/grid/grid.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/chunkfragments.py` & `chromatinhd-0.0.20/src/chromatinhd/loaders/chunkfragments.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/fragments.pyx` & `chromatinhd-0.0.20/src/chromatinhd/loaders/extraction/fragments.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/motifs.pyx` & `chromatinhd-0.0.20/src/chromatinhd/loaders/extraction/motifs.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/fragmentmotif.py` & `chromatinhd-0.0.20/src/chromatinhd/loaders/fragmentmotif.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import numpy as np
+
 import pyximport
 
 pyximport.install(
     reload_support=True,
     language_level=3,
     setup_args=dict(include_dirs=[np.get_include()]),
 )
@@ -77,27 +78,27 @@
             *self.window,
             self.window_width,
             *self.cutwindow,
             self.out_fragment_indptr.numpy(),
             self.out_motif_ix.numpy(),
             self.out_score.numpy(),
             self.out_distance.numpy(),
-            self.out_motifcounts.numpy()
+            self.out_motifcounts.numpy(),
         )
         self.out_fragment_indptr.resize_(n_fragments + 1)
         self.out_motif_ix.resize_(n_motifs)
         self.out_score.resize_(n_motifs)
         self.out_distance.resize_(n_motifs)
         self.out_motifcounts.resize_((n_fragments, self.out_motifcounts.shape[1]))
 
         return FullResult(
             motifcounts=self.out_motifcounts,
             local_cellxgene_ix=self.out_local_cellxgene_ix,
             n_fragments=n_fragments,
-            **minibatch.items()
+            **minibatch.items(),
         )
 
 
 @dataclasses.dataclass
 class MotifcountsResult(Result):
     motifcounts: torch.Tensor
 
@@ -132,25 +133,25 @@
             self.out_genemapping.numpy(),
             self.motifscan_indptr,
             self.motifscan_indices,
             self.motifscan_data,
             *self.window,
             self.window_width,
             *self.cutwindow,
-            out_motifcounts
+            out_motifcounts,
         )
         out_motifcounts.resize((n_fragments, self.n_features))
 
         return MotifcountsResult(
             motifcounts=torch.from_numpy(out_motifcounts).to(torch.float),
             local_cellxgene_ix=self.out_local_cellxgene_ix,
             coordinates=self.out_coordinates,
             genemapping=self.out_genemapping,
             n_fragments=n_fragments,
-            **minibatch.items()
+            **minibatch.items(),
         )
 
 
 class MotifcountsSplit(Fragments):
     def __init__(
         self, fragments, motifscan, cellxgene_batch_size, window, cutwindow, **kwargs
     ):
@@ -181,25 +182,25 @@
             self.motifscan_indptr,
             self.motifscan_indices,
             self.motifscan_data,
             self.n_motifs,
             *self.window,
             self.window_width,
             *self.cutwindow,
-            out_motifcounts
+            out_motifcounts,
         )
         out_motifcounts.resize((n_fragments, self.n_features))
 
         return MotifcountsResult(
             motifcounts=torch.from_numpy(out_motifcounts).to(torch.float),
             local_cellxgene_ix=self.out_local_cellxgene_ix,
             coordinates=self.out_coordinates,
             genemapping=self.out_genemapping,
             n_fragments=n_fragments,
-            **minibatch.items()
+            **minibatch.items(),
         )
 
 
 class MotifcountsMultiple(Fragments):
     def __init__(
         self, fragments, motifscan, cellxgene_batch_size, window, cutwindows, **kwargs
     ):
@@ -229,38 +230,38 @@
             self.motifscan_indptr,
             self.motifscan_indices,
             self.motifscan_data,
             self.n_motifs,
             *self.window,
             self.window_width,
             self.cutwindows,
-            out_motifcounts
+            out_motifcounts,
         )
         out_motifcounts.resize((n_fragments, self.n_features))
 
         return MotifcountsResult(
             motifcounts=torch.from_numpy(out_motifcounts).to(torch.float),
             local_cellxgene_ix=self.out_local_cellxgene_ix,
             coordinates=self.out_coordinates,
             genemapping=self.out_genemapping,
             n_fragments=n_fragments,
-            **minibatch.items()
+            **minibatch.items(),
         )
 
 
 class MotifcountsRelative(Fragments):
     def __init__(
         self,
         fragments,
         motifscan,
         cellxgene_batch_size,
         window,
         cutwindow,
         promoter_width,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(fragments, cellxgene_batch_size, window, **kwargs)
 
         # store auxilliary information
         self.cutwindow = cutwindow
         self.cutwindow_width = cutwindow[1] - cutwindow[0]
 
@@ -288,19 +289,19 @@
             self.motifscan_indices,
             self.motifscan_data,
             self.n_motifs,
             *self.window,
             self.window_width,
             *self.cutwindow,
             self.promoter_width,
-            out_motifcounts
+            out_motifcounts,
         )
         out_motifcounts.resize((n_fragments, self.n_features))
 
         return MotifcountsResult(
             motifcounts=torch.from_numpy(out_motifcounts).to(torch.float),
             local_cellxgene_ix=self.out_local_cellxgene_ix,
             coordinates=self.out_coordinates,
             genemapping=self.out_genemapping,
             n_fragments=n_fragments,
-            **minibatch.items()
+            **minibatch.items(),
         )
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/fragments.py` & `chromatinhd-0.0.20/src/chromatinhd/loaders/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import torch
 import numpy as np
-import pyximport
 from typing import List
 
+import pyximport
+
 pyximport.install(
     reload_support=True,
     language_level=3,
     setup_args=dict(include_dirs=[np.get_include()]),
 )
-import chromatinhd.data.fragments
 import chromatinhd.loaders.extraction.fragments
+
+import chromatinhd.data.fragments
+
 import dataclasses
 from functools import cached_property
 
 
 @dataclasses.dataclass
 class Result:
     coordinates: torch.Tensor
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/minibatching.py` & `chromatinhd-0.0.20/src/chromatinhd/loaders/minibatching.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/peakcounts.py` & `chromatinhd-0.0.20/src/chromatinhd/loaders/peakcounts.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/loaders/pool.py` & `chromatinhd-0.0.20/src/chromatinhd/loaders/pool.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/__init__.py` & `chromatinhd-0.0.20/src/chromatinhd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/differential.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/differential.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/enrichment.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/enrichment/enrichment.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/genepositional.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/interpret/genepositional.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,63 @@
 import chromatinhd as chd
 import numpy as np
 import pandas as pd
 import xarray as xr
 import pickle
-import scipy.stats
 import tqdm.auto as tqdm
 import torch
+from chromatinhd import default_device
+from chromatinhd.data.clustering import Clustering
+from chromatinhd.data.fragments import Fragments
+from chromatinhd.models.diff.model.cutnf import Models
 
 
 def fdr(p_vals):
     from scipy.stats import rankdata
 
     ranked_p_values = rankdata(p_vals)
     fdr = p_vals * len(p_vals) / ranked_p_values
     fdr[fdr > 1] = 1
 
     return fdr
 
 
 class GenePositional(chd.flow.Flow):
+    """
+    Positional interpretation of *diff* models
+    """
+
     genes = chd.flow.Stored("genes", default=set)
 
     def score(
         self,
-        fragments,
-        clustering,
-        models,
-        folds,
+        fragments: Fragments,
+        clustering: Clustering,
+        models: Models,
         genes=None,
         force=False,
-        device="cuda",
+        device=default_device,
     ):
+        """
+        Main scoring function
+
+        Parameters:
+            fragments:
+                the fragments
+            clustering:
+                the clustering
+            models:
+                the models
+            genes:
+                the genes to score, if None, all genes are scored
+            force:
+                whether to force rescoring even if the scores already exist
+            device:
+                the device to use
+        """
         force_ = force
 
         if genes is None:
             genes = fragments.var.index
 
         pbar = tqdm.tqdm(genes, leave=False)
 
@@ -90,14 +113,15 @@
                             design_subset["gene_ix"].values.astype(int)
                         )
 
                         prob = model.evaluate_pseudo(
                             pseudocoordinates,
                             clustering=pseudocluster,
                             gene_ix=gene_ix,
+                            device=device,
                         )
 
                         probs_model.append(prob.numpy())
                     probs_model = np.hstack(probs_model)
                     probs.append(probs_model)
 
                 probs = np.vstack(probs)
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/clustering.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering_cuts.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/clustering_cuts.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/cuts.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/cuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import torch
 import numpy as np
-import pyximport
 
-pyximport.install(
-    reload_support=True,
-    language_level=3,
-    setup_args=dict(include_dirs=[np.get_include()]),
-)
-from . import fragments_helpers  # pylint: disable=C0413,E0611
+# try to load the shared library
+# typically, this will be installed as a python extension
+try:
+    from . import fragments_helpers  # pylint: disable=C0413,E0611
+# however, during developement, we want to load the cython source directly
+except ImportError:
+    import pyximport
+
+    pyximport.install(
+        reload_support=True,
+        language_level=3,
+        setup_args=dict(include_dirs=[np.get_include()]),
+    )
+
 import dataclasses
 
 import chromatinhd.data.fragments
 
 
 @dataclasses.dataclass
 class Result:
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/fragments_helpers.pyx` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/fragments_helpers.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/minibatches.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/loader/minibatches.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/cutnf.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/model/cutnf.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,14 @@
 
         cell_mapping = np.zeros(fragments.n_cells, dtype=np.int64)
         cell_mapping[cell_ixs] = np.arange(len(cell_ixs))
 
         gene_mapping = np.zeros(fragments.n_genes, dtype=np.int64)
         gene_mapping[gene_ixs] = np.arange(len(gene_ixs))
 
-        device = "cuda"
         self.eval()
         self = self.to(device)
 
         for data in loaders:
             data = data.to(device)
             with torch.no_grad():
                 self.forward(data)
@@ -547,15 +546,15 @@
         prob = self.track["likelihood"].detach().cpu()
         return prob.detach().cpu()
 
     def rank(
         self,
         window: np.ndarray,
         n_latent: int,
-        device: torch.DeviceObjType = "cuda",
+        device: torch.DeviceObjType = default_device,
         how: str = "probs_diff_masked",
         prob_cutoff: float = None,
     ) -> np.ndarray:
         n_genes = self.rho_bias.shape[0]
 
         self = self.to(device).eval()
 
@@ -655,15 +654,15 @@
     @property
     def models_path(self):
         path = self.path / "models"
         path.mkdir(exist_ok=True)
         return path
 
     def train_models(
-        self, fragments, clustering, folds, device="cuda", n_epochs=30, **kwargs
+        self, fragments, clustering, folds, device=default_device, n_epochs=30, **kwargs
     ):
         """
         Trains the models
 
         Parameters:
             fragments:
                 Fragments object
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/spline.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/model/spline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import torch
 import tqdm.auto as tqdm
 import math
 from chromatinhd.models.diff.model import splines
 from chromatinhd.embedding import EmbeddingTensor
 
+from chromatinhd import default_device
+
 
 class TransformedDistribution(torch.nn.Module):
     def __init__(self, transform):
         super().__init__()
         self.transform = transform
 
     def log_prob(self, x, *args, **kwargs):
         log_prob = torch.zeros_like(x)
         x_ = x
         x_, logabsdet = self.transform.transform_forward(x_, *args, **kwargs)
         log_prob = log_prob + logabsdet
         return log_prob
 
-    def sample(self, sample_shape=torch.Size(), *args, device=None, **kwargs):
+    def sample(self, *args, sample_shape=torch.Size(), device=None, **kwargs):
         y = torch.rand(sample_shape, device=device)
         y, _ = self.transform.transform_inverse(y, *args, **kwargs)
         return y
 
     def parameters_sparse(self):
         return self.transform.parameters_sparse()
 
     def parameters_dense(self):
         return self.transform.parameters_dense()
 
+    def forward(self, input):
+        pass
+
 
 class QuadraticSplineTransform(torch.nn.Module):
     bijective = True
     domain = torch.distributions.constraints.real
     codomain = torch.distributions.constraints.real
 
     def __init__(self, unnormalized_widths, unnormalized_heights):
@@ -74,15 +79,17 @@
 
     chosen_idx = torch.argsort(-possible_scores.abs())[: (n - 2)]
     chosen = torch.nn.functional.pad(torch.sort(possible[chosen_idx])[0], (1, 1))
     chosen[..., -1] = 1.0
     return chosen
 
 
-def initialize_from_previous(x, n, local_gene_ix, n_genes, transforms, device="cuda"):
+def initialize_from_previous(
+    x, n, local_gene_ix, n_genes, transforms, device=default_device
+):
     q2_orig = torch.linspace(0, 1, n).expand(n_genes, -1)
     # q2_orig = prioritize(x, n).expand(n_genes, -1)
     q2 = q2_orig
 
     # calculate bin widths
     for transform in transforms:
         q2 = (
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/cubic.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/cubic.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/linear.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/linear.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/quadratic.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/model/splines/quadratic.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/__init__.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/plot/differential.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential_expression.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/plot/differential_expression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import matplotlib as mpl
 import seaborn as sns
 import pandas as pd
 import numpy as np
 import chromatinhd
-import scanpy as sc
 
 
 def get_cmap_rna_diff():
     return mpl.cm.BuGn
 
 
 class DifferentialExpression(chromatinhd.grid.Wrap):
@@ -81,14 +80,16 @@
                 va="center",
             )
 
     @classmethod
     def from_transcriptome(
         cls, transcriptome, clustering, gene, width=0.5, panel_height=0.5, **kwargs
     ):
+        import scanpy as sc
+
         transcriptome.adata.obs["cluster"] = clustering.labels
         plotdata_expression = sc.get.obs_df(
             transcriptome.adata, [gene, "cluster"]
         ).rename(columns={gene: "expression"})
         plotdata_expression_clusters = plotdata_expression.groupby("cluster")[
             "expression"
         ].mean()
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/trainer.py` & `chromatinhd-0.0.20/src/chromatinhd/models/diff/trainer/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tqdm.auto as tqdm
 import torch
 import numpy as np
 from chromatinhd.train import Trace
+from chromatinhd import default_device
 
 import logging
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 
@@ -16,15 +17,15 @@
         loaders_train,
         loaders_validation,
         minibatcher_train,
         minibatcher_validation,
         optim,
         hooks_checkpoint=None,
         hooks_checkpoint2=None,
-        device="cuda",
+        device=default_device,
         n_epochs=30,
         checkpoint_every_epoch=1,
         optimize_every_step=1,
     ):
         self.model = model
         self.loaders_train = loaders_train
         self.loaders_validation = loaders_validation
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/censorers.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/censorers.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genemultiwindow.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/genemultiwindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import chromatinhd as chd
 import numpy as np
 import pandas as pd
 import xarray as xr
 import pickle
 import scipy.stats
 import tqdm.auto as tqdm
+from chromatinhd import default_device
 
 
 def fdr(p_vals):
     from scipy.stats import rankdata
 
     ranked_p_values = rankdata(p_vals)
-    fdr = p_vals * len(p_vals) / ranked_p_values
-    fdr[fdr > 1] = 1
+    qval = p_vals * len(p_vals) / ranked_p_values
+    qval[qval > 1] = 1
 
-    return fdr
+    return qval
 
 
 class GeneMultiWindow(chd.flow.Flow):
     """
     Interpret a *pred* model positionally by censoring windows of across multiple window sizes.
     """
 
@@ -37,15 +38,15 @@
         fragments,
         transcriptome,
         models,
         folds,
         genes,
         censorer,
         force=False,
-        device="cuda",
+        device=default_device,
     ):
         force_ = force
         design = censorer.design.iloc[1:].copy()
         self.design = design
 
         pbar = tqdm.tqdm(genes, leave=False)
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genepairwindow.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/interpret/genepairwindow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,85 @@
-import chromatinhd as chd
+import itertools
+import pickle
+from typing import List, Optional
+
 import numpy as np
 import pandas as pd
-import xarray as xr
-import pickle
-import scipy.stats
 import tqdm.auto as tqdm
-import numpy as np
-import itertools
+import xarray as xr
+
+import chromatinhd as chd
+from chromatinhd import default_device
+from chromatinhd.data.folds import Folds
+from chromatinhd.data.fragments import Fragments
+from chromatinhd.data.transcriptome import Transcriptome
+from chromatinhd.models.pred.model.additive import Models
 
 
 def zscore(x, dim=0):
     return (x - x.mean(axis=dim, keepdims=True)) / x.std(axis=dim, keepdims=True)
 
 
 def zscore_relative(x, y, dim=0):
     return (x - y.mean(axis=dim, keepdims=True)) / y.std(axis=dim, keepdims=True)
 
 
 def fdr(p_vals):
     from scipy.stats import rankdata
 
     ranked_p_values = rankdata(p_vals)
-    fdr = p_vals * len(p_vals) / ranked_p_values
-    fdr[fdr > 1] = 1
+    qval = p_vals * len(p_vals) / ranked_p_values
+    qval[qval > 1] = 1
 
-    return fdr
+    return qval
 
 
 class GenePairWindow(chd.flow.Flow):
+    """
+    Interpret a *pred* model positionally by censoring windows and comparing the decrease in predictivity per cell between pairs of windows
+    """
+
     design = chd.flow.Stored("design")
 
     genes = chd.flow.Stored("genes", default=set)
 
     def score(
         self,
-        fragments,
-        transcriptome,
-        models,
-        folds,
-        genes,
+        fragments: Fragments,
+        transcriptome: Transcriptome,
+        models: Models,
+        folds: Folds,
         censorer,
+        genes: Optional[List] = None,
         force=False,
-        device="cuda",
+        device=default_device,
     ):
+        """
+        Score the models
+
+        Parameters:
+            fragments:
+                the fragments
+            transcriptome:
+                the transcriptome
+            models:
+                the models
+            folds:
+                the folds
+            genes:
+                which genes to score, defaults to all
+
+        """
         force_ = force
         design = censorer.design.iloc[1:].copy()
         self.design = design
 
+        if genes is None:
+            genes = transcriptome.var.index
+
         pbar = tqdm.tqdm(genes, leave=False)
 
         for gene in pbar:
             pbar.set_description(gene)
             scores_file = self.get_scoring_path(gene) / "scores.pkl"
             interaction_file = self.get_scoring_path(gene) / "interaction.pkl"
 
@@ -106,15 +135,14 @@
 
                     deltacor_folds.append(deltacor)
                     lost_folds.append(lost)
 
                 lost_folds = np.stack(lost_folds, 0)
                 deltacor_folds = np.stack(deltacor_folds, 0)
                 copredictivity_folds = np.stack(copredictivity_folds, 0)
-                print(copredictivity_folds.shape)
 
                 result = xr.Dataset(
                     {
                         "deltacor": xr.DataArray(
                             deltacor_folds,
                             coords=[
                                 ("model", np.arange(len(models))),
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/fragments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import torch
 import numpy as np
-import pyximport
 
-pyximport.install(
-    reload_support=True,
-    language_level=3,
-    setup_args=dict(include_dirs=[np.get_include()]),
-)
-from . import fragments_helpers
+# try to load the shared library
+# typically, this will be installed as a python extension
+try:
+    from . import fragments_helpers  # pylint: disable=C0413,E0611
+# however, during developement, we want to load the cython source directly
+except ImportError:
+    import pyximport
+
+    pyximport.install(
+        reload_support=True,
+        language_level=3,
+        setup_args=dict(include_dirs=[np.get_include()]),
+    )
+
 import dataclasses
-from functools import cached_property
 
 import chromatinhd.data.fragments
 
 
 @dataclasses.dataclass
 class Result:
     coordinates: torch.Tensor
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments_helpers.pyx` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/fragments_helpers.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/minibatches.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/minibatches.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import dataclasses
 import itertools
 import math
 import torch
+import random
 
 
 @dataclasses.dataclass
 class Minibatch:
     cells_oi: np.ndarray
     genes_oi: np.ndarray
     phase: str = "train"
@@ -110,11 +111,18 @@
         gene_bins = [genes[a:b] for a, b in zip(gene_cuts[:-1], gene_cuts[1:])]
 
         cell_cuts = [*np.arange(0, len(cells), step=self.n_cells_step)]
         if self.use_all_cells:
             cell_cuts.append(len(cells))
         cell_bins = [cells[a:b] for a, b in zip(cell_cuts[:-1], cell_cuts[1:])]
 
-        for cells_oi, genes_oi in itertools.product(cell_bins, gene_bins):
+        product = itertools.product(cell_bins, gene_bins)
+
+        if self.permute_cells and self.permute_genes:
+            rng = random.Random(self.i)
+            product = list(product)
+            rng.shuffle(list(product))
+
+        for cells_oi, genes_oi in product:
             yield Minibatch(cells_oi=cells_oi, genes_oi=genes_oi)
 
         self.i += 1
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/transcriptome.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import chromatinhd.data.transcriptome
 import dataclasses
 import torch
+import chromatinhd.sparse
 
 
 @dataclasses.dataclass
 class Result:
     value: torch.Tensor
 
     def to(self, device):
@@ -14,12 +15,18 @@
 
 class Transcriptome:
     def __init__(
         self,
         transcriptome: chromatinhd.data.transcriptome.Transcriptome,
         layer: str = "X",
     ):
-        self.X = torch.from_numpy(transcriptome.layers[layer])
+        X = transcriptome.layers[layer]
+        if chromatinhd.sparse.is_sparse(X):
+            self.X = X.dense()
+        elif torch.is_tensor(X):
+            self.X = X
+        else:
+            self.X = torch.from_numpy(X)
 
     def load(self, minibatch):
         X = self.X[minibatch.cells_oi, :][:, minibatch.genes_oi]
         return Result(value=X)
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome_fragments.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/loader/transcriptome_fragments.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/model/across.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/model/additive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 """
 Additive model for predicting gene expression from fragments
 """
 
 
-import math
-import pickle
-
-import numpy as np
-import pandas as pd
 import torch
 import torch_scatter
+import math
+import numpy as np
 import xarray as xr
+import pandas as pd
+
+import pickle
 
 from chromatinhd.embedding import EmbeddingTensor
-from chromatinhd.flow import Flow, Stored
-from chromatinhd.loaders import LoaderPool2
 from chromatinhd.models import HybridModel
+from chromatinhd.flow import Linked, Flow, Stored
+
 from chromatinhd.models.pred.loader.minibatches import Minibatcher
 from chromatinhd.models.pred.loader.transcriptome_fragments import (
     TranscriptomeFragments,
 )
+from chromatinhd.data.fragments import Fragments
+from chromatinhd.data.transcriptome import Transcriptome
 from chromatinhd.models.pred.trainer import Trainer
+from chromatinhd.loaders import LoaderPool2
 from chromatinhd.optim import SparseDenseAdam
 
+from chromatinhd import default_device
+
 from .loss import paircor, paircor_loss, gene_paircor_loss
 
+from typing import Any
+
 
 class SineEncoding(torch.nn.Module):
     def __init__(self, n_frequencies):
         super().__init__()
 
         self.register_buffer(
             "frequencies",
@@ -73,53 +80,66 @@
         self.dropout_rate = dropout_rate
 
         super().__init__(**kwargs)
 
         self.sine_encoding = SineEncoding(n_frequencies=n_frequencies)
 
         # default initialization same as a torch.nn.Linear
-        self.bias1 = torch.nn.Parameter(torch.zeros((self.n_embedding_dimensions,)))
+        self.bias1 = EmbeddingTensor(
+            n_genes,
+            (self.n_embedding_dimensions,),
+            sparse=True,
+        )
+        self.bias1.data.zero_()
 
-        self.weight1 = torch.nn.Parameter(
-            torch.zeros(
-                (
-                    self.sine_encoding.n_embedding_dimensions,
-                    self.n_embedding_dimensions,
-                ),
-            )
+        self.weight1 = EmbeddingTensor(
+            n_genes,
+            (
+                self.sine_encoding.n_embedding_dimensions,
+                self.n_embedding_dimensions,
+            ),
+            sparse=True,
         )
+        stdv = 1.0 / math.sqrt(self.weight1.shape[-1])  # / 100
+        self.weight1.data.uniform_(-stdv, stdv)
 
-    def forward(self, coordinates):
+    def forward(self, coordinates, gene_ix):
         embedding = self.sine_encoding(coordinates)
-        embedding = torch.matmul(embedding, self.weight1) + self.bias1
+        embedding = torch.einsum(
+            "ab,abc->ac", embedding, self.weight1(gene_ix)
+        ) + self.bias1(gene_ix)
+        # embedding = (embedding[..., None] * self.weight1[gene_ix]).sum(-2)
 
         # non-linear
         if self.nonlinear is True:
             embedding = torch.sigmoid(embedding)
         elif isinstance(self.nonlinear, str) and self.nonlinear == "relu":
             embedding = torch.relu(embedding)
         elif isinstance(self.nonlinear, str) and self.nonlinear == "elu":
             embedding = torch.nn.functional.elu(embedding)
 
         if self.dropout_rate > 0:
             embedding = torch.nn.functional.dropout(embedding, self.dropout_rate)
 
         return embedding
 
+    def parameters_sparse(self):
+        return [self.bias1.weight, self.weight1.weight]
+
 
 class FragmentEmbedderCounter(torch.nn.Sequential):
     """
     Dummy embedding of fragments in a single embedding dimension of ones
     """
 
     def __init__(self, *args, **kwargs):
         self.n_embedding_dimensions = 1
         super().__init__(*args, **kwargs)
 
-    def forward(self, coordinates):
+    def forward(self, coordinates, gene_ix):
         return torch.ones(
             (*coordinates.shape[:-1], 1), device=coordinates.device, dtype=torch.float
         )
 
 
 class EmbeddingGenePooler(torch.nn.Module):
     """
@@ -179,32 +199,57 @@
             self.weight1.data[:, :5] = 1.0
             self.weight1.data[:, 5:] = 0.0
             self.weight1.data[:, -1] = -1.0
         elif initialization == "smaller":
             stdv = 1.0 / math.sqrt(self.weight1.data.size(-1)) / 100
             self.weight1.data.uniform_(-stdv, stdv)
 
-    def forward(self, cell_gene_embedding):
-        out = torch.matmul(cell_gene_embedding, self.weight1) + self.bias1
+    def forward(self, cell_gene_embedding, gene_ix):
+        out = (cell_gene_embedding * self.weight1(gene_ix)).sum(-1) + self.bias1(
+            gene_ix
+        ).squeeze()
         return out
 
+    def parameters_sparse(self):
+        return [self.bias1.weight, self.weight1.weight]
+
 
 class Model(torch.nn.Module, HybridModel):
+    """
+    Predicting gene expression from raw fragments using an additive model across fragments from the same cell
+
+    Parameters:
+        n_genes:
+            the number of genes
+        dummy:
+            whether to use a dummy model that just counts fragments
+        n_frequencies:
+            the number of frequencies to use for sine encoding
+        reduce:
+            the reduction to use for pooling fragments across genes and cells
+        nonlinear:
+            whether to use a non-linear activation function
+        n_embedding_dimensions:
+            the number of embedding dimensions
+        dropout_rate:
+            the dropout rate
+    """
+
     def __init__(
         self,
-        n_genes,
-        dummy=False,
-        n_frequencies=50,
-        reduce="sum",
-        nonlinear=True,
-        n_embedding_dimensions=10,
-        dropout_rate=0.0,
-        embedding_to_expression_initialization="default",
-        **kwargs,
-    ):
+        n_genes: int,
+        dummy: bool = False,
+        n_frequencies: int = 50,
+        reduce: str = "sum",
+        nonlinear: bool = True,
+        n_embedding_dimensions: int = 10,
+        dropout_rate: float = 0.0,
+        embedding_to_expression_initialization: str = "default",
+        **kwargs: Any,
+    ) -> None:
         super().__init__()
 
         if dummy:
             self.fragment_embedder = FragmentEmbedderCounter()
         else:
             self.fragment_embedder = FragmentEmbedder(
                 n_frequencies=n_frequencies,
@@ -217,14 +262,17 @@
         self.embedding_to_expression = EmbeddingToExpression(
             n_genes=n_genes,
             n_embedding_dimensions=self.fragment_embedder.n_embedding_dimensions,
             initialization=embedding_to_expression_initialization,
         )
 
     def forward(self, data):
+        """
+        Make a prediction given a data object
+        """
         fragment_embedding = self.fragment_embedder(
             data.fragments.coordinates, data.fragments.genemapping
         )
         cell_gene_embedding = self.embedding_gene_pooler(
             fragment_embedding,
             data.fragments.local_cellxgene_ix,
             data.minibatch.n_cells,
@@ -232,19 +280,25 @@
         )
         expression_predicted = self.embedding_to_expression(
             cell_gene_embedding, data.minibatch.genes_oi_torch
         )
         return expression_predicted
 
     def forward_loss(self, data):
+        """
+        Make a prediction and calculate the loss given a data object
+        """
         expression_predicted = self.forward(data)
         expression_true = data.transcriptome.value
         return paircor_loss(expression_predicted, expression_true)
 
     def forward_gene_loss(self, data):
+        """
+        Make a prediction and calculate the loss given a data object
+        """
         expression_predicted = self.forward(data)
         expression_true = data.transcriptome.value
         return gene_paircor_loss(expression_predicted, expression_true)
 
     def forward_multiple(self, data, fragments_oi, min_fragments=1):
         fragment_embedding = self.fragment_embedder(
             data.fragments.coordinates, data.fragments.genemapping
@@ -259,15 +313,15 @@
             fragment_embedding,
             data.fragments.local_cellxgene_ix,
             data.minibatch.n_cells,
             data.minibatch.n_genes,
         )
 
         total_expression_predicted = self.embedding_to_expression.forward(
-            total_cell_gene_embedding
+            total_cell_gene_embedding, data.minibatch.genes_oi_torch
         )
 
         for fragments_oi_ in fragments_oi:
             if (fragments_oi_ is not None) and ((~fragments_oi_).sum() > min_fragments):
                 lost_fragments_oi = ~fragments_oi_
                 lost_local_cellxgene_ix = data.fragments.local_cellxgene_ix[
                     lost_fragments_oi
@@ -283,23 +337,34 @@
                         lost_local_cellxgene_ix,
                         data.minibatch.n_cells,
                         data.minibatch.n_genes,
                     )
                 )
 
                 expression_predicted = self.embedding_to_expression.forward(
-                    cell_gene_embedding
+                    cell_gene_embedding, data.minibatch.genes_oi_torch
                 )
             else:
                 n_fragments = total_n_fragments
                 expression_predicted = total_expression_predicted
 
             yield expression_predicted, n_fragments
 
-    def train_model(self, fragments, transcriptome, fold, device="cuda"):
+    def train_model(
+        self,
+        fragments: Fragments,
+        transcriptome: Transcriptome,
+        fold: list,
+        device=default_device,
+        lr=1e-2,
+        n_epochs=30,
+    ):
+        """
+        Train the model
+        """
         # set up minibatchers and loaders
         minibatcher_train = Minibatcher(
             fold["cells_train"],
             range(fragments.n_genes),
             n_genes_step=500,
             n_cells_step=200,
         )
@@ -336,18 +401,18 @@
             loaders_train,
             loaders_validation,
             minibatcher_train,
             minibatcher_validation,
             SparseDenseAdam(
                 self.parameters_sparse(),
                 self.parameters_dense(),
-                lr=1e-2,
+                lr=lr,
                 weight_decay=1e-5,
             ),
-            n_epochs=30,
+            n_epochs=n_epochs,
             checkpoint_every_epoch=1,
             optimize_every_step=1,
             device=device,
         )
 
         trainer.train()
         # trainer.trace.plot()
@@ -356,15 +421,15 @@
         self,
         fragments,
         transcriptome,
         cells=None,
         cell_ixs=None,
         genes=None,
         gene_ixs=None,
-        device="cuda",
+        device=default_device,
         return_raw=False,
     ):
         """
         Returns the prediction of a dataset
         """
         if cell_ixs is None:
             if cells is None:
@@ -399,22 +464,24 @@
                 fragments=fragments,
                 cellxgene_batch_size=minibatches.cellxgene_batch_size,
             ),
             n_workers=5,
         )
         loaders.initialize(minibatches)
 
-        predicted = np.zeros((len(cell_ixs), fragments.n_genes))
-        expected = np.zeros((len(cell_ixs), fragments.n_genes))
-        n_fragments = np.zeros((len(cell_ixs), fragments.n_genes))
+        predicted = np.zeros((len(cell_ixs), len(gene_ixs)))
+        expected = np.zeros((len(cell_ixs), len(gene_ixs)))
+        n_fragments = np.zeros((len(cell_ixs), len(gene_ixs)))
 
         cell_mapping = np.zeros(fragments.n_cells, dtype=np.int64)
         cell_mapping[cell_ixs] = np.arange(len(cell_ixs))
 
-        device = "cuda"
+        gene_mapping = np.zeros(fragments.n_genes, dtype=np.int64)
+        gene_mapping[gene_ixs] = np.arange(len(gene_ixs))
+
         self.eval()
         self = self.to(device)
 
         for data in loaders:
             data = data.to(device)
             with torch.no_grad():
                 pred_mb = self.forward(data)
@@ -443,40 +510,40 @@
             return predicted, expected, n_fragments
 
         result = xr.Dataset(
             {
                 "predicted": xr.DataArray(
                     predicted,
                     dims=("cell", "gene"),
-                    coords={"cell": cells, "gene": fragments.var.index},
+                    coords={"cell": cells, "gene": genes},
                 ),
                 "expected": xr.DataArray(
                     expected,
                     dims=("cell", "gene"),
-                    coords={"cell": cells, "gene": fragments.var.index},
+                    coords={"cell": cells, "gene": genes},
                 ),
                 "n_fragments": xr.DataArray(
                     n_fragments,
                     dims=("cell", "gene"),
-                    coords={"cell": cells, "gene": fragments.var.index},
+                    coords={"cell": cells, "gene": genes},
                 ),
             }
         )
         return result
 
     def get_prediction_censored(
         self,
         fragments,
         transcriptome,
         censorer,
         cells=None,
         cell_ixs=None,
         genes=None,
         gene_ixs=None,
-        device="cuda",
+        device=default_device,
     ):
         """
         Returns the prediction of multiple censored dataset
         """
         if cell_ixs is None:
             if cells is None:
                 cells = fragments.obs.index
@@ -558,15 +625,15 @@
 
     @property
     def models_path(self):
         path = self.path / "models"
         path.mkdir(exist_ok=True)
         return path
 
-    def train_models(self, fragments, transcriptome, folds, device="cuda"):
+    def train_models(self, fragments, transcriptome, folds, device=default_device):
         self.n_models = len(folds)
         for fold_ix, fold in [(fold_ix, fold) for fold_ix, fold in enumerate(folds)]:
             desired_outputs = [self.models_path / ("model_" + str(fold_ix) + ".pkl")]
             force = False
             if not all([desired_output.exists() for desired_output in desired_outputs]):
                 force = True
 
@@ -591,15 +658,15 @@
     def __len__(self):
         return self.n_models
 
     def __iter__(self):
         for ix in range(len(self)):
             yield self[ix]
 
-    def get_gene_cors(self, fragments, transcriptome, folds, device="cuda"):
+    def get_gene_cors(self, fragments, transcriptome, folds, device=default_device):
         cor_predicted = np.zeros((len(fragments.var.index), len(folds)))
         cor_n_fragments = np.zeros((len(fragments.var.index), len(folds)))
         n_fragments = np.zeros((len(fragments.var.index), len(folds)))
         for model_ix, (model, fold) in enumerate(zip(self, folds)):
             prediction = model.get_prediction(
                 fragments, transcriptome, cell_ixs=fold["cells_test"], device=device
             )
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/model/additive.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/model/across.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
 Additive model for predicting gene expression from fragments
 """
 
+import pickle
 
+import numpy as np
+import pandas as pd
 import torch
 import torch_scatter
-import math
-import numpy as np
 import xarray as xr
-import pandas as pd
-
-import pickle
 
-from chromatinhd.embedding import EmbeddingTensor
+from chromatinhd.flow import Flow, Stored
+from chromatinhd.loaders import LoaderPool2
 from chromatinhd.models import HybridModel
-from chromatinhd.flow import Linked, Flow, Stored
-
 from chromatinhd.models.pred.loader.minibatches import Minibatcher
 from chromatinhd.models.pred.loader.transcriptome_fragments import (
     TranscriptomeFragments,
 )
-from chromatinhd.models.pred.trainer import Trainer
-from chromatinhd.loaders import LoaderPool2
+from chromatinhd.models.pred.trainer import Trainer2
 from chromatinhd.optim import SparseDenseAdam
 
-from .loss import paircor, paircor_loss, gene_paircor_loss
+from chromatinhd import default_device
+
+from .loss import gene_paircor_loss, paircor, paircor_loss
 
 
 class SineEncoding(torch.nn.Module):
-    def __init__(self, n_frequencies):
+    def __init__(self, n_frequencies, add_length=False):
         super().__init__()
 
         self.register_buffer(
             "frequencies",
             torch.tensor(
                 [
                     [1 / 1000 ** (2 * i / n_frequencies)] * 2
@@ -45,95 +43,124 @@
             torch.tensor(
                 [[0, torch.pi / 2] for _ in range(1, n_frequencies + 1)]
             ).flatten(-2),
         )
 
         self.n_embedding_dimensions = n_frequencies * 2 * 2
 
+        if add_length:
+            self.n_embedding_dimensions += n_frequencies * 2
+        self.add_length = add_length
+
     def forward(self, coordinates):
         embedding = torch.sin(
             (coordinates[..., None] * self.frequencies + self.shifts).flatten(-2)
         )
+        if self.add_length:
+            embedding = torch.cat(
+                [
+                    embedding,
+                    torch.sin(
+                        (
+                            (coordinates[..., 0, None] - coordinates[..., 1, None])[
+                                ..., None
+                            ]
+                            * self.frequencies
+                            + self.shifts
+                        ).flatten(-2)
+                    ),
+                ],
+                -1,
+            )
         return embedding
 
 
 class FragmentEmbedder(torch.nn.Module):
     dropout_rate = 0.0
 
     def __init__(
         self,
-        n_genes,
         n_frequencies=10,
         n_embedding_dimensions=5,
+        n_layers=1,
         nonlinear=True,
         dropout_rate=0.0,
+        add_length=False,
+        add_residual_count=False,
         **kwargs,
     ):
         self.n_embedding_dimensions = n_embedding_dimensions
 
         self.nonlinear = nonlinear
         self.dropout_rate = dropout_rate
 
         super().__init__(**kwargs)
 
-        self.sine_encoding = SineEncoding(n_frequencies=n_frequencies)
+        self.sine_encoding = SineEncoding(
+            n_frequencies=n_frequencies, add_length=add_length
+        )
 
-        # default initialization same as a torch.nn.Linear
-        self.bias1 = EmbeddingTensor(
-            n_genes,
-            (self.n_embedding_dimensions,),
-            sparse=True,
-        )
-        self.bias1.data.zero_()
-
-        self.weight1 = EmbeddingTensor(
-            n_genes,
-            (
-                self.sine_encoding.n_embedding_dimensions,
-                self.n_embedding_dimensions,
-            ),
-            sparse=True,
+        layers = []
+        for layer_ix in range(n_layers):
+            if layer_ix == 0:
+                layers.append(
+                    torch.nn.Linear(
+                        self.sine_encoding.n_embedding_dimensions,
+                        self.n_embedding_dimensions,
+                    )
+                )
+            else:
+                layers.append(
+                    torch.nn.Linear(
+                        self.n_embedding_dimensions, self.n_embedding_dimensions
+                    )
+                )
+            layers.append(torch.nn.Sigmoid())
+            if self.dropout_rate > 0:
+                layers.append(torch.nn.Dropout(self.dropout_rate))
+        layers.append(
+            torch.nn.Linear(self.n_embedding_dimensions, self.n_embedding_dimensions)
         )
-        stdv = 1.0 / math.sqrt(self.weight1.shape[-1])  # / 100
-        self.weight1.data.uniform_(-stdv, stdv)
 
-    def forward(self, coordinates, gene_ix):
+        self.nn = torch.nn.Sequential(*layers)
+
+        if add_residual_count:
+            self.n_embedding_dimensions += 1
+        self.add_residual_count = add_residual_count
+
+    def forward(self, coordinates):
         embedding = self.sine_encoding(coordinates)
-        embedding = torch.einsum(
-            "ab,abc->ac", embedding, self.weight1(gene_ix)
-        ) + self.bias1(gene_ix)
-        # embedding = (embedding[..., None] * self.weight1[gene_ix]).sum(-2)
-
-        # non-linear
-        if self.nonlinear is True:
-            embedding = torch.sigmoid(embedding)
-        elif isinstance(self.nonlinear, str) and self.nonlinear == "relu":
-            embedding = torch.relu(embedding)
-        elif isinstance(self.nonlinear, str) and self.nonlinear == "elu":
-            embedding = torch.nn.functional.elu(embedding)
+        embedding = self.nn(embedding)
 
-        if self.dropout_rate > 0:
-            embedding = torch.nn.functional.dropout(embedding, self.dropout_rate)
+        if self.add_residual_count:
+            embedding = torch.cat(
+                [
+                    embedding,
+                    torch.ones(
+                        (*coordinates.shape[:-1], 1),
+                        device=coordinates.device,
+                        dtype=torch.float,
+                    ),
+                ],
+                -1,
+            )
 
         return embedding
 
-    def parameters_sparse(self):
-        return [self.bias1.weight, self.weight1.weight]
 
-
-class FragmentEmbedderCounter(torch.nn.Sequential):
+class FragmentEmbedderCounter(torch.nn.Module):
     """
     Dummy embedding of fragments in a single embedding dimension of ones
     """
 
     def __init__(self, *args, **kwargs):
         self.n_embedding_dimensions = 1
         super().__init__(*args, **kwargs)
 
-    def forward(self, coordinates, gene_ix):
+    def forward(self, coordinates):
         return torch.ones(
             (*coordinates.shape[:-1], 1), device=coordinates.device, dtype=torch.float
         )
 
 
 class EmbeddingGenePooler(torch.nn.Module):
     """
@@ -162,100 +189,85 @@
 
 
 class EmbeddingToExpression(torch.nn.Module):
     """
     Predicts gene expression using a [cell, gene, component] embedding in a gene-specific manner
     """
 
-    def __init__(
-        self, n_genes, n_embedding_dimensions=5, initialization="default", **kwargs
-    ):
-        self.n_genes = n_genes
+    def __init__(self, n_embedding_dimensions=5, n_layers=1):
         self.n_embedding_dimensions = n_embedding_dimensions
 
         super().__init__()
 
-        # set bias to empirical mean
-        self.bias1 = EmbeddingTensor(
-            n_genes,
-            tuple(),
-            sparse=True,
-        )
-        self.bias1.data[:] = 0.0
-
-        self.weight1 = EmbeddingTensor(
-            n_genes,
-            (n_embedding_dimensions,),
-            sparse=True,
-        )
-        if initialization == "ones":
-            self.weight1.data[:] = 1.0
-        elif initialization == "default":
-            self.weight1.data[:, :5] = 1.0
-            self.weight1.data[:, 5:] = 0.0
-            self.weight1.data[:, -1] = -1.0
-        elif initialization == "smaller":
-            stdv = 1.0 / math.sqrt(self.weight1.data.size(-1)) / 100
-            self.weight1.data.uniform_(-stdv, stdv)
-
-    def forward(self, cell_gene_embedding, gene_ix):
-        out = (cell_gene_embedding * self.weight1(gene_ix)).sum(-1) + self.bias1(
-            gene_ix
-        ).squeeze()
-        return out
+        layers = []
+        for layer_ix in range(n_layers):
+            if layer_ix == 0:
+                layers.append(
+                    torch.nn.Linear(
+                        self.n_embedding_dimensions, self.n_embedding_dimensions
+                    )
+                )
+            else:
+                layers.append(
+                    torch.nn.Linear(
+                        self.n_embedding_dimensions, self.n_embedding_dimensions
+                    )
+                )
+            layers.append(torch.nn.Sigmoid())
+        layers.append(torch.nn.Linear(self.n_embedding_dimensions, 1))
+        self.nn = torch.nn.Sequential(*layers)
 
-    def parameters_sparse(self):
-        return [self.bias1.weight, self.weight1.weight]
+    def forward(self, cell_gene_embedding):
+        out = self.nn(cell_gene_embedding).squeeze(-1)
+        return out
 
 
 class Model(torch.nn.Module, HybridModel):
     def __init__(
         self,
-        n_genes,
         dummy=False,
         n_frequencies=50,
+        n_fragment_embedder_layers=1,
+        n_embedding_to_expression_layers=1,
         reduce="sum",
         nonlinear=True,
         n_embedding_dimensions=10,
         dropout_rate=0.0,
-        embedding_to_expression_initialization="default",
-        **kwargs,
+        add_length=False,
+        add_residual_count=False,
     ):
         super().__init__()
 
         if dummy:
             self.fragment_embedder = FragmentEmbedderCounter()
         else:
             self.fragment_embedder = FragmentEmbedder(
                 n_frequencies=n_frequencies,
-                n_genes=n_genes,
                 nonlinear=nonlinear,
                 n_embedding_dimensions=n_embedding_dimensions,
                 dropout_rate=dropout_rate,
+                n_layers=n_fragment_embedder_layers,
+                add_length=add_length,
+                add_residual_count=add_residual_count,
             )
         self.embedding_gene_pooler = EmbeddingGenePooler(reduce=reduce)
         self.embedding_to_expression = EmbeddingToExpression(
-            n_genes=n_genes,
             n_embedding_dimensions=self.fragment_embedder.n_embedding_dimensions,
-            initialization=embedding_to_expression_initialization,
+            n_layers=n_embedding_to_expression_layers if not dummy else 0,
         )
 
     def forward(self, data):
-        fragment_embedding = self.fragment_embedder(
-            data.fragments.coordinates, data.fragments.genemapping
-        )
+        fragment_embedding = self.fragment_embedder(data.fragments.coordinates)
         cell_gene_embedding = self.embedding_gene_pooler(
             fragment_embedding,
             data.fragments.local_cellxgene_ix,
             data.minibatch.n_cells,
             data.minibatch.n_genes,
         )
-        expression_predicted = self.embedding_to_expression(
-            cell_gene_embedding, data.minibatch.genes_oi_torch
-        )
+        expression_predicted = self.embedding_to_expression(cell_gene_embedding)
         return expression_predicted
 
     def forward_loss(self, data):
         expression_predicted = self.forward(data)
         expression_true = data.transcriptome.value
         return paircor_loss(expression_predicted, expression_true)
 
@@ -278,15 +290,15 @@
             fragment_embedding,
             data.fragments.local_cellxgene_ix,
             data.minibatch.n_cells,
             data.minibatch.n_genes,
         )
 
         total_expression_predicted = self.embedding_to_expression.forward(
-            total_cell_gene_embedding, data.minibatch.genes_oi_torch
+            total_cell_gene_embedding
         )
 
         for fragments_oi_ in fragments_oi:
             if (fragments_oi_ is not None) and ((~fragments_oi_).sum() > min_fragments):
                 lost_fragments_oi = ~fragments_oi_
                 lost_local_cellxgene_ix = data.fragments.local_cellxgene_ix[
                     lost_fragments_oi
@@ -302,35 +314,37 @@
                         lost_local_cellxgene_ix,
                         data.minibatch.n_cells,
                         data.minibatch.n_genes,
                     )
                 )
 
                 expression_predicted = self.embedding_to_expression.forward(
-                    cell_gene_embedding, data.minibatch.genes_oi_torch
+                    cell_gene_embedding
                 )
             else:
                 n_fragments = total_n_fragments
                 expression_predicted = total_expression_predicted
 
             yield expression_predicted, n_fragments
 
-    def train_model(self, fragments, transcriptome, fold, device="cuda"):
+    def train_model(self, fragments, transcriptome, fold, device=default_device):
         # set up minibatchers and loaders
         minibatcher_train = Minibatcher(
             fold["cells_train"],
-            range(fragments.n_genes),
+            fold["genes_train"],
             n_genes_step=500,
-            n_cells_step=200,
+            n_cells_step=500,
+            permute_cells=True,
+            permute_genes=True,
         )
         minibatcher_validation = Minibatcher(
             fold["cells_validation"],
-            range(fragments.n_genes),
-            n_genes_step=10,
-            n_cells_step=10000,
+            fold["genes_validation"],
+            n_genes_step=500,
+            n_cells_step=500,
             permute_cells=False,
             permute_genes=False,
         )
 
         loaders_train = LoaderPool2(
             TranscriptomeFragments,
             dict(
@@ -346,44 +360,45 @@
                 transcriptome=transcriptome,
                 fragments=fragments,
                 cellxgene_batch_size=minibatcher_validation.cellxgene_batch_size,
             ),
             n_workers=5,
         )
 
-        trainer = Trainer(
+        trainer = Trainer2(
             self,
             loaders_train,
             loaders_validation,
             minibatcher_train,
             minibatcher_validation,
             SparseDenseAdam(
                 self.parameters_sparse(),
                 self.parameters_dense(),
-                lr=1e-2,
+                lr=1e-3,
                 weight_decay=1e-5,
             ),
             n_epochs=30,
             checkpoint_every_epoch=1,
             optimize_every_step=1,
             device=device,
         )
 
         trainer.train()
+        self.trace = trainer.trace
         # trainer.trace.plot()
 
     def get_prediction(
         self,
         fragments,
         transcriptome,
         cells=None,
         cell_ixs=None,
         genes=None,
         gene_ixs=None,
-        device="cuda",
+        device=default_device,
         return_raw=False,
     ):
         """
         Returns the prediction of a dataset
         """
         if cell_ixs is None:
             if cells is None:
@@ -418,37 +433,48 @@
                 fragments=fragments,
                 cellxgene_batch_size=minibatches.cellxgene_batch_size,
             ),
             n_workers=5,
         )
         loaders.initialize(minibatches)
 
-        predicted = np.zeros((len(cell_ixs), fragments.n_genes))
-        expected = np.zeros((len(cell_ixs), fragments.n_genes))
-        n_fragments = np.zeros((len(cell_ixs), fragments.n_genes))
+        predicted = np.zeros((len(cell_ixs), len(gene_ixs)))
+        expected = np.zeros((len(cell_ixs), len(gene_ixs)))
+        n_fragments = np.zeros((len(cell_ixs), len(gene_ixs)))
 
         cell_mapping = np.zeros(fragments.n_cells, dtype=np.int64)
         cell_mapping[cell_ixs] = np.arange(len(cell_ixs))
 
-        device = "cuda"
+        gene_mapping = np.zeros(fragments.n_genes, dtype=np.int64)
+        gene_mapping[gene_ixs] = np.arange(len(gene_ixs))
+
         self.eval()
         self = self.to(device)
 
         for data in loaders:
             data = data.to(device)
             with torch.no_grad():
                 pred_mb = self.forward(data)
             predicted[
-                np.ix_(cell_mapping[data.minibatch.cells_oi], data.minibatch.genes_oi)
+                np.ix_(
+                    cell_mapping[data.minibatch.cells_oi],
+                    gene_mapping[data.minibatch.genes_oi],
+                )
             ] = pred_mb.cpu().numpy()
             expected[
-                np.ix_(cell_mapping[data.minibatch.cells_oi], data.minibatch.genes_oi)
+                np.ix_(
+                    cell_mapping[data.minibatch.cells_oi],
+                    gene_mapping[data.minibatch.genes_oi],
+                )
             ] = data.transcriptome.value.cpu().numpy()
             n_fragments[
-                np.ix_(cell_mapping[data.minibatch.cells_oi], data.minibatch.genes_oi)
+                np.ix_(
+                    cell_mapping[data.minibatch.cells_oi],
+                    gene_mapping[data.minibatch.genes_oi],
+                )
             ] = (
                 torch.bincount(
                     data.fragments.local_cellxgene_ix,
                     minlength=len(data.minibatch.cells_oi)
                     * len(data.minibatch.genes_oi),
                 )
                 .reshape(len(data.minibatch.cells_oi), len(data.minibatch.genes_oi))
@@ -462,40 +488,40 @@
             return predicted, expected, n_fragments
 
         result = xr.Dataset(
             {
                 "predicted": xr.DataArray(
                     predicted,
                     dims=("cell", "gene"),
-                    coords={"cell": cells, "gene": fragments.var.index},
+                    coords={"cell": cells, "gene": genes},
                 ),
                 "expected": xr.DataArray(
                     expected,
                     dims=("cell", "gene"),
-                    coords={"cell": cells, "gene": fragments.var.index},
+                    coords={"cell": cells, "gene": genes},
                 ),
                 "n_fragments": xr.DataArray(
                     n_fragments,
                     dims=("cell", "gene"),
-                    coords={"cell": cells, "gene": fragments.var.index},
+                    coords={"cell": cells, "gene": genes},
                 ),
             }
         )
         return result
 
     def get_prediction_censored(
         self,
         fragments,
         transcriptome,
         censorer,
         cells=None,
         cell_ixs=None,
         genes=None,
         gene_ixs=None,
-        device="cuda",
+        device=default_device,
     ):
         """
         Returns the prediction of multiple censored dataset
         """
         if cell_ixs is None:
             if cells is None:
                 cells = fragments.obs.index
@@ -577,26 +603,24 @@
 
     @property
     def models_path(self):
         path = self.path / "models"
         path.mkdir(exist_ok=True)
         return path
 
-    def train_models(self, fragments, transcriptome, folds, device="cuda"):
+    def train_models(self, fragments, transcriptome, folds, device=default_device):
         self.n_models = len(folds)
         for fold_ix, fold in [(fold_ix, fold) for fold_ix, fold in enumerate(folds)]:
             desired_outputs = [self.models_path / ("model_" + str(fold_ix) + ".pkl")]
             force = False
             if not all([desired_output.exists() for desired_output in desired_outputs]):
                 force = True
 
             if force:
-                model = Model(
-                    n_genes=fragments.n_genes,
-                )
+                model = Model()
                 model.train_model(fragments, transcriptome, fold, device=device)
 
                 model = model.to("cpu")
 
                 pickle.dump(
                     model,
                     open(self.models_path / ("model_" + str(fold_ix) + ".pkl"), "wb"),
@@ -610,15 +634,15 @@
     def __len__(self):
         return self.n_models
 
     def __iter__(self):
         for ix in range(len(self)):
             yield self[ix]
 
-    def get_gene_cors(self, fragments, transcriptome, folds, device="cuda"):
+    def get_gene_cors(self, fragments, transcriptome, folds, device=default_device):
         cor_predicted = np.zeros((len(fragments.var.index), len(folds)))
         cor_n_fragments = np.zeros((len(fragments.var.index), len(folds)))
         n_fragments = np.zeros((len(fragments.var.index), len(folds)))
         for model_ix, (model, fold) in enumerate(zip(self, folds)):
             prediction = model.get_prediction(
                 fragments, transcriptome, cell_ixs=fold["cells_test"], device=device
             )
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/copredictivity.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/copredictivity.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/effect.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/effect.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/predictivity.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/plot/predictivity.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/trainer.py` & `chromatinhd-0.0.20/src/chromatinhd/models/pred/trainer/trainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import tqdm.auto as tqdm
-import torch
+import logging
+
 import numpy as np
-from chromatinhd.train import Trace
+import torch
+import tqdm.auto as tqdm
 
-import logging
+from chromatinhd import default_device
+from chromatinhd.train import Trace
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 
 def paircor(x, y, dim=0, eps=0.1):
     divisor = (y.std(dim) * x.std(dim)) + eps
@@ -33,15 +35,15 @@
         self,
         model,
         loaders_train,
         loaders_validation,
         minibatcher_train,
         minibatcher_validation,
         optim,
-        device="cuda",
+        device=default_device,
         n_epochs=30,
         checkpoint_every_epoch=1,
         optimize_every_step=10,
     ):
         self.model = model
         self.loaders_train = loaders_train
         self.loaders_validation = loaders_validation
@@ -126,14 +128,122 @@
 
             # train
             for data_train in self.loaders_train:
                 data_train = data_train.to(self.device)
 
                 loss = self.model.forward_loss(data_train)
                 loss.backward()
+
+                # check if optimization
+                if (self.step_ix % self.optimize_every_step) == 0:
+                    self.optim.step()
+                    self.optim.zero_grad()
+
+                self.step_ix += 1
+                pbar.update()
+
+                self.trace.append(loss.item(), self.epoch, self.step_ix, "train")
+            self.epoch += 1
+
+        pbar.update(n_steps_total)
+        pbar.close()
+
+        self.model = self.model.to("cpu")
+
+
+class Trainer2:
+    def __init__(
+        self,
+        model,
+        loaders_train,
+        loaders_validation,
+        minibatcher_train,
+        minibatcher_validation,
+        optim,
+        device=default_device,
+        n_epochs=30,
+        checkpoint_every_epoch=1,
+        optimize_every_step=10,
+    ):
+        self.model = model
+        self.loaders_train = loaders_train
+        self.loaders_validation = loaders_validation
+
+        self.trace = Trace()
+
+        self.optim = optim
+
+        self.step_ix = 0
+        self.epoch = 0
+        self.n_epochs = n_epochs
+
+        self.checkpoint_every_epoch = checkpoint_every_epoch
+        self.optimize_every_step = optimize_every_step
+
+        self.minibatcher_train = minibatcher_train
+        self.minibatcher_validation = minibatcher_validation
+
+        self.device = device
+
+    def train(self):
+        self.model = self.model.to(self.device)
+
+        prev_loss = None
+
+        self.loaders_train.initialize(self.minibatcher_train)
+        self.loaders_validation.initialize(self.minibatcher_validation)
+
+        n_steps_total = self.n_epochs * len(self.loaders_train)
+        pbar = tqdm.tqdm(total=n_steps_total, leave=False)
+
+        while self.epoch < self.n_epochs:
+            # checkpoint if necessary
+            if (self.epoch % self.checkpoint_every_epoch) == 0:
+                with torch.no_grad():
+                    losses = []
+                    for data_validation in self.loaders_validation:
+                        data_validation = data_validation.to(self.device)
+
+                        loss_mb = (
+                            (
+                                self.model.forward_loss(data_validation)
+                                .cpu()
+                                .detach()
+                                .numpy()
+                            )
+                            .mean()
+                            .item()
+                        )
+                        losses.append(loss_mb)
+                    loss = np.mean(losses)
+
+                self.trace.append(
+                    loss,
+                    self.epoch,
+                    self.step_ix,
+                    "validation",
+                )
+                logger.info(f"{'•'} {self.epoch}/{self.n_epochs} {'step':>15}")
+                self.trace.checkpoint(logger=logger)
+
+                if prev_loss is not None:
+                    improvement = loss - prev_loss
+                    print(improvement)
+                    logger.info(f"{improvement:.3f}")
+
+                    if improvement > 0.0:
+                        break
+                prev_loss = loss
+
+            # train
+            for data_train in self.loaders_train:
+                data_train = data_train.to(self.device)
+
+                loss = self.model.forward_loss(data_train)
+                loss.backward()
 
                 # check if optimization
                 if (self.step_ix % self.optimize_every_step) == 0:
                     self.optim.step()
                     self.optim.zero_grad()
 
                 self.step_ix += 1
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/optim.py` & `chromatinhd-0.0.20/src/chromatinhd/optim.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/plot/genome/genes.py` & `chromatinhd-0.0.20/src/chromatinhd/plot/genome/genes.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/plot/matshow45.py` & `chromatinhd-0.0.20/src/chromatinhd/plot/matshow45.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/plot/patch.py` & `chromatinhd-0.0.20/src/chromatinhd/plot/patch.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/plot/quasirandom.py` & `chromatinhd-0.0.20/src/chromatinhd/plot/quasirandom.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/plot/tickers.py` & `chromatinhd-0.0.20/src/chromatinhd/plot/tickers.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/sparse.py` & `chromatinhd-0.0.20/src/chromatinhd/sparse.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/train.py` & `chromatinhd-0.0.20/src/chromatinhd/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import tqdm.auto as tqdm
 import torch
 import pandas as pd
-from chromatinhd.utils.ansi import colorcodes
 
 
 class Trace:
     def __init__(self, n_significant_digits=3):
         self.train_steps = []
         self.validation_steps = []
         self.n_current_train_steps = 0
@@ -57,15 +56,15 @@
             current_loss = current_train_steps["loss"].mean()
             diff_loss = (
                 current_train_steps["loss"].mean() - last_train_steps["loss"].mean()
             )
             perc_diff_loss = diff_loss / current_loss
 
             logger.info(
-                f"{'train':>10} {current_loss:+.2f} Δ{colorcodes.color_sign(diff_loss, '{:+.3f}')} {perc_diff_loss:+.2%}"
+                f"{'train':>10} {current_loss:+.2f} Δ{diff_loss, '{:+.3f}'} {perc_diff_loss:+.2%}"
             )
         self.n_last_train_steps = self.n_current_train_steps
         self.n_current_train_steps = 0
 
         if len(self.validation_steps) > 0:
             current_validation_steps = pd.DataFrame(
                 self.validation_steps[-(self.n_current_validation_steps) :]
@@ -95,15 +94,15 @@
                     current_validation_steps["loss"].mean()
                     - last_validation_steps["loss"].mean()
                 )
                 self.last_validation_diff.append(diff_loss)
                 perc_diff_loss = diff_loss / current_loss
 
                 logger.info(
-                    f"{'validation':>10} {current_loss:+.2f} Δ{colorcodes.color_sign(diff_loss, '{:+.3f}')} {perc_diff_loss:+.2%}"
+                    f"{'validation':>10} {current_loss:+.2f} Δ{diff_loss, '{:+.3f}'} {perc_diff_loss:+.2%}"
                 )
             else:
                 logger.info(f"{'validation':>10} {current_loss:+.2f}")
             self.n_last_validation_steps = self.n_current_validation_steps
             self.n_current_validation_steps = 0
 
         self.current_checkpoint += 1
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/utils/__init__.py` & `chromatinhd-0.0.20/src/chromatinhd/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import os
 import pathlib
 import pickle
 import pandas as pd
 
 from .torch import interpolate_1d
 from .numpy import indices_to_indptr, indptr_to_indices
-from .ansi import colorcodes
 from .testing import repeated_kfold_corrected_t_test
 from . import ecdf
 
 __all__ = [
     "get_git_root",
     "get_output",
     "get_code",
     "name_window",
     "paircor",
     "interpolate_1d",
     "indices_to_indptr",
     "indptr_to_indices",
-    "colorcodes",
     "repeated_kfold_corrected_t_test",
     "ecdf",
 ]
 
 
 def get_git_root(cwd=None):
     """
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd/utils/ecdf.py` & `chromatinhd-0.0.20/src/chromatinhd/utils/ecdf.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/utils/testing.py` & `chromatinhd-0.0.20/src/chromatinhd/utils/testing.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd/utils/torch.py` & `chromatinhd-0.0.20/src/chromatinhd/utils/torch.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.19/src/chromatinhd.egg-info/PKG-INFO` & `chromatinhd-0.0.20/src/chromatinhd.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: chromatinhd
-Version: 0.0.19
+Version: 0.0.20
 Summary: High-definition modeling of (single-cell) chromatin + transcriptomics data
 Author-email: Wouter Saelens <wouter.saelens@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/DeplanckeLab/ChromatinHD
 Project-URL: Bug Tracker, https://github.com/DeplanckeLab/ChromatinHD/issues
 Keywords: bioinformatics,chromatin accessibility,transcriptomics
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE.md
 
 <p align="center">
-  <a href="https://deplanckelab.github.io/ChromatinHD/">
+  <a href="https://chromatinhd.eu">
     <img src="https://raw.githubusercontent.com/DeplanckeLab/ChromatinHD/main/docs/source/static/logo.png" width="300" />
   </a>
 </p>
 
-Documentation is available at https://deplanckelab.github.io/ChromatinHD/
+Documentation is available at <https://chromatinhd.eu>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.19 Summary: High-
+Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.20 Summary: High-
 definition modeling of (single-cell) chromatin + transcriptomics data Author-
 email: Wouter Saelens
 saelens@gmail.com> License: MIT Project-URL: Homepage, https://github.com/
 DeplanckeLab/ChromatinHD Project-URL: Bug Tracker, https://github.com/
 DeplanckeLab/ChromatinHD/issues Keywords: bioinformatics,chromatin
 accessibility,transcriptomics Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE.md
+dev Provides-Extra: test License-File: LICENSE.md
  [https://raw.githubusercontent.com/DeplanckeLab/ChromatinHD/main/docs/source/
                                static/logo.png]
-Documentation is available at https://deplanckelab.github.io/ChromatinHD/
+Documentation is available at
+chromatinhd.eu>
```

### Comparing `chromatinhd-0.0.19/src/chromatinhd.egg-info/SOURCES.txt` & `chromatinhd-0.0.20/src/chromatinhd.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE.md
 README.md
 mkdocs.yml
 pyproject.toml
+setup.py
 .github/workflows/ci.yml
 docs/override/main.html
 docs/source/index.md
 docs/source/index.py
 docs/source/jupytext.toml
+docs/source/javascripts/reference.js
 docs/source/quickstart/0_install.py
 docs/source/quickstart/1_data.py
 docs/source/quickstart/2_pred.py
 docs/source/quickstart/3_diff.py
 docs/source/reference/index.md
 docs/source/reference/data/clustering.md
+docs/source/reference/data/folds.md
 docs/source/reference/data/fragments.md
+docs/source/reference/data/motifscan.md
 docs/source/reference/data/regions.md
 docs/source/reference/data/transcriptome.md
+docs/source/reference/models/diff/interpret.md
+docs/source/reference/models/pred/interpret.md
+docs/source/reference/models/pred/model.md
 docs/source/reference/models/pred/plot.md
 docs/source/static/favicon.ai
 docs/source/static/favicon.png
 docs/source/static/logo.ai
 docs/source/static/logo.png
 docs/source/static/models/diff/logo.pdf
 docs/source/static/models/diff/1x/logo.png
@@ -29,22 +36,23 @@
 docs/source/static/models/dime/logo.png
 docs/source/static/models/pred/logo.pdf
 docs/source/static/models/pred/1x/logo.png
 docs/source/static/models/time/logo.pdf
 docs/source/static/models/time/logo.png
 docs/source/stylesheets/extra-reference.css
 docs/source/stylesheets/extra.css
-scripts/build.sh
+scripts/cythonize.sh
+scripts/dist.sh
+scripts/install.sh
 scripts/setup_data_tiny.py
 scripts/test.py
 src/chromatinhd/__init__.py
 src/chromatinhd/device.py
 src/chromatinhd/embedding.py
 src/chromatinhd/flow.py
-src/chromatinhd/loss.py
 src/chromatinhd/optim.py
 src/chromatinhd/sparse.py
 src/chromatinhd/train.py
 src/chromatinhd.egg-info/PKG-INFO
 src/chromatinhd.egg-info/SOURCES.txt
 src/chromatinhd.egg-info/dependency_links.txt
 src/chromatinhd.egg-info/requires.txt
@@ -63,14 +71,15 @@
 src/chromatinhd/data/folds/__init__.py
 src/chromatinhd/data/folds/folds.py
 src/chromatinhd/data/fragments/__init__.py
 src/chromatinhd/data/fragments/fragments.py
 src/chromatinhd/data/genotype/__init__.py
 src/chromatinhd/data/genotype/genotype.py
 src/chromatinhd/data/motifscan/__init__.py
+src/chromatinhd/data/motifscan/gwas.py
 src/chromatinhd/data/motifscan/motifscan.py
 src/chromatinhd/data/motifscan/motiftrack.py
 src/chromatinhd/data/peakcounts/__init__.py
 src/chromatinhd/data/peakcounts/peakcounts.py
 src/chromatinhd/data/transcriptome/__init__.py
 src/chromatinhd/data/transcriptome/transcriptome.py
 src/chromatinhd/grid/__init__.py
@@ -93,14 +102,15 @@
 src/chromatinhd/models/diff/enrichment/enrichment.py
 src/chromatinhd/models/diff/interpret/__init__.py
 src/chromatinhd/models/diff/interpret/genepositional.py
 src/chromatinhd/models/diff/loader/__init__.py
 src/chromatinhd/models/diff/loader/clustering.py
 src/chromatinhd/models/diff/loader/clustering_cuts.py
 src/chromatinhd/models/diff/loader/cuts.py
+src/chromatinhd/models/diff/loader/fragments_helpers.c
 src/chromatinhd/models/diff/loader/fragments_helpers.pyx
 src/chromatinhd/models/diff/loader/minibatches.py
 src/chromatinhd/models/diff/model/__init__.py
 src/chromatinhd/models/diff/model/cutnf.py
 src/chromatinhd/models/diff/model/spline.py
 src/chromatinhd/models/diff/model/splines/__init__.py
 src/chromatinhd/models/diff/model/splines/cubic.py
@@ -115,14 +125,15 @@
 src/chromatinhd/models/pred/interpret/__init__.py
 src/chromatinhd/models/pred/interpret/censorers.py
 src/chromatinhd/models/pred/interpret/filter.py
 src/chromatinhd/models/pred/interpret/genemultiwindow.py
 src/chromatinhd/models/pred/interpret/genepairwindow.py
 src/chromatinhd/models/pred/loader/__init__.py
 src/chromatinhd/models/pred/loader/fragments.py
+src/chromatinhd/models/pred/loader/fragments_helpers.c
 src/chromatinhd/models/pred/loader/fragments_helpers.pyx
 src/chromatinhd/models/pred/loader/minibatches.py
 src/chromatinhd/models/pred/loader/transcriptome.py
 src/chromatinhd/models/pred/loader/transcriptome_fragments.py
 src/chromatinhd/models/pred/model/__init__.py
 src/chromatinhd/models/pred/model/across.py
 src/chromatinhd/models/pred/model/additive.py
@@ -137,20 +148,19 @@
 src/chromatinhd/plot/matshow45.py
 src/chromatinhd/plot/patch.py
 src/chromatinhd/plot/quasirandom.py
 src/chromatinhd/plot/tickers.py
 src/chromatinhd/plot/genome/__init__.py
 src/chromatinhd/plot/genome/genes.py
 src/chromatinhd/utils/__init__.py
-src/chromatinhd/utils/ansi.py
 src/chromatinhd/utils/ecdf.py
 src/chromatinhd/utils/numpy.py
 src/chromatinhd/utils/testing.py
 src/chromatinhd/utils/torch.py
 tests/conftest.py
-tests/test_loss.py
 tests/biomart/conftest.py
 tests/biomart/tss_test.py
+tests/data/motifscan/test_motifscan.py
 tests/models/diff/loader/test_clustering_cuts.py
 tests/models/diff/model/test_cutnf.py
 tests/models/pred/loader/test_transcriptome_fragments.py
 tests/models/pred/model/test_additive.py
```

### Comparing `chromatinhd-0.0.19/tests/conftest.py` & `chromatinhd-0.0.20/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,7 +61,14 @@
         example_dataset_folder / "fragments.tsv.gz",
         example_regions,
         obs=example_transcriptome.obs,
         path=example_dataset_folder / "fragments",
     )
     fragments.create_cellxgene_indptr()
     return fragments
+
+
+@pytest.fixture(scope="session")
+def example_folds(example_dataset_folder, example_fragments):
+    folds = chd.data.folds.Folds(example_dataset_folder / "random_5fold")
+    folds.sample_cells(example_fragments, n_folds=5, n_repeats=1)
+    return folds
```

### Comparing `chromatinhd-0.0.19/tests/models/pred/loader/test_transcriptome_fragments.py` & `chromatinhd-0.0.20/tests/models/pred/loader/test_transcriptome_fragments.py`

 * *Files identical despite different names*

