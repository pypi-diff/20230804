# Comparing `tmp/pantea-0.8.1.tar.gz` & `tmp/pantea-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantea-0.8.1.tar", last modified: Wed Aug  2 17:55:35 2023, max compression
+gzip compressed data, was "pantea-0.8.2.tar", last modified: Fri Aug  4 16:35:42 2023, max compression
```

## Comparing `pantea-0.8.1.tar` & `pantea-0.8.2.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.966143 pantea-0.8.1/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 pantea-0.8.1/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3427 2023-08-02 17:31:18.000000 pantea-0.8.1/CONTRIBUTING.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      742 2023-08-02 17:36:01.000000 pantea-0.8.1/HISTORY.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1612 2023-08-02 17:31:18.000000 pantea-0.8.1/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 pantea-0.8.1/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6329 2023-08-02 17:55:35.966143 pantea-0.8.1/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5688 2023-08-02 17:46:57.000000 pantea-0.8.1/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.926143 pantea-0.8.1/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      607 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.902143 pantea-0.8.1/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.902143 pantea-0.8.1/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.926143 pantea-0.8.1/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11092 2023-08-02 16:54:23.000000 pantea-0.8.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-02 16:54:23.000000 pantea-0.8.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-02 16:54:23.000000 pantea-0.8.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.902143 pantea-0.8.1/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.930143 pantea-0.8.1/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11092 2023-08-02 16:54:23.000000 pantea-0.8.1/docs/_build/html/_images/notebooks_getting_started_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-02 16:54:23.000000 pantea-0.8.1/docs/_build/html/_images/notebooks_getting_started_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-02 16:54:23.000000 pantea-0.8.1/docs/_build/html/_images/notebooks_getting_started_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.930143 pantea-0.8.1/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 pantea-0.8.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 pantea-0.8.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 pantea-0.8.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 pantea-0.8.1/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6613 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 pantea-0.8.1/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       87 2023-07-22 19:34:04.000000 pantea-0.8.1/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 pantea-0.8.1/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.930143 pantea-0.8.1/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 pantea-0.8.1/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)   387986 2023-07-24 18:54:32.000000 pantea-0.8.1/docs/images/logo.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 pantea-0.8.1/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      316 2023-08-02 17:47:58.000000 pantea-0.8.1/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1873 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      804 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       55 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      775 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      504 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1113 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      623 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      698 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      407 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1311 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      471 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      986 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      969 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.simulation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      933 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/pantea.utils.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 pantea-0.8.1/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3834 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1161 2023-08-02 17:31:18.000000 pantea-0.8.1/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.934143 pantea-0.8.1/pantea/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      489 2023-08-02 17:49:46.000000 pantea-0.8.1/pantea/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-08-02 17:52:32.000000 pantea-0.8.1/pantea/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.938143 pantea-0.8.1/pantea/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      236 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1487 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3803 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6642 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3358 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    17798 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1124 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.938143 pantea-0.8.1/pantea/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      409 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/datasets/dataset.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6513 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/datasets/runner.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.938143 pantea-0.8.1/pantea/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      132 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.950143 pantea-0.8.1/pantea/descriptors/acsf/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      404 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5318 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     8156 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2239 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3902 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1498 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1019 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      617 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/descriptor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7535 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3762 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.950143 pantea-0.8.1/pantea/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       89 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      390 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/models/model.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.950143 pantea-0.8.1/pantea/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      183 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      618 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2896 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.954143 pantea-0.8.1/pantea/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      214 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1984 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      876 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1858 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.954143 pantea-0.8.1/pantea/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      240 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9530 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9590 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2641 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      547 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/nnp/nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    19323 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11439 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3626 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/pytree.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.958143 pantea-0.8.1/pantea/simulation/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      300 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/simulation/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2145 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/simulation/lj.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4386 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/simulation/mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9137 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/simulation/md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2516 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/simulation/run.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      840 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/simulation/thermostat.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/types.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.958143 pantea-0.8.1/pantea/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       74 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1424 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      586 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2037 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4484 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/utils/profiler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      670 2023-08-02 17:31:18.000000 pantea-0.8.1/pantea/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.934143 pantea-0.8.1/pantea.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6329 2023-08-02 17:55:35.000000 pantea-0.8.1/pantea.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3359 2023-08-02 17:55:35.000000 pantea-0.8.1/pantea.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-08-02 17:55:35.000000 pantea-0.8.1/pantea.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       43 2023-08-02 17:55:35.000000 pantea-0.8.1/pantea.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-08-02 17:55:35.000000 pantea-0.8.1/pantea.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-08-02 17:55:35.000000 pantea-0.8.1/pantea.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        7 2023-08-02 17:55:35.000000 pantea-0.8.1/pantea.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-08-02 17:55:35.966143 pantea-0.8.1/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1545 2023-08-02 17:31:18.000000 pantea-0.8.1/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.962143 pantea-0.8.1/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-02 17:55:35.966143 pantea-0.8.1/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 pantea-0.8.1/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 pantea-0.8.1/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 pantea-0.8.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 pantea-0.8.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       36 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 pantea-0.8.1/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 pantea-0.8.1/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-08-01 06:20:15.000000 pantea-0.8.1/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-08-01 06:20:15.000000 pantea-0.8.1/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5515 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2572 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3140 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4129 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3461 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5285 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2880 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5912 2023-08-02 17:31:18.000000 pantea-0.8.1/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-08-01 06:20:15.000000 pantea-0.8.1/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-08-01 06:20:15.000000 pantea-0.8.1/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.334341 pantea-0.8.2/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 pantea-0.8.2/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3427 2023-08-02 18:18:46.000000 pantea-0.8.2/CONTRIBUTING.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      755 2023-08-03 07:56:08.000000 pantea-0.8.2/HISTORY.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1612 2023-08-02 18:18:46.000000 pantea-0.8.2/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 pantea-0.8.2/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6242 2023-08-04 16:35:42.338341 pantea-0.8.2/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5597 2023-08-03 07:56:08.000000 pantea-0.8.2/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.262341 pantea-0.8.2/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      607 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.242341 pantea-0.8.2/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.242341 pantea-0.8.2/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.266341 pantea-0.8.2/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11092 2023-08-04 07:32:35.000000 pantea-0.8.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-04 07:32:35.000000 pantea-0.8.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-04 07:32:35.000000 pantea-0.8.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.242341 pantea-0.8.2/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.270341 pantea-0.8.2/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11092 2023-08-04 07:03:49.000000 pantea-0.8.2/docs/_build/html/_images/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-04 07:03:49.000000 pantea-0.8.2/docs/_build/html/_images/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9905 2023-08-04 07:03:49.000000 pantea-0.8.2/docs/_build/html/_images/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.270341 pantea-0.8.2/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 pantea-0.8.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 pantea-0.8.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 pantea-0.8.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 pantea-0.8.2/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6613 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 pantea-0.8.2/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       87 2023-07-22 19:34:04.000000 pantea-0.8.2/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 pantea-0.8.2/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.278341 pantea-0.8.2/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 pantea-0.8.2/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)   387986 2023-07-24 18:54:32.000000 pantea-0.8.2/docs/images/logo.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 pantea-0.8.2/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      316 2023-08-04 16:35:02.000000 pantea-0.8.2/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2108 2023-08-04 16:35:02.000000 pantea-0.8.2/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      804 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       55 2023-08-04 07:03:47.000000 pantea-0.8.2/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      775 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      504 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1113 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      623 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      698 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      407 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1311 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      471 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      986 2023-08-04 07:03:47.000000 pantea-0.8.2/docs/pantea.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      969 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.simulation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      933 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/pantea.utils.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 pantea-0.8.2/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3834 2023-08-02 18:18:46.000000 pantea-0.8.2/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1471 2023-08-04 16:35:02.000000 pantea-0.8.2/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.286341 pantea-0.8.2/pantea/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      489 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-08-04 16:35:02.000000 pantea-0.8.2/pantea/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.298341 pantea-0.8.2/pantea/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      236 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1487 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3803 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6642 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3358 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    17798 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1124 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.302341 pantea-0.8.2/pantea/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      409 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/datasets/dataset.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6513 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/datasets/runner.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.302341 pantea-0.8.2/pantea/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      132 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.306341 pantea-0.8.2/pantea/descriptors/acsf/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      404 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5318 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     8156 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2239 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3902 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1498 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1019 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      617 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/descriptor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7535 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3762 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.306341 pantea-0.8.2/pantea/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       89 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      390 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/models/model.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.306341 pantea-0.8.2/pantea/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      183 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      618 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2896 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.306341 pantea-0.8.2/pantea/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      214 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1984 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      876 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1858 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.310341 pantea-0.8.2/pantea/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      240 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9530 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9590 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2641 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      547 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/nnp/nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    19323 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11439 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3626 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/pytree.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.310341 pantea-0.8.2/pantea/simulation/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      300 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/simulation/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2145 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/simulation/lj.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4386 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/simulation/mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9137 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/simulation/md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2516 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/simulation/run.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      840 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/simulation/thermostat.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/types.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.314341 pantea-0.8.2/pantea/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       74 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1424 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      586 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2037 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4484 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/utils/profiler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      670 2023-08-02 18:18:46.000000 pantea-0.8.2/pantea/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.294341 pantea-0.8.2/pantea.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6242 2023-08-04 16:35:42.000000 pantea-0.8.2/pantea.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3359 2023-08-04 16:35:42.000000 pantea-0.8.2/pantea.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-08-04 16:35:42.000000 pantea-0.8.2/pantea.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       43 2023-08-04 16:35:42.000000 pantea-0.8.2/pantea.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-08-04 16:35:41.000000 pantea-0.8.2/pantea.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-08-04 16:35:42.000000 pantea-0.8.2/pantea.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        7 2023-08-04 16:35:42.000000 pantea-0.8.2/pantea.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-08-04 16:35:42.342341 pantea-0.8.2/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1549 2023-08-03 07:56:08.000000 pantea-0.8.2/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.330341 pantea-0.8.2/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-08-04 16:35:42.334341 pantea-0.8.2/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 pantea-0.8.2/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 pantea-0.8.2/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 pantea-0.8.2/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 pantea-0.8.2/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       36 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 pantea-0.8.2/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 pantea-0.8.2/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-08-01 06:20:15.000000 pantea-0.8.2/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-08-01 06:20:15.000000 pantea-0.8.2/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5515 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2572 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3140 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4129 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3461 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5285 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2880 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5912 2023-08-02 18:18:46.000000 pantea-0.8.2/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-08-01 06:20:15.000000 pantea-0.8.2/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-08-01 06:20:15.000000 pantea-0.8.2/tests/weights.008.pkl
```

### Comparing `pantea-0.8.1/CONTRIBUTING.rst` & `pantea-0.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/HISTORY.rst` & `pantea-0.8.2/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 0.7.x
 -------------------
 * Refactored structure including design, documentation, and performance (JIT kernels)
 * Refactored RuNNer dataset
 
 0.6.x
 -------------------
