# Comparing `tmp/irispie-0.1.4.tar.gz` & `tmp/irispie-0.1.5.tar.gz`

## Comparing `irispie-0.1.4.tar` & `irispie-0.1.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 irispie-0.1.4/.github/workflows/test.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/app.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/appearance.json
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/core-plugins.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/hotkeys.json
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/.obsidian/workspace.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/algorithms/detach-unit-roots.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/architecture/Untitled.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/architecture/steady.canvas
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/dates/Ranger.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/milestones/March-2023.md
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/milestones/iris-gray.png
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.4/docs/series/example.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/__init__.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equations.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/exceptions.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/incidence.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/quantities.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/requirements
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/session
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/tags
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/wrongdoings.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/adaptations.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/differentiators.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/express.py~
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/finite_differentiators.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/invariators.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/aldi/maps.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/databanks.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/dataslabs.py
--rw-r--r--   0        0        0    20362 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/dates.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/exports.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/filters.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/imports.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/imports2.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/plotly.py
--rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/series.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/dataman/views.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/abc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/plain.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/equators/steady.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/evaluators/printers.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/evaluators/steady.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/__init__.py
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/descriptors.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/simulators.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/solutions.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/steadiers.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/fords/systems.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/jacobians/abc.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/jacobians/steady.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/mixins/userdata.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/__init__.py
--rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/facade.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/flags.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/gettables.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/invariants.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/simulatables.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/sources.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/steadiables.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/models/variants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/common.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/model_source_parser.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/preparser.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/pseudofunctions.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/shifts.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.4/src/irispie/parsers/substitutions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.4/tests/.gitkeep
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.4/tests/dataman/series/hpf_test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.4/LICENCE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.4/README.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 irispie-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 irispie-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 irispie-0.1.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/.obsidian/app.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/.obsidian/appearance.json
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/.obsidian/hotkeys.json
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/.obsidian/workspace.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/algorithms/detach-unit-roots.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/architecture/Untitled.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/architecture/steady.canvas
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/dates/Ranger.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/milestones/March-2023.md
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/milestones/iris-gray.png
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.5/docs/series/example.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/__init__.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/equations.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/exceptions.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/incidence.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/quantities.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/requirements
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/session
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/tags
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/wrongdoings.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/aldi/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/aldi/adaptations.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/aldi/differentiators.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/aldi/express.py~
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/aldi/finite_differentiators.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/aldi/invariators.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/aldi/maps.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/databanks.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/dataslabs.py
+-rw-r--r--   0        0        0    20362 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/dates.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/exports.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/filters.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/imports.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/imports2.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/plotly.py
+-rw-r--r--   0        0        0    18606 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/series.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/dataman/views.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/equators/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/equators/abc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/equators/plain.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/equators/steady.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/evaluators/printers.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/evaluators/steady.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/fords/__init__.py
+-rw-r--r--   0        0        0    15846 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/fords/descriptors.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/fords/simulators.py
+-rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/fords/solutions.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/fords/steadiers.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/fords/systems.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/jacobians/abc.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/jacobians/steady.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/mixins/userdata.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/__init__.py
+-rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/facade.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/flags.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/gettables.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/invariants.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/simulatables.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/sources.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/steadiables.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/models/variants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/parsers/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/parsers/common.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/parsers/model_source_parser.py
+-rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/parsers/preparser.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/parsers/pseudofunctions.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/parsers/shifts.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.5/src/irispie/parsers/substitutions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.5/tests/.gitkeep
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.5/tests/dataman/series/hpf_test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.5/LICENCE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.5/README.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 irispie-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 irispie-0.1.5/PKG-INFO
```

### Comparing `irispie-0.1.4/.github/workflows/publish-to-pypi.yml` & `irispie-0.1.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/docs/.obsidian/core-plugins-migration.json` & `irispie-0.1.5/docs/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/docs/.obsidian/workspace.json` & `irispie-0.1.5/docs/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/docs/algorithms/detach-unit-roots.md` & `irispie-0.1.5/docs/algorithms/detach-unit-roots.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/docs/milestones/March-2023.md` & `irispie-0.1.5/docs/milestones/March-2023.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/docs/milestones/iris-gray.png` & `irispie-0.1.5/docs/milestones/iris-gray.png`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/docs/series/example.py` & `irispie-0.1.5/docs/series/example.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/equations.py` & `irispie-0.1.5/src/irispie/equations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/exceptions.py` & `irispie-0.1.5/src/irispie/exceptions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/incidence.py` & `irispie-0.1.5/src/irispie/incidence.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/quantities.py` & `irispie-0.1.5/src/irispie/quantities.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/requirements` & `irispie-0.1.5/src/irispie/requirements`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/session` & `irispie-0.1.5/src/irispie/session`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/tags` & `irispie-0.1.5/src/irispie/tags`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/wrongdoings.py` & `irispie-0.1.5/src/irispie/wrongdoings.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/aldi/adaptations.py` & `irispie-0.1.5/src/irispie/aldi/adaptations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/aldi/differentiators.py` & `irispie-0.1.5/src/irispie/aldi/differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/aldi/express.py~` & `irispie-0.1.5/src/irispie/aldi/express.py~`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/aldi/finite_differentiators.py` & `irispie-0.1.5/src/irispie/aldi/finite_differentiators.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Calculate first derivatives of a custom function using finite approximation
 """
 
 
 #[
 from __future__ import annotations
 
-from typing import (NoReturn, Callable, )
+from typing import (Callable, )
 import numpy as np_
 import copy as co_
 
 from ..aldi import (differentiators as ad_, )
 #]
```

