# Comparing `tmp/edx-event-routing-backends-5.5.4.tar.gz` & `tmp/edx-event-routing-backends-5.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-5.5.4.tar", last modified: Thu Aug  3 17:54:44 2023, max compression
+gzip compressed data, was "edx-event-routing-backends-5.5.5.tar", last modified: Fri Aug  4 13:27:31 2023, max compression
```

## Comparing `edx-event-routing-backends-5.5.4.tar` & `edx-event-routing-backends-5.5.5.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/
--rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4995 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-03 17:54:44.000000 edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8145 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27921 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.931186 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/event_log_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/queued_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    14350 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10799 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/transform_tracking_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9144 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.935186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.939186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4899 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/forum_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)    10068 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.927186 edx-event-routing-backends-5.5.4/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.927186 edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.927186 edx-event-routing-backends-5.5.4/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.943186 edx-event-routing-backends-5.5.4/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4473 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-08-03 17:54:44.947186 edx-event-routing-backends-5.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-08-03 17:54:36.000000 edx-event-routing-backends-5.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-08-04 13:27:31.000000 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4995 2023-08-04 13:27:31.000000 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 13:27:31.000000 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-08-04 13:27:31.000000 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 13:27:31.000000 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-08-04 13:27:31.000000 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-08-04 13:27:31.000000 edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8145 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/backends/events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27921 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/event_routing_backends/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/helpers/event_log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/helpers/queued_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.417323 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15371 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12158 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/transform_tracking_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9144 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.421323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5086 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/forum_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10068 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9988 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.413323 edx-event-routing-backends-5.5.5/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.413323 edx-event-routing-backends-5.5.5/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.413323 edx-event-routing-backends-5.5.5/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4473 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-08-04 13:27:31.425323 edx-event-routing-backends-5.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-08-04 13:27:27.000000 edx-event-routing-backends-5.5.5/setup.py
```

### Comparing `edx-event-routing-backends-5.5.4/CHANGELOG.rst` & `edx-event-routing-backends-5.5.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/LICENSE.txt` & `edx-event-routing-backends-5.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/PKG-INFO` & `edx-event-routing-backends-5.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.5.4
+Version: 5.5.5
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `edx-event-routing-backends-5.5.4/README.rst` & `edx-event-routing-backends-5.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.5.4
+Version: 5.5.5
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `edx-event-routing-backends-5.5.4/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-5.5.5/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/admin.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/admin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/apps.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/backends/events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/backends/tests/test_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/helpers.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/event_log_parser.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/helpers/event_log_parser.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/helpers/queued_sender.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/helpers/queued_sender.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pytest
 from django.core.management import call_command
 from libcloud.storage.types import ContainerDoesNotExistError
 
 import event_routing_backends.management.commands.transform_tracking_logs as transform_tracking_logs
 from event_routing_backends.management.commands.helpers.queued_sender import QueuedSender
 from event_routing_backends.management.commands.transform_tracking_logs import (
+    _get_chunks,
     get_dest_config_from_options,
     get_libcloud_drivers,
     get_source_config_from_options,
     validate_source_and_files,
 )
 
 LOCAL_CONFIG = json.dumps({"key": "/openedx/", "container": "data", "prefix": ""})