-* Implemented Molecular dynamics (MD) and Monte-Carlo (MC) simulators
+* Implemented Molecular dynamics (MD) simulator
+* Added Monte-Carlo (MC) simulator
 
 0.5.x
 -------------------
 * Implemented Kalman filter trainer 
 
 0.4.x
 -------------------
```

### Comparing `pantea-0.8.1/LICENSE` & `pantea-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/PKG-INFO` & `pantea-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pantea
-Version: 0.8.1
-Summary: An optimized Python package for developing machine learning interatomic potentials
+Version: 0.8.2
+Summary: A Python package for developing machine learning interatomic potentials, based on JAX.
 Home-page: https://github.com/hghcomphys/pantea
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: pantea
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,14 @@
 .. .. image:: docs/images/logo.png
 ..         :alt: logo
         
 ======
 Pantea
 ======
 
-**A Python package for developing machine learning interatomic potentials, based on JAX**
-
 
 .. image:: https://img.shields.io/pypi/v/pantea.svg
         :target: https://pypi.python.org/pypi/pantea
 
 .. image:: https://github.com/hghcomphys/pantea/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/hghcomphys/pantea/blob/main/.github/workflows/tests.yml
```

### Comparing `pantea-0.8.1/README.rst` & `pantea-0.8.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 .. .. image:: docs/images/logo.png
 ..         :alt: logo
         
 ======
 Pantea
 ======
 