### Comparing `irispie-0.1.4/src/irispie/aldi/invariators.py` & `irispie-0.1.5/src/irispie/aldi/invariators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 """
 
 
 #[
 from __future__ import annotations
 
-from typing import (Self, NoReturn, )
+from typing import (Self, )
 from numbers import (Number, )
 import numpy as np_
 
 from ..aldi import (differentiators as ad_, )
 from .. import (incidence as in_, )
 #]
 
@@ -18,15 +18,15 @@
     """
     Atomic value for invariance testing
     """
     _data_context: np_.ndarray | None = None
     _logly_context: dict[int, bool] | None = None
     _is_atom: bool = True
     #[
-    def __init__(self) -> NoReturn:
+    def __init__(self) -> None:
         """
         """
         self._diff = None
         self._invariant = None
         self._logly = None
         self._logly_index = None
```

### Comparing `irispie-0.1.4/src/irispie/aldi/maps.py` & `irispie-0.1.5/src/irispie/aldi/maps.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,58 +3,58 @@
 sparse) Jacobian matrix
 """
 
 
 #[
 from __future__ import annotations
 
-from typing import (Self, NoReturn, Any, )
+from typing import (Self, Any, )
 from collections.abc import (Iterable, )
 import itertools as it_
 import dataclasses as dc_
 #]
 
 
 @dc_.dataclass
 class ArrayMap:
     """
     """
     lhs: tuple[list[int], list[int]] | None = None
     rhs: tuple[list[int], list[int]] | None = None
     #[
-    def __init__(self, /, ) -> NoReturn:
+    def __init__(self, /, ) -> None:
         self.lhs = ([], [])
         self.rhs = ([], [])
 
     def __len__(self, /, ) -> int:
         return len(self.lhs[0])
 
     def append(
         self,
         lhs: tuple[int, int], 
         rhs: tuple[int, int],
         /
-    ) -> NoReturn:
+    ) -> None:
         """
         """
         self.lhs[0].append(lhs[0])
         self.lhs[1].append(lhs[1])
         self.rhs[0].append(rhs[0])
         self.rhs[1].append(rhs[1])
 
     def merge_with(
         self,
         other: Self,
-    ) -> NoReturn:
+    ) -> None:
         """
         """
         self.lhs = (self.lhs[0]+other.lhs[0], self.lhs[1]+other.lhs[1])
         self.rhs = (self.rhs[0]+other.rhs[0], self.rhs[1]+other.rhs[1])
 
-    def remove_nones(self) -> NoReturn:
+    def remove_nones(self) -> None:
         """
         Remove any map entry that has a None for the row index on the LHS
         """
         if not self.lhs[0]:
             return
         zipped_pruned = [
             i for i in zip(self.lhs[0], self.lhs[1], self.rhs[0], self.rhs[1])
```

### Comparing `irispie-0.1.4/src/irispie/dataman/databanks.py` & `irispie-0.1.5/src/irispie/dataman/databanks.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/dataman/dataslabs.py` & `irispie-0.1.5/src/irispie/dataman/dataslabs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 #[
 from __future__ import annotations
 
 import numpy as np_
-from typing import (Self, NoReturn, )
+from typing import (Self, )
 from collections.abc import (Iterable, )
 
 from . import databanks as db_
 from . import dates as da_
 from . import series as se_
 #]
 
@@ -56,15 +56,15 @@
         self.missing_names = missing_names
         return self
 
     def remove_columns(
         self,
         remove: int,
         /,
-    ) -> NoReturn:
+    ) -> None:
         """
         """
         if remove > 0:
             self.data = self.data[:, remove:]
             self.column_dates = self.column_dates[remove:]
         elif remove < 0:
             self.data = self.data[:, :remove]
```

### Comparing `irispie-0.1.4/src/irispie/dataman/dates.py` & `irispie-0.1.5/src/irispie/dataman/dates.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/dataman/exports.py` & `irispie-0.1.5/src/irispie/dataman/exports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/dataman/filters.py` & `irispie-0.1.5/src/irispie/dataman/filters.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/dataman/imports.py` & `irispie-0.1.5/src/irispie/dataman/imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Databank imports
 """
 
 
 #[
 from __future__ import annotations
