# Comparing `tmp/hf-deepali-0.4.2.tar.gz` & `tmp/hf-deepali-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf-deepali-0.4.2.tar", last modified: Fri Jul 28 13:34:00 2023, max compression
+gzip compressed data, was "hf-deepali-0.4.3.tar", last modified: Fri Aug  4 16:38:38 2023, max compression
```

## Comparing `hf-deepali-0.4.2.tar` & `hf-deepali-0.4.3.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.853740 hf-deepali-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.857740 hf-deepali-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.861740 hf-deepali-0.4.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.861740 hf-deepali-0.4.2/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   550833 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.conda-lock.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.devenv.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53576 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.linux-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    45592 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.osx-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    48151 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.win-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/conda/environment.win-64.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.861740 hf-deepali-0.4.2/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docker/build
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docker/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/basics/example-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/basics/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.853740 hf-deepali-0.4.2/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/domain.md
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/flow.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/image.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/core/kernels.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/data/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/sampler.md
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/data/transforms.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/losses/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/modules/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.865740 hf-deepali-0.4.2/docs/reference/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/networks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/docs/reference/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/common.md
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/composite.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/spatial/transformer.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/docs/reference/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/reference/utils/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/example-myst-notebook.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/example-notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45126 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/docs/tutorials/pairwise-registration-intro.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.869741 hf-deepali-0.4.2/examples/ffd/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/ffd/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.873741 hf-deepali-0.4.2/examples/istn/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.873741 hf-deepali-0.4.2/examples/istn/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/models/itn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/models/stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/examples/istn/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.857740 hf-deepali-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.857740 hf-deepali-0.4.2/src/deepali/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.877741 hf-deepali-0.4.2/src/deepali/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/_kornia.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    79771 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/nnutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/psutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/tempfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/core/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/data/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/transforms/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/data/transforms/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    68167 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/losses/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.881741 hf-deepali-0.4.2/src/deepali/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/modules/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.885742 hf-deepali-0.4.2/src/deepali/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.885742 hf-deepali-0.4.2/src/deepali/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/blocks/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/blocks/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.885742 hf-deepali-0.4.2/src/deepali/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/acti.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/nonrigid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/spatial/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/aws/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.889742 hf-deepali-0.4.2/src/deepali/utils/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/average_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/multilabel_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/output_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ignite/score_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/imageio/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/imageio/sitk.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/ipython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/simpleitk/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/imageio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/simpleitk/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/deepali/utils/vtk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/polydataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/src/deepali/utils/vtk/simpleitk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.893742 hf-deepali-0.4.2/src/hf_deepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 13:34:00.000000 hf-deepali-0.4.2/src/hf_deepali.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:00.897742 hf-deepali-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/_test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_image_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_core_tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_data_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_data_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_network_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_spatial_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-28 13:33:37.000000 hf-deepali-0.4.2/tests/test_utils_imageio_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.643792 hf-deepali-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.591791 hf-deepali-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.595791 hf-deepali-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.595791 hf-deepali-0.4.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-08-04 16:38:38.643792 hf-deepali-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   619294 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.conda-lock.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.devenv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    59741 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.linux-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    51617 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    15299 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.osx-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    54530 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/conda/environment.win-64.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docker/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docker/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/_citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/_images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/basics/example-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/basics/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.591791 hf-deepali-0.4.3/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/docs/reference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/core/domain.md
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/core/flow.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/core/image.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/core/kernels.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/docs/reference/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/data/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/data/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/data/sampler.md
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/data/tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/data/transforms.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.599791 hf-deepali-0.4.3/docs/reference/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/losses/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/docs/reference/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/modules/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/docs/reference/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/networks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/docs/reference/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/spatial/common.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/spatial/composite.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/spatial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/spatial/transformer.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/reference/utils/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/tutorials/example-myst-notebook.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/tutorials/example-notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45126 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/docs/tutorials/pairwise-registration-intro.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/examples/ffd/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/ffd/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.603791 hf-deepali-0.4.3/examples/istn/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.607791 hf-deepali-0.4.3/examples/istn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/models/itn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/models/stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/examples/istn/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:38:38.643792 hf-deepali-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.595791 hf-deepali-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.591791 hf-deepali-0.4.3/src/deepali/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.615791 hf-deepali-0.4.3/src/deepali/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/_kornia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79771 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/nnutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/core/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.615791 hf-deepali-0.4.3/src/deepali/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.619792 hf-deepali-0.4.3/src/deepali/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/transforms/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/data/transforms/item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.619792 hf-deepali-0.4.3/src/deepali/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68167 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/losses/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.623792 hf-deepali-0.4.3/src/deepali/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/modules/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.623792 hf-deepali-0.4.3/src/deepali/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.623792 hf-deepali-0.4.3/src/deepali/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/blocks/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/blocks/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.627792 hf-deepali-0.4.3/src/deepali/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/acti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.631792 hf-deepali-0.4.3/src/deepali/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29833 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/nonrigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/spatial/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.631792 hf-deepali-0.4.3/src/deepali/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.631792 hf-deepali-0.4.3/src/deepali/utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.631792 hf-deepali-0.4.3/src/deepali/utils/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/aws/s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/aws/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/aws/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.631792 hf-deepali-0.4.3/src/deepali/utils/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.635792 hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/average_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/multilabel_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/output_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ignite/score_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.635792 hf-deepali-0.4.3/src/deepali/utils/imageio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/imageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/imageio/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/imageio/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/imageio/sitk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.635792 hf-deepali-0.4.3/src/deepali/utils/simpleitk/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/simpleitk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/simpleitk/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/simpleitk/imageio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/simpleitk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/simpleitk/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/simpleitk/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.639792 hf-deepali-0.4.3/src/deepali/utils/vtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/vtk/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/vtk/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/vtk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/vtk/polydataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/src/deepali/utils/vtk/simpleitk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.639792 hf-deepali-0.4.3/src/hf_deepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-08-04 16:38:38.000000 hf-deepali-0.4.3/src/hf_deepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-04 16:38:38.000000 hf-deepali-0.4.3/src/hf_deepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:38:38.000000 hf-deepali-0.4.3/src/hf_deepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-04 16:38:38.000000 hf-deepali-0.4.3/src/hf_deepali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 16:38:38.000000 hf-deepali-0.4.3/src/hf_deepali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:38.643792 hf-deepali-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/_test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_core_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_core_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_core_image_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_core_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_core_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_core_tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_data_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_data_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_network_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_network_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_network_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_network_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_spatial_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-08-04 16:38:22.000000 hf-deepali-0.4.3/tests/test_utils_imageio_meta.py
```

### Comparing `hf-deepali-0.4.2/.github/workflows/docs.yml` & `hf-deepali-0.4.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/.github/workflows/release.yml` & `hf-deepali-0.4.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/.github/workflows/tests.yml` & `hf-deepali-0.4.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/.gitignore` & `hf-deepali-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/.vscode/extensions.json` & `hf-deepali-0.4.3/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/.vscode/launch.json` & `hf-deepali-0.4.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/.vscode/settings.json` & `hf-deepali-0.4.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/CITATION.cff` & `hf-deepali-0.4.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/CODE_OF_CONDUCT.md` & `hf-deepali-0.4.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/LICENSE` & `hf-deepali-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/PKG-INFO` & `hf-deepali-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.4.2
+Version: 0.4.3
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
```

### Comparing `hf-deepali-0.4.2/README.md` & `hf-deepali-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/TODO` & `hf-deepali-0.4.3/TODO`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/conda/Makefile` & `hf-deepali-0.4.3/conda/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 # Default name of conda environment
 NAME = deepali
 
 # Relative path of repository root directory
 ROOT = ..
 
-# Commands
-CONDA = mamba
-CONDA_OPTS = --no-banner
-CONDA_DEVENV = conda devenv
-CONDA_LOCK = conda-lock
-CONDA_LOCK_OPTS = --mamba
-
 # Name of conda-devenv configuration file
 DEVENV = environment.devenv.yml
 
 # Name of conda-lock output file
 LOCKFILE = environment.conda-lock.yml
 
 # Detect operating system
@@ -62,36 +55,36 @@
 win: clear lock-win render
 
 clear:
 	@echo "Remove all generated files"
 	@rm -f $(LOCKFILE) environment.devenv.{linux-64,osx-64,win-64}.yml environment.{linux-64,osx-64,win-64}.{lock,yml}
 
 lock-linux:
-	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=linux-64 --print > environment.devenv.linux-64.yml
-	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform linux-64 --file environment.devenv.linux-64.yml
+	conda devenv --name $(NAME) --file $(DEVENV) --env-manager conda --env-var PLATFORM=linux-64 --print > environment.devenv.linux-64.yml
+	conda lock --lockfile $(LOCKFILE) --platform linux-64 --file environment.devenv.linux-64.yml
 
 lock-osx:
-	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=osx-64 --print > environment.devenv.osx-64.yml
-	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform osx-64 --file environment.devenv.osx-64.yml
+	conda devenv --name $(NAME) --file $(DEVENV) --env-manager conda --env-var PLATFORM=osx-64 --print > environment.devenv.osx-64.yml
+	conda lock --lockfile $(LOCKFILE) --platform osx-64 --file environment.devenv.osx-64.yml
 
 lock-win:
-	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=win-64 --print > environment.devenv.win-64.yml
-	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform win-64 --file environment.devenv.win-64.yml
+	conda devenv --name $(NAME) --file $(DEVENV) --env-manager conda --env-var PLATFORM=win-64 --print > environment.devenv.win-64.yml
+	conda lock --lockfile $(LOCKFILE) --platform win-64 --file environment.devenv.win-64.yml
 
 render:
-	@$(CONDA_LOCK) render $(LOCKFILE) --kind env --filename-template environment.{platform}
-	@$(CONDA_LOCK) render $(LOCKFILE) --kind explicit --filename-template environment.{platform}.lock
+	conda lock render $(LOCKFILE) --kind env --filename-template environment.{platform}
+	conda lock render $(LOCKFILE) --kind explicit --filename-template environment.{platform}.lock
 	@if ! grep -e 'pytorch.*cuda' environment.linux-64.lock > /dev/null 2> /dev/null; then \
 		echo "Expected PyTorch with CUDA support for PLATFORM=linux-64. Check conda configuration."; \
 	fi
 
 
 env: create-env install
 
 create-env:
-	@$(CONDA) $(CONDA_OPTS) create --name $(NAME) --file environment.$(PLATFORM).lock
+	conda create --name $(NAME) --file environment.$(PLATFORM).lock
 
 update-env:
-	@$(CONDA) $(CONDA_OPTS) update --name $(NAME) --file environment.$(PLATFORM).lock --prune
+	conda update --name $(NAME) --file environment.$(PLATFORM).lock --prune
 
 install:
-	@$(CONDA) $(CONDA_OPTS) run --name $(NAME) pip install $(PIP_INSTALL_OPTS) ./$(ROOT)[utils]
+	conda run --name $(NAME) pip install $(PIP_INSTALL_OPTS) ./$(ROOT)[utils]
```

### Comparing `hf-deepali-0.4.2/conda/README.md` & `hf-deepali-0.4.3/conda/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Conda configuration
 
 Conda environment configurations for `deepali` libraries.
 
 
 ## Create environment
 
-If not done before, install either [Miniconda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda](https://www.anaconda.com/).
+If not done before, install either [Anaconda], [Miniconda], or [Mambaforge].
 
 A conda environment for this project can be created using the `env` Makefile target, i.e.,
 
 ```
 make env [NAME=deepali] [EDITABLE=1]
 ```
 
@@ -18,15 +18,15 @@
 Alternatively, run the following `conda` commands intead of using `make`:
 
 ```
 NAME=deepali
 PLATFORM=linux-64
 
 conda create --name $NAME --file environment.$PLATFORM.lock
-conda run --name $NAME pip install [--editable] ..
+conda run --name $NAME pip install ..[utils]
 ```
 
 where `PLATFORM` is one of the following values.
 
 | **Platform**  | **Description**                             |
 | ------------- | ------------------------------------------- |
 | `linux-64`    | 64-bit Linux distribution (e.g., CentOS 7). |
@@ -34,20 +34,25 @@
 | `win-64`      | 64-bit Microsoft Windows with CUDA device.  |
 
 
 ## Manage dependencies
 
 The following tools are required to update the generated dependency files.
 
-1. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html): Package dependency management tool.
-2. Install [mamba](https://mamba.readthedocs.io/en/latest/): Faster dependency resolution and more informative error messages.
-   - `conda install mamba=0.23 --name base --channel conda-forge`
-3. Install [conda-devenv](https://conda-devenv.readthedocs.io/en/latest/): Advanced conda environment configuration such as conditional dependencies.
-   - `conda install conda-devenv=2.3 --name base --channel conda-forge`
-4. Install [conda-lock](https://conda-incubator.github.io/conda-lock/): Lock versions of dependencies and generate explicit lockfiles.
-   - `conda install conda-lock=1.0 --name base --channel conda-forge`
+1. Install [Mambaforge]: Package dependency management tool.
+3. Install [conda-devenv]: Advanced conda environment configuration such as conditional dependencies.
+   - `mamba --no-banner install conda-devenv=2.3 --name base --channel conda-forge`
+4. Install [conda-lock]: Lock versions of dependencies and generate explicit lockfiles.
+   - `mamba --no-banner install conda-lock=1.0 --name base --channel conda-forge`
 
 After editing the `environment.devenv.yml` file to add, remove, or update required and optional dependencies, run the following command to re-generate the `environment.conda-lock.yml` and `environment.*.lock` files.
 
 ```
 make all
 ```
+
+
+[Anaconda]: https://www.anaconda.com/
+[Mambaforge]: https://mamba.readthedocs.io/en/latest/installation.html
+[Miniconda]: https://docs.conda.io/en/latest/miniconda.html
+[conda-devenv]: https://conda-devenv.readthedocs.io/en/latest/
+[conda-lock]: https://conda-incubator.github.io/conda-lock/
```

### Comparing `hf-deepali-0.4.2/conda/environment.conda-lock.yml` & `hf-deepali-0.4.3/conda/environment.conda-lock.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
   - url: pytorch
     used_env_vars: []
   - url: nvidia
     used_env_vars: []
   - url: nodefaults
     used_env_vars: []
   content_hash:
-    linux-64: c6bd68ba63788a00937c8cd1d91bb1e5813d242d7089005156ab1a663f53aee1
-    osx-64: 533a7567b393584157366e71374225596e814fe74cfcb03642d3b4e184d58c87
-    win-64: 6255d416b6866feefaa84cbaf27b3a7608f8bb60e8d5e51ca00574e0f3970f20
+    linux-64: 586016f05a089668afa3f0a057304e5826b41e87317e8d51969529896659d6a0
+    osx-64: 1e6e6cea02ff8fd576a8852899876561e48ebb709abcd877d8d931d3b50338da
+    win-64: f9e524a368611b4591c0b79cc851d7fd034bcb935240ad118e3fe4c7b27edeb4
   platforms:
   - linux-64
   - osx-64
   - win-64
   sources:
   - environment.devenv.linux-64.yml
   - environment.devenv.osx-64.yml
@@ -43,22 +43,22 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
   version: '0.1'
 - category: main
   dependencies: {}
   hash:
-    md5: f5c65075fc34438d5b456c7f3f5ab695
-    sha256: 0cf1bb3d0bfc5519b60af2c360fa4888fb838e1476b1e0f65b9dbc48b45c7345
+    md5: a73ecd2988327ad4c8f2c331482917f2
+    sha256: 525b7b6b5135b952ec1808de84e5eca57c7c7ff144e29ef3e96ae4040ff432c1
   manager: conda
   name: ca-certificates
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda
-  version: 2023.5.7
+  url: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.7.22-hbcca054_0.conda
+  version: 2023.7.22
 - category: main
   dependencies: {}
   hash:
     md5: b68c7ef3eda01e95d5903fb508c5e440
     sha256: f8cf96ae45acf1bef5ff0be3e849d87e3543144ec8c0075db235f4933113a3b0
   manager: conda
   name: cuda-cudart
@@ -459,22 +459,22 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/double-conversion-3.2.0-h27087fc_1.tar.bz2
   version: 3.2.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
   hash:
-    md5: c2acfc9bc0d0c53f83bbf0f582cb0e7a
-    sha256: 1dfe42f82ccd06ca4b19cfbbef483385f284be90f6b40c26831004b192c98bda
+    md5: b1b879d6d093f55dd40d58b5eb2f0699
+    sha256: 53b15a98aadbe0704479bacaf7a5618fcb32d1577be320630674574241639b34
   manager: conda
   name: eigen
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.1-h00ab1b0_0.conda
-  version: 3.4.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.0-h00ab1b0_0.conda
+  version: 3.4.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libgfortran-ng: ''
     libgfortran5: '>=11.4.0'
     libstdcxx-ng: '>=12'
   hash:
@@ -1011,22 +1011,22 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/openh264-2.3.1-hcb278e6_2.conda
   version: 2.3.1
 - category: main
   dependencies:
     ca-certificates: ''
     libgcc-ng: '>=12'
   hash:
-    md5: 2e1d7b458ac8f1e3ca4e18b77add6277
-    sha256: 407d655643389bdb49266842a816815c981ae98f3513a6a2059b908b3abb380a
+    md5: e5ac5227582d6c83ccf247288c0eb095
+    sha256: b113fbac327c90cdc29c2fac0f2a2e5cc0d1918b2a5ffa7abd49b695b9b3c6e9
   manager: conda
   name: openssl
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda
-  version: 3.1.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.2-hd590300_0.conda
+  version: 3.1.2
 - category: main
   dependencies:
     libgcc-ng: '>=7.5.0'
   hash:
     md5: 660e72c82f2e75a6b3fe6a6e75c79f19
     sha256: 6a0630fff84b5a683af6185a6c67adc8bdfa2043047fcb251add0d352ef60e79
   manager: conda
@@ -2157,14 +2157,26 @@
   name: alabaster
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda
   version: 0.7.13
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: 5f095bc6454094e96f146491fd03633b
+    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
+  manager: conda
+  name: appdirs
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
+  version: 1.4.4
+- category: main
+  dependencies:
     libgcc-ng: '>=12'
     libglib: '>=2.74.1,<3.0a0'
     libstdcxx-ng: '>=12'
   hash:
     md5: 6c72ec3e660a51736913ef6ea68c454b
     sha256: 2f9314de13c1f0b54510a2afa0cdc02c0e3f828fccfc4277734f9590b11a65f1
   manager: conda
@@ -2219,14 +2231,26 @@
   name: blinker
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda
   version: 1.6.2
 - category: main
   dependencies:
+    python: 2.7.*|>=3.7
+  hash:
+    md5: 033eb25fffd222aceeca6d58cd953680
+    sha256: 4ff828cceb8f55cb26d23b1a4c174d22c7cd92350221724bcaf2d6632e33fdee
+  manager: conda
+  name: boltons
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/boltons-23.0.0-pyhd8ed1ab_0.conda
+  version: 23.0.0
+- category: main
+  dependencies:
     brotli-bin: 1.0.9 h166bdaf_9
     libbrotlidec: 1.0.9 h166bdaf_9
     libbrotlienc: 1.0.9 h166bdaf_9
     libgcc-ng: '>=12'
   hash:
     md5: 4601544b4982ba1861fa9b9c607b2c06
     sha256: 2357d205931912def55df0dc53573361156b27856f9bf359d464da162812ec1f
@@ -2234,36 +2258,48 @@
   name: brotli
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda
   version: 1.0.9
 - category: main
   dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 576d629e47797577ab0f1b351297ef4a
+    sha256: 6dbf7a5070cc43d90a1e4c2ec0c541c69d8e30a0e25f50ce9f6e4a432e42c5d7
+  manager: conda
+  name: cached_property
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 60b5eb16d9a7a5482ba37f67aa49db5b
     sha256: 8d30a41a88900730c748f5b296730a0d48e5cfa2c8b260aab60fa9f26ffafcc0
   manager: conda
   name: cachetools
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda
   version: 5.3.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 5d1b71c942b8421285934dad1d891ebc
-    sha256: f839a6e04d94069f90dd85337ea9108f058dc76771bb469a413f32bb1ba0b256
+    md5: 7f3dbc9179b4dde7da98dfb151d0ad22
+    sha256: db66e31866ff4250c190788769e3a8a1709237c3e9c38d7143aae95ab75fcb31
   manager: conda
   name: certifi
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda
-  version: 2023.5.7
+  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.7.22-pyhd8ed1ab_0.conda
+  version: 2023.7.22
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 313516e9a4b08b12dfb1e1cd390a96e3
     sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   manager: conda
@@ -2295,14 +2331,26 @@
   name: colorama
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
   version: 0.4.6
 - category: main
   dependencies:
+    python: '>=3.6,<4.0'
+  hash:
+    md5: 709a2295dd907bb34afb57d54320642f
+    sha256: 2f05954a3faf0700c14c1deddc085385160ee32abe111699c78d9cb277e915cc
+  manager: conda
+  name: crashtest
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.4.1
+- category: main
+  dependencies:
     python: '>=3.6'
   hash:
     md5: a50559fad0affdbb33729a68669ca1cb
     sha256: 3b594bc8aa0b9a51269d54c7a4ef6af777d7fad4bee16b05695e1124de6563f6
   manager: conda
   name: cycler
   optional: false
@@ -2338,22 +2386,22 @@
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 8ffb020d2b722c962f0b4f06a304f533
-    sha256: 4e476f11daa93d7740eaa8b13238db48c8c9e416d127bb1cda30300b63a26b52
+    md5: 397d3d6153c0b8de807e1bdc58b16013
+    sha256: da916d36136e7e756964d7e9d68ab6f1012f3d0f6fe0a57783863a4bf66819f4
   manager: conda
   name: debugpy
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py310heca2aa9_0.conda
-  version: 1.6.7
+  url: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.8-py310hc6cd4ac_0.conda
+  version: 1.6.8
 - category: main
   dependencies:
     python: '>=3.5'
   hash:
     md5: 43afe5ab04e35e17ba28649471dd7364
     sha256: 328a6a379f9bdfd0230e51de291ce858e6479411ea4b0545fb377c71662ef3e2
   manager: conda
@@ -2372,14 +2420,26 @@
   name: defusedxml
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2
   version: 0.7.1
 - category: main
   dependencies:
+    python: 2.7|>=3.6
+  hash:
+    md5: 12d8aae6994f342618443a8f05c652a0
+    sha256: 13c887cb4a29e1e853a118cfc0e42b72a7e1d1c50c66c0974885d37f0db30619
+  manager: conda
+  name: distlib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda
+  version: 0.3.7
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 785160da087cf1d70e989afbb761f01c
     sha256: 805631ed866cdbbb6bbe90f7cd397ada1c76494a1ba97b6093a8ce121c208c71
   manager: conda
   name: docutils
@@ -2633,24 +2693,48 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2
   version: 0.2.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
+    md5: 9800ad1699b42612478755a2d26c722d
+    sha256: 16639759b811866d63315fe1391f6fb45f5478b823972f4d3d9f0392b7dd80b8
+  manager: conda
+  name: jeepney
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.8.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
     md5: 2cfa3e1cf3fb51bb9b17acc5b5e9ea11
     sha256: 95ac5f9ee95fd4e34dc051746fc86016d3d4f6abefed113e2ede049d59ec2991
   manager: conda
   name: jmespath
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2
   version: 1.0.1
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: 07d85c22a3beb102a48cd123df84c2a6
+    sha256: da279af2285d8f575a7f5652e83bf7f36155c4c63154e385a9d171efcc607bc1
+  manager: conda
+  name: jsonpointer
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonpointer-2.0-py_0.tar.bz2
+  version: '2.0'
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 2bc3ca2f7387af385dd06706b4fb2d35
     sha256: 0781ed7a4f35ff1309e95381c40c8d8f96263ca4260a72baaafda87c975a972a
   manager: conda
   name: jupyterlab_widgets
   optional: false
@@ -2703,21 +2787,21 @@
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libllvm15: '>=15.0.7,<15.1.0a0'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 907344cee64101d44d806bbe0fccb01d
-    sha256: d9f9fb5622489d7e5c3237a4a6a46db20ead3c6bafb7277de1a25278db59b863
+    md5: 1720df000b48e31842500323cb7be18c
+    sha256: df1221a9a05b9bb3bd9b43c08a7e2fe57a0e15a0010ef26065f7ed7666083f45
   manager: conda
   name: libclang13
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libclang13-15.0.7-default_h9986a30_2.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libclang13-15.0.7-default_h9986a30_3.conda
   version: 15.0.7
 - category: main
   dependencies:
     krb5: '>=1.20.1,<1.21.0a0'
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
@@ -2796,14 +2880,26 @@
   name: libwebp
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.2.4-h522a892_0.tar.bz2
   version: 1.2.4
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: c104d98e09c47519950cffb8dd5b4f10
+    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
+  manager: conda
+  name: lockfile
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
+  version: 0.12.2
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 9e0d689557f3fdcb521c1239c13d29ec
     sha256: 287c1968e9d5b5b25adb43f9a72a8b249ef5c80fc35fd6e182fdd04d9366ab8b
   manager: conda
   name: loguru
@@ -2859,27 +2955,54 @@
   name: mistune
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda
   version: 3.0.0
 - category: main
   dependencies:
+    python: '>=3.8'
+  hash:
+    md5: 8549fafed0351bbfaa1ddaa15fdf9b4e
+    sha256: 07ce65497dec537e490992758934ddbc4fb5ed9285b41387a7cca966f1a98a0f
+  manager: conda
+  name: more-itertools
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.1.0-pyhd8ed1ab_0.conda
+  version: 10.1.0
+- category: main
+  dependencies:
     python: '>=3.6'
   hash:
     md5: dbf6e2d89137da32fa6670f3bffc024e
     sha256: a4f025c712ec1502a55c471b56a640eaeebfce38dd497d5a1a33729014cac47a
   manager: conda
   name: mpmath
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda
   version: 1.3.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 5311a49aaea44b73935c84a6d9a68e5f
+    sha256: da5030f22f6d1293ccdefefde17fcf1a5f337f87179c54dee2a2a1fc16d6d73a
+  manager: conda
+  name: msgpack-python
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py310hdf3cbec_0.conda
+  version: 1.0.5
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: b33287be963a70f8fb4b143b4561ba62
     sha256: 14312ac727a741224d45ab07f75253ca99235ec0534ba9603e627818666ff49a
   manager: conda
   name: multidict
@@ -2987,22 +3110,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2
   version: 0.8.3
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: dbb80d1e8dc2dba5c8b106dc0768ad45
-    sha256: d94463e0a140ead5c01990b565a1a21b85cb3831d56fed5955b5446bd5df33fe
+    md5: e41debb259e68490e3ab81e46b639ab6
+    sha256: 7bcfa6d86359d45572ba9ccaeaedc04b0452e2654fe44b6fe378d0d37b8745e1
   manager: conda
   name: pathspec
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda
-  version: 0.11.1
+  url: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.2-pyhd8ed1ab_0.conda
+  version: 0.11.2
 - category: main
   dependencies:
     python: '>=3'
   hash:
     md5: 415f0ebb6198cc2801c73438a9fb5761
     sha256: a1ed1a094dd0d1b94a09ed85c283a0eb28943f2e6f22161fb45e128d35229738
   manager: conda
@@ -3011,14 +3134,26 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
   version: 0.7.5
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
+    md5: be1e9f1c65a1ed0f2ae9352fec99db64
+    sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
+  manager: conda
+  name: pkginfo
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
+  version: 1.9.6
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
     md5: 89e3c7cdde7d3aaa2aee933b604dd07f
     sha256: 7d055ffc8a02bf781a89d069db3454b453605cdaff300b82cedcc7133283e47e
   manager: conda
   name: pkgutil-resolve-name
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2
@@ -3119,14 +3254,28 @@
   name: pycodestyle
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda
   version: 2.10.0
 - category: main
   dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 0e565d732f6660374b45d76761c09b06
+    sha256: 9bf587a2a0f0f73b71740b079507ec99282b73c596ec73cc602d7ccf73350709
+  manager: conda
+  name: pycosat
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pycosat-0.6.4-py310h5764c6d_1.tar.bz2
+  version: 0.6.4
+- category: main
+  dependencies:
     python: 2.7.*|>=3.4
   hash:
     md5: 076becd9e05608f8dc72757d5f3a91ff
     sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
   manager: conda
   name: pycparser
   optional: false
@@ -3208,22 +3357,34 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
   version: 1.7.1
 - category: main
   dependencies:
     python: '>=3.3'
   hash:
-    md5: dd4f393d857e9283eef2442234bd05e3
-    sha256: b7a8b9b2310b3ee74ba99eef9692e477bb8bddf110eff45784dee7d81a693455
+    md5: 3be9466311564f80f8056c0851fc5bb7
+    sha256: 73985a9a2dd7ccf77b7428a12148e1b381c8635e9195e47a652397e9a56284ce
   manager: conda
   name: python-fastjsonschema
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda
-  version: 2.17.1
+  url: https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.18.0-pyhd8ed1ab_0.conda
+  version: 2.18.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 65dea78f903d686c8b0c2feaf0e15e1f
+    sha256: 822f95b7786cfa61a6519153117b21d93194890e02a884b9f66ee4275e4f1c0a
+  manager: conda
+  name: python-installer
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/python-installer-0.7.0-pyhd8ed1ab_0.conda
+  version: 0.7.0
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
     md5: a61bf9ec79426938ff785eb69dbb1960
     sha256: 4790787fe1f4e8da616edca4acf6a4f8ed4e7c6967aa31b920208fc8f95efcca
   manager: conda
@@ -3348,14 +3509,26 @@
   name: setuptools
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
   version: 67.7.2
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 1de44299f48f522caa2e0074231614e1
+    sha256: 3cb4a4a83b617fdfef9b92751634488db0b8961c80340be8068bf6d4f1d5ac25
+  manager: conda
+  name: shellingham
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.1-pyhd8ed1ab_0.conda
+  version: 1.5.1
+- category: main
+  dependencies:
     python: ''
   hash:
     md5: e5f25f8dbc060e9a8d912e432202afc2
     sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
   manager: conda
   name: six
   optional: false
@@ -3533,14 +3706,38 @@
   name: tomli
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
   version: 2.0.1
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 62f5b331c53d73e2f6c4c130b53518a0
+    sha256: dc4abf58ca42f29e12b8c0f8aadedfca49cc1e97dab025d15cf000b1787df773
+  manager: conda
+  name: tomlkit
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.1-pyha770c72_0.conda
+  version: 0.12.1
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 92facfec94bc02d6ccf42e7173831a36
+    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
+  manager: conda
+  name: toolz
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.12.0
+- category: main
+  dependencies:
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 1c510e74c87dc9b8fe1f7f9e8dbcef96
     sha256: 56bcfc59da0f6fc78afe79447b8b1327e9149a52c9dc6ee805ac73bf18ac22b6
   manager: conda
@@ -3559,28 +3756,52 @@
   name: traitlets
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda
   version: 5.9.0
 - category: main
   dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c9918f6a3973e28a792e747289734cd3
+    sha256: a3b13371ece96434028c9c4cc5561d3a04afdb26165290b630578c1d00b462f7
+  manager: conda
+  name: trove-classifiers
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2023.7.6-pyhd8ed1ab_0.conda
+  version: 2023.7.6
+- category: main
+  dependencies:
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 48d1b46a82b8b4fb6057711dd213977f
     sha256: 1c5fe69f7729a7cde3cf5c1d96ea5c56c3c07209bb48c6d8247e2fa279ba01ca
   manager: conda
   name: typed-ast
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.5-py310h2372a71_0.conda
   version: 1.5.5
 - category: main
   dependencies:
+    python: '>=3'
+  hash:
+    md5: e6573ac68718f17b9d4f5c8eda3190f2
+    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
+  manager: conda
+  name: typing
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.10.0.0
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: c39d6a09fe819de4951c2642629d9115
     sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   manager: conda
   name: typing_extensions
   optional: false
@@ -3635,14 +3856,38 @@
   name: unidecode
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2
   version: 1.3.6
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 0944dc65cb4a9b5b68522c3bb585d41c
+    sha256: b76904b53721dc88a46352324c79d2b077c2f74a9f7208ad2c4249892669ae94
+  manager: conda
+  name: uri-template
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda
+  version: 1.3.0
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 166212fe82dad8735550030488a01d03
+    sha256: 6e097d5fe92849ad3af2c2a313771ad2fbf1cadd4dc4afd552303b2bf3f85211
+  manager: conda
+  name: webcolors
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda
+  version: '1.13'
+- category: main
+  dependencies:
     python: ''
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   manager: conda
   name: webencodings
   optional: false
@@ -3661,22 +3906,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: c95fac682453aeffa12db7ae5a721bec
-    sha256: e91cbb3c0ad9a9507dd030f5493831cb52da120329e0d0793711e8300a36db22
+    md5: 66beb36a1fa7e0dc9d9bf843a80eb82c
+    sha256: c35e6b6c8100e9e42ed0968aef99680b1d1ec5358d4ca0d2b2175f68c6b21dd6
   manager: conda
   name: wheel
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda
-  version: 0.40.0
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.41.0-pyhd8ed1ab_0.conda
+  version: 0.41.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 2e9ebddf0b93d0fb203d0906b8052c4f
     sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
   manager: conda
@@ -3850,14 +4095,27 @@
   name: babel
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda
   version: 2.12.1
 - category: main
   dependencies:
+    python: '>=3.6'
+    typing: '>=3.6'
+  hash:
+    md5: 0e1df3978dd516e20ef88c86d51e5432
+    sha256: 1d86eafb5e9ed078f891e12b46692d786723652907dfb01b047c7da31f92b862
+  manager: conda
+  name: backports.cached-property
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/backports.cached-property-1.0.2-pyhd8ed1ab_0.tar.bz2
+  version: 1.0.2
+- category: main
+  dependencies:
     backports: ''
     python: '>=3.6'
     setuptools: ''
   hash:
     md5: 6b1b907661838a75d067a22f87996b2e
     sha256: 7027bb689dd4ca4a08e3b25805de9d04239be6b31125993558f21f102a9d2700
   manager: conda
@@ -3893,14 +4151,26 @@
   name: bleach
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda
   version: 6.0.0
 - category: main
   dependencies:
+    cached_property: '>=1.5.2,<1.5.3.0a0'
+  hash:
+    md5: 9b347a7ec10940d3f7941ff6c460b551
+    sha256: 561e6660f26c35d137ee150187d89767c988413c978e1b712d53f27ddf70ea17
+  manager: conda
+  name: cached-property
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
     fontconfig: '>=2.13.96,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
     icu: '>=70.1,<71.0a0'
     libgcc-ng: '>=12'
     libglib: '>=2.72.1,<3.0a0'
     libpng: '>=1.6.38,<1.7.0a0'
@@ -3936,25 +4206,38 @@
   name: cffi
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_3.conda
   version: 1.15.1
 - category: main
   dependencies:
+    click: ''
+    python: '>=3.6'
+  hash:
+    md5: 72a46ffc25701c173932fd55cf0965d3
+    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
+  manager: conda
+  name: click-default-group
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.2
+- category: main
+  dependencies:
     python: '>=3.6'
     traitlets: '>=5.3'
   hash:
-    md5: 168ae0f82cdf7505048e81054c7354e4
-    sha256: 657e0a513c8705dc542c54c4c5234e813b7f4e2f412688796d611e83ddf132ea
+    md5: c8eaca39e2b6abae1fc96acc929ae939
+    sha256: 11057745946a95ee7cc4c98900a60c7362266a4cb28bc97d96cd88e3056eb701
   manager: conda
   name: comm
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda
-  version: 0.1.3
+  url: https://conda.anaconda.org/conda-forge/noarch/comm-0.1.4-pyhd8ed1ab_0.conda
+  version: 0.1.4
 - category: main
   dependencies:
     krb5: '>=1.20.1,<1.21.0a0'
     libcurl: 8.1.2 h409715c_0
     libgcc-ng: '>=12'
     libssh2: '>=1.10.0,<2.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
@@ -4015,22 +4298,22 @@
     brotli: ''
     libgcc-ng: '>=12'
     munkres: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     unicodedata2: '>=14.0.0'
   hash:
-    md5: 606aea800172f81896b21cabc5575206
-    sha256: b9e1a3b84c670fab1c491b29c6b36f630aa520f45f08a44440851f46750d85c1
+    md5: f939fe2998c888a77b310926a6c666f3
+    sha256: 6f511ea8de64bf72fb8c247654c7291f5a661c7d34778a000290c75d9bc63211
   manager: conda
   name: fonttools
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.41.0-py310h2372a71_0.conda
-  version: 4.41.0
+  url: https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.42.0-py310h2372a71_0.conda
+  version: 4.42.0
 - category: main
   dependencies:
     libgcc-ng: '>=9.3.0'
     libglu: ''
     libstdcxx-ng: '>=9.3.0'
     xorg-libx11: ''
     xorg-libxext: ''
@@ -4078,14 +4361,28 @@
   name: hdf5
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.12.2-nompi_h4df4325_101.conda
   version: 1.12.2
 - category: main
   dependencies:
+    python: ''
+    six: '>=1.9'
+    webencodings: ''
+  hash:
+    md5: b2355343d6315c892543200231d7154a
+    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
+  manager: conda
+  name: html5lib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
+  version: '1.1'
+- category: main
+  dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
   hash:
     md5: 4e9f59a060c3be52bc4ddc46ee9b6946
     sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   manager: conda
   name: importlib-metadata
@@ -4104,25 +4401,38 @@
   name: importlib_resources
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda
   version: 6.0.0
 - category: main
   dependencies:
+    more-itertools: ''
+    python: '>=3.7'
+  hash:
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
+  manager: conda
+  name: jaraco.classes
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
+  version: 3.3.0
+- category: main
+  dependencies:
     parso: '>=0.8.0,<0.9.0'
     python: '>=3.6'
   hash:
-    md5: b5e695ef9c3f0d27d6cd96bf5adc9e07
-    sha256: abe63ae6e1b13f83500608d94004cb8d485b264083511d77f79253e775cd546c
+    md5: 1cd7f70057cdffc10977b613fb75425d
+    sha256: d2d9e885cbc1efa63107b616588c61000063d4c223c0585962485bd016e77ce8
   manager: conda
   name: jedi
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda
-  version: 0.18.2
+  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.0-pyhd8ed1ab_0.conda
+  version: 0.19.0
 - category: main
   dependencies:
     markupsafe: '>=2.0'
     python: '>=3.7'
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
@@ -4130,14 +4440,27 @@
   name: jinja2
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   version: 3.1.2
 - category: main
   dependencies:
+    jsonpointer: '>=1.9'
+    python: '>=3.6'
+  hash:
+    md5: 09150b51b0528a31a0f6500b96fdde82
+    sha256: d87fd8da2d3327744821b6b1d1e5b76e4077224fb626ce02d6623a1bc6ee2563
+  manager: conda
+  name: jsonpatch
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonpatch-1.32-pyhd8ed1ab_0.tar.bz2
+  version: '1.32'
+- category: main
+  dependencies:
     pygments: '>=2.4.1,<3'
     python: '>=3.7'
   hash:
     md5: 243f63592c8e449f40cd42eb5cf32f40
     sha256: 08453e09d5a6bbaeeca839553a5dfd7a377a97550efab96019c334a8042f54f5
   manager: conda
   name: jupyterlab_pygments
@@ -4156,27 +4479,27 @@
   name: latexcodec
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2
   version: 2.0.1
 - category: main
   dependencies:
-    libclang13: 15.0.7 default_h9986a30_2
+    libclang13: 15.0.7 default_h9986a30_3
     libgcc-ng: '>=12'
     libllvm15: '>=15.0.7,<15.1.0a0'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 1a4fe5162abe4a19b5a9dedf158a0ff9
-    sha256: 9fd064ed59a07ed096fe3c641752be5279f6696bc8b25da0ca4e41fb92758a5b
+    md5: 0922208521c0463e690bbaebba7eb551
+    sha256: c2b0c8dd675e30d86bad410679f258820bc36723fbadffc13c2f60249be91815
   manager: conda
   name: libclang
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libclang-15.0.7-default_h7634d5b_2.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/libclang-15.0.7-default_h7634d5b_3.conda
   version: 15.0.7
 - category: main
   dependencies:
     expat: '>=2.4.8,<3.0a0'
     fontconfig: '>=2.13.96,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.10.4,<3.0a0'
@@ -4527,22 +4850,22 @@
     libstdcxx-ng: '>=12'
     packaging: ''
     ply: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tomli: ''
   hash:
-    md5: a3217e1bff09702dfdfcb536825fc12d
-    sha256: 828ecab2c5b6fd6da4727d4147a856fd643b95801970e8cddc3090204e4c8f8d
+    md5: be1a7e420b7bac4ee02353d0e3161918
+    sha256: c2c7f9791b0809ab5ffca1ef5c68812da01efb1eda88071a9031895334be4007
   manager: conda
   name: sip
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py310hc6cd4ac_0.conda
-  version: 6.7.9
+  url: https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.11-py310hc6cd4ac_0.conda
+  version: 6.7.11
 - category: main
   dependencies:
     __unix: ''
     gmpy2: '>=2.0.8'
     mpmath: '>=0.19'
     python: '>=3.8'
   hash:
@@ -4648,14 +4971,27 @@
   name: yarl
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/yarl-1.9.2-py310h2372a71_0.conda
   version: 1.9.2
 - category: main
   dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  manager: conda
+  name: annotated-types
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  version: 0.5.0
+- category: main
+  dependencies:
     cffi: '>=1.0.1'
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 12f70cd23e4ea88f913dba50b0f0aba0
     sha256: 66cc235b93b36b36c90b5986979067c2e8fb2c5d9729f3a29d068664e90ffc7a
@@ -4663,14 +4999,28 @@
   name: argon2-cffi-bindings
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py310h5764c6d_3.tar.bz2
   version: 21.2.0
 - category: main
   dependencies:
+    python: '>=3.6'
+    python-dateutil: '>=2.7.0'
+    typing_extensions: ''
+  hash:
+    md5: fd1967c76eda3a3dd9e8e6cb7a15a028
+    sha256: a0434c2770cf5b0ab5a33913c0b202b1521bc13f755b762d16a86b110425cdc2
+  manager: conda
+  name: arrow
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/arrow-1.2.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.2.3
+- category: main
+  dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.0.0'
     wrapt: <2,>=1.11
   hash:
     md5: 8ad02555d6ecdb8fd5f1963690c59699
@@ -4753,14 +5103,27 @@
   name: ffmpeg
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/ffmpeg-5.1.2-gpl_h8dda1f0_106.conda
   version: 5.1.2
 - category: main
   dependencies:
+    cached-property: '>=1.3.0'
+    python: '>=2.7,<4'
+  hash:
+    md5: 642d35437078749ef23a5dca2c9bb1f3
+    sha256: 6cfd1f9bcd2358a69fb571f4b3af049b630d52647d906822dbedac03e84e4f63
+  manager: conda
+  name: fqdn
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2
+  version: 1.5.1
+- category: main
+  dependencies:
     python: '>=3.6'
     python-dateutil: '>=2.8.1'
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
   manager: conda
   name: ghp-import
@@ -4903,22 +5266,22 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.8.1-nompi_h261ec11_106.tar.bz2
   version: 4.8.1
 - category: main
   dependencies:
     importlib-metadata: '>=4.4'
     python: '>=3.6'
   hash:
-    md5: 89ed59ad509c05db6f5f2f573d499bfe
-    sha256: e32ac2c95112caa8cd81f0cbc710f4f4903180a115c7260f03b010d5a0aa771b
+    md5: 6b8ab17bc8ff1ca89b3ea28ea3d566ca
+    sha256: cf1b3778cf99bd0301c4eb4f5d3d575e8c4248c15a019189b3892131a2675854
   manager: conda
   name: markdown
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda
-  version: 3.4.3
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.4-pyhd8ed1ab_0.conda
+  version: 3.4.4
 - category: main
   dependencies:
     markdown-it-py: '>=1.0.0,<4.0.0'
     python: '>=3.8'
   hash:
     md5: 6c5358a10873a15398b6f15f60cb5e1f
     sha256: 1ddac8d2be448cd1fbe49d2ca09df7e10d99679d53146a917f8bb4899f76d0ca
@@ -4942,22 +5305,35 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/mkl-devel-2022.1.0-ha770c72_916.tar.bz2
   version: 2022.1.0
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 044e7a1e0ad42c4e67110bd078150a63
-    sha256: 885611bd528abaf3e31bc0bfaad3a619cfe89db61d886b53c2a9ec9ff50edebe
+    md5: 0809187ef9b89a3d94a5c24d13936236
+    sha256: 1b5c0ca2f4260c7dd8cfccd8a641c1e41876c79dc594506be379cde08f5b471e
   manager: conda
   name: platformdirs
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda
-  version: 3.9.1
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.10.0-pyhd8ed1ab_0.conda
+  version: 3.10.0
+- category: main
+  dependencies:
+    importlib-metadata: '>=1.7.0'
+    python: '>=3.7'
+  hash:
+    md5: a6d1f61527c27fcc0165a6701a46b9f4
+    sha256: 6f6a66476908a1c109e36c852d934eedceb07e0cbc44d3fcd87c6f39521b57be
+  manager: conda
+  name: poetry-core
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-core-1.6.1-pyhd8ed1ab_0.conda
+  version: 1.6.1
 - category: main
   dependencies:
     alsa-lib: '>=1.2.8,<1.2.9.0a0'
     dbus: '>=1.13.6,<2.0a0'
     fftw: '>=3.3.10,<4.0a0'
     gstreamer-orc: '>=0.4.33,<0.5.0a0'
     jack: '>=1.9.22,<1.10.0a0'
@@ -4994,29 +5370,44 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2
   version: 0.24.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    typing-extensions: '>=4.6.0'
+  hash:
+    md5: 10c338c86b8b23f150948de8a80e70e5
+    sha256: 1ed54895757b85206da6c880ee0cb400188c788567049497519297f01225baed
+  manager: conda
+  name: pydantic-core
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.4.0-py310hcb5633a_0.conda
+  version: 2.4.0
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     packaging: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     sip: ''
     toml: ''
   hash:
-    md5: 3b1946b676534472ce65181dda0b9554
-    sha256: 7b58a8ca0bd2ab65d2c77017b288a551522dc5fe07d5d2dfa5189cdbb71019e8
+    md5: 345beb10601d5360a15c033d68165a4f
+    sha256: 04926c525f5e4a3bf63d9fab739a3bbdf09891b95b79944ceeda71e24c3ab84e
   manager: conda
   name: pyqt5-sip
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py310heca2aa9_3.conda
-  version: 12.11.0
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py310hc6cd4ac_4.conda
+  version: 12.12.2
 - category: main
   dependencies:
     colorama: ''
     importlib-metadata: '>=0.22'
     packaging: '>=19.0'
     pyproject_hooks: ''
     python: '>=3.7'
@@ -5088,14 +5479,30 @@
   name: wcwidth
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda
   version: 0.2.6
 - category: main
   dependencies:
+    cffi: '>=1.11'
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: a2b48edcd52593cdf007158ce10e1520
+    sha256: 76a443ffcda1c290dbcc8c0bbe15a0f0ee0b57009cf842940f3382672780ddd8
+  manager: conda
+  name: zstandard
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.19.0-py310h1275a96_2.conda
+  version: 0.19.0
+- category: main
+  dependencies:
     aiosignal: '>=1.1.2'
     async-timeout: <5.0,>=4.0.0a3
     attrs: '>=17.3.0'
     charset-normalizer: '>=2.0,<4.0'
     frozenlist: '>=1.1.1'
     libgcc-ng: '>=12'
     multidict: '>=4.5,<7.0'
@@ -5143,14 +5550,27 @@
   name: black
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2
   version: 22.3.0
 - category: main
   dependencies:
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 38253361efb303deead3eab39ae9269b
+    sha256: 654a2488f77bf43555787d952dbffdc5d97956ff4aa9e0414a7131bb741dcf4c
+  manager: conda
+  name: conda-package-streaming
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.9.0-pyhd8ed1ab_0.conda
+  version: 0.9.0
+- category: main
+  dependencies:
     __glibc: '>=2.17,<3.0.a0'
     alsa-lib: '>=1.2.8,<1.2.9.0a0'
     gettext: '>=0.21.1,<1.0a0'
     gstreamer: 1.22.0 h25f0c4b_2
     libgcc-ng: '>=12'
     libglib: '>=2.74.1,<3.0a0'
     libopus: '>=1.3.1,<2.0a0'
@@ -5166,14 +5586,27 @@
   name: gst-plugins-base
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.0-h4243ec0_2.conda
   version: 1.22.0
 - category: main
   dependencies:
+    arrow: '>=0.15.0'
+    python: '>=3.7'
+  hash:
+    md5: 4cb68948e0b8429534380243d063a27a
+    sha256: 7bb5c4d994361022f47a807b5e7d101b3dce16f7dd8a0af6ffad9f479d346493
+  manager: conda
+  name: isoduration
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2
+  version: 20.11.0
+- category: main
+  dependencies:
     platformdirs: '>=2.5'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     traitlets: '>=5.3'
   hash:
     md5: 63264f5a6dd5483475968016b614f525
     sha256: ef2758f0f0ee5e31df2122280eeb9aa2a44abffe2b583654ed0c343d65bb7f3e
@@ -5181,32 +5614,14 @@
   name: jupyter_core
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py310hff52083_0.conda
   version: 5.3.1
 - category: main
   dependencies:
-    jsonschema: '>=3.2'
-    python: '>=3.7'
-    python-json-logger: '>=2.0.4'
-    pyyaml: '>=5.3'
-    rfc3339-validator: ''
-    rfc3986-validator: '>=0.1.1'
-    traitlets: '>=5.3'
-  hash:
-    md5: d98c5196ab6ffeb0c2feca2912801353
-    sha256: 16f73833537e05384d3eef27e62edb31de344d6d26666e1a465c1819014f2655
-  manager: conda
-  name: jupyter_events
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda
-  version: 0.6.3
-- category: main
-  dependencies:
     libblas: 3.9.0 16_linux64_mkl
   hash:
     md5: 361bf757b95488de76c4f123805742d3
     sha256: 892ba10508f22310ccfe748df1fd3b6c7f20e7b6f6b79e69ed337863551c1bd8
   manager: conda
   name: libcblas
   optional: false
@@ -5258,14 +5673,27 @@
   name: pango
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/pango-1.50.14-hd33c08f_0.conda
   version: 1.50.14
 - category: main
   dependencies:
+    poetry-core: '>=1.6.0,<2.0.0'
+    python: '>=3.7,<4.0'
+  hash:
+    md5: 00893c7ea4f9f7620706e0aa94c01b6e
+    sha256: 54478b283b5967a85ee5da717f1512d7ec97eb07c7b52d1f2ad3cb080d56c0ac
+  manager: conda
+  name: poetry-plugin-export
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-plugin-export-1.4.0-pyhd8ed1ab_0.conda
+  version: 1.4.0
+- category: main
+  dependencies:
     python: '>=3.7'
     wcwidth: ''
   hash:
     md5: a4986c6bb5b0d05a38855b0880a5f425
     sha256: 10e7fdc75d4b85633be6b12a70b857053987127a808caa0f88b2cba4b3ce6359
   manager: conda
   name: prompt-toolkit
@@ -5301,27 +5729,58 @@
   name: pybtex-docutils
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.2-py310hff52083_2.tar.bz2
   version: 1.0.2
 - category: main
   dependencies:
+    annotated-types: '>=0.4.0'
+    pydantic-core: 2.4.0
+    python: '>=3.7'
+    typing-extensions: '>=4.6.1'
+  hash:
+    md5: 7964a624018707909044b509f58b937a
+    sha256: ee8a995c201e83421f3fb24f359c609900b8891d99331fc23dae32166931d744
+  manager: conda
+  name: pydantic
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.1.1-pyhd8ed1ab_0.conda
+  version: 2.1.1
+- category: main
+  dependencies:
     cryptography: '>=38.0.0,<42,!=40.0.0,!=40.0.1'
     python: '>=3.6'
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   manager: conda
   name: pyopenssl
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda
   version: 23.2.0
 - category: main
   dependencies:
+    cryptography: ''
+    dbus: ''
+    jeepney: '>=0.6'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: e135d0e3bbb226e8d53d31b4e4f6d93c
+    sha256: 25d2a00bf24a3cab81eba8f77eba8f70a7b3995041fc227f535c0f174536670f
+  manager: conda
+  name: secretstorage
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py310hff52083_1.tar.bz2
+  version: 3.3.3
+- category: main
+  dependencies:
     fftw: '>=3.3.10,<4.0a0'
     libgcc-ng: '>=12'
     libitk: 5.3.0 hcedbc38_0
     libstdcxx-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
@@ -5331,14 +5790,43 @@
   name: simpleitk
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/simpleitk-2.2.1-py310h2b9ea3a_1.conda
   version: 2.2.1
 - category: main
   dependencies:
+    distlib: <1,>=0.3.7
+    filelock: <4,>=3.12.2
+    platformdirs: <4,>=3.9.1
+    python: '>=3.8'
+  hash:
+    md5: a218f3be8ab6185a475c8168a86e18ae
+    sha256: 3e508638077bcba79db4d26037c8e97bf6b7b43d156a06c9c25cdd2136468459
+  manager: conda
+  name: virtualenv
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.2-pyhd8ed1ab_0.conda
+  version: 20.24.2
+- category: main
+  dependencies:
+    conda-package-streaming: '>=0.9.0'
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 8a3ae7f6318376aa08ea753367bb7dd6
+    sha256: 9a221808405d813d8c555efce6944379b907d36d79e77d526d573efa6b996d26
+  manager: conda
+  name: conda-package-handling
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.2.0-pyh38be061_0.conda
+  version: 2.2.0
+- category: main
+  dependencies:
     black: '>=22.1.0'
     flake8: '>=3'
     python: '>=3.7'
     tomli: ''
   hash:
     md5: 61649e6e9b39ac0c7d10938025f6fe4f
     sha256: 736dbadccbd0ce6371ffa011b761c03bf9e9d329582d0c5daecdbff0e96e2a36
@@ -5364,14 +5852,35 @@
   name: gtk2
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h90689f9_2.tar.bz2
   version: 2.24.33
 - category: main
   dependencies:
+    fqdn: ''
+    idna: ''
+    isoduration: ''
+    jsonpointer: '>1.13'
+    jsonschema: '>=4.17.3,<5.0a0'
+    python: ''
+    rfc3339-validator: ''
+    rfc3986-validator: '>0.1.0'
+    uri-template: ''
+    webcolors: '>=1.11'
+  hash:
+    md5: 7a709748e93f0b2c33d6b5b676b6d9d0
+    sha256: 767da9c47d64e1dc826d3173e46ff6fd4e858c94ff61d67ff4f976c7bc9502a2
+  manager: conda
+  name: jsonschema-with-format-nongpl
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.17.3-pyhd8ed1ab_0.conda
+  version: 4.17.3
+- category: main
+  dependencies:
     importlib_metadata: '>=4.8.3'
     jupyter_core: '>=4.12,!=5.0.*'
     python: '>=3.8'
     python-dateutil: '>=2.8.2'
     pyzmq: '>=23.0'
     tornado: '>=6.2'
     traitlets: '>=5.3'
@@ -5382,14 +5891,31 @@
   name: jupyter_client
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda
   version: 8.3.0
 - category: main
   dependencies:
+    importlib_metadata: '>=4.11.4'
+    jaraco.classes: ''
+    jeepney: '>=0.4.2'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    secretstorage: '>=3.2'
+  hash:
+    md5: 85da2982e8456156e2f38e6a3f75cd89
+    sha256: c709408ded9e04b193a5f6c77f6586ab4ab93bdb5a5413eeecc9530165ccf312
+  manager: conda
+  name: keyring
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/keyring-23.13.1-py310hff52083_0.conda
+  version: 23.13.1
+- category: main
+  dependencies:
     libblas: 3.9.0 16_linux64_mkl
     libcblas: 3.9.0 16_linux64_mkl
     liblapack: 3.9.0 16_linux64_mkl
   hash:
     md5: 44ccc4d4dca6a8d57fa17442bc64b5a1
     sha256: 935036dc46c483cba8288c6de58d461ab3f42915715ffe9485105ad1dd203a0e
   manager: conda
@@ -5420,40 +5946,40 @@
   dependencies:
     jsonschema: '>=2.6'
     jupyter_core: ''
     python: '>=3.8'
     python-fastjsonschema: ''
     traitlets: '>=5.1'
   hash:
-    md5: 3ec35d84fc1775215061517eb4660693
-    sha256: d8b1ad3c219b39e5e325785606853ff1cd334769228490ac977b85aa95e94ba0
+    md5: 61ba076de6530d9301a0053b02f093d2
+    sha256: fc82c5a9116820757b03ffb836b36f0f50e4cd390018024dbadb0ee0217f6992
   manager: conda
   name: nbformat
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda
-  version: 5.9.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.2-pyhd8ed1ab_0.conda
+  version: 5.9.2
 - category: main
   dependencies:
     libblas: '>=3.9.0,<4.0a0'
     libcblas: '>=3.9.0,<4.0a0'
     libgcc-ng: '>=12'
     liblapack: '>=3.9.0,<4.0a0'
     libstdcxx-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 3810cbf2635cb1d0edb97715d4ad74e7
-    sha256: 38ec15fe0afe9fb90bd50314ccd506f0e7d1642db0c7eb2b77627d448aa9ee6c
+    md5: 188e72aa313da668464e35309e9a32b0
+    sha256: 81bba557f0f6109f7a1cb8f4d739e5c9ef310a49f8a2842f1fc67bd3545067b0
   manager: conda
   name: numpy
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.1-py310ha4c1d20_0.conda
-  version: 1.25.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.2-py310ha4c1d20_0.conda
+  version: 1.25.2
 - category: main
   dependencies:
     prompt-toolkit: '>=3.0.39,<3.0.40.0a0'
   hash:
     md5: 4bbbe67d5df19db30f04b8e344dc9976
     sha256: 89f7fecc7355181dbc2ab851e668a2fce6aa4830b336a34c93b59bda93206270
   manager: conda
@@ -5588,14 +6114,34 @@
   name: contourpy
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py310hd41b1e2_0.conda
   version: 1.1.0
 - category: main
   dependencies:
+    certifi: ''
+    cryptography: '>=1.3.4'
+    idna: '>=2.0.0'
+    libgcc-ng: '>=12'
+    pyopenssl: '>=0.14'
+    pysocks: '>=1.5.6,<2.0,!=1.5.7'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    urllib3: ''
+  hash:
+    md5: 58ee4d1dd828531bb6d69fd6bd304882
+    sha256: 61008637ae756df19f97667141d365a16d16de53322c680606f20ef69c73f481
+  manager: conda
+  name: dulwich
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/dulwich-0.21.5-py310h2372a71_0.conda
+  version: 0.21.5
+- category: main
+  dependencies:
     cairo: '>=1.16.0,<2.0a0'
     expat: '>=2.5.0,<3.0a0'
     fontconfig: '>=2.14.1,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
     gdk-pixbuf: '>=2.42.8,<3.0a0'
     gtk2: ''
@@ -5641,14 +6187,32 @@
   name: ipython
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda
   version: 8.14.0
 - category: main
   dependencies:
+    jsonschema-with-format-nongpl: '>=3.2'
+    python: '>=3.7'
+    python-json-logger: '>=2.0.4'
+    pyyaml: '>=5.3'
+    rfc3339-validator: ''
+    rfc3986-validator: '>=0.1.1'
+    traitlets: '>=5.3'
+  hash:
+    md5: 279fed93be42722de98e998ec80be8a1
+    sha256: 1b168cd11337dcbd2eae71b91ad7624c5afed0561e4f703d5eeee27e182f98c1
+  manager: conda
+  name: jupyter_events
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.7.0-pyhd8ed1ab_0.conda
+  version: 0.7.0
+- category: main
+  dependencies:
     jupyter_client: '>=6.1.12'
     jupyter_core: '>=4.12,!=5.0.*'
     nbformat: '>=5.1'
     python: '>=3.7'
     traitlets: '>=5.3'
   hash:
     md5: f7aa15f77d29b11caa1df1eb15383c59
@@ -5692,28 +6256,44 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py310h9b08913_1.conda
   version: 1.5.3
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
-    pyqt5-sip: 12.11.0 py310heca2aa9_3
+    pyqt5-sip: 12.12.2 py310hc6cd4ac_4
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
-    qt-main: '>=5.15.6,<5.16.0a0'
-    sip: '>=6.7.5,<6.8.0a0'
+    qt-main: '>=5.15.8,<5.16.0a0'
+    sip: '>=6.7.10,<6.8.0a0'
   hash:
-    md5: d049da3204bf5ecb54a852b622f2d7d2
-    sha256: 9210571612b135979541c5c65d28eda82941b3d613f3c8c792971bdfb7b4383a
+    md5: db878a0696f9a7980171fd3cf29cca22
+    sha256: 6919204ea9e653c3f6710e962436adfd5e86eaea0c8980f1466b36750a2e7765
   manager: conda
   name: pyqt
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py310hab646b1_3.conda
-  version: 5.15.7
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py310h04931ad_4.conda
+  version: 5.15.9
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
+    numpy: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 542887fb70fae388f9df109866469ca1
+    sha256: 14e8ff789947e25614574a02eee3b561476a1b65bf780c8cd5055ff9aba15f73
+  manager: conda
+  name: rapidfuzz
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/rapidfuzz-2.15.1-py310heca2aa9_0.conda
+  version: 2.15.1
 - category: main
   dependencies:
     certifi: '>=2017.4.17'
     charset-normalizer: '>=2,<4'
     idna: '>=2.5,<4'
     python: '>=3.7'
     urllib3: '>=1.21.1,<3'
@@ -5793,14 +6373,83 @@
   name: blas
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/blas-2.116-mkl.tar.bz2
   version: '2.116'
 - category: main
   dependencies:
+    msgpack-python: '>=0.5.2'
+    python: '>=3.6'
+    requests: '>=2.16.0'
+  hash:
+    md5: db23395890ef31be3c2320fb41b665b0
+    sha256: 99b68d1e9b1e148c9dfa5886cdd9b6082e968328658ba71a5b76cdc93a92ef02
+  manager: conda
+  name: cachecontrol
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.14-pyhd8ed1ab_0.conda
+  version: 0.12.14
+- category: main
+  dependencies:
+    crashtest: '>=0.4.1,<0.5.0'
+    python: '>=3.7,<4.0'
+    rapidfuzz: '>=2.2.0,<3.0.0'
+  hash:
+    md5: f1c5f2af6676cbe9206e191d1e70f661
+    sha256: cf9bc4c9356ad8eb68512446eebc076386f2bfb8ca86626e8796621bc5a13082
+  manager: conda
+  name: cleo
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cleo-2.0.1-pyhd8ed1ab_0.conda
+  version: 2.0.1
+- category: main
+  dependencies:
+    boltons: '>=23.0.0'
+    conda-package-handling: '>=1.3.0'
+    jsonpatch: '>=1.32'
+    packaging: '>=23.0'
+    pluggy: '>=1.0.0'
+    pycosat: '>=0.6.3'
+    pyopenssl: '>=16.2.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.27.0,<3'
+    ruamel.yaml: '>=0.11.14,<0.18'
+    setuptools: '>=60.0.0'
+    toolz: '>=0.8.1'
+    tqdm: '>=4'
+  hash:
+    md5: c5d666e682ca57f5853304d1fe82c131
+    sha256: bd89b661853b2f2646b17bc8a27a0c74dcebd0e7e932bc5163f350438a8c7cee
+  manager: conda
+  name: conda
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/conda-23.7.2-py310hff52083_0.conda
+  version: 23.7.2
+- category: main
+  dependencies:
+    appdirs: ''
+    click: '>=5.1'
+    filelock: ''
+    python: '>=3.7'
+    requests: '>=2'
+  hash:
+    md5: c99ae3abf501990769047b4b40a98f17
+    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
+  manager: conda
+  name: ensureconda
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.3
+- category: main
+  dependencies:
     aiohttp: '>=3.6.2,<4.0.0dev'
     cachetools: '>=2.0.0,<6.0'
     pyasn1-modules: '>=0.2.1'
     pyopenssl: '>=20.0.0'
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
@@ -5839,14 +6488,31 @@
   name: ipykernel
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda
   version: 6.23.3
 - category: main
   dependencies:
+    comm: '>=0.1.3'
+    ipython: '>=6.1.0'
+    jupyterlab_widgets: '>=3.0.7,<3.1.0'
+    python: '>=3.7'
+    traitlets: '>=4.3.1'
+    widgetsnbextension: '>=4.0.7,<4.1.0'
+  hash:
+    md5: 6fe1e9c8e93261e978998c0e90e36275
+    sha256: 71f920b0b89eb177511ff2d8bd9904c9c6c96d731f90ec97168cc28bc86ed623
+  manager: conda
+  name: ipywidgets
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.0-pyhd8ed1ab_0.conda
+  version: 8.1.0
+- category: main
+  dependencies:
     attrs: ''
     click: ''
     importlib-metadata: ''
     nbclient: '>=0.2,<0.8'
     nbformat: ''
     python: '>=3.8'
     pyyaml: ''
@@ -5904,22 +6570,22 @@
     packaging: ''
     pandocfilters: '>=1.4.1'
     pygments: '>=2.4.1'
     python: '>=3.8'
     tinycss2: ''
     traitlets: '>=5.0'
   hash:
-    md5: 32dde1678bb003c90d4bc0c2dbd21814
-    sha256: 76ad7689d35fe031459c422f142c9d8e7a02f6922049b7a0183fc70aaef02f0a
+    md5: 063c1fda5480050b8d989478c97a4c55
+    sha256: c5db2ba740b2ffddf11a5ba67a3afa7c05bff4656dae3d5f61a9b57c57ea3f8b
   manager: conda
   name: nbconvert-core
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     packaging: '>=20.0'
     platformdirs: '>=2.5.0'
     python: '>=3.7'
     requests: '>=2.19.0'
   hash:
@@ -5943,14 +6609,27 @@
   name: requests-oauthlib
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2
   version: 1.3.1
 - category: main
   dependencies:
+    python: '>=3.6'
+    requests: '>=2.0.1,<3.0.0'
+  hash:
+    md5: 99c98318c8646b08cc764f90ce98906e
+    sha256: 20eaefc5dba74ff6c31e537533dde59b5b20f69e74df49dff19d43be59785fa3
+  manager: conda
+  name: requests-toolbelt
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
+  version: 1.0.0
+- category: main
+  dependencies:
     botocore: '>=1.12.36,<2.0a.0'
     python: '>=3.7'
   hash:
     md5: b19a857ac845097e9c823c9f4d35f80e
     sha256: 99512bf4f4e297cc7565c94eee8ccc908411f836b341668e2b5d064273e21762
   manager: conda
   name: s3transfer
@@ -6000,14 +6679,44 @@
   name: boto3
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda
   version: 1.26.165
 - category: main
   dependencies:
+    cachecontrol: 0.12.14 pyhd8ed1ab_0
+    lockfile: '>=0.9'
+    python: '>=3.6'
+  hash:
+    md5: 43ed0c094b39bb352382db8105ab0b94
+    sha256: 23af777f65d74f18aaee1641add3b15bd442096f9c4940270151704f1aa38198
+  manager: conda
+  name: cachecontrol-with-filecache
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.14-pyhd8ed1ab_0.conda
+  version: 0.12.14
+- category: main
+  dependencies:
+    conda: '>=4.3'
+    jinja2: ''
+    packaging: ''
+    python: '>=3.6'
+    pyyaml: ''
+  hash:
+    md5: 9b175e69c1c601d01ab5edccf822363c
+    sha256: 3244e025f3d185f56fb44a44d02526797ce3e95302a868867af6dc9e2e55ebe3
+  manager: conda
+  name: conda-devenv
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-devenv-2.3.0-pyhd8ed1ab_0.tar.bz2
+  version: 2.3.0
+- category: main
+  dependencies:
     click: '>=6.0.0'
     google-auth: '>=2.15.0'
     python: '>=3.6'
     requests-oauthlib: '>=0.7.0'
   hash:
     md5: 569e62e95b01b53e4ec7d9abe83b7385
     sha256: f89613643658a51a1ac0fb7c7950526fadc2a6ce1ae13755d786e14cfce1633c
@@ -6015,31 +6724,14 @@
   name: google-auth-oauthlib
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda
   version: 1.0.0
 - category: main
   dependencies:
-    ipykernel: '>=4.5.1'
-    ipython: '>=6.1.0'
-    jupyterlab_widgets: '>=3.0.7,<3.1.0'
-    python: '>=3.7'
-    traitlets: '>=4.3.1'
-    widgetsnbextension: '>=4.0.7,<4.1.0'
-  hash:
-    md5: 4b0f4e8fe2a303e472674eae0340bdad
-    sha256: 3b17ad90294f0684fca9191f1e696e9b4f03a652d5e588b6ff0feb5647fcf116
-  manager: conda
-  name: ipywidgets
-  optional: false
-  platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda
-  version: 8.0.7
-- category: main
-  dependencies:
     ipykernel: '>=6.14'
     ipython: ''
     jupyter_client: '>=7.0.0'
     jupyter_core: '>=4.12,!=5.0.*'
     prompt_toolkit: '>=3.0.30'
     pygments: ''
     python: '>=3.7'
@@ -6117,26 +6809,26 @@
   name: myst-parser
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2
   version: 0.18.1
 - category: main
   dependencies:
-    nbconvert-core: 7.7.1 pyhd8ed1ab_1
+    nbconvert-core: 7.7.3 pyhd8ed1ab_0
     pandoc: ''
     python: '>=3.8'
   hash:
-    md5: 796b056965d7146bcac082fa2a83943d
-    sha256: b5b2823e7951a5ba41b1020b7cce109fec7f2ebe540234bf8a17c54615c2f679
+    md5: f44109e52a40b8149156f5ddd9c11b26
+    sha256: c9fceb914dd4a8fe64b1403a0c7b0c69b5c67fc726aa8239e5ecb450d27e6963
   manager: conda
   name: nbconvert-pandoc
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     accessible-pygments: ''
     babel: ''
     beautifulsoup4: ''
     docutils: '!=0.17.0'
     packaging: ''
@@ -6394,26 +7086,26 @@
   name: myst-nb
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda
   version: 0.17.2
 - category: main
   dependencies:
-    nbconvert-core: 7.7.1 pyhd8ed1ab_1
-    nbconvert-pandoc: 7.7.1 pyhd8ed1ab_1
+    nbconvert-core: 7.7.3 pyhd8ed1ab_0
+    nbconvert-pandoc: 7.7.3 pyhd8ed1ab_0
     python: '>=3.8'
   hash:
-    md5: 95d9d1523df069792cd059f412be0d6e
-    sha256: c49a87861db316b322f919825820bc7193cbfa8a4a8b21b5ffe16a133644d400
+    md5: f53d92ecd7d8563b006107f6a33e55c6
+    sha256: 2b9e7bc41ee0882d7829e984cb1a18f039a5f756b5b747f6a3ce352bc72e5103
   manager: conda
   name: nbconvert
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     jupyter_server: '>=1.8,<3'
     python: '>=3.7'
   hash:
     md5: 67e0fe74c156267d9159e9133df7fd37
     sha256: f028d7ad1f2175cde307db08b60d07e371b9d6f035cfae6c81ea94b4c408c538
@@ -6421,14 +7113,55 @@
   name: notebook-shim
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda
   version: 0.2.3
 - category: main
   dependencies:
+    __linux: ''
+    backports.cached-property: '>=1.0.2,<2.0.0'
+    cachecontrol-with-filecache: '>=0.12.9,<0.13.0'
+    cleo: '>=2.0.0,<3.0.0'
+    crashtest: '>=0.4.1,<0.5.0'
+    dulwich: '>=0.21.2,<0.22.0'
+    filelock: '>=3.8.0,<4.0.0'
+    html5lib: '>=1.0.0,<2.0.0'
+    importlib-metadata: '>=4.4'
+    jsonschema: '>=4.10.0,<5.0.0'
+    keyring: '>=23.9.0,<24.0.0'
+    lockfile: '>=0.12.2,<0.13.0'
+    packaging: '>=20.4'
+    pexpect: '>=4.7.0,<5.0.0'
+    pkginfo: '>=1.9.4,<2.0'
+    platformdirs: '>=3.0.0,<4.0.0'
+    poetry-core: 1.6.1.*
+    poetry-plugin-export: '>=1.4.0,<2.0.0'
+    pyproject_hooks: '>=1.0.0,<2.0.0'
+    python: '>=3.7.0,<4.0.0'
+    python-build: '>=0.10.0,<0.11.0'
+    python-installer: '>=0.7.0,<0.8.0'
+    requests: '>=2.18,<3.0'
+    requests-toolbelt: '>=0.9.1,<2'
+    shellingham: '>=1.5.0,<2.0.0'
+    tomli: '>=2.0.1,<3.0.0'
+    tomlkit: '>=0.11.4,<1.0.0'
+    trove-classifiers: '>=2022.5.19'
+    urllib3: '>=1.26.0,<2.0.0'
+    virtualenv: '>=20.22.0,<21.0.0'
+  hash:
+    md5: 7aae42823198731808dd8e7a9745547f
+    sha256: 754fb55e83fe06366f4532fbb25344bc9c7d46ac71d2a1c35209e818f7fa9d10
+  manager: conda
+  name: poetry
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-1.5.1-linux_pyhd8ed1ab_0.conda
+  version: 1.5.1
+- category: main
+  dependencies:
     pyqt: ''
     python: '>=3.7'
     qtconsole-base: '>=5.4.3,<5.4.4.0a0'
   hash:
     md5: 3777f933bec5113d5a292de10b03d0f6
     sha256: 6443de033408a3d5f915dcd5b0b52806a86b20e54d85859f042ed71443651231
   manager: conda
@@ -6508,14 +7241,38 @@
   name: tensorboard
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda
   version: 2.13.0
 - category: main
   dependencies:
+    click: '>=8.0'
+    click-default-group: ''
+    ensureconda: '>=1.3'
+    jinja2: ''
+    poetry: ''
+    pydantic: '>=1.8.1'
+    python: '>=3.6'
+    pyyaml: '>=5.1'
+    requests: '>=2'
+    ruamel.yaml: ''
+    setuptools: ''
+    toml: ''
+    typing-extensions: ''
+  hash:
+    md5: 1c31d380288fc1599fb5f4c76c8c828c
+    sha256: 2895546468293f358395b072846ebf8a2e04339d1355009fb96787d804250bb0
+  manager: conda
+  name: conda-lock
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.0.5-pyhd8ed1ab_1.tar.bz2
+  version: 1.0.5
+- category: main
+  dependencies:
     click: '>=7.1,<9'
     docutils: '>=0.15,<0.19'
     jinja2: ''
     jsonschema: <5
     linkify-it-py: '>=2.0.0,<2.1.0'
     myst-nb: '>=0.17.1,<0.18.0'
     python: '>=3.7'
@@ -6711,22 +7468,22 @@
     pytorch: '>=1.11.0'
     pyyaml: '>=5.4'
     requests: ''
     torchmetrics: '>=0.7.0'
     tqdm: '>=4.57.0'
     typing_extensions: '>=4.0.0'
   hash:
-    md5: ce9d626b181c6f8cceb5047f6a819f7d
-    sha256: a049296b4b33bceedf3bafd378e8a4112bca71b453734f1e0daaca2a72598593
+    md5: 5325b6adf171d4d69968100af806994e
+    sha256: 54efb4be9a8f73692cf24f85923a226c0ed6d035000704479b0f27288bb0a874
   manager: conda
   name: pytorch-lightning
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda
-  version: 2.0.4
+  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.6-pyhd8ed1ab_0.conda
+  version: 2.0.6
 - category: main
   dependencies: {}
   hash:
     md5: 37edc4e6304ca87316e160f5ca0bd1b5
     sha256: 60ba4c64f5d0afca0d283c7addba577d3e2efc0db86002808dadb0498661b2f2
   manager: conda
   name: bzip2
@@ -6744,22 +7501,22 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda
   version: 1.19.1
 - category: main
   dependencies: {}
   hash:
-    md5: b704e4b79ba0d887c4870b7b09d6a4df
-    sha256: a06c9c788de81da3a3868ac56781680cc1fc50a0b5a545d4453818975c141b2c
+    md5: bf2c54c18997bf3542af074c10191771
+    sha256: 27de15e18a12117e83ac1eb8a8e52eb65731cc7f0b607a7922206a15e2460c7b
   manager: conda
   name: ca-certificates
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda
-  version: 2023.5.7
+  url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.7.22-h8857fd0_0.conda
+  version: 2023.7.22
 - category: main
   dependencies: {}
   hash:
     md5: 0c96522c6bdaed4b1566d11387caaf45
     sha256: 58d7f40d2940dd0a8aa28651239adbf5613254df0f75789919c4e6762054403b
   manager: conda
   name: font-ttf-dejavu-sans-mono
@@ -7198,22 +7955,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/double-conversion-3.2.0-hf0c8a7f_1.tar.bz2
   version: 3.2.0
 - category: main
   dependencies:
     libcxx: '>=15.0.7'
   hash:
-    md5: 4b30cbb5ec44b4ce28e92daac53f3132
-    sha256: 1a78245598a5665a7fd3451a171e11ac3ee9ef954a833454bf9522eadf0fb528
+    md5: 5b2cfc277e3d42d84a2a648825761156
+    sha256: 187c0677e0cdcdc39aed716687a6290dd5b7f52b49eedaef2ed76be6cd0a5a3d
   manager: conda
   name: eigen
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.1-h1c7c39f_0.conda
-  version: 3.4.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.0-h1c7c39f_0.conda
+  version: 3.4.0
 - category: main
   dependencies:
     libexpat: 2.5.0 hf0c8a7f_1
   hash:
     md5: e12630038077877cbb6c7851e139c17c
     sha256: 15c04a5a690b337b50fb7550cce057d843cf94dd0109d576ec9bc3448a8571d0
   manager: conda
@@ -7381,22 +8138,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2
   version: 3.1.20191231
 - category: main
   dependencies:
     llvm-openmp: '>=8.0.0'
   hash:
-    md5: 5a544130e584b1f204ac896ff071d5b3
-    sha256: 42ae06bbb3cf7f7c3194482894f4287fad7bc39214d1a0dbf0c43f8efb8d3c1a
+    md5: 209e462211f65827cdc01a0d7a72286f
+    sha256: b33deb1bab5fb8f1dbf47a53f3b7352e288427554545157029c084dc27e862a4
   manager: conda
   name: libgfortran5
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda
-  version: 12.2.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.3.0-hbd3c1fe_1.conda
+  version: 12.3.0
 - category: main
   dependencies:
     libcxx: '>=12.a0'
     libzlib: '>=1.2.11,<1.3.0a0'
   hash:
     md5: bac1c6f12f44f40e19274e6e04e9bad5
     sha256: ea05949ee38b51fd6391c57ec8365e41737108d24e5ff2266da3c6d3b20c3a23
@@ -7505,22 +8262,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/openh264-2.3.1-hf0c8a7f_2.conda
   version: 2.3.1
 - category: main
   dependencies:
     ca-certificates: ''
   hash:
-    md5: c7822d6ee74e34af1fd74365cfd18983
-    sha256: 67855f92bf50f24cbbc44879864d7a040b1f351e95b599cfcf4cc49b2cc3fd08
+    md5: 85d5377436d19183c8ac5afbb8e713a1
+    sha256: 5d28695e086e69150e0b674f11ad87df603870fb3256bd590e305b708fc1faf7
   manager: conda
   name: openssl
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda
-  version: 3.1.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.2-h8a1eda9_0.conda
+  version: 3.1.2
 - category: main
   dependencies:
     libffi: '>=3.4.2,<3.5.0a0'
     libtasn1: '>=4.18.0,<5.0a0'
   hash:
     md5: e936a0ee28be948846108582f00e2d61
     sha256: e16fbaadb2714c0965cb76de32fe7d13a21874cec02c97efef8ac51f4fda86fc
@@ -7601,24 +8358,24 @@
   name: svt-av1
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/svt-av1-1.4.1-hf0c8a7f_0.conda
   version: 1.4.1
 - category: main
   dependencies:
-    libcxx: '>=14.0.6'
+    libcxx: '>=15.0.7'
   hash:
-    md5: 6aedf8fdcdf5f2d7b4db21853a7d42ed
-    sha256: c778c2e7ba7573dcbb6002fdc6ab357f8e1cd63e1c39329af202233814a26fb8
+    md5: 7d866c2f94d867282a403460cfa8b3f8
+    sha256: a2d9591c90cd19559c8e704dddc559ebcaebf0718f6e5a2ad00135a5e4b7ad0b
   manager: conda
   name: tbb
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/tbb-2021.9.0-hb8565cd_0.conda
-  version: 2021.9.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/tbb-2021.10.0-h1c7c39f_0.conda
+  version: 2021.10.0
 - category: main
   dependencies:
     libzlib: '>=1.2.11,<1.3.0a0'
   hash:
     md5: 8e9480d9c47061db2ed1b4ecce519a7f
     sha256: 331aa1137a264fd9cc905f04f09a161c801fe504b93da08b4e6697bd7c9ae6a6
   manager: conda
@@ -7754,36 +8511,36 @@
   name: krb5
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda
   version: 1.20.1
 - category: main
   dependencies:
-    libcxx: '>=15.0.7'
+    libcxx: '>=16.0.6'
     libllvm13: '>=13.0.1,<13.1.0a0'
   hash:
-    md5: 7ffe2879ebb140302889d22a1ec41d84
-    sha256: 95d29fd75bf2d7930fdc458cf89eb55cc7702c5f6e1f282e66643e41057c745f
+    md5: 5d71eab2f706fb237a7023e04a6e4f73
+    sha256: 55e3894d23224dc93af5aef99978bdc0264fa102f5da6344701571ace18b6894
   manager: conda
   name: libclang
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libclang-13.0.1-default_h255f2f3_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libclang-13.0.1-root_62804_h2961583_3.conda
   version: 13.0.1
 - category: main
   dependencies:
-    libgfortran5: ''
+    libgfortran5: 12.3.0 hbd3c1fe_1
   hash:
-    md5: 97451338600bd9c5b535eb224ef6c471
-    sha256: 55d3c81ce8cd931260c3cb8c85868e36223d2bd0d5e2f35a79503810ee172769
+    md5: 3dfbc4ce09c598763cffcc667686f412
+    sha256: 096794b8155e4b5f9745b18e0a8ba2f9bde3dcf1bdf334d6077ff7937eed7fd5
   manager: conda
   name: libgfortran
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-12_3_0_h97931a8_1.conda
   version: 5.0.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     libcxx: '>=15.0.7'
     libffi: '>=3.4,<4.0a0'
     libiconv: '>=1.17,<2.0a0'
@@ -8004,25 +8761,25 @@
   name: sqlite
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.42.0-h2b0dec6_0.conda
   version: 3.42.0
 - category: main
   dependencies:
-    libcxx: '>=14.0.6'
-    tbb: 2021.9.0 hb8565cd_0
+    libcxx: '>=15.0.7'
+    tbb: 2021.10.0 h1c7c39f_0
   hash:
-    md5: 23fd9e2cb5478ed8b6ba925a741af61b
-    sha256: 31862cb9ee2f694ab7b5810916b10ff61897c21abce3259bebd7277972ccd076
+    md5: 3f66beb4d0e5cab00d6629ed7a77a062
+    sha256: ed896d1bd633bfb8bf7b6af1ade8ac8882e8209216d6d28fac02b5811d566472
   manager: conda
   name: tbb-devel
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/tbb-devel-2021.9.0-hb8565cd_0.conda
-  version: 2021.9.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/tbb-devel-2021.10.0-h1c7c39f_0.conda
+  version: 2021.10.0
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
     md5: dd5eed01874c75bebef810a2faec673e
     sha256: 1cc3eb4ee86271dfcfb0673cb7aa2632e43024b7f1324ca23689dcfbe0631b2f
   manager: conda
@@ -8041,14 +8798,26 @@
   name: alabaster
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda
   version: 0.7.13
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: 5f095bc6454094e96f146491fd03633b
+    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
+  manager: conda
+  name: appdirs
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
+  version: 1.4.4
+- category: main
+  dependencies:
     python: '>=2.7'
   hash:
     md5: 54ac328d703bff191256ffa1183126d1
     sha256: b209a68ac55eb9ecad7042f0d4eedef5da924699f6cdf54ac1826869cfdae742
   manager: conda
   name: appnope
   optional: false
@@ -8114,50 +8883,74 @@
   name: blinker
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda
   version: 1.6.2
 - category: main
   dependencies:
+    python: 2.7.*|>=3.7
+  hash:
+    md5: 033eb25fffd222aceeca6d58cd953680
+    sha256: 4ff828cceb8f55cb26d23b1a4c174d22c7cd92350221724bcaf2d6632e33fdee
+  manager: conda
+  name: boltons
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/boltons-23.0.0-pyhd8ed1ab_0.conda
+  version: 23.0.0
+- category: main
+  dependencies:
     brotli-bin: 1.0.9 hb7f2c08_9
     libbrotlidec: 1.0.9 hb7f2c08_9
     libbrotlienc: 1.0.9 hb7f2c08_9
   hash:
     md5: 53cff90f0cea22e13e5b791f0e5a8e7d
     sha256: eb425d4075f90d90bf9de5c2e8f88fe783d70177fcdfd3d3da5ef48e444ca148
   manager: conda
   name: brotli
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda
   version: 1.0.9
 - category: main
   dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 576d629e47797577ab0f1b351297ef4a
+    sha256: 6dbf7a5070cc43d90a1e4c2ec0c541c69d8e30a0e25f50ce9f6e4a432e42c5d7
+  manager: conda
+  name: cached_property
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 60b5eb16d9a7a5482ba37f67aa49db5b
     sha256: 8d30a41a88900730c748f5b296730a0d48e5cfa2c8b260aab60fa9f26ffafcc0
   manager: conda
   name: cachetools
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda
   version: 5.3.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 5d1b71c942b8421285934dad1d891ebc
-    sha256: f839a6e04d94069f90dd85337ea9108f058dc76771bb469a413f32bb1ba0b256
+    md5: 7f3dbc9179b4dde7da98dfb151d0ad22
+    sha256: db66e31866ff4250c190788769e3a8a1709237c3e9c38d7143aae95ab75fcb31
   manager: conda
   name: certifi
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda
-  version: 2023.5.7
+  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.7.22-pyhd8ed1ab_0.conda
+  version: 2023.7.22
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 313516e9a4b08b12dfb1e1cd390a96e3
     sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   manager: conda
@@ -8189,14 +8982,26 @@
   name: colorama
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
   version: 0.4.6
 - category: main
   dependencies:
+    python: '>=3.6,<4.0'
+  hash:
+    md5: 709a2295dd907bb34afb57d54320642f
+    sha256: 2f05954a3faf0700c14c1deddc085385160ee32abe111699c78d9cb277e915cc
+  manager: conda
+  name: crashtest
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.4.1
+- category: main
+  dependencies:
     python: '>=3.6'
   hash:
     md5: a50559fad0affdbb33729a68669ca1cb
     sha256: 3b594bc8aa0b9a51269d54c7a4ef6af777d7fad4bee16b05695e1124de6563f6
   manager: conda
   name: cycler
   optional: false
@@ -8213,26 +9018,26 @@
   name: dataclasses
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2
   version: '0.8'
 - category: main
   dependencies:
-    libcxx: '>=14.0.6'
+    libcxx: '>=15.0.7'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 549f7722839c44ee8a859fc0b94a5884
-    sha256: 103c7c29afd44fc4a5a94e999be1ff26ec6cde6a2814732095e4b40bbf90968f
+    md5: 1cf76f1cacf74894e317a4aa4da54cf7
+    sha256: ea6dc2e2a44528153792c48d50e20e2108dbcce6c3848df852690b9cb287d2af
   manager: conda
   name: debugpy
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py310h7a76584_0.conda
-  version: 1.6.7
+  url: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.8-py310h9e9d8ca_0.conda
+  version: 1.6.8
 - category: main
   dependencies:
     python: '>=3.5'
   hash:
     md5: 43afe5ab04e35e17ba28649471dd7364
     sha256: 328a6a379f9bdfd0230e51de291ce858e6479411ea4b0545fb377c71662ef3e2
   manager: conda
@@ -8251,14 +9056,26 @@
   name: defusedxml
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2
   version: 0.7.1
 - category: main
   dependencies:
+    python: 2.7|>=3.6
+  hash:
+    md5: 12d8aae6994f342618443a8f05c652a0
+    sha256: 13c887cb4a29e1e853a118cfc0e42b72a7e1d1c50c66c0974885d37f0db30619
+  manager: conda
+  name: distlib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda
+  version: 0.3.7
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 69b3569d320b0fc940449fcc25b01e31
     sha256: 128bb3316102708225932a5fb1fc7f2d1900055fae2fc7ef237025d5b53a1348
   manager: conda
   name: docutils
@@ -8513,14 +9330,26 @@
   name: jmespath
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2
   version: 1.0.1
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: 07d85c22a3beb102a48cd123df84c2a6
+    sha256: da279af2285d8f575a7f5652e83bf7f36155c4c63154e385a9d171efcc607bc1
+  manager: conda
+  name: jsonpointer
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonpointer-2.0-py_0.tar.bz2
+  version: '2.0'
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 2bc3ca2f7387af385dd06706b4fb2d35
     sha256: 0781ed7a4f35ff1309e95381c40c8d8f96263ca4260a72baaafda87c975a972a
   manager: conda
   name: jupyterlab_widgets
   optional: false
@@ -8643,14 +9472,26 @@
   name: libwebp
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libwebp-1.2.4-hfa4350a_0.tar.bz2
   version: 1.2.4
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: c104d98e09c47519950cffb8dd5b4f10
+    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
+  manager: conda
+  name: lockfile
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
+  version: 0.12.2
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 632a71feccc9f651c844c402efe61884
     sha256: cfba42cf3992305d44a3f80e39f0c8fc39a110307e6f2d7ff6ab42a6c8b1a1a1
   manager: conda
   name: loguru
@@ -8718,14 +9559,26 @@
   name: mkl-devel
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/mkl-devel-2022.1.0-h694c41f_929.tar.bz2
   version: 2022.1.0
 - category: main
   dependencies:
+    python: '>=3.8'
+  hash:
+    md5: 8549fafed0351bbfaa1ddaa15fdf9b4e
+    sha256: 07ce65497dec537e490992758934ddbc4fb5ed9285b41387a7cca966f1a98a0f
+  manager: conda
+  name: more-itertools
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.1.0-pyhd8ed1ab_0.conda
+  version: 10.1.0
+- category: main
+  dependencies:
     gmp: '>=6.2.1,<7.0a0'
     mpfr: '>=4.1.0,<5.0a0'
   hash:
     md5: c752c0eb6c250919559172c011e5f65b
     sha256: 2ae945a15c8a984d581dcfb974ad3b5d877a6527de2c95a3363e6b4490b2f312
   manager: conda
   name: mpc
@@ -8743,14 +9596,28 @@
   name: mpmath
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda
   version: 1.3.0
 - category: main
   dependencies:
+    libcxx: '>=14.0.6'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: eaca50d68ad312e2930b2f9eca8756ef
+    sha256: bdc32bff84d9d757092ca2d8683cdb019bb29f8e7ecfe8b687aa9c3b5c589997
+  manager: conda
+  name: msgpack-python
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py310ha23aa8a_0.conda
+  version: 1.0.5
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 0324181c4442d94c865cf9ae3b6a7fea
     sha256: 27d1eed1ba91e6e7ea6221ef7abe020924ac4d7c55d98f40c7841aa492744696
   manager: conda
   name: multidict
@@ -8873,22 +9740,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2
   version: 0.8.3
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: dbb80d1e8dc2dba5c8b106dc0768ad45
-    sha256: d94463e0a140ead5c01990b565a1a21b85cb3831d56fed5955b5446bd5df33fe
+    md5: e41debb259e68490e3ab81e46b639ab6
+    sha256: 7bcfa6d86359d45572ba9ccaeaedc04b0452e2654fe44b6fe378d0d37b8745e1
   manager: conda
   name: pathspec
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda
-  version: 0.11.1
+  url: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.2-pyhd8ed1ab_0.conda
+  version: 0.11.2
 - category: main
   dependencies:
     python: '>=3'
   hash:
     md5: 415f0ebb6198cc2801c73438a9fb5761
     sha256: a1ed1a094dd0d1b94a09ed85c283a0eb28943f2e6f22161fb45e128d35229738
   manager: conda
@@ -8897,14 +9764,26 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
   version: 0.7.5
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
+    md5: be1e9f1c65a1ed0f2ae9352fec99db64
+    sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
+  manager: conda
+  name: pkginfo
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
+  version: 1.9.6
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
     md5: 89e3c7cdde7d3aaa2aee933b604dd07f
     sha256: 7d055ffc8a02bf781a89d069db3454b453605cdaff300b82cedcc7133283e47e
   manager: conda
   name: pkgutil-resolve-name
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2
@@ -9004,14 +9883,27 @@
   name: pycodestyle
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda
   version: 2.10.0
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 95c032c354c500001a935aac4c059376
+    sha256: 28012e6ae66102b9b4f69316d026985373b2c33161304bc6841c1d9c3f9ec34e
+  manager: conda
+  name: pycosat
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pycosat-0.6.4-py310h90acd4f_1.tar.bz2
+  version: 0.6.4
+- category: main
+  dependencies:
     python: 2.7.*|>=3.4
   hash:
     md5: 076becd9e05608f8dc72757d5f3a91ff
     sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
   manager: conda
   name: pycparser
   optional: false
@@ -9092,22 +9984,34 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
   version: 1.7.1
 - category: main
   dependencies:
     python: '>=3.3'
   hash:
-    md5: dd4f393d857e9283eef2442234bd05e3
-    sha256: b7a8b9b2310b3ee74ba99eef9692e477bb8bddf110eff45784dee7d81a693455
+    md5: 3be9466311564f80f8056c0851fc5bb7
+    sha256: 73985a9a2dd7ccf77b7428a12148e1b381c8635e9195e47a652397e9a56284ce
   manager: conda
   name: python-fastjsonschema
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda
-  version: 2.17.1
+  url: https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.18.0-pyhd8ed1ab_0.conda
+  version: 2.18.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 65dea78f903d686c8b0c2feaf0e15e1f
+    sha256: 822f95b7786cfa61a6519153117b21d93194890e02a884b9f66ee4275e4f1c0a
+  manager: conda
+  name: python-installer
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/python-installer-0.7.0-pyhd8ed1ab_0.conda
+  version: 0.7.0
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
     md5: a61bf9ec79426938ff785eb69dbb1960
     sha256: 4790787fe1f4e8da616edca4acf6a4f8ed4e7c6967aa31b920208fc8f95efcca
   manager: conda
@@ -9193,14 +10097,26 @@
   name: setuptools
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
   version: 67.7.2
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 1de44299f48f522caa2e0074231614e1
+    sha256: 3cb4a4a83b617fdfef9b92751634488db0b8961c80340be8068bf6d4f1d5ac25
+  manager: conda
+  name: shellingham
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.1-pyhd8ed1ab_0.conda
+  version: 1.5.1
+- category: main
+  dependencies:
     python: ''
   hash:
     md5: e5f25f8dbc060e9a8d912e432202afc2
     sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
   manager: conda
   name: six
   optional: false
@@ -9363,14 +10279,38 @@
   name: tomli
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
   version: 2.0.1
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 62f5b331c53d73e2f6c4c130b53518a0
+    sha256: dc4abf58ca42f29e12b8c0f8aadedfca49cc1e97dab025d15cf000b1787df773
+  manager: conda
+  name: tomlkit
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.1-pyha770c72_0.conda
+  version: 0.12.1
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 92facfec94bc02d6ccf42e7173831a36
+    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
+  manager: conda
+  name: toolz
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.12.0
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 369ce2c5cd18205e4917f515b4052376
     sha256: 732d346b83daf57ba80897a5db6cd14bf1152aa6576085552b2ed465be05aec1
   manager: conda
   name: tornado
@@ -9388,27 +10328,51 @@
   name: traitlets
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda
   version: 5.9.0
 - category: main
   dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c9918f6a3973e28a792e747289734cd3
+    sha256: a3b13371ece96434028c9c4cc5561d3a04afdb26165290b630578c1d00b462f7
+  manager: conda
+  name: trove-classifiers
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2023.7.6-pyhd8ed1ab_0.conda
+  version: 2023.7.6
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 189bf6e55cac449f8b34763502b18385
     sha256: eb18f777f51b490ccadf41363bc95fbbac62575b2067f1c2027633b4313a3f0d
   manager: conda
   name: typed-ast
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/typed-ast-1.5.4-py310h90acd4f_1.tar.bz2
   version: 1.5.4
 - category: main
   dependencies:
+    python: '>=3'
+  hash:
+    md5: e6573ac68718f17b9d4f5c8eda3190f2
+    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
+  manager: conda
+  name: typing
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.10.0.0
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: c39d6a09fe819de4951c2642629d9115
     sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   manager: conda
   name: typing_extensions
   optional: false
@@ -9462,14 +10426,38 @@
   name: unidecode
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2
   version: 1.3.6
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 0944dc65cb4a9b5b68522c3bb585d41c
+    sha256: b76904b53721dc88a46352324c79d2b077c2f74a9f7208ad2c4249892669ae94
+  manager: conda
+  name: uri-template
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda
+  version: 1.3.0
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 166212fe82dad8735550030488a01d03
+    sha256: 6e097d5fe92849ad3af2c2a313771ad2fbf1cadd4dc4afd552303b2bf3f85211
+  manager: conda
+  name: webcolors
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda
+  version: '1.13'
+- category: main
+  dependencies:
     python: ''
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   manager: conda
   name: webencodings
   optional: false
@@ -9488,22 +10476,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: c95fac682453aeffa12db7ae5a721bec
-    sha256: e91cbb3c0ad9a9507dd030f5493831cb52da120329e0d0793711e8300a36db22
+    md5: 66beb36a1fa7e0dc9d9bf843a80eb82c
+    sha256: c35e6b6c8100e9e42ed0968aef99680b1d1ec5358d4ca0d2b2175f68c6b21dd6
   manager: conda
   name: wheel
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda
-  version: 0.40.0
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.41.0-pyhd8ed1ab_0.conda
+  version: 0.41.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 2e9ebddf0b93d0fb203d0906b8052c4f
     sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
   manager: conda
@@ -9603,14 +10591,27 @@
   name: babel
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda
   version: 2.12.1
 - category: main
   dependencies:
+    python: '>=3.6'
+    typing: '>=3.6'
+  hash:
+    md5: 0e1df3978dd516e20ef88c86d51e5432
+    sha256: 1d86eafb5e9ed078f891e12b46692d786723652907dfb01b047c7da31f92b862
+  manager: conda
+  name: backports.cached-property
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/backports.cached-property-1.0.2-pyhd8ed1ab_0.tar.bz2
+  version: 1.0.2
+- category: main
+  dependencies:
     backports: ''
     python: '>=3.6'
     setuptools: ''
   hash:
     md5: 6b1b907661838a75d067a22f87996b2e
     sha256: 7027bb689dd4ca4a08e3b25805de9d04239be6b31125993558f21f102a9d2700
   manager: conda
@@ -9646,14 +10647,26 @@
   name: bleach
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda
   version: 6.0.0
 - category: main
   dependencies:
+    cached_property: '>=1.5.2,<1.5.3.0a0'
+  hash:
+    md5: 9b347a7ec10940d3f7941ff6c460b551
+    sha256: 561e6660f26c35d137ee150187d89767c988413c978e1b712d53f27ddf70ea17
+  manager: conda
+  name: cached-property
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
     fontconfig: '>=2.13.96,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
     icu: '>=70.1,<71.0a0'
     libglib: '>=2.72.1,<3.0a0'
     libpng: '>=1.6.38,<1.7.0a0'
     libzlib: '>=1.2.12,<1.3.0a0'
@@ -9681,25 +10694,38 @@
   name: cffi
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310ha78151a_3.conda
   version: 1.15.1
 - category: main
   dependencies:
+    click: ''
+    python: '>=3.6'
+  hash:
+    md5: 72a46ffc25701c173932fd55cf0965d3
+    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
+  manager: conda
+  name: click-default-group
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.2
+- category: main
+  dependencies:
     python: '>=3.6'
     traitlets: '>=5.3'
   hash:
-    md5: 168ae0f82cdf7505048e81054c7354e4
-    sha256: 657e0a513c8705dc542c54c4c5234e813b7f4e2f412688796d611e83ddf132ea
+    md5: c8eaca39e2b6abae1fc96acc929ae939
+    sha256: 11057745946a95ee7cc4c98900a60c7362266a4cb28bc97d96cd88e3056eb701
   manager: conda
   name: comm
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda
-  version: 0.1.3
+  url: https://conda.anaconda.org/conda-forge/noarch/comm-0.1.4-pyhd8ed1ab_0.conda
+  version: 0.1.4
 - category: main
   dependencies:
     krb5: '>=1.20.1,<1.21.0a0'
     libcurl: 8.1.2 hbee3ae8_0
     libssh2: '>=1.10.0,<2.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.0,<4.0a0'
@@ -9787,22 +10813,22 @@
   dependencies:
     brotli: ''
     munkres: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     unicodedata2: '>=14.0.0'
   hash:
-    md5: 2de0c6bd77a2ea8aa4e82943273c5dd3
-    sha256: 76ae3255902589a8076f76b4821c3e47e6622af9b2a8aba5ce432da5bc848632
+    md5: f23e7e0fd82662cc9ddd8124ef45d5b4
+    sha256: 82771cfc1d8aa7249b8d53f3f29bab9025c10134128936d231dd9c16e28240cb
   manager: conda
   name: fonttools
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.41.0-py310h6729b98_0.conda
-  version: 4.41.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.42.0-py310h6729b98_0.conda
+  version: 4.42.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     glib-tools: 2.76.4 h7d26f99_0
     libcxx: '>=15.0.7'
     libglib: 2.76.4 hc62aa5d_0
     libzlib: '>=1.2.13,<1.3.0a0'
@@ -9865,14 +10891,28 @@
   name: hdf5
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.12.2-nompi_h48135f9_101.conda
   version: 1.12.2
 - category: main
   dependencies:
+    python: ''
+    six: '>=1.9'
+    webencodings: ''
+  hash:
+    md5: b2355343d6315c892543200231d7154a
+    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
+  manager: conda
+  name: html5lib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
+  version: '1.1'
+- category: main
+  dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
   hash:
     md5: 4e9f59a060c3be52bc4ddc46ee9b6946
     sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   manager: conda
   name: importlib-metadata
@@ -9891,25 +10931,38 @@
   name: importlib_resources
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda
   version: 6.0.0
 - category: main
   dependencies:
+    more-itertools: ''
+    python: '>=3.7'
+  hash:
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
+  manager: conda
+  name: jaraco.classes
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
+  version: 3.3.0
+- category: main
+  dependencies:
     parso: '>=0.8.0,<0.9.0'
     python: '>=3.6'
   hash:
-    md5: b5e695ef9c3f0d27d6cd96bf5adc9e07
-    sha256: abe63ae6e1b13f83500608d94004cb8d485b264083511d77f79253e775cd546c
+    md5: 1cd7f70057cdffc10977b613fb75425d
+    sha256: d2d9e885cbc1efa63107b616588c61000063d4c223c0585962485bd016e77ce8
   manager: conda
   name: jedi
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda
-  version: 0.18.2
+  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.0-pyhd8ed1ab_0.conda
+  version: 0.19.0
 - category: main
   dependencies:
     markupsafe: '>=2.0'
     python: '>=3.7'
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
@@ -9917,14 +10970,27 @@
   name: jinja2
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   version: 3.1.2
 - category: main
   dependencies:
+    jsonpointer: '>=1.9'
+    python: '>=3.6'
+  hash:
+    md5: 09150b51b0528a31a0f6500b96fdde82
+    sha256: d87fd8da2d3327744821b6b1d1e5b76e4077224fb626ce02d6623a1bc6ee2563
+  manager: conda
+  name: jsonpatch
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonpatch-1.32-pyhd8ed1ab_0.tar.bz2
+  version: '1.32'
+- category: main
+  dependencies:
     pygments: '>=2.4.1,<3'
     python: '>=3.7'
   hash:
     md5: 243f63592c8e449f40cd42eb5cf32f40
     sha256: 08453e09d5a6bbaeeca839553a5dfd7a377a97550efab96019c334a8042f54f5
   manager: conda
   name: jupyterlab_pygments
@@ -10286,22 +11352,22 @@
     libcxx: '>=15.0.7'
     packaging: ''
     ply: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tomli: ''
   hash:
-    md5: 5aae43762f6fe7bbdd3e0e2bbd567999
-    sha256: f6ebbdc44064289812091840d0a2ec06fb2af485a264a2a37057404aeb79be90
+    md5: 985292668e418bea78567353d03098db
+    sha256: 761d8ad81b2a9bf1788efcba339b87ece87ad6bbd83f488c4d70b063727ee9d2
   manager: conda
   name: sip
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/sip-6.7.9-py310h9e9d8ca_0.conda
-  version: 6.7.9
+  url: https://conda.anaconda.org/conda-forge/osx-64/sip-6.7.11-py310h9e9d8ca_0.conda
+  version: 6.7.11
 - category: main
   dependencies:
     __osx: ''
     ptyprocess: ''
     python: '>=3.7'
     tornado: '>=6.1.0'
   hash:
@@ -10377,28 +11443,55 @@
   name: yarl
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/yarl-1.9.2-py310h6729b98_0.conda
   version: 1.9.2
 - category: main
   dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  manager: conda
+  name: annotated-types
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  version: 0.5.0
+- category: main
+  dependencies:
     cffi: '>=1.0.1'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 952166ee5ce75092167a7385a4e243e3
     sha256: 6b8ca16921f72b82aa3ad16a1c7a46e35cbcccec59c1b6eb3f53fa748f59b548
   manager: conda
   name: argon2-cffi-bindings
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py310h90acd4f_3.tar.bz2
   version: 21.2.0
 - category: main
   dependencies:
+    python: '>=3.6'
+    python-dateutil: '>=2.7.0'
+    typing_extensions: ''
+  hash:
+    md5: fd1967c76eda3a3dd9e8e6cb7a15a028
+    sha256: a0434c2770cf5b0ab5a33913c0b202b1521bc13f755b762d16a86b110425cdc2
+  manager: conda
+  name: arrow
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/arrow-1.2.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.2.3
+- category: main
+  dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.0.0'
     wrapt: <2,>=1.11
   hash:
     md5: 2812b75db400abe651a33b99a7173ee6
@@ -10449,41 +11542,54 @@
   name: cryptography
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.2-py310ha1817de_0.conda
   version: 41.0.2
 - category: main
   dependencies:
+    cached-property: '>=1.3.0'
+    python: '>=2.7,<4'
+  hash:
+    md5: 642d35437078749ef23a5dca2c9bb1f3
+    sha256: 6cfd1f9bcd2358a69fb571f4b3af049b630d52647d906822dbedac03e84e4f63
+  manager: conda
+  name: fqdn
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2
+  version: 1.5.1
+- category: main
+  dependencies:
     python: '>=3.6'
     python-dateutil: '>=2.8.1'
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
   manager: conda
   name: ghp-import
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   version: 2.1.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    glib: '>=2.76.3,<3.0a0'
+    glib: '>=2.76.4,<3.0a0'
     libcxx: '>=15.0.7'
-    libglib: '>=2.76.3,<3.0a0'
+    libglib: '>=2.76.4,<3.0a0'
     libiconv: '>=1.17,<2.0a0'
   hash:
-    md5: 659321735840756bc2c6ba7195ed9d8b
-    sha256: 362e945e55e729d11351b760622d25049272178ef1dc6f74c5d7e518ca3f2ed3
+    md5: 34b61e048ab804e3699fc449a4884fce
+    sha256: fa2c01670cbc6aba96e0bd23a3385abfc8e32de84ab225a4bd6436b7d89b39c4
   manager: conda
   name: gstreamer
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_1.conda
-  version: 1.22.4
+  url: https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.5-h840fbdc_0.conda
+  version: 1.22.5
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     freetype: '>=2.12.1,<3.0a0'
     graphite2: ''
     icu: '>=70.1,<71.0a0'
     libcxx: '>=14.0.6'
@@ -10597,22 +11703,22 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.8.1-nompi_hc61b76e_106.tar.bz2
   version: 4.8.1
 - category: main
   dependencies:
     importlib-metadata: '>=4.4'
     python: '>=3.6'
   hash:
-    md5: 89ed59ad509c05db6f5f2f573d499bfe
-    sha256: e32ac2c95112caa8cd81f0cbc710f4f4903180a115c7260f03b010d5a0aa771b
+    md5: 6b8ab17bc8ff1ca89b3ea28ea3d566ca
+    sha256: cf1b3778cf99bd0301c4eb4f5d3d575e8c4248c15a019189b3892131a2675854
   manager: conda
   name: markdown
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda
-  version: 3.4.3
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.4-pyhd8ed1ab_0.conda
+  version: 3.4.4
 - category: main
   dependencies:
     markdown-it-py: '>=1.0.0,<4.0.0'
     python: '>=3.8'
   hash:
     md5: 6c5358a10873a15398b6f15f60cb5e1f
     sha256: 1ddac8d2be448cd1fbe49d2ca09df7e10d99679d53146a917f8bb4899f76d0ca
@@ -10627,35 +11733,48 @@
     libblas: '>=3.9.0,<4.0a0'
     libcblas: '>=3.9.0,<4.0a0'
     libcxx: '>=15.0.7'
     liblapack: '>=3.9.0,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 525db32fd93b63f2f7ca3ece8576b9c8
-    sha256: 32fe99f86e998169999514fb7f96695fdec9215bd0e7061425c1b4e399ca2cae
+    md5: a0f919ff93f102cb1720f71448010c61
+    sha256: 77dbf044b2b9149e2038fdc4e99bacbff5e6163136abf84c3f94bbc438ead546
   manager: conda
   name: numpy
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.1-py310h7451ae0_0.conda
-  version: 1.25.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.2-py310h7451ae0_0.conda
+  version: 1.25.2
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 044e7a1e0ad42c4e67110bd078150a63
-    sha256: 885611bd528abaf3e31bc0bfaad3a619cfe89db61d886b53c2a9ec9ff50edebe
+    md5: 0809187ef9b89a3d94a5c24d13936236
+    sha256: 1b5c0ca2f4260c7dd8cfccd8a641c1e41876c79dc594506be379cde08f5b471e
   manager: conda
   name: platformdirs
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda
-  version: 3.9.1
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.10.0-pyhd8ed1ab_0.conda
+  version: 3.10.0
+- category: main
+  dependencies:
+    importlib-metadata: '>=1.7.0'
+    python: '>=3.7'
+  hash:
+    md5: a6d1f61527c27fcc0165a6701a46b9f4
+    sha256: 6f6a66476908a1c109e36c852d934eedceb07e0cbc44d3fcd87c6f39521b57be
+  manager: conda
+  name: poetry-core
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-core-1.6.1-pyhd8ed1ab_0.conda
+  version: 1.6.1
 - category: main
   dependencies:
     latexcodec: '>=1.0.4'
     python: '>=3.6'
     pyyaml: '>=3.01'
     setuptools: ''
     six: ''
@@ -10666,14 +11785,28 @@
   name: pybtex
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2
   version: 0.24.0
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    typing-extensions: '>=4.6.0'
+  hash:
+    md5: 697e1a00773e5bc8232e862b5ae76186
+    sha256: d7876275e04618798f0d1d74a0d322a069af964a41dd1b353dc20ed3f4e4dca0
+  manager: conda
+  name: pydantic-core
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.4.0-py310h3461e44_0.conda
+  version: 2.4.0
+- category: main
+  dependencies:
     libffi: '>=3.4,<4.0a0'
     pyobjc-core: 9.2.*
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 0874355241e82a01cd15c6e6b28c7187
     sha256: c9f10735105782a85b077d30cf5933eff7821bf70a806526b8bca3077c5ae057
@@ -10681,29 +11814,29 @@
   name: pyobjc-framework-cocoa
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py310hef2d279_0.conda
   version: '9.2'
 - category: main
   dependencies:
-    libcxx: '>=14.0.6'
+    libcxx: '>=15.0.7'
     packaging: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     sip: ''
     toml: ''
   hash:
-    md5: 6c56916bf99c55b1f57a53ed689f2561
-    sha256: c03844f8939bc8d02f902b2b5e0cede89177739ff7db1295363b33dc23ee8e8d
+    md5: 1b383c6ab90e71d5429104a1573d25f3
+    sha256: 67f82f305d81682e5c84b45bbdb953620be09fa0523608dbb5f2c63b9829113f
   manager: conda
   name: pyqt5-sip
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyqt5-sip-12.11.0-py310h415000c_3.conda
-  version: 12.11.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyqt5-sip-12.12.2-py310h018f80b_4.conda
+  version: 12.12.2
 - category: main
   dependencies:
     colorama: ''
     importlib-metadata: '>=0.22'
     packaging: '>=19.0'
     pyproject_hooks: ''
     python: '>=3.7'
@@ -10789,14 +11922,43 @@
   name: wcwidth
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda
   version: 0.2.6
 - category: main
   dependencies:
+    cffi: '>=1.0.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: d267890f1fba643f1803d7ce417e20b9
+    sha256: 7d5706e6067dc81238c8410945565f223146d73c6d44d2218b6d9a6204e0d5be
+  manager: conda
+  name: xattr
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/xattr-0.10.1-py310h90acd4f_0.conda
+  version: 0.10.1
+- category: main
+  dependencies:
+    cffi: '>=1.11'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: 8bd43a6390a6905fbc0dd14883fd3166
+    sha256: b5c1008e8d933de908924be48d0790809569169b1991bbc4bd70dc86aeb901c7
+  manager: conda
+  name: zstandard
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.19.0-py310h151724a_2.conda
+  version: 0.19.0
+- category: main
+  dependencies:
     aiosignal: '>=1.1.2'
     async-timeout: <5.0,>=4.0.0a3
     attrs: '>=17.3.0'
     charset-normalizer: '>=2.0,<4.0'
     frozenlist: '>=1.1.1'
     multidict: '>=4.5,<7.0'
     python: '>=3.10,<3.11.0a0'
@@ -10860,14 +12022,27 @@
   name: blas-devel
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/blas-devel-3.9.0-17_osx64_mkl.conda
   version: 3.9.0
 - category: main
   dependencies:
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 38253361efb303deead3eab39ae9269b
+    sha256: 654a2488f77bf43555787d952dbffdc5d97956ff4aa9e0414a7131bb741dcf4c
+  manager: conda
+  name: conda-package-streaming
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.9.0-pyhd8ed1ab_0.conda
+  version: 0.9.0
+- category: main
+  dependencies:
     libcxx: '>=15.0.7'
     numpy: '>=1.16'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 0cfd4a8d0f1d785675d5e41e17c8b122
     sha256: 24d649ccfeeb6b0ffff6fb315a8794ccedba2b0d6fbc8a3f80aeb99cdbad7d00
@@ -10876,31 +12051,44 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py310h88cfcbd_0.conda
   version: 1.1.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    gstreamer: 1.22.4 h840fbdc_1
+    gstreamer: 1.22.5 h840fbdc_0
     libcxx: '>=15.0.7'
-    libglib: '>=2.76.3,<3.0a0'
+    libglib: '>=2.76.4,<3.0a0'
     libogg: '>=1.3.4,<1.4.0a0'
     libopus: '>=1.3.1,<2.0a0'
     libpng: '>=1.6.39,<1.7.0a0'
     libvorbis: '>=1.3.7,<1.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 504bc1e992fc2d59e55cbd0102e117b0
-    sha256: ade088cd9e124e033f56926ab97012a9a0af186251d7d904005476900eb3da9d
+    md5: b352c9e0490352a101e6299daa98196b
+    sha256: 587ae78fa8a0798d59f9dc51ad86c306138edda571592eb955516d0677ad93b7
   manager: conda
   name: gst-plugins-base
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_1.conda
-  version: 1.22.4
+  url: https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.5-hb5d3a86_0.conda
+  version: 1.22.5
+- category: main
+  dependencies:
+    arrow: '>=0.15.0'
+    python: '>=3.7'
+  hash:
+    md5: 4cb68948e0b8429534380243d063a27a
+    sha256: 7bb5c4d994361022f47a807b5e7d101b3dce16f7dd8a0af6ffad9f479d346493
+  manager: conda
+  name: isoduration
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2
+  version: 20.11.0
 - category: main
   dependencies:
     platformdirs: '>=2.5'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     traitlets: '>=5.3'
   hash:
@@ -10910,30 +12098,27 @@
   name: jupyter_core
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py310h2ec42d9_0.conda
   version: 5.3.1
 - category: main
   dependencies:
-    jsonschema: '>=3.2'
-    python: '>=3.7'
-    python-json-logger: '>=2.0.4'
-    pyyaml: '>=5.3'
-    rfc3339-validator: ''
-    rfc3986-validator: '>=0.1.1'
-    traitlets: '>=5.3'
+    importlib_metadata: '>=4.11.4'
+    jaraco.classes: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
   hash:
-    md5: d98c5196ab6ffeb0c2feca2912801353
-    sha256: 16f73833537e05384d3eef27e62edb31de344d6d26666e1a465c1819014f2655
+    md5: 612970525fa53375995933f14718551c
+    sha256: e38f648c0fe236cc9d0d19dc9729acc463e74d1561ccebdea5a8789331714031
   manager: conda
-  name: jupyter_events
+  name: keyring
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda
-  version: 0.6.3
+  url: https://conda.anaconda.org/conda-forge/osx-64/keyring-23.13.1-py310h2ec42d9_0.conda
+  version: 23.13.1
 - category: main
   dependencies:
     numpy: '>=1.19'
     packaging: '>=17'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
@@ -10994,14 +12179,27 @@
   name: pango
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/pango-1.50.14-hbd9bf65_0.conda
   version: 1.50.14
 - category: main
   dependencies:
+    poetry-core: '>=1.6.0,<2.0.0'
+    python: '>=3.7,<4.0'
+  hash:
+    md5: 00893c7ea4f9f7620706e0aa94c01b6e
+    sha256: 54478b283b5967a85ee5da717f1512d7ec97eb07c7b52d1f2ad3cb080d56c0ac
+  manager: conda
+  name: poetry-plugin-export
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-plugin-export-1.4.0-pyhd8ed1ab_0.conda
+  version: 1.4.0
+- category: main
+  dependencies:
     python: '>=3.7'
     wcwidth: ''
   hash:
     md5: a4986c6bb5b0d05a38855b0880a5f425
     sha256: 10e7fdc75d4b85633be6b12a70b857053987127a808caa0f88b2cba4b3ce6359
   manager: conda
   name: prompt-toolkit
@@ -11023,27 +12221,57 @@
   name: pybtex-docutils
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py310h2ec42d9_2.tar.bz2
   version: 1.0.2
 - category: main
   dependencies:
+    annotated-types: '>=0.4.0'
+    pydantic-core: 2.4.0
+    python: '>=3.7'
+    typing-extensions: '>=4.6.1'
+  hash:
+    md5: 7964a624018707909044b509f58b937a
+    sha256: ee8a995c201e83421f3fb24f359c609900b8891d99331fc23dae32166931d744
+  manager: conda
+  name: pydantic
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.1.1-pyhd8ed1ab_0.conda
+  version: 2.1.1
+- category: main
+  dependencies:
     cryptography: '>=38.0.0,<42,!=40.0.0,!=40.0.1'
     python: '>=3.6'
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   manager: conda
   name: pyopenssl
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda
   version: 23.2.0
 - category: main
   dependencies:
+    libcxx: '>=14.0.6'
+    numpy: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: df0e628847158f0e1331b61f3aa04d84
+    sha256: 8abed1f40d6b82428eb7cbfeab8b7ca5937365394b10116d3e3f5e35866887be
+  manager: conda
+  name: rapidfuzz
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/rapidfuzz-2.15.1-py310h7a76584_0.conda
+  version: 2.15.1
+- category: main
+  dependencies:
     __osx: ''
     pyobjc-framework-cocoa: ''
     python: '>=3.6'
   hash:
     md5: 2657c3de5371c571aef6678afb4aaadd
     sha256: dca4022bae47618ed738ab7d45ead5202d174b741cfb98e4484acdc6e76da32a
   manager: conda
@@ -11066,14 +12294,29 @@
   name: simpleitk
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/simpleitk-2.2.1-py310h4447650_1.conda
   version: 2.2.1
 - category: main
   dependencies:
+    distlib: <1,>=0.3.7
+    filelock: <4,>=3.12.2
+    platformdirs: <4,>=3.9.1
+    python: '>=3.8'
+  hash:
+    md5: a218f3be8ab6185a475c8168a86e18ae
+    sha256: 3e508638077bcba79db4d26037c8e97bf6b7b43d156a06c9c25cdd2136468459
+  manager: conda
+  name: virtualenv
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.2-pyhd8ed1ab_0.conda
+  version: 20.24.2
+- category: main
+  dependencies:
     blas-devel: 3.9.0 17_osx64_mkl
     libblas: 3.9.0 17_osx64_mkl
     libcblas: 3.9.0 17_osx64_mkl
     libgfortran: 5.*
     libgfortran5: '>=12.2.0'
     liblapack: 3.9.0 17_osx64_mkl
     liblapacke: 3.9.0 17_osx64_mkl
@@ -11084,14 +12327,42 @@
   name: blas
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/blas-2.117-mkl.conda
   version: '2.117'
 - category: main
   dependencies:
+    crashtest: '>=0.4.1,<0.5.0'
+    python: '>=3.7,<4.0'
+    rapidfuzz: '>=2.2.0,<3.0.0'
+  hash:
+    md5: f1c5f2af6676cbe9206e191d1e70f661
+    sha256: cf9bc4c9356ad8eb68512446eebc076386f2bfb8ca86626e8796621bc5a13082
+  manager: conda
+  name: cleo
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cleo-2.0.1-pyhd8ed1ab_0.conda
+  version: 2.0.1
+- category: main
+  dependencies:
+    conda-package-streaming: '>=0.9.0'
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 8a3ae7f6318376aa08ea753367bb7dd6
+    sha256: 9a221808405d813d8c555efce6944379b907d36d79e77d526d573efa6b996d26
+  manager: conda
+  name: conda-package-handling
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.2.0-pyh38be061_0.conda
+  version: 2.2.0
+- category: main
+  dependencies:
     black: '>=22.1.0'
     flake8: '>=3'
     python: '>=3.7'
     tomli: ''
   hash:
     md5: 61649e6e9b39ac0c7d10938025f6fe4f
     sha256: 736dbadccbd0ce6371ffa011b761c03bf9e9d329582d0c5daecdbff0e96e2a36
@@ -11116,14 +12387,35 @@
   name: gtk2
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/gtk2-2.24.33-h7c1209e_2.tar.bz2
   version: 2.24.33
 - category: main
   dependencies:
+    fqdn: ''
+    idna: ''
+    isoduration: ''
+    jsonpointer: '>1.13'
+    jsonschema: '>=4.17.3,<5.0a0'
+    python: ''
+    rfc3339-validator: ''
+    rfc3986-validator: '>0.1.0'
+    uri-template: ''
+    webcolors: '>=1.11'
+  hash:
+    md5: 7a709748e93f0b2c33d6b5b676b6d9d0
+    sha256: 767da9c47d64e1dc826d3173e46ff6fd4e858c94ff61d67ff4f976c7bc9502a2
+  manager: conda
+  name: jsonschema-with-format-nongpl
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.17.3-pyhd8ed1ab_0.conda
+  version: 4.17.3
+- category: main
+  dependencies:
     importlib_metadata: '>=4.8.3'
     jupyter_core: '>=4.12,!=5.0.*'
     python: '>=3.8'
     python-dateutil: '>=2.8.2'
     pyzmq: '>=23.0'
     tornado: '>=6.2'
     traitlets: '>=5.3'
@@ -11183,22 +12475,22 @@
   dependencies:
     jsonschema: '>=2.6'
     jupyter_core: ''
     python: '>=3.8'
     python-fastjsonschema: ''
     traitlets: '>=5.1'
   hash:
-    md5: 3ec35d84fc1775215061517eb4660693
-    sha256: d8b1ad3c219b39e5e325785606853ff1cd334769228490ac977b85aa95e94ba0
+    md5: 61ba076de6530d9301a0053b02f093d2
+    sha256: fc82c5a9116820757b03ffb836b36f0f50e4cd390018024dbadb0ee0217f6992
   manager: conda
   name: nbformat
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda
-  version: 5.9.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.2-pyhd8ed1ab_0.conda
+  version: 5.9.2
 - category: main
   dependencies:
     prompt-toolkit: '>=3.0.39,<3.0.40.0a0'
   hash:
     md5: 4bbbe67d5df19db30f04b8e344dc9976
     sha256: 89f7fecc7355181dbc2ab851e668a2fce6aa4830b336a34c93b59bda93206270
   manager: conda
@@ -11278,14 +12570,33 @@
   name: botocore
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda
   version: 1.29.165
 - category: main
   dependencies:
+    certifi: ''
+    cryptography: '>=1.3.4'
+    idna: '>=2.0.0'
+    pyopenssl: '>=0.14'
+    pysocks: '>=1.5.6,<2.0,!=1.5.7'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    urllib3: ''
+  hash:
+    md5: 21f217991c9bf115e814038cffec4daf
+    sha256: 9e8b05d3b4bb5ba843db486491f789c182183262beb30b9697b2a349c7ac9921
+  manager: conda
+  name: dulwich
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/dulwich-0.21.5-py310h6729b98_0.conda
+  version: 0.21.5
+- category: main
+  dependencies:
     cairo: '>=1.16.0,<2.0a0'
     expat: '>=2.5.0,<3.0a0'
     fontconfig: '>=2.14.1,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
     gdk-pixbuf: '>=2.42.8,<3.0a0'
     gtk2: ''
@@ -11331,14 +12642,32 @@
   name: ipython
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda
   version: 8.14.0
 - category: main
   dependencies:
+    jsonschema-with-format-nongpl: '>=3.2'
+    python: '>=3.7'
+    python-json-logger: '>=2.0.4'
+    pyyaml: '>=5.3'
+    rfc3339-validator: ''
+    rfc3986-validator: '>=0.1.1'
+    traitlets: '>=5.3'
+  hash:
+    md5: 279fed93be42722de98e998ec80be8a1
+    sha256: 1b168cd11337dcbd2eae71b91ad7624c5afed0561e4f703d5eeee27e182f98c1
+  manager: conda
+  name: jupyter_events
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.7.0-pyhd8ed1ab_0.conda
+  version: 0.7.0
+- category: main
+  dependencies:
     matplotlib-base: '>=3.7.2,<3.7.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tornado: '>=5'
   hash:
     md5: 4fe2e1daa542b330507af9a2ca079d1c
     sha256: a47920246485fdd4a9e0dadc04359a9264017f9b18c4b77cfe94213fe6a14c65
@@ -11362,29 +12691,29 @@
   name: nbclient
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda
   version: 0.7.4
 - category: main
   dependencies:
-    libcxx: '>=14.0.6'
-    pyqt5-sip: 12.11.0 py310h415000c_3
+    libcxx: '>=15.0.7'
+    pyqt5-sip: 12.12.2 py310h018f80b_4
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
-    qt-main: '>=5.15.6,<5.16.0a0'
-    sip: '>=6.7.5,<6.8.0a0'
+    qt-main: '>=5.15.8,<5.16.0a0'
+    sip: '>=6.7.10,<6.8.0a0'
   hash:
-    md5: c652959992036327b71a2d5ff593cf72
-    sha256: 42a3c561ff6c81416b2b37db0a53c0698b637e474b46d8e9f6f9a84635718ec2
+    md5: eba55c15090ca812a17cf393ef61ba7c
+    sha256: 06fa4984ac167b48a3e6aeb9d6b23ad30926ad1aa71651431d47f4060fe1cd51
   manager: conda
   name: pyqt
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyqt-5.15.7-py310hdd03f62_3.conda
-  version: 5.15.7
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyqt-5.15.9-py310hecc045f_4.conda
+  version: 5.15.9
 - category: main
   dependencies:
     blas: '* mkl'
     filelock: ''
     jinja2: ''
     mkl: '>=2018'
     networkx: ''
@@ -11460,14 +12789,69 @@
   name: vtk
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/vtk-9.2.5-qt_py310hea5b068_200.conda
   version: 9.2.5
 - category: main
   dependencies:
+    msgpack-python: '>=0.5.2'
+    python: '>=3.6'
+    requests: '>=2.16.0'
+  hash:
+    md5: db23395890ef31be3c2320fb41b665b0
+    sha256: 99b68d1e9b1e148c9dfa5886cdd9b6082e968328658ba71a5b76cdc93a92ef02
+  manager: conda
+  name: cachecontrol
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.14-pyhd8ed1ab_0.conda
+  version: 0.12.14
+- category: main
+  dependencies:
+    boltons: '>=23.0.0'
+    conda-package-handling: '>=1.3.0'
+    jsonpatch: '>=1.32'
+    packaging: '>=23.0'
+    pluggy: '>=1.0.0'
+    pycosat: '>=0.6.3'
+    pyopenssl: '>=16.2.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.27.0,<3'
+    ruamel.yaml: '>=0.11.14,<0.18'
+    setuptools: '>=60.0.0'
+    toolz: '>=0.8.1'
+    tqdm: '>=4'
+  hash:
+    md5: dff2e97c1fcf3b9fe5f55b28b0effb97
+    sha256: d94e23ef9e09522bcda061e301acc9b91392482d92f1c933fce22c86b8506c47
+  manager: conda
+  name: conda
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/conda-23.7.2-py310h2ec42d9_0.conda
+  version: 23.7.2
+- category: main
+  dependencies:
+    appdirs: ''
+    click: '>=5.1'
+    filelock: ''
+    python: '>=3.7'
+    requests: '>=2'
+  hash:
+    md5: c99ae3abf501990769047b4b40a98f17
+    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
+  manager: conda
+  name: ensureconda
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.3
+- category: main
+  dependencies:
     aiohttp: '>=3.6.2,<4.0.0dev'
     cachetools: '>=2.0.0,<6.0'
     pyasn1-modules: '>=0.2.1'
     pyopenssl: '>=20.0.0'
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
@@ -11507,14 +12891,31 @@
   name: ipykernel
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda
   version: 6.23.3
 - category: main
   dependencies:
+    comm: '>=0.1.3'
+    ipython: '>=6.1.0'
+    jupyterlab_widgets: '>=3.0.7,<3.1.0'
+    python: '>=3.7'
+    traitlets: '>=4.3.1'
+    widgetsnbextension: '>=4.0.7,<4.1.0'
+  hash:
+    md5: 6fe1e9c8e93261e978998c0e90e36275
+    sha256: 71f920b0b89eb177511ff2d8bd9904c9c6c96d731f90ec97168cc28bc86ed623
+  manager: conda
+  name: ipywidgets
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.0-pyhd8ed1ab_0.conda
+  version: 8.1.0
+- category: main
+  dependencies:
     attrs: ''
     click: ''
     importlib-metadata: ''
     nbclient: '>=0.2,<0.8'
     nbformat: ''
     python: '>=3.8'
     pyyaml: ''
@@ -11545,22 +12946,22 @@
     packaging: ''
     pandocfilters: '>=1.4.1'
     pygments: '>=2.4.1'
     python: '>=3.8'
     tinycss2: ''
     traitlets: '>=5.0'
   hash:
-    md5: 32dde1678bb003c90d4bc0c2dbd21814
-    sha256: 76ad7689d35fe031459c422f142c9d8e7a02f6922049b7a0183fc70aaef02f0a
+    md5: 063c1fda5480050b8d989478c97a4c55
+    sha256: c5db2ba740b2ffddf11a5ba67a3afa7c05bff4656dae3d5f61a9b57c57ea3f8b
   manager: conda
   name: nbconvert-core
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     packaging: '>=20.0'
     platformdirs: '>=2.5.0'
     python: '>=3.7'
     requests: '>=2.19.0'
   hash:
@@ -11584,14 +12985,27 @@
   name: requests-oauthlib
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2
   version: 1.3.1
 - category: main
   dependencies:
+    python: '>=3.6'
+    requests: '>=2.0.1,<3.0.0'
+  hash:
+    md5: 99c98318c8646b08cc764f90ce98906e
+    sha256: 20eaefc5dba74ff6c31e537533dde59b5b20f69e74df49dff19d43be59785fa3
+  manager: conda
+  name: requests-toolbelt
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
+  version: 1.0.0
+- category: main
+  dependencies:
     botocore: '>=1.12.36,<2.0a.0'
     python: '>=3.7'
   hash:
     md5: b19a857ac845097e9c823c9f4d35f80e
     sha256: 99512bf4f4e297cc7565c94eee8ccc908411f836b341668e2b5d064273e21762
   manager: conda
   name: s3transfer
@@ -11688,14 +13102,44 @@
   name: boto3
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda
   version: 1.26.165
 - category: main
   dependencies:
+    cachecontrol: 0.12.14 pyhd8ed1ab_0
+    lockfile: '>=0.9'
+    python: '>=3.6'
+  hash:
+    md5: 43ed0c094b39bb352382db8105ab0b94
+    sha256: 23af777f65d74f18aaee1641add3b15bd442096f9c4940270151704f1aa38198
+  manager: conda
+  name: cachecontrol-with-filecache
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.14-pyhd8ed1ab_0.conda
+  version: 0.12.14
+- category: main
+  dependencies:
+    conda: '>=4.3'
+    jinja2: ''
+    packaging: ''
+    python: '>=3.6'
+    pyyaml: ''
+  hash:
+    md5: 9b175e69c1c601d01ab5edccf822363c
+    sha256: 3244e025f3d185f56fb44a44d02526797ce3e95302a868867af6dc9e2e55ebe3
+  manager: conda
+  name: conda-devenv
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-devenv-2.3.0-pyhd8ed1ab_0.tar.bz2
+  version: 2.3.0
+- category: main
+  dependencies:
     click: '>=6.0.0'
     google-auth: '>=2.15.0'
     python: '>=3.6'
     requests-oauthlib: '>=0.7.0'
   hash:
     md5: 569e62e95b01b53e4ec7d9abe83b7385
     sha256: f89613643658a51a1ac0fb7c7950526fadc2a6ce1ae13755d786e14cfce1633c
@@ -11703,31 +13147,14 @@
   name: google-auth-oauthlib
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda
   version: 1.0.0
 - category: main
   dependencies:
-    ipykernel: '>=4.5.1'
-    ipython: '>=6.1.0'
-    jupyterlab_widgets: '>=3.0.7,<3.1.0'
-    python: '>=3.7'
-    traitlets: '>=4.3.1'
-    widgetsnbextension: '>=4.0.7,<4.1.0'
-  hash:
-    md5: 4b0f4e8fe2a303e472674eae0340bdad
-    sha256: 3b17ad90294f0684fca9191f1e696e9b4f03a652d5e588b6ff0feb5647fcf116
-  manager: conda
-  name: ipywidgets
-  optional: false
-  platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda
-  version: 8.0.7
-- category: main
-  dependencies:
     ipykernel: '>=6.14'
     ipython: ''
     jupyter_client: '>=7.0.0'
     jupyter_core: '>=4.12,!=5.0.*'
     prompt_toolkit: '>=3.0.30'
     pygments: ''
     python: '>=3.7'
@@ -11789,26 +13216,26 @@
   name: myst-parser
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2
   version: 0.18.1
 - category: main
   dependencies:
-    nbconvert-core: 7.7.1 pyhd8ed1ab_1
+    nbconvert-core: 7.7.3 pyhd8ed1ab_0
     pandoc: ''
     python: '>=3.8'
   hash:
-    md5: 796b056965d7146bcac082fa2a83943d
-    sha256: b5b2823e7951a5ba41b1020b7cce109fec7f2ebe540234bf8a17c54615c2f679
+    md5: f44109e52a40b8149156f5ddd9c11b26
+    sha256: c9fceb914dd4a8fe64b1403a0c7b0c69b5c67fc726aa8239e5ecb450d27e6963
   manager: conda
   name: nbconvert-pandoc
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     accessible-pygments: ''
     babel: ''
     beautifulsoup4: ''
     docutils: '!=0.17.0'
     packaging: ''
@@ -11834,22 +13261,22 @@
     pytorch: '>=1.11.0'
     pyyaml: '>=5.4'
     requests: ''
     torchmetrics: '>=0.7.0'
     tqdm: '>=4.57.0'
     typing_extensions: '>=4.0.0'
   hash:
-    md5: ce9d626b181c6f8cceb5047f6a819f7d
-    sha256: a049296b4b33bceedf3bafd378e8a4112bca71b453734f1e0daaca2a72598593
+    md5: 5325b6adf171d4d69968100af806994e
+    sha256: 54efb4be9a8f73692cf24f85923a226c0ed6d035000704479b0f27288bb0a874
   manager: conda
   name: pytorch-lightning
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda
-  version: 2.0.4
+  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.6-pyhd8ed1ab_0.conda
+  version: 2.0.6
 - category: main
   dependencies:
     ipykernel: '>=4.1'
     ipython_genutils: ''
     jupyter_client: '>=4.1'
     jupyter_core: ''
     packaging: ''
@@ -12087,26 +13514,26 @@
   name: myst-nb
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda
   version: 0.17.2
 - category: main
   dependencies:
-    nbconvert-core: 7.7.1 pyhd8ed1ab_1
-    nbconvert-pandoc: 7.7.1 pyhd8ed1ab_1
+    nbconvert-core: 7.7.3 pyhd8ed1ab_0
+    nbconvert-pandoc: 7.7.3 pyhd8ed1ab_0
     python: '>=3.8'
   hash:
-    md5: 95d9d1523df069792cd059f412be0d6e
-    sha256: c49a87861db316b322f919825820bc7193cbfa8a4a8b21b5ffe16a133644d400
+    md5: f53d92ecd7d8563b006107f6a33e55c6
+    sha256: 2b9e7bc41ee0882d7829e984cb1a18f039a5f756b5b747f6a3ce352bc72e5103
   manager: conda
   name: nbconvert
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     jupyter_server: '>=1.8,<3'
     python: '>=3.7'
   hash:
     md5: 67e0fe74c156267d9159e9133df7fd37
     sha256: f028d7ad1f2175cde307db08b60d07e371b9d6f035cfae6c81ea94b4c408c538
@@ -12114,14 +13541,56 @@
   name: notebook-shim
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda
   version: 0.2.3
 - category: main
   dependencies:
+    __osx: ''
+    backports.cached-property: '>=1.0.2,<2.0.0'
+    cachecontrol-with-filecache: '>=0.12.9,<0.13.0'
+    cleo: '>=2.0.0,<3.0.0'
+    crashtest: '>=0.4.1,<0.5.0'
+    dulwich: '>=0.21.2,<0.22.0'
+    filelock: '>=3.8.0,<4.0.0'
+    html5lib: '>=1.0.0,<2.0.0'
+    importlib-metadata: '>=4.4'
+    jsonschema: '>=4.10.0,<5.0.0'
+    keyring: '>=23.9.0,<24.0.0'
+    lockfile: '>=0.12.2,<0.13.0'
+    packaging: '>=20.4'
+    pexpect: '>=4.7.0,<5.0.0'
+    pkginfo: '>=1.9.4,<2.0'
+    platformdirs: '>=3.0.0,<4.0.0'
+    poetry-core: 1.6.1.*
+    poetry-plugin-export: '>=1.4.0,<2.0.0'
+    pyproject_hooks: '>=1.0.0,<2.0.0'
+    python: '>=3.7.0,<4.0.0'
+    python-build: '>=0.10.0,<0.11.0'
+    python-installer: '>=0.7.0,<0.8.0'
+    requests: '>=2.18,<3.0'
+    requests-toolbelt: '>=0.9.1,<2'
+    shellingham: '>=1.5.0,<2.0.0'
+    tomli: '>=2.0.1,<3.0.0'
+    tomlkit: '>=0.11.4,<1.0.0'
+    trove-classifiers: '>=2022.5.19'
+    urllib3: '>=1.26.0,<2.0.0'
+    virtualenv: '>=20.22.0,<21.0.0'
+    xattr: '>=0.10.0,<0.11.0'
+  hash:
+    md5: cb22f4398986b6cde646b8ec6efe141f
+    sha256: 9a24f0249abad2b3afbe6ff13f71abc35699e8f4e04bed3d9739c7d93689aade
+  manager: conda
+  name: poetry
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-1.5.1-osx_pyhd8ed1ab_0.conda
+  version: 1.5.1
+- category: main
+  dependencies:
     pyqt: ''
     python: '>=3.7'
     qtconsole-base: '>=5.4.3,<5.4.4.0a0'
   hash:
     md5: 3777f933bec5113d5a292de10b03d0f6
     sha256: 6443de033408a3d5f915dcd5b0b52806a86b20e54d85859f042ed71443651231
   manager: conda
@@ -12201,14 +13670,38 @@
   name: tensorboard
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda
   version: 2.13.0
 - category: main
   dependencies:
+    click: '>=8.0'
+    click-default-group: ''
+    ensureconda: '>=1.3'
+    jinja2: ''
+    poetry: ''
+    pydantic: '>=1.8.1'
+    python: '>=3.6'
+    pyyaml: '>=5.1'
+    requests: '>=2'
+    ruamel.yaml: ''
+    setuptools: ''
+    toml: ''
+    typing-extensions: ''
+  hash:
+    md5: 1c31d380288fc1599fb5f4c76c8c828c
+    sha256: 2895546468293f358395b072846ebf8a2e04339d1355009fb96787d804250bb0
+  manager: conda
+  name: conda-lock
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.0.5-pyhd8ed1ab_1.tar.bz2
+  version: 1.0.5
+- category: main
+  dependencies:
     click: '>=7.1,<9'
     docutils: '>=0.15,<0.19'
     jinja2: ''
     jsonschema: <5
     linkify-it-py: '>=2.0.0,<2.1.0'
     myst-nb: '>=0.17.1,<0.18.0'
     python: '>=3.7'
@@ -12308,22 +13801,22 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/jupyter-1.0.0-py310h2ec42d9_8.conda
   version: 1.0.0
 - category: main
   dependencies: {}
   hash:
-    md5: 604212634bd8c4d6f20d44b946e8eedb
-    sha256: d0488a3e7a86cc11f8c847a7c12a5f1fb8567f05646faae78944807862f9d167
+    md5: b1c2327b36f1a25d96f2039b0d3e3739
+    sha256: b85a6f307f8e1c803cb570bdfb9e4d811a361417873ecd2ecf687587405a72e0
   manager: conda
   name: ca-certificates
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda
-  version: 2023.5.7
+  url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.7.22-h56e8100_0.conda
+  version: 2023.7.22
 - category: main
   dependencies: {}
   hash:
     md5: 6ddbe275ebb9ae875355baf8ade34b3f
     sha256: 77a19b9b7e8b50d0907b8d69de0e11b7fdecdc66d37e31acdcee3892297b26a7
   manager: conda
   name: cuda-cccl-impl
@@ -12374,22 +13867,22 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/nvidia/win-64/cuda-nvtx-11.8.86-0.tar.bz2
   version: 11.8.86
 - category: main
   dependencies: {}
   hash:
-    md5: 93cb84c3524a1612cbce98ead299c735
-    sha256: 26ab725d6db651e09943f88cc94a90afe8147cabe0e444dccf10bc70420f62a8
+    md5: d3277124e5bca9acbd74ad709d1714b5
+    sha256: 8e325783cab2fc6c6484741aede20c80ffe1cdc4ff84b247715435d7a77bae60
   manager: conda
   name: cuda-profiler-api
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.2.53-0.tar.bz2
-  version: 12.2.53
+  url: https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.2.128-0.tar.bz2
+  version: 12.2.128
 - category: main
   dependencies: {}
   hash:
     md5: c9f9d925118c389a1a3f4267b6272b98
     sha256: 1634892d2b95f7cc27bb1cfaa5ba0de6f2478582961a0fd2d309f3956e883640
   manager: conda
   name: cuda-version
@@ -12440,22 +13933,22 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2
   version: '0.83'
 - category: main
   dependencies: {}
   hash:
-    md5: dbc4636f419722fbf3ab6501377228ba
-    sha256: b3006690844eedbb51030e71778767acc9967f4148b6f335ba3fddf8aa42aa5b
+    md5: f2e71622520883ffdbc379b13049534c
+    sha256: e9c3cab6b4534bcab0a31e843d28d73326312d6983b2098b91ed5f37af2c865b
   manager: conda
   name: intel-openmp
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2023.1.0-h57928b3_46319.conda
-  version: 2023.1.0
+  url: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2023.2.0-h57928b3_49496.conda
+  version: 2023.2.0
 - category: main
   dependencies: {}
   hash:
     md5: 750e01875ed59059ae043d09d262968d
     sha256: 94a715cddad661b3e9f6114f52c2334961d169e513f8a28ee402d7d1bc7b59a5
   manager: conda
   name: libcublas
@@ -12944,22 +14437,22 @@
   version: 3.2.0
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 3671ee2bcd1d915690de5b1445fdf004
-    sha256: adcf12c65b6d1e8ef875ee2845f687957461a7869a1b1474cf6c4ac9024678df
+    md5: 305b3ca7023ac046b9a42a48661f6512
+    sha256: 633a6a8db1f9a010cb0619f3446fb61f62dea348b09615ffae9744ab1001c24c
   manager: conda
   name: eigen
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.1-h91493d7_0.conda
-  version: 3.4.1
+  url: https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.0-h91493d7_0.conda
+  version: 3.4.0
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
     md5: 09196a7ba69b70d2124aff7b2763035d
@@ -13221,24 +14714,25 @@
   name: libsqlite
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda
   version: 3.42.0
 - category: main
   dependencies:
-    vc: '>=14.1,<15'
-    vs2015_runtime: '>=14.16.27033'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 0d45ae978c33ff0b5f95ea24c717d5cf
-    sha256: 446090f3995a76fad652f505cb373775e0c1cd8b0a62ab8f624541bf6622589f
+    md5: db1816a489a1b69dd1fd93e523cf026a
+    sha256: d602dc13e1b0a955aa5f14772a3b8dc5ee72a4f68a4d63adb82a1ee105ffe4b2
   manager: conda
   name: libuv
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libuv-1.44.2-h8ffe710_0.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/win-64/libuv-1.44.2-hcfcfb64_1.conda
   version: 1.44.2
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
@@ -13308,22 +14802,22 @@
 - category: main
   dependencies:
     ca-certificates: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 1d913a5de46c6b2f7e4cfbd26b106b8b
-    sha256: 4424486fb9a2aeaba912a8dd8a5b5cdb6fcd65d7708fd854e3ea27449bb352a3
+    md5: 79b3f40f27cd80a265c276cea6714507
+    sha256: 676b78a786bf845cdca96fa830459f1ffa6603954a88ad86f476456d0a909f4e
   manager: conda
   name: openssl
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda
-  version: 3.1.1
+  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.2-hcfcfb64_0.conda
+  version: 3.1.2
 - category: main
   dependencies:
     vc: '>=14.1,<15.0a0'
     vs2015_runtime: '>=14.16.27012'
   hash:
     md5: 32b45d3fcffddc84cc1a014a0b5f0d58
     sha256: 7f0ceed590a717ddc7612f67657119df1e6df0d031a822b570d741a89a3ba784
@@ -13532,21 +15026,21 @@
 - category: main
   dependencies:
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: c2e1def32a19610ac26db453501760b6
-    sha256: 0be9e57f50f33c813df6e1ad65b8bf8ccf1c23f734785236146b56b9078e7c7b
+    md5: ba26634d038b91466bb4242c8b5e0cfa
+    sha256: 9cff68d1bd3b1b956133f9f5f35d475014402f3f4e7956047bf3a70f2107f11c
   manager: conda
   name: libclang13
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libclang13-15.0.7-default_h77d9078_2.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/libclang13-15.0.7-default_h77d9078_3.conda
   version: 15.0.7
 - category: main
   dependencies:
     cuda-version: '>=12.0.0,<12.1.0a0'
     libcurand: 10.3.1.50 h63175ca_0
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
@@ -13816,14 +15310,26 @@
   name: alabaster
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda
   version: 0.7.13
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: 5f095bc6454094e96f146491fd03633b
+    sha256: ae9fb8f68281f84482f2c234379aa12405a9e365151d43af20b3ae1f17312111
+  manager: conda
+  name: appdirs
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2
+  version: 1.4.4
+- category: main
+  dependencies:
     python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*'
   hash:
     md5: f70280205d7044c8b8358c8de3190e5d
     sha256: 79cc289deb95b30d4bdedbba5d5dbdcd0ed95b3c306757dc1f83d9164f0c2d88
   manager: conda
   name: attrs
   optional: false
@@ -13864,14 +15370,26 @@
   name: blinker
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda
   version: 1.6.2
 - category: main
   dependencies:
+    python: 2.7.*|>=3.7
+  hash:
+    md5: 033eb25fffd222aceeca6d58cd953680
+    sha256: 4ff828cceb8f55cb26d23b1a4c174d22c7cd92350221724bcaf2d6632e33fdee
+  manager: conda
+  name: boltons
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/boltons-23.0.0-pyhd8ed1ab_0.conda
+  version: 23.0.0
+- category: main
+  dependencies:
     libbrotlidec: 1.0.9 hcfcfb64_9
     libbrotlienc: 1.0.9 hcfcfb64_9
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
     md5: ba8ae6c24cf47da3fb73270e4f119f08
@@ -13880,36 +15398,48 @@
   name: brotli-bin
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_9.conda
   version: 1.0.9
 - category: main
   dependencies:
+    python: '>=3.6'
+  hash:
+    md5: 576d629e47797577ab0f1b351297ef4a
+    sha256: 6dbf7a5070cc43d90a1e4c2ec0c541c69d8e30a0e25f50ce9f6e4a432e42c5d7
+  manager: conda
+  name: cached_property
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 60b5eb16d9a7a5482ba37f67aa49db5b
     sha256: 8d30a41a88900730c748f5b296730a0d48e5cfa2c8b260aab60fa9f26ffafcc0
   manager: conda
   name: cachetools
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda
   version: 5.3.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 5d1b71c942b8421285934dad1d891ebc
-    sha256: f839a6e04d94069f90dd85337ea9108f058dc76771bb469a413f32bb1ba0b256
+    md5: 7f3dbc9179b4dde7da98dfb151d0ad22
+    sha256: db66e31866ff4250c190788769e3a8a1709237c3e9c38d7143aae95ab75fcb31
   manager: conda
   name: certifi
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda
-  version: 2023.5.7
+  url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.7.22-pyhd8ed1ab_0.conda
+  version: 2023.7.22
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 313516e9a4b08b12dfb1e1cd390a96e3
     sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   manager: conda
@@ -13928,14 +15458,26 @@
   name: colorama
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
   version: 0.4.6
 - category: main
   dependencies:
+    python: '>=3.6,<4.0'
+  hash:
+    md5: 709a2295dd907bb34afb57d54320642f
+    sha256: 2f05954a3faf0700c14c1deddc085385160ee32abe111699c78d9cb277e915cc
+  manager: conda
+  name: crashtest
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2
+  version: 0.4.1
+- category: main
+  dependencies:
     cuda-cccl: '>=11.8.89'
     cuda-cudart-dev: '>=11.8.89'
     cuda-nvrtc-dev: '>=11.8.89'
     cuda-profiler-api: '>=11.8.86'
     libcublas-dev: '>=11.11.3.6'
     libcufft-dev: '>=10.9.0.58'
     libcurand-dev: '>=10.3.0.86'
@@ -13990,24 +15532,24 @@
   version: '0.8'
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: b7defb941402f3581384d16070ed1456
-    sha256: ac5dc3ee00cd88ac5362d0ad657fd2152efa4928a9eed83b018b101343601a89
+    md5: 8c8e0940454d91fd5d24dc82c3f76a29
+    sha256: 0eff270033c94a6631694ca37b0e1996e017e066a04e8e9a77183faf228006f2
   manager: conda
   name: debugpy
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py310h00ffb61_0.conda
-  version: 1.6.7
+  url: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.8-py310h00ffb61_0.conda
+  version: 1.6.8
 - category: main
   dependencies:
     python: '>=3.5'
   hash:
     md5: 43afe5ab04e35e17ba28649471dd7364
     sha256: 328a6a379f9bdfd0230e51de291ce858e6479411ea4b0545fb377c71662ef3e2
   manager: conda
@@ -14026,14 +15568,26 @@
   name: defusedxml
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2
   version: 0.7.1
 - category: main
   dependencies:
+    python: 2.7|>=3.6
+  hash:
+    md5: 12d8aae6994f342618443a8f05c652a0
+    sha256: 13c887cb4a29e1e853a118cfc0e42b72a7e1d1c50c66c0974885d37f0db30619
+  manager: conda
+  name: distlib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda
+  version: 0.3.7
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: cdc0acfc953b7bd34229b7f229eae46a
     sha256: e1a6a645d16823662ebbe3b7770ec0bac7925ad7e6237652886b17d78dc5aa99
   manager: conda
   name: docutils
@@ -14250,14 +15804,26 @@
   name: jmespath
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2
   version: 1.0.1
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: 07d85c22a3beb102a48cd123df84c2a6
+    sha256: da279af2285d8f575a7f5652e83bf7f36155c4c63154e385a9d171efcc607bc1
+  manager: conda
+  name: jsonpointer
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonpointer-2.0-py_0.tar.bz2
+  version: '2.0'
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 2bc3ca2f7387af385dd06706b4fb2d35
     sha256: 0781ed7a4f35ff1309e95381c40c8d8f96263ca4260a72baaafda87c975a972a
   manager: conda
   name: jupyterlab_widgets
   optional: false
@@ -14294,27 +15860,27 @@
   name: lazy-object-proxy
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/lazy-object-proxy-1.9.0-py310h8d17308_0.conda
   version: 1.9.0
 - category: main
   dependencies:
-    libclang13: 15.0.7 default_h77d9078_2
+    libclang13: 15.0.7 default_h77d9078_3
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 70188b1b3e0b1716405adab9050894d1
-    sha256: af265f9358565c650ec3f09557d47c6ced441164d10cd500b74651513f61be46
+    md5: 71c8b6249c9e9e18b3aec705e95c1040
+    sha256: d54ad3cc60469f3c885cef45acd7216bab9d941dec8f37e75ece48b9baba145b
   manager: conda
   name: libclang
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libclang-15.0.7-default_h77d9078_2.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/libclang-15.0.7-default_h77d9078_3.conda
   version: 15.0.7
 - category: main
   dependencies:
     krb5: '>=1.20.1,<1.21.0a0'
     libssh2: '>=1.10.0,<2.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
@@ -14402,14 +15968,26 @@
   name: libtiff
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libtiff-4.4.0-hc4f729c_5.conda
   version: 4.4.0
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: c104d98e09c47519950cffb8dd5b4f10
+    sha256: d3a68045ef74a2a7b8c8a55b242fdbc875d362e37adcf793613cf0d8c8e4fbf7
+  manager: conda
+  name: lockfile
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2
+  version: 0.12.2
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
     md5: e6deeae9d0dac4d17c6ef2fa62b3efff
@@ -14442,26 +16020,51 @@
   name: mdurl
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2
   version: 0.1.0
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 15cfc917187d7c173647dd65d340259b
+    sha256: 606f9ed8839ba6ba1926ecf1a99cde0e8f02f47cb8d657a390ae13872e019efa
+  manager: conda
+  name: menuinst
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/menuinst-1.4.19-py310h5588dad_1.tar.bz2
+  version: 1.4.19
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: c7d0ea64c37752ecbe6da458aee662d2
     sha256: 0f913186537ce2c8df3440a934a1dbe9faefe6ab5df44fc48cb854c0704abb60
   manager: conda
   name: mistune
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda
   version: 3.0.0
 - category: main
   dependencies:
+    python: '>=3.8'
+  hash:
+    md5: 8549fafed0351bbfaa1ddaa15fdf9b4e
+    sha256: 07ce65497dec537e490992758934ddbc4fb5ed9285b41387a7cca966f1a98a0f
+  manager: conda
+  name: more-itertools
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.1.0-pyhd8ed1ab_0.conda
+  version: 10.1.0
+- category: main
+  dependencies:
     python: '>=3.6'
   hash:
     md5: dbf6e2d89137da32fa6670f3bffc024e
     sha256: a4f025c712ec1502a55c471b56a640eaeebfce38dd497d5a1a33729014cac47a
   manager: conda
   name: mpmath
   optional: false
@@ -14472,14 +16075,30 @@
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
   hash:
+    md5: 03f6096e23f3861934af853ac987c185
+    sha256: 03960db66d81c662f123322efb60ba3b1ca9c03c8b3a936913aa9d72a4dbc78e
+  manager: conda
+  name: msgpack-python
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.5-py310h232114e_0.conda
+  version: 1.0.5
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
     md5: 23a55d74d8f91c7667555b81030034bf
     sha256: 564e7e984814863a8f9fa31acbc50706dfe67d4e8601b3e74e4003a9c6ceba14
   manager: conda
   name: multidict
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/multidict-6.0.4-py310h8d17308_0.conda
@@ -14568,22 +16187,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2
   version: 0.8.3
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: dbb80d1e8dc2dba5c8b106dc0768ad45
-    sha256: d94463e0a140ead5c01990b565a1a21b85cb3831d56fed5955b5446bd5df33fe
+    md5: e41debb259e68490e3ab81e46b639ab6
+    sha256: 7bcfa6d86359d45572ba9ccaeaedc04b0452e2654fe44b6fe378d0d37b8745e1
   manager: conda
   name: pathspec
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda
-  version: 0.11.1
+  url: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.2-pyhd8ed1ab_0.conda
+  version: 0.11.2
 - category: main
   dependencies:
     python: '>=3'
   hash:
     md5: 415f0ebb6198cc2801c73438a9fb5761
     sha256: a1ed1a094dd0d1b94a09ed85c283a0eb28943f2e6f22161fb45e128d35229738
   manager: conda
@@ -14592,14 +16211,26 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
   version: 0.7.5
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
+    md5: be1e9f1c65a1ed0f2ae9352fec99db64
+    sha256: 7ea5a5af62a15376d9f4f9f3c134874d0b0710f39be719e849b7fa9ca8870502
+  manager: conda
+  name: pkginfo
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda
+  version: 1.9.6
+- category: main
+  dependencies:
+    python: '>=3.6'
+  hash:
     md5: 89e3c7cdde7d3aaa2aee933b604dd07f
     sha256: 7d055ffc8a02bf781a89d069db3454b453605cdaff300b82cedcc7133283e47e
   manager: conda
   name: pkgutil-resolve-name
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2
@@ -14666,14 +16297,26 @@
   name: pthread-stubs
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2
   version: '0.4'
 - category: main
   dependencies:
+    python: ''
+  hash:
+    md5: 359eeb6536da0e687af562ed265ec263
+    sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
+  manager: conda
+  name: ptyprocess
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+  version: 0.7.0
+- category: main
+  dependencies:
     python: '>=3.5'
   hash:
     md5: 6784285c7e55cb7212efabc79e4c2883
     sha256: 72792f9fc2b1820e37cc57f84a27bc819c71088c3002ca6db05a2e56404f9d44
   manager: conda
   name: pure_eval
   optional: false
@@ -14702,14 +16345,30 @@
   name: pycodestyle
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda
   version: 2.10.0
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 3324f50e5d46a04309d8f8f956c17244
+    sha256: 2e74d789ff6846181bd7e32260b9c0d57b91d4fcc0311274fca4279f8a35b048
+  manager: conda
+  name: pycosat
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pycosat-0.6.4-py310h8d17308_1.tar.bz2
+  version: 0.6.4
+- category: main
+  dependencies:
     python: 2.7.*|>=3.4
   hash:
     md5: 076becd9e05608f8dc72757d5f3a91ff
     sha256: 74c63fd03f1f1ea2b54e8bc529fd1a600aaafb24027b738d0db87909ee3a33dc
   manager: conda
   name: pycparser
   optional: false
@@ -14780,22 +16439,34 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py310h8d17308_0.conda
   version: 0.19.3
 - category: main
   dependencies:
     python: '>=3.3'
   hash:
-    md5: dd4f393d857e9283eef2442234bd05e3
-    sha256: b7a8b9b2310b3ee74ba99eef9692e477bb8bddf110eff45784dee7d81a693455
+    md5: 3be9466311564f80f8056c0851fc5bb7
+    sha256: 73985a9a2dd7ccf77b7428a12148e1b381c8635e9195e47a652397e9a56284ce
   manager: conda
   name: python-fastjsonschema
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda
-  version: 2.17.1
+  url: https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.18.0-pyhd8ed1ab_0.conda
+  version: 2.18.0
+- category: main
+  dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 65dea78f903d686c8b0c2feaf0e15e1f
+    sha256: 822f95b7786cfa61a6519153117b21d93194890e02a884b9f66ee4275e4f1c0a
+  manager: conda
+  name: python-installer
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/python-installer-0.7.0-pyhd8ed1ab_0.conda
+  version: 0.7.0
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
     md5: a61bf9ec79426938ff785eb69dbb1960
     sha256: 4790787fe1f4e8da616edca4acf6a4f8ed4e7c6967aa31b920208fc8f95efcca
   manager: conda
@@ -14832,14 +16503,27 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py310h00ffb61_2.tar.bz2
   version: '304'
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
+  hash:
+    md5: 9f60b973d0238c7e62a2324767acb62f
+    sha256: a9a9daf75f1ce507456a4bbfb3d3ee27a2c805fceac534dcaaff670791f457eb
+  manager: conda
+  name: pywin32-ctypes
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py310h5588dad_0.conda
+  version: 0.2.2
+- category: main
+  dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
     winpty: ''
   hash:
     md5: 685cf7fe1b0724628476c991329017ad
     sha256: 92145040d25738e56feb5c766eb6a613776ec574c4a3abb5eddc3cbe31d078da
@@ -14922,14 +16606,26 @@
   name: setuptools
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda
   version: 67.7.2
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 1de44299f48f522caa2e0074231614e1
+    sha256: 3cb4a4a83b617fdfef9b92751634488db0b8961c80340be8068bf6d4f1d5ac25
+  manager: conda
+  name: shellingham
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.1-pyhd8ed1ab_0.conda
+  version: 1.5.1
+- category: main
+  dependencies:
     python: ''
   hash:
     md5: e5f25f8dbc060e9a8d912e432202afc2
     sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
   manager: conda
   name: six
   optional: false
@@ -15091,14 +16787,38 @@
   name: tomli
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
   version: 2.0.1
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 62f5b331c53d73e2f6c4c130b53518a0
+    sha256: dc4abf58ca42f29e12b8c0f8aadedfca49cc1e97dab025d15cf000b1787df773
+  manager: conda
+  name: tomlkit
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.1-pyha770c72_0.conda
+  version: 0.12.1
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 92facfec94bc02d6ccf42e7173831a36
+    sha256: 90229da7665175b0185183ab7b53f50af487c7f9b0f47cf09c184cbc139fd24b
+  manager: conda
+  name: toolz
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2
+  version: 0.12.0
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
     md5: 6cd035ff75b46eb8ae7403b3dded2def
@@ -15119,14 +16839,26 @@
   name: traitlets
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda
   version: 5.9.0
 - category: main
   dependencies:
+    python: '>=3.6'
+  hash:
+    md5: c9918f6a3973e28a792e747289734cd3
+    sha256: a3b13371ece96434028c9c4cc5561d3a04afdb26165290b630578c1d00b462f7
+  manager: conda
+  name: trove-classifiers
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2023.7.6-pyhd8ed1ab_0.conda
+  version: 2023.7.6
+- category: main
+  dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
     md5: a2ac0e6c5a06b35dea207c3d77f94f74
@@ -15135,14 +16867,26 @@
   name: typed-ast
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.5-py310h8d17308_0.conda
   version: 1.5.5
 - category: main
   dependencies:
+    python: '>=3'
+  hash:
+    md5: e6573ac68718f17b9d4f5c8eda3190f2
+    sha256: ec1cfe0b7dc55a22223562cad799e0b16d122dab611c9923b6068d27a784ba2f
+  manager: conda
+  name: typing
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2
+  version: 3.10.0.0
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: c39d6a09fe819de4951c2642629d9115
     sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   manager: conda
   name: typing_extensions
   optional: false
@@ -15199,14 +16943,38 @@
   name: unidecode
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2
   version: 1.3.6
 - category: main
   dependencies:
+    python: '>=3.7'
+  hash:
+    md5: 0944dc65cb4a9b5b68522c3bb585d41c
+    sha256: b76904b53721dc88a46352324c79d2b077c2f74a9f7208ad2c4249892669ae94
+  manager: conda
+  name: uri-template
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda
+  version: 1.3.0
+- category: main
+  dependencies:
+    python: '>=3.5'
+  hash:
+    md5: 166212fe82dad8735550030488a01d03
+    sha256: 6e097d5fe92849ad3af2c2a313771ad2fbf1cadd4dc4afd552303b2bf3f85211
+  manager: conda
+  name: webcolors
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda
+  version: '1.13'
+- category: main
+  dependencies:
     python: ''
   hash:
     md5: 3563be4c5611a44210d9ba0c16113136
     sha256: 302f4f4bd1ad00c0be1426ecf6bb01db59cfd8aff3de0cf1596526dca1a6b70e
   manager: conda
   name: webencodings
   optional: false
@@ -15225,22 +16993,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: c95fac682453aeffa12db7ae5a721bec
-    sha256: e91cbb3c0ad9a9507dd030f5493831cb52da120329e0d0793711e8300a36db22
+    md5: 66beb36a1fa7e0dc9d9bf843a80eb82c
+    sha256: c35e6b6c8100e9e42ed0968aef99680b1d1ec5358d4ca0d2b2175f68c6b21dd6
   manager: conda
   name: wheel
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda
-  version: 0.40.0
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.41.0-pyhd8ed1ab_0.conda
+  version: 0.41.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 2e9ebddf0b93d0fb203d0906b8052c4f
     sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
   manager: conda
@@ -15441,14 +17209,27 @@
   name: babel
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda
   version: 2.12.1
 - category: main
   dependencies:
+    python: '>=3.6'
+    typing: '>=3.6'
+  hash:
+    md5: 0e1df3978dd516e20ef88c86d51e5432
+    sha256: 1d86eafb5e9ed078f891e12b46692d786723652907dfb01b047c7da31f92b862
+  manager: conda
+  name: backports.cached-property
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/backports.cached-property-1.0.2-pyhd8ed1ab_0.tar.bz2
+  version: 1.0.2
+- category: main
+  dependencies:
     backports: ''
     python: '>=3.6'
     setuptools: ''
   hash:
     md5: 6b1b907661838a75d067a22f87996b2e
     sha256: 7027bb689dd4ca4a08e3b25805de9d04239be6b31125993558f21f102a9d2700
   manager: conda
@@ -15501,14 +17282,26 @@
   name: brotli
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_9.conda
   version: 1.0.9
 - category: main
   dependencies:
+    cached_property: '>=1.5.2,<1.5.3.0a0'
+  hash:
+    md5: 9b347a7ec10940d3f7941ff6c460b551
+    sha256: 561e6660f26c35d137ee150187d89767c988413c978e1b712d53f27ddf70ea17
+  manager: conda
+  name: cached-property
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2
+  version: 1.5.2
+- category: main
+  dependencies:
     pycparser: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
   hash:
@@ -15535,22 +17328,22 @@
   url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-win_pyh7428d3b_0.conda
   version: 8.1.6
 - category: main
   dependencies:
     python: '>=3.6'
     traitlets: '>=5.3'
   hash:
-    md5: 168ae0f82cdf7505048e81054c7354e4
-    sha256: 657e0a513c8705dc542c54c4c5234e813b7f4e2f412688796d611e83ddf132ea
+    md5: c8eaca39e2b6abae1fc96acc929ae939
+    sha256: 11057745946a95ee7cc4c98900a60c7362266a4cb28bc97d96cd88e3056eb701
   manager: conda
   name: comm
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda
-  version: 0.1.3
+  url: https://conda.anaconda.org/conda-forge/noarch/comm-0.1.4-pyhd8ed1ab_0.conda
+  version: 0.1.4
 - category: main
   dependencies:
     krb5: '>=1.20.1,<1.21.0a0'
     libcurl: 8.1.2 h68f0423_0
     libssh2: '>=1.10.0,<2.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
@@ -15688,14 +17481,28 @@
   name: hdf5
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/hdf5-1.12.2-nompi_h57737ce_101.conda
   version: 1.12.2
 - category: main
   dependencies:
+    python: ''
+    six: '>=1.9'
+    webencodings: ''
+  hash:
+    md5: b2355343d6315c892543200231d7154a
+    sha256: 9ad06446fe9847e86cb20d220bf11614afcd2cbe9f58096f08d5d4018877bee4
+  manager: conda
+  name: html5lib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2
+  version: '1.1'
+- category: main
+  dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
   hash:
     md5: 4e9f59a060c3be52bc4ddc46ee9b6946
     sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   manager: conda
   name: importlib-metadata
@@ -15714,25 +17521,38 @@
   name: importlib_resources
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda
   version: 6.0.0
 - category: main
   dependencies:
+    more-itertools: ''
+    python: '>=3.7'
+  hash:
+    md5: e9f79248d30e942f7c358ff21a1790f5
+    sha256: 14f5240c3834e1b784dd41a5a14392d9150dff62a74ae851f73e65d2e2bbd891
+  manager: conda
+  name: jaraco.classes
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda
+  version: 3.3.0
+- category: main
+  dependencies:
     parso: '>=0.8.0,<0.9.0'
     python: '>=3.6'
   hash:
-    md5: b5e695ef9c3f0d27d6cd96bf5adc9e07
-    sha256: abe63ae6e1b13f83500608d94004cb8d485b264083511d77f79253e775cd546c
+    md5: 1cd7f70057cdffc10977b613fb75425d
+    sha256: d2d9e885cbc1efa63107b616588c61000063d4c223c0585962485bd016e77ce8
   manager: conda
   name: jedi
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda
-  version: 0.18.2
+  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.0-pyhd8ed1ab_0.conda
+  version: 0.19.0
 - category: main
   dependencies:
     markupsafe: '>=2.0'
     python: '>=3.7'
   hash:
     md5: c8490ed5c70966d232fdd389d0dbed37
     sha256: b045faba7130ab263db6a8fdc96b1a3de5fcf85c4a607c5f11a49e76851500b5
@@ -15740,14 +17560,27 @@
   name: jinja2
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2
   version: 3.1.2
 - category: main
   dependencies:
+    jsonpointer: '>=1.9'
+    python: '>=3.6'
+  hash:
+    md5: 09150b51b0528a31a0f6500b96fdde82
+    sha256: d87fd8da2d3327744821b6b1d1e5b76e4077224fb626ce02d6623a1bc6ee2563
+  manager: conda
+  name: jsonpatch
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonpatch-1.32-pyhd8ed1ab_0.tar.bz2
+  version: '1.32'
+- category: main
+  dependencies:
     pygments: '>=2.4.1,<3'
     python: '>=3.7'
   hash:
     md5: 243f63592c8e449f40cd42eb5cf32f40
     sha256: 08453e09d5a6bbaeeca839553a5dfd7a377a97550efab96019c334a8042f54f5
   manager: conda
   name: jupyterlab_pygments
@@ -15895,14 +17728,27 @@
   name: overrides
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2
   version: 7.3.1
 - category: main
   dependencies:
+    ptyprocess: '>=0.5'
+    python: ''
+  hash:
+    md5: 330448ce4403cc74990ac07c555942a1
+    sha256: 07706c0417ead94f359ca7278f65452d3c396448777aba1da6a11fc351bdca9a
+  manager: conda
+  name: pexpect
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2
+  version: 4.8.0
+- category: main
+  dependencies:
     python: '>=3.7'
     setuptools: ''
     wheel: ''
   hash:
     md5: 7288da0d36821349cf1126e8670292df
     sha256: 4fe1f47f6eac5b2635a622b6f985640bf835843c1d8d7ccbbae0f7d27cadec92
   manager: conda
@@ -16139,24 +17985,24 @@
     packaging: ''
     ply: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tomli: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: a249b5eefc4c36146ade59e2b237b7fd
-    sha256: 300d6da8641aed7d9baf63e2d7fe99383bdb7c1215834932283579e5a7c1b1ae
+    md5: adde89badfc7fd6e238aa4e5c2381e91
+    sha256: 0fed98aa10d930ec254c23ad935049b97e15a709650403d2c0f3d714485aa69f
   manager: conda
   name: sip
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/sip-6.7.9-py310h00ffb61_0.conda
-  version: 6.7.9
+  url: https://conda.anaconda.org/conda-forge/win-64/sip-6.7.11-py310h00ffb61_0.conda
+  version: 6.7.11
 - category: main
   dependencies:
     mpmath: '>=0.19'
     python: '>=3.8'
   hash:
     md5: 6af285473a6a49ea8068e0b5b28ed7de
     sha256: 75b525ecb0948380796f519fe723470d52f9369e23c68f194c28f34df5e49b39
@@ -16276,14 +18122,27 @@
   name: yarl
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/yarl-1.9.2-py310h8d17308_0.conda
   version: 1.9.2
 - category: main
   dependencies:
+    python: '>=3.7'
+    typing-extensions: '>=4.0.0'
+  hash:
+    md5: 578ae086f225bc2380c79f3b551ff2f7
+    sha256: bbabfd4400b03ba6c50d0a55e777e0c3ba900af8dabedb9b8aded774484b5d53
+  manager: conda
+  name: annotated-types
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda
+  version: 0.5.0
+- category: main
+  dependencies:
     cffi: '>=1.0.1'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
   hash:
@@ -16293,14 +18152,28 @@
   name: argon2-cffi-bindings
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py310h8d17308_3.tar.bz2
   version: 21.2.0
 - category: main
   dependencies:
+    python: '>=3.6'
+    python-dateutil: '>=2.7.0'
+    typing_extensions: ''
+  hash:
+    md5: fd1967c76eda3a3dd9e8e6cb7a15a028
+    sha256: a0434c2770cf5b0ab5a33913c0b202b1521bc13f755b762d16a86b110425cdc2
+  manager: conda
+  name: arrow
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/arrow-1.2.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.2.3
+- category: main
+  dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.0.0'
     wrapt: <2,>=1.11
   hash:
     md5: a1e30c9be3eb810b8efdd581449983cc
@@ -16361,14 +18234,27 @@
   name: cairo
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/cairo-1.16.0-hd694305_1014.tar.bz2
   version: 1.16.0
 - category: main
   dependencies:
+    click: ''
+    python: '>=3.6'
+  hash:
+    md5: 72a46ffc25701c173932fd55cf0965d3
+    sha256: 7384b6c194f9822d7cc2c9d82409b2fd571fad96f95e6e27c9098f63772d36fd
+  manager: conda
+  name: click-default-group
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2
+  version: 1.2.2
+- category: main
+  dependencies:
     cffi: '>=1.12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
@@ -16415,22 +18301,35 @@
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     unicodedata2: '>=14.0.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 496704d1b32153ed96e60de270a3e2f4
-    sha256: 484cccfac21ddb4eef4daded8e95df485ee525fcc38f27efdafeb5d48c330cc9
+    md5: ec31ba91f0feb2bbc6dd48f620e48129
+    sha256: b62403e12e321e41da0414cc810b5deb9aea0d51194ec57b5b813af5b7022b15
   manager: conda
   name: fonttools
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/fonttools-4.41.0-py310h8d17308_0.conda
-  version: 4.41.0
+  url: https://conda.anaconda.org/conda-forge/win-64/fonttools-4.42.0-py310h8d17308_0.conda
+  version: 4.42.0
+- category: main
+  dependencies:
+    cached-property: '>=1.3.0'
+    python: '>=2.7,<4'
+  hash:
+    md5: 642d35437078749ef23a5dca2c9bb1f3
+    sha256: 6cfd1f9bcd2358a69fb571f4b3af049b630d52647d906822dbedac03e84e4f63
+  manager: conda
+  name: fqdn
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2
+  version: 1.5.1
 - category: main
   dependencies:
     python: '>=3.6'
     python-dateutil: '>=2.8.1'
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
@@ -16545,22 +18444,22 @@
   url: https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.8.1-nompi_h8c042bf_106.tar.bz2
   version: 4.8.1
 - category: main
   dependencies:
     importlib-metadata: '>=4.4'
     python: '>=3.6'
   hash:
-    md5: 89ed59ad509c05db6f5f2f573d499bfe
-    sha256: e32ac2c95112caa8cd81f0cbc710f4f4903180a115c7260f03b010d5a0aa771b
+    md5: 6b8ab17bc8ff1ca89b3ea28ea3d566ca
+    sha256: cf1b3778cf99bd0301c4eb4f5d3d575e8c4248c15a019189b3892131a2675854
   manager: conda
   name: markdown
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda
-  version: 3.4.3
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.4-pyhd8ed1ab_0.conda
+  version: 3.4.4
 - category: main
   dependencies:
     markdown-it-py: '>=1.0.0,<4.0.0'
     python: '>=3.8'
   hash:
     md5: 6c5358a10873a15398b6f15f60cb5e1f
     sha256: 1ddac8d2be448cd1fbe49d2ca09df7e10d99679d53146a917f8bb4899f76d0ca
@@ -16609,22 +18508,35 @@
   url: https://conda.anaconda.org/conda-forge/win-64/pillow-9.2.0-py310hd4fb230_3.tar.bz2
   version: 9.2.0
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 044e7a1e0ad42c4e67110bd078150a63
-    sha256: 885611bd528abaf3e31bc0bfaad3a619cfe89db61d886b53c2a9ec9ff50edebe
+    md5: 0809187ef9b89a3d94a5c24d13936236
+    sha256: 1b5c0ca2f4260c7dd8cfccd8a641c1e41876c79dc594506be379cde08f5b471e
   manager: conda
   name: platformdirs
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda
-  version: 3.9.1
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.10.0-pyhd8ed1ab_0.conda
+  version: 3.10.0
+- category: main
+  dependencies:
+    importlib-metadata: '>=1.7.0'
+    python: '>=3.7'
+  hash:
+    md5: a6d1f61527c27fcc0165a6701a46b9f4
+    sha256: 6f6a66476908a1c109e36c852d934eedceb07e0cbc44d3fcd87c6f39521b57be
+  manager: conda
+  name: poetry-core
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-core-1.6.1-pyhd8ed1ab_0.conda
+  version: 1.6.1
 - category: main
   dependencies:
     latexcodec: '>=1.0.4'
     python: '>=3.6'
     pyyaml: '>=3.01'
     setuptools: ''
     six: ''
@@ -16635,31 +18547,48 @@
   name: pybtex
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2
   version: 0.24.0
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    typing-extensions: '>=4.6.0'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vc14_runtime: '>=14.29.30139'
+  hash:
+    md5: 1b2ffeb2d0c1f05218979ef85ccfa008
+    sha256: 25003ea6cf2e736781fc9926fd097eee189549232fb305f10df04b83abd0c625
+  manager: conda
+  name: pydantic-core
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.4.0-py310h87d50f1_0.conda
+  version: 2.4.0
+- category: main
+  dependencies:
     packaging: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     sip: ''
     toml: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: a4c757150f616bae079bc08cea956138
-    sha256: fde9316830224ba2903d8a8db97ca68628304af878c5caba0f1decc7336dc68e
+    md5: 571fa855e337706187fd018e1ba49fcd
+    sha256: a745addb44baa9ea87df07a4bae2f1ffcfeede5d1b6acbb698fd5ef1ab632720
   manager: conda
   name: pyqt5-sip
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.11.0-py310h00ffb61_3.conda
-  version: 12.11.0
+  url: https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py310h00ffb61_4.conda
+  version: 12.12.2
 - category: main
   dependencies:
     colorama: ''
     importlib-metadata: '>=0.22'
     packaging: '>=19.0'
     pyproject_hooks: ''
     python: '>=3.7'
@@ -16765,14 +18694,32 @@
   name: xorg-libx11
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/xorg-libx11-1.8.4-hcd874cb_0.conda
   version: 1.8.4
 - category: main
   dependencies:
+    cffi: '>=1.11'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vc14_runtime: '>=14.29.30139'
+    zstd: '>=1.5.2,<1.6.0a0'
+  hash:
+    md5: 82b3f10667553f6d262593a16851fbba
+    sha256: d0ab25221f8a914851e1095bed9e15487696011d6be7a3c2e90acb79213abd78
+  manager: conda
+  name: zstandard
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.19.0-py310h0009e47_2.conda
+  version: 0.19.0
+- category: main
+  dependencies:
     aiosignal: '>=1.1.2'
     async-timeout: <5.0,>=4.0.0a3
     attrs: '>=17.3.0'
     charset-normalizer: '>=2.0,<4.0'
     frozenlist: '>=1.1.1'
     multidict: '>=4.5,<7.0'
     python: '>=3.10,<3.11.0a0'
@@ -16822,30 +18769,43 @@
   name: black
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2
   version: 22.3.0
 - category: main
   dependencies:
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 38253361efb303deead3eab39ae9269b
+    sha256: 654a2488f77bf43555787d952dbffdc5d97956ff4aa9e0414a7131bb741dcf4c
+  manager: conda
+  name: conda-package-streaming
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.9.0-pyhd8ed1ab_0.conda
+  version: 0.9.0
+- category: main
+  dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    glib: '>=2.76.3,<3.0a0'
-    libglib: '>=2.76.3,<3.0a0'
+    glib: '>=2.76.4,<3.0a0'
+    libglib: '>=2.76.4,<3.0a0'
     libiconv: '>=1.17,<2.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 42f53931331420f6b748f91ef356a558
-    sha256: 5f9e74b2114872ed0ababbeaf5915a59729d1cc993a453de7584eaece1ddab91
+    md5: 489c30d6f35bdbea9a79c369cde19c6f
+    sha256: 07364ab63aff131a7bad064e4c0b83ca6856817f8ec206118c86ca6a20b3b708
   manager: conda
   name: gstreamer
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_1.conda
-  version: 1.22.4
+  url: https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.5-hb4038d2_0.conda
+  version: 1.22.5
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     freetype: '>=2.12.1,<3.0a0'
     graphite2: ''
     icu: '>=70.1,<71.0a0'
     libglib: '>=2.74.1,<3.0a0'
@@ -16859,14 +18819,27 @@
   name: harfbuzz
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/harfbuzz-6.0.0-he256f1b_0.conda
   version: 6.0.0
 - category: main
   dependencies:
+    arrow: '>=0.15.0'
+    python: '>=3.7'
+  hash:
+    md5: 4cb68948e0b8429534380243d063a27a
+    sha256: 7bb5c4d994361022f47a807b5e7d101b3dce16f7dd8a0af6ffad9f479d346493
+  manager: conda
+  name: isoduration
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2
+  version: 20.11.0
+- category: main
+  dependencies:
     platformdirs: '>=2.5'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     pywin32: '>=300'
     traitlets: '>=5.3'
   hash:
     md5: 39614170bdabdaa7531cb1dc2846c37c
@@ -16875,30 +18848,28 @@
   name: jupyter_core
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py310h5588dad_0.conda
   version: 5.3.1
 - category: main
   dependencies:
-    jsonschema: '>=3.2'
-    python: '>=3.7'
-    python-json-logger: '>=2.0.4'
-    pyyaml: '>=5.3'
-    rfc3339-validator: ''
-    rfc3986-validator: '>=0.1.1'
-    traitlets: '>=5.3'
+    importlib_metadata: '>=4.11.4'
+    jaraco.classes: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    pywin32-ctypes: ''
   hash:
-    md5: d98c5196ab6ffeb0c2feca2912801353
-    sha256: 16f73833537e05384d3eef27e62edb31de344d6d26666e1a465c1819014f2655
+    md5: 30210ff7bf71d7e193251e21d87f2838
+    sha256: 7544fc803f0a4b8a95c2ad2009dff5c6b9663352fd91b566a84f5a86479ed710
   manager: conda
-  name: jupyter_events
+  name: keyring
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda
-  version: 0.6.3
+  url: https://conda.anaconda.org/conda-forge/win-64/keyring-23.13.1-py310h5588dad_0.conda
+  version: 23.13.1
 - category: main
   dependencies:
     mkl: 2022.1.0 h6a75c08_874
   hash:
     md5: 9e42ac6b256b96bfaa19f829c25940e8
     sha256: 56c5394e80c429acfee53a075e3d1b6ccd8c294510084cd6a2a4b7d8cc80abfb
   manager: conda
@@ -16933,14 +18904,27 @@
   name: oauthlib
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2
   version: 3.2.2
 - category: main
   dependencies:
+    poetry-core: '>=1.6.0,<2.0.0'
+    python: '>=3.7,<4.0'
+  hash:
+    md5: 00893c7ea4f9f7620706e0aa94c01b6e
+    sha256: 54478b283b5967a85ee5da717f1512d7ec97eb07c7b52d1f2ad3cb080d56c0ac
+  manager: conda
+  name: poetry-plugin-export
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-plugin-export-1.4.0-pyhd8ed1ab_0.conda
+  version: 1.4.0
+- category: main
+  dependencies:
     python: '>=3.7'
     wcwidth: ''
   hash:
     md5: a4986c6bb5b0d05a38855b0880a5f425
     sha256: 10e7fdc75d4b85633be6b12a70b857053987127a808caa0f88b2cba4b3ce6359
   manager: conda
   name: prompt-toolkit
@@ -16962,14 +18946,29 @@
   name: pybtex-docutils
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pybtex-docutils-1.0.2-py310h5588dad_2.tar.bz2
   version: 1.0.2
 - category: main
   dependencies:
+    annotated-types: '>=0.4.0'
+    pydantic-core: 2.4.0
+    python: '>=3.7'
+    typing-extensions: '>=4.6.1'
+  hash:
+    md5: 7964a624018707909044b509f58b937a
+    sha256: ee8a995c201e83421f3fb24f359c609900b8891d99331fc23dae32166931d744
+  manager: conda
+  name: pydantic
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.1.1-pyhd8ed1ab_0.conda
+  version: 2.1.1
+- category: main
+  dependencies:
     cryptography: '>=38.0.0,<42,!=40.0.0,!=40.0.1'
     python: '>=3.6'
   hash:
     md5: 34f7d568bf59d18e3fef8c405cbece21
     sha256: 4daea3dc896987cc1334956fccfc0ed738663a84ad0c1d3f576a7a7936091534
   manager: conda
   name: pyopenssl
@@ -16993,14 +18992,29 @@
   name: simpleitk
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/simpleitk-2.2.1-py310hcf936e6_1.conda
   version: 2.2.1
 - category: main
   dependencies:
+    distlib: <1,>=0.3.7
+    filelock: <4,>=3.12.2
+    platformdirs: <4,>=3.9.1
+    python: '>=3.8'
+  hash:
+    md5: a218f3be8ab6185a475c8168a86e18ae
+    sha256: 3e508638077bcba79db4d26037c8e97bf6b7b43d156a06c9c25cdd2136468459
+  manager: conda
+  name: virtualenv
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.2-pyhd8ed1ab_0.conda
+  version: 20.24.2
+- category: main
+  dependencies:
     m2w64-gcc-libs: ''
     xorg-libx11: '>=1.7.2,<2.0a0'
     xorg-xextproto: ''
   hash:
     md5: 2aa695ac3c56193fd8d526e3b511e021
     sha256: 829320f05866ea1cc51924828427f215f4d0db093e748a662e3bb68b764785a4
   manager: conda
@@ -17025,14 +19039,28 @@
   name: xorg-libxt
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/xorg-libxt-1.3.0-hcd874cb_0.conda
   version: 1.3.0
 - category: main
   dependencies:
+    conda-package-streaming: '>=0.9.0'
+    python: '>=3.7'
+    zstandard: '>=0.15'
+  hash:
+    md5: 8a3ae7f6318376aa08ea753367bb7dd6
+    sha256: 9a221808405d813d8c555efce6944379b907d36d79e77d526d573efa6b996d26
+  manager: conda
+  name: conda-package-handling
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.2.0-pyh38be061_0.conda
+  version: 2.2.0
+- category: main
+  dependencies:
     black: '>=22.1.0'
     flake8: '>=3'
     python: '>=3.7'
     tomli: ''
   hash:
     md5: 61649e6e9b39ac0c7d10938025f6fe4f
     sha256: 736dbadccbd0ce6371ffa011b761c03bf9e9d329582d0c5daecdbff0e96e2a36
@@ -17041,31 +19069,52 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda
   version: 0.3.6
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    gstreamer: 1.22.4 hb4038d2_1
-    libglib: '>=2.76.3,<3.0a0'
+    gstreamer: 1.22.5 hb4038d2_0
+    libglib: '>=2.76.4,<3.0a0'
     libogg: '>=1.3.4,<1.4.0a0'
     libvorbis: '>=1.3.7,<1.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: ce797dd3d60901f6260e84e84674c829
-    sha256: 796b63de19fa87c76583e0253e02796937d635d98701976390494589b5109d54
+    md5: 56cea78b747eaf6e8ec60cfbbf0416ff
+    sha256: dc6613e6c9449ad511cc8f2874481a2da556880cf5fcb2a9ea29f6a8978e993b
   manager: conda
   name: gst-plugins-base
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_1.conda
-  version: 1.22.4
+  url: https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.5-h001b923_0.conda
+  version: 1.22.5
+- category: main
+  dependencies:
+    fqdn: ''
+    idna: ''
+    isoduration: ''
+    jsonpointer: '>1.13'
+    jsonschema: '>=4.17.3,<5.0a0'
+    python: ''
+    rfc3339-validator: ''
+    rfc3986-validator: '>0.1.0'
+    uri-template: ''
+    webcolors: '>=1.11'
+  hash:
+    md5: 7a709748e93f0b2c33d6b5b676b6d9d0
+    sha256: 767da9c47d64e1dc826d3173e46ff6fd4e858c94ff61d67ff4f976c7bc9502a2
+  manager: conda
+  name: jsonschema-with-format-nongpl
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.17.3-pyhd8ed1ab_0.conda
+  version: 4.17.3
 - category: main
   dependencies:
     importlib_metadata: '>=4.8.3'
     jupyter_core: '>=4.12,!=5.0.*'
     python: '>=3.8'
     python-dateutil: '>=2.8.2'
     pyzmq: '>=23.0'
@@ -17108,22 +19157,22 @@
   dependencies:
     jsonschema: '>=2.6'
     jupyter_core: ''
     python: '>=3.8'
     python-fastjsonschema: ''
     traitlets: '>=5.1'
   hash:
-    md5: 3ec35d84fc1775215061517eb4660693
-    sha256: d8b1ad3c219b39e5e325785606853ff1cd334769228490ac977b85aa95e94ba0
+    md5: 61ba076de6530d9301a0053b02f093d2
+    sha256: fc82c5a9116820757b03ffb836b36f0f50e4cd390018024dbadb0ee0217f6992
   manager: conda
   name: nbformat
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda
-  version: 5.9.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.2-pyhd8ed1ab_0.conda
+  version: 5.9.2
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     fontconfig: '>=2.14.2,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
     fribidi: '>=1.0.10,<2.0a0'
@@ -17213,14 +19262,36 @@
   name: botocore
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda
   version: 1.29.165
 - category: main
   dependencies:
+    certifi: ''
+    cryptography: '>=1.3.4'
+    idna: '>=2.0.0'
+    pyopenssl: '>=0.14'
+    pysocks: '>=1.5.6,<2.0,!=1.5.7'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    urllib3: ''
+    vc: '>=14.2,<15'
+    vc14_runtime: '>=14.29.30139'
+  hash:
+    md5: 9c3adc3bcee36c492dcaaa682741d0da
+    sha256: 7bd3298aef6a7b8fa4398f05a3524a4d71e362d8a8d575c50398b1d40f31a8a6
+  manager: conda
+  name: dulwich
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/dulwich-0.21.5-py310h8d17308_0.conda
+  version: 0.21.5
+- category: main
+  dependencies:
     __win: ''
     backcall: ''
     colorama: ''
     decorator: ''
     jedi: '>=0.16'
     matplotlib-inline: ''
     pickleshare: ''
@@ -17237,14 +19308,32 @@
   name: ipython
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda
   version: 8.14.0
 - category: main
   dependencies:
+    jsonschema-with-format-nongpl: '>=3.2'
+    python: '>=3.7'
+    python-json-logger: '>=2.0.4'
+    pyyaml: '>=5.3'
+    rfc3339-validator: ''
+    rfc3986-validator: '>=0.1.1'
+    traitlets: '>=5.3'
+  hash:
+    md5: 279fed93be42722de98e998ec80be8a1
+    sha256: 1b168cd11337dcbd2eae71b91ad7624c5afed0561e4f703d5eeee27e182f98c1
+  manager: conda
+  name: jupyter_events
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.7.0-pyhd8ed1ab_0.conda
+  version: 0.7.0
+- category: main
+  dependencies:
     expat: '>=2.4.8,<3.0a0'
     fontconfig: '>=2.13.96,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.10.4,<3.0a0'
     icu: '>=70.1,<71.0a0'
     jpeg: '>=9e,<10a'
     libpng: '>=1.6.37,<1.7.0a0'
@@ -17302,22 +19391,22 @@
     liblapack: '>=3.9.0,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 922f75b8698c5b9909bf03c658898117
-    sha256: 25e07d23dd78641537082fd9b0c4183784fcc1d84c65f207d6e2e7ede7702c8f
+    md5: faeadcd33c1207e7bedd0ee8621ba25a
+    sha256: 4418a99e711ed162b69d57f3c277f5e4999501dc80c89fb75f51cc59abfbcdc4
   manager: conda
   name: numpy
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.1-py310hd02465a_0.conda
-  version: 1.25.1
+  url: https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.2-py310hd02465a_0.conda
+  version: 1.25.2
 - category: main
   dependencies:
     gst-plugins-base: '>=1.22.0,<1.23.0a0'
     gstreamer: '>=1.22.0,<1.23.0a0'
     icu: '>=70.1,<71.0a0'
     jpeg: '>=9e,<10a'
     krb5: '>=1.20.1,<1.21.0a0'
@@ -17372,14 +19461,54 @@
   name: blas-devel
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/blas-devel-3.9.0-17_win64_mkl.conda
   version: 3.9.0
 - category: main
   dependencies:
+    msgpack-python: '>=0.5.2'
+    python: '>=3.6'
+    requests: '>=2.16.0'
+  hash:
+    md5: db23395890ef31be3c2320fb41b665b0
+    sha256: 99b68d1e9b1e148c9dfa5886cdd9b6082e968328658ba71a5b76cdc93a92ef02
+  manager: conda
+  name: cachecontrol
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.14-pyhd8ed1ab_0.conda
+  version: 0.12.14
+- category: main
+  dependencies:
+    boltons: '>=23.0.0'
+    conda-package-handling: '>=1.3.0'
+    jsonpatch: '>=1.32'
+    menuinst: '>=1.4.11,<2'
+    packaging: '>=23.0'
+    pluggy: '>=1.0.0'
+    pycosat: '>=0.6.3'
+    pyopenssl: '>=16.2.0'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    requests: '>=2.27.0,<3'
+    ruamel.yaml: '>=0.11.14,<0.18'
+    setuptools: '>=60.0.0'
+    toolz: '>=0.8.1'
+    tqdm: '>=4'
+  hash:
+    md5: 8d47d845a64022a75bd84f815ca66423
+    sha256: 212a20030f52691632d0c5324a42e3cc41af213e2a6a49ae270a5c3eedb8d08d
+  manager: conda
+  name: conda
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/conda-23.7.2-py310h5588dad_0.conda
+  version: 23.7.2
+- category: main
+  dependencies:
     numpy: '>=1.16'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
@@ -17389,14 +19518,30 @@
   name: contourpy
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/contourpy-1.1.0-py310h232114e_0.conda
   version: 1.1.0
 - category: main
   dependencies:
+    appdirs: ''
+    click: '>=5.1'
+    filelock: ''
+    python: '>=3.7'
+    requests: '>=2'
+  hash:
+    md5: c99ae3abf501990769047b4b40a98f17
+    sha256: b71784b6c24d2320b2f796d074e75e7dd1be7b7fc0f719c5cf3a582270b368d6
+  manager: conda
+  name: ensureconda
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2
+  version: 1.4.3
+- category: main
+  dependencies:
     aiohttp: '>=3.6.2,<4.0.0dev'
     cachetools: '>=2.0.0,<6.0'
     pyasn1-modules: '>=0.2.1'
     pyopenssl: '>=20.0.0'
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
@@ -17457,14 +19602,31 @@
   name: ipykernel
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda
   version: 6.23.3
 - category: main
   dependencies:
+    comm: '>=0.1.3'
+    ipython: '>=6.1.0'
+    jupyterlab_widgets: '>=3.0.7,<3.1.0'
+    python: '>=3.7'
+    traitlets: '>=4.3.1'
+    widgetsnbextension: '>=4.0.7,<4.1.0'
+  hash:
+    md5: 6fe1e9c8e93261e978998c0e90e36275
+    sha256: 71f920b0b89eb177511ff2d8bd9904c9c6c96d731f90ec97168cc28bc86ed623
+  manager: conda
+  name: ipywidgets
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.0-pyhd8ed1ab_0.conda
+  version: 8.1.0
+- category: main
+  dependencies:
     attrs: ''
     click: ''
     importlib-metadata: ''
     nbclient: '>=0.2,<0.8'
     nbformat: ''
     python: '>=3.8'
     pyyaml: ''
@@ -17495,22 +19657,22 @@
     packaging: ''
     pandocfilters: '>=1.4.1'
     pygments: '>=2.4.1'
     python: '>=3.8'
     tinycss2: ''
     traitlets: '>=5.0'
   hash:
-    md5: 32dde1678bb003c90d4bc0c2dbd21814
-    sha256: 76ad7689d35fe031459c422f142c9d8e7a02f6922049b7a0183fc70aaef02f0a
+    md5: 063c1fda5480050b8d989478c97a4c55
+    sha256: c5db2ba740b2ffddf11a5ba67a3afa7c05bff4656dae3d5f61a9b57c57ea3f8b
   manager: conda
   name: nbconvert-core
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     numpy: '>=1.19'
     packaging: '>=17'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
@@ -17554,31 +19716,48 @@
   name: pooch
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda
   version: 1.7.0
 - category: main
   dependencies:
-    pyqt5-sip: 12.11.0 py310h00ffb61_3
+    pyqt5-sip: 12.12.2 py310h00ffb61_4
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
-    qt-main: '>=5.15.6,<5.16.0a0'
-    sip: '>=6.7.5,<6.8.0a0'
+    qt-main: '>=5.15.8,<5.16.0a0'
+    sip: '>=6.7.10,<6.8.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 4012c5ed74c63b82c344e38cf3e68a26
-    sha256: 401d4650825a608bfae07f55bd6b7d0e302d026009efc495df7d1cb508b281db
+    md5: bf76044f5e0ac24513f386ea728862e6
+    sha256: 0874f118a20eadedee35281248deefff13f43629d12077c6c9f384664ca314db
   manager: conda
   name: pyqt
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.7-py310h1fd54f2_3.conda
-  version: 5.15.7
+  url: https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py310h1fd54f2_4.conda
+  version: 5.15.9
+- category: main
+  dependencies:
+    numpy: ''
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: 7e623c5592d080ea8211f94e3755ee76
+    sha256: 648ab3a1c42a8ce056c4ab11bd36f6d8023f9a124360b9c43037e87bcf78b704
+  manager: conda
+  name: rapidfuzz
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/rapidfuzz-2.15.1-py310h00ffb61_0.conda
+  version: 2.15.1
 - category: main
   dependencies:
     oauthlib: '>=3.0.0'
     python: '>=3.4'
     requests: '>=2.0.0'
   hash:
     md5: 61b279f051eef9c89d58f4d813e75e04
@@ -17587,14 +19766,27 @@
   name: requests-oauthlib
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2
   version: 1.3.1
 - category: main
   dependencies:
+    python: '>=3.6'
+    requests: '>=2.0.1,<3.0.0'
+  hash:
+    md5: 99c98318c8646b08cc764f90ce98906e
+    sha256: 20eaefc5dba74ff6c31e537533dde59b5b20f69e74df49dff19d43be59785fa3
+  manager: conda
+  name: requests-toolbelt
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
+  version: 1.0.0
+- category: main
+  dependencies:
     botocore: '>=1.12.36,<2.0a.0'
     python: '>=3.7'
   hash:
     md5: b19a857ac845097e9c823c9f4d35f80e
     sha256: 99512bf4f4e297cc7565c94eee8ccc908411f836b341668e2b5d064273e21762
   manager: conda
   name: s3transfer
@@ -17709,14 +19901,58 @@
   name: boto3
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda
   version: 1.26.165
 - category: main
   dependencies:
+    cachecontrol: 0.12.14 pyhd8ed1ab_0
+    lockfile: '>=0.9'
+    python: '>=3.6'
+  hash:
+    md5: 43ed0c094b39bb352382db8105ab0b94
+    sha256: 23af777f65d74f18aaee1641add3b15bd442096f9c4940270151704f1aa38198
+  manager: conda
+  name: cachecontrol-with-filecache
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.14-pyhd8ed1ab_0.conda
+  version: 0.12.14
+- category: main
+  dependencies:
+    crashtest: '>=0.4.1,<0.5.0'
+    python: '>=3.7,<4.0'
+    rapidfuzz: '>=2.2.0,<3.0.0'
+  hash:
+    md5: f1c5f2af6676cbe9206e191d1e70f661
+    sha256: cf9bc4c9356ad8eb68512446eebc076386f2bfb8ca86626e8796621bc5a13082
+  manager: conda
+  name: cleo
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/cleo-2.0.1-pyhd8ed1ab_0.conda
+  version: 2.0.1
+- category: main
+  dependencies:
+    conda: '>=4.3'
+    jinja2: ''
+    packaging: ''
+    python: '>=3.6'
+    pyyaml: ''
+  hash:
+    md5: 9b175e69c1c601d01ab5edccf822363c
+    sha256: 3244e025f3d185f56fb44a44d02526797ce3e95302a868867af6dc9e2e55ebe3
+  manager: conda
+  name: conda-devenv
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-devenv-2.3.0-pyhd8ed1ab_0.tar.bz2
+  version: 2.3.0
+- category: main
+  dependencies:
     click: '>=6.0.0'
     google-auth: '>=2.15.0'
     python: '>=3.6'
     requests-oauthlib: '>=0.7.0'
   hash:
     md5: 569e62e95b01b53e4ec7d9abe83b7385
     sha256: f89613643658a51a1ac0fb7c7950526fadc2a6ce1ae13755d786e14cfce1633c
@@ -17724,31 +19960,14 @@
   name: google-auth-oauthlib
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda
   version: 1.0.0
 - category: main
   dependencies:
-    ipykernel: '>=4.5.1'
-    ipython: '>=6.1.0'
-    jupyterlab_widgets: '>=3.0.7,<3.1.0'
-    python: '>=3.7'
-    traitlets: '>=4.3.1'
-    widgetsnbextension: '>=4.0.7,<4.1.0'
-  hash:
-    md5: 4b0f4e8fe2a303e472674eae0340bdad
-    sha256: 3b17ad90294f0684fca9191f1e696e9b4f03a652d5e588b6ff0feb5647fcf116
-  manager: conda
-  name: ipywidgets
-  optional: false
-  platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda
-  version: 8.0.7
-- category: main
-  dependencies:
     ipykernel: '>=6.14'
     ipython: ''
     jupyter_client: '>=7.0.0'
     jupyter_core: '>=4.12,!=5.0.*'
     prompt_toolkit: '>=3.0.30'
     pygments: ''
     python: '>=3.7'
@@ -17837,26 +20056,26 @@
   name: myst-parser
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2
   version: 0.18.1
 - category: main
   dependencies:
-    nbconvert-core: 7.7.1 pyhd8ed1ab_1
+    nbconvert-core: 7.7.3 pyhd8ed1ab_0
     pandoc: ''
     python: '>=3.8'
   hash:
-    md5: 796b056965d7146bcac082fa2a83943d
-    sha256: b5b2823e7951a5ba41b1020b7cce109fec7f2ebe540234bf8a17c54615c2f679
+    md5: f44109e52a40b8149156f5ddd9c11b26
+    sha256: c9fceb914dd4a8fe64b1403a0c7b0c69b5c67fc726aa8239e5ecb450d27e6963
   manager: conda
   name: nbconvert-pandoc
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     accessible-pygments: ''
     babel: ''
     beautifulsoup4: ''
     docutils: '!=0.17.0'
     packaging: ''
@@ -18131,26 +20350,26 @@
   name: myst-nb
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda
   version: 0.17.2
 - category: main
   dependencies:
-    nbconvert-core: 7.7.1 pyhd8ed1ab_1
-    nbconvert-pandoc: 7.7.1 pyhd8ed1ab_1
+    nbconvert-core: 7.7.3 pyhd8ed1ab_0
+    nbconvert-pandoc: 7.7.3 pyhd8ed1ab_0
     python: '>=3.8'
   hash:
-    md5: 95d9d1523df069792cd059f412be0d6e
-    sha256: c49a87861db316b322f919825820bc7193cbfa8a4a8b21b5ffe16a133644d400
+    md5: f53d92ecd7d8563b006107f6a33e55c6
+    sha256: 2b9e7bc41ee0882d7829e984cb1a18f039a5f756b5b747f6a3ce352bc72e5103
   manager: conda
   name: nbconvert
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda
-  version: 7.7.1
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.3-pyhd8ed1ab_0.conda
+  version: 7.7.3
 - category: main
   dependencies:
     jupyter_server: '>=1.8,<3'
     python: '>=3.7'
   hash:
     md5: 67e0fe74c156267d9159e9133df7fd37
     sha256: f028d7ad1f2175cde307db08b60d07e371b9d6f035cfae6c81ea94b4c408c538
@@ -18158,14 +20377,55 @@
   name: notebook-shim
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda
   version: 0.2.3
 - category: main
   dependencies:
+    __win: ''
+    backports.cached-property: '>=1.0.2,<2.0.0'
+    cachecontrol-with-filecache: '>=0.12.9,<0.13.0'
+    cleo: '>=2.0.0,<3.0.0'
+    crashtest: '>=0.4.1,<0.5.0'
+    dulwich: '>=0.21.2,<0.22.0'
+    filelock: '>=3.8.0,<4.0.0'
+    html5lib: '>=1.0.0,<2.0.0'
+    importlib-metadata: '>=4.4'
+    jsonschema: '>=4.10.0,<5.0.0'
+    keyring: '>=23.9.0,<24.0.0'
+    lockfile: '>=0.12.2,<0.13.0'
+    packaging: '>=20.4'
+    pexpect: '>=4.7.0,<5.0.0'
+    pkginfo: '>=1.9.4,<2.0'
+    platformdirs: '>=3.0.0,<4.0.0'
+    poetry-core: 1.6.1.*
+    poetry-plugin-export: '>=1.4.0,<2.0.0'
+    pyproject_hooks: '>=1.0.0,<2.0.0'
+    python: '>=3.7.0,<4.0.0'
+    python-build: '>=0.10.0,<0.11.0'
+    python-installer: '>=0.7.0,<0.8.0'
+    requests: '>=2.18,<3.0'
+    requests-toolbelt: '>=0.9.1,<2'
+    shellingham: '>=1.5.0,<2.0.0'
+    tomli: '>=2.0.1,<3.0.0'
+    tomlkit: '>=0.11.4,<1.0.0'
+    trove-classifiers: '>=2022.5.19'
+    urllib3: '>=1.26.0,<2.0.0'
+    virtualenv: '>=20.22.0,<21.0.0'
+  hash:
+    md5: 278a253d341cdb93af47a14c794f6c02
+    sha256: 03eee33329dceb0b2a5d88eac3bff5a316bf75046f4634b53d1e6816588325a8
+  manager: conda
+  name: poetry
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/poetry-1.5.1-win_pyhd8ed1ab_0.conda
+  version: 1.5.1
+- category: main
+  dependencies:
     blas: '* mkl'
     filelock: ''
     intel-openmp: ''
     jinja2: ''
     libuv: '>=1.44.2,<2.0a0'
     mkl: '>=2018'
     networkx: ''
@@ -18268,14 +20528,38 @@
   name: tensorboard
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda
   version: 2.13.0
 - category: main
   dependencies:
+    click: '>=8.0'
+    click-default-group: ''
+    ensureconda: '>=1.3'
+    jinja2: ''
+    poetry: ''
+    pydantic: '>=1.8.1'
+    python: '>=3.6'
+    pyyaml: '>=5.1'
+    requests: '>=2'
+    ruamel.yaml: ''
+    setuptools: ''
+    toml: ''
+    typing-extensions: ''
+  hash:
+    md5: 1c31d380288fc1599fb5f4c76c8c828c
+    sha256: 2895546468293f358395b072846ebf8a2e04339d1355009fb96787d804250bb0
+  manager: conda
+  name: conda-lock
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.0.5-pyhd8ed1ab_1.tar.bz2
+  version: 1.0.5
+- category: main
+  dependencies:
     click: '>=7.1,<9'
     docutils: '>=0.15,<0.19'
     jinja2: ''
     jsonschema: <5
     linkify-it-py: '>=2.0.0,<2.1.0'
     myst-nb: '>=0.17.1,<0.18.0'
     python: '>=3.7'
@@ -18415,22 +20699,22 @@
     pytorch: '>=1.11.0'
     pyyaml: '>=5.4'
     requests: ''
     torchmetrics: '>=0.7.0'
     tqdm: '>=4.57.0'
     typing_extensions: '>=4.0.0'
   hash:
-    md5: ce9d626b181c6f8cceb5047f6a819f7d
-    sha256: a049296b4b33bceedf3bafd378e8a4112bca71b453734f1e0daaca2a72598593
+    md5: 5325b6adf171d4d69968100af806994e
+    sha256: 54efb4be9a8f73692cf24f85923a226c0ed6d035000704479b0f27288bb0a874
   manager: conda
   name: pytorch-lightning
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda
-  version: 2.0.4
+  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.6-pyhd8ed1ab_0.conda
+  version: 2.0.6
 - category: main
   dependencies:
     ipykernel: ''
     ipywidgets: ''
     jupyter_console: ''
     nbconvert: ''
     notebook: ''
```

### Comparing `hf-deepali-0.4.2/conda/environment.devenv.yml` & `hf-deepali-0.4.3/conda/environment.devenv.yml`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
   - python =3.10
   # Installation tools
   - pip =23.1
   - setuptools =67.7
   - setuptools-scm =7.1
   # Developer tools
   - black =22.3
+  - conda-devenv=2.3
+  - conda-lock=1.0
   - docutils =0.17
   - flake8 =6.0
   - flake8-black =0.3.6
   - ghp-import =2.1
   - graphviz =7.0
   - ipykernel =6.23
   - jupyter =1.0
@@ -35,15 +37,14 @@
   - deprecation =2.1
   - nibabel =5.1
   - numpy =1.25
   - pandas =1.5
   - pytorch =2.0,!=2.0.0  # ["osx" not in get_env("PLATFORM")]
   - pytorch-cuda =11.8  # ["osx" not in get_env("PLATFORM")]
   - pytorch::pytorch =2.0,!=2.0.0  # ["osx" in get_env("PLATFORM")]
-  - pyyaml =6.0
   - ruamel.yaml =0.17
   - SimpleITK =2.2
   # Utility libraries
   - boto3 =1.26
   - matplotlib =3.7
   - scipy =1.10
   - tensorboard =2.13
```

### Comparing `hf-deepali-0.4.2/conda/environment.linux-64.lock` & `hf-deepali-0.4.3/conda/environment.linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: c6bd68ba63788a00937c8cd1d91bb1e5813d242d7089005156ab1a663f53aee1
+# input_hash: 586016f05a089668afa3f0a057304e5826b41e87317e8d51969529896659d6a0
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.7.22-hbcca054_0.conda#a73ecd2988327ad4c8f2c331482917f2
 https://conda.anaconda.org/nvidia/linux-64/cuda-cudart-11.8.89-0.tar.bz2#b68c7ef3eda01e95d5903fb508c5e440
 https://conda.anaconda.org/nvidia/linux-64/cuda-cupti-11.8.87-0.tar.bz2#2f4b4933285400137cf029fef9a7daa6
 https://conda.anaconda.org/nvidia/linux-64/cuda-nvrtc-11.8.89-0.tar.bz2#f4af75ee32661708c979630cdb8f4987
 https://conda.anaconda.org/nvidia/linux-64/cuda-nvtx-11.8.86-0.tar.bz2#1825ffc3feb608f2752073935e90bb49
 https://conda.anaconda.org/conda-forge/noarch/cuda-version-12.0-hffde075_2.conda#c9f9d925118c389a1a3f4267b6272b98
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
@@ -35,15 +35,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.8-h166bdaf_0.tar.bz2#be733e69048951df1e4b4b7bb8c7666f
 https://conda.anaconda.org/conda-forge/linux-64/aom-3.5.0-h27087fc_0.tar.bz2#a08150fd2298460cd1fcccf626305642
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.19.1-hd590300_0.conda#e8c18d865be43e2fb3f7a145b6adf1f5
 https://conda.anaconda.org/conda-forge/linux-64/double-conversion-3.2.0-h27087fc_1.tar.bz2#5a7e0df95874e7ffe8b7840907058563
-https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.1-h00ab1b0_0.conda#c2acfc9bc0d0c53f83bbf0f582cb0e7a
+https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.0-h00ab1b0_0.conda#b1b879d6d093f55dd40d58b5eb2f0699
 https://conda.anaconda.org/conda-forge/linux-64/fftw-3.3.10-nompi_hc118613_108.conda#6fa90698000b05dfe8ce6515794fe71a
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
 https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.1-h0b41bf4_3.conda#96f3b11872ef6fad973eac856cd2624f
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-orc-0.4.34-hd590300_0.conda#7ea223fa114cc8134b8c4d398d3e5afe
@@ -79,15 +79,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
 https://conda.anaconda.org/conda-forge/linux-64/nettle-3.8.1-hc379101_1.tar.bz2#3cb2c7df59990bd37c2ce27fd906de68
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openh264-2.3.1-hcb278e6_2.conda#37d01894f256b2a6921c5a218f42f8a2
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.2-hd590300_0.conda#e5ac5227582d6c83ccf247288c0eb095
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
 https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
 https://conda.anaconda.org/conda-forge/linux-64/pugixml-1.11.4-h59595ed_1.conda#32835434dcf8ca46d357a76fbd1f152b
 https://conda.anaconda.org/conda-forge/linux-64/re2-2023.03.02-h8c504da_0.conda#206f8fa808748f6e90599c3368a1114e
 https://conda.anaconda.org/conda-forge/linux-64/svt-av1-1.4.1-hcb278e6_0.conda#2b32b8a10fa6ec9c18c897c4527720dc
 https://conda.anaconda.org/conda-forge/linux-64/x264-1!164.3095-h166bdaf_2.tar.bz2#6c99772d483f566d59e25037fea2c4b1
 https://conda.anaconda.org/conda-forge/linux-64/x265-3.5-h924138e_3.tar.bz2#e7f6ed84d4623d52ee581325c1587a6b
@@ -160,31 +160,36 @@
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-h516909a_0.tar.bz2#a88ab22508ba067b689dc12696157cee
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h516909a_0.tar.bz2#d04a6285315c4f03ebaf37355be272f9
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-h166bdaf_0.tar.bz2#732e22f1741bccea861f5668cf7342a7
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h516909a_0.tar.bz2#847df113dba16f0079758cacf9024409
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.4-h0b41bf4_0.conda#ea8fbfeb976ac49cbeb594e985393514
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
+https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
+https://conda.anaconda.org/conda-forge/noarch/boltons-23.0.0-pyhd8ed1ab_0.conda#033eb25fffd222aceeca6d58cd953680
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
+https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
-https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.7.22-pyhd8ed1ab_0.conda#7f3dbc9179b4dde7da98dfb151d0ad22
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py310heca2aa9_0.conda#8ffb020d2b722c962f0b4f06a304f533
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.8-py310hc6cd4ac_0.conda#397d3d6153c0b8de807e1bdc58b16013
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda#12d8aae6994f342618443a8f05c652a0
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py310hff52083_3.tar.bz2#785160da087cf1d70e989afbb761f01c
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
@@ -196,68 +201,77 @@
 https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py310hc6cd4ac_1.conda#934c4eb3214284125eff6dd665e9568a
 https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.56.2-py310h1b8f574_0.conda#0828bcffd8123a89f688e83ba95a356b
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
+https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
+https://conda.anaconda.org/conda-forge/noarch/jsonpointer-2.0-py_0.tar.bz2#07d85c22a3beb102a48cd123df84c2a6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py310hbf28c38_1.tar.bz2#ad5647e517ba68e2868ef2e6e6ff7723
 https://conda.anaconda.org/conda-forge/linux-64/lazy-object-proxy-1.9.0-py310h1fa729e_0.conda#8664f43451412071a7111211fe7e38f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.14-h6ed2654_0.tar.bz2#dcc588839de1445d90995a0a2c4f3a39
-https://conda.anaconda.org/conda-forge/linux-64/libclang13-15.0.7-default_h9986a30_2.conda#907344cee64101d44d806bbe0fccb01d
+https://conda.anaconda.org/conda-forge/linux-64/libclang13-15.0.7-default_h9986a30_3.conda#1720df000b48e31842500323cb7be18c
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
 https://conda.anaconda.org/conda-forge/linux-64/libpq-15.3-hbcd7760_1.conda#8afb2a97d256ffde95b91a6283bc598c
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-253-h8c4010b_1.conda#9176b1e2cb8beca37a7510b0e801e38f
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-1.2.4-h522a892_0.tar.bz2#802e43f480122a85ae6a34c1909f8f98
+https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
 https://conda.anaconda.org/conda-forge/linux-64/loguru-0.7.0-py310hff52083_0.conda#9e0d689557f3fdcb521c1239c13d29ec
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py310h2372a71_0.conda#5597d9f9778af6883ae64f0e7d39416c
 https://conda.anaconda.org/conda-forge/noarch/mccabe-0.7.0-pyhd8ed1ab_0.tar.bz2#34fc335fc50eef0b5ea708f2b5f54e0c
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
+https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.1.0-pyhd8ed1ab_0.conda#8549fafed0351bbfaa1ddaa15fdf9b4e
 https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda#dbf6e2d89137da32fa6670f3bffc024e
+https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py310hdf3cbec_0.conda#5311a49aaea44b73935c84a6d9a68e5f
 https://conda.anaconda.org/conda-forge/linux-64/multidict-6.0.4-py310h1fa729e_0.conda#b33287be963a70f8fb4b143b4561ba62
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-h7d73246_1.tar.bz2#a11b4df9271a8d7917686725aa04c8f2
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
+https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.2-pyhd8ed1ab_0.conda#e41debb259e68490e3ab81e46b639ab6
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
+https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py310h1fa729e_0.conda#b0f0a014fc04012c05f39df15fe270ce
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
+https://conda.anaconda.org/conda-forge/linux-64/pycosat-0.6.4-py310h5764c6d_1.tar.bz2#0e565d732f6660374b45d76761c09b06
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyflakes-3.0.1-pyhd8ed1ab_0.conda#44b7d77d96560c93e0e11437a3c35254
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda#912c0194f898fdb783021fd25f913c31
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
 https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py310h1fa729e_0.conda#f732bec05ecc2e302a868d971ae484e0
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.18.0-pyhd8ed1ab_0.conda#3be9466311564f80f8056c0851fc5bb7
+https://conda.anaconda.org/conda-forge/noarch/python-installer-0.7.0-pyhd8ed1ab_0.conda#65dea78f903d686c8b0c2feaf0e15e1f
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/pytorch/linux-64/pytorch-cuda-11.8-h7e8668a_5.tar.bz2#48e990086eb245cce92f09b45a34651e
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py310h5764c6d_5.tar.bz2#9e68d2ff6d98737c855b65f48dd3c597
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py310h5bbb5d0_0.conda#58017b4bb8fec6088a8b9ae44744ce4b
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py310h1fa729e_1.conda#2f9b517412af46255cef5e53a22c264e
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.1-pyhd8ed1ab_0.conda#1de44299f48f522caa2e0074231614e1
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
@@ -265,59 +279,71 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/linux-64/tbb-2021.9.0-hf52228f_0.conda#f495e42d3d2020b025705625edf35490
 https://conda.anaconda.org/conda-forge/linux-64/tensorboard-data-server-0.7.0-py310h34c0648_0.conda#350fb40a1b4820cf02f546dfe6764fe9
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.1-pyha770c72_0.conda#62f5b331c53d73e2f6c4c130b53518a0
+https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py310h2372a71_0.conda#1c510e74c87dc9b8fe1f7f9e8dbcef96
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2023.7.6-pyhd8ed1ab_0.conda#c9918f6a3973e28a792e747289734cd3
 https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.5-py310h2372a71_0.conda#48d1b46a82b8b4fb6057711dd213977f
+https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2#e6573ac68718f17b9d4f5c8eda3190f2
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py310h5764c6d_0.tar.bz2#e972c5a1f472561cf4a91962cb01f4b4
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
+https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
+https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.41.0-pyhd8ed1ab_0.conda#66beb36a1fa7e0dc9d9bf843a80eb82c
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/linux-64/wrapt-1.15.0-py310h1fa729e_0.conda#cbfdcc9c243ac7f080cf60833b482f97
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h166bdaf_0.tar.bz2#c9b568bd804cb2903c6be6f5f68182e4
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxfixes-5.0.3-h7f98852_1004.tar.bz2#e9a21aa4d5e3e5f1aed71e8cefd46b6a
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxt-1.3.0-hd590300_0.conda#ab2044e8d87dda9f74652e8e084a5569
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
+https://conda.anaconda.org/conda-forge/noarch/backports.cached-property-1.0.2-pyhd8ed1ab_0.tar.bz2#0e1df3978dd516e20ef88c86d51e5432
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-ha61ee94_1014.tar.bz2#d1a88f3ed5b52e1024b80d4bcd26a7a0
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_3.conda#800596144bb613cd7ac58b80900ce835
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.4-pyhd8ed1ab_0.conda#c8eaca39e2b6abae1fc96acc929ae939
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.41.0-py310h2372a71_0.conda#606aea800172f81896b21cabc5575206
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.42.0-py310h2372a71_0.conda#f939fe2998c888a77b310926a6c666f3
 https://conda.anaconda.org/conda-forge/linux-64/glew-2.1.0-h9c3ff4c_2.tar.bz2#fb05eb5c47590b247658243d27fc32f1
 https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.4-hfc55251_0.conda#dbcec5fd9c6c8be24b23575048755a59
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.12.2-nompi_h4df4325_101.conda#162a25904af6586b234b2dd52ee99c61
+https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda#e9f79248d30e942f7c358ff21a1790f5
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.0-pyhd8ed1ab_0.conda#1cd7f70057cdffc10977b613fb75425d
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/noarch/jsonpatch-1.32-pyhd8ed1ab_0.tar.bz2#09150b51b0528a31a0f6500b96fdde82
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
-https://conda.anaconda.org/conda-forge/linux-64/libclang-15.0.7-default_h7634d5b_2.conda#1a4fe5162abe4a19b5a9dedf158a0ff9
+https://conda.anaconda.org/conda-forge/linux-64/libclang-15.0.7-default_h7634d5b_3.conda#0922208521c0463e690bbaebba7eb551
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h18fbbfe_3.tar.bz2#ea9758cf553476ddf75c789fdd239dc5
 https://conda.anaconda.org/conda-forge/linux-64/libva-2.18.0-h0b41bf4_0.conda#56e049224de34bbe0478aad422227942
 https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda#c71f7ec8b80a536e58b979299b230251
 https://conda.anaconda.org/conda-forge/noarch/linkify-it-py-2.0.0-pyhd8ed1ab_0.tar.bz2#25b93e66067eb496ac10da888e25cc33
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/linux-64/mkl-2022.1.0-h84fe81f_915.tar.bz2#b9c8f925797a93dbff45e1626b025a6b
@@ -333,105 +359,129 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2#03bf410858b2cefc267316408a77c436
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py310h2372a71_0.conda#9a03abf74d5069bda767c1bce7a41e0b
-https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py310hc6cd4ac_0.conda#a3217e1bff09702dfdfcb536825fc12d
+https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.11-py310hc6cd4ac_0.conda#be1a7e420b7bac4ee02353d0e3161918
 https://conda.anaconda.org/conda-forge/noarch/sympy-1.12-pypyh9d50eac_103.conda#2f7d6347d7acf6edf1ac7f2189f44c8f
 https://conda.anaconda.org/conda-forge/linux-64/tbb-devel-2021.9.0-hf52228f_0.conda#b44ecd26bd0318a9eef65705483c70bc
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/werkzeug-2.3.6-pyhd8ed1ab_0.conda#55fbbb3e67185820ee2007395bfe0073
 https://conda.anaconda.org/conda-forge/linux-64/yarl-1.9.2-py310h2372a71_0.conda#73deaf595eb21f3e76a02ba1ae2edee6
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py310h5764c6d_3.tar.bz2#12f70cd23e4ea88f913dba50b0f0aba0
+https://conda.anaconda.org/conda-forge/noarch/arrow-1.2.3-pyhd8ed1ab_0.tar.bz2#fd1967c76eda3a3dd9e8e6cb7a15a028
 https://conda.anaconda.org/conda-forge/linux-64/astroid-2.15.6-py310hff52083_0.conda#8ad02555d6ecdb8fd5f1963690c59699
 https://conda.anaconda.org/conda-forge/noarch/async-timeout-4.0.2-pyhd8ed1ab_0.tar.bz2#25e79f9a1133556671becbd65a170c78
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py310h5764c6d_1005.tar.bz2#87669c3468dff637bbd0363bc0f895cf
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.2-py310h75e40e8_0.conda#3e80a669e7a1890ebb91370f2e818129
 https://conda.anaconda.org/conda-forge/linux-64/ffmpeg-5.1.2-gpl_h8dda1f0_106.conda#6845420373a9e260942bfbc5c786a4bb
+https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2#6d8d61116031a3f5b1f32e7899785866
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.0-h25f0c4b_2.conda#461541cb1b387c2a28ab6217f3d38502
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-6.0.0-h8e241bc_0.conda#448fe40d2fed88ccf4d9ded37cbb2b38
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-16_linux64_mkl.tar.bz2#85f61af03fd291dae33150ffe89dc09a
 https://conda.anaconda.org/conda-forge/linux-64/libitk-5.3.0-hcedbc38_0.conda#85b4afd676357f69ab154096f1977884
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.8.1-nompi_h261ec11_106.tar.bz2#9b25de670ce5753a33c18b1090d1d3bf
-https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
+https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.4-pyhd8ed1ab_0.conda#6b8ab17bc8ff1ca89b3ea28ea3d566ca
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/mkl-devel-2022.1.0-ha770c72_916.tar.bz2#69ba49e445f87aea2cba343a71a35ca2
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.10.0-pyhd8ed1ab_0.conda#0809187ef9b89a3d94a5c24d13936236
+https://conda.anaconda.org/conda-forge/noarch/poetry-core-1.6.1-pyhd8ed1ab_0.conda#a6d1f61527c27fcc0165a6701a46b9f4
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-daemon-16.1-ha8d29e2_3.conda#34d9d75ca896f5919c372a34e25f23ea
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py310heca2aa9_3.conda#3b1946b676534472ce65181dda0b9554
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.4.0-py310hcb5633a_0.conda#10c338c86b8b23f150948de8a80e70e5
+https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.12.2-py310hc6cd4ac_4.conda#345beb10601d5360a15c033d68165a4f
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
 https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.19-py310h2372a71_0.conda#2460f5ca3ab3265b80ee06a1d4b5b374
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.19.0-py310h1275a96_2.conda#a2b48edcd52593cdf007158ce10e1520
 https://conda.anaconda.org/conda-forge/linux-64/aiohttp-3.8.5-py310h2372a71_0.conda#0b05c509a96d0bf4bb424fe184170795
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
+https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.9.0-pyhd8ed1ab_0.conda#38253361efb303deead3eab39ae9269b
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.0-h4243ec0_2.conda#0d0c6604c8ac4ad5e51efa7bb58da05c
+https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py310hff52083_0.conda#63264f5a6dd5483475968016b614f525
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-16_linux64_mkl.tar.bz2#361bf757b95488de76c4f123805742d3
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-16_linux64_mkl.tar.bz2#a2f166748917d6d6e4707841ca1f519e
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
 https://conda.anaconda.org/conda-forge/linux-64/pango-1.50.14-hd33c08f_0.conda#a8b9e35dd7be2c945b0de4fe19a7c3a9
+https://conda.anaconda.org/conda-forge/noarch/poetry-plugin-export-1.4.0-pyhd8ed1ab_0.conda#00893c7ea4f9f7620706e0aa94c01b6e
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-16.1-hcb278e6_3.conda#8b452ab959166d91949af4c2d28f81db
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.2-py310hff52083_2.tar.bz2#dc929612cad7834bb4726a4de6575a3c
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.1.1-pyhd8ed1ab_0.conda#7964a624018707909044b509f58b937a
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py310hff52083_1.tar.bz2#e135d0e3bbb226e8d53d31b4e4f6d93c
 https://conda.anaconda.org/conda-forge/linux-64/simpleitk-2.2.1-py310h2b9ea3a_1.conda#ec09bbee37ea5d3b6022bab2e9b4d5a4
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.2-pyhd8ed1ab_0.conda#a218f3be8ab6185a475c8168a86e18ae
+https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.2.0-pyh38be061_0.conda#8a3ae7f6318376aa08ea753367bb7dd6
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
 https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h90689f9_2.tar.bz2#957a0255ab58aaf394a91725d73ab422
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.17.3-pyhd8ed1ab_0.conda#7a709748e93f0b2c33d6b5b676b6d9d0
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/linux-64/keyring-23.13.1-py310hff52083_0.conda#85da2982e8456156e2f38e6a3f75cd89
 https://conda.anaconda.org/conda-forge/linux-64/liblapacke-3.9.0-16_linux64_mkl.tar.bz2#44ccc4d4dca6a8d57fa17442bc64b5a1
 https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.54.4-h7abd40a_0.tar.bz2#921e53675ed5ea352f022b79abab076a
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.1-py310ha4c1d20_0.conda#3810cbf2635cb1d0edb97715d4ad74e7
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.2-pyhd8ed1ab_0.conda#61ba076de6530d9301a0053b02f093d2
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.2-py310ha4c1d20_0.conda#188e72aa313da668464e35309e9a32b0
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h5d23da1_6.conda#59c73debd9405771690ddbbad6c57b69
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/linux-64/blas-devel-3.9.0-16_linux64_mkl.tar.bz2#3f92c1c9e1c0e183462c5071aa02cae1
 https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py310hd41b1e2_0.conda#684399f9ddc0b9d6f3b6164f6107098e
+https://conda.anaconda.org/conda-forge/linux-64/dulwich-0.21.5-py310h2372a71_0.conda#58ee4d1dd828531bb6d69fd6bd304882
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-7.0.5-h2e5815a_0.conda#96bf06b24d74a5bf826485e9032c9312
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.7.0-pyhd8ed1ab_0.conda#279fed93be42722de98e998ec80be8a1
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
 https://conda.anaconda.org/conda-forge/linux-64/nibabel-5.1.0-py310hff52083_2.conda#01c0095d68f52a2ebe4154974b668bef
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py310h9b08913_1.conda#331c9dd2560aeb308e26f821280f19d0
-https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py310hab646b1_3.conda#d049da3204bf5ecb54a852b622f2d7d2
+https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.9-py310h04931ad_4.conda#db878a0696f9a7980171fd3cf29cca22
+https://conda.anaconda.org/conda-forge/linux-64/rapidfuzz-2.15.1-py310heca2aa9_0.conda#542887fb70fae388f9df109866469ca1
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/linux-64/vtk-9.2.5-qt_py310hc895abb_200.conda#3462cb0fb18182f4203cdb6e73434a31
 https://conda.anaconda.org/conda-forge/linux-64/blas-2.116-mkl.tar.bz2#c196a26abf6b4f132c88828ab7c2231c
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.14-pyhd8ed1ab_0.conda#db23395890ef31be3c2320fb41b665b0
+https://conda.anaconda.org/conda-forge/noarch/cleo-2.0.1-pyhd8ed1ab_0.conda#f1c5f2af6676cbe9206e191d1e70f661
+https://conda.anaconda.org/conda-forge/linux-64/conda-23.7.2-py310hff52083_0.conda#c5d666e682ca57f5853304d1fe82c131
+https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda#5583192796d1ebcf39b1e3e0958aa259
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.0-pyhd8ed1ab_0.conda#6fe1e9c8e93261e978998c0e90e36275
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.2-py310hf38f957_0.conda#9b55c9041c5a7f80f184a2cb05ec9663
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.3-pyhd8ed1ab_0.conda#063c1fda5480050b8d989478c97a4c55
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
+https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.14-pyhd8ed1ab_0.conda#43ed0c094b39bb352382db8105ab0b94
+https://conda.anaconda.org/conda-forge/noarch/conda-devenv-2.3.0-pyhd8ed1ab_0.tar.bz2#9b175e69c1c601d01ab5edccf822363c
 https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.2-py310hff52083_0.conda#7e454b4a61754714a4a4d183641374da
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.3-pyhd8ed1ab_0.conda#f44109e52a40b8149156f5ddd9c11b26
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py310ha4c1d20_3.conda#0414d57832172f3cdcf56b5f053e177d
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.3.0-pyhd8ed1ab_0.tar.bz2#83d1a712e6d2bab6b298b1d2f42ad355
 https://conda.anaconda.org/conda-forge/noarch/sphinx-external-toc-0.3.1-pyhd8ed1ab_0.conda#561bdf7b598d38e2962c46557bd1da12
@@ -441,24 +491,26 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinx-thebe-0.2.1-pyhd8ed1ab_0.conda#8a4151bde2af98c6cbc42ee12b48eb7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0.tar.bz2#382738101934261ea7931d1460e64868
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-dotnetdomain-0.4-py_0.tar.bz2#fb61a7369f505b4bb98e1530c3e09f9f
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-golangdomain-0.2.0.dev0-py_0.tar.bz2#d1a73c192888d08cedec232602c22f32
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jquery-4.1-pyhd8ed1ab_0.conda#914897066d5873acfb13e75705276ad1
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.3-pyhd8ed1ab_0.conda#f53d92ecd7d8563b006107f6a33e55c6
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/poetry-1.5.1-linux_pyhd8ed1ab_0.conda#7aae42823198731808dd8e7a9745547f
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-5.4.3-pyhd8ed1ab_0.conda#3777f933bec5113d5a292de10b03d0f6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autoapi-2.1.0-pyhd8ed1ab_0.conda#6cb2b182390f837ce98737e92b9461f7
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
 https://conda.anaconda.org/conda-forge/noarch/sphinx_rtd_theme-1.2.2-pyha770c72_0.conda#5ef6aaf2cfb3b656cdadb431daed6a9f
 https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda#321151b2405f11ec6681a9a6f30822b4
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.0.5-pyhd8ed1ab_1.tar.bz2#1c31d380288fc1599fb5f4c76c8c828c
 https://conda.anaconda.org/conda-forge/noarch/jupyter-book-0.15.1-pyhd8ed1ab_0.conda#f10d556d3b3dc0aeae6aee37c412ea60
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/linux-64/jupyter-1.0.0-py310hff52083_8.conda#6ecb24d6906d5d2a6f091cf4b0045079
 https://conda.anaconda.org/pytorch/linux-64/pytorch-2.0.1-py3.10_cuda11.8_cudnn8.7.0_0.tar.bz2#e8dd4a234ce193267c4cbc981c042429
 https://conda.anaconda.org/conda-forge/noarch/torchinfo-1.8.0-pyhd8ed1ab_0.conda#fba98fc95a945e2a6b93a77b39dd52dc
 https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda#480cb2b6d502003e937d9e4326bc398f
 https://conda.anaconda.org/pytorch/linux-64/torchtriton-2.0.0-py310.tar.bz2#e34aa90f6d7c20babf28fc9225b2a3eb
 https://conda.anaconda.org/pytorch/linux-64/torchvision-0.15.2-py310_cu118.tar.bz2#b38f7082cde2a86ca981194e9ef51028
-https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda#ce9d626b181c6f8cceb5047f6a819f7d
+https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.6-pyhd8ed1ab_0.conda#5325b6adf171d4d69968100af806994e
```

### Comparing `hf-deepali-0.4.2/conda/environment.linux-64.yml` & `hf-deepali-0.4.3/conda/environment.linux-64.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: c6bd68ba63788a00937c8cd1d91bb1e5813d242d7089005156ab1a663f53aee1
+# input_hash: 586016f05a089668afa3f0a057304e5826b41e87317e8d51969529896659d6a0
 
 channels:
   - conda-forge
   - pytorch
   - nvidia
   - nodefaults
 dependencies:
   - _libgcc_mutex=0.1=conda_forge
-  - ca-certificates=2023.5.7=hbcca054_0
+  - ca-certificates=2023.7.22=hbcca054_0
   - cuda-cudart=11.8.89=0
   - cuda-cupti=11.8.87=0
   - cuda-nvrtc=11.8.89=0
   - cuda-nvtx=11.8.86=0
   - cuda-version=12.0=hffde075_2
   - font-ttf-dejavu-sans-mono=2.37=hab24e00_0
   - font-ttf-inconsolata=3.000=h77eed37_0
@@ -41,15 +41,15 @@
   - libgcc-ng=13.1.0=he5830b7_0
   - alsa-lib=1.2.8=h166bdaf_0
   - aom=3.5.0=h27087fc_0
   - attr=2.5.1=h166bdaf_1
   - bzip2=1.0.8=h7f98852_4
   - c-ares=1.19.1=hd590300_0
   - double-conversion=3.2.0=h27087fc_1
-  - eigen=3.4.1=h00ab1b0_0
+  - eigen=3.4.0=h00ab1b0_0
   - fftw=3.3.10=nompi_hc118613_108
   - fribidi=1.0.10=h36c2ea0_0
   - gettext=0.21.1=h27087fc_0
   - giflib=5.2.1=h0b41bf4_3
   - gmp=6.2.1=h58526e2_0
   - graphite2=1.3.13=h58526e2_1001
   - gstreamer-orc=0.4.34=hd590300_0
@@ -85,15 +85,15 @@
   - libzlib=1.2.13=hd590300_5
   - lz4-c=1.9.4=hcb278e6_0
   - mpg123=1.31.3=hcb278e6_0
   - ncurses=6.4=hcb278e6_0
   - nettle=3.8.1=hc379101_1
   - nspr=4.35=h27087fc_0
   - openh264=2.3.1=hcb278e6_2
-  - openssl=3.1.1=hd590300_1
+  - openssl=3.1.2=hd590300_0
   - pixman=0.40.0=h36c2ea0_0
   - pthread-stubs=0.4=h36c2ea0_1001
   - pugixml=1.11.4=h59595ed_1
   - re2=2023.03.02=h8c504da_0
   - svt-av1=1.4.1=hcb278e6_0
   - x264=1!164.3095=h166bdaf_2
   - x265=3.5=h924138e_3
@@ -166,31 +166,36 @@
   - xcb-util=0.4.0=h516909a_0
   - xcb-util-keysyms=0.4.0=h516909a_0
   - xcb-util-renderutil=0.3.9=h166bdaf_0
   - xcb-util-wm=0.4.1=h516909a_0
   - xorg-libx11=1.8.4=h0b41bf4_0
   - absl-py=1.4.0=pyhd8ed1ab_0
   - alabaster=0.7.13=pyhd8ed1ab_0
+  - appdirs=1.4.4=pyh9f0ad1d_0
   - atk-1.0=2.38.0=hd4edc92_1
   - attrs=21.4.0=pyhd8ed1ab_0
   - backcall=0.2.0=pyh9f0ad1d_0
   - backports=1.0=pyhd8ed1ab_3
   - blinker=1.6.2=pyhd8ed1ab_0
+  - boltons=23.0.0=pyhd8ed1ab_0
   - brotli=1.0.9=h166bdaf_9
+  - cached_property=1.5.2=pyha770c72_1
   - cachetools=5.3.1=pyhd8ed1ab_0
-  - certifi=2023.5.7=pyhd8ed1ab_0
+  - certifi=2023.7.22=pyhd8ed1ab_0
   - charset-normalizer=3.2.0=pyhd8ed1ab_0
   - click=8.1.6=unix_pyh707e725_0
   - colorama=0.4.6=pyhd8ed1ab_0
+  - crashtest=0.4.1=pyhd8ed1ab_0
   - cycler=0.11.0=pyhd8ed1ab_0
   - dataclasses=0.8=pyhc8e2a94_3
   - dbus=1.13.6=h5008d03_3
-  - debugpy=1.6.7=py310heca2aa9_0
+  - debugpy=1.6.8=py310hc6cd4ac_0
   - decorator=5.1.1=pyhd8ed1ab_0
   - defusedxml=0.7.1=pyhd8ed1ab_0
+  - distlib=0.3.7=pyhd8ed1ab_0
   - docutils=0.17.1=py310hff52083_3
   - entrypoints=0.4=pyhd8ed1ab_0
   - exceptiongroup=1.1.2=pyhd8ed1ab_0
   - executing=1.2.0=pyhd8ed1ab_0
   - filelock=3.12.2=pyhd8ed1ab_0
   - flit-core=3.9.0=pyhd8ed1ab_0
   - fontconfig=2.14.2=h14ed4e7_0
@@ -202,68 +207,77 @@
   - greenlet=2.0.2=py310hc6cd4ac_1
   - grpcio=1.56.2=py310h1b8f574_0
   - gts=0.7.6=h977cf35_4
   - idna=3.4=pyhd8ed1ab_0
   - imagesize=1.4.1=pyhd8ed1ab_0
   - iniconfig=2.0.0=pyhd8ed1ab_0
   - ipython_genutils=0.2.0=py_1
+  - jeepney=0.8.0=pyhd8ed1ab_0
   - jmespath=1.0.1=pyhd8ed1ab_0
+  - jsonpointer=2.0=py_0
   - jupyterlab_widgets=3.0.8=pyhd8ed1ab_0
   - kiwisolver=1.4.4=py310hbf28c38_1
   - lazy-object-proxy=1.9.0=py310h1fa729e_0
   - lcms2=2.14=h6ed2654_0
-  - libclang13=15.0.7=default_h9986a30_2
+  - libclang13=15.0.7=default_h9986a30_3
   - libcups=2.3.3=h36d4200_3
   - libcurl=8.1.2=h409715c_0
   - libpq=15.3=hbcd7760_1
   - libsystemd0=253=h8c4010b_1
   - libwebp=1.2.4=h522a892_0
+  - lockfile=0.12.2=py_1
   - loguru=0.7.0=py310hff52083_0
   - markupsafe=2.1.3=py310h2372a71_0
   - mccabe=0.7.0=pyhd8ed1ab_0
   - mdurl=0.1.0=pyhd8ed1ab_0
   - mistune=3.0.0=pyhd8ed1ab_0
+  - more-itertools=10.1.0=pyhd8ed1ab_0
   - mpmath=1.3.0=pyhd8ed1ab_0
+  - msgpack-python=1.0.5=py310hdf3cbec_0
   - multidict=6.0.4=py310h1fa729e_0
   - munkres=1.1.4=pyh9f0ad1d_0
   - mypy_extensions=1.0.0=pyha770c72_0
   - nest-asyncio=1.5.6=pyhd8ed1ab_0
   - networkx=3.1=pyhd8ed1ab_0
   - openjpeg=2.5.0=h7d73246_1
   - packaging=23.1=pyhd8ed1ab_0
   - pandocfilters=1.5.0=pyhd8ed1ab_0
   - parso=0.8.3=pyhd8ed1ab_0
-  - pathspec=0.11.1=pyhd8ed1ab_0
+  - pathspec=0.11.2=pyhd8ed1ab_0
   - pickleshare=0.7.5=py_1003
+  - pkginfo=1.9.6=pyhd8ed1ab_0
   - pkgutil-resolve-name=1.3.10=pyhd8ed1ab_0
   - pluggy=1.2.0=pyhd8ed1ab_0
   - ply=3.11=py_1
   - prometheus_client=0.17.1=pyhd8ed1ab_0
   - psutil=5.9.5=py310h1fa729e_0
   - ptyprocess=0.7.0=pyhd3deb0d_0
   - pure_eval=0.2.2=pyhd8ed1ab_0
   - pyasn1=0.4.8=py_0
   - pycodestyle=2.10.0=pyhd8ed1ab_0
+  - pycosat=0.6.4=py310h5764c6d_1
   - pycparser=2.21=pyhd8ed1ab_0
   - pyflakes=3.0.1=pyhd8ed1ab_0
   - pygments=2.15.1=pyhd8ed1ab_0
   - pyjwt=2.8.0=pyhd8ed1ab_0
   - pyparsing=3.0.9=pyhd8ed1ab_0
   - pyrsistent=0.19.3=py310h1fa729e_0
   - pysocks=1.7.1=pyha2e5f31_6
-  - python-fastjsonschema=2.17.1=pyhd8ed1ab_0
+  - python-fastjsonschema=2.18.0=pyhd8ed1ab_0
+  - python-installer=0.7.0=pyhd8ed1ab_0
   - python-json-logger=2.0.7=pyhd8ed1ab_0
   - pytorch-cuda=11.8=h7e8668a_5
   - pytz=2023.3=pyhd8ed1ab_0
   - pyyaml=6.0=py310h5764c6d_5
   - pyzmq=25.1.0=py310h5bbb5d0_0
   - rfc3986-validator=0.1.1=pyh9f0ad1d_0
   - ruamel.yaml.clib=0.2.7=py310h1fa729e_1
   - send2trash=1.8.2=pyh41d4057_0
   - setuptools=67.7.2=pyhd8ed1ab_0
+  - shellingham=1.5.1=pyhd8ed1ab_0
   - six=1.16.0=pyh6c4a22f_0
   - sniffio=1.3.0=pyhd8ed1ab_0
   - snowballstemmer=2.2.0=pyhd8ed1ab_0
   - soupsieve=2.3.2.post1=pyhd8ed1ab_0
   - sphinxcontrib-applehelp=1.0.4=pyhd8ed1ab_0
   - sphinxcontrib-devhelp=1.0.2=py_0
   - sphinxcontrib-htmlhelp=2.0.1=pyhd8ed1ab_0
@@ -271,59 +285,71 @@
   - sphinxcontrib-qthelp=1.0.3=py_0
   - sphinxcontrib-serializinghtml=1.1.5=pyhd8ed1ab_2
   - tabulate=0.9.0=pyhd8ed1ab_1
   - tbb=2021.9.0=hf52228f_0
   - tensorboard-data-server=0.7.0=py310h34c0648_0
   - toml=0.10.2=pyhd8ed1ab_0
   - tomli=2.0.1=pyhd8ed1ab_0
+  - tomlkit=0.12.1=pyha770c72_0
+  - toolz=0.12.0=pyhd8ed1ab_0
   - tornado=6.3.2=py310h2372a71_0
   - traitlets=5.9.0=pyhd8ed1ab_0
+  - trove-classifiers=2023.7.6=pyhd8ed1ab_0
   - typed-ast=1.5.5=py310h2372a71_0
+  - typing=3.10.0.0=pyhd8ed1ab_0
   - typing_extensions=4.7.1=pyha770c72_0
   - typing_utils=0.1.0=pyhd8ed1ab_0
   - uc-micro-py=1.0.1=pyhd8ed1ab_0
   - unicodedata2=15.0.0=py310h5764c6d_0
   - unidecode=1.3.6=pyhd8ed1ab_0
+  - uri-template=1.3.0=pyhd8ed1ab_0
+  - webcolors=1.13=pyhd8ed1ab_0
   - webencodings=0.5.1=py_1
   - websocket-client=1.6.1=pyhd8ed1ab_0
-  - wheel=0.40.0=pyhd8ed1ab_1
+  - wheel=0.41.0=pyhd8ed1ab_0
   - widgetsnbextension=4.0.8=pyhd8ed1ab_0
   - wrapt=1.15.0=py310h1fa729e_0
   - xcb-util-image=0.4.0=h166bdaf_0
   - xorg-libxext=1.3.4=h0b41bf4_2
   - xorg-libxfixes=5.0.3=h7f98852_1004
   - xorg-libxrender=0.9.10=h7f98852_1003
   - xorg-libxt=1.3.0=hd590300_0
   - zipp=3.16.2=pyhd8ed1ab_0
   - accessible-pygments=0.0.4=pyhd8ed1ab_0
   - aiosignal=1.3.1=pyhd8ed1ab_0
   - anyio=3.7.1=pyhd8ed1ab_0
   - asttokens=2.2.1=pyhd8ed1ab_0
   - babel=2.12.1=pyhd8ed1ab_1
+  - backports.cached-property=1.0.2=pyhd8ed1ab_0
   - backports.functools_lru_cache=1.6.5=pyhd8ed1ab_0
   - beautifulsoup4=4.12.2=pyha770c72_0
   - bleach=6.0.0=pyhd8ed1ab_0
+  - cached-property=1.5.2=hd8ed1ab_1
   - cairo=1.16.0=ha61ee94_1014
   - cffi=1.15.1=py310h255011f_3
-  - comm=0.1.3=pyhd8ed1ab_0
+  - click-default-group=1.2.2=pyhd8ed1ab_1
+  - comm=0.1.4=pyhd8ed1ab_0
   - curl=8.1.2=h409715c_0
   - dacite=1.8.0=pyhd8ed1ab_0
   - deprecation=2.1.0=pyh9f0ad1d_0
   - flake8=6.0.0=pyhd8ed1ab_0
-  - fonttools=4.41.0=py310h2372a71_0
+  - fonttools=4.42.0=py310h2372a71_0
   - glew=2.1.0=h9c3ff4c_2
   - glib=2.76.4=hfc55251_0
   - hdf5=1.12.2=nompi_h4df4325_101
+  - html5lib=1.1=pyh9f0ad1d_0
   - importlib-metadata=6.8.0=pyha770c72_0
   - importlib_resources=6.0.0=pyhd8ed1ab_1
-  - jedi=0.18.2=pyhd8ed1ab_0
+  - jaraco.classes=3.3.0=pyhd8ed1ab_0
+  - jedi=0.19.0=pyhd8ed1ab_0
   - jinja2=3.1.2=pyhd8ed1ab_1
+  - jsonpatch=1.32=pyhd8ed1ab_0
   - jupyterlab_pygments=0.2.2=pyhd8ed1ab_0
   - latexcodec=2.0.1=pyh9f0ad1d_0
-  - libclang=15.0.7=default_h7634d5b_2
+  - libclang=15.0.7=default_h7634d5b_3
   - libgd=2.3.3=h18fbbfe_3
   - libva=2.18.0=h0b41bf4_0
   - lightning-utilities=0.9.0=pyhd8ed1ab_0
   - linkify-it-py=2.0.0=pyhd8ed1ab_0
   - markdown-it-py=2.2.0=pyhd8ed1ab_0
   - matplotlib-inline=0.1.6=pyhd8ed1ab_0
   - mkl=2022.1.0=h84fe81f_915
@@ -339,105 +365,129 @@
   - pytest=7.3.2=pyhd8ed1ab_1
   - python-dateutil=2.8.2=pyhd8ed1ab_0
   - pyu2f=0.1.5=pyhd8ed1ab_0
   - qtpy=2.3.1=pyhd8ed1ab_0
   - rfc3339-validator=0.1.4=pyhd8ed1ab_0
   - rsa=4.9=pyhd8ed1ab_0
   - ruamel.yaml=0.17.32=py310h2372a71_0
-  - sip=6.7.9=py310hc6cd4ac_0
+  - sip=6.7.11=py310hc6cd4ac_0
   - sympy=1.12=pypyh9d50eac_103
   - tbb-devel=2021.9.0=hf52228f_0
   - terminado=0.17.1=pyh41d4057_0
   - tinycss2=1.2.1=pyhd8ed1ab_0
   - tqdm=4.65.0=pyhd8ed1ab_1
   - typing-extensions=4.7.1=hd8ed1ab_0
   - werkzeug=2.3.6=pyhd8ed1ab_0
   - yarl=1.9.2=py310h2372a71_0
+  - annotated-types=0.5.0=pyhd8ed1ab_0
   - argon2-cffi-bindings=21.2.0=py310h5764c6d_3
+  - arrow=1.2.3=pyhd8ed1ab_0
   - astroid=2.15.6=py310hff52083_0
   - async-timeout=4.0.2=pyhd8ed1ab_0
   - brotlipy=0.7.0=py310h5764c6d_1005
   - cryptography=41.0.2=py310h75e40e8_0
   - ffmpeg=5.1.2=gpl_h8dda1f0_106
+  - fqdn=1.5.1=pyhd8ed1ab_0
   - ghp-import=2.1.0=pyhd8ed1ab_0
   - gstreamer=1.22.0=h25f0c4b_2
   - harfbuzz=6.0.0=h8e241bc_0
   - importlib_metadata=6.8.0=hd8ed1ab_0
   - jsonschema=4.17.3=pyhd8ed1ab_0
   - jupyter_server_terminals=0.4.4=pyhd8ed1ab_1
   - libblas=3.9.0=16_linux64_mkl
   - libitk=5.3.0=hcedbc38_0
   - libnetcdf=4.8.1=nompi_h261ec11_106
-  - markdown=3.4.3=pyhd8ed1ab_0
+  - markdown=3.4.4=pyhd8ed1ab_0
   - mdit-py-plugins=0.4.0=pyhd8ed1ab_0
   - mkl-devel=2022.1.0=ha770c72_916
-  - platformdirs=3.9.1=pyhd8ed1ab_0
+  - platformdirs=3.10.0=pyhd8ed1ab_0
+  - poetry-core=1.6.1=pyhd8ed1ab_0
   - pulseaudio-daemon=16.1=ha8d29e2_3
   - pybtex=0.24.0=pyhd8ed1ab_2
-  - pyqt5-sip=12.11.0=py310heca2aa9_3
+  - pydantic-core=2.4.0=py310hcb5633a_0
+  - pyqt5-sip=12.12.2=py310hc6cd4ac_4
   - python-build=0.10.0=pyhd8ed1ab_1
   - setuptools-scm=7.1.0=pyhd8ed1ab_0
   - sqlalchemy=2.0.19=py310h2372a71_0
   - stack_data=0.6.2=pyhd8ed1ab_0
   - wcwidth=0.2.6=pyhd8ed1ab_0
+  - zstandard=0.19.0=py310h1275a96_2
   - aiohttp=3.8.5=py310h2372a71_0
   - argon2-cffi=21.3.0=pyhd8ed1ab_0
   - black=22.3.0=pyhd8ed1ab_0
+  - conda-package-streaming=0.9.0=pyhd8ed1ab_0
   - gst-plugins-base=1.22.0=h4243ec0_2
+  - isoduration=20.11.0=pyhd8ed1ab_0
   - jupyter_core=5.3.1=py310hff52083_0
-  - jupyter_events=0.6.3=pyhd8ed1ab_0
   - libcblas=3.9.0=16_linux64_mkl
   - liblapack=3.9.0=16_linux64_mkl
   - oauthlib=3.2.2=pyhd8ed1ab_0
   - pango=1.50.14=hd33c08f_0
+  - poetry-plugin-export=1.4.0=pyhd8ed1ab_0
   - prompt-toolkit=3.0.39=pyha770c72_0
   - pulseaudio=16.1=hcb278e6_3
   - pybtex-docutils=1.0.2=py310hff52083_2
+  - pydantic=2.1.1=pyhd8ed1ab_0
   - pyopenssl=23.2.0=pyhd8ed1ab_1
+  - secretstorage=3.3.3=py310hff52083_1
   - simpleitk=2.2.1=py310h2b9ea3a_1
+  - virtualenv=20.24.2=pyhd8ed1ab_0
+  - conda-package-handling=2.2.0=pyh38be061_0
   - flake8-black=0.3.6=pyhd8ed1ab_0
   - gtk2=2.24.33=h90689f9_2
+  - jsonschema-with-format-nongpl=4.17.3=pyhd8ed1ab_0
   - jupyter_client=8.3.0=pyhd8ed1ab_0
+  - keyring=23.13.1=py310hff52083_0
   - liblapacke=3.9.0=16_linux64_mkl
   - librsvg=2.54.4=h7abd40a_0
-  - nbformat=5.9.1=pyhd8ed1ab_0
-  - numpy=1.25.1=py310ha4c1d20_0
+  - nbformat=5.9.2=pyhd8ed1ab_0
+  - numpy=1.25.2=py310ha4c1d20_0
   - prompt_toolkit=3.0.39=hd8ed1ab_0
   - qt-main=5.15.8=h5d23da1_6
   - urllib3=1.26.15=pyhd8ed1ab_0
   - wslink=1.11.1=pyhd8ed1ab_0
   - blas-devel=3.9.0=16_linux64_mkl
   - botocore=1.29.165=pyhd8ed1ab_0
   - contourpy=1.1.0=py310hd41b1e2_0
+  - dulwich=0.21.5=py310h2372a71_0
   - graphviz=7.0.5=h2e5815a_0
   - ipython=8.14.0=pyh41d4057_0
+  - jupyter_events=0.7.0=pyhd8ed1ab_0
   - nbclient=0.7.4=pyhd8ed1ab_0
   - nibabel=5.1.0=py310hff52083_2
   - pandas=1.5.3=py310h9b08913_1
-  - pyqt=5.15.7=py310hab646b1_3
+  - pyqt=5.15.9=py310h04931ad_4
+  - rapidfuzz=2.15.1=py310heca2aa9_0
   - requests=2.31.0=pyhd8ed1ab_0
   - vtk=9.2.5=qt_py310hc895abb_200
   - blas=2.116=mkl
+  - cachecontrol=0.12.14=pyhd8ed1ab_0
+  - cleo=2.0.1=pyhd8ed1ab_0
+  - conda=23.7.2=py310hff52083_0
+  - ensureconda=1.4.3=pyhd8ed1ab_0
   - google-auth=2.22.0=pyh1a96a4e_0
   - ipykernel=6.23.3=pyh71e2992_0
+  - ipywidgets=8.1.0=pyhd8ed1ab_0
   - jupyter-cache=0.6.1=pyhd8ed1ab_0
   - matplotlib-base=3.7.2=py310hf38f957_0
-  - nbconvert-core=7.7.1=pyhd8ed1ab_1
+  - nbconvert-core=7.7.3=pyhd8ed1ab_0
   - pooch=1.7.0=pyha770c72_3
   - requests-oauthlib=1.3.1=pyhd8ed1ab_0
+  - requests-toolbelt=1.0.0=pyhd8ed1ab_0
   - s3transfer=0.6.1=pyhd8ed1ab_0
   - sphinx=4.5.0=pyh6c4a22f_0
   - boto3=1.26.165=pyhd8ed1ab_0
+  - cachecontrol-with-filecache=0.12.14=pyhd8ed1ab_0
+  - conda-devenv=2.3.0=pyhd8ed1ab_0
   - google-auth-oauthlib=1.0.0=pyhd8ed1ab_1
-  - ipywidgets=8.0.7=pyhd8ed1ab_0
   - jupyter_console=6.6.3=pyhd8ed1ab_0
   - jupyter_server=2.7.0=pyhd8ed1ab_0
   - matplotlib=3.7.2=py310hff52083_0
   - myst-parser=0.18.1=pyhd8ed1ab_0
-  - nbconvert-pandoc=7.7.1=pyhd8ed1ab_1
+  - nbconvert-pandoc=7.7.3=pyhd8ed1ab_0
   - pydata-sphinx-theme=0.13.3=pyhd8ed1ab_0
   - qtconsole-base=5.4.3=pyha770c72_0
   - scipy=1.10.1=py310ha4c1d20_3
   - sphinx-comments=0.0.3=pyh9f0ad1d_0
   - sphinx-copybutton=0.5.2=pyhd8ed1ab_0
   - sphinx-design=0.3.0=pyhd8ed1ab_0
   - sphinx-external-toc=0.3.1=pyhd8ed1ab_0
@@ -447,24 +497,26 @@
   - sphinx-thebe=0.2.1=pyhd8ed1ab_0
   - sphinx-togglebutton=0.3.2=pyhd8ed1ab_0
   - sphinxcontrib-bibtex=2.5.0=pyhd8ed1ab_0
   - sphinxcontrib-dotnetdomain=0.4=py_0
   - sphinxcontrib-golangdomain=0.2.0.dev0=py_0
   - sphinxcontrib-jquery=4.1=pyhd8ed1ab_0
   - myst-nb=0.17.2=pyhd8ed1ab_0
-  - nbconvert=7.7.1=pyhd8ed1ab_1
+  - nbconvert=7.7.3=pyhd8ed1ab_0
   - notebook-shim=0.2.3=pyhd8ed1ab_0
+  - poetry=1.5.1=linux_pyhd8ed1ab_0
   - qtconsole=5.4.3=pyhd8ed1ab_0
   - sphinx-autoapi=2.1.0=pyhd8ed1ab_0
   - sphinx-book-theme=1.0.1=pyhd8ed1ab_0
   - sphinx_rtd_theme=1.2.2=pyha770c72_0
   - tensorboard=2.13.0=pyhd8ed1ab_0
+  - conda-lock=1.0.5=pyhd8ed1ab_1
   - jupyter-book=0.15.1=pyhd8ed1ab_0
   - nbclassic=1.0.0=pyhb4ecaf3_1
   - notebook=6.5.4=pyha770c72_0
   - jupyter=1.0.0=py310hff52083_8
   - pytorch=2.0.1=py3.10_cuda11.8_cudnn8.7.0_0
   - torchinfo=1.8.0=pyhd8ed1ab_0
   - torchmetrics=0.11.4=pyhd8ed1ab_0
   - torchtriton=2.0.0=py310
   - torchvision=0.15.2=py310_cu118
-  - pytorch-lightning=2.0.4=pyhd8ed1ab_0
+  - pytorch-lightning=2.0.6=pyhd8ed1ab_0
```

### Comparing `hf-deepali-0.4.2/conda/environment.osx-64.lock` & `hf-deepali-0.4.3/conda/environment.osx-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 533a7567b393584157366e71374225596e814fe74cfcb03642d3b4e184d58c87
+# input_hash: 1e6e6cea02ff8fd576a8852899876561e48ebb709abcd877d8d931d3b50338da
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
+https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.7.22-h8857fd0_0.conda#bf2c54c18997bf3542af074c10191771
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
 https://conda.anaconda.org/conda-forge/osx-64/fribidi-1.0.10-hbcb3906_0.tar.bz2#f1c6b41e0f56998ecd9a3e210faa1dc0
 https://conda.anaconda.org/conda-forge/osx-64/giflib-5.2.1-hb7f2c08_3.conda#aca150b0186836f893ebac79019e5498
 https://conda.anaconda.org/conda-forge/osx-64/jpeg-9e-hb7f2c08_3.conda#6b55131ae9445ef38746dc6b080acda9
@@ -41,61 +41,61 @@
 https://conda.anaconda.org/conda-forge/osx-64/x264-1!164.3095-h775f41a_2.tar.bz2#23e9c3180e2c0f9449bb042914ec2200
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
 https://conda.anaconda.org/conda-forge/osx-64/aom-3.5.0-hf0c8a7f_0.tar.bz2#9110390ac33346f643e26051a92de5ce
 https://conda.anaconda.org/conda-forge/osx-64/double-conversion-3.2.0-hf0c8a7f_1.tar.bz2#3c2d7d657d83eac1507bc6fbab9eb297
-https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.1-h1c7c39f_0.conda#4b30cbb5ec44b4ce28e92daac53f3132
+https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.0-h1c7c39f_0.conda#5b2cfc277e3d42d84a2a648825761156
 https://conda.anaconda.org/conda-forge/osx-64/expat-2.5.0-hf0c8a7f_1.conda#e12630038077877cbb6c7851e139c17c
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
 https://conda.anaconda.org/conda-forge/osx-64/gettext-0.21.1-h8a4c099_0.tar.bz2#1e3aff29ce703d421c43f371ad676cc5
 https://conda.anaconda.org/conda-forge/osx-64/glew-2.1.0-h046ec9c_2.tar.bz2#6b753c8c7e4c46a8eb17b6f1781f958a
 https://conda.anaconda.org/conda-forge/osx-64/gmp-6.2.1-h2e338ed_0.tar.bz2#dedc96914428dae572a39e69ee2a392f
 https://conda.anaconda.org/conda-forge/osx-64/graphite2-1.3.13-h2e338ed_1001.tar.bz2#5f6e7f98caddd0fc2d345b207531814c
 https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
 https://conda.anaconda.org/conda-forge/osx-64/jsoncpp-1.9.5-h940c156_1.tar.bz2#45824afbfd843fe0584ae8df22f1d99a
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libabseil-20230125.3-cxx17_h000cb23_0.conda#1d883cd421a0b0af624c38fa8d043f98
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.3.0-hbd3c1fe_1.conda#209e462211f65827cdc01a0d7a72286f
 https://conda.anaconda.org/conda-forge/osx-64/libllvm13-13.0.1-h64f94b2_2.tar.bz2#bac1c6f12f44f40e19274e6e04e9bad5
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libvorbis-1.3.7-h046ec9c_0.tar.bz2#fbbda1fede0aadaa252f6919148c4ce1
 https://conda.anaconda.org/conda-forge/osx-64/libvpx-1.11.0-he49afe7_3.tar.bz2#4ad2e740535a74d4ab65550b8a41f99f
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.13-h0d85af4_1004.tar.bz2#eb7860935e14aec936065cbc21a1a962
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/nspr-4.35-hea0b92c_0.conda#a9e56c98d13d8b7ce72bf4357317c29b
 https://conda.anaconda.org/conda-forge/osx-64/openh264-2.3.1-hf0c8a7f_2.conda#989ba22b08353c5ca0e6fba80bcd4321
-https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.2-h8a1eda9_0.conda#85d5377436d19183c8ac5afbb8e713a1
 https://conda.anaconda.org/conda-forge/osx-64/p11-kit-0.24.1-h65f8906_0.tar.bz2#e936a0ee28be948846108582f00e2d61
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/pcre2-10.40-h1c4e4bc_0.tar.bz2#e0f80c8f3a0352a54eddfe59cd2b25b1
 https://conda.anaconda.org/conda-forge/osx-64/pugixml-1.11.4-he965462_1.conda#f147ec845c13ddafae4abdb5430875bc
 https://conda.anaconda.org/conda-forge/osx-64/re2-2023.03.02-h096449b_0.conda#68580e997396899915eef7771ef3a646
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/svt-av1-1.4.1-hf0c8a7f_0.conda#86739428e1e1c8882fe14067a7ac371a
-https://conda.anaconda.org/conda-forge/osx-64/tbb-2021.9.0-hb8565cd_0.conda#6aedf8fdcdf5f2d7b4db21853a7d42ed
+https://conda.anaconda.org/conda-forge/osx-64/tbb-2021.10.0-h1c7c39f_0.conda#7d866c2f94d867282a403460cfa8b3f8
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/x265-3.5-hbb4e6a2_3.tar.bz2#a3bf3e95b7795871a6734a784400fcea
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-h829000d_7.conda#b274ec4dbf15a6e20900e397610567a0
 https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/gl2ps-1.4.2-h4cff582_0.tar.bz2#a9e91533b95cd019d58f4b3ef9bbddf0
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h7aa5921_5.tar.bz2#a5e171d71c6b524409de40d81c098758
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
-https://conda.anaconda.org/conda-forge/osx-64/libclang-13.0.1-default_h255f2f3_1.conda#7ffe2879ebb140302889d22a1ec41d84
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
+https://conda.anaconda.org/conda-forge/osx-64/libclang-13.0.1-root_62804_h2961583_3.conda#5d71eab2f706fb237a7023e04a6e4f73
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-12_3_0_h97931a8_1.conda#3dfbc4ce09c598763cffcc667686f412
 https://conda.anaconda.org/conda-forge/osx-64/libglib-2.76.4-hc62aa5d_0.conda#05c728fccc40277119bf94cf08e38384
 https://conda.anaconda.org/conda-forge/osx-64/libidn2-2.3.4-hb7f2c08_0.tar.bz2#bd109fd705b4ce40a62759129bc4ef5a
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
 https://conda.anaconda.org/conda-forge/osx-64/libprotobuf-4.23.3-h5feb325_0.conda#b9e780ed0d0a365ff10b8e83c64471ce
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtheora-1.1.1-h0d85af4_1005.tar.bz2#e63b84ed4c2d84901332de92a98a2f2b
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.4.0-h6268bbc_5.conda#551fc78ba147767ea5905d0746e2fbb5
@@ -103,34 +103,39 @@
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/mkl-2022.1.0-h860c996_928.tar.bz2#98a4d58de0ba6e61ce46620b775c19ce
 https://conda.anaconda.org/conda-forge/osx-64/mpfr-4.2.0-h4f9bd69_0.conda#f48a2f4515be334c5cfeed82517b96e0
 https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_2.conda#6f1f77589d0af4e85e32f896d2a51f4e
 https://conda.anaconda.org/conda-forge/osx-64/nss-3.89-h78b00b3_0.conda#1eb1408ecae62d98a902636d46f5595c
 https://conda.anaconda.org/conda-forge/osx-64/python-3.10.12-had23ca6_0_cpython.conda#351b8aa0687f3510620cf06ad11229f4
 https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.42.0-h2b0dec6_0.conda#6c22b83608a6e3bd324ab29d3092592f
-https://conda.anaconda.org/conda-forge/osx-64/tbb-devel-2021.9.0-hb8565cd_0.conda#23fd9e2cb5478ed8b6ba925a741af61b
+https://conda.anaconda.org/conda-forge/osx-64/tbb-devel-2021.10.0-h1c7c39f_0.conda#3f66beb4d0e5cab00d6629ed7a77a062
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
+https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h1d18e73_1.tar.bz2#5a538295f97a484ee332aacc131718b5
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
+https://conda.anaconda.org/conda-forge/noarch/boltons-23.0.0-pyhd8ed1ab_0.conda#033eb25fffd222aceeca6d58cd953680
 https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
+https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
-https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.7.22-pyhd8ed1ab_0.conda#7f3dbc9179b4dde7da98dfb151d0ad22
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
-https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py310h7a76584_0.conda#549f7722839c44ee8a859fc0b94a5884
+https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.8-py310h9e9d8ca_0.conda#1cf76f1cacf74894e317a4aa4da54cf7
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda#12d8aae6994f342618443a8f05c652a0
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py310h2ec42d9_3.tar.bz2#69b3569d320b0fc940449fcc25b01e31
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/osx-64/fftw-3.3.10-nompi_h4fa670e_108.conda#39132ce6ed3180b42b54d40289cd4157
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
@@ -143,120 +148,140 @@
 https://conda.anaconda.org/conda-forge/osx-64/greenlet-2.0.2-py310h9e9d8ca_1.conda#699b3a96666340fe9349c3547f047e29
 https://conda.anaconda.org/conda-forge/osx-64/gts-0.7.6-h53e17e3_4.conda#848cc963fcfbd063c7a023024aa3bec0
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
+https://conda.anaconda.org/conda-forge/noarch/jsonpointer-2.0-py_0.tar.bz2#07d85c22a3beb102a48cd123df84c2a6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py310ha23aa8a_1.tar.bz2#cc358fb878ac593c60cea08b28ac7423
 https://conda.anaconda.org/conda-forge/osx-64/lazy-object-proxy-1.9.0-py310h90acd4f_0.conda#b0b1dc46dd92f49877ea8eecd56f2d00
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.14-h90f4b2a_0.tar.bz2#e56c432e9a78c63692fa6bd076a15713
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_mkl.conda#e5d4b69958f8eb30b932828880b847f3
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
 https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.56.2-he6801ca_0.conda#c0bb2505f166b769ae3e1e01dce31fe9
 https://conda.anaconda.org/conda-forge/osx-64/libpq-15.3-h9dc22bb_1.conda#571aa9141d1a823202bb4cd794c939b0
 https://conda.anaconda.org/conda-forge/osx-64/libwebp-1.2.4-hfa4350a_0.tar.bz2#d3b5a56369701e6a11bf300ba3394391
+https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
 https://conda.anaconda.org/conda-forge/osx-64/loguru-0.7.0-py310h2ec42d9_0.conda#632a71feccc9f651c844c402efe61884
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py310h6729b98_0.conda#b23ce1495527802905791489c3b1f129
 https://conda.anaconda.org/conda-forge/noarch/mccabe-0.7.0-pyhd8ed1ab_0.tar.bz2#34fc335fc50eef0b5ea708f2b5f54e0c
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/osx-64/mkl-devel-2022.1.0-h694c41f_929.tar.bz2#041ceef009fe6d29cbd2555907c23ab3
+https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.1.0-pyhd8ed1ab_0.conda#8549fafed0351bbfaa1ddaa15fdf9b4e
 https://conda.anaconda.org/conda-forge/osx-64/mpc-1.3.1-h81bd1dd_0.conda#c752c0eb6c250919559172c011e5f65b
 https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda#dbf6e2d89137da32fa6670f3bffc024e
+https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py310ha23aa8a_0.conda#eaca50d68ad312e2930b2f9eca8756ef
 https://conda.anaconda.org/conda-forge/osx-64/multidict-6.0.4-py310h90acd4f_0.conda#0324181c4442d94c865cf9ae3b6a7fea
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_2.conda#0e750706160c8e178864b890d3afd164
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.0-h5d0d7b0_1.tar.bz2#be533cc782981a0ec5eed28aa618470a
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
+https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.2-pyhd8ed1ab_0.conda#e41debb259e68490e3ab81e46b639ab6
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
+https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py310h90acd4f_0.conda#1111504c53989e065a98171156fc376a
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
+https://conda.anaconda.org/conda-forge/osx-64/pycosat-0.6.4-py310h90acd4f_1.tar.bz2#95c032c354c500001a935aac4c059376
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyflakes-3.0.1-pyhd8ed1ab_0.conda#44b7d77d96560c93e0e11437a3c35254
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda#912c0194f898fdb783021fd25f913c31
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
 https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py310h90acd4f_0.conda#2de2b931546de39d852e5d21e58876c1
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.18.0-pyhd8ed1ab_0.conda#3be9466311564f80f8056c0851fc5bb7
+https://conda.anaconda.org/conda-forge/noarch/python-installer-0.7.0-pyhd8ed1ab_0.conda#65dea78f903d686c8b0c2feaf0e15e1f
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py310h90acd4f_5.tar.bz2#e0ba2009f52ccda088c63dedf0d1c5ec
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py310h998be00_0.conda#d31ade96a299a26bcb59b74a9b3c1dd6
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py310h90acd4f_1.conda#d27546735a054dd67e626b17ff07c089
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.1-pyhd8ed1ab_0.conda#1de44299f48f522caa2e0074231614e1
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/osx-64/tensorboard-data-server-0.7.0-py310hdd0c95c_0.conda#a57f926841a85a41249ee67023498281
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.1-pyha770c72_0.conda#62f5b331c53d73e2f6c4c130b53518a0
+https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py310h6729b98_0.conda#369ce2c5cd18205e4917f515b4052376
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2023.7.6-pyhd8ed1ab_0.conda#c9918f6a3973e28a792e747289734cd3
 https://conda.anaconda.org/conda-forge/osx-64/typed-ast-1.5.4-py310h90acd4f_1.tar.bz2#189bf6e55cac449f8b34763502b18385
+https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2#e6573ac68718f17b9d4f5c8eda3190f2
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py310h90acd4f_0.tar.bz2#b62adca3645b3bbc46940d5b1833d59b
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
+https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
+https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.41.0-pyhd8ed1ab_0.conda#66beb36a1fa7e0dc9d9bf843a80eb82c
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/osx-64/wrapt-1.15.0-py310h90acd4f_0.conda#f91dbc3c63e137a27a4de2964d56e6e3
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
+https://conda.anaconda.org/conda-forge/noarch/backports.cached-property-1.0.2-pyhd8ed1ab_0.tar.bz2#0e1df3978dd516e20ef88c86d51e5432
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/osx-64/cairo-1.16.0-h904041c_1014.tar.bz2#2e7b4350178ed52bb6fd2b1ecbeeed4f
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310ha78151a_3.conda#652082e4a6cf9d26e43d0d362590c276
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.4-pyhd8ed1ab_0.conda#c8eaca39e2b6abae1fc96acc929ae939
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/osx-64/ffmpeg-5.1.2-gpl_h8b4fe81_106.conda#3c62afa3457aeb6f058b40f1f41f772a
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
-https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.41.0-py310h6729b98_0.conda#2de0c6bd77a2ea8aa4e82943273c5dd3
+https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.42.0-py310h6729b98_0.conda#f23e7e0fd82662cc9ddd8124ef45d5b4
 https://conda.anaconda.org/conda-forge/osx-64/glib-2.76.4-h7d26f99_0.conda#4176982aebeacb4f6914ea5528dc2853
 https://conda.anaconda.org/conda-forge/osx-64/gmpy2-2.1.2-py310hb691cb2_1.tar.bz2#a495ede1fb673f39133b7c2628af7259
 https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.56.2-py310h0d4bf3c_0.conda#6be89e336739268b0415850c065cc0d8
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.12.2-nompi_h48135f9_101.conda#2ee4811ba5f72f7f12f69b3ec2d6cd96
+https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda#e9f79248d30e942f7c358ff21a1790f5
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.0-pyhd8ed1ab_0.conda#1cd7f70057cdffc10977b613fb75425d
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/noarch/jsonpatch-1.32-pyhd8ed1ab_0.tar.bz2#09150b51b0528a31a0f6500b96fdde82
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_mkl.conda#5adcad22978f80fa101047022e79d9eb
 https://conda.anaconda.org/conda-forge/osx-64/libgd-2.3.3-h1e214de_3.tar.bz2#350af2b75c58dc16985fa97298469143
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_mkl.conda#5557060dea295fcbb224be17b3947d16
 https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda#c71f7ec8b80a536e58b979299b230251
 https://conda.anaconda.org/conda-forge/noarch/linkify-it-py-2.0.0-pyhd8ed1ab_0.tar.bz2#25b93e66067eb496ac10da888e25cc33
@@ -274,105 +299,129 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2#03bf410858b2cefc267316408a77c436
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py310h6729b98_0.conda#4c87395e8169331108914e30ab46d2a4
-https://conda.anaconda.org/conda-forge/osx-64/sip-6.7.9-py310h9e9d8ca_0.conda#5aae43762f6fe7bbdd3e0e2bbd567999
+https://conda.anaconda.org/conda-forge/osx-64/sip-6.7.11-py310h9e9d8ca_0.conda#985292668e418bea78567353d03098db
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/werkzeug-2.3.6-pyhd8ed1ab_0.conda#55fbbb3e67185820ee2007395bfe0073
 https://conda.anaconda.org/conda-forge/osx-64/yarl-1.9.2-py310h6729b98_0.conda#f8a1c7107b3b661accf1a7d86c8fd4e1
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py310h90acd4f_3.tar.bz2#952166ee5ce75092167a7385a4e243e3
+https://conda.anaconda.org/conda-forge/noarch/arrow-1.2.3-pyhd8ed1ab_0.tar.bz2#fd1967c76eda3a3dd9e8e6cb7a15a028
 https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.6-py310h2ec42d9_0.conda#2812b75db400abe651a33b99a7173ee6
 https://conda.anaconda.org/conda-forge/noarch/async-timeout-4.0.2-pyhd8ed1ab_0.tar.bz2#25e79f9a1133556671becbd65a170c78
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py310h90acd4f_1005.tar.bz2#63accc45f2b9ae1dad4db9cdfaa903b4
 https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.2-py310ha1817de_0.conda#f7f258c457df7e0617c2b92e24a7b47f
+https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2#6d8d61116031a3f5b1f32e7899785866
-https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_1.conda#659321735840756bc2c6ba7195ed9d8b
+https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.5-h840fbdc_0.conda#34b61e048ab804e3699fc449a4884fce
 https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-6.0.0-h08f8713_0.conda#3852d6ef7b77da3e81074a8e487e7df5
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libitk-5.3.0-h10ab89a_0.conda#73b9bad009f8759bd1854cbc6deca726
 https://conda.anaconda.org/conda-forge/osx-64/liblapacke-3.9.0-17_osx64_mkl.conda#678af3918e54ac46249290a05e7e69b1
 https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.8.1-nompi_hc61b76e_106.tar.bz2#502e31e4a400216854da4e9933fb21c2
-https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
+https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.4-pyhd8ed1ab_0.conda#6b8ab17bc8ff1ca89b3ea28ea3d566ca
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.1-py310h7451ae0_0.conda#525db32fd93b63f2f7ca3ece8576b9c8
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.2-py310h7451ae0_0.conda#a0f919ff93f102cb1720f71448010c61
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.10.0-pyhd8ed1ab_0.conda#0809187ef9b89a3d94a5c24d13936236
+https://conda.anaconda.org/conda-forge/noarch/poetry-core-1.6.1-pyhd8ed1ab_0.conda#a6d1f61527c27fcc0165a6701a46b9f4
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.4.0-py310h3461e44_0.conda#697e1a00773e5bc8232e862b5ae76186
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py310hef2d279_0.conda#0874355241e82a01cd15c6e6b28c7187
-https://conda.anaconda.org/conda-forge/osx-64/pyqt5-sip-12.11.0-py310h415000c_3.conda#6c56916bf99c55b1f57a53ed689f2561
+https://conda.anaconda.org/conda-forge/osx-64/pyqt5-sip-12.12.2-py310h018f80b_4.conda#1b383c6ab90e71d5429104a1573d25f3
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
 https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.19-py310h6729b98_0.conda#9560749662f11f766ce19db9fa6271a4
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/sympy-1.12-pypyh9d50eac_103.conda#2f7d6347d7acf6edf1ac7f2189f44c8f
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/osx-64/xattr-0.10.1-py310h90acd4f_0.conda#d267890f1fba643f1803d7ce417e20b9
+https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.19.0-py310h151724a_2.conda#8bd43a6390a6905fbc0dd14883fd3166
 https://conda.anaconda.org/conda-forge/osx-64/aiohttp-3.8.5-py310h6729b98_0.conda#b91a4b8a80ba83d20ed0eabcc6949ebc
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
 https://conda.anaconda.org/conda-forge/osx-64/blas-devel-3.9.0-17_osx64_mkl.conda#b40b415e2be4d0d2a8d05d0f805240b7
+https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.9.0-pyhd8ed1ab_0.conda#38253361efb303deead3eab39ae9269b
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py310h88cfcbd_0.conda#0cfd4a8d0f1d785675d5e41e17c8b122
-https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_1.conda#504bc1e992fc2d59e55cbd0102e117b0
+https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.5-hb5d3a86_0.conda#b352c9e0490352a101e6299daa98196b
+https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py310h2ec42d9_0.conda#2df6b800f29e805b1453a5a32981b873
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/osx-64/keyring-23.13.1-py310h2ec42d9_0.conda#612970525fa53375995933f14718551c
 https://conda.anaconda.org/conda-forge/osx-64/nibabel-5.1.0-py310h2ec42d9_2.conda#04ba9603c2c52981e403da2295df8bc5
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py310hecf8f37_1.conda#116e61ed90d0332d30310b2210eb1db4
 https://conda.anaconda.org/conda-forge/osx-64/pango-1.50.14-hbd9bf65_0.conda#7de54d83e9c685b742e0a4d81b271de0
+https://conda.anaconda.org/conda-forge/noarch/poetry-plugin-export-1.4.0-pyhd8ed1ab_0.conda#00893c7ea4f9f7620706e0aa94c01b6e
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py310h2ec42d9_2.tar.bz2#7dac3c5087b676102bf38bd984499219
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.1.1-pyhd8ed1ab_0.conda#7964a624018707909044b509f58b937a
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/osx-64/rapidfuzz-2.15.1-py310h7a76584_0.conda#df0e628847158f0e1331b61f3aa04d84
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/osx-64/simpleitk-2.2.1-py310h4447650_1.conda#ca28f25ff59b4907686307195de35927
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.2-pyhd8ed1ab_0.conda#a218f3be8ab6185a475c8168a86e18ae
 https://conda.anaconda.org/conda-forge/osx-64/blas-2.117-mkl.conda#4c921079b5298ce08bb336fc025b96d7
+https://conda.anaconda.org/conda-forge/noarch/cleo-2.0.1-pyhd8ed1ab_0.conda#f1c5f2af6676cbe9206e191d1e70f661
+https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.2.0-pyh38be061_0.conda#8a3ae7f6318376aa08ea753367bb7dd6
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
 https://conda.anaconda.org/conda-forge/osx-64/gtk2-2.24.33-h7c1209e_2.tar.bz2#307614630946527e302b7dd042a5cfa2
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.17.3-pyhd8ed1ab_0.conda#7a709748e93f0b2c33d6b5b676b6d9d0
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.54.4-h3d48ba6_0.tar.bz2#1a106d9119086f73b5f88c650f700210
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.2-py310h475a17b_0.conda#ffc8dbf00f18c1ca9d3c02854cb72aee
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.2-pyhd8ed1ab_0.conda#61ba076de6530d9301a0053b02f093d2
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/osx-64/qt-main-5.15.8-h1d3b3f8_6.conda#5d816352174169f7ab45fb54a0fba4ed
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
+https://conda.anaconda.org/conda-forge/osx-64/dulwich-0.21.5-py310h6729b98_0.conda#21f217991c9bf115e814038cffec4daf
 https://conda.anaconda.org/conda-forge/osx-64/graphviz-7.0.5-hc51f7b9_0.conda#589501e7b16648c032a537b6a0870dbe
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.7.0-pyhd8ed1ab_0.conda#279fed93be42722de98e998ec80be8a1
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.2-py310h2ec42d9_0.conda#4fe2e1daa542b330507af9a2ca079d1c
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-https://conda.anaconda.org/conda-forge/osx-64/pyqt-5.15.7-py310hdd03f62_3.conda#c652959992036327b71a2d5ff593cf72
+https://conda.anaconda.org/conda-forge/osx-64/pyqt-5.15.9-py310hecc045f_4.conda#eba55c15090ca812a17cf393ef61ba7c
 https://conda.anaconda.org/pytorch/osx-64/pytorch-2.0.1-py3.10_0.tar.bz2#527aa8793c545ed93288d32bb45d009d
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/osx-64/vtk-9.2.5-qt_py310hea5b068_200.conda#8210705bd78317d38a376b01f6cfab46
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.14-pyhd8ed1ab_0.conda#db23395890ef31be3c2320fb41b665b0
+https://conda.anaconda.org/conda-forge/osx-64/conda-23.7.2-py310h2ec42d9_0.conda#dff2e97c1fcf3b9fe5f55b28b0effb97
+https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda#5583192796d1ebcf39b1e3e0958aa259
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.0-pyhd8ed1ab_0.conda#6fe1e9c8e93261e978998c0e90e36275
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.3-pyhd8ed1ab_0.conda#063c1fda5480050b8d989478c97a4c55
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
+https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/noarch/torchinfo-1.8.0-pyhd8ed1ab_0.conda#fba98fc95a945e2a6b93a77b39dd52dc
 https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda#480cb2b6d502003e937d9e4326bc398f
 https://conda.anaconda.org/pytorch/osx-64/torchvision-0.15.2-py310_cpu.tar.bz2#5c3600915df5413045fc3335c7b66ece
 https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.14-pyhd8ed1ab_0.conda#43ed0c094b39bb352382db8105ab0b94
+https://conda.anaconda.org/conda-forge/noarch/conda-devenv-2.3.0-pyhd8ed1ab_0.tar.bz2#9b175e69c1c601d01ab5edccf822363c
 https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.3-pyhd8ed1ab_0.conda#f44109e52a40b8149156f5ddd9c11b26
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda#ce9d626b181c6f8cceb5047f6a819f7d
+https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.6-pyhd8ed1ab_0.conda#5325b6adf171d4d69968100af806994e
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py310h3900cf1_3.conda#02fb6b5a4f5a89fecae4a11d6bc4a0b1
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.3.0-pyhd8ed1ab_0.tar.bz2#83d1a712e6d2bab6b298b1d2f42ad355
 https://conda.anaconda.org/conda-forge/noarch/sphinx-external-toc-0.3.1-pyhd8ed1ab_0.conda#561bdf7b598d38e2962c46557bd1da12
 https://conda.anaconda.org/conda-forge/noarch/sphinx-jupyterbook-latex-0.5.2-pyhd8ed1ab_0.tar.bz2#88fc7863c8675f297b03e0ca50500b7f
@@ -381,18 +430,20 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinx-thebe-0.2.1-pyhd8ed1ab_0.conda#8a4151bde2af98c6cbc42ee12b48eb7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0.tar.bz2#382738101934261ea7931d1460e64868
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-dotnetdomain-0.4-py_0.tar.bz2#fb61a7369f505b4bb98e1530c3e09f9f
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-golangdomain-0.2.0.dev0-py_0.tar.bz2#d1a73c192888d08cedec232602c22f32
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jquery-4.1-pyhd8ed1ab_0.conda#914897066d5873acfb13e75705276ad1
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.3-pyhd8ed1ab_0.conda#f53d92ecd7d8563b006107f6a33e55c6
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/poetry-1.5.1-osx_pyhd8ed1ab_0.conda#cb22f4398986b6cde646b8ec6efe141f
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-5.4.3-pyhd8ed1ab_0.conda#3777f933bec5113d5a292de10b03d0f6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autoapi-2.1.0-pyhd8ed1ab_0.conda#6cb2b182390f837ce98737e92b9461f7
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
 https://conda.anaconda.org/conda-forge/noarch/sphinx_rtd_theme-1.2.2-pyha770c72_0.conda#5ef6aaf2cfb3b656cdadb431daed6a9f
 https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda#321151b2405f11ec6681a9a6f30822b4
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.0.5-pyhd8ed1ab_1.tar.bz2#1c31d380288fc1599fb5f4c76c8c828c
 https://conda.anaconda.org/conda-forge/noarch/jupyter-book-0.15.1-pyhd8ed1ab_0.conda#f10d556d3b3dc0aeae6aee37c412ea60
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/osx-64/jupyter-1.0.0-py310h2ec42d9_8.conda#89804ceb46b07bb0ee25093f4bfe97c7
```

### Comparing `hf-deepali-0.4.2/conda/environment.osx-64.yml` & `hf-deepali-0.4.3/conda/environment.osx-64.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 533a7567b393584157366e71374225596e814fe74cfcb03642d3b4e184d58c87
+# input_hash: 1e6e6cea02ff8fd576a8852899876561e48ebb709abcd877d8d931d3b50338da
 
 channels:
   - conda-forge
   - pytorch
   - nvidia
   - nodefaults
 dependencies:
   - bzip2=1.0.8=h0d85af4_4
   - c-ares=1.19.1=h0dc2134_0
-  - ca-certificates=2023.5.7=h8857fd0_0
+  - ca-certificates=2023.7.22=h8857fd0_0
   - font-ttf-dejavu-sans-mono=2.37=hab24e00_0
   - font-ttf-inconsolata=3.000=h77eed37_0
   - font-ttf-source-code-pro=2.038=h77eed37_0
   - font-ttf-ubuntu=0.83=hab24e00_0
   - fribidi=1.0.10=hbcb3906_0
   - giflib=5.2.1=hb7f2c08_3
   - jpeg=9e=hb7f2c08_3
@@ -47,61 +47,61 @@
   - x264=1!164.3095=h775f41a_2
   - xorg-libxau=1.0.11=h0dc2134_0
   - xorg-libxdmcp=1.1.3=h35c211d_0
   - xz=5.2.6=h775f41a_0
   - yaml=0.2.5=h0d85af4_2
   - aom=3.5.0=hf0c8a7f_0
   - double-conversion=3.2.0=hf0c8a7f_1
-  - eigen=3.4.1=h1c7c39f_0
+  - eigen=3.4.0=h1c7c39f_0
   - expat=2.5.0=hf0c8a7f_1
   - fonts-conda-forge=1=0
   - gettext=0.21.1=h8a4c099_0
   - glew=2.1.0=h046ec9c_2
   - gmp=6.2.1=h2e338ed_0
   - graphite2=1.3.13=h2e338ed_1001
   - icu=70.1=h96cf925_0
   - jsoncpp=1.9.5=h940c156_1
   - lerc=4.0.0=hb486fe8_0
   - libabseil=20230125.3=cxx17_h000cb23_0
   - libaec=1.0.6=hf0c8a7f_1
   - libbrotlidec=1.0.9=hb7f2c08_9
   - libbrotlienc=1.0.9=hb7f2c08_9
   - libedit=3.1.20191231=h0678c8f_2
-  - libgfortran5=12.2.0=he409387_31
+  - libgfortran5=12.3.0=hbd3c1fe_1
   - libllvm13=13.0.1=h64f94b2_2
   - libpng=1.6.39=ha978bb4_0
   - libsqlite=3.42.0=h58db7d2_0
   - libvorbis=1.3.7=h046ec9c_0
   - libvpx=1.11.0=he49afe7_3
   - libxcb=1.13=h0d85af4_1004
   - lz4-c=1.9.4=hf0c8a7f_0
   - nspr=4.35=hea0b92c_0
   - openh264=2.3.1=hf0c8a7f_2
-  - openssl=3.1.1=h8a1eda9_1
+  - openssl=3.1.2=h8a1eda9_0
   - p11-kit=0.24.1=h65f8906_0
   - pandoc=3.1.3=h9d075a6_0
   - pcre2=10.40=h1c4e4bc_0
   - pugixml=1.11.4=he965462_1
   - re2=2023.03.02=h096449b_0
   - readline=8.2=h9e318b2_1
   - svt-av1=1.4.1=hf0c8a7f_0
-  - tbb=2021.9.0=hb8565cd_0
+  - tbb=2021.10.0=h1c7c39f_0
   - tk=8.6.12=h5dbffcc_0
   - x265=3.5=hbb4e6a2_3
   - zeromq=4.3.4=he49afe7_1
   - zlib=1.2.13=h8a1eda9_5
   - zstd=1.5.2=h829000d_7
   - brotli-bin=1.0.9=hb7f2c08_9
   - fonts-conda-ecosystem=1=0
   - freetype=2.12.1=h3f81eb7_1
   - gl2ps=1.4.2=h4cff582_0
   - hdf4=4.2.15=h7aa5921_5
   - krb5=1.20.1=h049b76e_0
-  - libclang=13.0.1=default_h255f2f3_1
-  - libgfortran=5.0.0=11_3_0_h97931a8_31
+  - libclang=13.0.1=root_62804_h2961583_3
+  - libgfortran=5.0.0=12_3_0_h97931a8_1
   - libglib=2.76.4=hc62aa5d_0
   - libidn2=2.3.4=hb7f2c08_0
   - libnghttp2=1.52.0=he2ab024_0
   - libprotobuf=4.23.3=h5feb325_0
   - libssh2=1.11.0=hd019ec5_0
   - libtheora=1.1.1=h0d85af4_1005
   - libtiff=4.4.0=h6268bbc_5
@@ -109,34 +109,39 @@
   - libzip=1.9.2=h6db710c_1
   - mkl=2022.1.0=h860c996_928
   - mpfr=4.2.0=h4f9bd69_0
   - mysql-common=8.0.33=hc6116ba_2
   - nss=3.89=h78b00b3_0
   - python=3.10.12=had23ca6_0_cpython
   - sqlite=3.42.0=h2b0dec6_0
-  - tbb-devel=2021.9.0=hb8565cd_0
+  - tbb-devel=2021.10.0=h1c7c39f_0
   - absl-py=1.4.0=pyhd8ed1ab_0
   - alabaster=0.7.13=pyhd8ed1ab_0
+  - appdirs=1.4.4=pyh9f0ad1d_0
   - appnope=0.1.3=pyhd8ed1ab_0
   - atk-1.0=2.38.0=h1d18e73_1
   - attrs=21.4.0=pyhd8ed1ab_0
   - backcall=0.2.0=pyh9f0ad1d_0
   - backports=1.0=pyhd8ed1ab_3
   - blinker=1.6.2=pyhd8ed1ab_0
+  - boltons=23.0.0=pyhd8ed1ab_0
   - brotli=1.0.9=hb7f2c08_9
+  - cached_property=1.5.2=pyha770c72_1
   - cachetools=5.3.1=pyhd8ed1ab_0
-  - certifi=2023.5.7=pyhd8ed1ab_0
+  - certifi=2023.7.22=pyhd8ed1ab_0
   - charset-normalizer=3.2.0=pyhd8ed1ab_0
   - click=8.1.6=unix_pyh707e725_0
   - colorama=0.4.6=pyhd8ed1ab_0
+  - crashtest=0.4.1=pyhd8ed1ab_0
   - cycler=0.11.0=pyhd8ed1ab_0
   - dataclasses=0.8=pyhc8e2a94_3
-  - debugpy=1.6.7=py310h7a76584_0
+  - debugpy=1.6.8=py310h9e9d8ca_0
   - decorator=5.1.1=pyhd8ed1ab_0
   - defusedxml=0.7.1=pyhd8ed1ab_0
+  - distlib=0.3.7=pyhd8ed1ab_0
   - docutils=0.17.1=py310h2ec42d9_3
   - entrypoints=0.4=pyhd8ed1ab_0
   - exceptiongroup=1.1.2=pyhd8ed1ab_0
   - executing=1.2.0=pyhd8ed1ab_0
   - fftw=3.3.10=nompi_h4fa670e_108
   - filelock=3.12.2=pyhd8ed1ab_0
   - flit-core=3.9.0=pyhd8ed1ab_0
@@ -149,120 +154,140 @@
   - greenlet=2.0.2=py310h9e9d8ca_1
   - gts=0.7.6=h53e17e3_4
   - idna=3.4=pyhd8ed1ab_0
   - imagesize=1.4.1=pyhd8ed1ab_0
   - iniconfig=2.0.0=pyhd8ed1ab_0
   - ipython_genutils=0.2.0=py_1
   - jmespath=1.0.1=pyhd8ed1ab_0
+  - jsonpointer=2.0=py_0
   - jupyterlab_widgets=3.0.8=pyhd8ed1ab_0
   - kiwisolver=1.4.4=py310ha23aa8a_1
   - lazy-object-proxy=1.9.0=py310h90acd4f_0
   - lcms2=2.14=h90f4b2a_0
   - libblas=3.9.0=17_osx64_mkl
   - libcurl=8.1.2=hbee3ae8_0
   - libgrpc=1.56.2=he6801ca_0
   - libpq=15.3=h9dc22bb_1
   - libwebp=1.2.4=hfa4350a_0
+  - lockfile=0.12.2=py_1
   - loguru=0.7.0=py310h2ec42d9_0
   - markupsafe=2.1.3=py310h6729b98_0
   - mccabe=0.7.0=pyhd8ed1ab_0
   - mdurl=0.1.0=pyhd8ed1ab_0
   - mistune=3.0.0=pyhd8ed1ab_0
   - mkl-devel=2022.1.0=h694c41f_929
+  - more-itertools=10.1.0=pyhd8ed1ab_0
   - mpc=1.3.1=h81bd1dd_0
   - mpmath=1.3.0=pyhd8ed1ab_0
+  - msgpack-python=1.0.5=py310ha23aa8a_0
   - multidict=6.0.4=py310h90acd4f_0
   - munkres=1.1.4=pyh9f0ad1d_0
   - mypy_extensions=1.0.0=pyha770c72_0
   - mysql-libs=8.0.33=haa61052_2
   - nest-asyncio=1.5.6=pyhd8ed1ab_0
   - networkx=3.1=pyhd8ed1ab_0
   - openjpeg=2.5.0=h5d0d7b0_1
   - packaging=23.1=pyhd8ed1ab_0
   - pandocfilters=1.5.0=pyhd8ed1ab_0
   - parso=0.8.3=pyhd8ed1ab_0
-  - pathspec=0.11.1=pyhd8ed1ab_0
+  - pathspec=0.11.2=pyhd8ed1ab_0
   - pickleshare=0.7.5=py_1003
+  - pkginfo=1.9.6=pyhd8ed1ab_0
   - pkgutil-resolve-name=1.3.10=pyhd8ed1ab_0
   - pluggy=1.2.0=pyhd8ed1ab_0
   - ply=3.11=py_1
   - prometheus_client=0.17.1=pyhd8ed1ab_0
   - psutil=5.9.5=py310h90acd4f_0
   - ptyprocess=0.7.0=pyhd3deb0d_0
   - pure_eval=0.2.2=pyhd8ed1ab_0
   - pyasn1=0.4.8=py_0
   - pycodestyle=2.10.0=pyhd8ed1ab_0
+  - pycosat=0.6.4=py310h90acd4f_1
   - pycparser=2.21=pyhd8ed1ab_0
   - pyflakes=3.0.1=pyhd8ed1ab_0
   - pygments=2.15.1=pyhd8ed1ab_0
   - pyjwt=2.8.0=pyhd8ed1ab_0
   - pyparsing=3.0.9=pyhd8ed1ab_0
   - pyrsistent=0.19.3=py310h90acd4f_0
   - pysocks=1.7.1=pyha2e5f31_6
-  - python-fastjsonschema=2.17.1=pyhd8ed1ab_0
+  - python-fastjsonschema=2.18.0=pyhd8ed1ab_0
+  - python-installer=0.7.0=pyhd8ed1ab_0
   - python-json-logger=2.0.7=pyhd8ed1ab_0
   - pytz=2023.3=pyhd8ed1ab_0
   - pyyaml=6.0=py310h90acd4f_5
   - pyzmq=25.1.0=py310h998be00_0
   - rfc3986-validator=0.1.1=pyh9f0ad1d_0
   - ruamel.yaml.clib=0.2.7=py310h90acd4f_1
   - setuptools=67.7.2=pyhd8ed1ab_0
+  - shellingham=1.5.1=pyhd8ed1ab_0
   - six=1.16.0=pyh6c4a22f_0
   - sniffio=1.3.0=pyhd8ed1ab_0
   - snowballstemmer=2.2.0=pyhd8ed1ab_0
   - soupsieve=2.3.2.post1=pyhd8ed1ab_0
   - sphinxcontrib-applehelp=1.0.4=pyhd8ed1ab_0
   - sphinxcontrib-devhelp=1.0.2=py_0
   - sphinxcontrib-htmlhelp=2.0.1=pyhd8ed1ab_0
   - sphinxcontrib-jsmath=1.0.1=py_0
   - sphinxcontrib-qthelp=1.0.3=py_0
   - sphinxcontrib-serializinghtml=1.1.5=pyhd8ed1ab_2
   - tabulate=0.9.0=pyhd8ed1ab_1
   - tensorboard-data-server=0.7.0=py310hdd0c95c_0
   - toml=0.10.2=pyhd8ed1ab_0
   - tomli=2.0.1=pyhd8ed1ab_0
+  - tomlkit=0.12.1=pyha770c72_0
+  - toolz=0.12.0=pyhd8ed1ab_0
   - tornado=6.3.2=py310h6729b98_0
   - traitlets=5.9.0=pyhd8ed1ab_0
+  - trove-classifiers=2023.7.6=pyhd8ed1ab_0
   - typed-ast=1.5.4=py310h90acd4f_1
+  - typing=3.10.0.0=pyhd8ed1ab_0
   - typing_extensions=4.7.1=pyha770c72_0
   - typing_utils=0.1.0=pyhd8ed1ab_0
   - uc-micro-py=1.0.1=pyhd8ed1ab_0
   - unicodedata2=15.0.0=py310h90acd4f_0
   - unidecode=1.3.6=pyhd8ed1ab_0
+  - uri-template=1.3.0=pyhd8ed1ab_0
+  - webcolors=1.13=pyhd8ed1ab_0
   - webencodings=0.5.1=py_1
   - websocket-client=1.6.1=pyhd8ed1ab_0
-  - wheel=0.40.0=pyhd8ed1ab_1
+  - wheel=0.41.0=pyhd8ed1ab_0
   - widgetsnbextension=4.0.8=pyhd8ed1ab_0
   - wrapt=1.15.0=py310h90acd4f_0
   - zipp=3.16.2=pyhd8ed1ab_0
   - accessible-pygments=0.0.4=pyhd8ed1ab_0
   - aiosignal=1.3.1=pyhd8ed1ab_0
   - anyio=3.7.1=pyhd8ed1ab_0
   - asttokens=2.2.1=pyhd8ed1ab_0
   - babel=2.12.1=pyhd8ed1ab_1
+  - backports.cached-property=1.0.2=pyhd8ed1ab_0
   - backports.functools_lru_cache=1.6.5=pyhd8ed1ab_0
   - beautifulsoup4=4.12.2=pyha770c72_0
   - bleach=6.0.0=pyhd8ed1ab_0
+  - cached-property=1.5.2=hd8ed1ab_1
   - cairo=1.16.0=h904041c_1014
   - cffi=1.15.1=py310ha78151a_3
-  - comm=0.1.3=pyhd8ed1ab_0
+  - click-default-group=1.2.2=pyhd8ed1ab_1
+  - comm=0.1.4=pyhd8ed1ab_0
   - curl=8.1.2=hbee3ae8_0
   - dacite=1.8.0=pyhd8ed1ab_0
   - deprecation=2.1.0=pyh9f0ad1d_0
   - ffmpeg=5.1.2=gpl_h8b4fe81_106
   - flake8=6.0.0=pyhd8ed1ab_0
-  - fonttools=4.41.0=py310h6729b98_0
+  - fonttools=4.42.0=py310h6729b98_0
   - glib=2.76.4=h7d26f99_0
   - gmpy2=2.1.2=py310hb691cb2_1
   - grpcio=1.56.2=py310h0d4bf3c_0
   - hdf5=1.12.2=nompi_h48135f9_101
+  - html5lib=1.1=pyh9f0ad1d_0
   - importlib-metadata=6.8.0=pyha770c72_0
   - importlib_resources=6.0.0=pyhd8ed1ab_1
-  - jedi=0.18.2=pyhd8ed1ab_0
+  - jaraco.classes=3.3.0=pyhd8ed1ab_0
+  - jedi=0.19.0=pyhd8ed1ab_0
   - jinja2=3.1.2=pyhd8ed1ab_1
+  - jsonpatch=1.32=pyhd8ed1ab_0
   - jupyterlab_pygments=0.2.2=pyhd8ed1ab_0
   - latexcodec=2.0.1=pyh9f0ad1d_0
   - libcblas=3.9.0=17_osx64_mkl
   - libgd=2.3.3=h1e214de_3
   - liblapack=3.9.0=17_osx64_mkl
   - lightning-utilities=0.9.0=pyhd8ed1ab_0
   - linkify-it-py=2.0.0=pyhd8ed1ab_0
@@ -280,105 +305,129 @@
   - pytest=7.3.2=pyhd8ed1ab_1
   - python-dateutil=2.8.2=pyhd8ed1ab_0
   - pyu2f=0.1.5=pyhd8ed1ab_0
   - qtpy=2.3.1=pyhd8ed1ab_0
   - rfc3339-validator=0.1.4=pyhd8ed1ab_0
   - rsa=4.9=pyhd8ed1ab_0
   - ruamel.yaml=0.17.32=py310h6729b98_0
-  - sip=6.7.9=py310h9e9d8ca_0
+  - sip=6.7.11=py310h9e9d8ca_0
   - terminado=0.17.1=pyhd1c38e8_0
   - tinycss2=1.2.1=pyhd8ed1ab_0
   - tqdm=4.65.0=pyhd8ed1ab_1
   - typing-extensions=4.7.1=hd8ed1ab_0
   - werkzeug=2.3.6=pyhd8ed1ab_0
   - yarl=1.9.2=py310h6729b98_0
+  - annotated-types=0.5.0=pyhd8ed1ab_0
   - argon2-cffi-bindings=21.2.0=py310h90acd4f_3
+  - arrow=1.2.3=pyhd8ed1ab_0
   - astroid=2.15.6=py310h2ec42d9_0
   - async-timeout=4.0.2=pyhd8ed1ab_0
   - brotlipy=0.7.0=py310h90acd4f_1005
   - cryptography=41.0.2=py310ha1817de_0
+  - fqdn=1.5.1=pyhd8ed1ab_0
   - ghp-import=2.1.0=pyhd8ed1ab_0
-  - gstreamer=1.22.4=h840fbdc_1
+  - gstreamer=1.22.5=h840fbdc_0
   - harfbuzz=6.0.0=h08f8713_0
   - importlib_metadata=6.8.0=hd8ed1ab_0
   - jsonschema=4.17.3=pyhd8ed1ab_0
   - jupyter_server_terminals=0.4.4=pyhd8ed1ab_1
   - libitk=5.3.0=h10ab89a_0
   - liblapacke=3.9.0=17_osx64_mkl
   - libnetcdf=4.8.1=nompi_hc61b76e_106
-  - markdown=3.4.3=pyhd8ed1ab_0
+  - markdown=3.4.4=pyhd8ed1ab_0
   - mdit-py-plugins=0.4.0=pyhd8ed1ab_0
-  - numpy=1.25.1=py310h7451ae0_0
-  - platformdirs=3.9.1=pyhd8ed1ab_0
+  - numpy=1.25.2=py310h7451ae0_0
+  - platformdirs=3.10.0=pyhd8ed1ab_0
+  - poetry-core=1.6.1=pyhd8ed1ab_0
   - pybtex=0.24.0=pyhd8ed1ab_2
+  - pydantic-core=2.4.0=py310h3461e44_0
   - pyobjc-framework-cocoa=9.2=py310hef2d279_0
-  - pyqt5-sip=12.11.0=py310h415000c_3
+  - pyqt5-sip=12.12.2=py310h018f80b_4
   - python-build=0.10.0=pyhd8ed1ab_1
   - setuptools-scm=7.1.0=pyhd8ed1ab_0
   - sqlalchemy=2.0.19=py310h6729b98_0
   - stack_data=0.6.2=pyhd8ed1ab_0
   - sympy=1.12=pypyh9d50eac_103
   - wcwidth=0.2.6=pyhd8ed1ab_0
+  - xattr=0.10.1=py310h90acd4f_0
+  - zstandard=0.19.0=py310h151724a_2
   - aiohttp=3.8.5=py310h6729b98_0
   - argon2-cffi=21.3.0=pyhd8ed1ab_0
   - black=22.3.0=pyhd8ed1ab_0
   - blas-devel=3.9.0=17_osx64_mkl
+  - conda-package-streaming=0.9.0=pyhd8ed1ab_0
   - contourpy=1.1.0=py310h88cfcbd_0
-  - gst-plugins-base=1.22.4=hb5d3a86_1
+  - gst-plugins-base=1.22.5=hb5d3a86_0
+  - isoduration=20.11.0=pyhd8ed1ab_0
   - jupyter_core=5.3.1=py310h2ec42d9_0
-  - jupyter_events=0.6.3=pyhd8ed1ab_0
+  - keyring=23.13.1=py310h2ec42d9_0
   - nibabel=5.1.0=py310h2ec42d9_2
   - oauthlib=3.2.2=pyhd8ed1ab_0
   - pandas=1.5.3=py310hecf8f37_1
   - pango=1.50.14=hbd9bf65_0
+  - poetry-plugin-export=1.4.0=pyhd8ed1ab_0
   - prompt-toolkit=3.0.39=pyha770c72_0
   - pybtex-docutils=1.0.2=py310h2ec42d9_2
+  - pydantic=2.1.1=pyhd8ed1ab_0
   - pyopenssl=23.2.0=pyhd8ed1ab_1
+  - rapidfuzz=2.15.1=py310h7a76584_0
   - send2trash=1.8.2=pyhd1c38e8_0
   - simpleitk=2.2.1=py310h4447650_1
+  - virtualenv=20.24.2=pyhd8ed1ab_0
   - blas=2.117=mkl
+  - cleo=2.0.1=pyhd8ed1ab_0
+  - conda-package-handling=2.2.0=pyh38be061_0
   - flake8-black=0.3.6=pyhd8ed1ab_0
   - gtk2=2.24.33=h7c1209e_2
+  - jsonschema-with-format-nongpl=4.17.3=pyhd8ed1ab_0
   - jupyter_client=8.3.0=pyhd8ed1ab_0
   - librsvg=2.54.4=h3d48ba6_0
   - matplotlib-base=3.7.2=py310h475a17b_0
-  - nbformat=5.9.1=pyhd8ed1ab_0
+  - nbformat=5.9.2=pyhd8ed1ab_0
   - prompt_toolkit=3.0.39=hd8ed1ab_0
   - qt-main=5.15.8=h1d3b3f8_6
   - urllib3=1.26.15=pyhd8ed1ab_0
   - wslink=1.11.1=pyhd8ed1ab_0
   - botocore=1.29.165=pyhd8ed1ab_0
+  - dulwich=0.21.5=py310h6729b98_0
   - graphviz=7.0.5=hc51f7b9_0
   - ipython=8.14.0=pyhd1c38e8_0
+  - jupyter_events=0.7.0=pyhd8ed1ab_0
   - matplotlib=3.7.2=py310h2ec42d9_0
   - nbclient=0.7.4=pyhd8ed1ab_0
-  - pyqt=5.15.7=py310hdd03f62_3
+  - pyqt=5.15.9=py310hecc045f_4
   - pytorch=2.0.1=py3.10_0
   - requests=2.31.0=pyhd8ed1ab_0
   - vtk=9.2.5=qt_py310hea5b068_200
+  - cachecontrol=0.12.14=pyhd8ed1ab_0
+  - conda=23.7.2=py310h2ec42d9_0
+  - ensureconda=1.4.3=pyhd8ed1ab_0
   - google-auth=2.22.0=pyh1a96a4e_0
   - ipykernel=6.23.3=pyh5fb750a_0
+  - ipywidgets=8.1.0=pyhd8ed1ab_0
   - jupyter-cache=0.6.1=pyhd8ed1ab_0
-  - nbconvert-core=7.7.1=pyhd8ed1ab_1
+  - nbconvert-core=7.7.3=pyhd8ed1ab_0
   - pooch=1.7.0=pyha770c72_3
   - requests-oauthlib=1.3.1=pyhd8ed1ab_0
+  - requests-toolbelt=1.0.0=pyhd8ed1ab_0
   - s3transfer=0.6.1=pyhd8ed1ab_0
   - sphinx=4.5.0=pyh6c4a22f_0
   - torchinfo=1.8.0=pyhd8ed1ab_0
   - torchmetrics=0.11.4=pyhd8ed1ab_0
   - torchvision=0.15.2=py310_cpu
   - boto3=1.26.165=pyhd8ed1ab_0
+  - cachecontrol-with-filecache=0.12.14=pyhd8ed1ab_0
+  - conda-devenv=2.3.0=pyhd8ed1ab_0
   - google-auth-oauthlib=1.0.0=pyhd8ed1ab_1
-  - ipywidgets=8.0.7=pyhd8ed1ab_0
   - jupyter_console=6.6.3=pyhd8ed1ab_0
   - jupyter_server=2.7.0=pyhd8ed1ab_0
   - myst-parser=0.18.1=pyhd8ed1ab_0
-  - nbconvert-pandoc=7.7.1=pyhd8ed1ab_1
+  - nbconvert-pandoc=7.7.3=pyhd8ed1ab_0
   - pydata-sphinx-theme=0.13.3=pyhd8ed1ab_0
-  - pytorch-lightning=2.0.4=pyhd8ed1ab_0
+  - pytorch-lightning=2.0.6=pyhd8ed1ab_0
   - qtconsole-base=5.4.3=pyha770c72_0
   - scipy=1.10.1=py310h3900cf1_3
   - sphinx-comments=0.0.3=pyh9f0ad1d_0
   - sphinx-copybutton=0.5.2=pyhd8ed1ab_0
   - sphinx-design=0.3.0=pyhd8ed1ab_0
   - sphinx-external-toc=0.3.1=pyhd8ed1ab_0
   - sphinx-jupyterbook-latex=0.5.2=pyhd8ed1ab_0
@@ -387,18 +436,20 @@
   - sphinx-thebe=0.2.1=pyhd8ed1ab_0
   - sphinx-togglebutton=0.3.2=pyhd8ed1ab_0
   - sphinxcontrib-bibtex=2.5.0=pyhd8ed1ab_0
   - sphinxcontrib-dotnetdomain=0.4=py_0
   - sphinxcontrib-golangdomain=0.2.0.dev0=py_0
   - sphinxcontrib-jquery=4.1=pyhd8ed1ab_0
   - myst-nb=0.17.2=pyhd8ed1ab_0
-  - nbconvert=7.7.1=pyhd8ed1ab_1
+  - nbconvert=7.7.3=pyhd8ed1ab_0
   - notebook-shim=0.2.3=pyhd8ed1ab_0
+  - poetry=1.5.1=osx_pyhd8ed1ab_0
   - qtconsole=5.4.3=pyhd8ed1ab_0
   - sphinx-autoapi=2.1.0=pyhd8ed1ab_0
   - sphinx-book-theme=1.0.1=pyhd8ed1ab_0
   - sphinx_rtd_theme=1.2.2=pyha770c72_0
   - tensorboard=2.13.0=pyhd8ed1ab_0
+  - conda-lock=1.0.5=pyhd8ed1ab_1
   - jupyter-book=0.15.1=pyhd8ed1ab_0
   - nbclassic=1.0.0=pyhb4ecaf3_1
   - notebook=6.5.4=pyha770c72_0
   - jupyter=1.0.0=py310h2ec42d9_8
```

### Comparing `hf-deepali-0.4.2/conda/environment.win-64.lock` & `hf-deepali-0.4.3/conda/environment.win-64.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: 6255d416b6866feefaa84cbaf27b3a7608f8bb60e8d5e51ca00574e0f3970f20
+# input_hash: f9e524a368611b4591c0b79cc851d7fd034bcb935240ad118e3fe4c7b27edeb4
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.7.22-h56e8100_0.conda#b1c2327b36f1a25d96f2039b0d3e3739
 https://conda.anaconda.org/conda-forge/win-64/cuda-cccl-impl-2.0.1-h57928b3_0.conda#6ddbe275ebb9ae875355baf8ade34b3f
 https://conda.anaconda.org/nvidia/win-64/cuda-cudart-11.8.89-0.tar.bz2#cd0f6ab42e0ccba5f6899c531ea193c1
 https://conda.anaconda.org/nvidia/win-64/cuda-cupti-11.8.87-0.tar.bz2#f18f6268a222d476c804d4adadd4926a
 https://conda.anaconda.org/nvidia/win-64/cuda-nvrtc-11.8.89-0.tar.bz2#d692bd090a4a9638ac15709cde2400da
 https://conda.anaconda.org/nvidia/win-64/cuda-nvtx-11.8.86-0.tar.bz2#7874207353c834d34217555785859dba
-https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.2.53-0.tar.bz2#93cb84c3524a1612cbce98ead299c735
+https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.2.128-0.tar.bz2#d3277124e5bca9acbd74ad709d1714b5
 https://conda.anaconda.org/conda-forge/noarch/cuda-version-12.0-hffde075_2.conda#c9f9d925118c389a1a3f4267b6272b98
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2023.1.0-h57928b3_46319.conda#dbc4636f419722fbf3ab6501377228ba
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2023.2.0-h57928b3_49496.conda#f2e71622520883ffdbc379b13049534c
 https://conda.anaconda.org/nvidia/win-64/libcublas-11.11.3.6-0.tar.bz2#750e01875ed59059ae043d09d262968d
 https://conda.anaconda.org/nvidia/win-64/libcufft-10.9.0.58-0.tar.bz2#df178db30b5abcaa0a5f3a369a1fe19c
 https://conda.anaconda.org/nvidia/win-64/libcusolver-11.4.1.48-0.tar.bz2#43cd3c2bcbdfac91708e96fe6b554676
 https://conda.anaconda.org/nvidia/win-64/libcusparse-11.7.5.86-0.tar.bz2#b2cbca2503fdb48486228f97265fc4dd
 https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
 https://conda.anaconda.org/nvidia/win-64/libnpp-11.8.0.86-0.tar.bz2#84696e7fac0af2c9fe57eec5e2ca56f5
 https://conda.anaconda.org/nvidia/win-64/libnvjpeg-11.9.0.86-0.tar.bz2#9ddfe10567159ae9380d4b10d8cf1670
@@ -52,15 +52,15 @@
 https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/aom-3.5.0-h63175ca_0.tar.bz2#455524d2bf9625a42a1848c0d08ac063
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
 https://conda.anaconda.org/conda-forge/win-64/c-ares-1.19.1-hcfcfb64_0.conda#8aa74d9a74ed3a31d9ed38a387a8ca50
 https://conda.anaconda.org/nvidia/win-64/cuda-cudart-dev-11.8.89-0.tar.bz2#a4b0b3a1b7aa79ff39f6d3b1e7c62de3
 https://conda.anaconda.org/conda-forge/win-64/dav1d-1.2.0-hcfcfb64_0.conda#0ce7020bd3aadfb999f987d2b1cc0e25
 https://conda.anaconda.org/conda-forge/win-64/double-conversion-3.2.0-h63175ca_1.tar.bz2#d1b86ea3cf6e902694a592e6440b1fa5
-https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.1-h91493d7_0.conda#3671ee2bcd1d915690de5b1445fdf004
+https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.0-h91493d7_0.conda#305b3ca7023ac046b9a42a48661f6512
 https://conda.anaconda.org/conda-forge/win-64/fftw-3.3.10-nompi_h38027f0_108.conda#09196a7ba69b70d2124aff7b2763035d
 https://conda.anaconda.org/conda-forge/win-64/fribidi-1.0.10-h8d14728_0.tar.bz2#807e81d915f2bb2e49951648615241f6
 https://conda.anaconda.org/conda-forge/win-64/getopt-win32-0.1-h8ffe710_0.tar.bz2#9ac4874e2958f18e01c386649208fe40
 https://conda.anaconda.org/conda-forge/win-64/glew-2.1.0-h39d44d4_2.tar.bz2#840d21c1ee66b91af3d0211e7766393a
 https://conda.anaconda.org/conda-forge/win-64/graphite2-1.3.13-1000.tar.bz2#8fc0e04e5c852cadf2cad68b86a906ab
 https://conda.anaconda.org/conda-forge/win-64/icu-70.1-h0e60522_0.tar.bz2#64073396a905b6df895ab2489fae3847
 https://conda.anaconda.org/conda-forge/win-64/jpeg-9e-hcfcfb64_3.conda#824f1e030d224e9e376a4655032fdbc7
@@ -73,21 +73,21 @@
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.14-hcfcfb64_0.tar.bz2#4366e00d3270eb229c026920474a6dda
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
 https://conda.anaconda.org/conda-forge/win-64/libopus-1.3.1-h8ffe710_1.tar.bz2#e35a6bcfeb20ea83aab21dfc50ae62a4
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libuv-1.44.2-h8ffe710_0.tar.bz2#0d45ae978c33ff0b5f95ea24c717d5cf
+https://conda.anaconda.org/conda-forge/win-64/libuv-1.44.2-hcfcfb64_1.conda#db1816a489a1b69dd1fd93e523cf026a
 https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.1-hcfcfb64_0.conda#f89e765213cac556a8ed72ba8c1b5071
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openh264-2.3.1-h63175ca_2.conda#76e822d93cdc32b00b61810d3fa030e0
-https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.2-hcfcfb64_0.conda#79b3f40f27cd80a265c276cea6714507
 https://conda.anaconda.org/conda-forge/win-64/pixman-0.40.0-h8ffe710_0.tar.bz2#32b45d3fcffddc84cc1a014a0b5f0d58
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
 https://conda.anaconda.org/conda-forge/win-64/pugixml-1.11.4-h63175ca_1.conda#ab36cd750c0828a85bf00259f3442208
 https://conda.anaconda.org/conda-forge/win-64/re2-2023.03.02-hd4eee63_0.conda#a59c371d7364446cf1d0b8299e05c1ea
 https://conda.anaconda.org/conda-forge/win-64/svt-av1-1.4.1-h63175ca_0.conda#4e0b494c944e58a4de7aed21bb80645c
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
 https://conda.anaconda.org/conda-forge/win-64/x264-1!164.3095-h8ffe710_2.tar.bz2#19e39905184459760ccb8cf5c75f148b
@@ -95,15 +95,15 @@
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/nvidia/win-64/cuda-libraries-11.8.0-0.tar.bz2#4a0d16015f1480c6b6845a4d17b9563b
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.21.1-h5728263_0.tar.bz2#299d4fd6798a45337042ff5a48219e5f
 https://conda.anaconda.org/conda-forge/win-64/krb5-1.20.1-heb0366b_0.conda#a07b05ee8f451ab15698397185efe989
 https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_9.conda#4c502e4846bdc22b944ab9aa5a55a58f
 https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_9.conda#19029748649ae0d48871d7012918efef
-https://conda.anaconda.org/conda-forge/win-64/libclang13-15.0.7-default_h77d9078_2.conda#c2e1def32a19610ac26db453501760b6
+https://conda.anaconda.org/conda-forge/win-64/libclang13-15.0.7-default_h77d9078_3.conda#ba26634d038b91466bb4242c8b5e0cfa
 https://conda.anaconda.org/conda-forge/win-64/libcurand-dev-10.3.1.50-h63175ca_0.conda#e6c08a829cbd187b1b0e2eafa8f2712e
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.39-h19919ed_0.conda#ab6febdb2dbd9c00803609079db4de71
 https://conda.anaconda.org/conda-forge/win-64/libprotobuf-4.23.3-h1975477_0.conda#6386184da6e9e58de0d8e0a9e9aeb736
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libtheora-1.1.1-h8d14728_1005.tar.bz2#8ad3f8ea1dbd5ac4fe1299a3250cbd1b
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
 https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.1-hcfcfb64_0.conda#cc9d668f51da7f6506185ab1130bcd57
@@ -114,30 +114,35 @@
 https://conda.anaconda.org/conda-forge/win-64/python-3.10.12-h4de0772_0_cpython.conda#14273454ca348a123ce09ab9d39c1a6e
 https://conda.anaconda.org/conda-forge/win-64/sqlite-3.42.0-hcfcfb64_0.conda#c505cc64dba674d4c419c0de772c8579
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_7.conda#f3c3879d8cda1c5a6885435dd48a470e
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
+https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
+https://conda.anaconda.org/conda-forge/noarch/boltons-23.0.0-pyhd8ed1ab_0.conda#033eb25fffd222aceeca6d58cd953680
 https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_9.conda#ba8ae6c24cf47da3fb73270e4f119f08
+https://conda.anaconda.org/conda-forge/noarch/cached_property-1.5.2-pyha770c72_1.tar.bz2#576d629e47797577ab0f1b351297ef4a
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
-https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.7.22-pyhd8ed1ab_0.conda#7f3dbc9179b4dde7da98dfb151d0ad22
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/nvidia/win-64/cuda-libraries-dev-11.8.0-0.tar.bz2#4dceddb905013e47bee99757d42dfdd4
 https://conda.anaconda.org/nvidia/win-64/cuda-runtime-11.8.0-0.tar.bz2#9782ebd2dc96d2fd463c0d4a99254da6
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
-https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py310h00ffb61_0.conda#b7defb941402f3581384d16070ed1456
+https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.8-py310h00ffb61_0.conda#8c8e0940454d91fd5d24dc82c3f76a29
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda#12d8aae6994f342618443a8f05c652a0
 https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py310h5588dad_3.tar.bz2#cdc0acfc953b7bd34229b7f229eae46a
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-h546665d_1.conda#1b513009cd012591f3fdc9e03a74ec0a
@@ -147,88 +152,105 @@
 https://conda.anaconda.org/conda-forge/win-64/greenlet-2.0.2-py310h00ffb61_1.conda#7535b10dbe0b5fbf63fede10a4f8666b
 https://conda.anaconda.org/conda-forge/win-64/hdf4-4.2.15-h1b1b6ef_5.tar.bz2#bfb6a2d82ef9a30455cc0900d89eed20
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
+https://conda.anaconda.org/conda-forge/noarch/jsonpointer-2.0-py_0.tar.bz2#07d85c22a3beb102a48cd123df84c2a6
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.4-py310h232114e_1.tar.bz2#c55fe943d5f212d49d27d08580f5a610
 https://conda.anaconda.org/conda-forge/win-64/lazy-object-proxy-1.9.0-py310h8d17308_0.conda#696baee03eafd09ed9c4ab6a095b620f
-https://conda.anaconda.org/conda-forge/win-64/libclang-15.0.7-default_h77d9078_2.conda#70188b1b3e0b1716405adab9050894d1
+https://conda.anaconda.org/conda-forge/win-64/libclang-15.0.7-default_h77d9078_3.conda#71c8b6249c9e9e18b3aec705e95c1040
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.1.2-h68f0423_0.conda#94b9b7d0e882461fdb72d8d4e7441746
 https://conda.anaconda.org/conda-forge/win-64/libglib-2.76.4-he8f3873_0.conda#8c3f24acdc0403eeb3fb42ab75e8a659
 https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.56.2-hea2d5f7_0.conda#240221f7a200e718c242637e6c437b61
 https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.1-h51c2c0f_0.conda#8ec5920f3ed67faa0264a36c0b533ed0
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.4.0-hc4f729c_5.conda#fe00c2f95c1215e355c34094b00480d7
+https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py310h8d17308_0.conda#e6deeae9d0dac4d17c6ef2fa62b3efff
 https://conda.anaconda.org/conda-forge/noarch/mccabe-0.7.0-pyhd8ed1ab_0.tar.bz2#34fc335fc50eef0b5ea708f2b5f54e0c
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
+https://conda.anaconda.org/conda-forge/win-64/menuinst-1.4.19-py310h5588dad_1.tar.bz2#15cfc917187d7c173647dd65d340259b
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
+https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.1.0-pyhd8ed1ab_0.conda#8549fafed0351bbfaa1ddaa15fdf9b4e
 https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda#dbf6e2d89137da32fa6670f3bffc024e
+https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.5-py310h232114e_0.conda#03f6096e23f3861934af853ac987c185
 https://conda.anaconda.org/conda-forge/win-64/multidict-6.0.4-py310h8d17308_0.conda#23a55d74d8f91c7667555b81030034bf
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
+https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.2-pyhd8ed1ab_0.conda#e41debb259e68490e3ab81e46b639ab6
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
+https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py310h8d17308_0.conda#9f98965e4f7dc2e4eb84abd50406d3a0
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
+https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
+https://conda.anaconda.org/conda-forge/win-64/pycosat-0.6.4-py310h8d17308_1.tar.bz2#3324f50e5d46a04309d8f8f956c17244
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyflakes-3.0.1-pyhd8ed1ab_0.conda#44b7d77d96560c93e0e11437a3c35254
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda#912c0194f898fdb783021fd25f913c31
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
 https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py310h8d17308_0.conda#ddba6aad7d1857d16675d41a6e8b0224
-https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.18.0-pyhd8ed1ab_0.conda#3be9466311564f80f8056c0851fc5bb7
+https://conda.anaconda.org/conda-forge/noarch/python-installer-0.7.0-pyhd8ed1ab_0.conda#65dea78f903d686c8b0c2feaf0e15e1f
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py310h00ffb61_2.tar.bz2#e1401844b4f4ec959e099452a953e764
+https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py310h5588dad_0.conda#9f60b973d0238c7e62a2324767acb62f
 https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.11-py310h00ffb61_0.conda#685cf7fe1b0724628476c991329017ad
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py310h8d17308_5.tar.bz2#d0daf3eed98dd2bf4337ed08d8011eb8
 https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py310hcd737a0_0.conda#75b926fbf2e2c67eb5210c68e1ac8f18
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.7-py310h8d17308_1.conda#e7cee92d4b0e9f8a68823d2501a87063
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.1-pyhd8ed1ab_0.conda#1de44299f48f522caa2e0074231614e1
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/win-64/tensorboard-data-server-0.7.0-py310h5588dad_0.conda#1aa33e391e578ec1f6b23d10e005aa2e
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.1-pyha770c72_0.conda#62f5b331c53d73e2f6c4c130b53518a0
+https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py310h8d17308_0.conda#6cd035ff75b46eb8ae7403b3dded2def
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2023.7.6-pyhd8ed1ab_0.conda#c9918f6a3973e28a792e747289734cd3
 https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.5-py310h8d17308_0.conda#a2ac0e6c5a06b35dea207c3d77f94f74
+https://conda.anaconda.org/conda-forge/noarch/typing-3.10.0.0-pyhd8ed1ab_0.tar.bz2#e6573ac68718f17b9d4f5c8eda3190f2
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.0.0-py310h8d17308_0.tar.bz2#5d14ba562f7740b64be9c8059498cfbf
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
+https://conda.anaconda.org/conda-forge/noarch/uri-template-1.3.0-pyhd8ed1ab_0.conda#0944dc65cb4a9b5b68522c3bb585d41c
+https://conda.anaconda.org/conda-forge/noarch/webcolors-1.13-pyhd8ed1ab_0.conda#166212fe82dad8735550030488a01d03
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.41.0-pyhd8ed1ab_0.conda#66beb36a1fa7e0dc9d9bf843a80eb82c
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win32_setctime-1.1.0-pyhd8ed1ab_0.tar.bz2#dc80c0c2b01f7d6d6d5df4b63ef54f17
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/wrapt-1.15.0-py310h8d17308_0.conda#2ec4d850e6fbe1da9971a7bb801a1ebd
 https://conda.anaconda.org/conda-forge/win-64/xorg-kbproto-1.0.7-hcd874cb_1002.tar.bz2#8d11c1dac4756ca57e78c1bfe173bba4
 https://conda.anaconda.org/conda-forge/win-64/xorg-libice-1.0.10-hcd874cb_0.tar.bz2#8f45beee385cb67e42d6732bdb1b6a40
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
@@ -237,45 +259,51 @@
 https://conda.anaconda.org/conda-forge/win-64/xorg-xproto-7.0.31-hcd874cb_1007.tar.bz2#88f3c65d2ad13826a9e0b162063be023
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
+https://conda.anaconda.org/conda-forge/noarch/backports.cached-property-1.0.2-pyhd8ed1ab_0.tar.bz2#0e1df3978dd516e20ef88c86d51e5432
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_9.conda#5275e2634840f6d156934a16b7c0c813
+https://conda.anaconda.org/conda-forge/noarch/cached-property-1.5.2-hd8ed1ab_1.tar.bz2#9b347a7ec10940d3f7941ff6c460b551
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py310h628cb3f_3.conda#b7ca236d34501eb6a70691c1e29a0234
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-win_pyh7428d3b_0.conda#c1e57b6771510a3d2648ed6e76277391
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.4-pyhd8ed1ab_0.conda#c8eaca39e2b6abae1fc96acc929ae939
 https://conda.anaconda.org/conda-forge/win-64/curl-8.1.2-h68f0423_0.conda#fc67d347f9eaa7922fd7bc26bfa5419b
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
 https://conda.anaconda.org/conda-forge/win-64/fontconfig-2.14.2-hbde0cde_0.conda#08767992f1a4f1336a257af1241034bd
 https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.76.4-h12be248_0.conda#88237d3ddd338164196043cb7e927246
 https://conda.anaconda.org/conda-forge/win-64/grpcio-1.56.2-py310hb84602e_0.conda#1c43b1323746f119bfea36e689930225
 https://conda.anaconda.org/conda-forge/win-64/gts-0.7.6-h6b5321d_4.conda#a41f14768d5e377426ad60c613f2923b
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.12.2-nompi_h57737ce_101.conda#3e2b84f2f7bcf6915d1baa21e5b1a862
+https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda#e9f79248d30e942f7c358ff21a1790f5
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.0-pyhd8ed1ab_0.conda#1cd7f70057cdffc10977b613fb75425d
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/noarch/jsonpatch-1.32-pyhd8ed1ab_0.tar.bz2#09150b51b0528a31a0f6500b96fdde82
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.14-h90d422f_0.tar.bz2#a0deec92aa16fca7bf5a6717d05f88ee
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.13-hcd874cb_1004.tar.bz2#a6d7fd030532378ecb6ba435cd9f8234
 https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda#c71f7ec8b80a536e58b979299b230251
 https://conda.anaconda.org/conda-forge/noarch/linkify-it-py-2.0.0-pyhd8ed1ab_0.tar.bz2#25b93e66067eb496ac10da888e25cc33
 https://conda.anaconda.org/conda-forge/win-64/loguru-0.7.0-py310h5588dad_0.conda#418204da701dc43d8992ba8131c17848
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.0-hc9384bd_1.tar.bz2#a6834096f8d834339eca7ef4d23bcc44
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/win-64/proj-9.1.0-h3863b3b_0.tar.bz2#40201019efe10a1373387506cffa8cb1
 https://conda.anaconda.org/conda-forge/win-64/protobuf-4.23.3-py310ha3d488f_0.conda#a65f902a101c1ec7bedfe48b65756379
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-modules-0.2.7-py_0.tar.bz2#ad1e886d09700b2304975335f714bd9c
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
@@ -283,112 +311,136 @@
 https://conda.anaconda.org/pytorch/win-64/pytorch-cuda-11.8-h24eeafa_5.tar.bz2#6c31007cf6837eac42629e117ef1d947
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2#03bf410858b2cefc267316408a77c436
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.32-py310h8d17308_0.conda#c13c515dcc8f25ea5407630e172ed83c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
-https://conda.anaconda.org/conda-forge/win-64/sip-6.7.9-py310h00ffb61_0.conda#a249b5eefc4c36146ade59e2b237b7fd
+https://conda.anaconda.org/conda-forge/win-64/sip-6.7.11-py310h00ffb61_0.conda#adde89badfc7fd6e238aa4e5c2381e91
 https://conda.anaconda.org/conda-forge/noarch/sympy-1.12-pyh04b8f61_3.conda#6af285473a6a49ea8068e0b5b28ed7de
 https://conda.anaconda.org/conda-forge/win-64/tbb-2021.9.0-h91493d7_0.conda#6aa3f1becefeaa00a4d2a79b2a478aee
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
 https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/werkzeug-2.3.6-pyhd8ed1ab_0.conda#55fbbb3e67185820ee2007395bfe0073
 https://conda.anaconda.org/conda-forge/win-64/xorg-libsm-1.2.3-hcd874cb_1000.tar.bz2#76a765e735668a9922da3d58e746a7a6
 https://conda.anaconda.org/conda-forge/win-64/yarl-1.9.2-py310h8d17308_0.conda#0dfd2f264553d751449a0585d030adf7
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py310h8d17308_3.tar.bz2#3f6daa76891876a933722b5c9ee7dcaa
+https://conda.anaconda.org/conda-forge/noarch/arrow-1.2.3-pyhd8ed1ab_0.tar.bz2#fd1967c76eda3a3dd9e8e6cb7a15a028
 https://conda.anaconda.org/conda-forge/win-64/astroid-2.15.6-py310h5588dad_0.conda#a1e30c9be3eb810b8efdd581449983cc
 https://conda.anaconda.org/conda-forge/noarch/async-timeout-4.0.2-pyhd8ed1ab_0.tar.bz2#25e79f9a1133556671becbd65a170c78
 https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py310h8d17308_1005.tar.bz2#6cb010e0fa21d7b606a13038a89ccbc2
 https://conda.anaconda.org/conda-forge/win-64/cairo-1.16.0-hd694305_1014.tar.bz2#91f08ed9ff25a969ddd06237454dae0d
+https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.2-py310h6e82f81_0.conda#507f1964c07ee129d1317e601a2bfb94
 https://conda.anaconda.org/conda-forge/win-64/ffmpeg-5.1.2-gpl_h5037a79_109.conda#57b15431095a5632832088a38b7318b7
-https://conda.anaconda.org/conda-forge/win-64/fonttools-4.41.0-py310h8d17308_0.conda#496704d1b32153ed96e60de270a3e2f4
+https://conda.anaconda.org/conda-forge/win-64/fonttools-4.42.0-py310h8d17308_0.conda#ec31ba91f0feb2bbc6dd48f620e48129
+https://conda.anaconda.org/conda-forge/noarch/fqdn-1.5.1-pyhd8ed1ab_0.tar.bz2#642d35437078749ef23a5dca2c9bb1f3
 https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2#6d8d61116031a3f5b1f32e7899785866
 https://conda.anaconda.org/conda-forge/win-64/glib-2.76.4-h12be248_0.conda#4d7ae53ee4b7e08f3fbd1d3a7efd4812
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/win-64/libitk-5.3.0-h6e1890f_0.conda#705a9011eeac84184b34f157ca927ec0
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.8.1-nompi_h8c042bf_106.tar.bz2#90515eee0f7575b5fd296b6ba8d91dae
-https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
+https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.4-pyhd8ed1ab_0.conda#6b8ab17bc8ff1ca89b3ea28ea3d566ca
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/win-64/mkl-2022.1.0-h6a75c08_874.tar.bz2#2ff89a7337a9636029b4db9466e9f8e3
 https://conda.anaconda.org/conda-forge/win-64/pillow-9.2.0-py310hd4fb230_3.tar.bz2#96a1ddd65392fb64636dd8311f862e14
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.10.0-pyhd8ed1ab_0.conda#0809187ef9b89a3d94a5c24d13936236
+https://conda.anaconda.org/conda-forge/noarch/poetry-core-1.6.1-pyhd8ed1ab_0.conda#a6d1f61527c27fcc0165a6701a46b9f4
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.11.0-py310h00ffb61_3.conda#a4c757150f616bae079bc08cea956138
+https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.4.0-py310h87d50f1_0.conda#1b2ffeb2d0c1f05218979ef85ccfa008
+https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.12.2-py310h00ffb61_4.conda#571fa855e337706187fd018e1ba49fcd
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
 https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.19-py310h8d17308_0.conda#4cfc2aca9d88ef166474d84cb9c51451
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/win-64/tbb-devel-2021.9.0-h91493d7_0.conda#ece1b712d5d6c96f916ec0f11e52b391
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/win-64/xorg-libx11-1.8.4-hcd874cb_0.conda#ebdb02b455647e13fa697da89d9bdf84
+https://conda.anaconda.org/conda-forge/win-64/zstandard-0.19.0-py310h0009e47_2.conda#82b3f10667553f6d262593a16851fbba
 https://conda.anaconda.org/conda-forge/win-64/aiohttp-3.8.5-py310h8d17308_0.conda#cb4d6c6556ca7dfad7f75b1b371ecb30
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
-https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_1.conda#42f53931331420f6b748f91ef356a558
+https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.9.0-pyhd8ed1ab_0.conda#38253361efb303deead3eab39ae9269b
+https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.5-hb4038d2_0.conda#489c30d6f35bdbea9a79c369cde19c6f
 https://conda.anaconda.org/conda-forge/win-64/harfbuzz-6.0.0-he256f1b_0.conda#15422d4ff786ed835173cfb8e6735679
+https://conda.anaconda.org/conda-forge/noarch/isoduration-20.11.0-pyhd8ed1ab_0.tar.bz2#4cb68948e0b8429534380243d063a27a
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py310h5588dad_0.conda#39614170bdabdaa7531cb1dc2846c37c
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/win-64/keyring-23.13.1-py310h5588dad_0.conda#30210ff7bf71d7e193251e21d87f2838
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_mkl.conda#9e42ac6b256b96bfaa19f829c25940e8
 https://conda.anaconda.org/conda-forge/win-64/mkl-devel-2022.1.0-h57928b3_875.tar.bz2#6319a06307af296c1dfae93687c283b2
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
+https://conda.anaconda.org/conda-forge/noarch/poetry-plugin-export-1.4.0-pyhd8ed1ab_0.conda#00893c7ea4f9f7620706e0aa94c01b6e
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/win-64/pybtex-docutils-1.0.2-py310h5588dad_2.tar.bz2#a69da1e6eb6ce9a7794d379a54e06990
+https://conda.anaconda.org/conda-forge/noarch/pydantic-2.1.1-pyhd8ed1ab_0.conda#7964a624018707909044b509f58b937a
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/win-64/simpleitk-2.2.1-py310hcf936e6_1.conda#39ff6e62452d8ccdbc0bdfe8566932f5
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.2-pyhd8ed1ab_0.conda#a218f3be8ab6185a475c8168a86e18ae
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxext-1.3.4-hcd874cb_2.conda#2aa695ac3c56193fd8d526e3b511e021
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxt-1.3.0-hcd874cb_0.conda#f7db1a67cd97a9bd0f59ee6997a77159
+https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.2.0-pyh38be061_0.conda#8a3ae7f6318376aa08ea753367bb7dd6
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
-https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_1.conda#ce797dd3d60901f6260e84e84674c829
+https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.5-h001b923_0.conda#56cea78b747eaf6e8ec60cfbbf0416ff
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-with-format-nongpl-4.17.3-pyhd8ed1ab_0.conda#7a709748e93f0b2c33d6b5b676b6d9d0
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_mkl.conda#768b2c3be666ecf9e62f939ea919f819
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-17_win64_mkl.conda#278121fe8f0d65d496998aa290f36322
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.2-pyhd8ed1ab_0.conda#61ba076de6530d9301a0053b02f093d2
 https://conda.anaconda.org/conda-forge/win-64/pango-1.50.14-hdffb7b3_0.conda#a613f324e0f213238baec720d5c4ed00
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxpm-3.5.16-hcd874cb_0.conda#e74445e2a4ad70fc358ae2bf87c20f41
 https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
+https://conda.anaconda.org/conda-forge/win-64/dulwich-0.21.5-py310h8d17308_0.conda#9c3adc3bcee36c492dcaaa682741d0da
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.7.0-pyhd8ed1ab_0.conda#279fed93be42722de98e998ec80be8a1
 https://conda.anaconda.org/conda-forge/win-64/libgd-2.3.3-h891f43f_3.tar.bz2#0d66b24e1ba733a75df08e0af6f20be1
 https://conda.anaconda.org/conda-forge/win-64/liblapacke-3.9.0-17_win64_mkl.conda#6c98bb1c41479063f089459dcdedcecb
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.1-py310hd02465a_0.conda#922f75b8698c5b9909bf03c658898117
+https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.2-py310hd02465a_0.conda#faeadcd33c1207e7bedd0ee8621ba25a
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-h720456b_6.conda#3047b05190091b66cf60017b8968a562
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/win-64/blas-devel-3.9.0-17_win64_mkl.conda#bfcbcc96906ca944d944eb4ae340371a
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.14-pyhd8ed1ab_0.conda#db23395890ef31be3c2320fb41b665b0
+https://conda.anaconda.org/conda-forge/win-64/conda-23.7.2-py310h5588dad_0.conda#8d47d845a64022a75bd84f815ca66423
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.1.0-py310h232114e_0.conda#4079a644cfc3b1fbd72571dc0a87ea33
+https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda#5583192796d1ebcf39b1e3e0958aa259
 https://conda.anaconda.org/conda-forge/win-64/graphviz-7.0.6-h51cb2cd_0.conda#136eb298a1c96b07f935dd0525fbd11c
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda#b71d6766fc67ea676f75d121965da056
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.1.0-pyhd8ed1ab_0.conda#6fe1e9c8e93261e978998c0e90e36275
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.3-pyhd8ed1ab_0.conda#063c1fda5480050b8d989478c97a4c55
 https://conda.anaconda.org/conda-forge/win-64/nibabel-5.1.0-py310h5588dad_2.conda#9d814866ce7bef15844c53bf669a77d7
 https://conda.anaconda.org/conda-forge/win-64/pandas-1.5.3-py310h1c4a608_1.conda#3e3b61b47b88cf649025e67223bee77f
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
-https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.7-py310h1fd54f2_3.conda#4012c5ed74c63b82c344e38cf3e68a26
+https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.9-py310h1fd54f2_4.conda#bf76044f5e0ac24513f386ea728862e6
+https://conda.anaconda.org/conda-forge/win-64/rapidfuzz-2.15.1-py310h00ffb61_0.conda#7e623c5592d080ea8211f94e3755ee76
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
+https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/win-64/vtk-9.2.5-qt_py310h2fd250f_200.conda#fccf10ecfe3ea51109abdd5354071823
 https://conda.anaconda.org/conda-forge/win-64/blas-2.117-mkl.conda#a6b489be6ddbc3259df7cc8a440b8950
 https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.14-pyhd8ed1ab_0.conda#43ed0c094b39bb352382db8105ab0b94
+https://conda.anaconda.org/conda-forge/noarch/cleo-2.0.1-pyhd8ed1ab_0.conda#f1c5f2af6676cbe9206e191d1e70f661
+https://conda.anaconda.org/conda-forge/noarch/conda-devenv-2.3.0-pyhd8ed1ab_0.tar.bz2#9b175e69c1c601d01ab5edccf822363c
 https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.7.2-py310h51140c5_0.conda#f485fd7d59c2719f79aa4323caa5f1e3
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.3-pyhd8ed1ab_0.conda#f44109e52a40b8149156f5ddd9c11b26
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.10.1-py310h578b7cb_3.conda#d44c1bad75bb3e4d40066b3d3dd718ed
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.3.0-pyhd8ed1ab_0.tar.bz2#83d1a712e6d2bab6b298b1d2f42ad355
 https://conda.anaconda.org/conda-forge/noarch/sphinx-external-toc-0.3.1-pyhd8ed1ab_0.conda#561bdf7b598d38e2962c46557bd1da12
@@ -399,23 +451,25 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0.tar.bz2#382738101934261ea7931d1460e64868
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-dotnetdomain-0.4-py_0.tar.bz2#fb61a7369f505b4bb98e1530c3e09f9f
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-golangdomain-0.2.0.dev0-py_0.tar.bz2#d1a73c192888d08cedec232602c22f32
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jquery-4.1-pyhd8ed1ab_0.conda#914897066d5873acfb13e75705276ad1
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.7.2-py310h5588dad_0.conda#5059435ea4238f449ace9c04387433bd
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.3-pyhd8ed1ab_0.conda#f53d92ecd7d8563b006107f6a33e55c6
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/poetry-1.5.1-win_pyhd8ed1ab_0.conda#278a253d341cdb93af47a14c794f6c02
 https://conda.anaconda.org/pytorch/win-64/pytorch-2.0.1-py3.10_cuda11.8_cudnn8_0.tar.bz2#798f578b07f4a959d587c98dc922d051
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-5.4.3-pyhd8ed1ab_0.conda#3777f933bec5113d5a292de10b03d0f6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autoapi-2.1.0-pyhd8ed1ab_0.conda#6cb2b182390f837ce98737e92b9461f7
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
 https://conda.anaconda.org/conda-forge/noarch/sphinx_rtd_theme-1.2.2-pyha770c72_0.conda#5ef6aaf2cfb3b656cdadb431daed6a9f
 https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda#321151b2405f11ec6681a9a6f30822b4
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.0.5-pyhd8ed1ab_1.tar.bz2#1c31d380288fc1599fb5f4c76c8c828c
 https://conda.anaconda.org/conda-forge/noarch/jupyter-book-0.15.1-pyhd8ed1ab_0.conda#f10d556d3b3dc0aeae6aee37c412ea60
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/torchinfo-1.8.0-pyhd8ed1ab_0.conda#fba98fc95a945e2a6b93a77b39dd52dc
 https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda#480cb2b6d502003e937d9e4326bc398f
 https://conda.anaconda.org/pytorch/win-64/torchvision-0.15.2-py310_cu118.tar.bz2#140ec95434b375beaa3b12159b9f0caf
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda#ce9d626b181c6f8cceb5047f6a819f7d
+https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.6-pyhd8ed1ab_0.conda#5325b6adf171d4d69968100af806994e
 https://conda.anaconda.org/conda-forge/win-64/jupyter-1.0.0-py310h5588dad_8.conda#5fe66001841554f8b30f7db775d9ba81
```

### Comparing `hf-deepali-0.4.2/conda/environment.win-64.yml` & `hf-deepali-0.4.3/conda/environment.win-64.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: 6255d416b6866feefaa84cbaf27b3a7608f8bb60e8d5e51ca00574e0f3970f20
+# input_hash: f9e524a368611b4591c0b79cc851d7fd034bcb935240ad118e3fe4c7b27edeb4
 
 channels:
   - conda-forge
   - pytorch
   - nvidia
   - nodefaults
 dependencies:
-  - ca-certificates=2023.5.7=h56e8100_0
+  - ca-certificates=2023.7.22=h56e8100_0
   - cuda-cccl-impl=2.0.1=h57928b3_0
   - cuda-cudart=11.8.89=0
   - cuda-cupti=11.8.87=0
   - cuda-nvrtc=11.8.89=0
   - cuda-nvtx=11.8.86=0
-  - cuda-profiler-api=12.2.53=0
+  - cuda-profiler-api=12.2.128=0
   - cuda-version=12.0=hffde075_2
   - font-ttf-dejavu-sans-mono=2.37=hab24e00_0
   - font-ttf-inconsolata=3.000=h77eed37_0
   - font-ttf-source-code-pro=2.038=h77eed37_0
   - font-ttf-ubuntu=0.83=hab24e00_0
-  - intel-openmp=2023.1.0=h57928b3_46319
+  - intel-openmp=2023.2.0=h57928b3_49496
   - libcublas=11.11.3.6=0
   - libcufft=10.9.0.58=0
   - libcusolver=11.4.1.48=0
   - libcusparse=11.7.5.86=0
   - libexpat=2.5.0=h63175ca_1
   - libnpp=11.8.0.86=0
   - libnvjpeg=11.9.0.86=0
@@ -58,15 +58,15 @@
   - vs2015_runtime=14.36.32532=h05e6639_17
   - aom=3.5.0=h63175ca_0
   - bzip2=1.0.8=h8ffe710_4
   - c-ares=1.19.1=hcfcfb64_0
   - cuda-cudart-dev=11.8.89=0
   - dav1d=1.2.0=hcfcfb64_0
   - double-conversion=3.2.0=h63175ca_1
-  - eigen=3.4.1=h91493d7_0
+  - eigen=3.4.0=h91493d7_0
   - fftw=3.3.10=nompi_h38027f0_108
   - fribidi=1.0.10=h8d14728_0
   - getopt-win32=0.1=h8ffe710_0
   - glew=2.1.0=h39d44d4_2
   - graphite2=1.3.13=1000
   - icu=70.1=h0e60522_0
   - jpeg=9e=hcfcfb64_3
@@ -79,21 +79,21 @@
   - libdeflate=1.14=hcfcfb64_0
   - libffi=3.4.2=h8ffe710_5
   - libiconv=1.17=h8ffe710_0
   - libogg=1.3.4=h8ffe710_1
   - libopus=1.3.1=h8ffe710_1
   - libsodium=1.0.18=h8d14728_1
   - libsqlite=3.42.0=hcfcfb64_0
-  - libuv=1.44.2=h8ffe710_0
+  - libuv=1.44.2=hcfcfb64_1
   - libwebp-base=1.3.1=hcfcfb64_0
   - libzlib=1.2.13=hcfcfb64_5
   - lz4-c=1.9.4=hcfcfb64_0
   - m2w64-gcc-libgfortran=5.3.0=6
   - openh264=2.3.1=h63175ca_2
-  - openssl=3.1.1=hcfcfb64_1
+  - openssl=3.1.2=hcfcfb64_0
   - pixman=0.40.0=h8ffe710_0
   - pthreads-win32=2.9.1=hfa6e2cd_3
   - pugixml=1.11.4=h63175ca_1
   - re2=2023.03.02=hd4eee63_0
   - svt-av1=1.4.1=h63175ca_0
   - tk=8.6.12=h8ffe710_0
   - x264=1!164.3095=h8ffe710_2
@@ -101,15 +101,15 @@
   - xz=5.2.6=h8d14728_0
   - yaml=0.2.5=h8ffe710_2
   - cuda-libraries=11.8.0=0
   - gettext=0.21.1=h5728263_0
   - krb5=1.20.1=heb0366b_0
   - libbrotlidec=1.0.9=hcfcfb64_9
   - libbrotlienc=1.0.9=hcfcfb64_9
-  - libclang13=15.0.7=default_h77d9078_2
+  - libclang13=15.0.7=default_h77d9078_3
   - libcurand-dev=10.3.1.50=h63175ca_0
   - libpng=1.6.39=h19919ed_0
   - libprotobuf=4.23.3=h1975477_0
   - libssh2=1.11.0=h7dfc565_0
   - libtheora=1.1.1=h8d14728_1005
   - libvorbis=1.3.7=h0e60522_0
   - libwebp=1.3.1=hcfcfb64_0
@@ -120,30 +120,35 @@
   - python=3.10.12=h4de0772_0_cpython
   - sqlite=3.42.0=hcfcfb64_0
   - zeromq=4.3.4=h0e60522_1
   - zlib=1.2.13=hcfcfb64_5
   - zstd=1.5.2=h12be248_7
   - absl-py=1.4.0=pyhd8ed1ab_0
   - alabaster=0.7.13=pyhd8ed1ab_0
+  - appdirs=1.4.4=pyh9f0ad1d_0
   - attrs=21.4.0=pyhd8ed1ab_0
   - backcall=0.2.0=pyh9f0ad1d_0
   - backports=1.0=pyhd8ed1ab_3
   - blinker=1.6.2=pyhd8ed1ab_0
+  - boltons=23.0.0=pyhd8ed1ab_0
   - brotli-bin=1.0.9=hcfcfb64_9
+  - cached_property=1.5.2=pyha770c72_1
   - cachetools=5.3.1=pyhd8ed1ab_0
-  - certifi=2023.5.7=pyhd8ed1ab_0
+  - certifi=2023.7.22=pyhd8ed1ab_0
   - charset-normalizer=3.2.0=pyhd8ed1ab_0
   - colorama=0.4.6=pyhd8ed1ab_0
+  - crashtest=0.4.1=pyhd8ed1ab_0
   - cuda-libraries-dev=11.8.0=0
   - cuda-runtime=11.8.0=0
   - cycler=0.11.0=pyhd8ed1ab_0
   - dataclasses=0.8=pyhc8e2a94_3
-  - debugpy=1.6.7=py310h00ffb61_0
+  - debugpy=1.6.8=py310h00ffb61_0
   - decorator=5.1.1=pyhd8ed1ab_0
   - defusedxml=0.7.1=pyhd8ed1ab_0
+  - distlib=0.3.7=pyhd8ed1ab_0
   - docutils=0.17.1=py310h5588dad_3
   - entrypoints=0.4=pyhd8ed1ab_0
   - exceptiongroup=1.1.2=pyhd8ed1ab_0
   - executing=1.2.0=pyhd8ed1ab_0
   - filelock=3.12.2=pyhd8ed1ab_0
   - flit-core=3.9.0=pyhd8ed1ab_0
   - freetype=2.12.1=h546665d_1
@@ -153,88 +158,105 @@
   - greenlet=2.0.2=py310h00ffb61_1
   - hdf4=4.2.15=h1b1b6ef_5
   - idna=3.4=pyhd8ed1ab_0
   - imagesize=1.4.1=pyhd8ed1ab_0
   - iniconfig=2.0.0=pyhd8ed1ab_0
   - ipython_genutils=0.2.0=py_1
   - jmespath=1.0.1=pyhd8ed1ab_0
+  - jsonpointer=2.0=py_0
   - jupyterlab_widgets=3.0.8=pyhd8ed1ab_0
   - kiwisolver=1.4.4=py310h232114e_1
   - lazy-object-proxy=1.9.0=py310h8d17308_0
-  - libclang=15.0.7=default_h77d9078_2
+  - libclang=15.0.7=default_h77d9078_3
   - libcurl=8.1.2=h68f0423_0
   - libglib=2.76.4=he8f3873_0
   - libgrpc=1.56.2=hea2d5f7_0
   - libhwloc=2.9.1=h51c2c0f_0
   - libtiff=4.4.0=hc4f729c_5
+  - lockfile=0.12.2=py_1
   - markupsafe=2.1.3=py310h8d17308_0
   - mccabe=0.7.0=pyhd8ed1ab_0
   - mdurl=0.1.0=pyhd8ed1ab_0
+  - menuinst=1.4.19=py310h5588dad_1
   - mistune=3.0.0=pyhd8ed1ab_0
+  - more-itertools=10.1.0=pyhd8ed1ab_0
   - mpmath=1.3.0=pyhd8ed1ab_0
+  - msgpack-python=1.0.5=py310h232114e_0
   - multidict=6.0.4=py310h8d17308_0
   - munkres=1.1.4=pyh9f0ad1d_0
   - mypy_extensions=1.0.0=pyha770c72_0
   - nest-asyncio=1.5.6=pyhd8ed1ab_0
   - networkx=3.1=pyhd8ed1ab_0
   - packaging=23.1=pyhd8ed1ab_0
   - pandocfilters=1.5.0=pyhd8ed1ab_0
   - parso=0.8.3=pyhd8ed1ab_0
-  - pathspec=0.11.1=pyhd8ed1ab_0
+  - pathspec=0.11.2=pyhd8ed1ab_0
   - pickleshare=0.7.5=py_1003
+  - pkginfo=1.9.6=pyhd8ed1ab_0
   - pkgutil-resolve-name=1.3.10=pyhd8ed1ab_0
   - pluggy=1.2.0=pyhd8ed1ab_0
   - ply=3.11=py_1
   - prometheus_client=0.17.1=pyhd8ed1ab_0
   - psutil=5.9.5=py310h8d17308_0
   - pthread-stubs=0.4=hcd874cb_1001
+  - ptyprocess=0.7.0=pyhd3deb0d_0
   - pure_eval=0.2.2=pyhd8ed1ab_0
   - pyasn1=0.4.8=py_0
   - pycodestyle=2.10.0=pyhd8ed1ab_0
+  - pycosat=0.6.4=py310h8d17308_1
   - pycparser=2.21=pyhd8ed1ab_0
   - pyflakes=3.0.1=pyhd8ed1ab_0
   - pygments=2.15.1=pyhd8ed1ab_0
   - pyjwt=2.8.0=pyhd8ed1ab_0
   - pyparsing=3.0.9=pyhd8ed1ab_0
   - pyrsistent=0.19.3=py310h8d17308_0
-  - python-fastjsonschema=2.17.1=pyhd8ed1ab_0
+  - python-fastjsonschema=2.18.0=pyhd8ed1ab_0
+  - python-installer=0.7.0=pyhd8ed1ab_0
   - python-json-logger=2.0.7=pyhd8ed1ab_0
   - pytz=2023.3=pyhd8ed1ab_0
   - pywin32=304=py310h00ffb61_2
+  - pywin32-ctypes=0.2.2=py310h5588dad_0
   - pywinpty=2.0.11=py310h00ffb61_0
   - pyyaml=6.0=py310h8d17308_5
   - pyzmq=25.1.0=py310hcd737a0_0
   - rfc3986-validator=0.1.1=pyh9f0ad1d_0
   - ruamel.yaml.clib=0.2.7=py310h8d17308_1
   - setuptools=67.7.2=pyhd8ed1ab_0
+  - shellingham=1.5.1=pyhd8ed1ab_0
   - six=1.16.0=pyh6c4a22f_0
   - sniffio=1.3.0=pyhd8ed1ab_0
   - snowballstemmer=2.2.0=pyhd8ed1ab_0
   - soupsieve=2.3.2.post1=pyhd8ed1ab_0
   - sphinxcontrib-applehelp=1.0.4=pyhd8ed1ab_0
   - sphinxcontrib-devhelp=1.0.2=py_0
   - sphinxcontrib-htmlhelp=2.0.1=pyhd8ed1ab_0
   - sphinxcontrib-jsmath=1.0.1=py_0
   - sphinxcontrib-qthelp=1.0.3=py_0
   - sphinxcontrib-serializinghtml=1.1.5=pyhd8ed1ab_2
   - tabulate=0.9.0=pyhd8ed1ab_1
   - tensorboard-data-server=0.7.0=py310h5588dad_0
   - toml=0.10.2=pyhd8ed1ab_0
   - tomli=2.0.1=pyhd8ed1ab_0
+  - tomlkit=0.12.1=pyha770c72_0
+  - toolz=0.12.0=pyhd8ed1ab_0
   - tornado=6.3.2=py310h8d17308_0
   - traitlets=5.9.0=pyhd8ed1ab_0
+  - trove-classifiers=2023.7.6=pyhd8ed1ab_0
   - typed-ast=1.5.5=py310h8d17308_0
+  - typing=3.10.0.0=pyhd8ed1ab_0
   - typing_extensions=4.7.1=pyha770c72_0
   - typing_utils=0.1.0=pyhd8ed1ab_0
   - uc-micro-py=1.0.1=pyhd8ed1ab_0
   - unicodedata2=15.0.0=py310h8d17308_0
   - unidecode=1.3.6=pyhd8ed1ab_0
+  - uri-template=1.3.0=pyhd8ed1ab_0
+  - webcolors=1.13=pyhd8ed1ab_0
   - webencodings=0.5.1=py_1
   - websocket-client=1.6.1=pyhd8ed1ab_0
-  - wheel=0.40.0=pyhd8ed1ab_1
+  - wheel=0.41.0=pyhd8ed1ab_0
   - widgetsnbextension=4.0.8=pyhd8ed1ab_0
   - win32_setctime=1.1.0=pyhd8ed1ab_0
   - win_inet_pton=1.1.0=pyhd8ed1ab_6
   - wrapt=1.15.0=py310h8d17308_0
   - xorg-kbproto=1.0.7=hcd874cb_1002
   - xorg-libice=1.0.10=hcd874cb_0
   - xorg-libxau=1.0.11=hcd874cb_0
@@ -243,45 +265,51 @@
   - xorg-xproto=7.0.31=hcd874cb_1007
   - zipp=3.16.2=pyhd8ed1ab_0
   - accessible-pygments=0.0.4=pyhd8ed1ab_0
   - aiosignal=1.3.1=pyhd8ed1ab_0
   - anyio=3.7.1=pyhd8ed1ab_0
   - asttokens=2.2.1=pyhd8ed1ab_0
   - babel=2.12.1=pyhd8ed1ab_1
+  - backports.cached-property=1.0.2=pyhd8ed1ab_0
   - backports.functools_lru_cache=1.6.5=pyhd8ed1ab_0
   - beautifulsoup4=4.12.2=pyha770c72_0
   - bleach=6.0.0=pyhd8ed1ab_0
   - brotli=1.0.9=hcfcfb64_9
+  - cached-property=1.5.2=hd8ed1ab_1
   - cffi=1.15.1=py310h628cb3f_3
   - click=8.1.6=win_pyh7428d3b_0
-  - comm=0.1.3=pyhd8ed1ab_0
+  - comm=0.1.4=pyhd8ed1ab_0
   - curl=8.1.2=h68f0423_0
   - dacite=1.8.0=pyhd8ed1ab_0
   - deprecation=2.1.0=pyh9f0ad1d_0
   - flake8=6.0.0=pyhd8ed1ab_0
   - fontconfig=2.14.2=hbde0cde_0
   - glib-tools=2.76.4=h12be248_0
   - grpcio=1.56.2=py310hb84602e_0
   - gts=0.7.6=h6b5321d_4
   - hdf5=1.12.2=nompi_h57737ce_101
+  - html5lib=1.1=pyh9f0ad1d_0
   - importlib-metadata=6.8.0=pyha770c72_0
   - importlib_resources=6.0.0=pyhd8ed1ab_1
-  - jedi=0.18.2=pyhd8ed1ab_0
+  - jaraco.classes=3.3.0=pyhd8ed1ab_0
+  - jedi=0.19.0=pyhd8ed1ab_0
   - jinja2=3.1.2=pyhd8ed1ab_1
+  - jsonpatch=1.32=pyhd8ed1ab_0
   - jupyterlab_pygments=0.2.2=pyhd8ed1ab_0
   - latexcodec=2.0.1=pyh9f0ad1d_0
   - lcms2=2.14=h90d422f_0
   - libxcb=1.13=hcd874cb_1004
   - lightning-utilities=0.9.0=pyhd8ed1ab_0
   - linkify-it-py=2.0.0=pyhd8ed1ab_0
   - loguru=0.7.0=py310h5588dad_0
   - markdown-it-py=2.2.0=pyhd8ed1ab_0
   - matplotlib-inline=0.1.6=pyhd8ed1ab_0
   - openjpeg=2.5.0=hc9384bd_1
   - overrides=7.3.1=pyhd8ed1ab_0
+  - pexpect=4.8.0=pyh1a96a4e_2
   - pip=23.1.2=pyhd8ed1ab_0
   - proj=9.1.0=h3863b3b_0
   - protobuf=4.23.3=py310ha3d488f_0
   - pyasn1-modules=0.2.7=py_0
   - pyproject_hooks=1.0.0=pyhd8ed1ab_0
   - pysocks=1.7.1=pyh0701188_6
   - pytest=7.3.2=pyhd8ed1ab_1
@@ -289,112 +317,136 @@
   - pytorch-cuda=11.8=h24eeafa_5
   - pyu2f=0.1.5=pyhd8ed1ab_0
   - qtpy=2.3.1=pyhd8ed1ab_0
   - rfc3339-validator=0.1.4=pyhd8ed1ab_0
   - rsa=4.9=pyhd8ed1ab_0
   - ruamel.yaml=0.17.32=py310h8d17308_0
   - send2trash=1.8.2=pyh08f2357_0
-  - sip=6.7.9=py310h00ffb61_0
+  - sip=6.7.11=py310h00ffb61_0
   - sympy=1.12=pyh04b8f61_3
   - tbb=2021.9.0=h91493d7_0
   - terminado=0.17.0=pyh08f2357_0
   - tinycss2=1.2.1=pyhd8ed1ab_0
   - tqdm=4.65.0=pyhd8ed1ab_1
   - typing-extensions=4.7.1=hd8ed1ab_0
   - werkzeug=2.3.6=pyhd8ed1ab_0
   - xorg-libsm=1.2.3=hcd874cb_1000
   - yarl=1.9.2=py310h8d17308_0
+  - annotated-types=0.5.0=pyhd8ed1ab_0
   - argon2-cffi-bindings=21.2.0=py310h8d17308_3
+  - arrow=1.2.3=pyhd8ed1ab_0
   - astroid=2.15.6=py310h5588dad_0
   - async-timeout=4.0.2=pyhd8ed1ab_0
   - brotlipy=0.7.0=py310h8d17308_1005
   - cairo=1.16.0=hd694305_1014
+  - click-default-group=1.2.2=pyhd8ed1ab_1
   - cryptography=41.0.2=py310h6e82f81_0
   - ffmpeg=5.1.2=gpl_h5037a79_109
-  - fonttools=4.41.0=py310h8d17308_0
+  - fonttools=4.42.0=py310h8d17308_0
+  - fqdn=1.5.1=pyhd8ed1ab_0
   - ghp-import=2.1.0=pyhd8ed1ab_0
   - glib=2.76.4=h12be248_0
   - importlib_metadata=6.8.0=hd8ed1ab_0
   - jsonschema=4.17.3=pyhd8ed1ab_0
   - jupyter_server_terminals=0.4.4=pyhd8ed1ab_1
   - libitk=5.3.0=h6e1890f_0
   - libnetcdf=4.8.1=nompi_h8c042bf_106
-  - markdown=3.4.3=pyhd8ed1ab_0
+  - markdown=3.4.4=pyhd8ed1ab_0
   - mdit-py-plugins=0.4.0=pyhd8ed1ab_0
   - mkl=2022.1.0=h6a75c08_874
   - pillow=9.2.0=py310hd4fb230_3
-  - platformdirs=3.9.1=pyhd8ed1ab_0
+  - platformdirs=3.10.0=pyhd8ed1ab_0
+  - poetry-core=1.6.1=pyhd8ed1ab_0
   - pybtex=0.24.0=pyhd8ed1ab_2
-  - pyqt5-sip=12.11.0=py310h00ffb61_3
+  - pydantic-core=2.4.0=py310h87d50f1_0
+  - pyqt5-sip=12.12.2=py310h00ffb61_4
   - python-build=0.10.0=pyhd8ed1ab_1
   - setuptools-scm=7.1.0=pyhd8ed1ab_0
   - sqlalchemy=2.0.19=py310h8d17308_0
   - stack_data=0.6.2=pyhd8ed1ab_0
   - tbb-devel=2021.9.0=h91493d7_0
   - wcwidth=0.2.6=pyhd8ed1ab_0
   - xorg-libx11=1.8.4=hcd874cb_0
+  - zstandard=0.19.0=py310h0009e47_2
   - aiohttp=3.8.5=py310h8d17308_0
   - argon2-cffi=21.3.0=pyhd8ed1ab_0
   - black=22.3.0=pyhd8ed1ab_0
-  - gstreamer=1.22.4=hb4038d2_1
+  - conda-package-streaming=0.9.0=pyhd8ed1ab_0
+  - gstreamer=1.22.5=hb4038d2_0
   - harfbuzz=6.0.0=he256f1b_0
+  - isoduration=20.11.0=pyhd8ed1ab_0
   - jupyter_core=5.3.1=py310h5588dad_0
-  - jupyter_events=0.6.3=pyhd8ed1ab_0
+  - keyring=23.13.1=py310h5588dad_0
   - libblas=3.9.0=17_win64_mkl
   - mkl-devel=2022.1.0=h57928b3_875
   - oauthlib=3.2.2=pyhd8ed1ab_0
+  - poetry-plugin-export=1.4.0=pyhd8ed1ab_0
   - prompt-toolkit=3.0.39=pyha770c72_0
   - pybtex-docutils=1.0.2=py310h5588dad_2
+  - pydantic=2.1.1=pyhd8ed1ab_0
   - pyopenssl=23.2.0=pyhd8ed1ab_1
   - simpleitk=2.2.1=py310hcf936e6_1
+  - virtualenv=20.24.2=pyhd8ed1ab_0
   - xorg-libxext=1.3.4=hcd874cb_2
   - xorg-libxt=1.3.0=hcd874cb_0
+  - conda-package-handling=2.2.0=pyh38be061_0
   - flake8-black=0.3.6=pyhd8ed1ab_0
-  - gst-plugins-base=1.22.4=h001b923_1
+  - gst-plugins-base=1.22.5=h001b923_0
+  - jsonschema-with-format-nongpl=4.17.3=pyhd8ed1ab_0
   - jupyter_client=8.3.0=pyhd8ed1ab_0
   - libcblas=3.9.0=17_win64_mkl
   - liblapack=3.9.0=17_win64_mkl
-  - nbformat=5.9.1=pyhd8ed1ab_0
+  - nbformat=5.9.2=pyhd8ed1ab_0
   - pango=1.50.14=hdffb7b3_0
   - prompt_toolkit=3.0.39=hd8ed1ab_0
   - urllib3=1.26.15=pyhd8ed1ab_0
   - wslink=1.11.1=pyhd8ed1ab_0
   - xorg-libxpm=3.5.16=hcd874cb_0
   - botocore=1.29.165=pyhd8ed1ab_0
+  - dulwich=0.21.5=py310h8d17308_0
   - ipython=8.14.0=pyh08f2357_0
+  - jupyter_events=0.7.0=pyhd8ed1ab_0
   - libgd=2.3.3=h891f43f_3
   - liblapacke=3.9.0=17_win64_mkl
   - nbclient=0.7.4=pyhd8ed1ab_0
-  - numpy=1.25.1=py310hd02465a_0
+  - numpy=1.25.2=py310hd02465a_0
   - qt-main=5.15.8=h720456b_6
   - requests=2.31.0=pyhd8ed1ab_0
   - blas-devel=3.9.0=17_win64_mkl
+  - cachecontrol=0.12.14=pyhd8ed1ab_0
+  - conda=23.7.2=py310h5588dad_0
   - contourpy=1.1.0=py310h232114e_0
+  - ensureconda=1.4.3=pyhd8ed1ab_0
   - google-auth=2.22.0=pyh1a96a4e_0
   - graphviz=7.0.6=h51cb2cd_0
   - ipykernel=6.23.3=pyh6817e22_0
+  - ipywidgets=8.1.0=pyhd8ed1ab_0
   - jupyter-cache=0.6.1=pyhd8ed1ab_0
-  - nbconvert-core=7.7.1=pyhd8ed1ab_1
+  - nbconvert-core=7.7.3=pyhd8ed1ab_0
   - nibabel=5.1.0=py310h5588dad_2
   - pandas=1.5.3=py310h1c4a608_1
   - pooch=1.7.0=pyha770c72_3
-  - pyqt=5.15.7=py310h1fd54f2_3
+  - pyqt=5.15.9=py310h1fd54f2_4
+  - rapidfuzz=2.15.1=py310h00ffb61_0
   - requests-oauthlib=1.3.1=pyhd8ed1ab_0
+  - requests-toolbelt=1.0.0=pyhd8ed1ab_0
   - s3transfer=0.6.1=pyhd8ed1ab_0
   - sphinx=4.5.0=pyh6c4a22f_0
   - vtk=9.2.5=qt_py310h2fd250f_200
   - blas=2.117=mkl
   - boto3=1.26.165=pyhd8ed1ab_0
+  - cachecontrol-with-filecache=0.12.14=pyhd8ed1ab_0
+  - cleo=2.0.1=pyhd8ed1ab_0
+  - conda-devenv=2.3.0=pyhd8ed1ab_0
   - google-auth-oauthlib=1.0.0=pyhd8ed1ab_1
-  - ipywidgets=8.0.7=pyhd8ed1ab_0
   - jupyter_console=6.6.3=pyhd8ed1ab_0
   - jupyter_server=2.7.0=pyhd8ed1ab_0
   - matplotlib-base=3.7.2=py310h51140c5_0
   - myst-parser=0.18.1=pyhd8ed1ab_0
-  - nbconvert-pandoc=7.7.1=pyhd8ed1ab_1
+  - nbconvert-pandoc=7.7.3=pyhd8ed1ab_0
   - pydata-sphinx-theme=0.13.3=pyhd8ed1ab_0
   - qtconsole-base=5.4.3=pyha770c72_0
   - scipy=1.10.1=py310h578b7cb_3
   - sphinx-comments=0.0.3=pyh9f0ad1d_0
   - sphinx-copybutton=0.5.2=pyhd8ed1ab_0
   - sphinx-design=0.3.0=pyhd8ed1ab_0
   - sphinx-external-toc=0.3.1=pyhd8ed1ab_0
@@ -405,23 +457,25 @@
   - sphinx-togglebutton=0.3.2=pyhd8ed1ab_0
   - sphinxcontrib-bibtex=2.5.0=pyhd8ed1ab_0
   - sphinxcontrib-dotnetdomain=0.4=py_0
   - sphinxcontrib-golangdomain=0.2.0.dev0=py_0
   - sphinxcontrib-jquery=4.1=pyhd8ed1ab_0
   - matplotlib=3.7.2=py310h5588dad_0
   - myst-nb=0.17.2=pyhd8ed1ab_0
-  - nbconvert=7.7.1=pyhd8ed1ab_1
+  - nbconvert=7.7.3=pyhd8ed1ab_0
   - notebook-shim=0.2.3=pyhd8ed1ab_0
+  - poetry=1.5.1=win_pyhd8ed1ab_0
   - pytorch=2.0.1=py3.10_cuda11.8_cudnn8_0
   - qtconsole=5.4.3=pyhd8ed1ab_0
   - sphinx-autoapi=2.1.0=pyhd8ed1ab_0
   - sphinx-book-theme=1.0.1=pyhd8ed1ab_0
   - sphinx_rtd_theme=1.2.2=pyha770c72_0
   - tensorboard=2.13.0=pyhd8ed1ab_0
+  - conda-lock=1.0.5=pyhd8ed1ab_1
   - jupyter-book=0.15.1=pyhd8ed1ab_0
   - nbclassic=1.0.0=pyhb4ecaf3_1
   - torchinfo=1.8.0=pyhd8ed1ab_0
   - torchmetrics=0.11.4=pyhd8ed1ab_0
   - torchvision=0.15.2=py310_cu118
   - notebook=6.5.4=pyha770c72_0
-  - pytorch-lightning=2.0.4=pyhd8ed1ab_0
+  - pytorch-lightning=2.0.6=pyhd8ed1ab_0
   - jupyter=1.0.0=py310h5588dad_8
```

### Comparing `hf-deepali-0.4.2/docker/Dockerfile` & `hf-deepali-0.4.3/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docker/build` & `hf-deepali-0.4.3/docker/build`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docker/run` & `hf-deepali-0.4.3/docker/run`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/_citations.bib` & `hf-deepali-0.4.3/docs/_citations.bib`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/_config.yml` & `hf-deepali-0.4.3/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/_images/logo.png` & `hf-deepali-0.4.3/docs/_images/logo.png`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/_toc.yml` & `hf-deepali-0.4.3/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/basics/example-page.md` & `hf-deepali-0.4.3/docs/basics/example-page.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/basics/installation.md` & `hf-deepali-0.4.3/docs/basics/installation.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/index.md` & `hf-deepali-0.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/reference/core/flow.md` & `hf-deepali-0.4.3/docs/reference/core/flow.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/reference/core/image.md` & `hf-deepali-0.4.3/docs/reference/core/image.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/reference/data/transforms.md` & `hf-deepali-0.4.3/docs/reference/data/transforms.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/reference/spatial/common.md` & `hf-deepali-0.4.3/docs/reference/spatial/common.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/reference/spatial/composite.md` & `hf-deepali-0.4.3/docs/reference/spatial/composite.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/reference/utils/index.md` & `hf-deepali-0.4.3/docs/reference/utils/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/tutorials/example-myst-notebook.md` & `hf-deepali-0.4.3/docs/tutorials/example-myst-notebook.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/tutorials/example-notebook.ipynb` & `hf-deepali-0.4.3/docs/tutorials/example-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/docs/tutorials/pairwise-registration-intro.ipynb` & `hf-deepali-0.4.3/docs/tutorials/pairwise-registration-intro.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/README.md` & `hf-deepali-0.4.3/examples/ffd/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/engine.py` & `hf-deepali-0.4.3/examples/ffd/engine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/hooks.py` & `hf-deepali-0.4.3/examples/ffd/hooks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/losses.py` & `hf-deepali-0.4.3/examples/ffd/losses.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/optim.py` & `hf-deepali-0.4.3/examples/ffd/optim.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/pairwise.py` & `hf-deepali-0.4.3/examples/ffd/pairwise.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/params.yaml` & `hf-deepali-0.4.3/examples/ffd/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/ffd/register.py` & `hf-deepali-0.4.3/examples/ffd/register.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 r"""Example implementation of free-form deformation (FFD) algorithm."""
 
 import logging
 from pathlib import Path
 import sys
 from timeit import default_timer as timer
-from typing import Any, Dict
-
-import json
-import yaml
 
 import torch
 import torch.cuda
 from torch import Tensor
 
 from deepali.core.argparse import ArgumentParser, Args, main_func
+from deepali.core.config import read_config_dict
 from deepali.core.environ import cuda_visible_devices
 from deepali.core.grid import Grid
 from deepali.core.logging import configure_logging
-from deepali.core.pathlib import PathStr, unlink_or_mkdir
+from deepali.core.pathlib import unlink_or_mkdir
 from deepali.data import Image
 from deepali.modules import TransformImage
 
 from .pairwise import register_pairwise
 
 log = logging.getLogger()
 
@@ -99,15 +96,15 @@
             log.error("CUDA_VISIBLE_DEVICES must be set to one GPU")
             return 1
     return 0
 
 
 def func(args: Args) -> int:
     r"""Execute registration given parsed arguments."""
-    config = load_config(args.config)
+    config = read_config_dict(args.config)
     device = torch.device("cuda:0" if args.device == "cuda" else "cpu")
     start = timer()
     transform = register_pairwise(
         target={"img": args.target_img, "seg": args.target_seg},
         source={"img": args.source_img, "seg": args.source_seg},
         config=config,
         outdir=args.debug_dir,
@@ -149,19 +146,9 @@
             transform.flow()[0].write(path)
     return 0
 
 
 main = main_func(parser, func, init=init)
 
 
-def load_config(path: PathStr) -> Dict[str, Any]:
-    r"""Load registration parameters from configuration file."""
-    config_path = Path(path).absolute()
-    log.info(f"Load configuration from {config_path}")
-    config_text = config_path.read_text()
-    if config_path.suffix == ".json":
-        return json.loads(config_text)
-    return yaml.safe_load(config_text)
-
-
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `hf-deepali-0.4.2/examples/istn/models/__init__.py` & `hf-deepali-0.4.3/examples/istn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/istn/models/itn.py` & `hf-deepali-0.4.3/examples/istn/models/itn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/istn/models/stn.py` & `hf-deepali-0.4.3/examples/istn/models/stn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/istn/params.yaml` & `hf-deepali-0.4.3/examples/istn/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/examples/istn/train.py` & `hf-deepali-0.4.3/examples/istn/train.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/pyproject.toml` & `hf-deepali-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 requires-python = ">=3.9"
 dynamic = ["version"]
 
 dependencies = [
     "dacite",
     "deprecation",
     "pandas",
-    "pyyaml",
     "ruamel.yaml",
     "torch>=1.9",
     "typing-extensions",
 ]
 
 [project.optional-dependencies]
 all = [
```

### Comparing `hf-deepali-0.4.2/src/deepali/core/__init__.py` & `hf-deepali-0.4.3/src/deepali/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 from .cube import Cube
 from .grid import Grid
 from .grid import grid_points_transform
 from .grid import grid_vectors_transform
 from .grid import grid_transform_points
 from .grid import grid_transform_vectors
 
+from .pathlib import is_uri
+from .pathlib import to_uri
+from .storage import StorageObject
+
 from .typing import Array
 from .typing import Batch
 from .typing import Dataclass
 from .typing import Device
 from .typing import DeviceStr
 from .typing import DType
 from .typing import DTypeStr
@@ -82,19 +86,22 @@
     "Scalar",
     "ScalarOrTuple",
     "ScalarOrTuple1d",
     "ScalarOrTuple2d",
     "ScalarOrTuple3d",
     "Size",
     "Shape",
+    "StorageObject",
     "TensorCollection",
     "grid_points_transform",
     "grid_vectors_transform",
     "grid_transform_points",
     "grid_transform_vectors",
     "is_bool_dtype",
     "is_float_dtype",
     "is_int_dtype",
     "is_uint_dtype",
     "is_namedtuple",
     "is_path_str",
+    "is_uri",
+    "to_uri",
 )
```

### Comparing `hf-deepali-0.4.2/src/deepali/core/_kornia.py` & `hf-deepali-0.4.3/src/deepali/core/_kornia.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/affine.py` & `hf-deepali-0.4.3/src/deepali/core/affine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/argparse.py` & `hf-deepali-0.4.3/src/deepali/core/argparse.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/bspline.py` & `hf-deepali-0.4.3/src/deepali/core/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/collections.py` & `hf-deepali-0.4.3/src/deepali/core/collections.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/config.py` & `hf-deepali-0.4.3/src/deepali/core/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 r"""Auxiliary functions and classes for dealing with configuration files."""
 
 from __future__ import annotations
 
 from dataclasses import asdict, fields
-from pathlib import Path
+from io import StringIO
 from typing import Any, Dict, Mapping, Optional, Sequence, TypeVar, Type
 
 import dacite
 import json
 
 # PyYAML does not support YAML 1.2, which is required by DVC for example
 # (cf. https://github.com/iterative/dvc/issues/8466#issuecomment-1290757564)
 from ruamel.yaml import YAML
 
-from .pathlib import PathStr, abspath_template
+from .pathlib import Path, PathUri, abspath_template
+from .storage import StorageObject
 from .typing import is_path_str_field
 
 
 T = TypeVar("T", bound="DataclassConfig")
 
 
 class DataclassConfig(object):
@@ -38,52 +39,33 @@
     def from_dict(cls: Type[T], arg: Mapping[str, Any], parent: Optional[Path] = None) -> T:
         r"""Create configuration from dictionary."""
         config = cls._from_dict(arg, parent=parent)
         config._finalize(parent)
         return config
 
     @classmethod
-    def from_path(cls: Type[T], path: PathStr, section: Optional[str] = None) -> T:
+    def from_path(cls: Type[T], path: PathUri, section: Optional[str] = None) -> T:
         r"""Load configuration from file."""
-        path = Path(path).absolute()
-        if path.suffix not in (".json", ".yaml", ".yml"):
-            raise ValueError(f"{cls.__name__}.write() 'path' has unsupported suffix {path.suffix}")
-        with path.open("rt") as fp:
-            if path.suffix == ".json":
-                config = json.load(fp)
-            else:
-                config = YAML(typ="safe").load(fp)
-        if config is None:
-            config = {}
+        config = read_config_dict(path)
         if section is None:
             section = cls.section()
         if section:
             for key in section.split("."):
                 config = config.get(key, {})
         return cls.from_dict(config, parent=path.parent)
 
     @classmethod
-    def read(cls: Type[T], path: PathStr, section: Optional[str] = None) -> T:
-        r"""Load configuration from file."""
+    def read(cls: Type[T], path: PathUri, section: Optional[str] = None) -> T:
+        r"""Load configuration from JSON or YAML file."""
         return cls.from_path(path, section=section)
 
-    def write(self, path: PathStr) -> None:
-        r"""Write configuration to file."""
+    def write(self, path: PathUri) -> None:
+        r"""Save configuration to JSON or YAML file."""
         config = self.asdict()
-        path = Path(path).absolute()
-        if path.suffix not in (".json", ".yaml", ".yml"):
-            raise ValueError(
-                f"{type(self).__name__}.write() 'path' has unsupported suffix {path.suffix}"
-            )
-        path.parent.mkdir(parents=True, exist_ok=True)
-        with path.open("wt") as fp:
-            if path.suffix == ".json":
-                json.dump(config, fp)
-            else:
-                YAML(typ="safe").dump(config, fp)
+        write_config_dict(config, path)
 
     def asdict(self) -> Dict[str, Any]:
         r"""Get configuration dictionary."""
         return asdict(self)
 
     def _finalize(self: T, parent: Optional[Path] = None) -> None:
         r"""Finalize parameters after loading these from input file."""
@@ -180,7 +162,38 @@
                     if name in kwargs:
                         raise ValueError(
                             f"join_kwargs_in_sequence() 'arg' has duplicate kwarg {name}"
                         )
                     kwargs[name] = value
             arg = kwargs if start == 0 else (arg[0], kwargs)
     return arg
+
+
+def read_config_dict(path: PathUri) -> Dict[str, Any]:
+    r"""Read configuration from JSON or YAML file."""
+    with StorageObject.from_path(path) as config_object:
+        config_suffix = config_object.path.suffix
+        if config_suffix.lower() not in (".json", ".yaml", ".yml"):
+            raise ValueError(f"read_config_dict() 'path' has unsupported suffix {config_suffix}")
+        config_text = config_object.read_text()
+        if config_suffix == ".json":
+            config_dict = json.loads(config_text)
+        else:
+            config_dict = YAML(typ="safe").load(config_text)
+    if config_dict is None:
+        config_dict = {}
+    return config_dict
+
+
+def write_config_dict(config: Dict[str, Any], path: PathUri) -> None:
+    r"""Write configuration to JSON or YAML file."""
+    with StorageObject.from_path(path) as config_object:
+        config_suffix = config_object.path.suffix
+        if config_suffix.lower() not in (".json", ".yaml", ".yml"):
+            raise ValueError(f"write_config_dict() 'path' has unsupported suffix {config_suffix}")
+        if config_suffix == ".json":
+            config_text = json.dumps(config) + "\n"
+        else:
+            buffer = StringIO()
+            YAML(typ="safe").dump(config, buffer)
+            config_text = buffer.getvalue()
+        config_object.write_text(config_text)
```

### Comparing `hf-deepali-0.4.2/src/deepali/core/cube.py` & `hf-deepali-0.4.3/src/deepali/core/cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/enum.py` & `hf-deepali-0.4.3/src/deepali/core/enum.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/environ.py` & `hf-deepali-0.4.3/src/deepali/core/environ.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/flow.py` & `hf-deepali-0.4.3/src/deepali/core/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/functional.py` & `hf-deepali-0.4.3/src/deepali/core/functional.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/grid.py` & `hf-deepali-0.4.3/src/deepali/core/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/image.py` & `hf-deepali-0.4.3/src/deepali/core/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/itertools.py` & `hf-deepali-0.4.3/src/deepali/core/itertools.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/kernels.py` & `hf-deepali-0.4.3/src/deepali/core/kernels.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/linalg.py` & `hf-deepali-0.4.3/src/deepali/core/linalg.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/math.py` & `hf-deepali-0.4.3/src/deepali/core/math.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/nnutils.py` & `hf-deepali-0.4.3/src/deepali/core/nnutils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/pathlib.py` & `hf-deepali-0.4.3/src/deepali/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/pointset.py` & `hf-deepali-0.4.3/src/deepali/core/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/psutil.py` & `hf-deepali-0.4.3/src/deepali/core/psutil.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/random.py` & `hf-deepali-0.4.3/src/deepali/core/random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/tempfile.py` & `hf-deepali-0.4.3/src/deepali/core/tempfile.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/tensor.py` & `hf-deepali-0.4.3/src/deepali/core/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/core/typing.py` & `hf-deepali-0.4.3/src/deepali/core/typing.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/__init__.py` & `hf-deepali-0.4.3/src/deepali/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/collate.py` & `hf-deepali-0.4.3/src/deepali/data/collate.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/dataset.py` & `hf-deepali-0.4.3/src/deepali/data/dataset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/flow.py` & `hf-deepali-0.4.3/src/deepali/data/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/image.py` & `hf-deepali-0.4.3/src/deepali/data/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/partition.py` & `hf-deepali-0.4.3/src/deepali/data/partition.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/prepare.py` & `hf-deepali-0.4.3/src/deepali/data/prepare.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/sample.py` & `hf-deepali-0.4.3/src/deepali/data/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/sampler.py` & `hf-deepali-0.4.3/src/deepali/data/sampler.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/tensor.py` & `hf-deepali-0.4.3/src/deepali/data/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/transforms/__init__.py` & `hf-deepali-0.4.3/src/deepali/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/transforms/image.py` & `hf-deepali-0.4.3/src/deepali/data/transforms/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/data/transforms/item.py` & `hf-deepali-0.4.3/src/deepali/data/transforms/item.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/losses/__init__.py` & `hf-deepali-0.4.3/src/deepali/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/losses/base.py` & `hf-deepali-0.4.3/src/deepali/losses/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/losses/flow.py` & `hf-deepali-0.4.3/src/deepali/losses/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/losses/functional.py` & `hf-deepali-0.4.3/src/deepali/losses/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
         num_bins: Number of bin edges to discretize the density estimation.
         num_samples: Number of voxels in the image domain randomly sampled to compute the loss,
             ignored if `sample_ratio` is also set.
         sample_ratio: Ratio of voxels in the image domain randomly sampled to compute the loss.
         normalized: Calculate Normalized Mutual Information instead of Mutual Information if True.
 
     Returns:
-        Negative mutual information. If ``normalized=True``, 2 is added such that the loss value is in [0, 1].
+        Negative mutual information. If ``normalized=True``, 2 is added such that the loss value is in [0, 2].
 
     """
 
     if target.ndim < 3:
         raise ValueError("mi_loss() 'target' must be tensor of shape (N, C, ..., X)")
     if input.shape != target.shape:
         raise ValueError("ssd_loss() 'input' must have same shape as 'target'")
```

### Comparing `hf-deepali-0.4.2/src/deepali/losses/image.py` & `hf-deepali-0.4.3/src/deepali/losses/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/losses/params.py` & `hf-deepali-0.4.3/src/deepali/losses/params.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/losses/pointset.py` & `hf-deepali-0.4.3/src/deepali/losses/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/__init__.py` & `hf-deepali-0.4.3/src/deepali/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/basic.py` & `hf-deepali-0.4.3/src/deepali/modules/basic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/flow.py` & `hf-deepali-0.4.3/src/deepali/modules/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/image.py` & `hf-deepali-0.4.3/src/deepali/modules/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/lambd.py` & `hf-deepali-0.4.3/src/deepali/modules/lambd.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/mixins.py` & `hf-deepali-0.4.3/src/deepali/modules/mixins.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/output.py` & `hf-deepali-0.4.3/src/deepali/modules/output.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/sample.py` & `hf-deepali-0.4.3/src/deepali/modules/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/modules/utilities.py` & `hf-deepali-0.4.3/src/deepali/modules/utilities.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/__init__.py` & `hf-deepali-0.4.3/src/deepali/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/blocks/residual.py` & `hf-deepali-0.4.3/src/deepali/networks/blocks/residual.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/blocks/skip.py` & `hf-deepali-0.4.3/src/deepali/networks/blocks/skip.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/__init__.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/acti.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/acti.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/conv.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/conv.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/join.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/join.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/linear.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/norm.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/norm.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/pool.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/pool.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/layers/upsample.py` & `hf-deepali-0.4.3/src/deepali/networks/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/resnet.py` & `hf-deepali-0.4.3/src/deepali/networks/resnet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/unet.py` & `hf-deepali-0.4.3/src/deepali/networks/unet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/networks/utils.py` & `hf-deepali-0.4.3/src/deepali/networks/utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/__init__.py` & `hf-deepali-0.4.3/src/deepali/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/base.py` & `hf-deepali-0.4.3/src/deepali/spatial/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/bspline.py` & `hf-deepali-0.4.3/src/deepali/spatial/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/composite.py` & `hf-deepali-0.4.3/src/deepali/spatial/composite.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/generic.py` & `hf-deepali-0.4.3/src/deepali/spatial/generic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/linear.py` & `hf-deepali-0.4.3/src/deepali/spatial/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,26 @@
         if self.has_parameters():
             params = params.div(math.pi).atanh()
             if params.isnan().any():
                 raise ValueError("EulerRotation.angles() 'arg' must be in range [-pi, pi]")
         self.data_(params)
         return self
 
+    def matrix_(self: EulerRotation, arg: Tensor) -> EulerRotation:
+        r"""Set rotation angles from rotation matrix."""
+        if not isinstance(arg, Tensor):
+            raise TypeError("EulerRotation.matrix() 'arg' must be tensor")
+        if arg.ndim != 3:
+            raise ValueError("EulerRotation.matrix() 'arg' must be 3-dimensional tensor")
+        shape = (arg.shape[0], 3, 3)
+        if arg.shape != shape:
+            raise ValueError(f"Rotation matrix must have shape {shape!r}")
+        angles = U.euler_rotation_angles(arg, order=self.order)
+        return self.angles_(angles)
+
     def tensor(self: EulerRotation) -> Tensor:
         r"""Get tensor representation of this transformation
 
         Returns:
             Batch of homogeneous transformation matrices as tensor of shape ``(N, D, D)``.
 
         """
```

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/nonrigid.py` & `hf-deepali-0.4.3/src/deepali/spatial/nonrigid.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         if params is None:
             raise AssertionError(f"{type(self).__name__}.data() 'params' must be set first")
         grid = self.grid()
         if not callable(params):
             grid = self.grid().resize(self.data_shape[:1:-1])
         flow = flow.to(self.device)
         flow = flow.sample(grid)
-        flow = flow.axes(Axes.from_grid(grid))
+        flow = flow.axes(grid.axes())
         if callable(params):
             self._fit(flow, **kwargs)
         else:
             self.data_(flow.tensor())
         return self
 
     def update(self) -> DisplacementFieldTransform:
```

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/parametric.py` & `hf-deepali-0.4.3/src/deepali/spatial/parametric.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/spatial/transformer.py` & `hf-deepali-0.4.3/src/deepali/spatial/transformer.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/aws/s3/client.py` & `hf-deepali-0.4.3/src/deepali/utils/aws/s3/client.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/aws/s3/config.py` & `hf-deepali-0.4.3/src/deepali/utils/aws/s3/config.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/aws/s3/object.py` & `hf-deepali-0.4.3/src/deepali/utils/aws/s3/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from copy import deepcopy
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Generator, Optional
 
 from deepali.core.pathlib import PathStr, to_uri
-from deepali.utils.storage import StorageObject
+from deepali.core.storage import StorageObject
 
 from .client import S3Client
 
 
 class S3Object(StorageObject):
     r"""Object stored in AWS Simple Storage Service (S3)."""
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/ignite/handlers.py` & `hf-deepali-0.4.3/src/deepali/utils/ignite/handlers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/average_loss.py` & `hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/average_loss.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/binary_classification.py` & `hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/binary_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/ignite/metrics/multilabel_classification.py` & `hf-deepali-0.4.3/src/deepali/utils/ignite/metrics/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/ignite/output_transforms.py` & `hf-deepali-0.4.3/src/deepali/utils/ignite/output_transforms.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/ignite/score_functions.py` & `hf-deepali-0.4.3/src/deepali/utils/ignite/score_functions.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/imageio/__init__.py` & `hf-deepali-0.4.3/src/deepali/utils/imageio/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/imageio/meta.py` & `hf-deepali-0.4.3/src/deepali/utils/imageio/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 import torch
 from torch import Tensor
 
 from deepali.core.grid import Grid
 from deepali.core.pathlib import PathUri, path_suffix
-from deepali.utils.storage import StorageObject
+from deepali.core.storage import StorageObject
 
 
 META_IMAGE_SUFFIXES = (".mha", ".mhd")
 
 
 def has_meta_image_suffix(path: PathUri) -> bool:
     r"""Check whether filename ends in a MetaImage extension."""
@@ -60,14 +60,18 @@
     spacing = meta.get("ElementSpacing")
     grid = Grid(
         size=size,
         origin=origin,
         spacing=spacing,
         direction=matrix,
     )
+    if data.dtype == np.uint16:
+        data = data.astype(np.int32)
+    elif data.dtype == np.uint32:
+        data = data.astype(np.int64)
     return torch.from_numpy(data), grid
 
 
 def write_meta_image(data: Tensor, grid: Grid, path: PathUri, compress: bool = True) -> None:
     r"""Write image data and grid attributes to MetaImage file."""
     suffix = path_suffix(path).lower()
     if suffix == ".mha":
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/imageio/nifti.py` & `hf-deepali-0.4.3/src/deepali/utils/imageio/nifti.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import numpy as np
 import torch
 from torch import Tensor
 
 from deepali.core.grid import Grid
 from deepali.core.pathlib import PathUri, path_suffix, unlink_or_mkdir
-from deepali.utils.storage import StorageObject
+from deepali.core.storage import StorageObject
 
 
 NIFTI_IMAGE_SUFFIXES = (".nia", ".nii", ".nii.gz", ".hdr", ".hdr.gz", ".img", ".img.gz")
 
 
 def has_nifti_image_suffix(path: PathUri) -> bool:
     r"""Check whether filename ends in a NIfTI image extension."""
@@ -84,14 +84,18 @@
     data = np.reshape(data, data.shape[:realdim] + data.shape[5:])
     # Reverse order of axes
     data = np.transpose(data, axes=tuple(reversed(range(data.ndim))))
     # Add leading channel dimension
     grid = Grid(size=size, origin=origin, spacing=spacing, direction=direction)
     if data.ndim == grid.ndim:
         data = np.expand_dims(data, 0)
+    if data.dtype == np.uint16:
+        data = data.astype(np.int32)
+    elif data.dtype == np.uint32:
+        data = data.astype(np.int64)
     return torch.from_numpy(data), grid
 
 
 def write_nifti_image(data: Tensor, grid: Grid, path: PathUri) -> None:
     r"""Write image data and grid attributes to NIfTI image file."""
     if not has_nifti_image_suffix(path):
         raise ValueError(f"NIfTI image filename suffix must be one of {NIFTI_IMAGE_SUFFIXES}")
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/imageio/sitk.py` & `hf-deepali-0.4.3/src/deepali/utils/imageio/sitk.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,10 +19,10 @@
     return data, grid
 
 
 def write_sitk_image(data: Tensor, grid: Grid, path: PathUri, compress: bool = True) -> None:
     r"""Write image file in any format supported by SimpleITK."""
     origin = grid.origin().tolist()
     spacing = grid.spacing().tolist()
-    direction = grid.direction().tolist()
+    direction = grid.direction().flatten().tolist()
     image = image_from_tensor(data, origin=origin, spacing=spacing, direction=direction)
     _write_image(image, path, compress=compress)
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/simpleitk/grid.py` & `hf-deepali-0.4.3/src/deepali/utils/simpleitk/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/simpleitk/imageio.py` & `hf-deepali-0.4.3/src/deepali/utils/simpleitk/imageio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from deepali.core.pathlib import PathUri, unlink_or_mkdir
-from deepali.utils.storage import StorageObject
+from deepali.core.storage import StorageObject
 
 import SimpleITK as sitk
 
 
 def read_image(path: PathUri) -> sitk.Image:
     r"""Read image from file."""
     with StorageObject.from_path(path) as obj:
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/simpleitk/numpy.py` & `hf-deepali-0.4.3/src/deepali/utils/simpleitk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/simpleitk/sample.py` & `hf-deepali-0.4.3/src/deepali/utils/simpleitk/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/simpleitk/torch.py` & `hf-deepali-0.4.3/src/deepali/utils/simpleitk/torch.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,14 @@
     image: sitk.Image,
     dtype: Optional[torch.dtype] = None,
     device: Optional[torch.device] = None,
 ) -> torch.Tensor:
     r"""Create image data tensor from ``SimpleITK.Image``."""
     if image.GetPixelID() == sitk.sitkUInt16:
         image = sitk.Cast(image, sitk.sitkInt32)
-    elif image.GetPixelID() == sitk.sitkUInt16:
+    elif image.GetPixelID() == sitk.sitkUInt32:
         image = sitk.Cast(image, sitk.sitkInt64)
     data = torch.from_numpy(sitk.GetArrayFromImage(image))
     data = data.unsqueeze(0)
     if image.GetNumberOfComponentsPerPixel() > 1:
         data = data.transpose(0, -1).squeeze(-1)
     return data.to(dtype=dtype, device=device)
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/storage.py` & `hf-deepali-0.4.3/src/deepali/core/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from copy import deepcopy
 from pathlib import Path
 import re
 import shutil
 from typing import Generator, Optional, TypeVar, cast
 from urllib.parse import urlsplit
 
-from deepali.core.pathlib import PathStr, PathUri, to_uri, unlink_or_mkdir
+from .pathlib import PathStr, PathUri, to_uri, unlink_or_mkdir
 
 
 __all__ = (
     "LocalObject",
     "StorageObject",
     "copy_file",
 )
@@ -141,16 +141,18 @@
         res = urlsplit(uri, scheme="file")
         if res.scheme == "file":
             match = re.match(r"/+([a-zA-Z]:.*)", res.path)
             path = match.group(1) if match else res.path
             return LocalObject(Path("/" + res.netloc + "/" + path if res.netloc else path))
         if res.scheme == "s3":
             # DO NOT import at module level to avoid cyclical import!
-            from .aws.s3.object import S3Object
-
+            try:
+                from deepali.utils.aws.s3.object import S3Object
+            except ImportError:
+                raise ImportError("StorageObject.from_uri() requires AWS S3 deepali[utils]")
             return cast(StorageObject, S3Object.from_uri(uri))
         raise ValueError("Invalid or unsupported storage object URI: %s", uri)
 
     @property
     def uri(self) -> str:
         r"""
         Returns:
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/tensorboard.py` & `hf-deepali-0.4.3/src/deepali/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/vtk/idlist.py` & `hf-deepali-0.4.3/src/deepali/utils/vtk/idlist.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/vtk/image.py` & `hf-deepali-0.4.3/src/deepali/utils/vtk/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/vtk/numpy.py` & `hf-deepali-0.4.3/src/deepali/utils/vtk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/deepali/utils/vtk/polydataio.py` & `hf-deepali-0.4.3/src/deepali/utils/vtk/polydataio.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from vtk import vtkCellArray, vtkPoints, vtkPolyData
 from vtk import vtkOBJReader, vtkOBJWriter
 from vtk import vtkPLYReader, vtkPLYWriter
 from vtk import vtkXMLPolyDataReader, vtkXMLPolyDataWriter
 from vtk import vtkPolyDataReader, vtkPolyDataWriter
 
 from deepali.core.pathlib import PathUri
-from deepali.utils.storage import StorageObject
+from deepali.core.storage import StorageObject
 
 from .numpy import vtk_to_numpy_array, vtk_to_numpy_points
 
 
 def read_polydata(path: PathUri) -> vtkPolyData:
     r"""Read vtkPolyData from specified file."""
     with StorageObject.from_path(path) as obj:
```

### Comparing `hf-deepali-0.4.2/src/deepali/utils/vtk/simpleitk.py` & `hf-deepali-0.4.3/src/deepali/utils/vtk/simpleitk.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/src/hf_deepali.egg-info/PKG-INFO` & `hf-deepali-0.4.3/src/hf_deepali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.4.2
+Version: 0.4.3
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
```

### Comparing `hf-deepali-0.4.2/src/hf_deepali.egg-info/SOURCES.txt` & `hf-deepali-0.4.3/src/hf_deepali.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 src/deepali/core/logging.py
 src/deepali/core/math.py
 src/deepali/core/nnutils.py
 src/deepali/core/pathlib.py
 src/deepali/core/pointset.py
 src/deepali/core/psutil.py
 src/deepali/core/random.py
+src/deepali/core/storage.py
 src/deepali/core/tempfile.py
 src/deepali/core/tensor.py
 src/deepali/core/typing.py
 src/deepali/data/__init__.py
 src/deepali/data/collate.py
 src/deepali/data/dataset.py
 src/deepali/data/flow.py
@@ -157,15 +158,14 @@
 src/deepali/spatial/image.py
 src/deepali/spatial/linear.py
 src/deepali/spatial/nonrigid.py
 src/deepali/spatial/parametric.py
 src/deepali/spatial/transformer.py
 src/deepali/utils/__init__.py
 src/deepali/utils/ipython.py
-src/deepali/utils/storage.py
 src/deepali/utils/tensorboard.py
 src/deepali/utils/aws/__init__.py
 src/deepali/utils/aws/s3/__init__.py
 src/deepali/utils/aws/s3/client.py
 src/deepali/utils/aws/s3/config.py
 src/deepali/utils/aws/s3/object.py
 src/deepali/utils/ignite/__init__.py
```

### Comparing `hf-deepali-0.4.2/tests/_test_core_bspline.py` & `hf-deepali-0.4.3/tests/_test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_core_bspline.py` & `hf-deepali-0.4.3/tests/test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_core_cube.py` & `hf-deepali-0.4.3/tests/test_core_cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_core_grid.py` & `hf-deepali-0.4.3/tests/test_core_grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_core_image_create.py` & `hf-deepali-0.4.3/tests/test_core_image_create.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_core_image_utils.py` & `hf-deepali-0.4.3/tests/test_core_image_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_core_random.py` & `hf-deepali-0.4.3/tests/test_core_random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_core_tensor_utils.py` & `hf-deepali-0.4.3/tests/test_core_tensor_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_data_flow.py` & `hf-deepali-0.4.3/tests/test_data_flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_data_image.py` & `hf-deepali-0.4.3/tests/test_data_image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_network_blocks.py` & `hf-deepali-0.4.3/tests/test_network_blocks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_network_layers.py` & `hf-deepali-0.4.3/tests/test_network_layers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_network_unet.py` & `hf-deepali-0.4.3/tests/test_network_unet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_spatial_transformer.py` & `hf-deepali-0.4.3/tests/test_spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.2/tests/test_utils_imageio_meta.py` & `hf-deepali-0.4.3/tests/test_utils_imageio_meta.py`

 * *Files identical despite different names*