-**A Python package for developing machine learning interatomic potentials, based on JAX**
-
 
 .. image:: https://img.shields.io/pypi/v/pantea.svg
         :target: https://pypi.python.org/pypi/pantea
 
 .. image:: https://github.com/hghcomphys/pantea/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/hghcomphys/pantea/blob/main/.github/workflows/tests.yml
```

### Comparing `pantea-0.8.1/docs/Makefile` & `pantea-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png` & `pantea-0.8.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png` & `pantea-0.8.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png` & `pantea-0.8.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/_build/html/_images/notebooks_getting_started_38_0.png` & `pantea-0.8.2/docs/_build/html/_images/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/_build/html/_images/notebooks_getting_started_45_0.png` & `pantea-0.8.2/docs/_build/html/_images/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/_build/html/_images/notebooks_getting_started_51_0.png` & `pantea-0.8.2/docs/_build/html/_images/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/conf.py` & `pantea-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/images/flowchart.drawio.png` & `pantea-0.8.2/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/images/logo.png` & `pantea-0.8.2/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/images/water.png` & `pantea-0.8.2/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/installation.rst` & `pantea-0.8.2/docs/installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,24 @@
 Please refer to the `JAX Install Guide`_ for full installation instructions.
 
 
 .. _JAX: https://github.com/google/jax
 .. _`JAX Install Guide`: https://github.com/google/jax#installation
 
 