-# from IPython import embed
 
-from typing import (Self, NoReturn, )
+from typing import (Self, )
 from collections.abc import (Iterable, Callable, )
 import csv as cs_
 import numpy as np_
 import dataclasses as dc_
 
 from ..dataman import (dates as dd_, series as ds_, )
 #]
```

### Comparing `irispie-0.1.4/src/irispie/dataman/imports2.py` & `irispie-0.1.5/src/irispie/dataman/imports2.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/dataman/plotly.py` & `irispie-0.1.5/src/irispie/dataman/plotly.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/dataman/series.py` & `irispie-0.1.5/src/irispie/dataman/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Time series
 """
 
 #[
 from __future__ import annotations
-# from IPython import embed
 
 from numbers import Number
 from collections.abc import (Iterable, Callable, )
 from typing import (Self, TypeAlias, )
 from types import (EllipsisType, )
 import numpy as np_
 import itertools as it_
```

### Comparing `irispie-0.1.4/src/irispie/dataman/views.py` & `irispie-0.1.5/src/irispie/dataman/views.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/equators/abc.py` & `irispie-0.1.5/src/irispie/equators/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/equators/plain.py` & `irispie-0.1.5/src/irispie/equators/plain.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/equators/steady.py` & `irispie-0.1.5/src/irispie/equators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/evaluators/printers.py` & `irispie-0.1.5/src/irispie/evaluators/printers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/evaluators/steady.py` & `irispie-0.1.5/src/irispie/evaluators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/fords/descriptors.py` & `irispie-0.1.5/src/irispie/fords/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 $$
 """
 
 
 #[
 from __future__ import annotations
 
-from typing import (Self, NoReturn, )
+from typing import (Self, )
 from collections.abc import (Iterable, )
 import itertools as it_
 import dataclasses as _dc
 import numpy as np_
 
 from .. import (incidence as in_, equations as eq_, quantities as qu_, )
 from ..aldi import (differentiators as ad_, )
