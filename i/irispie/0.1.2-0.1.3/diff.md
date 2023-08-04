# Comparing `tmp/irispie-0.1.2.tar.gz` & `tmp/irispie-0.1.3.tar.gz`

## Comparing `irispie-0.1.2.tar` & `irispie-0.1.3.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/app.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/appearance.json
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/core-plugins.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/hotkeys.json
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/workspace.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/algorithms/detach-unit-roots.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/architecture/Untitled.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/architecture/steady.canvas
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/dates/Ranger.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/milestones/March-2023.md
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/milestones/iris-gray.png
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/series/example.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/__init__.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equations.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/exceptions.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/incidence.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/quantities.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/requirements
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/session
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/tags
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/wrongdoings.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/adaptations.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/differentiators.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/express.py~
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/finite_differentiators.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/invariators.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/maps.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/__init__.py
--rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/databanks.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/dataslabs.py
--rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/dates.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/exports.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/filters.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/imports.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/imports2.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/plotly.py
--rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/series.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/views.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/abc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/plain.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/steady.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/evaluators/printers.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/evaluators/steady.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/__init__.py
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/descriptors.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/simulators.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/solutions.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/steadiers.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/systems.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/jacobians/abc.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/jacobians/steady.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/mixins/userdata.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/__init__.py
--rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/facade.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/flags.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/gettables.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/invariants.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/simulatables.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/sources.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/steadiables.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/variants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/common.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/model_source_parser.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/preparser.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/pseudofunctions.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/shifts.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/substitutions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.2/tests/.gitkeep
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.2/tests/dataman/series/hpf_test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.2/LICENCE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.2/README.md
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 irispie-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 irispie-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 irispie-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/app.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/appearance.json
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/hotkeys.json
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/.obsidian/workspace.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/algorithms/detach-unit-roots.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/architecture/Untitled.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/architecture/steady.canvas
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/dates/Ranger.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/milestones/March-2023.md
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/milestones/iris-gray.png
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.3/docs/series/example.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/__init__.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equations.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/exceptions.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/incidence.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/quantities.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/requirements
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/session
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/tags
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/wrongdoings.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/adaptations.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/differentiators.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/express.py~
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/finite_differentiators.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/invariators.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/aldi/maps.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/databanks.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/dataslabs.py
+-rw-r--r--   0        0        0    20362 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/dates.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/exports.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/filters.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/imports.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/imports2.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/plotly.py
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/series.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/dataman/views.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/abc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/plain.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/equators/steady.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/evaluators/printers.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/evaluators/steady.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/__init__.py
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/descriptors.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/simulators.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/solutions.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/steadiers.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/fords/systems.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/jacobians/abc.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/jacobians/steady.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/mixins/userdata.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/__init__.py
+-rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/facade.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/flags.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/gettables.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/invariants.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/simulatables.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/sources.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/steadiables.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/models/variants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/common.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/model_source_parser.py
+-rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/preparser.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/pseudofunctions.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/shifts.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.3/src/irispie/parsers/substitutions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.3/tests/.gitkeep
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.3/tests/dataman/series/hpf_test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.3/LICENCE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.3/README.md
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 irispie-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 irispie-0.1.3/PKG-INFO
```

### Comparing `irispie-0.1.2/.github/workflows/publish-to-pypi.yml` & `irispie-0.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/docs/.obsidian/core-plugins-migration.json` & `irispie-0.1.3/docs/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/docs/.obsidian/workspace.json` & `irispie-0.1.3/docs/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/docs/algorithms/detach-unit-roots.md` & `irispie-0.1.3/docs/algorithms/detach-unit-roots.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/docs/milestones/March-2023.md` & `irispie-0.1.3/docs/milestones/March-2023.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/docs/milestones/iris-gray.png` & `irispie-0.1.3/docs/milestones/iris-gray.png`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/docs/series/example.py` & `irispie-0.1.3/docs/series/example.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/equations.py` & `irispie-0.1.3/src/irispie/equations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/exceptions.py` & `irispie-0.1.3/src/irispie/exceptions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/incidence.py` & `irispie-0.1.3/src/irispie/incidence.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/quantities.py` & `irispie-0.1.3/src/irispie/quantities.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/requirements` & `irispie-0.1.3/src/irispie/requirements`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/session` & `irispie-0.1.3/src/irispie/session`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/tags` & `irispie-0.1.3/src/irispie/tags`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/wrongdoings.py` & `irispie-0.1.3/src/irispie/wrongdoings.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/aldi/adaptations.py` & `irispie-0.1.3/src/irispie/aldi/adaptations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/aldi/differentiators.py` & `irispie-0.1.3/src/irispie/aldi/differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/aldi/express.py~` & `irispie-0.1.3/src/irispie/aldi/express.py~`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/aldi/finite_differentiators.py` & `irispie-0.1.3/src/irispie/aldi/finite_differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/aldi/invariators.py` & `irispie-0.1.3/src/irispie/aldi/invariators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/aldi/maps.py` & `irispie-0.1.3/src/irispie/aldi/maps.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/dataman/databanks.py` & `irispie-0.1.3/src/irispie/dataman/databanks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 """
 
 
 #[
 from __future__ import annotations
-# from IPython import embed
 
 import json as js_
 import copy as co_
 import types as ty_
 import numpy as np_
 import re as re_
 import operator as op_
```