+For atom visualization in Jupyter Notebooks, it is also recommended to
+install `nglview`_ using conda as follows:
+
+.. code-block:: python
+
+    $ conda install -c conda-forge nglview
+
+.. _nglview: https://github.com/nglviewer/nglview
+
+
 Stable release
 --------------
 
 To install Pantea, run this command in your terminal:
 
 .. code-block:: console
```

### Comparing `pantea-0.8.1/docs/make.bat` & `pantea-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.atoms.rst` & `pantea-0.8.2/docs/pantea.atoms.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.descriptors.acsf.rst` & `pantea-0.8.2/docs/pantea.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.descriptors.rst` & `pantea-0.8.2/docs/pantea.descriptors.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.models.nn.rst` & `pantea-0.8.2/docs/pantea.models.nn.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.potentials.nnp.rst` & `pantea-0.8.2/docs/pantea.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.rst` & `pantea-0.8.2/docs/pantea.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.simulation.rst` & `pantea-0.8.2/docs/pantea.simulation.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/pantea.utils.rst` & `pantea-0.8.2/docs/pantea.utils.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/docs/theory.rst` & `pantea-0.8.2/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/atoms/_structure.py` & `pantea-0.8.2/pantea/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/atoms/box.py` & `pantea-0.8.2/pantea/atoms/box.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/atoms/element.py` & `pantea-0.8.2/pantea/atoms/element.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/atoms/neighbor.py` & `pantea-0.8.2/pantea/atoms/neighbor.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/atoms/structure.py` & `pantea-0.8.2/pantea/atoms/structure.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/config.py` & `pantea-0.8.2/pantea/config.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/datasets/runner.py` & `pantea-0.8.2/pantea/datasets/runner.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/acsf/_acsf.py` & `pantea-0.8.2/pantea/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/acsf/acsf.py` & `pantea-0.8.2/pantea/descriptors/acsf/acsf.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/acsf/angular.py` & `pantea-0.8.2/pantea/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/acsf/cutoff.py` & `pantea-0.8.2/pantea/descriptors/acsf/cutoff.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/acsf/radial.py` & `pantea-0.8.2/pantea/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/acsf/symmetry.py` & `pantea-0.8.2/pantea/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/descriptor.py` & `pantea-0.8.2/pantea/descriptors/descriptor.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/descriptors/scaler.py` & `pantea-0.8.2/pantea/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/logger.py` & `pantea-0.8.2/pantea/logger.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/models/nn/activation.py` & `pantea-0.8.2/pantea/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/models/nn/initializer.py` & `pantea-0.8.2/pantea/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/models/nn/network.py` & `pantea-0.8.2/pantea/models/nn/network.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/_energy.py` & `pantea-0.8.2/pantea/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/_force.py` & `pantea-0.8.2/pantea/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/atomic_potential.py` & `pantea-0.8.2/pantea/potentials/atomic_potential.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/nnp/gradient_descent.py` & `pantea-0.8.2/pantea/potentials/nnp/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/nnp/kalman_filter.py` & `pantea-0.8.2/pantea/potentials/nnp/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/nnp/metrics.py` & `pantea-0.8.2/pantea/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/nnp/nnp.py` & `pantea-0.8.2/pantea/potentials/nnp/nnp.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/nnp/potential.py` & `pantea-0.8.2/pantea/potentials/nnp/potential.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/potentials/nnp/settings.py` & `pantea-0.8.2/pantea/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/pytree.py` & `pantea-0.8.2/pantea/pytree.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/simulation/lj.py` & `pantea-0.8.2/pantea/simulation/lj.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/simulation/mc.py` & `pantea-0.8.2/pantea/simulation/mc.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/simulation/md.py` & `pantea-0.8.2/pantea/simulation/md.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/simulation/run.py` & `pantea-0.8.2/pantea/simulation/run.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/simulation/thermostat.py` & `pantea-0.8.2/pantea/simulation/thermostat.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/types.py` & `pantea-0.8.2/pantea/types.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/units.py` & `pantea-0.8.2/pantea/units.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/utils/attribute.py` & `pantea-0.8.2/pantea/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/utils/batch.py` & `pantea-0.8.2/pantea/utils/batch.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/utils/compare.py` & `pantea-0.8.2/pantea/utils/compare.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/utils/profiler.py` & `pantea-0.8.2/pantea/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea/utils/tokenize.py` & `pantea-0.8.2/pantea/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/pantea.egg-info/PKG-INFO` & `pantea-0.8.2/pantea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pantea
-Version: 0.8.1
-Summary: An optimized Python package for developing machine learning interatomic potentials
+Version: 0.8.2
+Summary: A Python package for developing machine learning interatomic potentials, based on JAX.
 Home-page: https://github.com/hghcomphys/pantea
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: pantea
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,14 @@
 .. .. image:: docs/images/logo.png
 ..         :alt: logo
         
 ======
 Pantea
 ======
 