@@ -78,15 +78,15 @@
 
     def __init__(
         self,
         equations: eq_.Equations,
         quantities: qu_.Quantities,
         custom_functions: dict | None,
         /,
-    ) -> NoReturn:
+    ) -> None:
         self.system_vectors = SystemVectors(equations, quantities)
         self.solution_vectors = SolutionVectors(self.system_vectors)
         self.system_map = SystemMap(self.system_vectors)
         #
         # Create the context for the algorithmic differentiator
         system_equations = _select_system_equations_from_equations(
             equations,
@@ -161,15 +161,15 @@
     shape_C_excl_dynid: tuple[int, int] | None = None
     shape_D_excl_dynid: tuple[int, int] | None = None
     shape_F: tuple[int, int] | None = None
     shape_G: tuple[int, int] | None = None
     shape_H: tuple[int, int] | None = None
     shape_J: tuple[int, int] | None = None
 
-    def __init__(self, equations: eq_.Equations, quantities: qu_.Quantities) -> NoReturn:
+    def __init__(self, equations: eq_.Equations, quantities: qu_.Quantities) -> None:
         """
         Construct system vectors from a list of equations and a list of quantities
         """
         self.transition_eids = sorted([eqn.id for eqn in equations if eqn.kind in eq_.EquationKind.TRANSITION_EQUATION])
         self.measurement_eids = sorted([eqn.id for eqn in equations if eqn.kind in eq_.EquationKind.MEASUREMENT_EQUATION])
         qid_to_kind = qu_.create_qid_to_kind(quantities)
         all_tokens = set(eq_.generate_all_tokens_from_equations(equations))
@@ -217,15 +217,15 @@
     #[
     transition_variables: in_.Tokens | None = None
     initial_conditions: Iterable[bool] | None = None,
     transition_shocks: in_.Tokens | None = None 
     measurement_variables: in_.Tokens | None = None
     measurement_shocks: in_.Tokens | None = None 
 
-    def __init__(self, system_vectors: SystemVectors, /, ) -> NoReturn:
+    def __init__(self, system_vectors: SystemVectors, /, ) -> None:
         """
         Construct solution vectors and initial conditions indicator
         """
         self.transition_variables, self.initial_conditions = _solution_vector_from_system_vector(system_vectors.transition_variables, system_vectors.initial_conditions)
         self.transition_shocks = system_vectors.transition_shocks
         self.measurement_variables = system_vectors.measurement_variables
         self.measurement_shocks = system_vectors.measurement_shocks
@@ -303,15 +303,15 @@
     G: am_.ArrayMap | None = None
     H: None = None
     J: am_.ArrayMap | None = None
 
     def __init__(
         self,
         system_vectors: SystemVectors,
-    ) -> NoReturn:
+    ) -> None:
         """
         """
         system_eids = system_vectors.transition_eids + system_vectors.measurement_eids
         #
         # Create the map from equation ids to rhs offset; the offset is the
         # number of rows in the Jacobian matrix that precede the equation
         eid_to_rhs_offset = am_.create_eid_to_rhs_offset(system_eids, system_vectors.eid_to_wrt_tokens)
```

### Comparing `irispie-0.1.4/src/irispie/fords/simulators.py` & `irispie-0.1.5/src/irispie/fords/simulators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 First-order system simulators
 """
 
 #[
 from __future__ import annotations
-# from IPython import embed
 
-from typing import (Self, TypeAlias, NoReturn, Literal, )
+from typing import (Self, TypeAlias, Literal, )
 import numpy as np_
 
 from ..fords import (solutions as sl_, descriptors as de_, )
 from ..dataman import (databanks as db_, )
 #]
```

### Comparing `irispie-0.1.4/src/irispie/fords/solutions.py` & `irispie-0.1.5/src/irispie/fords/solutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 
 #[
 import enum as en_
 import numpy as np_
 import scipy as sp_
-from typing import (Self, NoReturn, Callable, )
+from typing import (Self, Callable, )
 from numbers import (Number, )
 import dataclasses as _dc
 
 from ..fords import (systems as _fy, descriptors as _fd, )
 from ..models import (flags as _mg, )
 #]
```

### Comparing `irispie-0.1.4/src/irispie/fords/steadiers.py` & `irispie-0.1.5/src/irispie/fords/steadiers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/fords/systems.py` & `irispie-0.1.5/src/irispie/fords/systems.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def __init__(
         self,
         descriptor: fd_.Descriptor,
         data_array: np_.ndarray,
         steady_array: np_.ndarray,
         /,
-    ) -> NoReturn:
+    ) -> None:
         """
         """
         # Differentiate and evaluate constant
         td, tc = descriptor.aldi_context.eval_to_arrays(
             data_array, steady_array,
         )
```

### Comparing `irispie-0.1.4/src/irispie/jacobians/abc.py` & `irispie-0.1.5/src/irispie/jacobians/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/jacobians/steady.py` & `irispie-0.1.5/src/irispie/jacobians/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/models/facade.py` & `irispie-0.1.5/src/irispie/models/facade.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/models/flags.py` & `irispie-0.1.5/src/irispie/models/flags.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/models/gettables.py` & `irispie-0.1.5/src/irispie/models/gettables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/models/invariants.py` & `irispie-0.1.5/src/irispie/models/invariants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/models/simulatables.py` & `irispie-0.1.5/src/irispie/models/simulatables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 First-order system simulators
 """
 
 
 #[
 from __future__ import annotations