### Comparing `irispie-0.1.2/src/irispie/dataman/dataslabs.py` & `irispie-0.1.3/src/irispie/dataman/dataslabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 #[
 from __future__ import annotations
-# from IPython import embed
 
 import numpy as np_
 from typing import (Self, NoReturn, )
 from collections.abc import (Iterable, )
 
 from . import databanks as db_
 from . import dates as da_
```

### Comparing `irispie-0.1.2/src/irispie/dataman/dates.py` & `irispie-0.1.3/src/irispie/dataman/dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+"""
+Dates, date ranges, and date frequencies
+"""
+
 
 #[
+from __future__ import annotations
+
 import re as _re
 import datetime as _dt
 import enum as _en
 import functools as _ft
 from typing import (Union, Self, Any, Protocol, runtime_checkable, )
 from collections.abc import (Iterable, Callable, )
 from numbers import (Number, )
```

### Comparing `irispie-0.1.2/src/irispie/dataman/exports.py` & `irispie-0.1.3/src/irispie/dataman/exports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Exporting data to CSV sheets
 """
 
 
 #[
 from __future__ import annotations
-# from IPython import embed
 
 import csv as cs_
 import numpy as np_
 import dataclasses as dc_
 import itertools as it_
 
 from ..dataman import dates as da_
```

### Comparing `irispie-0.1.2/src/irispie/dataman/filters.py` & `irispie-0.1.3/src/irispie/dataman/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Univariate time series filters
 """
 
 
 #[
+from __future__ import annotations
+
 from numbers import (Number, )
 from collections.abc import (Iterable, Callable, )
 from types import (EllipsisType, )
 from typing import (Self, )
 import numpy as _np
 
 from ..dataman import (dates as _da, )
```

### Comparing `irispie-0.1.2/src/irispie/dataman/imports.py` & `irispie-0.1.3/src/irispie/dataman/imports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/dataman/imports2.py` & `irispie-0.1.3/src/irispie/dataman/imports2.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/dataman/plotly.py` & `irispie-0.1.3/src/irispie/dataman/plotly.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/dataman/series.py` & `irispie-0.1.3/src/irispie/dataman/series.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/dataman/views.py` & `irispie-0.1.3/src/irispie/dataman/views.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/equators/abc.py` & `irispie-0.1.3/src/irispie/equators/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/equators/plain.py` & `irispie-0.1.3/src/irispie/equators/plain.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/equators/steady.py` & `irispie-0.1.3/src/irispie/equators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/evaluators/printers.py` & `irispie-0.1.3/src/irispie/evaluators/printers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/evaluators/steady.py` & `irispie-0.1.3/src/irispie/evaluators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/fords/descriptors.py` & `irispie-0.1.3/src/irispie/fords/descriptors.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/fords/simulators.py` & `irispie-0.1.3/src/irispie/fords/simulators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/fords/solutions.py` & `irispie-0.1.3/src/irispie/fords/solutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/fords/steadiers.py` & `irispie-0.1.3/src/irispie/fords/steadiers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/fords/systems.py` & `irispie-0.1.3/src/irispie/fords/systems.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/jacobians/abc.py` & `irispie-0.1.3/src/irispie/jacobians/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/jacobians/steady.py` & `irispie-0.1.3/src/irispie/jacobians/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/facade.py` & `irispie-0.1.3/src/irispie/models/facade.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/flags.py` & `irispie-0.1.3/src/irispie/models/flags.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/gettables.py` & `irispie-0.1.3/src/irispie/models/gettables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/invariants.py` & `irispie-0.1.3/src/irispie/models/invariants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/simulatables.py` & `irispie-0.1.3/src/irispie/models/simulatables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/sources.py` & `irispie-0.1.3/src/irispie/models/sources.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/steadiables.py` & `irispie-0.1.3/src/irispie/models/steadiables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/models/variants.py` & `irispie-0.1.3/src/irispie/models/variants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/parsers/common.py` & `irispie-0.1.3/src/irispie/parsers/common.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/parsers/model_source_parser.py` & `irispie-0.1.3/src/irispie/parsers/model_source_parser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/parsers/preparser.py` & `irispie-0.1.3/src/irispie/parsers/preparser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/parsers/pseudofunctions.py` & `irispie-0.1.3/src/irispie/parsers/pseudofunctions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/src/irispie/parsers/substitutions.py` & `irispie-0.1.3/src/irispie/parsers/substitutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/LICENCE` & `irispie-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `irispie-0.1.2/pyproject.toml` & `irispie-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "irispie"
-    version = "0.1.2"
+    version = "0.1.3"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Macroeconomic modeling package"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
```

### Comparing `irispie-0.1.2/PKG-INFO` & `irispie-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irispie
-Version: 0.1.2
+Version: 0.1.3
 Summary: Macroeconomic modeling package
 Project-URL: Homepage, https://github.com/iris-solutions-team/irispie
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/irispie/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 License-File: LICENCE
 Keywords: dsge,economics,forecasting,macroeconomics,modeling,simulation
 Classifier: License :: OSI Approved :: MIT License
```

