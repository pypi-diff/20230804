# Comparing `tmp/irispie-0.1.3.tar.gz` & `tmp/irispie-0.1.4.tar.gz`

## Comparing `irispie-0.1.3.tar` & `irispie-0.1.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 irispie-0.1.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/app.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/appearance.json
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/core-plugins.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/hotkeys.json
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/workspace.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/algorithms/detach-unit-roots.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/architecture/Untitled.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/architecture/steady.canvas
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/dates/Ranger.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/milestones/March-2023.md
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/milestones/iris-gray.png
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/series/example.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/__init__.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equations.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/exceptions.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/incidence.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/quantities.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/requirements
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/session
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/tags
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/wrongdoings.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/adaptations.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/differentiators.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/express.py~
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/finite_differentiators.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/invariators.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/maps.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/databanks.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/dataslabs.py
--rw-r--r--   0        0        0    20362 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/dates.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/exports.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/filters.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/imports.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/imports2.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/plotly.py
--rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/series.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/views.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/abc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/plain.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/steady.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/evaluators/printers.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/evaluators/steady.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/__init__.py
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/descriptors.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/simulators.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/solutions.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/steadiers.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/systems.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/jacobians/abc.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/jacobians/steady.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/mixins/userdata.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/__init__.py
--rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/facade.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/flags.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/gettables.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/invariants.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/simulatables.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/sources.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/steadiables.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/variants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/common.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/model_source_parser.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/preparser.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/pseudofunctions.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/shifts.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/substitutions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.3/tests/.gitkeep
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.3/tests/dataman/series/hpf_test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.3/LICENCE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.3/README.md
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 irispie-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 irispie-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 irispie-0.1.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/app.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/appearance.json
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/hotkeys.json
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/workspace.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/algorithms/detach-unit-roots.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/architecture/Untitled.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/architecture/steady.canvas
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/dates/Ranger.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/milestones/March-2023.md
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/milestones/iris-gray.png
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/series/example.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/__init__.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equations.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/exceptions.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/incidence.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/quantities.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/requirements
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/session
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/tags
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/wrongdoings.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/adaptations.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/differentiators.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/express.py~
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/finite_differentiators.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/invariators.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/maps.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/databanks.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/dataslabs.py
+-rw-r--r--   0        0        0    20362 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/dates.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/exports.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/filters.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/imports.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/imports2.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/plotly.py
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/series.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/views.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/abc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/plain.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/steady.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/evaluators/printers.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/evaluators/steady.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/__init__.py
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/descriptors.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/simulators.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/solutions.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/steadiers.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/systems.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/jacobians/abc.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/jacobians/steady.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/mixins/userdata.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/__init__.py
+-rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/facade.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/flags.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/gettables.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/invariants.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/simulatables.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/sources.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/steadiables.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/variants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/common.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/model_source_parser.py
+-rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/preparser.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/pseudofunctions.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/shifts.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/substitutions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.4/tests/.gitkeep
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.4/tests/dataman/series/hpf_test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.4/LICENCE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.4/README.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 irispie-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 irispie-0.1.4/PKG-INFO
```

### Comparing `irispie-0.1.3/.github/workflows/publish-to-pypi.yml` & `irispie-0.1.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/docs/.obsidian/core-plugins-migration.json` & `irispie-0.1.4/docs/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/docs/.obsidian/workspace.json` & `irispie-0.1.4/docs/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/docs/algorithms/detach-unit-roots.md` & `irispie-0.1.4/docs/algorithms/detach-unit-roots.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/docs/milestones/March-2023.md` & `irispie-0.1.4/docs/milestones/March-2023.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/docs/milestones/iris-gray.png` & `irispie-0.1.4/docs/milestones/iris-gray.png`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/docs/series/example.py` & `irispie-0.1.4/docs/series/example.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/equations.py` & `irispie-0.1.4/src/irispie/equations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/exceptions.py` & `irispie-0.1.4/src/irispie/exceptions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/incidence.py` & `irispie-0.1.4/src/irispie/incidence.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/quantities.py` & `irispie-0.1.4/src/irispie/quantities.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/requirements` & `irispie-0.1.4/src/irispie/requirements`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/session` & `irispie-0.1.4/src/irispie/session`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/tags` & `irispie-0.1.4/src/irispie/tags`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/wrongdoings.py` & `irispie-0.1.4/src/irispie/wrongdoings.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/aldi/adaptations.py` & `irispie-0.1.4/src/irispie/aldi/adaptations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/aldi/differentiators.py` & `irispie-0.1.4/src/irispie/aldi/differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/aldi/express.py~` & `irispie-0.1.4/src/irispie/aldi/express.py~`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/aldi/finite_differentiators.py` & `irispie-0.1.4/src/irispie/aldi/finite_differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/aldi/invariators.py` & `irispie-0.1.4/src/irispie/aldi/invariators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/aldi/maps.py` & `irispie-0.1.4/src/irispie/aldi/maps.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/databanks.py` & `irispie-0.1.4/src/irispie/dataman/databanks.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/dataslabs.py` & `irispie-0.1.4/src/irispie/dataman/dataslabs.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/dates.py` & `irispie-0.1.4/src/irispie/dataman/dates.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/exports.py` & `irispie-0.1.4/src/irispie/dataman/exports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/filters.py` & `irispie-0.1.4/src/irispie/dataman/filters.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/imports.py` & `irispie-0.1.4/src/irispie/dataman/imports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/imports2.py` & `irispie-0.1.4/src/irispie/dataman/imports2.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/plotly.py` & `irispie-0.1.4/src/irispie/dataman/plotly.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Plotly interface to time series objects
 """
 
 
 #[
 from __future__ import annotations
 
-import plotly.graph_objects as pg
-import plotly.subplots as ps
+import plotly.graph_objects as _pg
+import plotly.subplots as _ps
 from types import (EllipsisType, )
 
-from ..dataman import (dates as da_, )
+from ..dataman import (dates as _da, )
 #]
 
 
 builtin_range = range
 
 
 __all__ = [
@@ -27,46 +27,47 @@
   "rgb(237,   177,    32)",
   "rgb(126,    47,   142)",
   "rgb(119,   172,    48)",
   "rgb( 77,   190,   238)",
   "rgb(162,    20,    47)",
 ]
 
+
 class PlotlyMixin:
     """
     """
     #[
     def plot(
         self,
         /,
-        range: Iterable[da_.Dater] | EllipsisType = ...,
+        range: Iterable[_da.Dater] | EllipsisType = ...,
         title: str | None = None,
         legend: Iterable[str] | None = None,
         show_legend: bool | None = None,
         figure = None,
         subplot: tuple[int|None, int|None] = (None, None),
         xline = None,
     ):
         range = self._resolve_dates(range)
         range = [ t for t in range ]
         data = self.get_data(range)
         num_columns = data.shape[1]
         date_str = [ t.to_plotly_date() for t in range ]
         date_format = range[0].frequency.plotly_format
-        figure = pg.Figure() if figure is None else figure
+        figure = _pg.Figure() if figure is None else figure
         for i in builtin_range(num_columns):
-            figure.add_trace(pg.Scatter(
+            figure.add_trace(_pg.Scatter(
                 x=date_str, y=data[:, i], name=legend[i] if legend else None,
                 line={"color": _COLOR_ORDER[i % len(_COLOR_ORDER)]},
             ), row=subplot[0], col=subplot[1])
         show_legend = show_legend if show_legend is not None else legend is not None
         figure.update_layout(title=title, xaxis={"tickformat": date_format}, showlegend=show_legend)
         if xline:
             xline = xline.to_plotly_date()
             figure.add_vline(xline)
         return figure
     #]
 
 
-make_subplots = ps.make_subplots
+make_subplots = _ps.make_subplots
```