-# from IPython import embed
 
-from typing import (Self, TypeAlias, NoReturn, Literal, Protocol, runtime_checkable)
+from typing import (Self, TypeAlias, Literal, Protocol, runtime_checkable)
 from collections.abc import (Iterable, )
 import numpy as _np
 
 from ..dataman import (databanks as _db, dataslabs as _ds, )
 from ..fords import (simulators as _sr, )
 from . import (variants as _va, )
 #]
```

### Comparing `irispie-0.1.4/src/irispie/models/sources.py` & `irispie-0.1.5/src/irispie/models/sources.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/models/steadiables.py` & `irispie-0.1.5/src/irispie/models/steadiables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/models/variants.py` & `irispie-0.1.5/src/irispie/models/variants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/parsers/common.py` & `irispie-0.1.5/src/irispie/parsers/common.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/parsers/model_source_parser.py` & `irispie-0.1.5/src/irispie/parsers/model_source_parser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/parsers/preparser.py` & `irispie-0.1.5/src/irispie/parsers/preparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 """
 
 
 #[
 from __future__ import annotations
-from IPython import embed
 
 import re as re_
 import parsimonious
 import functools
 import itertools
 from collections.abc import Iterable
 from typing import (TypeAlias, Protocol, )
@@ -280,15 +279,15 @@
     return re_.sub(_contextual_expression_pattern, _replace, text)
 
 
 def _is_preparser_needed(source: str, /, ) -> bool:
     return _KEYWORD_PREFIX in source
 
 
-def _save_preparsed_source(source: str, file_name: str, /, ) -> NoReturn:
+def _save_preparsed_source(source: str, file_name: str, /, ) -> None:
     if file_name:
         with open(file_name, "wt+") as fid:
             fid.write(source)
 
 def _run_preparser_on_source_string(source: str, context: dir, /, ) -> str:
     nodes = _GRAMMAR["source"].parse(source, )
     visitor = _Visitor()
```

### Comparing `irispie-0.1.4/src/irispie/parsers/pseudofunctions.py` & `irispie-0.1.5/src/irispie/parsers/pseudofunctions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/src/irispie/parsers/substitutions.py` & `irispie-0.1.5/src/irispie/parsers/substitutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/LICENCE` & `irispie-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `irispie-0.1.4/pyproject.toml` & `irispie-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "irispie"
-    version = "0.1.4"
+    version = "0.1.5"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Macroeconomic modeling package"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
```

### Comparing `irispie-0.1.4/PKG-INFO` & `irispie-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irispie
-Version: 0.1.4
+Version: 0.1.5
 Summary: Macroeconomic modeling package
 Project-URL: Homepage, https://github.com/iris-solutions-team/irispie
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/irispie/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 License-File: LICENCE
 Keywords: dsge,economics,forecasting,macroeconomics,modeling,simulation
 Classifier: License :: OSI Approved :: MIT License
```