-**A Python package for developing machine learning interatomic potentials, based on JAX**
-
 
 .. image:: https://img.shields.io/pypi/v/pantea.svg
         :target: https://pypi.python.org/pypi/pantea
 
 .. image:: https://github.com/hghcomphys/pantea/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/hghcomphys/pantea/blob/main/.github/workflows/tests.yml
```

### Comparing `pantea-0.8.1/pantea.egg-info/SOURCES.txt` & `pantea-0.8.2/pantea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/setup.py` & `pantea-0.8.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.8",
     ],
-    description="An optimized Python package for developing machine learning interatomic potentials",
+    description="A Python package for developing machine learning interatomic potentials, based on JAX.",
     entry_points={
         "console_scripts": [
             "pantea=pantea.cli:main",
         ],
     },
     install_requires=requirements,
     license="GNU General Public License v3",
```

### Comparing `pantea-0.8.1/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `pantea-0.8.2/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `pantea-0.8.2/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `pantea-0.8.2/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `pantea-0.8.2/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/h2o.data` & `pantea-0.8.2/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/h2o.json` & `pantea-0.8.2/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_acsf.py` & `pantea-0.8.2/tests/test_acsf.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_mc.py` & `pantea-0.8.2/tests/test_mc.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_md.py` & `pantea-0.8.2/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_nn.py` & `pantea-0.8.2/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_nnp.py` & `pantea-0.8.2/tests/test_nnp.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_runner.py` & `pantea-0.8.2/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_scaler.py` & `pantea-0.8.2/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/test_structure.py` & `pantea-0.8.2/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/weights.001.pkl` & `pantea-0.8.2/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `pantea-0.8.1/tests/weights.008.pkl` & `pantea-0.8.2/tests/weights.008.pkl`

 * *Files identical despite different names*