### Comparing `irispie-0.1.3/src/irispie/dataman/series.py` & `irispie-0.1.4/src/irispie/dataman/series.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/dataman/views.py` & `irispie-0.1.4/src/irispie/dataman/views.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/equators/abc.py` & `irispie-0.1.4/src/irispie/equators/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/equators/plain.py` & `irispie-0.1.4/src/irispie/equators/plain.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/equators/steady.py` & `irispie-0.1.4/src/irispie/equators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/evaluators/printers.py` & `irispie-0.1.4/src/irispie/evaluators/printers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/evaluators/steady.py` & `irispie-0.1.4/src/irispie/evaluators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/fords/descriptors.py` & `irispie-0.1.4/src/irispie/fords/descriptors.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/fords/simulators.py` & `irispie-0.1.4/src/irispie/fords/simulators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/fords/solutions.py` & `irispie-0.1.4/src/irispie/fords/solutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/fords/steadiers.py` & `irispie-0.1.4/src/irispie/fords/steadiers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/fords/systems.py` & `irispie-0.1.4/src/irispie/fords/systems.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/jacobians/abc.py` & `irispie-0.1.4/src/irispie/jacobians/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/jacobians/steady.py` & `irispie-0.1.4/src/irispie/jacobians/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/facade.py` & `irispie-0.1.4/src/irispie/models/facade.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/flags.py` & `irispie-0.1.4/src/irispie/models/flags.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/gettables.py` & `irispie-0.1.4/src/irispie/models/gettables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/invariants.py` & `irispie-0.1.4/src/irispie/models/invariants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/simulatables.py` & `irispie-0.1.4/src/irispie/models/simulatables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/sources.py` & `irispie-0.1.4/src/irispie/models/sources.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/steadiables.py` & `irispie-0.1.4/src/irispie/models/steadiables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/models/variants.py` & `irispie-0.1.4/src/irispie/models/variants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/parsers/common.py` & `irispie-0.1.4/src/irispie/parsers/common.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/parsers/model_source_parser.py` & `irispie-0.1.4/src/irispie/parsers/model_source_parser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/parsers/preparser.py` & `irispie-0.1.4/src/irispie/parsers/preparser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/parsers/pseudofunctions.py` & `irispie-0.1.4/src/irispie/parsers/pseudofunctions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/src/irispie/parsers/substitutions.py` & `irispie-0.1.4/src/irispie/parsers/substitutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/LICENCE` & `irispie-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `irispie-0.1.3/pyproject.toml` & `irispie-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "irispie"
-    version = "0.1.3"
+    version = "0.1.4"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Macroeconomic modeling package"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
@@ -23,13 +23,15 @@
         "simulation",
         "forecasting",
         "dsge",
     ]
     dependencies = [
         "numpy >= 1.25",
         "scipy >= 1.11",
+        "plotly >= 5.15",
+        "parsimonious >= 0.10",
     ]
 
 [project.urls]
     "Homepage" = "https://github.com/iris-solutions-team/irispie"
     "Bug Tracker" = "https://github.com/iris-solutions-team/irispie/issues"
```

### Comparing `irispie-0.1.3/PKG-INFO` & `irispie-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: irispie
-Version: 0.1.3
+Version: 0.1.4
 Summary: Macroeconomic modeling package
 Project-URL: Homepage, https://github.com/iris-solutions-team/irispie
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/irispie/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 License-File: LICENCE
 Keywords: dsge,economics,forecasting,macroeconomics,modeling,simulation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: numpy>=1.25
+Requires-Dist: parsimonious>=0.10
+Requires-Dist: plotly>=5.15
 Requires-Dist: scipy>=1.11
 Description-Content-Type: text/markdown
 
 # Iris Pie
 
 Macroeconomic modeling package for Python
```