@@ -390,7 +391,34 @@
     """
     options = {}
 
     config, container, prefix = get_dest_config_from_options("LRS", options)
     assert config is None
     assert container is None
     assert prefix is None
+
+
+def test_get_chunks():
+    """
+    Tests the retry functionality of the get_chunks function.
+    """
+    fake_source = MagicMock()
+    fake_source.download_object_range_as_stream.return_value = "abc"
+
+    # Check that we got the expected return value
+    assert _get_chunks(fake_source, "", 0, 1) == "abc"
+    # Check that we broke out of the retry loop as expected
+    assert fake_source.download_object_range_as_stream.call_count == 1
+
+    fake_source_err = MagicMock()
+    fake_source_err.download_object_range_as_stream.side_effect = Exception("boom")
+
+    # Speed up our test, don't wait for the sleep
+    with patch("event_routing_backends.management.commands.transform_tracking_logs.sleep"):
+        with pytest.raises(Exception) as e:
+            _get_chunks(fake_source_err, "", 0, 1)
+
+    # Make sure we're getting the error we expect
+    assert "boom" in str(e)
+
+    # Make sure we got the correct number of retries
+    assert fake_source_err.download_object_range_as_stream.call_count == 3
```

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/management/commands/transform_tracking_logs.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/management/commands/transform_tracking_logs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,61 @@
 """
 Management command for transforming tracking log files.
 """
 import json
 import os
 from io import BytesIO
 from textwrap import dedent
+from time import sleep
 
+from django.conf import settings
 from django.core.management.base import BaseCommand
 from libcloud.storage.providers import get_driver
 from libcloud.storage.types import Provider
 
 from event_routing_backends.management.commands.helpers.queued_sender import QueuedSender
 
 # Number of bytes to download at a time, this is 2 MB
 CHUNK_SIZE = 1024 * 1024 * 2
 
 
+def _get_chunks(source, file, start_byte, end_byte):
+    """
+    Fetch a chunk from the upstream source, retry 3 times if necessary.
+
+    Often an upstream provider like S3 will fail occasionally on big jobs. This
+    tries to handle any of those cases gracefully.
+    """
+    chunks = None
+    num_retries = getattr(settings, 'EVENT_ROUTING_BACKEND_BULK_DOWNLOAD_MAX_RETRIES', 3)
+    retry_countdown = getattr(settings, 'EVENT_ROUTING_BACKEND_BULK_DOWNLOAD_COUNTDOWN', 1)
+
+    # Skipping coverage here because it wants to test a branch that will never
+    # be hit (for -> return)
+    for try_number in range(1, num_retries+1):  # pragma: no cover
+        try:
+            chunks = source.download_object_range_as_stream(
+                file,
+                start_bytes=start_byte,
+                end_bytes=end_byte
+            )
+            break
+        # Catching all exceptions here because there's no telling what all
+        # the possible errors from different libcloud providers are.
+        except Exception as e:  # pylint: disable=broad-exception-caught
+            print(e)
+            if try_number == num_retries:
+                print(f"Try {try_number}: Error occurred downloading, giving up.")
+                raise
+            print(f"Try {try_number}: Error occurred downloading source file chunk. Trying again in 1 second.")
+            sleep(retry_countdown)
+
+    return chunks
+
+
 def transform_tracking_logs(
     source,
     source_container,
     source_prefix,
     sender
 ):
     """
@@ -41,19 +77,16 @@
 
         while last_successful_byte < int(file.size):
             end_byte = last_successful_byte + CHUNK_SIZE
 
             if end_byte > file.size:
                 end_byte = file.size
 
-            chunks = source.download_object_range_as_stream(
-                file,
-                start_bytes=last_successful_byte,
-                end_bytes=end_byte
-            )
+            chunks = _get_chunks(source, file, last_successful_byte, end_byte)
+
             for chunk in chunks:
                 chunk = chunk.decode('utf-8')
 
                 # Loop through this chunk, if we find a newline it's time to process
                 # otherwise just keep appending.
                 for char in chunk:
                     if char == "\n" and line:
```

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/models.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 XAPI_VERB_EXPERIENCED = 'http://adlnet.gov/expapi/verbs/experienced'
 XAPI_VERB_NAVIGATED = 'https://w3id.org/xapi/dod-isd/verbs/navigated'
 XAPI_VERB_POSTED = 'https://w3id.org/xapi/acrossx/verbs/posted'
 XAPI_VERB_EDITED = 'https://w3id.org/xapi/acrossx/verbs/edited'
 XAPI_VERB_VIEWED = 'http://id.tincanapi.com/verb/viewed'
 XAPI_VERB_DELETED = 'https://w3id.org/xapi/dod-isd/verbs/deleted'
 XAPI_VERB_VOTED = 'https://w3id.org/xapi/openedx/verb/voted'
+XAPI_VERB_REPORTED = 'https://w3id.org/xapi/acrossx/verbs/reported'
+XAPI_VERB_UNREPORTED = 'https://w3id.org/xapi/openedx/verb/unreported'
 
 XAPI_VERB_TERMINATED = 'http://adlnet.gov/expapi/verbs/terminated'
 XAPI_VERB_ASKED = 'http://adlnet.gov/expapi/verbs/asked'
 
 
 XAPI_VERB_INITIALIZED = 'http://adlnet.gov/expapi/verbs/initialized'
 XAPI_VERB_PLAYED = 'https://w3id.org/xapi/video/verbs/played'
@@ -89,14 +91,16 @@
 FAILED = 'failed'
 SEEKED = 'seeked'
 POSTED = 'posted'
 VIEWED = 'viewed'
 DELETED = 'deleted'
 EDITED = 'edited'
 VOTED = 'voted'
+REPORTED = 'reported'
+UNREPORTED = 'unreported'
 
 TERMINATED = 'terminated'
 NAVIGATED = 'navigated'
 ASKED = 'asked'
 
 # Open edX
 OPENEDX_OAUTH2_TOKEN_URL = '/oauth2/access_token'
```

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     EnrollmentActivatedTransformer,
     EnrollmentDeactivatedTransformer,
 )
 from event_routing_backends.processors.xapi.event_transformers.forum_events import (
     ThreadCreatedTransformer,
     ThreadDeletedTransformer,
     ThreadEditedTransformer,
+    ThreadResponseCreatedTransformer,
+    ThreadResponseReportedTransformer,
+    ThreadResponseUnReportedTransformer,
     ThreadViewedTransformer,
     ThreadVotedTransformer,
 )
 from event_routing_backends.processors.xapi.event_transformers.navigation_events import (
     LinkClickedTransformer,
     OutlineSelectedTransformer,
     TabNavigationTransformer,
```

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/processors/xapi/transformer_processor.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/settings/common.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/settings/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     """
     settings.CALIPER_EVENTS_ENABLED = False
     settings.CALIPER_EVENT_LOGGING_ENABLED = False
     settings.XAPI_EVENTS_ENABLED = True
     settings.XAPI_EVENT_LOGGING_ENABLED = True
     settings.EVENT_ROUTING_BACKEND_MAX_RETRIES = 3
     settings.EVENT_ROUTING_BACKEND_COUNTDOWN = 30
+    settings.EVENT_ROUTING_BACKEND_BULK_DOWNLOAD_MAX_RETRIES = 3
+    settings.EVENT_ROUTING_BACKEND_BULK_DOWNLOAD_COUNTDOWN = 1
 
     # .. setting_name: XAPI_AGENT_IFI_TYPE
     # .. setting_default: 'external_id'
     # .. setting_description: This setting can be used to specify the type of inverse functional identifier
     #    for actor in xAPI statements. Possible values are 'external_id', 'mbox_sha1sum' and 'mbox'
     #    when we set it to 'external_id' xAPI statement would represent actor like this
     #    ```
@@ -69,16 +71,24 @@
                                 'whitelist': [
                                     'edx.course.enrollment.activated',
                                     'edx.course.enrollment.deactivated',
                                     'edx.course.enrollment.mode_changed',
                                     'edx.forum.thread.created',
                                     'edx.forum.thread.deleted',
                                     'edx.forum.thread.edited',
-                                    'edx.forum.thread.viewed',
+                                    'edx.forum.thread.viewed'
+                                    'edx.forum.response.reported',
+                                    'edx.forum.thread.unreported',
                                     'edx.forum.thread.voted',
+                                    'edx.forum.response.created',
+                                    'edx.forum.response.deleted',
+                                    'edx.forum.response.edited',
+                                    'edx.forum.response.reported',
+                                    'edx.forum.response.unreported',
+                                    'edx.forum.response.voted',
                                     'edx.ui.lms.link_clicked',
                                     'edx.ui.lms.sequence.outline.selected',
                                     'edx.ui.lms.outline.selected',
                                     'edx.ui.lms.sequence.next_selected',
                                     'edx.ui.lms.sequence.previous_selected',
                                     'edx.ui.lms.sequence.tab_selected',
                                     'showanswer',
```

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/settings/production.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-5.5.5/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/tasks.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_helpers.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-5.5.5/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/requirements/constraints.txt` & `edx-event-routing-backends-5.5.5/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.4/setup.py` & `edx-event-routing-backends-5.5.5/setup.py`

 * *Files identical despite different names*

