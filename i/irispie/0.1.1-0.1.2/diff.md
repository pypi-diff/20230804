# Comparing `tmp/irispie-0.1.1.tar.gz` & `tmp/irispie-0.1.2.tar.gz`

## Comparing `irispie-0.1.1.tar` & `irispie-0.1.2.tar`

### file list

```diff
@@ -1,71 +1,79 @@
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 irispie-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/algorithms/detach-unit-roots.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/dates/Ranger.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/milestones/March-2023.md
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/milestones/iris-gray.png
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.1/docs/series/example.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/__init__.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equations.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/exceptions.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/incidence.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/quantities.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/requirements
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/session
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/tags
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/test.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/wrongdoings.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/adaptations.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/differentiators.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/express.py~
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/finite_differentiators.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/invariators.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/aldi/maps.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/__init__.py
--rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/databanks.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/dataslabs.py
--rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/dates.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/exports.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/filters.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/imports.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/imports2.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/plotly.py
--rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/series.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/dataman/views.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/abc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/plain.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/equators/steady.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/evaluators/printers.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/evaluators/steady.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/__init__.py
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/descriptors.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/simulators.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/solutions.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/steadiers.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/fords/systems.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/jacobians/abc.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/jacobians/steady.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/mixins/userdata.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/__init__.py
--rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/facade.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/flags.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/gettables.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/invariants.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/simulatables.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/sources.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/steadiables.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/models/variants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/common.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/model_source_parser.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/preparser.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/pseudofunctions.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/shifts.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.1/src/irispie/parsers/substitutions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.1/tests/.gitkeep
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.1/LICENCE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.1/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 irispie-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 irispie-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/app.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/appearance.json
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/hotkeys.json
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/.obsidian/workspace.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/algorithms/detach-unit-roots.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/architecture/Untitled.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/architecture/steady.canvas
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/dates/Ranger.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/milestones/March-2023.md
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/milestones/iris-gray.png
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.2/docs/series/example.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/__init__.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equations.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/exceptions.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/incidence.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/quantities.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/requirements
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/session
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/tags
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/wrongdoings.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/adaptations.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/differentiators.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/express.py~
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/finite_differentiators.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/invariators.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/aldi/maps.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/__init__.py
+-rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/databanks.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/dataslabs.py
+-rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/dates.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/exports.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/filters.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/imports.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/imports2.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/plotly.py
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/series.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/dataman/views.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/abc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/plain.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/equators/steady.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/evaluators/printers.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/evaluators/steady.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/__init__.py
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/descriptors.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/simulators.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/solutions.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/steadiers.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/fords/systems.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/jacobians/abc.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/jacobians/steady.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/mixins/userdata.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/__init__.py
+-rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/facade.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/flags.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/gettables.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/invariants.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/simulatables.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/sources.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/steadiables.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/models/variants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/common.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/model_source_parser.py
+-rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/preparser.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/pseudofunctions.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/shifts.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.2/src/irispie/parsers/substitutions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.2/tests/.gitkeep
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.2/tests/dataman/series/hpf_test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.2/LICENCE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.2/README.md
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 irispie-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 irispie-0.1.2/PKG-INFO
```

### Comparing `irispie-0.1.1/.github/workflows/publish-to-pypi.yml` & `irispie-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 jobs:
   deploy:
     name: Create and upload dist to PYPI
     runs-on: ubuntu-latest
     steps:
-      
+
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
 
       - name: Install build and twine
         run: |
@@ -26,26 +26,30 @@
         uses: actions/checkout@master
         with:
           fetch-depth: 0
           ref: master
           path: .
 
       - name: Capture version from pyproject.toml
-        id: captureversion
+        id: capture-version
         run: |
+          grep -m 1 version pyproject.toml
+          grep -m 1 version pyproject.toml | tr -d '[a-z=" ]'
           version=$(grep -m 1 version pyproject.toml | tr -d '[a-z=" ]')
+          echo $version
           echo "version=$version" >> "$GITHUB_OUTPUT"
 
       - name: Build dist files
         run: |
-          echo "Building version ${{ steps.captureversion.version }}"
+          echo "Building version ${{ steps.capture-version.outputs.version }}"
           python -m build
