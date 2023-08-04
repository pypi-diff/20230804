# Comparing `tmp/box-sdk-gen-0.1.1.tar.gz` & `tmp/box-sdk-gen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "box-sdk-gen-0.1.1.tar", last modified: Thu Aug  3 14:44:16 2023, max compression
+gzip compressed data, was "box-sdk-gen-0.1.2.tar", last modified: Fri Aug  4 14:50:18 2023, max compression
```

## Comparing `box-sdk-gen-0.1.1.tar` & `box-sdk-gen-0.1.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.967000 box-sdk-gen-0.1.1/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/LICENSE
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6030 2023-08-03 14:44:16.967000 box-sdk-gen-0.1.1/PKG-INFO
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4498 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/README.md
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.935000 box-sdk-gen-0.1.1/box_sdk_gen/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      354 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2929 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/auth_schemas.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3662 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/base_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      936 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/box_response.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4977 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/ccg_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    13031 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/client.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      486 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/developer_token_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7707 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/fetch.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10076 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/jwt_auth.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.966000 box-sdk-gen-0.1.1/box_sdk_gen/managers/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3919 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/authorization.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2862 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/avatars.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9741 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/chunked_uploads.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4876 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/classifications.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4613 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/collaboration_allowlist_entries.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4731 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4176 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/collections.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8911 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/comments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3607 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/device_pinners.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3195 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/downloads.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3081 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/email_aliases.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7939 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4838 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_classifications.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5749 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11200 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_requests.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3797 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_version_legal_holds.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4163 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_version_retentions.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10431 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_versions.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3927 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_watermarks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    20759 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/files.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5205 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_classifications.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4658 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_locks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6540 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4300 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_watermarks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    30103 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folders.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    13439 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/groups.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7382 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/integration_mappings.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4542 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/invites.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7825 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12243 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policy_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7783 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/list_collaborations.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11465 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/memberships.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8128 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/metadata_cascade_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8881 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/metadata_templates.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2417 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/recent_items.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    14453 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10382 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policy_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    22628 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/search.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2610 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/session_termination.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16235 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_files.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16356 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_folders.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    14822 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_web_links.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3644 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_reports.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6473 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segment_members.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7864 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5924 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6136 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barriers.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9174 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/sign_requests.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2328 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/sign_templates.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8343 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/skills.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2940 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7877 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policy_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6243 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/task_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7435 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/tasks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4931 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/terms_of_service_user_statuses.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4858 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/terms_of_services.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4544 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/transfer.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5963 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_files.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6747 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_folders.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4528 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_items.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4683 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_web_links.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11775 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/uploads.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11807 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/user_collaborations.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    22955 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/users.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7957 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/web_links.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7256 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/webhooks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5553 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/workflows.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5582 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/zip_downloads.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      137 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/network.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5726 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/oauth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)   455388 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/schemas.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2307 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/utils.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.937000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6030 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/PKG-INFO
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3415 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/SOURCES.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/dependency_links.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      154 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/requires.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       12 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/top_level.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       38 2023-08-03 14:44:16.967000 box-sdk-gen-0.1.1/setup.cfg
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2011 2023-08-03 14:44:04.000000 box-sdk-gen-0.1.1/setup.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-04 14:50:18.590000 box-sdk-gen-0.1.2/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/LICENSE
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6160 2023-08-04 14:50:18.589000 box-sdk-gen-0.1.2/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4628 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/README.md
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-04 14:50:18.567000 box-sdk-gen-0.1.2/box_sdk_gen/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      354 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2929 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/auth_schemas.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3662 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/base_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      936 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/box_response.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4977 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/ccg_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13031 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      486 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/developer_token_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7707 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/fetch.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10076 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/jwt_auth.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-04 14:50:18.589000 box-sdk-gen-0.1.2/box_sdk_gen/managers/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4296 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/authorization.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4018 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/avatars.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12228 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/chunked_uploads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6032 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6121 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/collaboration_allowlist_entries.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6239 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4930 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/collections.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10759 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/comments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4738 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/device_pinners.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3496 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/downloads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4237 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/email_aliases.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8693 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5994 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/file_classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7282 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/file_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12636 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/file_requests.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4551 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/file_version_legal_holds.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4917 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/file_version_retentions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12240 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/file_versions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5083 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/file_watermarks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    22416 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6361 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/folder_classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5789 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/folder_locks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8073 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/folder_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5456 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/folder_watermarks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    32061 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15324 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/groups.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8942 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/integration_mappings.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5296 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/invites.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9710 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/legal_hold_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14505 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/legal_hold_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9291 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/list_collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13727 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/memberships.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10013 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/metadata_cascade_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11520 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/metadata_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2794 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/recent_items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16338 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/retention_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12644 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/retention_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    23717 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/search.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3389 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/session_termination.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18044 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shared_links_files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18165 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shared_links_folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16631 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shared_links_web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4773 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shield_information_barrier_reports.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7981 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shield_information_barrier_segment_members.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9372 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7809 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shield_information_barrier_segments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7672 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/shield_information_barriers.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11039 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/sign_requests.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3082 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/sign_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9876 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/skills.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3694 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/storage_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9762 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/storage_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8153 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/task_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9419 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/tasks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6062 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/terms_of_service_user_statuses.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6366 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/terms_of_services.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4921 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/transfer.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7094 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/trashed_files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7878 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/trashed_folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4905 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/trashed_items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5814 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/trashed_web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12754 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/uploads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13389 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/user_collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    25217 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/users.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9389 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9141 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/webhooks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6307 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/workflows.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6706 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/managers/zip_downloads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      137 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/network.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5726 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/oauth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)   455388 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/schemas.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2307 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/box_sdk_gen/utils.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-04 14:50:18.568000 box-sdk-gen-0.1.2/box_sdk_gen.egg-info/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6160 2023-08-04 14:50:18.000000 box-sdk-gen-0.1.2/box_sdk_gen.egg-info/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3415 2023-08-04 14:50:18.000000 box-sdk-gen-0.1.2/box_sdk_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2023-08-04 14:50:18.000000 box-sdk-gen-0.1.2/box_sdk_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      154 2023-08-04 14:50:18.000000 box-sdk-gen-0.1.2/box_sdk_gen.egg-info/requires.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       12 2023-08-04 14:50:18.000000 box-sdk-gen-0.1.2/box_sdk_gen.egg-info/top_level.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       38 2023-08-04 14:50:18.590000 box-sdk-gen-0.1.2/setup.cfg
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2011 2023-08-04 14:50:06.000000 box-sdk-gen-0.1.2/setup.py
```

### Comparing `box-sdk-gen-0.1.1/LICENSE` & `box-sdk-gen-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/PKG-INFO` & `box-sdk-gen-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-sdk-gen
-Version: 0.1.1
+Version: 0.1.2
 Summary: [Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.
 Home-page: https://github.com/box/box-python-sdk-gen.git
 Author: Box
 Author-email: oss@box.com
 License: Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: box,sdk,api,rest,boxsdk
 Classifier: Development Status :: 4 - Beta
@@ -37,14 +37,16 @@
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Integration Tests](#integration-tests)
   - [Running integration tests locally](#running-integration-tests-locally)
     - [Create Custom Application](#create-custom-application)
     - [Export configuration](#export-configuration)
     - [Running tests](#running-tests)
+- [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
+- [Copyright and License](#copyright-and-license)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 # Installing
 
 ```console
 pip install box-sdk-gen
@@ -124,15 +126,15 @@
 tickets](https://github.com/box/box-python-sdk-generated/issues)! Or, if that
 doesn't work, [file a new
 one](https://github.com/box/box-python-sdk-generated/issues/new) and we will get
 back to you. If you have general questions about the Box API, you can
 post to the [Box Developer
 Forum](https://community.box.com/t5/Developer-Forum/bd-p/DeveloperForum).
 
-## Copyright and License
+# Copyright and License
 
 Copyright 2023 Box, Inc. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `box-sdk-gen-0.1.1/README.md` & `box-sdk-gen-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Integration Tests](#integration-tests)
   - [Running integration tests locally](#running-integration-tests-locally)
     - [Create Custom Application](#create-custom-application)
     - [Export configuration](#export-configuration)
     - [Running tests](#running-tests)
+- [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
+- [Copyright and License](#copyright-and-license)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 # Installing
 
 ```console
 pip install box-sdk-gen
@@ -93,15 +95,15 @@
 tickets](https://github.com/box/box-python-sdk-generated/issues)! Or, if that
 doesn't work, [file a new
 one](https://github.com/box/box-python-sdk-generated/issues/new) and we will get
 back to you. If you have general questions about the Box API, you can
 post to the [Box Developer
 Forum](https://community.box.com/t5/Developer-Forum/bd-p/DeveloperForum).
 
-## Copyright and License
+# Copyright and License
 
 Copyright 2023 Box, Inc. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/auth_schemas.py` & `box-sdk-gen-0.1.2/box_sdk_gen/auth_schemas.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/base_object.py` & `box-sdk-gen-0.1.2/box_sdk_gen/base_object.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/box_response.py` & `box-sdk-gen-0.1.2/box_sdk_gen/box_response.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/ccg_auth.py` & `box-sdk-gen-0.1.2/box_sdk_gen/ccg_auth.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/client.py` & `box-sdk-gen-0.1.2/box_sdk_gen/client.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/fetch.py` & `box-sdk-gen-0.1.2/box_sdk_gen/fetch.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/jwt_auth.py` & `box-sdk-gen-0.1.2/box_sdk_gen/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/authorization.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/authorization.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class GetAuthorizeResponseTypeArg(str, Enum):
     CODE = 'code'
 
 class AuthorizationManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_authorize(self, response_type: GetAuthorizeResponseTypeArg, client_id: str, redirect_uri: Optional[str] = None, state: Optional[str] = None, scope: Optional[str] = None) -> None:
+    def get_authorize(self, response_type: GetAuthorizeResponseTypeArg, client_id: str, redirect_uri: Optional[str] = None, state: Optional[str] = None, scope: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Authorize a user by sending them through the [Box](https://box.com)
         
         website and request their permission to act on their behalf.
 
         
         This is the first step when authenticating a user using
@@ -73,11 +73,16 @@
             can be used to identify a user on redirect, as well as protect
             against hijacked sessions and other exploits.
         :type state: Optional[str], optional
         :param scope: A comma-separated list of application scopes you'd like to
             authenticate the user for. This defaults to all the scopes configured
             for the application in its configuration page.
         :type scope: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'response_type': to_string(response_type), 'client_id': to_string(client_id), 'redirect_uri': to_string(redirect_uri), 'state': to_string(state), 'scope': to_string(scope)})
-        response: FetchResponse = fetch(''.join(['https://account.box.com/api/oauth2/authorize']), FetchOptions(method='GET', params=query_params_map, response_format=None, auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://account.box.com/api/oauth2/authorize']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/classifications.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/classifications.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import Enum
 
 from typing import Optional
 
+from typing import Dict
+
 import json
 
 from typing import List
 
 from typing import Union
 
 from box_sdk_gen.base_object import BaseObject
@@ -39,42 +41,52 @@
 class CreateMetadataTemplateSchemaClassificationDisplayNameArg(str, Enum):
     CLASSIFICATION = 'Classification'
 
 class ClassificationsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_metadata_template_enterprise_security_classification_schema(self) -> ClassificationTemplate:
+    def get_metadata_template_enterprise_security_classification_schema(self, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ClassificationTemplate:
         """
         Retrieves the classification metadata template and lists all the
         
         classifications available to this enterprise.
 
         
         This API can also be called by including the enterprise ID in the
 
         
         URL explicitly, for example
 
         
         `/metadata_templates/enterprise_12345/securityClassification-6VMVochwUWo/schema`.
 
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return ClassificationTemplate.from_dict(json.loads(response.text))
-    def delete_metadata_template_enterprise_security_classification_schema(self) -> None:
+    def delete_metadata_template_enterprise_security_classification_schema(self, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Delete all classifications by deleting the classification
         
         metadata template.
 
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema']), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def create_metadata_template_schema_classification(self, scope: CreateMetadataTemplateSchemaClassificationScopeArg, display_name: CreateMetadataTemplateSchemaClassificationDisplayNameArg, template_key: Optional[CreateMetadataTemplateSchemaClassificationTemplateKeyArg] = None, hidden: Optional[bool] = None, copy_instance_on_item_copy: Optional[bool] = None, fields: Optional[List] = None) -> ClassificationTemplate:
+    def create_metadata_template_schema_classification(self, scope: CreateMetadataTemplateSchemaClassificationScopeArg, display_name: CreateMetadataTemplateSchemaClassificationDisplayNameArg, template_key: Optional[CreateMetadataTemplateSchemaClassificationTemplateKeyArg] = None, hidden: Optional[bool] = None, copy_instance_on_item_copy: Optional[bool] = None, fields: Optional[List] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ClassificationTemplate:
         """
         When an enterprise does not yet have any classifications, this API call
         
         initializes the classification template with an initial set of
 
         
         classifications.
@@ -99,11 +111,16 @@
         :param hidden: `false`
         :type hidden: Optional[bool], optional
         :param copy_instance_on_item_copy: `false`
         :type copy_instance_on_item_copy: Optional[bool], optional
         :param fields: The classification template holds one field, which holds
             all the valid classification values.
         :type fields: Optional[List], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(scope=scope, template_key=template_key, display_name=display_name, hidden=hidden, copy_instance_on_item_copy=copy_instance_on_item_copy, fields=fields)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/schema#classifications']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/schema#classifications']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return ClassificationTemplate.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/collaboration_allowlist_entries.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/file_version_legal_holds.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-from enum import Enum
-
 from typing import Optional
 
 from typing import Dict
 
 import json
 
-from box_sdk_gen.base_object import BaseObject
-
-from box_sdk_gen.schemas import CollaborationAllowlistEntries
+from box_sdk_gen.schemas import FileVersionLegalHold
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import CollaborationAllowlistEntry
+from box_sdk_gen.schemas import FileVersionLegalHolds
 
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
@@ -26,70 +22,91 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class CreateCollaborationWhitelistEntryDirectionArg(str, Enum):
-    INBOUND = 'inbound'
-    OUTBOUND = 'outbound'
-    BOTH = 'both'
-
-class CollaborationAllowlistEntriesManager:
+class FileVersionLegalHoldsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_collaboration_whitelist_entries(self, marker: Optional[str] = None, limit: Optional[int] = None) -> CollaborationAllowlistEntries:
+    def get_file_version_legal_hold_by_id(self, file_version_legal_hold_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileVersionLegalHold:
         """
-        Returns the list domains that have been deemed safe to create collaborations
+        Retrieves information about the legal hold policies
         
-        for within the current enterprise.
+        assigned to a file version.
 
-        :param marker: Defines the position marker at which to begin returning results. This is
-            used when paginating using marker-based pagination.
-            This requires `usemarker` to be set to `true`.
-        :type marker: Optional[str], optional
-        :param limit: The maximum number of items to return per page.
-        :type limit: Optional[int], optional
+        :param file_version_legal_hold_id: The ID of the file version legal hold
+            Example: "2348213"
+        :type file_version_legal_hold_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_version_legal_holds/', file_version_legal_hold_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return FileVersionLegalHold.from_dict(json.loads(response.text))
+    def get_file_version_legal_holds(self, policy_id: str, marker: Optional[str] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileVersionLegalHolds:
         """
-        query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaboration_whitelist_entries']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return CollaborationAllowlistEntries.from_dict(json.loads(response.text))
-    def create_collaboration_whitelist_entry(self, domain: str, direction: CreateCollaborationWhitelistEntryDirectionArg) -> CollaborationAllowlistEntry:
-        """
-        Creates a new entry in the list of allowed domains to allow
+        Get a list of file versions on legal hold for a legal hold
         
-        collaboration for.
+        assignment.
 
-        :param domain: The domain to add to the list of allowed domains.
-        :type domain: str
-        :param direction: The direction in which to allow collaborations.
-        :type direction: CreateCollaborationWhitelistEntryDirectionArg
-        """
-        request_body: BaseObject = BaseObject(domain=domain, direction=direction)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaboration_whitelist_entries']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return CollaborationAllowlistEntry.from_dict(json.loads(response.text))
-    def get_collaboration_whitelist_entry_by_id(self, collaboration_whitelist_entry_id: str) -> CollaborationAllowlistEntry:
-        """
-        Returns a domain that has been deemed safe to create collaborations
         
-        for within the current enterprise.
+        Due to ongoing re-architecture efforts this API might not return all file
+
+        
+        versions for this policy ID.
+
+        
+        Instead, this API will only return file versions held in the legacy
+
+        
+        architecture. Two new endpoints will available to request any file versions
+
+        
+        held in the new architecture.
+
+        
+        For file versions held in the new architecture, the `GET
+
+        
+        /legal_hold_policy_assignments/:id/file_versions_on_hold` API can be used to
+
+        
+        return all past file versions available for this policy assignment, and the
+
+        
+        `GET /legal_hold_policy_assignments/:id/files_on_hold` API can be used to
+
+        
+        return any current (latest) versions of a file under legal hold.
 
-        :param collaboration_whitelist_entry_id: The ID of the entry in the list.
-            Example: "213123"
-        :type collaboration_whitelist_entry_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaboration_whitelist_entries/', collaboration_whitelist_entry_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return CollaborationAllowlistEntry.from_dict(json.loads(response.text))
-    def delete_collaboration_whitelist_entry_by_id(self, collaboration_whitelist_entry_id: str) -> None:
-        """
-        Removes a domain from the list of domains that have been deemed safe to create
         
-        collaborations for within the current enterprise.
+        The `GET /legal_hold_policy_assignments?policy_id={id}` API can be used to
 
-        :param collaboration_whitelist_entry_id: The ID of the entry in the list.
-            Example: "213123"
-        :type collaboration_whitelist_entry_id: str
+        
+        find a list of policy assignments for a given policy ID.
+
+        
+        Once the re-architecture is completed this API will be deprecated.
+
+        :param policy_id: The ID of the legal hold policy to get the file version legal
+            holds for.
+        :type policy_id: str
+        :param marker: Defines the position marker at which to begin returning results. This is
+            used when paginating using marker-based pagination.
+            This requires `usemarker` to be set to `true`.
+        :type marker: Optional[str], optional
+        :param limit: The maximum number of items to return per page.
+        :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaboration_whitelist_entries/', collaboration_whitelist_entry_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
-        return None
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'policy_id': to_string(policy_id), 'marker': to_string(marker), 'limit': to_string(limit)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_version_legal_holds']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return FileVersionLegalHolds.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/collections.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/collections.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from box_sdk_gen.fetch import FetchResponse
 
 class CollectionsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_collections(self, fields: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None) -> Collections:
+    def get_collections(self, fields: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collections:
         """
         Retrieves all collections for a given user.
         
         Currently, only the `favorites` collection
 
         
         is supported.
@@ -51,19 +51,24 @@
         :param offset: The offset of the item at which to begin the response.
             Queries with offset parameter value
             exceeding 10000 will be rejected
             with a 400 response.
         :type offset: Optional[int], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'offset': to_string(offset), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collections']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collections']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Collections.from_dict(json.loads(response.text))
-    def get_collection_items(self, collection_id: str, fields: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None) -> Items:
+    def get_collection_items(self, collection_id: str, fields: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Items:
         """
         Retrieves the files and/or folders contained within
         
         this collection.
 
         :param collection_id: The ID of the collection.
             Example: "926489"
@@ -80,11 +85,16 @@
         :param offset: The offset of the item at which to begin the response.
             Queries with offset parameter value
             exceeding 10000 will be rejected
             with a 400 response.
         :type offset: Optional[int], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'offset': to_string(offset), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collections/', collection_id, '/items']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collections/', collection_id, '/items']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Items.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/comments.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/comments.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.id = id
         self.type = type
 
 class CommentsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_comments(self, file_id: str, fields: Optional[str] = None, limit: Optional[int] = None, offset: Optional[int] = None) -> Comments:
+    def get_file_comments(self, file_id: str, fields: Optional[str] = None, limit: Optional[int] = None, offset: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Comments:
         """
         Retrieves a list of comments for a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
@@ -77,19 +77,24 @@
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
         :param offset: The offset of the item at which to begin the response.
             Queries with offset parameter value
             exceeding 10000 will be rejected
             with a 400 response.
         :type offset: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'limit': to_string(limit), 'offset': to_string(offset)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/comments']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/comments']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Comments.from_dict(json.loads(response.text))
-    def get_comment_by_id(self, comment_id: str, fields: Optional[str] = None) -> CommentFull:
+    def get_comment_by_id(self, comment_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> CommentFull:
         """
         Retrieves the message and metadata for a specific comment, as well
         
         as information on the user who created the comment.
 
         :param comment_id: The ID of the comment.
             Example: "12345"
@@ -99,19 +104,24 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments/', comment_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments/', comment_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return CommentFull.from_dict(json.loads(response.text))
-    def update_comment_by_id(self, comment_id: str, message: Optional[str] = None, fields: Optional[str] = None) -> CommentFull:
+    def update_comment_by_id(self, comment_id: str, message: Optional[str] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> CommentFull:
         """
         Update the message of a comment.
         :param comment_id: The ID of the comment.
             Example: "12345"
         :type comment_id: str
         :param message: The text of the comment to update
         :type message: Optional[str], optional
@@ -120,57 +130,72 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(message=message)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments/', comment_id]), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments/', comment_id]), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return CommentFull.from_dict(json.loads(response.text))
-    def delete_comment_by_id(self, comment_id: str) -> None:
+    def delete_comment_by_id(self, comment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Permanently deletes a comment.
         :param comment_id: The ID of the comment.
             Example: "12345"
         :type comment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments/', comment_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments/', comment_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def create_comment(self, message: str, tagged_message: Optional[str] = None, item: Optional[CreateCommentItemArg] = None, fields: Optional[str] = None) -> Comment:
+    def create_comment(self, message: str, item: CreateCommentItemArg, tagged_message: Optional[str] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Comment:
         """
         Adds a comment by the user to a specific file, or
         
         as a reply to an other comment.
 
         :param message: The text of the comment.
             To mention a user, use the `tagged_message`
             parameter instead.
         :type message: str
+        :param item: The item to attach the comment to.
+        :type item: CreateCommentItemArg
         :param tagged_message: The text of the comment, including `@[user_id:name]`
             somewhere in the message to mention another user, which
             will send them an email notification, letting them know
             they have been mentioned.
             The `user_id` is the target user's ID, where the `name`
             can be any custom phrase. In the Box UI this name will
             link to the user's profile.
             If you are not mentioning another user, use `message`
             instead.
         :type tagged_message: Optional[str], optional
-        :param item: The item to attach the comment to.
-        :type item: Optional[CreateCommentItemArg], optional
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(message=message, tagged_message=tagged_message, item=item)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/comments']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Comment.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/device_pinners.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/downloads.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-from enum import Enum
-
 from typing import Optional
 
-import json
-
 from typing import Dict
 
-from box_sdk_gen.schemas import DevicePinner
-
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import DevicePinners
-
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
 from box_sdk_gen.utils import to_string
@@ -24,58 +16,48 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class GetEnterpriseDevicePinnersDirectionArg(str, Enum):
-    ASC = 'ASC'
-    DESC = 'DESC'
-
-class DevicePinnersManager:
+class DownloadsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_device_pinner_by_id(self, device_pinner_id: str) -> DevicePinner:
-        """
-        Retrieves information about an individual device pin.
-        :param device_pinner_id: The ID of the device pin
-            Example: "2324234"
-        :type device_pinner_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/device_pinners/', device_pinner_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return DevicePinner.from_dict(json.loads(response.text))
-    def delete_device_pinner_by_id(self, device_pinner_id: str) -> None:
-        """
-        Deletes an individual device pin.
-        :param device_pinner_id: The ID of the device pin
-            Example: "2324234"
-        :type device_pinner_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/device_pinners/', device_pinner_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
-        return None
-    def get_enterprise_device_pinners(self, enterprise_id: str, marker: Optional[str] = None, limit: Optional[int] = None, direction: Optional[GetEnterpriseDevicePinnersDirectionArg] = None) -> DevicePinners:
-        """
-        Retrieves all the device pins within an enterprise.
-        
-        The user must have admin privileges, and the application
-
-        
-        needs the "manage enterprise" scope to make this call.
-
-        :param enterprise_id: The ID of the enterprise
-            Example: "3442311"
-        :type enterprise_id: str
-        :param marker: Defines the position marker at which to begin returning results. This is
-            used when paginating using marker-based pagination.
-            This requires `usemarker` to be set to `true`.
-        :type marker: Optional[str], optional
-        :param limit: The maximum number of items to return per page.
-        :type limit: Optional[int], optional
-        :param direction: The direction to sort results in. This can be either in alphabetical ascending
-            (`ASC`) or descending (`DESC`) order.
-        :type direction: Optional[GetEnterpriseDevicePinnersDirectionArg], optional
+    def download_file(self, file_id: str, version: Optional[str] = None, access_token: Optional[str] = None, range: Optional[str] = None, boxapi: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ByteStream:
         """
-        query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit), 'direction': to_string(direction)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/enterprises/', enterprise_id, '/device_pinners']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return DevicePinners.from_dict(json.loads(response.text))
+        Returns the contents of a file in binary format.
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
+            and copying the ID from the URL. For example,
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
+            Example: "12345"
+        :type file_id: str
+        :param version: The file version to download
+        :type version: Optional[str], optional
+        :param access_token: An optional access token that can be used to pre-authenticate this request, which means that a download link can be shared with a browser or a third party service without them needing to know how to handle the authentication.
+            When using this parameter, please make sure that the access token is sufficiently scoped down to only allow read access to that file and no other files or folders.
+        :type access_token: Optional[str], optional
+        :param range: The byte range of the content to download.
+            The format `bytes={start_byte}-{end_byte}` can be used to specify
+            what section of the file to download.
+        :type range: Optional[str], optional
+        :param boxapi: The URL, and optional password, for the shared link of this item.
+            This header can be used to access items that have not been
+            explicitly shared with a user.
+            Use the format `shared_link=[link]` or if a password is required then
+            use `shared_link=[link]&shared_link_password=[password]`.
+            This header can be used on the file or folder shared, as well as on any files
+            or folders nested within the item.
+        :type boxapi: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'version': to_string(version), 'access_token': to_string(access_token)})
+        headers_map: Dict[str, str] = prepare_params({'range': to_string(range), 'boxapi': to_string(boxapi), **extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/content']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='binary', auth=self.auth, network_session=self.network_session))
+        return response.content
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/downloads.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/recent_items.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import Optional
 
 from typing import Dict
 
+import json
+
+from box_sdk_gen.schemas import RecentItems
+
 from box_sdk_gen.schemas import ClientError
 
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
@@ -16,44 +20,44 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class DownloadsManager:
+class RecentItemsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def download_file(self, file_id: str, version: Optional[str] = None, access_token: Optional[str] = None, range: Optional[str] = None, boxapi: Optional[str] = None) -> ByteStream:
+    def get_recent_items(self, fields: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RecentItems:
         """
-        Returns the contents of a file in binary format.
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
-        :param version: The file version to download
-        :type version: Optional[str], optional
-        :param access_token: An optional access token that can be used to pre-authenticate this request, which means that a download link can be shared with a browser or a third party service without them needing to know how to handle the authentication.
-            When using this parameter, please make sure that the access token is sufficiently scoped down to only allow read access to that file and no other files or folders.
-        :type access_token: Optional[str], optional
-        :param range: The byte range of the content to download.
-            The format `bytes={start_byte}-{end_byte}` can be used to specify
-            what section of the file to download.
-        :type range: Optional[str], optional
-        :param boxapi: The URL, and optional password, for the shared link of this item.
-            This header can be used to access items that have not been
-            explicitly shared with a user.
-            Use the format `shared_link=[link]` or if a password is required then
-            use `shared_link=[link]&shared_link_password=[password]`.
-            This header can be used on the file or folder shared, as well as on any files
-            or folders nested within the item.
-        :type boxapi: Optional[str], optional
+        Returns information about the recent items accessed
+        
+        by a user, either in the last 90 days or up to the last
+
+        
+        1000 items accessed.
+
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param limit: The maximum number of items to return per page.
+        :type limit: Optional[int], optional
+        :param marker: Defines the position marker at which to begin returning results. This is
+            used when paginating using marker-based pagination.
+            This requires `usemarker` to be set to `true`.
+        :type marker: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        query_params_map: Dict[str, str] = prepare_params({'version': to_string(version), 'access_token': to_string(access_token)})
-        headers_map: Dict[str, str] = prepare_params({'range': to_string(range), 'boxapi': to_string(boxapi)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/content']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='binary', auth=self.auth, network_session=self.network_session))
-        return response.content
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'limit': to_string(limit), 'marker': to_string(marker)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/recent_items']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return RecentItems.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/events.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ADMIN_LOGS = 'admin_logs'
     ADMIN_LOGS_STREAMING = 'admin_logs_streaming'
 
 class EventsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_events(self, stream_type: Optional[GetEventsStreamTypeArg] = None, stream_position: Optional[str] = None, limit: Optional[int] = None, event_type: Optional[str] = None, created_after: Optional[str] = None, created_before: Optional[str] = None) -> Events:
+    def get_events(self, stream_type: Optional[GetEventsStreamTypeArg] = None, stream_position: Optional[str] = None, limit: Optional[int] = None, event_type: Optional[str] = None, created_after: Optional[str] = None, created_before: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Events:
         """
         Returns up to a year of past events for a given user
         
         or for the entire enterprise.
 
         
         By default this returns events for the authenticated user. To retrieve events
@@ -103,19 +103,24 @@
             when requesting the events with a `stream_type` of `admin_logs`. For any
             other `stream_type` this value will be ignored.
         :type created_after: Optional[str], optional
         :param created_before: The upper bound date and time to return events for. This can only be used
             when requesting the events with a `stream_type` of `admin_logs`. For any
             other `stream_type` this value will be ignored.
         :type created_before: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'stream_type': to_string(stream_type), 'stream_position': to_string(stream_position), 'limit': to_string(limit), 'event_type': to_string(event_type), 'created_after': to_string(created_after), 'created_before': to_string(created_before)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/events']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/events']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Events.from_dict(json.loads(response.text))
-    def get_events_with_long_polling(self) -> RealtimeServers:
+    def get_events_with_long_polling(self, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RealtimeServers:
         """
         Returns a list of real-time servers that can be used for long-polling updates
         
         to the [event stream](#get-events).
 
         
         Long polling is the concept where a HTTP request is kept open until the
@@ -182,10 +187,15 @@
 
         
         real-time server, you should start over by making a call to this endpoint
 
         
         first.
 
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/events']), FetchOptions(method='OPTIONS', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/events']), FetchOptions(method='OPTIONS', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return RealtimeServers.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_classifications.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/email_aliases.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import Optional
 
+from typing import Dict
+
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
-from box_sdk_gen.schemas import Classification
+from box_sdk_gen.schemas import EmailAliases
 
 from box_sdk_gen.schemas import ClientError
 
+from box_sdk_gen.schemas import EmailAlias
+
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
 from box_sdk_gen.utils import to_string
@@ -20,93 +24,67 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class FileClassificationsManager:
+class EmailAliasesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_metadata_enterprise_security_classification_6_vm_vochw_u_wo(self, file_id: str) -> Classification:
+    def get_user_email_aliases(self, user_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> EmailAliases:
         """
-        Retrieves the classification metadata instance that
-        
-        has been applied to a file.
-
-        
-        This API can also be called by including the enterprise ID in the
-
+        Retrieves all email aliases for a user. The collection
         
-        URL explicitly, for example
+        does not include the primary login for the user.
 
-        
-        `/files/:id//enterprise_12345/securityClassification-6VMVochwUWo`.
-
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
+        :param user_id: The ID of the user.
             Example: "12345"
-        :type file_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/enterprise/securityClassification-6VMVochwUWo']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return Classification.from_dict(json.loads(response.text))
-    def create_file_metadata_enterprise_security_classification(self, file_id: str, box_security_classification_key: Optional[str] = None) -> Classification:
+        :type user_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id, '/email_aliases']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return EmailAliases.from_dict(json.loads(response.text))
+    def create_user_email_alias(self, user_id: str, email: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> EmailAlias:
         """
-        Adds a classification to a file by specifying the label of the
-        
-        classification to add.
-
-        
-        This API can also be called by including the enterprise ID in the
-
-        
-        URL explicitly, for example
-
-        
-        `/files/:id//enterprise_12345/securityClassification-6VMVochwUWo`.
-
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
+        Adds a new email alias to a user account..
+        :param user_id: The ID of the user.
             Example: "12345"
-        :type file_id: str
-        :param box_security_classification_key: The name of the classification to apply to this file.
-            To list the available classifications in an enterprise,
-            use the classification API to retrieve the
-            [classification template](e://get_metadata_templates_enterprise_securityClassification-6VMVochwUWo_schema)
-            which lists all available classification keys.
-        :type box_security_classification_key: Optional[str], optional
-        """
-        request_body: BaseObject = BaseObject(box_security_classification_key=box_security_classification_key)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/enterprise/securityClassification-6VMVochwUWo']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return Classification.from_dict(json.loads(response.text))
-    def delete_file_metadata_enterprise_security_classification(self, file_id: str) -> None:
+        :type user_id: str
+        :param email: The email address to add to the account as an alias.
+            Note: The domain of the email alias needs to be registered
+             to your enterprise.
+            See the [domain verification guide](
+              https://support.box.com/hc/en-us/articles/4408619650579-Domain-Verification
+              ) for steps to add a new domain.
+        :type email: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(email=email)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id, '/email_aliases']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return EmailAlias.from_dict(json.loads(response.text))
+    def delete_user_email_alias_by_id(self, user_id: str, email_alias_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
-        Removes any classifications from a file.
-        
-        This API can also be called by including the enterprise ID in the
-
-        
-        URL explicitly, for example
-
-        
-        `/files/:id//enterprise_12345/securityClassification-6VMVochwUWo`.
-
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
+        Removes an email alias from a user.
+        :param user_id: The ID of the user.
             Example: "12345"
-        :type file_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/enterprise/securityClassification-6VMVochwUWo']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        :type user_id: str
+        :param email_alias_id: The ID of the email alias.
+            Example: "23432"
+        :type email_alias_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id, '/email_aliases/', email_alias_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_metadata.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/file_metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import Enum
 
 from typing import Optional
 
+from typing import Dict
+
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import Metadatas
 
 from box_sdk_gen.schemas import ClientError
@@ -42,29 +44,34 @@
     GLOBAL = 'global'
     ENTERPRISE = 'enterprise'
 
 class FileMetadataManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_metadata(self, file_id: str) -> Metadatas:
+    def get_file_metadata(self, file_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Metadatas:
         """
         Retrieves all metadata for a given file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
             the `file_id` is `123`.
             Example: "12345"
         :type file_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Metadatas.from_dict(json.loads(response.text))
-    def get_file_metadata_by_id(self, file_id: str, scope: GetFileMetadataByIdScopeArg, template_key: str) -> MetadataFull:
+    def get_file_metadata_by_id(self, file_id: str, scope: GetFileMetadataByIdScopeArg, template_key: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> MetadataFull:
         """
         Retrieves the instance of a metadata template that has been applied to a
         
         file.
 
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
@@ -76,18 +83,23 @@
         :type file_id: str
         :param scope: The scope of the metadata template
             Example: "global"
         :type scope: GetFileMetadataByIdScopeArg
         :param template_key: The name of the metadata template
             Example: "properties"
         :type template_key: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return MetadataFull.from_dict(json.loads(response.text))
-    def create_file_metadata_by_id(self, file_id: str, scope: CreateFileMetadataByIdScopeArg, template_key: str) -> Metadata:
+    def create_file_metadata_by_id(self, file_id: str, scope: CreateFileMetadataByIdScopeArg, template_key: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Metadata:
         """
         Applies an instance of a metadata template to a file.
         
         In most cases only values that are present in the metadata template
 
         
         will be accepted, except for the `global.properties` template which accepts
@@ -105,19 +117,24 @@
         :type file_id: str
         :param scope: The scope of the metadata template
             Example: "global"
         :type scope: CreateFileMetadataByIdScopeArg
         :param template_key: The name of the metadata template
             Example: "properties"
         :type template_key: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject()
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Metadata.from_dict(json.loads(response.text))
-    def delete_file_metadata_by_id(self, file_id: str, scope: DeleteFileMetadataByIdScopeArg, template_key: str) -> None:
+    def delete_file_metadata_by_id(self, file_id: str, scope: DeleteFileMetadataByIdScopeArg, template_key: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a piece of file metadata.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
@@ -126,10 +143,15 @@
         :type file_id: str
         :param scope: The scope of the metadata template
             Example: "global"
         :type scope: DeleteFileMetadataByIdScopeArg
         :param template_key: The name of the metadata template
             Example: "properties"
         :type template_key: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_requests.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/file_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from enum import Enum
 
 from typing import Optional
 
 from box_sdk_gen.base_object import BaseObject
 
-import json
-
 from typing import Dict
 
-from box_sdk_gen.base_object import BaseObject
+import json
 
 from box_sdk_gen.schemas import FileRequest
 
 from box_sdk_gen.schemas import ClientError
 
 from box_sdk_gen.schemas import FileRequestUpdateRequest
 
@@ -58,29 +56,34 @@
     ACTIVE = 'active'
     INACTIVE = 'inactive'
 
 class FileRequestsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_request_by_id(self, file_request_id: str) -> FileRequest:
+    def get_file_request_by_id(self, file_request_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileRequest:
         """
         Retrieves the information about a file request.
         :param file_request_id: The unique identifier that represent a file request.
             The ID for any file request can be determined
             by visiting a file request builder in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/filerequest/123`
             the `file_request_id` is `123`.
             Example: "123"
         :type file_request_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_requests/', file_request_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_requests/', file_request_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileRequest.from_dict(json.loads(response.text))
-    def update_file_request_by_id(self, file_request_id: str, title: Optional[str] = None, description: Optional[str] = None, status: Optional[UpdateFileRequestByIdStatusArg] = None, is_email_required: Optional[bool] = None, is_description_required: Optional[bool] = None, expires_at: Optional[str] = None, if_match: Optional[str] = None) -> FileRequest:
+    def update_file_request_by_id(self, file_request_id: str, title: Optional[str] = None, description: Optional[str] = None, status: Optional[UpdateFileRequestByIdStatusArg] = None, is_email_required: Optional[bool] = None, is_description_required: Optional[bool] = None, expires_at: Optional[str] = None, if_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileRequest:
         """
         Updates a file request. This can be used to activate or
         
         deactivate a file request.
 
         :param file_request_id: The unique identifier that represent a file request.
             The ID for any file request can be determined
@@ -126,34 +129,43 @@
         :param if_match: Ensures this item hasn't recently changed before
             making changes.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `412 Precondition Failed` if it
             has changed since.
         :type if_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        request_body: BaseObject = BaseObject(title=title, description=description, status=status, is_email_required=is_email_required, is_description_required=is_description_required, expires_at=expires_at)
-        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match)})
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: FileRequestUpdateRequest = FileRequestUpdateRequest(title=title, description=description, status=status, is_email_required=is_email_required, is_description_required=is_description_required, expires_at=expires_at)
+        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_requests/', file_request_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FileRequest.from_dict(json.loads(response.text))
-    def delete_file_request_by_id(self, file_request_id: str) -> None:
+    def delete_file_request_by_id(self, file_request_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a file request permanently.
         :param file_request_id: The unique identifier that represent a file request.
             The ID for any file request can be determined
             by visiting a file request builder in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/filerequest/123`
             the `file_request_id` is `123`.
             Example: "123"
         :type file_request_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_requests/', file_request_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_requests/', file_request_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def create_file_request_copy(self, file_request_id: str, folder: CreateFileRequestCopyFolderArg, title: Optional[str] = None, description: Optional[str] = None, status: Optional[CreateFileRequestCopyStatusArg] = None, is_email_required: Optional[bool] = None, is_description_required: Optional[bool] = None, expires_at: Optional[str] = None) -> FileRequest:
+    def create_file_request_copy(self, file_request_id: str, folder: CreateFileRequestCopyFolderArg, title: Optional[str] = None, description: Optional[str] = None, status: Optional[CreateFileRequestCopyStatusArg] = None, is_email_required: Optional[bool] = None, is_description_required: Optional[bool] = None, expires_at: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileRequest:
         """
         Copies an existing file request that is already present on one folder,
         
         and applies it to another folder.
 
         :param file_request_id: The unique identifier that represent a file request.
             The ID for any file request can be determined
@@ -194,11 +206,16 @@
         :type is_description_required: Optional[bool], optional
         :param expires_at: The date after which a file request will no longer accept new
             submissions.
             After this date, the `status` will automatically be set to
             `inactive`.
             This will default to the value on the existing file request.
         :type expires_at: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        request_body: BaseObject = BaseObject(folder=folder, title=title, description=description, status=status, is_email_required=is_email_required, is_description_required=is_description_required, expires_at=expires_at)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_requests/', file_request_id, '/copy']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: FileRequestCopyRequest = FileRequestCopyRequest(folder=folder, title=title, description=description, status=status, is_email_required=is_email_required, is_description_required=is_description_required, expires_at=expires_at)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_requests/', file_request_id, '/copy']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FileRequest.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_version_retentions.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/file_version_retentions.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     PERMANENTLY_DELETE = 'permanently_delete'
     REMOVE_RETENTION = 'remove_retention'
 
 class FileVersionRetentionsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_version_retentions(self, file_id: Optional[str] = None, file_version_id: Optional[str] = None, policy_id: Optional[str] = None, disposition_action: Optional[GetFileVersionRetentionsDispositionActionArg] = None, disposition_before: Optional[str] = None, disposition_after: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None) -> FileVersionRetentions:
+    def get_file_version_retentions(self, file_id: Optional[str] = None, file_version_id: Optional[str] = None, policy_id: Optional[str] = None, disposition_action: Optional[GetFileVersionRetentionsDispositionActionArg] = None, disposition_before: Optional[str] = None, disposition_after: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileVersionRetentions:
         """
         Retrieves all file version retentions for the given enterprise.
         :param file_id: Filters results by files with this ID.
         :type file_id: Optional[str], optional
         :param file_version_id: Filters results by file versions with this ID.
         :type file_version_id: Optional[str], optional
         :param policy_id: Filters results by the retention policy with this ID.
@@ -56,20 +56,30 @@
         :type disposition_after: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'file_id': to_string(file_id), 'file_version_id': to_string(file_version_id), 'policy_id': to_string(policy_id), 'disposition_action': to_string(disposition_action), 'disposition_before': to_string(disposition_before), 'disposition_after': to_string(disposition_after), 'limit': to_string(limit), 'marker': to_string(marker)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_version_retentions']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_version_retentions']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileVersionRetentions.from_dict(json.loads(response.text))
-    def get_file_version_retention_by_id(self, file_version_retention_id: str) -> FileVersionRetention:
+    def get_file_version_retention_by_id(self, file_version_retention_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileVersionRetention:
         """
         Returns information about a file version retention.
         :param file_version_retention_id: The ID of the file version retention
             Example: "3424234"
         :type file_version_retention_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_version_retentions/', file_version_retention_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/file_version_retentions/', file_version_retention_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileVersionRetention.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_versions.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/skills.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 from enum import Enum
 
 from typing import Optional
 
+from typing import List
+
+from typing import Union
+
+from box_sdk_gen.base_object import BaseObject
+
 from typing import Dict
 
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
-from box_sdk_gen.schemas import FileVersions
+from box_sdk_gen.schemas import SkillCardsMetadata
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import FileVersionFull
+from box_sdk_gen.schemas import KeywordSkillCard
+
+from box_sdk_gen.schemas import TimelineSkillCard
+
+from box_sdk_gen.schemas import TranscriptSkillCard
+
+from box_sdk_gen.schemas import StatusSkillCard
 
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
@@ -26,201 +38,161 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class PromoteFileVersionTypeArg(str, Enum):
+class UpdateSkillInvocationByIdStatusArg(str, Enum):
+    INVOKED = 'invoked'
+    PROCESSING = 'processing'
+    SUCCESS = 'success'
+    TRANSIENT_FAILURE = 'transient_failure'
+    PERMANENT_FAILURE = 'permanent_failure'
+
+class UpdateSkillInvocationByIdMetadataArg(BaseObject):
+    def __init__(self, cards: Optional[List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]]] = None, **kwargs):
+        """
+        :param cards: A list of Box Skill cards to apply to this file.
+        :type cards: Optional[List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]]], optional
+        """
+        super().__init__(**kwargs)
+        self.cards = cards
+
+class UpdateSkillInvocationByIdFileArgTypeField(str, Enum):
+    FILE = 'file'
+
+class UpdateSkillInvocationByIdFileArg(BaseObject):
+    def __init__(self, type: Optional[UpdateSkillInvocationByIdFileArgTypeField] = None, id: Optional[str] = None, **kwargs):
+        """
+        :param type: `file`
+        :type type: Optional[UpdateSkillInvocationByIdFileArgTypeField], optional
+        :param id: The ID of the file
+        :type id: Optional[str], optional
+        """
+        super().__init__(**kwargs)
+        self.type = type
+        self.id = id
+
+class UpdateSkillInvocationByIdFileVersionArgTypeField(str, Enum):
     FILE_VERSION = 'file_version'
 
-class FileVersionsManager:
+class UpdateSkillInvocationByIdFileVersionArg(BaseObject):
+    def __init__(self, type: Optional[UpdateSkillInvocationByIdFileVersionArgTypeField] = None, id: Optional[str] = None, **kwargs):
+        """
+        :param type: `file_version`
+        :type type: Optional[UpdateSkillInvocationByIdFileVersionArgTypeField], optional
+        :param id: The ID of the file version
+        :type id: Optional[str], optional
+        """
+        super().__init__(**kwargs)
+        self.type = type
+        self.id = id
+
+class UpdateSkillInvocationByIdUsageArg(BaseObject):
+    def __init__(self, unit: Optional[str] = None, value: Optional[int] = None, **kwargs):
+        """
+        :param unit: `file`
+        :type unit: Optional[str], optional
+        :param value: `1`
+        :type value: Optional[int], optional
+        """
+        super().__init__(**kwargs)
+        self.unit = unit
+        self.value = value
+
+class SkillsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_versions(self, file_id: str, fields: Optional[str] = None, limit: Optional[int] = None, offset: Optional[int] = None) -> FileVersions:
+    def get_file_metadata_global_box_skills_cards(self, file_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> SkillCardsMetadata:
         """
-        Retrieve a list of the past versions for a file.
-        
-        Versions are only tracked by Box users with premium accounts. To fetch the ID
-
-        
-        of the current version of a file, use the `GET /file/:id` API.
-
+        List the Box Skills metadata cards that are attached to a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
             the `file_id` is `123`.
             Example: "12345"
         :type file_id: str
-        :param fields: A comma-separated list of attributes to include in the
-            response. This can be used to request fields that are
-            not normally returned in a standard response.
-            Be aware that specifying this parameter will have the
-            effect that none of the standard fields are returned in
-            the response unless explicitly specified, instead only
-            fields for the mini representation are returned, additional
-            to the fields requested.
-        :type fields: Optional[str], optional
-        :param limit: The maximum number of items to return per page.
-        :type limit: Optional[int], optional
-        :param offset: The offset of the item at which to begin the response.
-            Queries with offset parameter value
-            exceeding 10000 will be rejected
-            with a 400 response.
-        :type offset: Optional[int], optional
-        """
-        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'limit': to_string(limit), 'offset': to_string(offset)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/versions']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return FileVersions.from_dict(json.loads(response.text))
-    def get_file_version_by_id(self, file_id: str, file_version_id: str, fields: Optional[str] = None) -> FileVersionFull:
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        Retrieve a specific version of a file.
-        
-        Versions are only tracked for Box users with premium accounts.
-
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
-        :param file_version_id: The ID of the file version
-            Example: "1234"
-        :type file_version_id: str
-        :param fields: A comma-separated list of attributes to include in the
-            response. This can be used to request fields that are
-            not normally returned in a standard response.
-            Be aware that specifying this parameter will have the
-            effect that none of the standard fields are returned in
-            the response unless explicitly specified, instead only
-            fields for the mini representation are returned, additional
-            to the fields requested.
-        :type fields: Optional[str], optional
-        """
-        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/versions/', file_version_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return FileVersionFull.from_dict(json.loads(response.text))
-    def update_file_version_by_id(self, file_id: str, file_version_id: str, trashed_at: Optional[str] = None) -> FileVersionFull:
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/global/boxSkillsCards']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return SkillCardsMetadata.from_dict(json.loads(response.text))
+    def create_file_metadata_global_box_skills_card(self, file_id: str, cards: List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]], extra_headers: Optional[Dict[str, Optional[str]]] = None) -> SkillCardsMetadata:
         """
-        Restores a specific version of a file after it was deleted.
-        
-        Don't use this endpoint to restore Box Notes,
-
-        
-        as it works with file formats such as PDF, DOC,
-
-        
-        PPTX or similar.
-
+        Applies one or more Box Skills metadata cards to a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
             the `file_id` is `123`.
             Example: "12345"
         :type file_id: str
-        :param file_version_id: The ID of the file version
-            Example: "1234"
-        :type file_version_id: str
-        :param trashed_at: Set this to `null` to clear
-            the date and restore the file.
-        :type trashed_at: Optional[str], optional
-        """
-        request_body: BaseObject = BaseObject(trashed_at=trashed_at)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/versions/', file_version_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return FileVersionFull.from_dict(json.loads(response.text))
-    def delete_file_version_by_id(self, file_id: str, file_version_id: str, if_match: Optional[str] = None) -> None:
+        :param cards: A list of Box Skill cards to apply to this file.
+        :type cards: List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]]
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(cards=cards)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/global/boxSkillsCards']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return SkillCardsMetadata.from_dict(json.loads(response.text))
+    def delete_file_metadata_global_box_skills_card(self, file_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
-        Move a file version to the trash.
-        
-        Versions are only tracked for Box users with premium accounts.
-
+        Removes any Box Skills cards metadata from a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
             the `file_id` is `123`.
             Example: "12345"
         :type file_id: str
-        :param file_version_id: The ID of the file version
-            Example: "1234"
-        :type file_version_id: str
-        :param if_match: Ensures this item hasn't recently changed before
-            making changes.
-            Pass in the item's last observed `etag` value
-            into this header and the endpoint will fail
-            with a `412 Precondition Failed` if it
-            has changed since.
-        :type if_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/versions/', file_version_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/global/boxSkillsCards']), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def promote_file_version(self, file_id: str, id: Optional[str] = None, type: Optional[PromoteFileVersionTypeArg] = None, fields: Optional[str] = None) -> FileVersionFull:
+    def update_skill_invocation_by_id(self, skill_id: str, status: UpdateSkillInvocationByIdStatusArg, metadata: UpdateSkillInvocationByIdMetadataArg, file: UpdateSkillInvocationByIdFileArg, file_version: Optional[UpdateSkillInvocationByIdFileVersionArg] = None, usage: Optional[UpdateSkillInvocationByIdUsageArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
-        Promote a specific version of a file.
-        
-        If previous versions exist, this method can be used to
-
-        
-        promote one of the older versions to the top of the version history.
-
-        
-        This creates a new copy of the old version and puts it at the
-
-        
-        top of the versions history. The file will have the exact same contents
-
-        
-        as the older version, with the the same hash digest, `etag`, and
-
-        
-        name as the original.
-
-        
-        Other properties such as comments do not get updated to their
-
-        
-        former values.
-
-        
-        Don't use this endpoint to restore Box Notes,
-
-        
-        as it works with file formats such as PDF, DOC,
-
+        An alternative method that can be used to overwrite and update all Box Skill
         
-        PPTX or similar.
+        metadata cards on a file.
 
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
-        :param id: The file version ID
-        :type id: Optional[str], optional
-        :param type: The type to promote
-        :type type: Optional[PromoteFileVersionTypeArg], optional
-        :param fields: A comma-separated list of attributes to include in the
-            response. This can be used to request fields that are
-            not normally returned in a standard response.
-            Be aware that specifying this parameter will have the
-            effect that none of the standard fields are returned in
-            the response unless explicitly specified, instead only
-            fields for the mini representation are returned, additional
-            to the fields requested.
-        :type fields: Optional[str], optional
-        """
-        request_body: BaseObject = BaseObject(id=id, type=type)
-        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/versions/current']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return FileVersionFull.from_dict(json.loads(response.text))
+        :param skill_id: The ID of the skill to apply this metadata for.
+            Example: "33243242"
+        :type skill_id: str
+        :param status: Defines the status of this invocation. Set this to `success` when setting Skill cards.
+        :type status: UpdateSkillInvocationByIdStatusArg
+        :param metadata: The metadata to set for this skill. This is a list of
+            Box Skills cards. These cards will overwrite any existing Box
+            skill cards on the file.
+        :type metadata: UpdateSkillInvocationByIdMetadataArg
+        :param file: The file to assign the cards to.
+        :type file: UpdateSkillInvocationByIdFileArg
+        :param file_version: The optional file version to assign the cards to.
+        :type file_version: Optional[UpdateSkillInvocationByIdFileVersionArg], optional
+        :param usage: A descriptor that defines what items are affected by this call.
+            Set this to the default values when setting a card to a `success`
+            state, and leave it out in most other situations.
+        :type usage: Optional[UpdateSkillInvocationByIdUsageArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(status=status, metadata=metadata, file=file, file_version=file_version, usage=usage)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/skill_invocations/', skill_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format=None, auth=self.auth, network_session=self.network_session))
+        return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/files.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     PNG = 'png'
     JPG = 'jpg'
 
 class FilesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_by_id(self, file_id: str, fields: Optional[str] = None, if_none_match: Optional[str] = None, boxapi: Optional[str] = None, x_rep_hints: Optional[str] = None) -> FileFull:
+    def get_file_by_id(self, file_id: str, fields: Optional[str] = None, if_none_match: Optional[str] = None, boxapi: Optional[str] = None, x_rep_hints: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Retrieves the details about a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
@@ -198,20 +198,24 @@
             hints.
             `x-rep-hints: [jpg?dimensions=32x32][jpg?dimensions=64x64]`
             Additionally, a `text` representation is available for all
             document file types in Box using the `[extracted_text]`
             representation.
             `x-rep-hints: [extracted_text]`
         :type x_rep_hints: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi), 'x-rep-hints': to_string(x_rep_hints)})
+        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi), 'x-rep-hints': to_string(x_rep_hints), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
-    def update_file_by_id(self, file_id: str, name: Optional[str] = None, description: Optional[str] = None, parent: Optional[UpdateFileByIdParentArg] = None, shared_link: Optional[UpdateFileByIdSharedLinkArg] = None, lock: Optional[UpdateFileByIdLockArg] = None, disposition_at: Optional[str] = None, permissions: Optional[UpdateFileByIdPermissionsArg] = None, collections: Optional[List] = None, tags: Optional[List[str]] = None, fields: Optional[str] = None, if_match: Optional[str] = None) -> FileFull:
+    def update_file_by_id(self, file_id: str, name: Optional[str] = None, description: Optional[str] = None, parent: Optional[UpdateFileByIdParentArg] = None, shared_link: Optional[UpdateFileByIdSharedLinkArg] = None, lock: Optional[UpdateFileByIdLockArg] = None, disposition_at: Optional[str] = None, permissions: Optional[UpdateFileByIdPermissionsArg] = None, collections: Optional[List] = None, tags: Optional[List[str]] = None, fields: Optional[str] = None, if_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Updates a file. This can be used to rename or move a file,
         
         create a shared link, or lock a file.
 
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
@@ -267,21 +271,25 @@
         :param if_match: Ensures this item hasn't recently changed before
             making changes.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `412 Precondition Failed` if it
             has changed since.
         :type if_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, description=description, parent=parent, shared_link=shared_link, lock=lock, disposition_at=disposition_at, permissions=permissions, collections=collections, tags=tags)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match)})
+        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id]), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
-    def delete_file_by_id(self, file_id: str, if_match: Optional[str] = None) -> None:
+    def delete_file_by_id(self, file_id: str, if_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a file, either permanently or by moving it to
         
         the trash.
 
         
         The the enterprise settings determine whether the item will
@@ -300,19 +308,23 @@
         :param if_match: Ensures this item hasn't recently changed before
             making changes.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `412 Precondition Failed` if it
             has changed since.
         :type if_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match)})
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def copy_file(self, file_id: str, parent: CopyFileParentArg, name: Optional[str] = None, version: Optional[str] = None, fields: Optional[str] = None) -> FileFull:
+    def copy_file(self, file_id: str, parent: CopyFileParentArg, name: Optional[str] = None, version: Optional[str] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Creates a copy of a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
@@ -335,20 +347,25 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, version=version, parent=parent)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/copy']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/copy']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
-    def get_file_thumbnail_by_id(self, file_id: str, extension: GetFileThumbnailByIdExtensionArg, min_height: Optional[int] = None, min_width: Optional[int] = None, max_height: Optional[int] = None, max_width: Optional[int] = None) -> ByteStream:
+    def get_file_thumbnail_by_id(self, file_id: str, extension: GetFileThumbnailByIdExtensionArg, min_height: Optional[int] = None, min_width: Optional[int] = None, max_height: Optional[int] = None, max_width: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ByteStream:
         """
         Retrieves a thumbnail, or smaller image representation, of a file.
         
         Sizes of `32x32`,`64x64`, `128x128`, and `256x256` can be returned in
 
         
         the `.png` format and sizes of `32x32`, `160x160`, and `320x320`
@@ -380,11 +397,16 @@
         :type min_height: Optional[int], optional
         :param min_width: The minimum width of the thumbnail
         :type min_width: Optional[int], optional
         :param max_height: The maximum height of the thumbnail
         :type max_height: Optional[int], optional
         :param max_width: The maximum width of the thumbnail
         :type max_width: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'min_height': to_string(min_height), 'min_width': to_string(min_width), 'max_height': to_string(max_height), 'max_width': to_string(max_width)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/thumbnail.', extension]), FetchOptions(method='GET', params=query_params_map, response_format='binary', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/thumbnail.', extension]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='binary', auth=self.auth, network_session=self.network_session))
         return response.content
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_classifications.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/transfer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from box_sdk_gen.base_object import BaseObject
+
 from typing import Optional
 
+from typing import Dict
+
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
-from box_sdk_gen.schemas import Classification
+from box_sdk_gen.schemas import FolderFull
 
 from box_sdk_gen.schemas import ClientError
 
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
@@ -20,99 +24,117 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class FolderClassificationsManager:
+class TransferOwnedFolderOwnedByArg(BaseObject):
+    def __init__(self, id: str, **kwargs):
+        """
+        :param id: The ID of the user who the folder will be
+            transferred to
+        :type id: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+
+class TransferManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_folder_metadata_enterprise_security_classification_6_vm_vochw_u_wo(self, folder_id: str) -> Classification:
+    def transfer_owned_folder(self, user_id: str, owned_by: TransferOwnedFolderOwnedByArg, fields: Optional[str] = None, notify: Optional[bool] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
-        Retrieves the classification metadata instance that
+        Move all of the items (files, folders and workflows) owned by a user into
         
-        has been applied to a folder.
+        another user's account
 
         
-        This API can also be called by including the enterprise ID in the
+        Only the root folder (`0`) can be transferred.
 
         
-        URL explicitly, for example
+        Folders can only be moved across users by users with administrative
 
         
-        `/folders/:id//enterprise_12345/securityClassification-6VMVochwUWo`.
+        permissions.
 
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
-            Example: "12345"
-        :type folder_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/enterprise/securityClassification-6VMVochwUWo']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return Classification.from_dict(json.loads(response.text))
-    def create_folder_metadata_enterprise_security_classification(self, folder_id: str, box_security_classification_key: Optional[str] = None) -> Classification:
-        """
-        Adds a classification to a folder by specifying the label of the
         
-        classification to add.
+        All existing shared links and folder-level collaborations are transferred
 
         
-        This API can also be called by including the enterprise ID in the
+        during the operation. Please note that while collaborations at the individual
 
         
-        URL explicitly, for example
+        file-level are transferred during the operation, the collaborations are
 
         
-        `/folders/:id//enterprise_12345/securityClassification-6VMVochwUWo`.
+        deleted when the original user is deleted.
+
+        
+        This call will be performed synchronously which might lead to a slow response
+
+        
+        when the source user has a large number of items in all of its folders.
+
+        
+        If the destination path has a metadata cascade policy attached to any of
 
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
-            Example: "12345"
-        :type folder_id: str
-        :param box_security_classification_key: The name of the classification to apply to this folder.
-            To list the available classifications in an enterprise,
-            use the classification API to retrieve the
-            [classification template](e://get_metadata_templates_enterprise_securityClassification-6VMVochwUWo_schema)
-            which lists all available classification keys.
-        :type box_security_classification_key: Optional[str], optional
-        """
-        request_body: BaseObject = BaseObject(box_security_classification_key=box_security_classification_key)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/enterprise/securityClassification-6VMVochwUWo']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return Classification.from_dict(json.loads(response.text))
-    def delete_folder_metadata_enterprise_security_classification(self, folder_id: str) -> None:
-        """
-        Removes any classifications from a folder.
         
-        This API can also be called by including the enterprise ID in the
+        the parent folders, a metadata cascade operation will be kicked off
 
         
-        URL explicitly, for example
+        asynchronously.
 
         
-        `/folders/:id//enterprise_12345/securityClassification-6VMVochwUWo`.
+        There is currently no way to check for when this operation is finished.
 
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
+        
+        The destination folder's name will be in the format `{User}'s Files and
+
+        
+        Folders`, where `{User}` is the display name of the user.
+
+        
+        To make this API call your application will need to have the "Read and write
+
+        
+        all files and folders stored in Box" scope enabled.
+
+        
+        Please make sure the destination user has access to `Relay` or `Relay Lite`,
+
+        
+        and has access to the files and folders involved in the workflows being
+
+        
+        transferred.
+
+        
+        Admins will receive an email when the operation is completed.
+
+        :param user_id: The ID of the user.
             Example: "12345"
-        :type folder_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/enterprise/securityClassification-6VMVochwUWo']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
-        return None
+        :type user_id: str
+        :param owned_by: The user who the folder will be transferred to
+        :type owned_by: TransferOwnedFolderOwnedByArg
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param notify: Determines if users should receive email notification
+            for the action performed.
+        :type notify: Optional[bool], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(owned_by=owned_by)
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'notify': to_string(notify)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id, '/folders/0']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return FolderFull.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_locks.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/invites.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 
 from typing import Dict
 
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
-from box_sdk_gen.schemas import FolderLocks
+from box_sdk_gen.schemas import Invite
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import FolderLock
-
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
 from box_sdk_gen.utils import to_string
@@ -26,95 +24,97 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class CreateFolderLockLockedOperationsArg(BaseObject):
-    def __init__(self, move: bool, delete: bool, **kwargs):
+class CreateInviteEnterpriseArg(BaseObject):
+    def __init__(self, id: str, **kwargs):
         """
-        :param move: Whether moving the folder should be locked.
-        :type move: bool
-        :param delete: Whether deleting the folder should be locked.
-        :type delete: bool
+        :param id: The ID of the enterprise
+        :type id: str
         """
         super().__init__(**kwargs)
-        self.move = move
-        self.delete = delete
+        self.id = id
 
-class CreateFolderLockFolderArg(BaseObject):
-    def __init__(self, type: str, id: str, **kwargs):
+class CreateInviteActionableByArg(BaseObject):
+    def __init__(self, login: Optional[str] = None, **kwargs):
         """
-        :param type: The content type the lock is being applied to. Only `folder`
-            is supported.
-        :type type: str
-        :param id: The ID of the folder.
-        :type id: str
+        :param login: The login of the invited user
+        :type login: Optional[str], optional
         """
         super().__init__(**kwargs)
-        self.type = type
-        self.id = id
+        self.login = login
 
-class FolderLocksManager:
+class InvitesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_folder_locks(self, folder_id: str) -> FolderLocks:
+    def create_invite(self, enterprise: CreateInviteEnterpriseArg, actionable_by: CreateInviteActionableByArg, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Invite:
         """
-        Retrieves folder lock details for a given folder.
+        Invites an existing external user to join an enterprise.
         
-        You must be authenticated as the owner or co-owner of the folder to
+        The existing user can not be part of another enterprise and
 
         
-        use this endpoint.
+        must already have a Box account. Once invited, the user will receive an
 
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
-        :type folder_id: str
-        """
-        query_params_map: Dict[str, str] = prepare_params({'folder_id': to_string(folder_id)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folder_locks']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return FolderLocks.from_dict(json.loads(response.text))
-    def create_folder_lock(self, folder: CreateFolderLockFolderArg, locked_operations: Optional[CreateFolderLockLockedOperationsArg] = None) -> FolderLock:
-        """
-        Creates a folder lock on a folder, preventing it from being moved and/or
         
-        deleted.
-
-        
-        You must be authenticated as the owner or co-owner of the folder to
-
-        
-        use this endpoint.
-
-        :param folder: The folder to apply the lock to.
-        :type folder: CreateFolderLockFolderArg
-        :param locked_operations: The operations to lock for the folder. If `locked_operations` is
-            included in the request, both `move` and `delete` must also be
-            included and both set to `true`.
-        :type locked_operations: Optional[CreateFolderLockLockedOperationsArg], optional
-        """
-        request_body: BaseObject = BaseObject(locked_operations=locked_operations, folder=folder)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folder_locks']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return FolderLock.from_dict(json.loads(response.text))
-    def delete_folder_lock_by_id(self, folder_lock_id: str) -> None:
-        """
-        Deletes a folder lock on a given folder.
-        
-        You must be authenticated as the owner or co-owner of the folder to
-
-        
-        use this endpoint.
-
-        :param folder_lock_id: The ID of the folder lock.
-            Example: "12345"
-        :type folder_lock_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folder_locks/', folder_lock_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
-        return None
+        email and are prompted to accept the invitation within the
+
+        
+        Box web application.
+
+        
+        This method requires the "Manage An Enterprise" scope enabled for
+
+        
+        the application, which can be enabled within the developer console.
+
+        :param enterprise: The enterprise to invite the user to
+        :type enterprise: CreateInviteEnterpriseArg
+        :param actionable_by: The user to invite
+        :type actionable_by: CreateInviteActionableByArg
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(enterprise=enterprise, actionable_by=actionable_by)
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/invites']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return Invite.from_dict(json.loads(response.text))
+    def get_invite_by_id(self, invite_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Invite:
+        """
+        Returns the status of a user invite.
+        :param invite_id: The ID of an invite.
+            Example: "213723"
+        :type invite_id: str
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/invites/', invite_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return Invite.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_metadata.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/folder_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import Enum
 
 from typing import Optional
 
+from typing import Dict
+
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import Metadatas
 
 from box_sdk_gen.schemas import ClientError
@@ -40,15 +42,15 @@
     GLOBAL = 'global'
     ENTERPRISE = 'enterprise'
 
 class FolderMetadataManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_folder_metadata(self, folder_id: str) -> Metadatas:
+    def get_folder_metadata(self, folder_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Metadatas:
         """
         Retrieves all metadata for a given folder. This can not be used on the root
         
         folder with ID `0`.
 
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
@@ -56,18 +58,23 @@
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/folder/123`
             the `folder_id` is `123`.
             The root folder of a Box account is
             always represented by the ID `0`.
             Example: "12345"
         :type folder_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Metadatas.from_dict(json.loads(response.text))
-    def get_folder_metadata_by_id(self, folder_id: str, scope: GetFolderMetadataByIdScopeArg, template_key: str) -> Metadata:
+    def get_folder_metadata_by_id(self, folder_id: str, scope: GetFolderMetadataByIdScopeArg, template_key: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Metadata:
         """
         Retrieves the instance of a metadata template that has been applied to a
         
         folder. This can not be used on the root folder with ID `0`.
 
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
@@ -81,18 +88,23 @@
         :type folder_id: str
         :param scope: The scope of the metadata template
             Example: "global"
         :type scope: GetFolderMetadataByIdScopeArg
         :param template_key: The name of the metadata template
             Example: "properties"
         :type template_key: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Metadata.from_dict(json.loads(response.text))
-    def create_folder_metadata_by_id(self, folder_id: str, scope: CreateFolderMetadataByIdScopeArg, template_key: str) -> Metadata:
+    def create_folder_metadata_by_id(self, folder_id: str, scope: CreateFolderMetadataByIdScopeArg, template_key: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Metadata:
         """
         Applies an instance of a metadata template to a folder.
         
         In most cases only values that are present in the metadata template
 
         
         will be accepted, except for the `global.properties` template which accepts
@@ -121,19 +133,24 @@
         :type folder_id: str
         :param scope: The scope of the metadata template
             Example: "global"
         :type scope: CreateFolderMetadataByIdScopeArg
         :param template_key: The name of the metadata template
             Example: "properties"
         :type template_key: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject()
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Metadata.from_dict(json.loads(response.text))
-    def delete_folder_metadata_by_id(self, folder_id: str, scope: DeleteFolderMetadataByIdScopeArg, template_key: str) -> None:
+    def delete_folder_metadata_by_id(self, folder_id: str, scope: DeleteFolderMetadataByIdScopeArg, template_key: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a piece of folder metadata.
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
             by visiting this folder in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/folder/123`
@@ -144,10 +161,15 @@
         :type folder_id: str
         :param scope: The scope of the metadata template
             Example: "global"
         :type scope: DeleteFolderMetadataByIdScopeArg
         :param template_key: The name of the metadata template
             Example: "properties"
         :type template_key: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_watermarks.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/file_watermarks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from enum import Enum
 
 from box_sdk_gen.base_object import BaseObject
 
 from typing import Optional
 
+from typing import Dict
+
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import Watermark
 
 from box_sdk_gen.schemas import ClientError
@@ -24,75 +26,84 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class UpdateFolderWatermarkWatermarkArgImprintField(str, Enum):
+class UpdateFileWatermarkWatermarkArgImprintField(str, Enum):
     DEFAULT = 'default'
 
-class UpdateFolderWatermarkWatermarkArg(BaseObject):
-    def __init__(self, imprint: UpdateFolderWatermarkWatermarkArgImprintField, **kwargs):
+class UpdateFileWatermarkWatermarkArg(BaseObject):
+    def __init__(self, imprint: UpdateFileWatermarkWatermarkArgImprintField, **kwargs):
         """
         :param imprint: The type of watermark to apply.
             Currently only supports one option.
-        :type imprint: UpdateFolderWatermarkWatermarkArgImprintField
+        :type imprint: UpdateFileWatermarkWatermarkArgImprintField
         """
         super().__init__(**kwargs)
         self.imprint = imprint
 
-class FolderWatermarksManager:
+class FileWatermarksManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_folder_watermark(self, folder_id: str) -> Watermark:
+    def get_file_watermark(self, file_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Watermark:
         """
-        Retrieve the watermark for a folder.
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
+        Retrieve the watermark for a file.
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
             and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
             Example: "12345"
-        :type folder_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/watermark']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        :type file_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/watermark']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Watermark.from_dict(json.loads(response.text))
-    def update_folder_watermark(self, folder_id: str, watermark: UpdateFolderWatermarkWatermarkArg) -> Watermark:
+    def update_file_watermark(self, file_id: str, watermark: UpdateFileWatermarkWatermarkArg, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Watermark:
         """
-        Applies or update a watermark on a folder.
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
+        Applies or update a watermark on a file.
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
             and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
             Example: "12345"
-        :type folder_id: str
-        :param watermark: The watermark to imprint on the folder
-        :type watermark: UpdateFolderWatermarkWatermarkArg
+        :type file_id: str
+        :param watermark: The watermark to imprint on the file
+        :type watermark: UpdateFileWatermarkWatermarkArg
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(watermark=watermark)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/watermark']), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/watermark']), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Watermark.from_dict(json.loads(response.text))
-    def delete_folder_watermark(self, folder_id: str) -> None:
+    def delete_file_watermark(self, file_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
-        Removes the watermark from a folder.
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
+        Removes the watermark from a file.
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
             and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
             Example: "12345"
-        :type folder_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/watermark']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        :type file_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/watermark']), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/folders.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/folders.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         super().__init__(**kwargs)
         self.id = id
 
 class FoldersManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_folder_by_id(self, folder_id: str, fields: Optional[str] = None, sort: Optional[GetFolderByIdSortArg] = None, direction: Optional[GetFolderByIdDirectionArg] = None, offset: Optional[int] = None, limit: Optional[int] = None, if_none_match: Optional[str] = None, boxapi: Optional[str] = None) -> FolderFull:
+    def get_folder_by_id(self, folder_id: str, fields: Optional[str] = None, sort: Optional[GetFolderByIdSortArg] = None, direction: Optional[GetFolderByIdDirectionArg] = None, offset: Optional[int] = None, limit: Optional[int] = None, if_none_match: Optional[str] = None, boxapi: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Retrieves details for a folder, including the first 100 entries
         
         in the folder.
 
         
         Passing `sort`, `direction`, `offset`, and `limit`
@@ -284,20 +284,24 @@
             This header can be used to access items that have not been
             explicitly shared with a user.
             Use the format `shared_link=[link]` or if a password is required then
             use `shared_link=[link]&shared_link_password=[password]`.
             This header can be used on the file or folder shared, as well as on any files
             or folders nested within the item.
         :type boxapi: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'sort': to_string(sort), 'direction': to_string(direction), 'offset': to_string(offset), 'limit': to_string(limit)})
-        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi)})
+        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
-    def update_folder_by_id(self, folder_id: str, name: Optional[str] = None, description: Optional[str] = None, sync_state: Optional[UpdateFolderByIdSyncStateArg] = None, can_non_owners_invite: Optional[bool] = None, parent: Optional[UpdateFolderByIdParentArg] = None, shared_link: Optional[UpdateFolderByIdSharedLinkArg] = None, folder_upload_email: Optional[UpdateFolderByIdFolderUploadEmailArg] = None, tags: Optional[List[str]] = None, is_collaboration_restricted_to_enterprise: Optional[bool] = None, collections: Optional[List] = None, can_non_owners_view_collaborators: Optional[bool] = None, fields: Optional[str] = None, if_match: Optional[str] = None) -> FolderFull:
+    def update_folder_by_id(self, folder_id: str, name: Optional[str] = None, description: Optional[str] = None, sync_state: Optional[UpdateFolderByIdSyncStateArg] = None, can_non_owners_invite: Optional[bool] = None, parent: Optional[UpdateFolderByIdParentArg] = None, shared_link: Optional[UpdateFolderByIdSharedLinkArg] = None, folder_upload_email: Optional[UpdateFolderByIdFolderUploadEmailArg] = None, tags: Optional[List[str]] = None, is_collaboration_restricted_to_enterprise: Optional[bool] = None, collections: Optional[List] = None, can_non_owners_view_collaborators: Optional[bool] = None, fields: Optional[str] = None, if_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Updates a folder. This can be also be used to move the folder,
         
         create shared links, update collaborations, and more.
 
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
@@ -364,21 +368,25 @@
         :param if_match: Ensures this item hasn't recently changed before
             making changes.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `412 Precondition Failed` if it
             has changed since.
         :type if_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, description=description, sync_state=sync_state, can_non_owners_invite=can_non_owners_invite, parent=parent, shared_link=shared_link, folder_upload_email=folder_upload_email, tags=tags, is_collaboration_restricted_to_enterprise=is_collaboration_restricted_to_enterprise, collections=collections, can_non_owners_view_collaborators=can_non_owners_view_collaborators)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match)})
+        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id]), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
-    def delete_folder_by_id(self, folder_id: str, recursive: Optional[bool] = None, if_match: Optional[str] = None) -> None:
+    def delete_folder_by_id(self, folder_id: str, recursive: Optional[bool] = None, if_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a folder, either permanently or by moving it to
         
         the trash.
 
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
@@ -396,20 +404,24 @@
         :param if_match: Ensures this item hasn't recently changed before
             making changes.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `412 Precondition Failed` if it
             has changed since.
         :type if_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'recursive': to_string(recursive)})
-        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match)})
+        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id]), FetchOptions(method='DELETE', params=query_params_map, headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def get_folder_items(self, folder_id: str, fields: Optional[str] = None, usemarker: Optional[bool] = None, marker: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None, sort: Optional[GetFolderItemsSortArg] = None, direction: Optional[GetFolderItemsDirectionArg] = None, boxapi: Optional[str] = None) -> Items:
+    def get_folder_items(self, folder_id: str, fields: Optional[str] = None, usemarker: Optional[bool] = None, marker: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None, sort: Optional[GetFolderItemsSortArg] = None, direction: Optional[GetFolderItemsDirectionArg] = None, boxapi: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Items:
         """
         Retrieves a page of items in a folder. These items can be files,
         
         folders, and web links.
 
         
         To request more information about the folder itself, like its size,
@@ -489,20 +501,24 @@
             This header can be used to access items that have not been
             explicitly shared with a user.
             Use the format `shared_link=[link]` or if a password is required then
             use `shared_link=[link]&shared_link_password=[password]`.
             This header can be used on the file or folder shared, as well as on any files
             or folders nested within the item.
         :type boxapi: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'usemarker': to_string(usemarker), 'marker': to_string(marker), 'offset': to_string(offset), 'limit': to_string(limit), 'sort': to_string(sort), 'direction': to_string(direction)})
-        headers_map: Dict[str, str] = prepare_params({'boxapi': to_string(boxapi)})
+        headers_map: Dict[str, str] = prepare_params({'boxapi': to_string(boxapi), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/items']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Items.from_dict(json.loads(response.text))
-    def create_folder(self, name: str, parent: CreateFolderParentArg, folder_upload_email: Optional[CreateFolderFolderUploadEmailArg] = None, sync_state: Optional[CreateFolderSyncStateArg] = None, fields: Optional[str] = None) -> FolderFull:
+    def create_folder(self, name: str, parent: CreateFolderParentArg, folder_upload_email: Optional[CreateFolderFolderUploadEmailArg] = None, sync_state: Optional[CreateFolderSyncStateArg] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Creates a new empty folder within the specified parent folder.
         :param name: The name for the new folder.
             There are some restrictions to the file name. Names containing
             non-printable ASCII characters, forward and backward slashes
             (`/`, `\`), as well as names with trailing spaces are
             prohibited.
@@ -520,20 +536,25 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, parent=parent, folder_upload_email=folder_upload_email, sync_state=sync_state)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
-    def copy_folder(self, folder_id: str, parent: CopyFolderParentArg, name: Optional[str] = None, fields: Optional[str] = None) -> FolderFull:
+    def copy_folder(self, folder_id: str, parent: CopyFolderParentArg, name: Optional[str] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Creates a copy of a folder within a destination folder.
         
         The original folder will not be changed.
 
         :param folder_id: The unique identifier of the folder to copy.
             The ID for any folder can be determined
@@ -559,12 +580,17 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, parent=parent)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/copy']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/copy']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/groups.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/groups.py`

 * *Files 17% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ADMINS_AND_MEMBERS = 'admins_and_members'
     ALL_MANAGED_USERS = 'all_managed_users'
 
 class GroupsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_groups(self, filter_term: Optional[str] = None, fields: Optional[str] = None, limit: Optional[int] = None, offset: Optional[int] = None) -> Groups:
+    def get_groups(self, filter_term: Optional[str] = None, fields: Optional[str] = None, limit: Optional[int] = None, offset: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Groups:
         """
         Retrieves all of the groups for a given enterprise. The user
         
         must have admin permissions to inspect enterprise's groups.
 
         :param filter_term: Limits the results to only groups whose `name` starts
             with the search term.
@@ -77,19 +77,24 @@
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
         :param offset: The offset of the item at which to begin the response.
             Queries with offset parameter value
             exceeding 10000 will be rejected
             with a 400 response.
         :type offset: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'filter_term': to_string(filter_term), 'fields': to_string(fields), 'limit': to_string(limit), 'offset': to_string(offset)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Groups.from_dict(json.loads(response.text))
-    def create_group(self, name: str, provenance: Optional[str] = None, external_sync_identifier: Optional[str] = None, description: Optional[str] = None, invitability_level: Optional[CreateGroupInvitabilityLevelArg] = None, member_viewability_level: Optional[CreateGroupMemberViewabilityLevelArg] = None, fields: Optional[str] = None) -> Group:
+    def create_group(self, name: str, provenance: Optional[str] = None, external_sync_identifier: Optional[str] = None, description: Optional[str] = None, invitability_level: Optional[CreateGroupInvitabilityLevelArg] = None, member_viewability_level: Optional[CreateGroupMemberViewabilityLevelArg] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Group:
         """
         Creates a new group of users in an enterprise. Only users with admin
         
         permissions can create new groups.
 
         :param name: The name of the new group to be created. This name must be unique
             within the enterprise.
@@ -134,20 +139,25 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, provenance=provenance, external_sync_identifier=external_sync_identifier, description=description, invitability_level=invitability_level, member_viewability_level=member_viewability_level)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Group.from_dict(json.loads(response.text))
-    def get_group_by_id(self, group_id: str, fields: Optional[str] = None) -> GroupFull:
+    def get_group_by_id(self, group_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> GroupFull:
         """
         Retrieves information about a group. Only members of this
         
         group or users with admin-level permissions will be able to
 
         
         use this API.
@@ -160,19 +170,24 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return GroupFull.from_dict(json.loads(response.text))
-    def update_group_by_id(self, group_id: str, name: Optional[str] = None, provenance: Optional[str] = None, external_sync_identifier: Optional[str] = None, description: Optional[str] = None, invitability_level: Optional[UpdateGroupByIdInvitabilityLevelArg] = None, member_viewability_level: Optional[UpdateGroupByIdMemberViewabilityLevelArg] = None, fields: Optional[str] = None) -> GroupFull:
+    def update_group_by_id(self, group_id: str, name: Optional[str] = None, provenance: Optional[str] = None, external_sync_identifier: Optional[str] = None, description: Optional[str] = None, invitability_level: Optional[UpdateGroupByIdInvitabilityLevelArg] = None, member_viewability_level: Optional[UpdateGroupByIdMemberViewabilityLevelArg] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> GroupFull:
         """
         Updates a specific group. Only admins of this
         
         group or users with admin-level permissions will be able to
 
         
         use this API.
@@ -223,24 +238,34 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, provenance=provenance, external_sync_identifier=external_sync_identifier, description=description, invitability_level=invitability_level, member_viewability_level=member_viewability_level)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id]), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id]), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return GroupFull.from_dict(json.loads(response.text))
-    def delete_group_by_id(self, group_id: str) -> None:
+    def delete_group_by_id(self, group_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Permanently deletes a group. Only users with
         
         admin-level permissions will be able to use this API.
 
         :param group_id: The ID of the group.
             Example: "57645"
         :type group_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policies.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/trashed_files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Optional
 
+from box_sdk_gen.base_object import BaseObject
+
 from typing import Dict
 
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
-from box_sdk_gen.schemas import LegalHoldPolicies
+from box_sdk_gen.schemas import TrashFileRestored
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import LegalHoldPolicy
+from box_sdk_gen.schemas import TrashFile
 
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
@@ -24,116 +26,133 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class LegalHoldPoliciesManager:
+class RestoreFileFromTrashParentArg(BaseObject):
+    def __init__(self, id: Optional[str] = None, **kwargs):
+        """
+        :param id: The ID of parent item
+        :type id: Optional[str], optional
+        """
+        super().__init__(**kwargs)
+        self.id = id
+
+class TrashedFilesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_legal_hold_policies(self, policy_name: Optional[str] = None, fields: Optional[str] = None, marker: Optional[str] = None, limit: Optional[int] = None) -> LegalHoldPolicies:
+    def restore_file_from_trash(self, file_id: str, name: Optional[str] = None, parent: Optional[RestoreFileFromTrashParentArg] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TrashFileRestored:
         """
-        Retrieves a list of legal hold policies that belong to
+        Restores a file that has been moved to the trash.
         
-        an enterprise.
+        An optional new parent ID can be provided to restore the file to in case the
 
-        :param policy_name: Limits results to policies for which the names start with
-            this search term. This is a case-insensitive prefix.
-        :type policy_name: Optional[str], optional
+        
+        original folder has been deleted.
+
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
+            and copying the ID from the URL. For example,
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
+            Example: "12345"
+        :type file_id: str
+        :param name: An optional new name for the file.
+        :type name: Optional[str], optional
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
-        :param marker: Defines the position marker at which to begin returning results. This is
-            used when paginating using marker-based pagination.
-            This requires `usemarker` to be set to `true`.
-        :type marker: Optional[str], optional
-        :param limit: The maximum number of items to return per page.
-        :type limit: Optional[int], optional
-        """
-        query_params_map: Dict[str, str] = prepare_params({'policy_name': to_string(policy_name), 'fields': to_string(fields), 'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policies']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return LegalHoldPolicies.from_dict(json.loads(response.text))
-    def create_legal_hold_policy(self, policy_name: str, description: Optional[str] = None, filter_started_at: Optional[str] = None, filter_ended_at: Optional[str] = None, is_ongoing: Optional[bool] = None) -> LegalHoldPolicy:
-        """
-        Create a new legal hold policy.
-        :param policy_name: The name of the policy.
-        :type policy_name: str
-        :param description: A description for the policy.
-        :type description: Optional[str], optional
-        :param filter_started_at: The filter start date.
-            When this policy is applied using a `custodian` legal
-            hold assignments, it will only apply to file versions
-            created or uploaded inside of the
-            date range. Other assignment types, such as folders and
-            files, will ignore the date filter.
-            Required if `is_ongoing` is set to `false`.
-        :type filter_started_at: Optional[str], optional
-        :param filter_ended_at: The filter end date.
-            When this policy is applied using a `custodian` legal
-            hold assignments, it will only apply to file versions
-            created or uploaded inside of the
-            date range. Other assignment types, such as folders and
-            files, will ignore the date filter.
-            Required if `is_ongoing` is set to `false`.
-        :type filter_ended_at: Optional[str], optional
-        :param is_ongoing: Whether new assignments under this policy should
-            continue applying to files even after initialization.
-            When this policy is applied using a legal hold assignment,
-            it will continue applying the policy to any new file versions
-            even after it has been applied.
-            For example, if a legal hold assignment is placed on a user
-            today, and that user uploads a file tomorrow, that file will
-            get held. This will continue until the policy is retired.
-            Required if no filter dates are set.
-        :type is_ongoing: Optional[bool], optional
-        """
-        request_body: BaseObject = BaseObject(policy_name=policy_name, description=description, filter_started_at=filter_started_at, filter_ended_at=filter_ended_at, is_ongoing=is_ongoing)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policies']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return LegalHoldPolicy.from_dict(json.loads(response.text))
-    def get_legal_hold_policy_by_id(self, legal_hold_policy_id: str) -> LegalHoldPolicy:
-        """
-        Retrieve a legal hold policy.
-        :param legal_hold_policy_id: The ID of the legal hold policy
-            Example: "324432"
-        :type legal_hold_policy_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policies/', legal_hold_policy_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return LegalHoldPolicy.from_dict(json.loads(response.text))
-    def update_legal_hold_policy_by_id(self, legal_hold_policy_id: str, policy_name: Optional[str] = None, description: Optional[str] = None, release_notes: Optional[str] = None) -> LegalHoldPolicy:
-        """
-        Update legal hold policy.
-        :param legal_hold_policy_id: The ID of the legal hold policy
-            Example: "324432"
-        :type legal_hold_policy_id: str
-        :param policy_name: The name of the policy.
-        :type policy_name: Optional[str], optional
-        :param description: A description for the policy.
-        :type description: Optional[str], optional
-        :param release_notes: Notes around why the policy was released.
-        :type release_notes: Optional[str], optional
-        """
-        request_body: BaseObject = BaseObject(policy_name=policy_name, description=description, release_notes=release_notes)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policies/', legal_hold_policy_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return LegalHoldPolicy.from_dict(json.loads(response.text))
-    def delete_legal_hold_policy_by_id(self, legal_hold_policy_id: str) -> None:
-        """
-        Delete an existing legal hold policy.
-        
-        This is an asynchronous process. The policy will not be
-
-        
-        fully deleted yet when the response returns.
-
-        :param legal_hold_policy_id: The ID of the legal hold policy
-            Example: "324432"
-        :type legal_hold_policy_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(name=name, parent=parent)
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id]), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return TrashFileRestored.from_dict(json.loads(response.text))
+    def get_file_trash(self, file_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TrashFile:
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policies/', legal_hold_policy_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        Retrieves a file that has been moved to the trash.
+        
+        Please note that only if the file itself has been moved to the
+
+        
+        trash can it be retrieved with this API call. If instead one of
+
+        
+        its parent folders was moved to the trash, only that folder
+
+        
+        can be inspected using the
+
+        
+        [`GET /folders/:id/trash`](e://get_folders_id_trash) API.
+
+        
+        To list all items that have been moved to the trash, please
+
+        
+        use the [`GET /folders/trash/items`](e://get-folders-trash-items/)
+
+        
+        API.
+
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
+            and copying the ID from the URL. For example,
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
+            Example: "12345"
+        :type file_id: str
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/trash']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return TrashFile.from_dict(json.loads(response.text))
+    def delete_file_trash(self, file_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
+        """
+        Permanently deletes a file that is in the trash.
+        
+        This action cannot be undone.
+
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
+            and copying the ID from the URL. For example,
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
+            Example: "12345"
+        :type file_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/trash']), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policy_assignments.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/legal_hold_policy_assignments.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.type = type
         self.id = id
 
 class LegalHoldPolicyAssignmentsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_legal_hold_policy_assignments(self, policy_id: str, assign_to_type: Optional[GetLegalHoldPolicyAssignmentsAssignToTypeArg] = None, assign_to_id: Optional[str] = None, marker: Optional[str] = None, limit: Optional[int] = None, fields: Optional[str] = None) -> LegalHoldPolicyAssignments:
+    def get_legal_hold_policy_assignments(self, policy_id: str, assign_to_type: Optional[GetLegalHoldPolicyAssignmentsAssignToTypeArg] = None, assign_to_id: Optional[str] = None, marker: Optional[str] = None, limit: Optional[int] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> LegalHoldPolicyAssignments:
         """
         Retrieves a list of items a legal hold policy has been assigned to.
         :param policy_id: The ID of the legal hold policy
         :type policy_id: str
         :param assign_to_type: Filters the results by the type of item the
             policy was applied to.
         :type assign_to_type: Optional[GetLegalHoldPolicyAssignmentsAssignToTypeArg], optional
@@ -84,54 +84,74 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'policy_id': to_string(policy_id), 'assign_to_type': to_string(assign_to_type), 'assign_to_id': to_string(assign_to_id), 'marker': to_string(marker), 'limit': to_string(limit), 'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return LegalHoldPolicyAssignments.from_dict(json.loads(response.text))
-    def create_legal_hold_policy_assignment(self, policy_id: str, assign_to: CreateLegalHoldPolicyAssignmentAssignToArg) -> LegalHoldPolicyAssignment:
+    def create_legal_hold_policy_assignment(self, policy_id: str, assign_to: CreateLegalHoldPolicyAssignmentAssignToArg, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> LegalHoldPolicyAssignment:
         """
         Assign a legal hold to a file, file version, folder, or user.
         :param policy_id: The ID of the policy to assign.
         :type policy_id: str
         :param assign_to: The item to assign the policy to
         :type assign_to: CreateLegalHoldPolicyAssignmentAssignToArg
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(policy_id=policy_id, assign_to=assign_to)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return LegalHoldPolicyAssignment.from_dict(json.loads(response.text))
-    def get_legal_hold_policy_assignment_by_id(self, legal_hold_policy_assignment_id: str) -> LegalHoldPolicyAssignment:
+    def get_legal_hold_policy_assignment_by_id(self, legal_hold_policy_assignment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> LegalHoldPolicyAssignment:
         """
         Retrieve a legal hold policy assignment.
         :param legal_hold_policy_assignment_id: The ID of the legal hold policy assignment
             Example: "753465"
         :type legal_hold_policy_assignment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return LegalHoldPolicyAssignment.from_dict(json.loads(response.text))
-    def delete_legal_hold_policy_assignment_by_id(self, legal_hold_policy_assignment_id: str) -> None:
+    def delete_legal_hold_policy_assignment_by_id(self, legal_hold_policy_assignment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Remove a legal hold from an item.
         
         This is an asynchronous process. The policy will not be
 
         
         fully removed yet when the response returns.
 
         :param legal_hold_policy_assignment_id: The ID of the legal hold policy assignment
             Example: "753465"
         :type legal_hold_policy_assignment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def get_legal_hold_policy_assignment_file_on_hold(self, legal_hold_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None, fields: Optional[str] = None) -> FileVersionLegalHolds:
+    def get_legal_hold_policy_assignment_file_on_hold(self, legal_hold_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileVersionLegalHolds:
         """
         Get a list of current file versions for a legal hold
         
         assignment.
 
         
         In some cases you may want to get previous file versions instead. In these
@@ -180,19 +200,24 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit), 'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id, '/files_on_hold']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id, '/files_on_hold']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileVersionLegalHolds.from_dict(json.loads(response.text))
-    def get_legal_hold_policy_assignment_file_version_on_hold(self, legal_hold_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None, fields: Optional[str] = None) -> FileVersionLegalHolds:
+    def get_legal_hold_policy_assignment_file_version_on_hold(self, legal_hold_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileVersionLegalHolds:
         """
         Get a list of previous file versions for a legal hold
         
         assignment.
 
         
         In some cases you may only need the latest file versions instead. In these
@@ -241,11 +266,16 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit), 'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id, '/file_versions_on_hold']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/legal_hold_policy_assignments/', legal_hold_policy_assignment_id, '/file_versions_on_hold']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileVersionLegalHolds.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/memberships.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/memberships.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 class MembershipsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_user_memberships(self, user_id: str, limit: Optional[int] = None, offset: Optional[int] = None) -> GroupMemberships:
+    def get_user_memberships(self, user_id: str, limit: Optional[int] = None, offset: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> GroupMemberships:
         """
         Retrieves all the groups for a user. Only members of this
         
         group or users with admin-level permissions will be able to
 
         
         use this API.
@@ -85,19 +85,24 @@
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
         :param offset: The offset of the item at which to begin the response.
             Queries with offset parameter value
             exceeding 10000 will be rejected
             with a 400 response.
         :type offset: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'limit': to_string(limit), 'offset': to_string(offset)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id, '/memberships']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id, '/memberships']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return GroupMemberships.from_dict(json.loads(response.text))
-    def get_group_memberships(self, group_id: str, limit: Optional[int] = None, offset: Optional[int] = None) -> GroupMemberships:
+    def get_group_memberships(self, group_id: str, limit: Optional[int] = None, offset: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> GroupMemberships:
         """
         Retrieves all the members for a group. Only members of this
         
         group or users with admin-level permissions will be able to
 
         
         use this API.
@@ -108,19 +113,24 @@
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
         :param offset: The offset of the item at which to begin the response.
             Queries with offset parameter value
             exceeding 10000 will be rejected
             with a 400 response.
         :type offset: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'limit': to_string(limit), 'offset': to_string(offset)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id, '/memberships']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id, '/memberships']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return GroupMemberships.from_dict(json.loads(response.text))
-    def create_group_membership(self, user: CreateGroupMembershipUserArg, group: CreateGroupMembershipGroupArg, role: Optional[CreateGroupMembershipRoleArg] = None, configurable_permissions: Optional[CreateGroupMembershipConfigurablePermissionsArg] = None, fields: Optional[str] = None) -> GroupMembership:
+    def create_group_membership(self, user: CreateGroupMembershipUserArg, group: CreateGroupMembershipGroupArg, role: Optional[CreateGroupMembershipRoleArg] = None, configurable_permissions: Optional[CreateGroupMembershipConfigurablePermissionsArg] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> GroupMembership:
         """
         Creates a group membership. Only users with
         
         admin-level permissions will be able to use this API.
 
         :param user: The user to add to the group.
         :type user: CreateGroupMembershipUserArg
@@ -142,20 +152,25 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(user=user, group=group, role=role, configurable_permissions=configurable_permissions)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return GroupMembership.from_dict(json.loads(response.text))
-    def get_group_membership_by_id(self, group_membership_id: str, fields: Optional[str] = None) -> GroupMembership:
+    def get_group_membership_by_id(self, group_membership_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> GroupMembership:
         """
         Retrieves a specific group membership. Only admins of this
         
         group or users with admin-level permissions will be able to
 
         
         use this API.
@@ -168,19 +183,24 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships/', group_membership_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships/', group_membership_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return GroupMembership.from_dict(json.loads(response.text))
-    def update_group_membership_by_id(self, group_membership_id: str, role: Optional[UpdateGroupMembershipByIdRoleArg] = None, configurable_permissions: Optional[UpdateGroupMembershipByIdConfigurablePermissionsArg] = None, fields: Optional[str] = None) -> GroupMembership:
+    def update_group_membership_by_id(self, group_membership_id: str, role: Optional[UpdateGroupMembershipByIdRoleArg] = None, configurable_permissions: Optional[UpdateGroupMembershipByIdConfigurablePermissionsArg] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> GroupMembership:
         """
         Updates a user's group membership. Only admins of this
         
         group or users with admin-level permissions will be able to
 
         
         use this API.
@@ -204,27 +224,37 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(role=role, configurable_permissions=configurable_permissions)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships/', group_membership_id]), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships/', group_membership_id]), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return GroupMembership.from_dict(json.loads(response.text))
-    def delete_group_membership_by_id(self, group_membership_id: str) -> None:
+    def delete_group_membership_by_id(self, group_membership_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a specific group membership. Only admins of this
         
         group or users with admin-level permissions will be able to
 
         
         use this API.
 
         :param group_membership_id: The ID of the group membership.
             Example: "434534"
         :type group_membership_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships/', group_membership_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/group_memberships/', group_membership_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/metadata_templates.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/list_collaborations.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,18 @@
 
 from typing import Optional
 
 from typing import Dict
 
 import json
 
-from typing import List
-
-from typing import Union
-
-from box_sdk_gen.base_object import BaseObject
-
-from box_sdk_gen.schemas import MetadataTemplates
+from box_sdk_gen.schemas import Collaborations
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import MetadataTemplate
-
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
 from box_sdk_gen.utils import to_string
@@ -30,140 +22,151 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class GetMetadataTemplateSchemaScopeArg(str, Enum):
-    GLOBAL = 'global'
-    ENTERPRISE = 'enterprise'
-
-class DeleteMetadataTemplateSchemaScopeArg(str, Enum):
-    GLOBAL = 'global'
-    ENTERPRISE = 'enterprise'
+class GetCollaborationsStatusArg(str, Enum):
+    PENDING = 'pending'
 
-class MetadataTemplatesManager:
+class ListCollaborationsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_metadata_templates(self, metadata_instance_id: str) -> MetadataTemplates:
-        """
-        Finds a metadata template by searching for the ID of an instance of the
-        
-        template.
-
-        :param metadata_instance_id: The ID of an instance of the metadata template to find.
-        :type metadata_instance_id: str
-        """
-        query_params_map: Dict[str, str] = prepare_params({'metadata_instance_id': to_string(metadata_instance_id)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return MetadataTemplates.from_dict(json.loads(response.text))
-    def get_metadata_template_schema(self, scope: GetMetadataTemplateSchemaScopeArg, template_key: str) -> MetadataTemplate:
+    def get_file_collaborations(self, file_id: str, fields: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collaborations:
         """
-        Retrieves a metadata template by its `scope` and `templateKey` values.
+        Retrieves a list of pending and active collaborations for a
         
-        To find the `scope` and `templateKey` for a template, list all templates for
+        file. This returns all the users that have access to the file
 
         
-        an enterprise or globally, or list all templates applied to a file or folder.
-
-        :param scope: The scope of the metadata template
-            Example: "global"
-        :type scope: GetMetadataTemplateSchemaScopeArg
-        :param template_key: The name of the metadata template
-            Example: "properties"
-        :type template_key: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/', scope, '/', template_key, '/schema']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return MetadataTemplate.from_dict(json.loads(response.text))
-    def delete_metadata_template_schema(self, scope: DeleteMetadataTemplateSchemaScopeArg, template_key: str) -> None:
-        """
-        Delete a metadata template and its instances.
-        
-        This deletion is permanent and can not be reversed.
-
-        :param scope: The scope of the metadata template
-            Example: "global"
-        :type scope: DeleteMetadataTemplateSchemaScopeArg
-        :param template_key: The name of the metadata template
-            Example: "properties"
-        :type template_key: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/', scope, '/', template_key, '/schema']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
-        return None
-    def get_metadata_template_by_id(self, template_id: str) -> MetadataTemplate:
-        """
-        Retrieves a metadata template by its ID.
-        :param template_id: The ID of the template
-            Example: "f7a9891f"
-        :type template_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/', template_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return MetadataTemplate.from_dict(json.loads(response.text))
-    def get_metadata_template_global(self, marker: Optional[str] = None, limit: Optional[int] = None) -> MetadataTemplates:
-        """
-        Used to retrieve all generic, global metadata templates available to all
-        
-        enterprises using Box.
+        or have been invited to the file.
 
+        :param file_id: The unique identifier that represents a file.
+            The ID for any file can be determined
+            by visiting a file in the web application
+            and copying the ID from the URL. For example,
+            for the URL `https://*.app.box.com/files/123`
+            the `file_id` is `123`.
+            Example: "12345"
+        :type file_id: str
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param limit: The maximum number of items to return per page.
+        :type limit: Optional[int], optional
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'limit': to_string(limit), 'marker': to_string(marker)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/collaborations']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return Collaborations.from_dict(json.loads(response.text))
+    def get_folder_collaborations(self, folder_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collaborations:
+        """
+        Retrieves a list of pending and active collaborations for a
+        
+        folder. This returns all the users that have access to the folder
+
+        
+        or have been invited to the folder.
+
+        :param folder_id: The unique identifier that represent a folder.
+            The ID for any folder can be determined
+            by visiting this folder in the web application
+            and copying the ID from the URL. For example,
+            for the URL `https://*.app.box.com/folder/123`
+            the `folder_id` is `123`.
+            Example: "12345"
+        :type folder_id: str
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/collaborations']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return Collaborations.from_dict(json.loads(response.text))
+    def get_collaborations(self, status: GetCollaborationsStatusArg, fields: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collaborations:
+        """
+        Retrieves all pending collaboration invites for this user.
+        :param status: The status of the collaborations to retrieve
+        :type status: GetCollaborationsStatusArg
+        :param fields: A comma-separated list of attributes to include in the
+            response. This can be used to request fields that are
+            not normally returned in a standard response.
+            Be aware that specifying this parameter will have the
+            effect that none of the standard fields are returned in
+            the response unless explicitly specified, instead only
+            fields for the mini representation are returned, additional
+            to the fields requested.
+        :type fields: Optional[str], optional
+        :param offset: The offset of the item at which to begin the response.
+            Queries with offset parameter value
+            exceeding 10000 will be rejected
+            with a 400 response.
+        :type offset: Optional[int], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/global']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return MetadataTemplates.from_dict(json.loads(response.text))
-    def get_metadata_template_enterprise(self, marker: Optional[str] = None, limit: Optional[int] = None) -> MetadataTemplates:
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'status': to_string(status), 'fields': to_string(fields), 'offset': to_string(offset), 'limit': to_string(limit)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return Collaborations.from_dict(json.loads(response.text))
+    def get_group_collaborations(self, group_id: str, limit: Optional[int] = None, offset: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collaborations:
         """
-        Used to retrieve all metadata templates created to be used specifically within
+        Retrieves all the collaborations for a group. The user
         
-        the user's enterprise
+        must have admin permissions to inspect enterprise's groups.
 
-        :param marker: Defines the position marker at which to begin returning results. This is
-            used when paginating using marker-based pagination.
-            This requires `usemarker` to be set to `true`.
-        :type marker: Optional[str], optional
+        
+        Each collaboration object has details on which files or
+
+        
+        folders the group has access to and with what role.
+
+        :param group_id: The ID of the group.
+            Example: "57645"
+        :type group_id: str
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
-        """
-        query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/enterprise']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return MetadataTemplates.from_dict(json.loads(response.text))
-    def create_metadata_template_schema(self, scope: str, display_name: str, template_key: Optional[str] = None, hidden: Optional[bool] = None, fields: Optional[List] = None, copy_instance_on_item_copy: Optional[bool] = None) -> MetadataTemplate:
-        """
-        Creates a new metadata template that can be applied to
-        
-        files and folders.
-
-        :param scope: The scope of the metadata template to create. Applications can
-            only create templates for use within the authenticated user's
-            enterprise.
-            This value needs to be set to `enterprise`, as `global` scopes can
-            not be created by applications.
-        :type scope: str
-        :param display_name: The display name of the template.
-        :type display_name: str
-        :param template_key: A unique identifier for the template. This identifier needs to be
-            unique across the enterprise for which the metadata template is
-            being created.
-            When not provided, the API will create a unique `templateKey`
-            based on the value of the `displayName`.
-        :type template_key: Optional[str], optional
-        :param hidden: Defines if this template is visible in the Box web app UI, or if
-            it is purely intended for usage through the API.
-        :type hidden: Optional[bool], optional
-        :param fields: An ordered list of template fields which are part of the template.
-            Each field can be a regular text field, date field, number field,
-            as well as a single or multi-select list.
-        :type fields: Optional[List], optional
-        :param copy_instance_on_item_copy: Whether or not to copy any metadata attached to a file or folder
-            when it is copied. By default, metadata is not copied along with a
-            file or folder when it is copied.
-        :type copy_instance_on_item_copy: Optional[bool], optional
-        """
-        request_body: BaseObject = BaseObject(scope=scope, template_key=template_key, display_name=display_name, hidden=hidden, fields=fields, copy_instance_on_item_copy=copy_instance_on_item_copy)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_templates/schema']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return MetadataTemplate.from_dict(json.loads(response.text))
+        :param offset: The offset of the item at which to begin the response.
+            Queries with offset parameter value
+            exceeding 10000 will be rejected
+            with a 400 response.
+        :type offset: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'limit': to_string(limit), 'offset': to_string(offset)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/', group_id, '/collaborations']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return Collaborations.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policies.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/retention_policies.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     PERMANENTLY_DELETE = 'permanently_delete'
     REMOVE_RETENTION = 'remove_retention'
 
 class RetentionPoliciesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_retention_policies(self, policy_name: Optional[str] = None, policy_type: Optional[GetRetentionPoliciesPolicyTypeArg] = None, created_by_user_id: Optional[str] = None, fields: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None) -> RetentionPolicies:
+    def get_retention_policies(self, policy_name: Optional[str] = None, policy_type: Optional[GetRetentionPoliciesPolicyTypeArg] = None, created_by_user_id: Optional[str] = None, fields: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RetentionPolicies:
         """
         Retrieves all of the retention policies for an enterprise.
         :param policy_name: Filters results by a case sensitive prefix of the name of
             retention policies.
         :type policy_name: Optional[str], optional
         :param policy_type: Filters results by the type of retention policy.
         :type policy_type: Optional[GetRetentionPoliciesPolicyTypeArg], optional
@@ -78,19 +78,24 @@
             to the fields requested.
         :type fields: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
         :type marker: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'policy_name': to_string(policy_name), 'policy_type': to_string(policy_type), 'created_by_user_id': to_string(created_by_user_id), 'fields': to_string(fields), 'limit': to_string(limit), 'marker': to_string(marker)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return RetentionPolicies.from_dict(json.loads(response.text))
-    def create_retention_policy(self, policy_name: str, policy_type: CreateRetentionPolicyPolicyTypeArg, disposition_action: CreateRetentionPolicyDispositionActionArg, description: Optional[str] = None, retention_length: Optional[str] = None, retention_type: Optional[CreateRetentionPolicyRetentionTypeArg] = None, can_owner_extend_retention: Optional[bool] = None, are_owners_notified: Optional[bool] = None, custom_notification_recipients: Optional[List[UserMini]] = None) -> RetentionPolicy:
+    def create_retention_policy(self, policy_name: str, policy_type: CreateRetentionPolicyPolicyTypeArg, disposition_action: CreateRetentionPolicyDispositionActionArg, description: Optional[str] = None, retention_length: Optional[str] = None, retention_type: Optional[CreateRetentionPolicyRetentionTypeArg] = None, can_owner_extend_retention: Optional[bool] = None, are_owners_notified: Optional[bool] = None, custom_notification_recipients: Optional[List[UserMini]] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RetentionPolicy:
         """
         Creates a retention policy.
         :param policy_name: The name for the retention policy
         :type policy_name: str
         :param policy_type: The type of the retention policy. A retention
             policy type can either be `finite`, where a
             specific amount of time to retain the content is known
@@ -132,38 +137,48 @@
         :type can_owner_extend_retention: Optional[bool], optional
         :param are_owners_notified: Whether owner and co-owners of a file are notified
             when the policy nears expiration.
         :type are_owners_notified: Optional[bool], optional
         :param custom_notification_recipients: A list of users notified when
             the retention policy duration is about to end.
         :type custom_notification_recipients: Optional[List[UserMini]], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(policy_name=policy_name, description=description, policy_type=policy_type, disposition_action=disposition_action, retention_length=retention_length, retention_type=retention_type, can_owner_extend_retention=can_owner_extend_retention, are_owners_notified=are_owners_notified, custom_notification_recipients=custom_notification_recipients)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return RetentionPolicy.from_dict(json.loads(response.text))
-    def get_retention_policy_by_id(self, retention_policy_id: str, fields: Optional[str] = None) -> RetentionPolicy:
+    def get_retention_policy_by_id(self, retention_policy_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RetentionPolicy:
         """
         Retrieves a retention policy.
         :param retention_policy_id: The ID of the retention policy.
             Example: "982312"
         :type retention_policy_id: str
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return RetentionPolicy.from_dict(json.loads(response.text))
-    def update_retention_policy_by_id(self, retention_policy_id: str, policy_name: Optional[str] = None, description: Optional[str] = None, disposition_action: Optional[UpdateRetentionPolicyByIdDispositionActionArg] = None, retention_type: Optional[str] = None, retention_length: Optional[str] = None, status: Optional[str] = None, can_owner_extend_retention: Optional[bool] = None, are_owners_notified: Optional[bool] = None, custom_notification_recipients: Optional[List[UserMini]] = None) -> RetentionPolicy:
+    def update_retention_policy_by_id(self, retention_policy_id: str, policy_name: Optional[str] = None, description: Optional[str] = None, disposition_action: Optional[UpdateRetentionPolicyByIdDispositionActionArg] = None, retention_type: Optional[str] = None, retention_length: Optional[str] = None, status: Optional[str] = None, can_owner_extend_retention: Optional[bool] = None, are_owners_notified: Optional[bool] = None, custom_notification_recipients: Optional[List[UserMini]] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RetentionPolicy:
         """
         Updates a retention policy.
         :param retention_policy_id: The ID of the retention policy.
             Example: "982312"
         :type retention_policy_id: str
         :param policy_name: The name for the retention policy
         :type policy_name: Optional[str], optional
@@ -211,20 +226,30 @@
         :type can_owner_extend_retention: Optional[bool], optional
         :param are_owners_notified: Determines if owners and co-owners of items
             under the policy are notified when
             the retention duration is about to end.
         :type are_owners_notified: Optional[bool], optional
         :param custom_notification_recipients: A list of users notified when the retention duration is about to end.
         :type custom_notification_recipients: Optional[List[UserMini]], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(policy_name=policy_name, description=description, disposition_action=disposition_action, retention_type=retention_type, retention_length=retention_length, status=status, can_owner_extend_retention=can_owner_extend_retention, are_owners_notified=are_owners_notified, custom_notification_recipients=custom_notification_recipients)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return RetentionPolicy.from_dict(json.loads(response.text))
-    def delete_retention_policy_by_id(self, retention_policy_id: str) -> None:
+    def delete_retention_policy_by_id(self, retention_policy_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Permanently deletes a retention policy.
         :param retention_policy_id: The ID of the retention policy.
             Example: "982312"
         :type retention_policy_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policy_assignments.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/retention_policy_assignments.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self.type = type
         self.id = id
 
 class RetentionPolicyAssignmentsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_retention_policy_assignments(self, retention_policy_id: str, type: Optional[GetRetentionPolicyAssignmentsTypeArg] = None, fields: Optional[str] = None, marker: Optional[str] = None, limit: Optional[int] = None) -> RetentionPolicyAssignments:
+    def get_retention_policy_assignments(self, retention_policy_id: str, type: Optional[GetRetentionPolicyAssignmentsTypeArg] = None, fields: Optional[str] = None, marker: Optional[str] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RetentionPolicyAssignments:
         """
         Returns a list of all retention policy assignments associated with a specified
         
         retention policy.
 
         :param retention_policy_id: The ID of the retention policy.
             Example: "982312"
@@ -85,19 +85,24 @@
             to the fields requested.
         :type fields: Optional[str], optional
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
         :type marker: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'type': to_string(type), 'fields': to_string(fields), 'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id, '/assignments']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policies/', retention_policy_id, '/assignments']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return RetentionPolicyAssignments.from_dict(json.loads(response.text))
-    def create_retention_policy_assignment(self, policy_id: str, assign_to: CreateRetentionPolicyAssignmentAssignToArg, filter_fields: Optional[List] = None, start_date_field: Optional[str] = None) -> RetentionPolicyAssignment:
+    def create_retention_policy_assignment(self, policy_id: str, assign_to: CreateRetentionPolicyAssignmentAssignToArg, filter_fields: Optional[List] = None, start_date_field: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RetentionPolicyAssignment:
         """
         Assigns a retention policy to an item.
         :param policy_id: The ID of the retention policy to assign
         :type policy_id: str
         :param assign_to: The item to assign the policy to
         :type assign_to: CreateRetentionPolicyAssignmentAssignToArg
         :param filter_fields: If the `assign_to` type is `metadata_template`,
@@ -105,77 +110,102 @@
             require an array of objects with a field entry and a value entry.
             Currently only one object of `field` and `value` is supported.
         :type filter_fields: Optional[List], optional
         :param start_date_field: The date the retention policy assignment begins.
             If the `assigned_to` type is `metadata_template`,
             this field can be a date field's metadata attribute key id.
         :type start_date_field: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(policy_id=policy_id, assign_to=assign_to, filter_fields=filter_fields, start_date_field=start_date_field)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return RetentionPolicyAssignment.from_dict(json.loads(response.text))
-    def get_retention_policy_assignment_by_id(self, retention_policy_assignment_id: str, fields: Optional[str] = None) -> RetentionPolicyAssignment:
+    def get_retention_policy_assignment_by_id(self, retention_policy_assignment_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> RetentionPolicyAssignment:
         """
         Retrieves a retention policy assignment
         :param retention_policy_assignment_id: The ID of the retention policy assignment.
             Example: "1233123"
         :type retention_policy_assignment_id: str
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return RetentionPolicyAssignment.from_dict(json.loads(response.text))
-    def delete_retention_policy_assignment_by_id(self, retention_policy_assignment_id: str) -> None:
+    def delete_retention_policy_assignment_by_id(self, retention_policy_assignment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Removes a retention policy assignment
         
         applied to content.
 
         :param retention_policy_assignment_id: The ID of the retention policy assignment.
             Example: "1233123"
         :type retention_policy_assignment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def get_retention_policy_assignment_file_under_retention(self, retention_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None) -> FilesUnderRetention:
+    def get_retention_policy_assignment_file_under_retention(self, retention_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FilesUnderRetention:
         """
         Returns a list of files under retention for a retention policy assignment.
         :param retention_policy_assignment_id: The ID of the retention policy assignment.
             Example: "1233123"
         :type retention_policy_assignment_id: str
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id, '/files_under_retention']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id, '/files_under_retention']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FilesUnderRetention.from_dict(json.loads(response.text))
-    def get_retention_policy_assignment_file_version_under_retention(self, retention_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None) -> FilesUnderRetention:
+    def get_retention_policy_assignment_file_version_under_retention(self, retention_policy_assignment_id: str, marker: Optional[str] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FilesUnderRetention:
         """
         Returns a list of file versions under retention for a retention policy
         
         assignment.
 
         :param retention_policy_assignment_id: The ID of the retention policy assignment.
             Example: "1233123"
         :type retention_policy_assignment_id: str
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id, '/file_versions_under_retention']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/retention_policy_assignments/', retention_policy_assignment_id, '/file_versions_under_retention']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FilesUnderRetention.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/search.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 
 from typing import Optional
 
 from typing import List
 
 from typing import Union
 
-import json
-
 from typing import Dict
 
-from box_sdk_gen.base_object import BaseObject
+import json
 
 from box_sdk_gen.schemas import MetadataQueryResults
 
 from box_sdk_gen.schemas import ClientError
 
 from box_sdk_gen.schemas import MetadataQuery
 
@@ -74,15 +72,15 @@
     DESC = 'DESC'
     ASC = 'ASC'
 
 class SearchManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def create_metadata_query_execute_read(self, from_: str, ancestor_folder_id: str, query: Optional[str] = None, query_params: Optional[CreateMetadataQueryExecuteReadQueryParamsArg] = None, order_by: Optional[List] = None, limit: Optional[int] = None, marker: Optional[str] = None, fields: Optional[List[str]] = None) -> MetadataQueryResults:
+    def create_metadata_query_execute_read(self, from_: str, ancestor_folder_id: str, query: Optional[str] = None, query_params: Optional[CreateMetadataQueryExecuteReadQueryParamsArg] = None, order_by: Optional[List] = None, limit: Optional[int] = None, marker: Optional[str] = None, fields: Optional[List[str]] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> MetadataQueryResults:
         """
         Create a search using SQL-like syntax to return items that match specific
         
         metadata.
 
         
         By default, this endpoint returns only the most basic info about the items for
@@ -136,30 +134,40 @@
             * `metadata.<scope>.<templateKey>` will return the mini-representation
             of the metadata instance identified by the `scope` and `templateKey`.
             * `metadata.<scope>.<templateKey>.<field>` will return all the mini-representation
             of the metadata instance identified by the `scope` and `templateKey` plus
             the field specified by the `field` name. Multiple fields for the same
             `scope` and `templateKey` can be defined.
         :type fields: Optional[List[str]], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        request_body: BaseObject = BaseObject(from_=from_, query=query, query_params=query_params, ancestor_folder_id=ancestor_folder_id, order_by=order_by, limit=limit, marker=marker, fields=fields)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_queries/execute_read']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: MetadataQuery = MetadataQuery(from_=from_, query=query, query_params=query_params, ancestor_folder_id=ancestor_folder_id, order_by=order_by, limit=limit, marker=marker, fields=fields)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_queries/execute_read']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return MetadataQueryResults.from_dict(json.loads(response.text))
-    def get_metadata_query_indices(self, scope: GetMetadataQueryIndicesScopeArg, template_key: str) -> MetadataQueryIndices:
+    def get_metadata_query_indices(self, scope: GetMetadataQueryIndicesScopeArg, template_key: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> MetadataQueryIndices:
         """
         Retrieves the metadata query indices for a given scope and template key.
         :param scope: The scope of the metadata template
         :type scope: GetMetadataQueryIndicesScopeArg
         :param template_key: The name of the metadata template
         :type template_key: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'scope': to_string(scope), 'template_key': to_string(template_key)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_query_indices']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/metadata_query_indices']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return MetadataQueryIndices.from_dict(json.loads(response.text))
-    def get_search(self, query: Optional[str] = None, scope: Optional[GetSearchScopeArg] = None, file_extensions: Optional[str] = None, created_at_range: Optional[str] = None, updated_at_range: Optional[str] = None, size_range: Optional[str] = None, owner_user_ids: Optional[str] = None, recent_updater_user_ids: Optional[str] = None, ancestor_folder_ids: Optional[str] = None, content_types: Optional[str] = None, type: Optional[GetSearchTypeArg] = None, trash_content: Optional[GetSearchTrashContentArg] = None, mdfilters: Optional[str] = None, sort: Optional[GetSearchSortArg] = None, direction: Optional[GetSearchDirectionArg] = None, limit: Optional[int] = None, include_recent_shared_links: Optional[bool] = None, fields: Optional[str] = None, offset: Optional[int] = None, deleted_user_ids: Optional[str] = None, deleted_at_range: Optional[str] = None) -> None:
+    def get_search(self, query: Optional[str] = None, scope: Optional[GetSearchScopeArg] = None, file_extensions: Optional[str] = None, created_at_range: Optional[str] = None, updated_at_range: Optional[str] = None, size_range: Optional[str] = None, owner_user_ids: Optional[str] = None, recent_updater_user_ids: Optional[str] = None, ancestor_folder_ids: Optional[str] = None, content_types: Optional[str] = None, type: Optional[GetSearchTypeArg] = None, trash_content: Optional[GetSearchTrashContentArg] = None, mdfilters: Optional[str] = None, sort: Optional[GetSearchSortArg] = None, direction: Optional[GetSearchDirectionArg] = None, limit: Optional[int] = None, include_recent_shared_links: Optional[bool] = None, fields: Optional[str] = None, offset: Optional[int] = None, deleted_user_ids: Optional[str] = None, deleted_at_range: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Searches for files, folders, web links, and shared files across the
         
         users content or across the entire enterprise.
 
         :param query: The string to search for. This query is matched against item names,
             descriptions, text content of files, and various other fields of
@@ -357,11 +365,16 @@
             If the end date is omitted (`2014-05-15T13:35:01-07:00`),
             the current date will be used as the end date instead.
             The `trash_content` parameter needs to be set to `trashed_only`.
             If searching in trash is not performed, then an empty result
             is returned.
             Data available from 2023-02-01 onwards.
         :type deleted_at_range: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'query': to_string(query), 'scope': to_string(scope), 'file_extensions': to_string(file_extensions), 'created_at_range': to_string(created_at_range), 'updated_at_range': to_string(updated_at_range), 'size_range': to_string(size_range), 'owner_user_ids': to_string(owner_user_ids), 'recent_updater_user_ids': to_string(recent_updater_user_ids), 'ancestor_folder_ids': to_string(ancestor_folder_ids), 'content_types': to_string(content_types), 'type': to_string(type), 'trash_content': to_string(trash_content), 'mdfilters': to_string(mdfilters), 'sort': to_string(sort), 'direction': to_string(direction), 'limit': to_string(limit), 'include_recent_shared_links': to_string(include_recent_shared_links), 'fields': to_string(fields), 'offset': to_string(offset), 'deleted_user_ids': to_string(deleted_user_ids), 'deleted_at_range': to_string(deleted_at_range)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/search']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/search']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/session_termination.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/session_termination.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Optional
 
 from typing import List
 
+from typing import Dict
+
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import SessionTerminationMessage
 
 from box_sdk_gen.schemas import ClientError
@@ -26,15 +28,15 @@
 
 from box_sdk_gen.fetch import FetchResponse
 
 class SessionTerminationManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def create_user_terminate_session(self, user_ids: List[str], user_logins: List[str]) -> SessionTerminationMessage:
+    def create_user_terminate_session(self, user_ids: List[str], user_logins: List[str], extra_headers: Optional[Dict[str, Optional[str]]] = None) -> SessionTerminationMessage:
         """
         Validates the roles and permissions of the user,
         
         and creates asynchronous jobs
 
         
         to terminate the user's sessions.
@@ -42,29 +44,39 @@
         
         Returns the status for the POST request.
 
         :param user_ids: A list of user IDs
         :type user_ids: List[str]
         :param user_logins: A list of user logins
         :type user_logins: List[str]
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(user_ids=user_ids, user_logins=user_logins)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/terminate_sessions']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/terminate_sessions']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return SessionTerminationMessage.from_dict(json.loads(response.text))
-    def create_group_terminate_session(self, group_ids: List[str]) -> SessionTerminationMessage:
+    def create_group_terminate_session(self, group_ids: List[str], extra_headers: Optional[Dict[str, Optional[str]]] = None) -> SessionTerminationMessage:
         """
         Validates the roles and permissions of the group,
         
         and creates asynchronous jobs
 
         
         to terminate the group's sessions.
 
         
         Returns the status for the POST request.
 
         :param group_ids: A list of group IDs
         :type group_ids: List[str]
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(group_ids=group_ids)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/terminate_sessions']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/groups/terminate_sessions']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return SessionTerminationMessage.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_files.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/shared_links_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 class SharedLinksFilesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_shared_items(self, boxapi: str, fields: Optional[str] = None, if_none_match: Optional[str] = None) -> FileFull:
+    def get_shared_items(self, boxapi: str, fields: Optional[str] = None, if_none_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Returns the file represented by a shared link.
         
         A shared file can be represented by a shared link,
 
         
         which can originate within the current enterprise or within another.
@@ -211,38 +211,47 @@
         :type fields: Optional[str], optional
         :param if_none_match: Ensures an item is only returned if it has changed.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `304 Not Modified` if the item has not
             changed since.
         :type if_none_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi)})
+        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shared_items']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
-    def get_file_get_shared_link(self, file_id: str, fields: str) -> FileFull:
+    def get_file_get_shared_link(self, file_id: str, fields: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Gets the information for a shared link on a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
             the `file_id` is `123`.
             Example: "12345"
         :type file_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#get_shared_link']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#get_shared_link']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
-    def update_file_add_shared_link(self, file_id: str, fields: str, shared_link: Optional[UpdateFileAddSharedLinkSharedLinkArg] = None) -> FileFull:
+    def update_file_add_shared_link(self, file_id: str, fields: str, shared_link: Optional[UpdateFileAddSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Adds a shared link to a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
@@ -252,20 +261,25 @@
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: The settings for the shared link to create on the file.
             Use an empty object (`{}`) to use the default settings for shared
             links.
         :type shared_link: Optional[UpdateFileAddSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#add_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#add_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
-    def update_file_update_shared_link(self, file_id: str, fields: str, shared_link: Optional[UpdateFileUpdateSharedLinkSharedLinkArg] = None) -> FileFull:
+    def update_file_update_shared_link(self, file_id: str, fields: str, shared_link: Optional[UpdateFileUpdateSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Updates a shared link on a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
@@ -273,20 +287,25 @@
             Example: "12345"
         :type file_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: The settings for the shared link to update.
         :type shared_link: Optional[UpdateFileUpdateSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#update_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#update_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
-    def update_file_remove_shared_link(self, file_id: str, fields: str, shared_link: Optional[UpdateFileRemoveSharedLinkSharedLinkArg] = None) -> FileFull:
+    def update_file_remove_shared_link(self, file_id: str, fields: str, shared_link: Optional[UpdateFileRemoveSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FileFull:
         """
         Removes a shared link from a file.
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
@@ -295,12 +314,17 @@
         :type file_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: By setting this value to `null`, the shared link
             is removed from the file.
         :type shared_link: Optional[UpdateFileRemoveSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#remove_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '#remove_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FileFull.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_folders.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/shared_links_folders.py`

 * *Files 9% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 class SharedLinksFoldersManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_shared_item_folders(self, boxapi: str, fields: Optional[str] = None, if_none_match: Optional[str] = None) -> FolderFull:
+    def get_shared_item_folders(self, boxapi: str, fields: Optional[str] = None, if_none_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Return the folder represented by a shared link.
         
         A shared folder can be represented by a shared link,
 
         
         which can originate within the current enterprise or within another.
@@ -199,20 +199,24 @@
         :type fields: Optional[str], optional
         :param if_none_match: Ensures an item is only returned if it has changed.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `304 Not Modified` if the item has not
             changed since.
         :type if_none_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi)})
+        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shared_items#folders']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
-    def get_folder_get_shared_link(self, folder_id: str, fields: str) -> FolderFull:
+    def get_folder_get_shared_link(self, folder_id: str, fields: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Gets the information for a shared link on a folder.
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
             by visiting this folder in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/folder/123`
@@ -220,19 +224,24 @@
             The root folder of a Box account is
             always represented by the ID `0`.
             Example: "12345"
         :type folder_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#get_shared_link']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#get_shared_link']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
-    def update_folder_add_shared_link(self, folder_id: str, fields: str, shared_link: Optional[UpdateFolderAddSharedLinkSharedLinkArg] = None) -> FolderFull:
+    def update_folder_add_shared_link(self, folder_id: str, fields: str, shared_link: Optional[UpdateFolderAddSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Adds a shared link to a folder.
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
             by visiting this folder in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/folder/123`
@@ -244,20 +253,25 @@
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: The settings for the shared link to create on the folder.
             Use an empty object (`{}`) to use the default settings for shared
             links.
         :type shared_link: Optional[UpdateFolderAddSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#add_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#add_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
-    def update_folder_update_shared_link(self, folder_id: str, fields: str, shared_link: Optional[UpdateFolderUpdateSharedLinkSharedLinkArg] = None) -> FolderFull:
+    def update_folder_update_shared_link(self, folder_id: str, fields: str, shared_link: Optional[UpdateFolderUpdateSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Updates a shared link on a folder.
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
             by visiting this folder in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/folder/123`
@@ -267,20 +281,25 @@
             Example: "12345"
         :type folder_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: The settings for the shared link to update.
         :type shared_link: Optional[UpdateFolderUpdateSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#update_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#update_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
-    def update_folder_remove_shared_link(self, folder_id: str, fields: str, shared_link: Optional[UpdateFolderRemoveSharedLinkSharedLinkArg] = None) -> FolderFull:
+    def update_folder_remove_shared_link(self, folder_id: str, fields: str, shared_link: Optional[UpdateFolderRemoveSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> FolderFull:
         """
         Removes a shared link from a folder.
         :param folder_id: The unique identifier that represent a folder.
             The ID for any folder can be determined
             by visiting this folder in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/folder/123`
@@ -291,12 +310,17 @@
         :type folder_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: By setting this value to `null`, the shared link
             is removed from the folder.
         :type shared_link: Optional[UpdateFolderRemoveSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#remove_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '#remove_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return FolderFull.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_web_links.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/shared_links_web_links.py`

 * *Files 9% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 class SharedLinksWebLinksManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_shared_item_web_links(self, boxapi: str, fields: Optional[str] = None, if_none_match: Optional[str] = None) -> WebLink:
+    def get_shared_item_web_links(self, boxapi: str, fields: Optional[str] = None, if_none_match: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
         Returns the web link represented by a shared link.
         
         A shared web link can be represented by a shared link,
 
         
         which can originate within the current enterprise or within another.
@@ -197,76 +197,100 @@
         :type fields: Optional[str], optional
         :param if_none_match: Ensures an item is only returned if it has changed.
             Pass in the item's last observed `etag` value
             into this header and the endpoint will fail
             with a `304 Not Modified` if the item has not
             changed since.
         :type if_none_match: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi)})
+        headers_map: Dict[str, str] = prepare_params({'if-none-match': to_string(if_none_match), 'boxapi': to_string(boxapi), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shared_items#web_links']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return WebLink.from_dict(json.loads(response.text))
-    def get_web_link_get_shared_link(self, web_link_id: str, fields: str) -> WebLink:
+    def get_web_link_get_shared_link(self, web_link_id: str, fields: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
         Gets the information for a shared link on a web link.
         :param web_link_id: The ID of the web link.
             Example: "12345"
         :type web_link_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#get_shared_link']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#get_shared_link']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return WebLink.from_dict(json.loads(response.text))
-    def update_web_link_add_shared_link(self, web_link_id: str, fields: str, shared_link: Optional[UpdateWebLinkAddSharedLinkSharedLinkArg] = None) -> WebLink:
+    def update_web_link_add_shared_link(self, web_link_id: str, fields: str, shared_link: Optional[UpdateWebLinkAddSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
         Adds a shared link to a web link.
         :param web_link_id: The ID of the web link.
             Example: "12345"
         :type web_link_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: The settings for the shared link to create on the web link.
             Use an empty object (`{}`) to use the default settings for shared
             links.
         :type shared_link: Optional[UpdateWebLinkAddSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#add_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#add_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return WebLink.from_dict(json.loads(response.text))
-    def update_web_link_update_shared_link(self, web_link_id: str, fields: str, shared_link: Optional[UpdateWebLinkUpdateSharedLinkSharedLinkArg] = None) -> WebLink:
+    def update_web_link_update_shared_link(self, web_link_id: str, fields: str, shared_link: Optional[UpdateWebLinkUpdateSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
         Updates a shared link on a web link.
         :param web_link_id: The ID of the web link.
             Example: "12345"
         :type web_link_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: The settings for the shared link to update.
         :type shared_link: Optional[UpdateWebLinkUpdateSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#update_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#update_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return WebLink.from_dict(json.loads(response.text))
-    def update_web_link_remove_shared_link(self, web_link_id: str, fields: str, shared_link: Optional[UpdateWebLinkRemoveSharedLinkSharedLinkArg] = None) -> WebLink:
+    def update_web_link_remove_shared_link(self, web_link_id: str, fields: str, shared_link: Optional[UpdateWebLinkRemoveSharedLinkSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
         Removes a shared link from a web link.
         :param web_link_id: The ID of the web link.
             Example: "12345"
         :type web_link_id: str
         :param fields: Explicitly request the `shared_link` fields
             to be returned for this item.
         :type fields: str
         :param shared_link: By setting this value to `null`, the shared link
             is removed from the web link.
         :type shared_link: Optional[UpdateWebLinkRemoveSharedLinkSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(shared_link=shared_link)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#remove_shared_link']), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '#remove_shared_link']), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return WebLink.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barriers.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/shield_information_barriers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 
 from typing import Optional
 
-import json
-
 from typing import Dict
 
+import json
+
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import EnterpriseBase
 
 from box_sdk_gen.schemas import UserBase
 
 from box_sdk_gen.schemas import ShieldInformationBarrier
@@ -46,51 +46,66 @@
     ENABLED = 'enabled'
     INVALID = 'invalid'
 
 class ShieldInformationBarriersManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_shield_information_barrier_by_id(self, shield_information_barrier_id: str) -> ShieldInformationBarrier:
+    def get_shield_information_barrier_by_id(self, shield_information_barrier_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ShieldInformationBarrier:
         """
         Get shield information barrier based on provided ID..
         :param shield_information_barrier_id: The ID of the shield information barrier.
             Example: "1910967"
         :type shield_information_barrier_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers/', shield_information_barrier_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers/', shield_information_barrier_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return ShieldInformationBarrier.from_dict(json.loads(response.text))
-    def create_shield_information_barrier_change_status(self, id: str, status: CreateShieldInformationBarrierChangeStatusStatusArg) -> ShieldInformationBarrier:
+    def create_shield_information_barrier_change_status(self, id: str, status: CreateShieldInformationBarrierChangeStatusStatusArg, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ShieldInformationBarrier:
         """
         Change status of shield information barrier with the specified ID.
         :param id: The ID of the shield information barrier.
         :type id: str
         :param status: The desired status for the shield information barrier.
         :type status: CreateShieldInformationBarrierChangeStatusStatusArg
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(id=id, status=status)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers/change_status']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers/change_status']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return ShieldInformationBarrier.from_dict(json.loads(response.text))
-    def get_shield_information_barriers(self, marker: Optional[str] = None, limit: Optional[int] = None) -> None:
+    def get_shield_information_barriers(self, marker: Optional[str] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Retrieves a list of shield information barrier objects
         
         for the enterprise of JWT.
 
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return None
-    def create_shield_information_barrier(self, id: Optional[str] = None, type: Optional[CreateShieldInformationBarrierTypeArg] = None, enterprise: Optional[EnterpriseBase] = None, status: Optional[CreateShieldInformationBarrierStatusArg] = None, created_at: Optional[str] = None, created_by: Optional[UserBase] = None, updated_at: Optional[str] = None, updated_by: Optional[UserBase] = None, enabled_at: Optional[str] = None, enabled_by: Optional[UserBase] = None) -> ShieldInformationBarrier:
+    def create_shield_information_barrier(self, id: Optional[str] = None, type: Optional[CreateShieldInformationBarrierTypeArg] = None, enterprise: Optional[EnterpriseBase] = None, status: Optional[CreateShieldInformationBarrierStatusArg] = None, created_at: Optional[str] = None, created_by: Optional[UserBase] = None, updated_at: Optional[str] = None, updated_by: Optional[UserBase] = None, enabled_at: Optional[str] = None, enabled_by: Optional[UserBase] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ShieldInformationBarrier:
         """
         Creates a shield information barrier to
         
         separate individuals/groups within the same
 
         
         firm and prevents confidential information passing between them.
@@ -104,11 +119,16 @@
         :param created_at: ISO date time string when this
             shield information barrier object was created.
         :type created_at: Optional[str], optional
         :param updated_at: ISO date time string when this shield information barrier was updated.
         :type updated_at: Optional[str], optional
         :param enabled_at: ISO date time string when this shield information barrier was enabled.
         :type enabled_at: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        request_body: BaseObject = BaseObject(id=id, type=type, enterprise=enterprise, status=status, created_at=created_at, created_by=created_by, updated_at=updated_at, updated_by=updated_by, enabled_at=enabled_at, enabled_by=enabled_by)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: ShieldInformationBarrier = ShieldInformationBarrier(id=id, type=type, enterprise=enterprise, status=status, created_at=created_at, created_by=created_by, updated_at=updated_at, updated_by=updated_by, enabled_at=enabled_at, enabled_by=enabled_by)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/shield_information_barriers']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return ShieldInformationBarrier.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/skills.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/web_links.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,23 @@
-from enum import Enum
+from box_sdk_gen.base_object import BaseObject
 
 from typing import Optional
 
-from typing import List
-
-from typing import Union
+from enum import Enum
 
-from box_sdk_gen.base_object import BaseObject
+from typing import Dict
 
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
-from box_sdk_gen.schemas import SkillCardsMetadata
+from box_sdk_gen.schemas import WebLink
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import KeywordSkillCard
-
-from box_sdk_gen.schemas import TimelineSkillCard
-
-from box_sdk_gen.schemas import TranscriptSkillCard
-
-from box_sdk_gen.schemas import StatusSkillCard
-
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
 from box_sdk_gen.utils import to_string
@@ -36,141 +26,154 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class UpdateSkillInvocationByIdStatusArg(str, Enum):
-    INVOKED = 'invoked'
-    PROCESSING = 'processing'
-    SUCCESS = 'success'
-    TRANSIENT_FAILURE = 'transient_failure'
-    PERMANENT_FAILURE = 'permanent_failure'
-
-class UpdateSkillInvocationByIdMetadataArg(BaseObject):
-    def __init__(self, cards: Optional[List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]]] = None, **kwargs):
-        """
-        :param cards: A list of Box Skill cards to apply to this file.
-        :type cards: Optional[List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]]], optional
-        """
-        super().__init__(**kwargs)
-        self.cards = cards
-
-class UpdateSkillInvocationByIdFileArgTypeField(str, Enum):
-    FILE = 'file'
-
-class UpdateSkillInvocationByIdFileArg(BaseObject):
-    def __init__(self, type: Optional[UpdateSkillInvocationByIdFileArgTypeField] = None, id: Optional[str] = None, **kwargs):
+class CreateWebLinkParentArg(BaseObject):
+    def __init__(self, id: str, **kwargs):
         """
-        :param type: `file`
-        :type type: Optional[UpdateSkillInvocationByIdFileArgTypeField], optional
-        :param id: The ID of the file
-        :type id: Optional[str], optional
+        :param id: The ID of parent folder
+        :type id: str
         """
         super().__init__(**kwargs)
-        self.type = type
         self.id = id
 
-class UpdateSkillInvocationByIdFileVersionArgTypeField(str, Enum):
-    FILE_VERSION = 'file_version'
-
-class UpdateSkillInvocationByIdFileVersionArg(BaseObject):
-    def __init__(self, type: Optional[UpdateSkillInvocationByIdFileVersionArgTypeField] = None, id: Optional[str] = None, **kwargs):
+class UpdateWebLinkByIdParentArg(BaseObject):
+    def __init__(self, id: Optional[str] = None, **kwargs):
         """
-        :param type: `file_version`
-        :type type: Optional[UpdateSkillInvocationByIdFileVersionArgTypeField], optional
-        :param id: The ID of the file version
+        :param id: The ID of parent item
         :type id: Optional[str], optional
         """
         super().__init__(**kwargs)
-        self.type = type
         self.id = id
 
-class UpdateSkillInvocationByIdUsageArg(BaseObject):
-    def __init__(self, unit: Optional[str] = None, value: Optional[int] = None, **kwargs):
-        """
-        :param unit: `file`
-        :type unit: Optional[str], optional
-        :param value: `1`
-        :type value: Optional[int], optional
+class UpdateWebLinkByIdSharedLinkArgAccessField(str, Enum):
+    OPEN = 'open'
+    COMPANY = 'company'
+    COLLABORATORS = 'collaborators'
+
+class UpdateWebLinkByIdSharedLinkArg(BaseObject):
+    def __init__(self, access: Optional[UpdateWebLinkByIdSharedLinkArgAccessField] = None, password: Optional[str] = None, vanity_name: Optional[str] = None, unshared_at: Optional[str] = None, **kwargs):
+        """
+        :param access: The level of access for the shared link. This can be
+            restricted to anyone with the link (`open`), only people
+            within the company (`company`) and only those who
+            have been invited to the folder (`collaborators`).
+            If not set, this field defaults to the access level specified
+            by the enterprise admin. To create a shared link with this
+            default setting pass the `shared_link` object with
+            no `access` field, for example `{ "shared_link": {} }`.
+            The `company` access level is only available to paid
+            accounts.
+        :type access: Optional[UpdateWebLinkByIdSharedLinkArgAccessField], optional
+        :param password: The password required to access the shared link. Set the
+            password to `null` to remove it.
+            Passwords must now be at least eight characters
+            long and include a number, upper case letter, or
+            a non-numeric or non-alphabetic character.
+            A password can only be set when `access` is set to `open`.
+        :type password: Optional[str], optional
+        :param vanity_name: Defines a custom vanity name to use in the shared link URL,
+            for example `https://app.box.com/v/my-shared-link`.
+            Custom URLs should not be used when sharing sensitive content
+            as vanity URLs are a lot easier to guess than regular shared
+            links.
+        :type vanity_name: Optional[str], optional
+        :param unshared_at: The timestamp at which this shared link will
+            expire. This field can only be set by
+            users with paid accounts. The value must be greater than the
+            current date and time.
+        :type unshared_at: Optional[str], optional
         """
         super().__init__(**kwargs)
-        self.unit = unit
-        self.value = value
+        self.access = access
+        self.password = password
+        self.vanity_name = vanity_name
+        self.unshared_at = unshared_at
 
-class SkillsManager:
+class WebLinksManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_metadata_global_box_skills_cards(self, file_id: str) -> SkillCardsMetadata:
+    def create_web_link(self, url: str, parent: CreateWebLinkParentArg, name: Optional[str] = None, description: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
-        List the Box Skills metadata cards that are attached to a file.
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
+        Creates a web link object within a folder.
+        :param url: The URL that this web link links to. Must start with
+            `"http://"` or `"https://"`.
+        :type url: str
+        :param parent: The parent folder to create the web link within.
+        :type parent: CreateWebLinkParentArg
+        :param name: Name of the web link. Defaults to the URL if not set.
+        :type name: Optional[str], optional
+        :param description: Description of the web link.
+        :type description: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(url=url, parent=parent, name=name, description=description)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return WebLink.from_dict(json.loads(response.text))
+    def get_web_link_by_id(self, web_link_id: str, boxapi: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/global/boxSkillsCards']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return SkillCardsMetadata.from_dict(json.loads(response.text))
-    def create_file_metadata_global_box_skills_card(self, file_id: str, cards: List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]]) -> SkillCardsMetadata:
-        """
-        Applies one or more Box Skills metadata cards to a file.
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
-        :param cards: A list of Box Skill cards to apply to this file.
-        :type cards: List[Union[KeywordSkillCard, TimelineSkillCard, TranscriptSkillCard, StatusSkillCard]]
-        """
-        request_body: BaseObject = BaseObject(cards=cards)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/global/boxSkillsCards']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return SkillCardsMetadata.from_dict(json.loads(response.text))
-    def delete_file_metadata_global_box_skills_card(self, file_id: str) -> None:
-        """
-        Removes any Box Skills cards metadata from a file.
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
+        Retrieve information about a web link.
+        :param web_link_id: The ID of the web link.
             Example: "12345"
-        :type file_id: str
+        :type web_link_id: str
+        :param boxapi: The URL, and optional password, for the shared link of this item.
+            This header can be used to access items that have not been
+            explicitly shared with a user.
+            Use the format `shared_link=[link]` or if a password is required then
+            use `shared_link=[link]&shared_link_password=[password]`.
+            This header can be used on the file or folder shared, as well as on any files
+            or folders nested within the item.
+        :type boxapi: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({'boxapi': to_string(boxapi), **extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return WebLink.from_dict(json.loads(response.text))
+    def update_web_link_by_id(self, web_link_id: str, url: Optional[str] = None, parent: Optional[UpdateWebLinkByIdParentArg] = None, name: Optional[str] = None, description: Optional[str] = None, shared_link: Optional[UpdateWebLinkByIdSharedLinkArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> WebLink:
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/global/boxSkillsCards']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
-        return None
-    def update_skill_invocation_by_id(self, skill_id: str, status: UpdateSkillInvocationByIdStatusArg, metadata: UpdateSkillInvocationByIdMetadataArg, file: UpdateSkillInvocationByIdFileArg, file_version: Optional[UpdateSkillInvocationByIdFileVersionArg] = None, usage: Optional[UpdateSkillInvocationByIdUsageArg] = None) -> None:
-        """
-        An alternative method that can be used to overwrite and update all Box Skill
-        
-        metadata cards on a file.
-
-        :param skill_id: The ID of the skill to apply this metadata for.
-            Example: "33243242"
-        :type skill_id: str
-        :param status: Defines the status of this invocation. Set this to `success` when setting Skill cards.
-        :type status: UpdateSkillInvocationByIdStatusArg
-        :param metadata: The metadata to set for this skill. This is a list of
-            Box Skills cards. These cards will overwrite any existing Box
-            skill cards on the file.
-        :type metadata: UpdateSkillInvocationByIdMetadataArg
-        :param file: The file to assign the cards to.
-        :type file: UpdateSkillInvocationByIdFileArg
-        :param file_version: The optional file version to assign the cards to.
-        :type file_version: Optional[UpdateSkillInvocationByIdFileVersionArg], optional
-        :param usage: A descriptor that defines what items are affected by this call.
-            Set this to the default values when setting a card to a `success`
-            state, and leave it out in most other situations.
-        :type usage: Optional[UpdateSkillInvocationByIdUsageArg], optional
+        Updates a web link object.
+        :param web_link_id: The ID of the web link.
+            Example: "12345"
+        :type web_link_id: str
+        :param url: The new URL that the web link links to. Must start with
+            `"http://"` or `"https://"`.
+        :type url: Optional[str], optional
+        :param name: A new name for the web link. Defaults to the URL if not set.
+        :type name: Optional[str], optional
+        :param description: A new description of the web link.
+        :type description: Optional[str], optional
+        :param shared_link: The settings for the shared link to update.
+        :type shared_link: Optional[UpdateWebLinkByIdSharedLinkArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: BaseObject = BaseObject(url=url, parent=parent, name=name, description=description, shared_link=shared_link)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return WebLink.from_dict(json.loads(response.text))
+    def delete_web_link_by_id(self, web_link_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
-        request_body: BaseObject = BaseObject(status=status, metadata=metadata, file=file, file_version=file_version, usage=usage)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/skill_invocations/', skill_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format=None, auth=self.auth, network_session=self.network_session))
+        Deletes a web link.
+        :param web_link_id: The ID of the web link.
+            Example: "12345"
+        :type web_link_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policies.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/storage_policies.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from box_sdk_gen.fetch import FetchResponse
 
 class StoragePoliciesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_storage_policies(self, fields: Optional[str] = None, marker: Optional[str] = None, limit: Optional[int] = None) -> StoragePolicies:
+    def get_storage_policies(self, fields: Optional[str] = None, marker: Optional[str] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> StoragePolicies:
         """
         Fetches all the storage policies in the enterprise.
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
@@ -44,20 +44,30 @@
         :type fields: Optional[str], optional
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policies']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policies']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return StoragePolicies.from_dict(json.loads(response.text))
-    def get_storage_policy_by_id(self, storage_policy_id: str) -> StoragePolicy:
+    def get_storage_policy_by_id(self, storage_policy_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> StoragePolicy:
         """
         Fetches a specific storage policy.
         :param storage_policy_id: The ID of the storage policy.
             Example: "34342"
         :type storage_policy_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policies/', storage_policy_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policies/', storage_policy_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return StoragePolicy.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policy_assignments.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/storage_policy_assignments.py`

 * *Files 27% similar despite different names*

```diff
@@ -82,65 +82,85 @@
         self.type = type
         self.id = id
 
 class StoragePolicyAssignmentsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_storage_policy_assignments(self, resolved_for_type: GetStoragePolicyAssignmentsResolvedForTypeArg, resolved_for_id: str, marker: Optional[str] = None) -> StoragePolicyAssignments:
+    def get_storage_policy_assignments(self, resolved_for_type: GetStoragePolicyAssignmentsResolvedForTypeArg, resolved_for_id: str, marker: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> StoragePolicyAssignments:
         """
         Fetches all the storage policy assignment for an enterprise or user.
         :param resolved_for_type: The target type to return assignments for
         :type resolved_for_type: GetStoragePolicyAssignmentsResolvedForTypeArg
         :param resolved_for_id: The ID of the user or enterprise to return assignments for
         :type resolved_for_id: str
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'resolved_for_type': to_string(resolved_for_type), 'resolved_for_id': to_string(resolved_for_id)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return StoragePolicyAssignments.from_dict(json.loads(response.text))
-    def create_storage_policy_assignment(self, storage_policy: CreateStoragePolicyAssignmentStoragePolicyArg, assigned_to: CreateStoragePolicyAssignmentAssignedToArg) -> StoragePolicyAssignment:
+    def create_storage_policy_assignment(self, storage_policy: CreateStoragePolicyAssignmentStoragePolicyArg, assigned_to: CreateStoragePolicyAssignmentAssignedToArg, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> StoragePolicyAssignment:
         """
         Creates a storage policy assignment for an enterprise or user.
         :param storage_policy: The storage policy to assign to the user or
             enterprise
         :type storage_policy: CreateStoragePolicyAssignmentStoragePolicyArg
         :param assigned_to: The user or enterprise to assign the storage
             policy to.
         :type assigned_to: CreateStoragePolicyAssignmentAssignedToArg
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(storage_policy=storage_policy, assigned_to=assigned_to)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return StoragePolicyAssignment.from_dict(json.loads(response.text))
-    def get_storage_policy_assignment_by_id(self, storage_policy_assignment_id: str) -> StoragePolicyAssignment:
+    def get_storage_policy_assignment_by_id(self, storage_policy_assignment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> StoragePolicyAssignment:
         """
         Fetches a specific storage policy assignment.
         :param storage_policy_assignment_id: The ID of the storage policy assignment.
             Example: "932483"
         :type storage_policy_assignment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments/', storage_policy_assignment_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments/', storage_policy_assignment_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return StoragePolicyAssignment.from_dict(json.loads(response.text))
-    def update_storage_policy_assignment_by_id(self, storage_policy_assignment_id: str, storage_policy: UpdateStoragePolicyAssignmentByIdStoragePolicyArg) -> StoragePolicyAssignment:
+    def update_storage_policy_assignment_by_id(self, storage_policy_assignment_id: str, storage_policy: UpdateStoragePolicyAssignmentByIdStoragePolicyArg, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> StoragePolicyAssignment:
         """
         Updates a specific storage policy assignment.
         :param storage_policy_assignment_id: The ID of the storage policy assignment.
             Example: "932483"
         :type storage_policy_assignment_id: str
         :param storage_policy: The storage policy to assign to the user or
             enterprise
         :type storage_policy: UpdateStoragePolicyAssignmentByIdStoragePolicyArg
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(storage_policy=storage_policy)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments/', storage_policy_assignment_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments/', storage_policy_assignment_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return StoragePolicyAssignment.from_dict(json.loads(response.text))
-    def delete_storage_policy_assignment_by_id(self, storage_policy_assignment_id: str) -> None:
+    def delete_storage_policy_assignment_by_id(self, storage_policy_assignment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Delete a storage policy assignment.
         
         Deleting a storage policy assignment on a user
 
         
         will have the user inherit the enterprise's default
@@ -153,10 +173,15 @@
 
         
         twice per user in a 24 hour time frame.
 
         :param storage_policy_assignment_id: The ID of the storage policy assignment.
             Example: "932483"
         :type storage_policy_assignment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments/', storage_policy_assignment_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/storage_policy_assignments/', storage_policy_assignment_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/task_assignments.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/task_assignments.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from enum import Enum
 
 from box_sdk_gen.base_object import BaseObject
 
 from typing import Optional
 
+from typing import Dict
+
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import TaskAssignments
 
 from box_sdk_gen.schemas import ClientError
@@ -67,50 +69,65 @@
     APPROVED = 'approved'
     REJECTED = 'rejected'
 
 class TaskAssignmentsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_task_assignments(self, task_id: str) -> TaskAssignments:
+    def get_task_assignments(self, task_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TaskAssignments:
         """
         Lists all of the assignments for a given task.
         :param task_id: The ID of the task.
             Example: "12345"
         :type task_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id, '/assignments']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id, '/assignments']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return TaskAssignments.from_dict(json.loads(response.text))
-    def create_task_assignment(self, task: CreateTaskAssignmentTaskArg, assign_to: CreateTaskAssignmentAssignToArg) -> TaskAssignment:
+    def create_task_assignment(self, task: CreateTaskAssignmentTaskArg, assign_to: CreateTaskAssignmentAssignToArg, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TaskAssignment:
         """
         Assigns a task to a user.
         
         A task can be assigned to more than one user by creating multiple
 
         
         assignments.
 
         :param task: The task to assign to a user.
         :type task: CreateTaskAssignmentTaskArg
         :param assign_to: The user to assign the task to.
         :type assign_to: CreateTaskAssignmentAssignToArg
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(task=task, assign_to=assign_to)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return TaskAssignment.from_dict(json.loads(response.text))
-    def get_task_assignment_by_id(self, task_assignment_id: str) -> TaskAssignment:
+    def get_task_assignment_by_id(self, task_assignment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TaskAssignment:
         """
         Retrieves information about a task assignment.
         :param task_assignment_id: The ID of the task assignment.
             Example: "12345"
         :type task_assignment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments/', task_assignment_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments/', task_assignment_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return TaskAssignment.from_dict(json.loads(response.text))
-    def update_task_assignment_by_id(self, task_assignment_id: str, message: Optional[str] = None, resolution_state: Optional[UpdateTaskAssignmentByIdResolutionStateArg] = None) -> TaskAssignment:
+    def update_task_assignment_by_id(self, task_assignment_id: str, message: Optional[str] = None, resolution_state: Optional[UpdateTaskAssignmentByIdResolutionStateArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TaskAssignment:
         """
         Updates a task assignment. This endpoint can be
         
         used to update the state of a task assigned to a user.
 
         :param task_assignment_id: The ID of the task assignment.
             Example: "12345"
@@ -119,20 +136,30 @@
         :type message: Optional[str], optional
         :param resolution_state: The state of the task assigned to the user.
             * For a task with an `action` value of `complete` this can be
             `incomplete` or `completed`.
             * For a task with an `action` of `review` this can be
             `incomplete`, `approved`, or `rejected`.
         :type resolution_state: Optional[UpdateTaskAssignmentByIdResolutionStateArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(message=message, resolution_state=resolution_state)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments/', task_assignment_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments/', task_assignment_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return TaskAssignment.from_dict(json.loads(response.text))
-    def delete_task_assignment_by_id(self, task_assignment_id: str) -> None:
+    def delete_task_assignment_by_id(self, task_assignment_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a specific task assignment.
         :param task_assignment_id: The ID of the task assignment.
             Example: "12345"
         :type task_assignment_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments/', task_assignment_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/task_assignments/', task_assignment_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/tasks.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/tasks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from enum import Enum
 
+from typing import Optional
+
 from box_sdk_gen.base_object import BaseObject
 
-from typing import Optional
+from typing import Dict
 
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import Tasks
 
@@ -30,20 +32,20 @@
 
 from box_sdk_gen.fetch import FetchResponse
 
 class CreateTaskItemArgTypeField(str, Enum):
     FILE = 'file'
 
 class CreateTaskItemArg(BaseObject):
-    def __init__(self, id: str, type: CreateTaskItemArgTypeField, **kwargs):
+    def __init__(self, id: Optional[str] = None, type: Optional[CreateTaskItemArgTypeField] = None, **kwargs):
         """
         :param id: The ID of the file
-        :type id: str
+        :type id: Optional[str], optional
         :param type: `file`
-        :type type: CreateTaskItemArgTypeField
+        :type type: Optional[CreateTaskItemArgTypeField], optional
         """
         super().__init__(**kwargs)
         self.id = id
         self.type = type
 
 class CreateTaskActionArg(str, Enum):
     REVIEW = 'review'
@@ -61,32 +63,37 @@
     ALL_ASSIGNEES = 'all_assignees'
     ANY_ASSIGNEE = 'any_assignee'
 
 class TasksManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_file_tasks(self, file_id: str) -> Tasks:
+    def get_file_tasks(self, file_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Tasks:
         """
         Retrieves a list of all the tasks for a file. This
         
         endpoint does not support pagination.
 
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
             by visiting a file in the web application
             and copying the ID from the URL. For example,
             for the URL `https://*.app.box.com/files/123`
             the `file_id` is `123`.
             Example: "12345"
         :type file_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/tasks']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/tasks']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Tasks.from_dict(json.loads(response.text))
-    def create_task(self, item: CreateTaskItemArg, action: Optional[CreateTaskActionArg] = None, message: Optional[str] = None, due_at: Optional[str] = None, completion_rule: Optional[CreateTaskCompletionRuleArg] = None) -> Task:
+    def create_task(self, item: CreateTaskItemArg, action: Optional[CreateTaskActionArg] = None, message: Optional[str] = None, due_at: Optional[str] = None, completion_rule: Optional[CreateTaskCompletionRuleArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Task:
         """
         Creates a single task on a file. This task is not assigned to any user and
         
         will need to be assigned separately.
 
         :param item: The file to attach the task to.
         :type item: CreateTaskItemArg
@@ -103,28 +110,38 @@
         :param completion_rule: Defines which assignees need to complete this task before the task
             is considered completed.
             * `all_assignees` (default) requires all assignees to review or
             approve the the task in order for it to be considered completed.
             * `any_assignee` accepts any one assignee to review or
             approve the the task in order for it to be considered completed.
         :type completion_rule: Optional[CreateTaskCompletionRuleArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(item=item, action=action, message=message, due_at=due_at, completion_rule=completion_rule)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Task.from_dict(json.loads(response.text))
-    def get_task_by_id(self, task_id: str) -> Task:
+    def get_task_by_id(self, task_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Task:
         """
         Retrieves information about a specific task.
         :param task_id: The ID of the task.
             Example: "12345"
         :type task_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Task.from_dict(json.loads(response.text))
-    def update_task_by_id(self, task_id: str, action: Optional[UpdateTaskByIdActionArg] = None, message: Optional[str] = None, due_at: Optional[str] = None, completion_rule: Optional[UpdateTaskByIdCompletionRuleArg] = None) -> Task:
+    def update_task_by_id(self, task_id: str, action: Optional[UpdateTaskByIdActionArg] = None, message: Optional[str] = None, due_at: Optional[str] = None, completion_rule: Optional[UpdateTaskByIdCompletionRuleArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Task:
         """
         Updates a task. This can be used to update a task's configuration, or to
         
         update its completion state.
 
         :param task_id: The ID of the task.
             Example: "12345"
@@ -141,20 +158,30 @@
         :param completion_rule: Defines which assignees need to complete this task before the task
             is considered completed.
             * `all_assignees` (default) requires all assignees to review or
             approve the the task in order for it to be considered completed.
             * `any_assignee` accepts any one assignee to review or
             approve the the task in order for it to be considered completed.
         :type completion_rule: Optional[UpdateTaskByIdCompletionRuleArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(action=action, message=message, due_at=due_at, completion_rule=completion_rule)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Task.from_dict(json.loads(response.text))
-    def delete_task_by_id(self, task_id: str) -> None:
+    def delete_task_by_id(self, task_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Removes a task from a file.
         :param task_id: The ID of the task.
             Example: "12345"
         :type task_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/tasks/', task_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/terms_of_service_user_statuses.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/terms_of_service_user_statuses.py`

 * *Files 20% similar despite different names*

```diff
@@ -62,49 +62,64 @@
         self.type = type
         self.id = id
 
 class TermsOfServiceUserStatusesManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_term_of_service_user_statuses(self, tos_id: str, user_id: Optional[str] = None) -> TermsOfServiceUserStatuses:
+    def get_term_of_service_user_statuses(self, tos_id: str, user_id: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TermsOfServiceUserStatuses:
         """
         Retrieves an overview of users and their status for a
         
         terms of service, including Whether they have accepted
 
         
         the terms and when.
 
         :param tos_id: The ID of the terms of service.
         :type tos_id: str
         :param user_id: Limits results to the given user ID.
         :type user_id: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'tos_id': to_string(tos_id), 'user_id': to_string(user_id)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/terms_of_service_user_statuses']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/terms_of_service_user_statuses']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return TermsOfServiceUserStatuses.from_dict(json.loads(response.text))
-    def create_term_of_service_user_status(self, tos: CreateTermOfServiceUserStatusTosArg, user: CreateTermOfServiceUserStatusUserArg, is_accepted: bool) -> TermsOfServiceUserStatus:
+    def create_term_of_service_user_status(self, tos: CreateTermOfServiceUserStatusTosArg, user: CreateTermOfServiceUserStatusUserArg, is_accepted: bool, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TermsOfServiceUserStatus:
         """
         Sets the status for a terms of service for a user.
         :param tos: The terms of service to set the status for.
         :type tos: CreateTermOfServiceUserStatusTosArg
         :param user: The user to set the status for.
         :type user: CreateTermOfServiceUserStatusUserArg
         :param is_accepted: Whether the user has accepted the terms.
         :type is_accepted: bool
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(tos=tos, user=user, is_accepted=is_accepted)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/terms_of_service_user_statuses']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/terms_of_service_user_statuses']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return TermsOfServiceUserStatus.from_dict(json.loads(response.text))
-    def update_term_of_service_user_status_by_id(self, terms_of_service_user_status_id: str, is_accepted: bool) -> TermsOfServiceUserStatus:
+    def update_term_of_service_user_status_by_id(self, terms_of_service_user_status_id: str, is_accepted: bool, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TermsOfServiceUserStatus:
         """
         Updates the status for a terms of service for a user.
         :param terms_of_service_user_status_id: The ID of the terms of service status.
             Example: "324234"
         :type terms_of_service_user_status_id: str
         :param is_accepted: Whether the user has accepted the terms.
         :type is_accepted: bool
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(is_accepted=is_accepted)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/terms_of_service_user_statuses/', terms_of_service_user_status_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/terms_of_service_user_statuses/', terms_of_service_user_status_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return TermsOfServiceUserStatus.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_files.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/trashed_items.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from typing import Optional
+from enum import Enum
 
-from box_sdk_gen.base_object import BaseObject
+from typing import Optional
 
 from typing import Dict
 
 import json
 
-from box_sdk_gen.base_object import BaseObject
-
-from box_sdk_gen.schemas import TrashFileRestored
+from box_sdk_gen.schemas import Items
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import TrashFile
-
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
 from box_sdk_gen.utils import to_string
@@ -26,118 +22,87 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class RestoreFileFromTrashParentArg(BaseObject):
-    def __init__(self, id: Optional[str] = None, **kwargs):
-        """
-        :param id: The ID of parent item
-        :type id: Optional[str], optional
-        """
-        super().__init__(**kwargs)
-        self.id = id
+class GetFolderTrashItemsDirectionArg(str, Enum):
+    ASC = 'ASC'
+    DESC = 'DESC'
+
+class GetFolderTrashItemsSortArg(str, Enum):
+    NAME = 'name'
+    DATE = 'date'
+    SIZE = 'size'
 
-class TrashedFilesManager:
+class TrashedItemsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def restore_file_from_trash(self, file_id: str, name: Optional[str] = None, parent: Optional[RestoreFileFromTrashParentArg] = None, fields: Optional[str] = None) -> TrashFileRestored:
-        """
-        Restores a file that has been moved to the trash.
-        
-        An optional new parent ID can be provided to restore the file to in case the
-
-        
-        original folder has been deleted.
-
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
-        :param name: An optional new name for the file.
-        :type name: Optional[str], optional
-        :param fields: A comma-separated list of attributes to include in the
-            response. This can be used to request fields that are
-            not normally returned in a standard response.
-            Be aware that specifying this parameter will have the
-            effect that none of the standard fields are returned in
-            the response unless explicitly specified, instead only
-            fields for the mini representation are returned, additional
-            to the fields requested.
-        :type fields: Optional[str], optional
-        """
-        request_body: BaseObject = BaseObject(name=name, parent=parent)
-        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id]), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return TrashFileRestored.from_dict(json.loads(response.text))
-    def get_file_trash(self, file_id: str, fields: Optional[str] = None) -> TrashFile:
+    def get_folder_trash_items(self, fields: Optional[str] = None, limit: Optional[int] = None, offset: Optional[int] = None, usemarker: Optional[bool] = None, marker: Optional[str] = None, direction: Optional[GetFolderTrashItemsDirectionArg] = None, sort: Optional[GetFolderTrashItemsSortArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Items:
         """
-        Retrieves a file that has been moved to the trash.
-        
-        Please note that only if the file itself has been moved to the
-
+        Retrieves the files and folders that have been moved
         
-        trash can it be retrieved with this API call. If instead one of
+        to the trash.
 
         
-        its parent folders was moved to the trash, only that folder
+        Any attribute in the full files or folders objects can be passed
 
         
-        can be inspected using the
+        in with the `fields` parameter to retrieve those specific
 
         
-        [`GET /folders/:id/trash`](e://get_folders_id_trash) API.
+        attributes that are not returned by default.
 
         
-        To list all items that have been moved to the trash, please
+        This endpoint defaults to use offset-based pagination, yet also supports
 
         
-        use the [`GET /folders/trash/items`](e://get-folders-trash-items/)
+        marker-based pagination using the `marker` parameter.
 
-        
-        API.
-
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
-        """
-        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/trash']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return TrashFile.from_dict(json.loads(response.text))
-    def delete_file_trash(self, file_id: str) -> None:
-        """
-        Permanently deletes a file that is in the trash.
-        
-        This action cannot be undone.
-
-        :param file_id: The unique identifier that represents a file.
-            The ID for any file can be determined
-            by visiting a file in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/files/123`
-            the `file_id` is `123`.
-            Example: "12345"
-        :type file_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/trash']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
-        return None
+        :param limit: The maximum number of items to return per page.
+        :type limit: Optional[int], optional
+        :param offset: The offset of the item at which to begin the response.
+            Queries with offset parameter value
+            exceeding 10000 will be rejected
+            with a 400 response.
+        :type offset: Optional[int], optional
+        :param usemarker: Specifies whether to use marker-based pagination instead of
+            offset-based pagination. Only one pagination method can
+            be used at a time.
+            By setting this value to true, the API will return a `marker` field
+            that can be passed as a parameter to this endpoint to get the next
+            page of the response.
+        :type usemarker: Optional[bool], optional
+        :param marker: Defines the position marker at which to begin returning results. This is
+            used when paginating using marker-based pagination.
+            This requires `usemarker` to be set to `true`.
+        :type marker: Optional[str], optional
+        :param direction: The direction to sort results in. This can be either in alphabetical ascending
+            (`ASC`) or descending (`DESC`) order.
+        :type direction: Optional[GetFolderTrashItemsDirectionArg], optional
+        :param sort: Defines the **second** attribute by which items
+            are sorted.
+            Items are always sorted by their `type` first, with
+            folders listed before files, and files listed
+            before web links.
+            This parameter is not supported when using marker-based pagination.
+        :type sort: Optional[GetFolderTrashItemsSortArg], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'limit': to_string(limit), 'offset': to_string(offset), 'usemarker': to_string(usemarker), 'marker': to_string(marker), 'direction': to_string(direction), 'sort': to_string(sort)})
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/trash/items']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return Items.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_folders.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/trashed_web_links.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from typing import Dict
 
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
-from box_sdk_gen.schemas import TrashFolderRestored
+from box_sdk_gen.schemas import TrashWebLinkRestored
 
 from box_sdk_gen.schemas import ClientError
 
-from box_sdk_gen.schemas import TrashFolder
+from box_sdk_gen.schemas import TrashWebLink
 
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
 
@@ -26,142 +26,94 @@
 
 from box_sdk_gen.fetch import fetch
 
 from box_sdk_gen.fetch import FetchOptions
 
 from box_sdk_gen.fetch import FetchResponse
 
-class RestoreFolderFromTrashParentArg(BaseObject):
+class CreateWebLinkByIdParentArg(BaseObject):
     def __init__(self, id: Optional[str] = None, **kwargs):
         """
         :param id: The ID of parent item
         :type id: Optional[str], optional
         """
         super().__init__(**kwargs)
         self.id = id
 
-class TrashedFoldersManager:
+class TrashedWebLinksManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def restore_folder_from_trash(self, folder_id: str, name: Optional[str] = None, parent: Optional[RestoreFolderFromTrashParentArg] = None, fields: Optional[str] = None) -> TrashFolderRestored:
+    def create_web_link_by_id(self, web_link_id: str, name: Optional[str] = None, parent: Optional[CreateWebLinkByIdParentArg] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TrashWebLinkRestored:
         """
-        Restores a folder that has been moved to the trash.
+        Restores a web link that has been moved to the trash.
         
-        An optional new parent ID can be provided to restore the folder to in case the
+        An optional new parent ID can be provided to restore the  web link to in case
 
         
-        original folder has been deleted.
+        the original folder has been deleted.
 
-        
-        # Folder locking
-
-        
-        During this operation, part of the file tree will be locked, mainly
-
-        
-        the source folder and all of its descendants, as well as the destination
-
-        
-        folder.
-
-        
-        For the duration of the operation, no other move, copy, delete, or restore
-
-        
-        operation can performed on any of the locked folders.
-
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
+        :param web_link_id: The ID of the web link.
             Example: "12345"
-        :type folder_id: str
-        :param name: An optional new name for the folder.
+        :type web_link_id: str
+        :param name: An optional new name for the web link.
         :type name: Optional[str], optional
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, parent=parent)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id]), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
-        return TrashFolderRestored.from_dict(json.loads(response.text))
-    def get_folder_trash(self, folder_id: str, fields: Optional[str] = None) -> TrashFolder:
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id]), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        return TrashWebLinkRestored.from_dict(json.loads(response.text))
+    def get_web_link_trash(self, web_link_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> TrashWebLink:
         """
-        Retrieves a folder that has been moved to the trash.
-        
-        Please note that only if the folder itself has been moved to the
-
-        
-        trash can it be retrieved with this API call. If instead one of
-
-        
-        its parent folders was moved to the trash, only that folder
-
-        
-        can be inspected using the
-
-        
-        [`GET /folders/:id/trash`](e://get_folders_id_trash) API.
-
-        
-        To list all items that have been moved to the trash, please
-
-        
-        use the [`GET /folders/trash/items`](e://get-folders-trash-items/)
-
-        
-        API.
-
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
+        Retrieves a web link that has been moved to the trash.
+        :param web_link_id: The ID of the web link.
             Example: "12345"
-        :type folder_id: str
+        :type web_link_id: str
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/trash']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
-        return TrashFolder.from_dict(json.loads(response.text))
-    def delete_folder_trash(self, folder_id: str) -> None:
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '/trash']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        return TrashWebLink.from_dict(json.loads(response.text))
+    def delete_web_link_trash(self, web_link_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
-        Permanently deletes a folder that is in the trash.
+        Permanently deletes a web link that is in the trash.
         
         This action cannot be undone.
 
-        :param folder_id: The unique identifier that represent a folder.
-            The ID for any folder can be determined
-            by visiting this folder in the web application
-            and copying the ID from the URL. For example,
-            for the URL `https://*.app.box.com/folder/123`
-            the `folder_id` is `123`.
-            The root folder of a Box account is
-            always represented by the ID `0`.
+        :param web_link_id: The ID of the web link.
             Example: "12345"
-        :type folder_id: str
-        """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/folders/', folder_id, '/trash']), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        :type web_link_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        """
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/web_links/', web_link_id, '/trash']), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/uploads.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/uploads.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         super().__init__(**kwargs)
         self.id = id
 
 class UploadsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def upload_file_version(self, file_id: str, attributes: UploadFileVersionAttributesArg, file: ByteStream, file_file_name: Optional[str] = None, file_content_type: Optional[str] = None, fields: Optional[str] = None, if_match: Optional[str] = None, content_md_5: Optional[str] = None) -> Files:
+    def upload_file_version(self, file_id: str, attributes: UploadFileVersionAttributesArg, file: ByteStream, file_file_name: Optional[str] = None, file_content_type: Optional[str] = None, fields: Optional[str] = None, if_match: Optional[str] = None, content_md_5: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Files:
         """
         Update a file's content. For file sizes over 50MB we recommend
         
         using the Chunk Upload APIs.
 
         
         # Request body order
@@ -153,21 +153,25 @@
             into this header and the endpoint will fail
             with a `412 Precondition Failed` if it
             has changed since.
         :type if_match: Optional[str], optional
         :param content_md_5: An optional header containing the SHA1 hash of the file to
             ensure that the file was not corrupted in transit.
         :type content_md_5: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(attributes=attributes, file=file, file_file_name=file_file_name, file_content_type=file_content_type)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match), 'content-md5': to_string(content_md_5)})
+        headers_map: Dict[str, str] = prepare_params({'if-match': to_string(if_match), 'content-md5': to_string(content_md_5), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://upload.box.com/api/2.0/files/', file_id, '/content']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, multipart_data=[MultipartItem(part_name='attributes', body=json.dumps(request_body.attributes.to_dict())), MultipartItem(part_name='file', file_stream=request_body.file, content_type=request_body.file_content_type, file_name=request_body.file_file_name)], content_type='multipart/form-data', response_format='json', auth=self.auth, network_session=self.network_session))
         return Files.from_dict(json.loads(response.text))
-    def upload_file(self, attributes: UploadFileAttributesArg, file: ByteStream, file_file_name: Optional[str] = None, file_content_type: Optional[str] = None, fields: Optional[str] = None, content_md_5: Optional[str] = None) -> Files:
+    def upload_file(self, attributes: UploadFileAttributesArg, file: ByteStream, file_file_name: Optional[str] = None, file_content_type: Optional[str] = None, fields: Optional[str] = None, content_md_5: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Files:
         """
         Uploads a small file to Box. For file sizes over 50MB we recommend
         
         using the Chunk Upload APIs.
 
         
         # Request body order
@@ -210,27 +214,36 @@
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
         :param content_md_5: An optional header containing the SHA1 hash of the file to
             ensure that the file was not corrupted in transit.
         :type content_md_5: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(attributes=attributes, file=file, file_file_name=file_file_name, file_content_type=file_content_type)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        headers_map: Dict[str, str] = prepare_params({'content-md5': to_string(content_md_5)})
+        headers_map: Dict[str, str] = prepare_params({'content-md5': to_string(content_md_5), **extra_headers})
         response: FetchResponse = fetch(''.join(['https://upload.box.com/api/2.0/files/content']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, multipart_data=[MultipartItem(part_name='attributes', body=json.dumps(request_body.attributes.to_dict())), MultipartItem(part_name='file', file_stream=request_body.file, content_type=request_body.file_content_type, file_name=request_body.file_file_name)], content_type='multipart/form-data', response_format='json', auth=self.auth, network_session=self.network_session))
         return Files.from_dict(json.loads(response.text))
-    def preflight_file_upload(self, name: Optional[str] = None, size: Optional[int] = None, parent: Optional[PreflightFileUploadParentArg] = None) -> UploadUrl:
+    def preflight_file_upload(self, name: Optional[str] = None, size: Optional[int] = None, parent: Optional[PreflightFileUploadParentArg] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> UploadUrl:
         """
         Performs a check to verify that a file will be accepted by Box
         
         before you upload the entire file.
 
         :param name: The name for the file
         :type name: Optional[str], optional
         :param size: The size of the file in bytes
         :type size: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, size=size, parent=parent)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/content']), FetchOptions(method='OPTIONS', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/content']), FetchOptions(method='OPTIONS', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return UploadUrl.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/user_collaborations.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/user_collaborations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 
-from box_sdk_gen.base_object import BaseObject
-
 from typing import Optional
 
+from box_sdk_gen.base_object import BaseObject
+
 from typing import Dict
 
 import json
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import Collaboration
@@ -46,21 +46,21 @@
     REJECTED = 'rejected'
 
 class CreateCollaborationItemArgTypeField(str, Enum):
     FILE = 'file'
     FOLDER = 'folder'
 
 class CreateCollaborationItemArg(BaseObject):
-    def __init__(self, type: CreateCollaborationItemArgTypeField, id: str, **kwargs):
+    def __init__(self, type: Optional[CreateCollaborationItemArgTypeField] = None, id: Optional[str] = None, **kwargs):
         """
         :param type: The type of the item that this collaboration will be
             granted access to
-        :type type: CreateCollaborationItemArgTypeField
+        :type type: Optional[CreateCollaborationItemArgTypeField], optional
         :param id: The ID of the item that will be granted access to
-        :type id: str
+        :type id: Optional[str], optional
         """
         super().__init__(**kwargs)
         self.type = type
         self.id = id
 
 class CreateCollaborationAccessibleByArgTypeField(str, Enum):
     USER = 'user'
@@ -93,34 +93,39 @@
     VIEWER_UPLOADER = 'viewer uploader'
     CO_OWNER = 'co-owner'
 
 class UserCollaborationsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_collaboration_by_id(self, collaboration_id: str, fields: Optional[str] = None) -> Collaboration:
+    def get_collaboration_by_id(self, collaboration_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collaboration:
         """
         Retrieves a single collaboration.
         :param collaboration_id: The ID of the collaboration
             Example: "1234"
         :type collaboration_id: str
         :param fields: A comma-separated list of attributes to include in the
             response. This can be used to request fields that are
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations/', collaboration_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations/', collaboration_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Collaboration.from_dict(json.loads(response.text))
-    def update_collaboration_by_id(self, collaboration_id: str, role: UpdateCollaborationByIdRoleArg, status: Optional[UpdateCollaborationByIdStatusArg] = None, expires_at: Optional[str] = None, can_view_path: Optional[bool] = None) -> Collaboration:
+    def update_collaboration_by_id(self, collaboration_id: str, role: UpdateCollaborationByIdRoleArg, status: Optional[UpdateCollaborationByIdStatusArg] = None, expires_at: Optional[str] = None, can_view_path: Optional[bool] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collaboration:
         """
         Updates a collaboration.
         
         Can be used to change the owner of an item, or to
 
         
         accept collaboration invites.
@@ -153,28 +158,38 @@
             Be aware that this meaningfully increases the time required to load the
             invitee's **All Files** page. We recommend you limit the number of
             collaborations with `can_view_path` enabled to 1,000 per user.
             Only owner or co-owners can invite collaborators with a `can_view_path` of
             `true`.
             `can_view_path` can only be used for folder collaborations.
         :type can_view_path: Optional[bool], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(role=role, status=status, expires_at=expires_at, can_view_path=can_view_path)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations/', collaboration_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations/', collaboration_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Collaboration.from_dict(json.loads(response.text))
-    def delete_collaboration_by_id(self, collaboration_id: str) -> None:
+    def delete_collaboration_by_id(self, collaboration_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a single collaboration.
         :param collaboration_id: The ID of the collaboration
             Example: "1234"
         :type collaboration_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations/', collaboration_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations/', collaboration_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
-    def create_collaboration(self, item: CreateCollaborationItemArg, accessible_by: CreateCollaborationAccessibleByArg, role: CreateCollaborationRoleArg, can_view_path: Optional[bool] = None, expires_at: Optional[str] = None, fields: Optional[str] = None, notify: Optional[bool] = None) -> Collaboration:
+    def create_collaboration(self, item: CreateCollaborationItemArg, accessible_by: CreateCollaborationAccessibleByArg, role: CreateCollaborationRoleArg, can_view_path: Optional[bool] = None, expires_at: Optional[str] = None, fields: Optional[str] = None, notify: Optional[bool] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Collaboration:
         """
         Adds a collaboration for a single user or a single group to a file
         
         or folder.
 
         
         Collaborations can be created using email address, user IDs, or a
@@ -237,12 +252,17 @@
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
         :param notify: Determines if users should receive email notification
             for the action performed.
         :type notify: Optional[bool], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(item=item, accessible_by=accessible_by, role=role, can_view_path=can_view_path, expires_at=expires_at)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields), 'notify': to_string(notify)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/collaborations']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Collaboration.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/users.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/users.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         super().__init__(**kwargs)
         self.email = email
 
 class UsersManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_users(self, filter_term: Optional[str] = None, user_type: Optional[GetUsersUserTypeArg] = None, external_app_user_id: Optional[str] = None, fields: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None, usemarker: Optional[bool] = None, marker: Optional[str] = None) -> Users:
+    def get_users(self, filter_term: Optional[str] = None, user_type: Optional[GetUsersUserTypeArg] = None, external_app_user_id: Optional[str] = None, fields: Optional[str] = None, offset: Optional[int] = None, limit: Optional[int] = None, usemarker: Optional[bool] = None, marker: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Users:
         """
         Returns a list of all users for the Enterprise along with their `user_id`,
         
         `public_name`, and `login`.
 
         
         The application and the authenticated user need to
@@ -139,19 +139,24 @@
             that can be passed as a parameter to this endpoint to get the next
             page of the response.
         :type usemarker: Optional[bool], optional
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'filter_term': to_string(filter_term), 'user_type': to_string(user_type), 'external_app_user_id': to_string(external_app_user_id), 'fields': to_string(fields), 'offset': to_string(offset), 'limit': to_string(limit), 'usemarker': to_string(usemarker), 'marker': to_string(marker)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Users.from_dict(json.loads(response.text))
-    def create_user(self, name: str, login: Optional[str] = None, is_platform_access_only: Optional[bool] = None, role: Optional[CreateUserRoleArg] = None, language: Optional[str] = None, is_sync_enabled: Optional[bool] = None, job_title: Optional[str] = None, phone: Optional[str] = None, address: Optional[str] = None, space_amount: Optional[int] = None, tracking_codes: Optional[List[TrackingCode]] = None, can_see_managed_users: Optional[bool] = None, timezone: Optional[str] = None, is_external_collab_restricted: Optional[bool] = None, is_exempt_from_device_limits: Optional[bool] = None, is_exempt_from_login_verification: Optional[bool] = None, status: Optional[CreateUserStatusArg] = None, external_app_user_id: Optional[str] = None, fields: Optional[str] = None) -> User:
+    def create_user(self, name: str, login: Optional[str] = None, is_platform_access_only: Optional[bool] = None, role: Optional[CreateUserRoleArg] = None, language: Optional[str] = None, is_sync_enabled: Optional[bool] = None, job_title: Optional[str] = None, phone: Optional[str] = None, address: Optional[str] = None, space_amount: Optional[int] = None, tracking_codes: Optional[List[TrackingCode]] = None, can_see_managed_users: Optional[bool] = None, timezone: Optional[str] = None, is_external_collab_restricted: Optional[bool] = None, is_exempt_from_device_limits: Optional[bool] = None, is_exempt_from_login_verification: Optional[bool] = None, status: Optional[CreateUserStatusArg] = None, external_app_user_id: Optional[str] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> User:
         """
         Creates a new managed user in an enterprise. This endpoint
         
         is only available to users and applications with the right
 
         
         admin permissions.
@@ -208,20 +213,25 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(name=name, login=login, is_platform_access_only=is_platform_access_only, role=role, language=language, is_sync_enabled=is_sync_enabled, job_title=job_title, phone=phone, address=address, space_amount=space_amount, tracking_codes=tracking_codes, can_see_managed_users=can_see_managed_users, timezone=timezone, is_external_collab_restricted=is_external_collab_restricted, is_exempt_from_device_limits=is_exempt_from_device_limits, is_exempt_from_login_verification=is_exempt_from_login_verification, status=status, external_app_user_id=external_app_user_id)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users']), FetchOptions(method='POST', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users']), FetchOptions(method='POST', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return User.from_dict(json.loads(response.text))
-    def get_user_me(self, fields: Optional[str] = None) -> UserFull:
+    def get_user_me(self, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> UserFull:
         """
         Retrieves information about the user who is currently authenticated.
         
         In the case of a client-side authenticated OAuth 2.0 application
 
         
         this will be the user who authorized the app.
@@ -243,19 +253,24 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/me']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/me']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return UserFull.from_dict(json.loads(response.text))
-    def get_user_by_id(self, user_id: str, fields: Optional[str] = None) -> UserFull:
+    def get_user_by_id(self, user_id: str, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> UserFull:
         """
         Retrieves information about a user in the enterprise.
         
         The application and the authenticated user need to
 
         
         have the permission to look up users in the entire
@@ -286,19 +301,24 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id]), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id]), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return UserFull.from_dict(json.loads(response.text))
-    def update_user_by_id(self, user_id: str, enterprise: Optional[str] = None, notify: Optional[bool] = None, name: Optional[str] = None, login: Optional[str] = None, role: Optional[UpdateUserByIdRoleArg] = None, language: Optional[str] = None, is_sync_enabled: Optional[bool] = None, job_title: Optional[str] = None, phone: Optional[str] = None, address: Optional[str] = None, tracking_codes: Optional[List[TrackingCode]] = None, can_see_managed_users: Optional[bool] = None, timezone: Optional[str] = None, is_external_collab_restricted: Optional[bool] = None, is_exempt_from_device_limits: Optional[bool] = None, is_exempt_from_login_verification: Optional[bool] = None, is_password_reset_required: Optional[bool] = None, status: Optional[UpdateUserByIdStatusArg] = None, space_amount: Optional[int] = None, notification_email: Optional[UpdateUserByIdNotificationEmailArg] = None, external_app_user_id: Optional[str] = None, fields: Optional[str] = None) -> UserFull:
+    def update_user_by_id(self, user_id: str, enterprise: Optional[str] = None, notify: Optional[bool] = None, name: Optional[str] = None, login: Optional[str] = None, role: Optional[UpdateUserByIdRoleArg] = None, language: Optional[str] = None, is_sync_enabled: Optional[bool] = None, job_title: Optional[str] = None, phone: Optional[str] = None, address: Optional[str] = None, tracking_codes: Optional[List[TrackingCode]] = None, can_see_managed_users: Optional[bool] = None, timezone: Optional[str] = None, is_external_collab_restricted: Optional[bool] = None, is_exempt_from_device_limits: Optional[bool] = None, is_exempt_from_login_verification: Optional[bool] = None, is_password_reset_required: Optional[bool] = None, status: Optional[UpdateUserByIdStatusArg] = None, space_amount: Optional[int] = None, notification_email: Optional[UpdateUserByIdNotificationEmailArg] = None, external_app_user_id: Optional[str] = None, fields: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> UserFull:
         """
         Updates a managed or app user in an enterprise. This endpoint
         
         is only available to users and applications with the right
 
         
         admin permissions.
@@ -372,20 +392,25 @@
             not normally returned in a standard response.
             Be aware that specifying this parameter will have the
             effect that none of the standard fields are returned in
             the response unless explicitly specified, instead only
             fields for the mini representation are returned, additional
             to the fields requested.
         :type fields: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(enterprise=enterprise, notify=notify, name=name, login=login, role=role, language=language, is_sync_enabled=is_sync_enabled, job_title=job_title, phone=phone, address=address, tracking_codes=tracking_codes, can_see_managed_users=can_see_managed_users, timezone=timezone, is_external_collab_restricted=is_external_collab_restricted, is_exempt_from_device_limits=is_exempt_from_device_limits, is_exempt_from_login_verification=is_exempt_from_login_verification, is_password_reset_required=is_password_reset_required, status=status, space_amount=space_amount, notification_email=notification_email, external_app_user_id=external_app_user_id)
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id]), FetchOptions(method='PUT', params=query_params_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id]), FetchOptions(method='PUT', params=query_params_map, headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return UserFull.from_dict(json.loads(response.text))
-    def delete_user_by_id(self, user_id: str, notify: Optional[bool] = None, force: Optional[bool] = None) -> None:
+    def delete_user_by_id(self, user_id: str, notify: Optional[bool] = None, force: Optional[bool] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a user. By default this will fail if the user
         
         still owns any content. Move their owned content first
 
         
         before proceeding, or use the `force` field to delete
@@ -398,11 +423,16 @@
         :type user_id: str
         :param notify: Whether the user will receive email notification of
             the deletion
         :type notify: Optional[bool], optional
         :param force: Whether the user should be deleted even if this user
             still own files
         :type force: Optional[bool], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'notify': to_string(notify), 'force': to_string(force)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id]), FetchOptions(method='DELETE', params=query_params_map, response_format=None, auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/users/', user_id]), FetchOptions(method='DELETE', params=query_params_map, headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/webhooks.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/webhooks.py`

 * *Files 24% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.id = id
         self.type = type
 
 class WebhooksManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_webhooks(self, marker: Optional[str] = None, limit: Optional[int] = None) -> Webhooks:
+    def get_webhooks(self, marker: Optional[str] = None, limit: Optional[int] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Webhooks:
         """
         Returns all defined webhooks for the requesting application.
         
         This API only returns webhooks that are applied to files or folders that are
 
         
         owned by the authenticated user. This means that an admin can not see webhooks
@@ -89,60 +89,85 @@
 
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'marker': to_string(marker), 'limit': to_string(limit)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Webhooks.from_dict(json.loads(response.text))
-    def create_webhook(self, target: CreateWebhookTargetArg, address: str, triggers: List[Union[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str]]) -> Webhook:
+    def create_webhook(self, target: CreateWebhookTargetArg, address: str, triggers: List[Union[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str]], extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Webhook:
         """
         Creates a webhook.
         :param target: The item that will trigger the webhook
         :type target: CreateWebhookTargetArg
         :param address: The URL that is notified by this webhook
         :type address: str
         :param triggers: An array of event names that this webhook is
             to be triggered for
         :type triggers: List[Union[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str]]
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(target=target, address=address, triggers=triggers)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Webhook.from_dict(json.loads(response.text))
-    def get_webhook_by_id(self, webhook_id: str) -> Webhook:
+    def get_webhook_by_id(self, webhook_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Webhook:
         """
         Retrieves a specific webhook
         :param webhook_id: The ID of the webhook.
             Example: "3321123"
         :type webhook_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks/', webhook_id]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks/', webhook_id]), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Webhook.from_dict(json.loads(response.text))
-    def update_webhook_by_id(self, webhook_id: str, target: Optional[UpdateWebhookByIdTargetArg] = None, address: Optional[str] = None, triggers: Optional[List[Union[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str]]] = None) -> Webhook:
+    def update_webhook_by_id(self, webhook_id: str, target: Optional[UpdateWebhookByIdTargetArg] = None, address: Optional[str] = None, triggers: Optional[List[Union[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str]]] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Webhook:
         """
         Updates a webhook.
         :param webhook_id: The ID of the webhook.
             Example: "3321123"
         :type webhook_id: str
         :param target: The item that will trigger the webhook
         :type target: Optional[UpdateWebhookByIdTargetArg], optional
         :param address: The URL that is notified by this webhook
         :type address: Optional[str], optional
         :param triggers: An array of event names that this webhook is
             to be triggered for
         :type triggers: Optional[List[Union[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str]]], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(target=target, address=address, triggers=triggers)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks/', webhook_id]), FetchOptions(method='PUT', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks/', webhook_id]), FetchOptions(method='PUT', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return Webhook.from_dict(json.loads(response.text))
-    def delete_webhook_by_id(self, webhook_id: str) -> None:
+    def delete_webhook_by_id(self, webhook_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Deletes a webhook.
         :param webhook_id: The ID of the webhook.
             Example: "3321123"
         :type webhook_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks/', webhook_id]), FetchOptions(method='DELETE', response_format=None, auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/webhooks/', webhook_id]), FetchOptions(method='DELETE', headers=headers_map, response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/workflows.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/workflows.py`

 * *Files 22% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self.type = type
         self.id = id
 
 class WorkflowsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def get_workflows(self, folder_id: str, trigger_type: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None) -> Workflows:
+    def get_workflows(self, folder_id: str, trigger_type: Optional[str] = None, limit: Optional[int] = None, marker: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> Workflows:
         """
         Returns list of workflows that act on a given `folder ID`, and
         
         have a flow with a trigger type of `WORKFLOW_MANUAL_START`.
 
         
         You application must be authorized to use the `Manage Box Relay` application
@@ -93,19 +93,24 @@
         :type trigger_type: Optional[str], optional
         :param limit: The maximum number of items to return per page.
         :type limit: Optional[int], optional
         :param marker: Defines the position marker at which to begin returning results. This is
             used when paginating using marker-based pagination.
             This requires `usemarker` to be set to `true`.
         :type marker: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'folder_id': to_string(folder_id), 'trigger_type': to_string(trigger_type), 'limit': to_string(limit), 'marker': to_string(marker)})
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/workflows']), FetchOptions(method='GET', params=query_params_map, response_format='json', auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/workflows']), FetchOptions(method='GET', params=query_params_map, headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return Workflows.from_dict(json.loads(response.text))
-    def create_workflow_start(self, workflow_id: str, flow: CreateWorkflowStartFlowArg, files: List, folder: CreateWorkflowStartFolderArg, type: Optional[CreateWorkflowStartTypeArg] = None, outcomes: Optional[List] = None) -> None:
+    def create_workflow_start(self, workflow_id: str, flow: CreateWorkflowStartFlowArg, files: List, folder: CreateWorkflowStartFolderArg, type: Optional[CreateWorkflowStartTypeArg] = None, outcomes: Optional[List] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> None:
         """
         Initiates a flow with a trigger type of `WORKFLOW_MANUAL_START`.
         
         You application must be authorized to use the `Manage Box Relay` application
 
         
         scope within the developer console.
@@ -120,11 +125,16 @@
         :type files: List
         :param folder: The folder object for which the workflow is configured.
         :type folder: CreateWorkflowStartFolderArg
         :param type: The type of the parameters object
         :type type: Optional[CreateWorkflowStartTypeArg], optional
         :param outcomes: A list of outcomes required to be configured at start time.
         :type outcomes: Optional[List], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
+        if extra_headers is None:
+            extra_headers = {}
         request_body: BaseObject = BaseObject(type=type, flow=flow, files=files, folder=folder, outcomes=outcomes)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/workflows/', workflow_id, '/start']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format=None, auth=self.auth, network_session=self.network_session))
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/workflows/', workflow_id, '/start']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format=None, auth=self.auth, network_session=self.network_session))
         return None
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/managers/zip_downloads.py` & `box-sdk-gen-0.1.2/box_sdk_gen/managers/zip_downloads.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 
 from typing import List
 
 from typing import Union
 
-import json
+from typing import Dict
 
-from box_sdk_gen.base_object import BaseObject
+import json
 
 from box_sdk_gen.schemas import ZipDownload
 
 from box_sdk_gen.schemas import ClientError
 
 from box_sdk_gen.schemas import ZipDownloadRequest
 
@@ -32,15 +32,15 @@
 
 from box_sdk_gen.fetch import FetchResponse
 
 class ZipDownloadsManager:
     def __init__(self, auth: Optional[Authentication] = None, network_session: Optional[NetworkSession] = None):
         self.auth = auth
         self.network_session = network_session
-    def create_zip_download(self, items: List, download_file_name: Optional[str] = None) -> ZipDownload:
+    def create_zip_download(self, items: List, download_file_name: Optional[str] = None, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ZipDownload:
         """
         Creates a request to download multiple files and folders as a single `zip`
         
         archive file. This API does not return the archive but instead performs all
 
         
         the checks to ensure that the user has access to all the items, and then
@@ -80,19 +80,24 @@
 
         :param items: A list of items to add to the `zip` archive. These can
             be folders or files.
         :type items: List
         :param download_file_name: The optional name of the `zip` archive. This name will be appended by the
             `.zip` file extension, for example `January Financials.zip`.
         :type download_file_name: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        request_body: BaseObject = BaseObject(items=items, download_file_name=download_file_name)
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/zip_downloads']), FetchOptions(method='POST', body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        request_body: ZipDownloadRequest = ZipDownloadRequest(items=items, download_file_name=download_file_name)
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/zip_downloads']), FetchOptions(method='POST', headers=headers_map, body=json.dumps(request_body.to_dict()), content_type='application/json', response_format='json', auth=self.auth, network_session=self.network_session))
         return ZipDownload.from_dict(json.loads(response.text))
-    def get_zip_download_content(self, zip_download_id: str) -> ByteStream:
+    def get_zip_download_content(self, zip_download_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ByteStream:
         """
         Returns the contents of a `zip` archive in binary format. This URL does not
         
         require any form of authentication and could be used in a user's browser to
 
         
         download the archive to a user's device.
@@ -120,18 +125,23 @@
 
         
         this endpoint.
 
         :param zip_download_id: The unique identifier that represent this `zip` archive.
             Example: "Lu6fA9Ob-jyysp3AAvMF4AkLEwZwAYbL=tgj2zIC=eK9RvJnJbjJl9rNh2qBgHDpyOCAOhpM=vajg2mKq8Mdd"
         :type zip_download_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://dl.boxcloud.com/2.0/zip_downloads/', zip_download_id, '/content']), FetchOptions(method='GET', response_format='binary', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://dl.boxcloud.com/2.0/zip_downloads/', zip_download_id, '/content']), FetchOptions(method='GET', headers=headers_map, response_format='binary', auth=self.auth, network_session=self.network_session))
         return response.content
-    def get_zip_download_status(self, zip_download_id: str) -> ZipDownloadStatus:
+    def get_zip_download_status(self, zip_download_id: str, extra_headers: Optional[Dict[str, Optional[str]]] = None) -> ZipDownloadStatus:
         """
         Returns the download status of a `zip` archive, allowing an application to
         
         inspect the progress of the download as well as the number of items that
 
         
         might have been skipped.
@@ -156,10 +166,15 @@
 
         
         this endpoint.
 
         :param zip_download_id: The unique identifier that represent this `zip` archive.
             Example: "Lu6fA9Ob-jyysp3AAvMF4AkLEwZwAYbL=tgj2zIC=eK9RvJnJbjJl9rNh2qBgHDpyOCAOhpM=vajg2mKq8Mdd"
         :type zip_download_id: str
+        :param extra_headers: Extra headers that will be included in the HTTP request.
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/zip_downloads/', zip_download_id, '/status']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
+        if extra_headers is None:
+            extra_headers = {}
+        headers_map: Dict[str, str] = prepare_params({**extra_headers})
+        response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/zip_downloads/', zip_download_id, '/status']), FetchOptions(method='GET', headers=headers_map, response_format='json', auth=self.auth, network_session=self.network_session))
         return ZipDownloadStatus.from_dict(json.loads(response.text))
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/oauth.py` & `box-sdk-gen-0.1.2/box_sdk_gen/oauth.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/schemas.py` & `box-sdk-gen-0.1.2/box_sdk_gen/schemas.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen/utils.py` & `box-sdk-gen-0.1.2/box_sdk_gen/utils.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen.egg-info/PKG-INFO` & `box-sdk-gen-0.1.2/box_sdk_gen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-sdk-gen
-Version: 0.1.1
+Version: 0.1.2
 Summary: [Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.
 Home-page: https://github.com/box/box-python-sdk-gen.git
 Author: Box
 Author-email: oss@box.com
 License: Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: box,sdk,api,rest,boxsdk
 Classifier: Development Status :: 4 - Beta
@@ -37,14 +37,16 @@
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Integration Tests](#integration-tests)
   - [Running integration tests locally](#running-integration-tests-locally)
     - [Create Custom Application](#create-custom-application)
     - [Export configuration](#export-configuration)
     - [Running tests](#running-tests)
+- [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
+- [Copyright and License](#copyright-and-license)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 # Installing
 
 ```console
 pip install box-sdk-gen
@@ -124,15 +126,15 @@
 tickets](https://github.com/box/box-python-sdk-generated/issues)! Or, if that
 doesn't work, [file a new
 one](https://github.com/box/box-python-sdk-generated/issues/new) and we will get
 back to you. If you have general questions about the Box API, you can
 post to the [Box Developer
 Forum](https://community.box.com/t5/Developer-Forum/bd-p/DeveloperForum).
 
-## Copyright and License
+# Copyright and License
 
 Copyright 2023 Box, Inc. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `box-sdk-gen-0.1.1/box_sdk_gen.egg-info/SOURCES.txt` & `box-sdk-gen-0.1.2/box_sdk_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.1/setup.py` & `box-sdk-gen-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 
 def main():
     install_requires = ['requests', 'requests_toolbelt', 'urllib3<2']
     tests_require = ['pytest', 'pytest-timeout', 'pytest-cov']
     dev_requires = ['tox']
     jwt_requires = ['pyjwt>=1.7.0', 'cryptography>=3']
     extras_require = {'test': tests_require + jwt_requires, 'dev': dev_requires, 'jwt': jwt_requires}
-    setup(name='box-sdk-gen', version='0.1.1', description='[Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.', url='https://github.com/box/box-python-sdk-gen.git', licence='Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0', author='Box', long_description_content_type='text/markdown', long_description=open(join(dirname(__file__), 'README.md'), encoding='utf-8').read(), author_email='oss@box.com', classifiers=['Development Status :: 4 - Beta', 'Intended Audience :: Developers', 'License :: OSI Approved :: Apache Software License', 'Programming Language :: Python', 'Programming Language :: Python :: 3.6', 'Programming Language :: Python :: 3.7', 'Programming Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: Implementation :: CPython', 'Programming Language :: Python :: Implementation :: PyPy', 'Operating System :: OS Independent', 'Operating System :: POSIX', 'Operating System :: Microsoft :: Windows', 'Operating System :: MacOS :: MacOS X', 'Topic :: Software Development :: Libraries :: Python Modules'], keywords='box, sdk, api, rest, boxsdk', install_requires=install_requires, tests_require=tests_require, extras_require=extras_require, packages=find_packages(exclude=['docs', '*test*']))
+    setup(name='box-sdk-gen', version='0.1.2', description='[Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.', url='https://github.com/box/box-python-sdk-gen.git', licence='Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0', author='Box', long_description_content_type='text/markdown', long_description=open(join(dirname(__file__), 'README.md'), encoding='utf-8').read(), author_email='oss@box.com', classifiers=['Development Status :: 4 - Beta', 'Intended Audience :: Developers', 'License :: OSI Approved :: Apache Software License', 'Programming Language :: Python', 'Programming Language :: Python :: 3.6', 'Programming Language :: Python :: 3.7', 'Programming Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: Implementation :: CPython', 'Programming Language :: Python :: Implementation :: PyPy', 'Operating System :: OS Independent', 'Operating System :: POSIX', 'Operating System :: Microsoft :: Windows', 'Operating System :: MacOS :: MacOS X', 'Topic :: Software Development :: Libraries :: Python Modules'], keywords='box, sdk, api, rest, boxsdk', install_requires=install_requires, tests_require=tests_require, extras_require=extras_require, packages=find_packages(exclude=['docs', '*test*']))
 
 if __name__ == '__main__':
     main()
```