-    
+
       - name: Upload
         run: |
           python -m twine upload dist/* -r pypi -u __token__ -p ${{ secrets.PYPI_API_TOKEN }}
-          
+
       - name: Create artifacts
         uses: actions/upload-artifact@master
-        with: 
-          name: dist-${{ steps.captureversion.version }}
+        with:
+          name: dist-${{ steps.capture-version.outputs.version }}
           path: dist/*
+
```

### Comparing `irispie-0.1.1/docs/algorithms/detach-unit-roots.md` & `irispie-0.1.2/docs/algorithms/detach-unit-roots.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/docs/milestones/March-2023.md` & `irispie-0.1.2/docs/milestones/March-2023.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/docs/milestones/iris-gray.png` & `irispie-0.1.2/docs/milestones/iris-gray.png`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/docs/series/example.py` & `irispie-0.1.2/docs/series/example.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/equations.py` & `irispie-0.1.2/src/irispie/equations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/exceptions.py` & `irispie-0.1.2/src/irispie/exceptions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/incidence.py` & `irispie-0.1.2/src/irispie/incidence.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/quantities.py` & `irispie-0.1.2/src/irispie/quantities.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/requirements` & `irispie-0.1.2/src/irispie/requirements`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/session` & `irispie-0.1.2/src/irispie/session`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/tags` & `irispie-0.1.2/src/irispie/tags`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/wrongdoings.py` & `irispie-0.1.2/src/irispie/wrongdoings.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/aldi/adaptations.py` & `irispie-0.1.2/src/irispie/aldi/adaptations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/aldi/differentiators.py` & `irispie-0.1.2/src/irispie/aldi/differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/aldi/express.py~` & `irispie-0.1.2/src/irispie/aldi/express.py~`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/aldi/finite_differentiators.py` & `irispie-0.1.2/src/irispie/aldi/finite_differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/aldi/invariators.py` & `irispie-0.1.2/src/irispie/aldi/invariators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/aldi/maps.py` & `irispie-0.1.2/src/irispie/aldi/maps.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/dataman/databanks.py` & `irispie-0.1.2/src/irispie/dataman/databanks.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/dataman/dataslabs.py` & `irispie-0.1.2/src/irispie/dataman/dataslabs.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/dataman/dates.py` & `irispie-0.1.2/src/irispie/dataman/dates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 
 #[
-from __future__ import annotations
-
-import re as re_
-import datetime as dt_
-import enum as en_
-import functools as ft_
-from typing import (NoReturn, Union, Self, Any, Protocol, runtime_checkable, )
+import re as _re
+import datetime as _dt
+import enum as _en
+import functools as _ft
+from typing import (Union, Self, Any, Protocol, runtime_checkable, )
 from collections.abc import (Iterable, Callable, )
 from numbers import (Number, )
 #]
 
 
 __all__ = [
     "Frequency",
     "yy", "hh", "qq", "mm", "dd", "ii",
     "Ranger", "start", "end",
     "dater_from_sdmx_string",
+    "dater_from_iso_string",
 ]
 
 
-class Frequency(en_.IntEnum):
+class Frequency(_en.IntEnum):
     """
     Enumeration of date frequencies
     """
     #[
     INTEGER = 0
     YEARLY = 1
     HALFYEARLY = 2
@@ -74,58 +73,58 @@
 }
 
 
 BASE_YEAR = 2020
 
 
 @runtime_checkable
-class ResolutionContextProtocol(Protocol):
+class ResolutionContextProtocol(Protocol, ):
     """
     Context protocol for contextual date resolution
     """
     start_date = ...
     end_date = ...
 
 
 @runtime_checkable
-class ResolvableProtocol(Protocol):
+class ResolvableProtocol(Protocol, ):
     """
     Contextual date protocol
     """
     needs_resolve = ...
     def resolve(self, context: ResolutionContextProtocol) -> Any: ...
 
 
 def _check_daters(first, second) -> None:
     if type(first) is not type(second):
         raise Exception("Dates must be the same date frequency")
 
 
-def _check_daters_decorate(func: Callable) -> Callable:
+def _check_daters_decorate(func: Callable, ) -> Callable:
     def wrapper(*args, **kwargs):
-        _check_daters(args[0], args[1])
-        return func(*args, **kwargs)
+        _check_daters(args[0], args[1], )
+        return func(*args, **kwargs, )
     return wrapper
 
 
-def _check_offset(offset) -> None:
-    if not isinstance(offset, int):
+def _check_offset(offset, ) -> None:
+    if not isinstance(offset, int, ):
         raise Exception("Date offset must be an integer")
 
 
 def _check_offset_decorator(func: Callable) -> Callable:
     def wrapper(*args, **kwargs):
         _check_offset(args[1])
         return func(*args, **kwargs)
     return wrapper
 
 
-def _remove_blanks_decorate(func: Callable) -> Callable:
-    def wrapper(*args, **kwargs):
-        return func(*args, **kwargs).replace(" ","")
+def _remove_blanks_decorate(func: Callable,) -> Callable:
+    def wrapper(*args, **kwargs, ):
+        return func(*args, **kwargs, ).replace(" ", "", )
     return wrapper
 
 
 class RangeableMixin:
     #[
     def __rshift__(self, end_date: Self) -> Ranger:
         """
@@ -145,26 +144,31 @@
         self: Self,
         /,
         position: Literal["start"] | Literal["center"] | Literal["end"] = "start",
     ) -> str:
         year, month, day = self.to_ymd()
         return f"{year:04g}-{month:02g}-{day:02g}"
 
-    to_plotly_date = ft_.partialmethod(to_iso_string, position="center")
+    @classmethod
+    def from_iso_string(cls: type, iso_string: str, ) -> Self:
+        year, month, day = iso_string.split("-", )
+        return cls.from_ymd(int(year), int(month), int(day), )
+
+    to_plotly_date = _ft.partialmethod(to_iso_string, position="center")
     #]
 
 
-class Dater(RangeableMixin):
+class Dater(RangeableMixin, ):
     """
     """
     #[
     frequency = None
     needs_resolve = False
 
-    def __init__(self, serial=0) -> NoReturn:
+    def __init__(self, serial=0) -> None:
         self.serial = int(serial)
 
     def get_distance_from_origin(self) -> int:
         return self.serial - self.origin
 
     def resolve(self, context: ResolutionContextProtocol) -> Self:
         return self
@@ -263,40 +267,40 @@
     #]
 
 
 class DailyDater(Dater, IsoMixin):
     #[
     frequency: Frequency = Frequency.DAILY
     needs_resolve = False
-    origin = dt_.date(BASE_YEAR, 1, 1).toordinal()
+    origin = _dt.date(BASE_YEAR, 1, 1).toordinal()
 
     @classmethod
     def from_ymd(cls: type, year: int, month: int=1, day: int=1) -> Self:
-        serial = dt_.date(year, month, day).toordinal()
+        serial = _dt.date(year, month, day).toordinal()
         return cls(serial)
 
     @classmethod
     def from_year_period(cls, year: int, period: int) -> Self:
-        boy_serial = dt_.date(year, 1, 1).toordinal()
+        boy_serial = _dt.date(year, 1, 1).toordinal()
         serial = boy_serial + int(period) - 1
         return cls(serial)
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> DailyDater:
         year, month, day = sdmx_string.split("-")
         return cls.from_ymd(int(year), int(month), int(day))
 
     def to_year_period(self: Self) -> tuple[int, int]:
-        boy_serial = dt_.date(dt_.date.fromordinal(self.serial).year, 1, 1)
+        boy_serial = _dt.date(_dt.date.fromordinal(self.serial).year, 1, 1)
         per = self.serial - boy_serial + 1
-        year = dt_.date.fromordinal(self.serial).year
+        year = _dt.date.fromordinal(self.serial).year
         return year, per
 
     def to_ymd(self: Self, /, **kwargs) -> tuple[int, int, int]:
-        py_date = dt_.date.fromordinal(self.serial)
+        py_date = _dt.date.fromordinal(self.serial)
         return py_date.year, py_date.month, py_date.day
 
     def __str__(self) -> str:
         year, month, day = self.to_ymd()
         letter = self.frequency.letter
         return self.frequency.sdmx_format.format(year=year, month=month, day=day, letter=letter)
 
@@ -306,27 +310,31 @@
     #]
 
 
 def _serial_from_ypf(year: int, per: int, freq: int) -> int:
     return int(year)*int(freq) + int(per) - 1
 
 
-class RegularDaterMixin:
+class RegularDaterMixin(IsoMixin, ):
     #[
     @classmethod
     def from_year_period(
             cls: type,
             year: int,
             per: int | str = 1,
         ) -> Self:
         if per=="end":
             per = cls.frequency.value
         new_serial = _serial_from_ypf(year, per, cls.frequency.value)
         return cls(new_serial)
 
+    @classmethod
+    def from_ymd(cls, year: int, month: int=1, day: int=1, ) -> YearlyDater:
+        return cls.from_year_period(year, cls.month_to_period(month, ), )
+
     def to_year_period(self) -> tuple[int, int]:
         return self.serial//self.frequency.value, self.serial%self.frequency.value+1
 
     def get_year(self) -> int:
         return self.to_year_period()[0]
 
     def to_ymd(
@@ -341,15 +349,15 @@
     def __str__(self) -> str:
         year, per = self.to_year_period()
         letter = self.frequency.letter
         return self.frequency.sdmx_format.format(year=year, per=per, letter=letter)
     #]
 
 
-class YearlyDater(Dater, RegularDaterMixin, IsoMixin): 
+class YearlyDater(Dater, RegularDaterMixin, ): 
     #[
     frequency: Frequency = Frequency.YEARLY
     needs_resolve: bool = False
     origin = _serial_from_ypf(BASE_YEAR, 1, Frequency.YEARLY)
     month_day_resolution = {
         "start": {1: (1, 1)},
         "center": {1: (6, 30)},
@@ -358,18 +366,22 @@
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> YearlyDater:
         return cls(int(sdmx_string))
 
     @_remove_blanks_decorate
     def __repr__(self) -> str: return f"yy({self.get_year()})"
+
+    @staticmethod
+    def month_to_period(month: int, ) -> int:
+        return 1
     #]
 
 
-class HalfyearlyDater(Dater, RegularDaterMixin, IsoMixin):
+class HalfyearlyDater(Dater, RegularDaterMixin, ):
     #[
     frequency: Frequency = Frequency.HALFYEARLY
     needs_resolve: bool = False
     origin = _serial_from_ypf(BASE_YEAR, 1, Frequency.HALFYEARLY)
     month_day_resolution = {
         "start": {1: (1, 1), 2: (7, 1)},
         "center": {1: (3, 15), 2: (9, 15)},
@@ -399,18 +411,22 @@
     def get_month(
         self,
         /,
         position: Literal["start"] | Literal["center"] | Literal["end"] = "center",
     ) -> int:
         _, per = self.to_year_period()
         return month_resolution[position][per]
+
+    @staticmethod
+    def month_to_period(month: int, ) -> int:
+        return 1+((month-1)//6)
     #]
 
 
-class QuarterlyDater(Dater, RegularDaterMixin, IsoMixin):
+class QuarterlyDater(Dater, RegularDaterMixin, ):
     frequency: Frequency = Frequency.QUARTERLY
     needs_resolve: bool = False
     origin = _serial_from_ypf(BASE_YEAR, 1, Frequency.QUARTERLY)
     month_day_resolution = {
         "start": {1: (1, 1), 2: (4, 1), 3: (7, 1), 4: (10, 1)},
         "center": {1: (2, 15), 2: (5, 15), 3: (8, 15), 4: (11, 15)},
         "end": {1: (3, 30), 2: (5, 31), 3: (8, 31), 4: (11, 30)},
@@ -421,16 +437,20 @@
         year, quarter = sdmx_string.split("-")
         quarter = quarter.upper().replace("Q", "")
         return cls.from_year_period(int(year), int(quarter))
 
     @_remove_blanks_decorate
     def __repr__(self) -> str: return f"qq{self.to_year_period()}"
 
+    @staticmethod
+    def month_to_period(month: int, ) -> int:
+        return 1+((month-1)//3)
+
 
-class MonthlyDater(Dater, RegularDaterMixin, IsoMixin):
+class MonthlyDater(Dater, RegularDaterMixin, ):
     #[
     frequency: Frequency = Frequency.MONTHLY
     needs_resolve: bool = False
     origin = _serial_from_ypf(BASE_YEAR, 1, Frequency.MONTHLY)
     month_day_resolution = {
         "start": {1: (1, 1), 2: (2, 1), 3: (2, 1), 4: (4, 1), 5: (5, 1), 6: (6, 1), 7: (7, 1), 8: (8, 1), 9: (9, 1), 10: (10, 1), 11: (11, 1), 12: (12, 1)},
         "center": {1: (1, 15), 2: (2, 15), 3: (2, 15), 4: (4, 15), 5: (5, 15), 6: (6, 15), 7: (7, 15), 8: (8, 15), 9: (9, 15), 10: (10, 15), 11: (11, 15), 12: (12, 15)},
@@ -440,14 +460,18 @@
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> MonthlyDater:
         year, month = sdmx_string.split("-")
         return cls.from_year_period(int(year), int(month))
 
     @_remove_blanks_decorate
     def __repr__(self) -> str: return f"mm{self.to_year_period()}"
+
+    @staticmethod
+    def month_to_period(month: int, ) -> int:
+        return month
     #]
 
 
 yy = YearlyDater.from_year_period
 
 hh = HalfyearlyDater.from_year_period
 
@@ -471,15 +495,15 @@
     #[
     def __init__(
         self, 
         start_date: Dater|None =None,
         end_date: Dater|None =None,
         step: int=1,
         /
-    ) -> NoReturn:
+    ) -> None:
         """
         Date range constructor
         """
         start_date = resolve_dater_or_integer(start_date)
         end_date = resolve_dater_or_integer(end_date)
         self._start_date = start_date if start_date is not None else start
         self._end_date = end_date if end_date is not None else end
@@ -635,31 +659,45 @@
     Frequency.HALFYEARLY: HalfyearlyDater,
     Frequency.QUARTERLY: QuarterlyDater,
     Frequency.MONTHLY: MonthlyDater,
     Frequency.DAILY: DailyDater,
 }
 
 
-def dater_from_sdmx_string(freq: Frequency, sdmx_string: str) -> Dater:
+def dater_from_sdmx_string(freq: Frequency, sdmx_string: str, ) -> Dater:
     """
     """
     return _DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_sdmx_string(sdmx_string)
 
 
+def dater_from_iso_string(freq: Frequency, iso_string: str, ) -> Dater:
+    """
+    """
+    return _DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_iso_string(iso_string)
+
+
 _FREQUENCY_FROM_STRING_RESOLUTION = {
     "I": Frequency.INTEGER,
     "Y": Frequency.YEARLY,
     "H": Frequency.HALFYEARLY,
     "Q": Frequency.QUARTERLY,
     "M": Frequency.MONTHLY,
     "W": Frequency.WEEKLY,
     "D": Frequency.DAILY,
 }
 
 
 def frequency_from_string(text: str) -> Frequency:
     """
     """
-    first_letter_match = re_.search("[A-Z]", text.upper() + "X")
+    first_letter_match = _re.search("[A-Z]", text.upper() + "X")
     return _FREQUENCY_FROM_STRING_RESOLUTION.get(first_letter_match.group(0), Frequency.UNKNOWN)
 
 
+def get_encompassing_range(*args: ResolutionContextProtocol, ) -> Ranger:
+    start_dates = [x.start_date for x in args if hasattr(x, "start_date") and x.start_date]
+    end_dates = [x.end_date for x in args if hasattr(x, "end_date") and x.end_date]
+    start_date = min(start_dates) if start_dates else None
+    end_date = max(end_dates) if end_dates else None
+    return Ranger(start_date, end_date)
+
+
```

### Comparing `irispie-0.1.1/src/irispie/dataman/exports.py` & `irispie-0.1.2/src/irispie/dataman/exports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/dataman/imports.py` & `irispie-0.1.2/src/irispie/dataman/imports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/dataman/imports2.py` & `irispie-0.1.2/src/irispie/dataman/imports2.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/dataman/plotly.py` & `irispie-0.1.2/src/irispie/dataman/plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,7 +65,8 @@
             figure.add_vline(xline)
         return figure
     #]
 
 
 make_subplots = ps.make_subplots
 
+
```

### Comparing `irispie-0.1.1/src/irispie/dataman/series.py` & `irispie-0.1.2/src/irispie/dataman/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 """
 
 #[
 from __future__ import annotations
 # from IPython import embed
 
 from numbers import Number
-from collections.abc import Iterable, Callable
-from typing import Self, TypeAlias, NoReturn
-from types import EllipsisType
+from collections.abc import (Iterable, Callable, )
+from typing import (Self, TypeAlias, )
+from types import (EllipsisType, )
 import numpy as np_
 import itertools as it_
 import copy as co_
 
 from ..dataman.dates import (Dater, Ranger, date_index, ResolvableProtocol, )
 from ..dataman import (views as vi_, )
-from ..dataman import (dates as da_, )
+from ..dataman import (dates as _da, )
 from ..dataman import (filters as fi_, )
 from ..dataman import (plotly as pl_, )
 from ..mixins import (userdata as ud_, )
 #]
 
 
 FUNCTION_ADAPTATIONS = ["log", "exp", "sqrt", "maximum", "minimum"] + ["cumsum"] + ["maxi", "mini", "mean", "median"]
@@ -110,15 +110,15 @@
 
     @property
     def end_date(self):
         return self.start_date + self.data.shape[0] - 1 if self.start_date else None
 
     @property
     def frequency(self):
-        return self.start_date.frequency if self.start_date is not None else da_.Frequency.UNKNOWN
+        return self.start_date.frequency if self.start_date is not None else _da.Frequency.UNKNOWN
 
     @classmethod
     def from_dates_and_data(
         cls,
         dates: Iterable[Dater],
         data: np_.ndarray,
         /,
@@ -132,15 +132,15 @@
     def from_start_date_and_data(
         cls,
         start_date: Dater,
         data: np_.ndarray,
         /,
         **kwargs,
     ) -> Self:
-        num_columns = data.shape[1]
+        num_columns = data.shape[1] if hasattr(data, "shape") else 1
         self = cls(num_columns=num_columns, **kwargs)
         self.start_date = start_date
         self.data = data
         return self
 
     @classmethod
     def from_func(
@@ -236,15 +236,15 @@
         column = column if column and column<self.data.shape[1] else 0
         return self.get_data(dates, column)
 
     def extract_columns(
         self,
         columns,
         /,
-    ) -> NoReturn:
+    ) -> None:
         if not isinstance(columns, Iterable):
             columns = (columns, )
         columns = [ c for c in columns ]
         self.data = self.data[:, columns]
         self.column_titles = [ self.column_titles[c] for c in columns ]
 
     def set_start_date(
@@ -307,30 +307,30 @@
         if not isinstance(index, tuple):
             index = (index, None, )
         return self.set_data(index[0], data, index[1])
 
     def hstack(self, *args):
         if not args:
             return co_.deepcopy(self)
-        encompassing_range = self._get_encompassing_range(*args)
+        encompassing_range = _da.get_encompassing_range(self, *args)
         new_data = self.get_data(encompassing_range)
         add_data = (
             x.get_data(encompassing_range) if hasattr(x, "get_data") else _create_data_from_number(x, encompassing_range, self.data_type)
             for x in args
         )
         new_data = np_.hstack((new_data, *add_data))
         new = Series(num_columns=new_data.shape[1]);
         new.set_data(encompassing_range, new_data)
         return new
 
     def clip(
         self,
         new_start_date: Dater | None,
         new_end_date: Dater | None,
-    ) -> NoReturn:
+    ) -> None:
         if new_start_date is None or new_start_date < self.start_date:
             new_start_date = self.start_date
         if new_end_date is None or new_end_date > self.end_date:
             new_end_date = self.end_date
         if new_start_date == self.start_date and new_end_date == self.end_date:
             return
         self.start_date = new_start_date
@@ -389,21 +389,14 @@
 
     def __lshift__(self, other):
         return co_.deepcopy(self).overlay_by_range(other, )
 
     def __rshift__(self, other):
         return co_.deepcopy(other).overlay_by_range(self, )
 
-    def _get_encompassing_range(*args) -> Ranger:
-        start_dates = [x.start_date for x in args if hasattr(x, "start_date") and x.start_date]
-        end_dates = [x.end_date for x in args if hasattr(x, "end_date") and x.end_date]
-        start_date = min(start_dates) if start_dates else None
-        end_date = max(end_dates) if end_dates else None
-        return Ranger(start_date, end_date)
-
     def _trim(self):
         if self.data.size==0:
             return self.reset()
         num_leading = _get_num_leading_missing_rows(self.data, self._test_missing_period)
         if num_leading == self.data.shape[0]:
             return self.reset()
         num_trailing = _get_num_leading_missing_rows(self.data[::-1], self._test_missing_period)
@@ -548,15 +541,15 @@
         else:
             raise Exception("Function applied on a time series resulted in a data array with an unexpected shape")
 
     def _binop(self, other, func, /, ):
         if not isinstance(other, type(self)):
             unop_func = lambda data: func(data, other)
             return apply(self, unop_func)
-        encompassing_range = self._get_encompassing_range(self, other)
+        encompassing_range = _da.get_encompassing_range(self, other)
         self_data = self.get_data(encompassing_range)
         other_data = other.get_data(encompassing_range)
         new = Series()
         new.start_date = encompassing_range[0]
         new.data = func(self_data, other_data)
         new._trim()
         return new
@@ -592,15 +585,14 @@
 
 # def apply(x, func: Callable, /, *args, **kwargs) -> object:
     # if isinstance(x, Series):
         # return x.apply(func, *args, **kwargs)
     # else:
         # return func(x, *args, **kwargs)
 
-
 def hstack(first, *args) -> Self:
     return first.hstack(*args)
 
 
 def _create_data_from_number(
     number: Number,
     range: Ranger,
```

### Comparing `irispie-0.1.1/src/irispie/dataman/views.py` & `irispie-0.1.2/src/irispie/dataman/views.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/equators/abc.py` & `irispie-0.1.2/src/irispie/equators/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/equators/plain.py` & `irispie-0.1.2/src/irispie/equators/plain.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/equators/steady.py` & `irispie-0.1.2/src/irispie/equators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/evaluators/printers.py` & `irispie-0.1.2/src/irispie/evaluators/printers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/evaluators/steady.py` & `irispie-0.1.2/src/irispie/evaluators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/fords/descriptors.py` & `irispie-0.1.2/src/irispie/fords/descriptors.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/fords/simulators.py` & `irispie-0.1.2/src/irispie/fords/simulators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/fords/solutions.py` & `irispie-0.1.2/src/irispie/fords/solutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/fords/steadiers.py` & `irispie-0.1.2/src/irispie/fords/steadiers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/fords/systems.py` & `irispie-0.1.2/src/irispie/fords/systems.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/jacobians/abc.py` & `irispie-0.1.2/src/irispie/jacobians/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/jacobians/steady.py` & `irispie-0.1.2/src/irispie/jacobians/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/facade.py` & `irispie-0.1.2/src/irispie/models/facade.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/flags.py` & `irispie-0.1.2/src/irispie/models/flags.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/gettables.py` & `irispie-0.1.2/src/irispie/models/gettables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/invariants.py` & `irispie-0.1.2/src/irispie/models/invariants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/simulatables.py` & `irispie-0.1.2/src/irispie/models/simulatables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/sources.py` & `irispie-0.1.2/src/irispie/models/sources.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/steadiables.py` & `irispie-0.1.2/src/irispie/models/steadiables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/models/variants.py` & `irispie-0.1.2/src/irispie/models/variants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/parsers/common.py` & `irispie-0.1.2/src/irispie/parsers/common.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/parsers/model_source_parser.py` & `irispie-0.1.2/src/irispie/parsers/model_source_parser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/parsers/preparser.py` & `irispie-0.1.2/src/irispie/parsers/preparser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/parsers/pseudofunctions.py` & `irispie-0.1.2/src/irispie/parsers/pseudofunctions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/src/irispie/parsers/substitutions.py` & `irispie-0.1.2/src/irispie/parsers/substitutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/LICENCE` & `irispie-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `irispie-0.1.1/pyproject.toml` & `irispie-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "irispie"
-    version = "0.1.1"
+    version = "0.1.2"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Macroeconomic modeling package"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
+    keywords = [
+        "macroeconomics",
+        "economics",
+        "modeling",
+        "simulation",
+        "forecasting",
+        "dsge",
+    ]
+    dependencies = [
+        "numpy >= 1.25",
+        "scipy >= 1.11",
+    ]
 
 [project.urls]
     "Homepage" = "https://github.com/iris-solutions-team/irispie"
     "Bug Tracker" = "https://github.com/iris-solutions-team/irispie/issues"
```

### Comparing `irispie-0.1.1/PKG-INFO` & `irispie-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: irispie
-Version: 0.1.1
+Version: 0.1.2
 Summary: Macroeconomic modeling package
 Project-URL: Homepage, https://github.com/iris-solutions-team/irispie
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/irispie/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 License-File: LICENCE
+Keywords: dsge,economics,forecasting,macroeconomics,modeling,simulation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
+Requires-Dist: numpy>=1.25
+Requires-Dist: scipy>=1.11
 Description-Content-Type: text/markdown
 
 # Iris Pie
 
 Macroeconomic modeling package for Python
```

