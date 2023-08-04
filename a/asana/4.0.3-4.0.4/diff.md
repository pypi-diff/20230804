# Comparing `tmp/asana-4.0.3.tar.gz` & `tmp/asana-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-rbjh1vw_/asana-4.0.3.tar", last modified: Thu Aug  3 02:44:38 2023, max compression
+gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-f537a91y/asana-4.0.4.tar", last modified: Fri Aug  4 17:19:08 2023, max compression
```

## Comparing `asana-4.0.3.tar` & `asana-4.0.4.tar`

### file list

```diff
@@ -1,941 +1,943 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:38.000000 asana-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-03 02:44:26.000000 asana-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    62600 2023-08-03 02:44:38.000000 asana-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    62371 2023-08-03 02:44:26.000000 asana-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:38.000000 asana-4.0.3/asana/
--rw-r--r--   0 runner    (1001) docker     (123)    33076 2023-08-03 02:44:26.000000 asana-4.0.3/asana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:38.000000 asana-4.0.3/asana/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45545 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28584 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52939 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/goals_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    63742 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   106576 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26060 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   163533 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29476 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api/workspaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25560 2023-08-03 02:44:26.000000 asana-4.0.3/asana/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-08-03 02:44:26.000000 asana-4.0.3/asana/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:38.000000 asana-4.0.3/asana/models/
--rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/add_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/add_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_project_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_project_template_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_project_template_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_story_response_new_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_story_response_old_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_compact_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_compact_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_request_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_request_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_user_task_list_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_workspace_membership_response_user_task_list_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/asana_named_resource_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/attachment_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/attachment_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/attachment_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/attachment_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/attachment_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/audit_log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/audit_log_event_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/audit_log_event_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/audit_log_event_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/audit_log_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/audit_log_event_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/batch_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/batch_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/batch_request_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/batch_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/batch_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/create_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/create_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_base_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_base_enum_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_base_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_gid_enum_options_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_response_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_response_people_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_field_setting_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_fields_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/custom_fields_custom_field_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/date_variable_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/date_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/empty_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/enum_option_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/enum_option_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/enum_option_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/enum_option_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/enum_options_enum_option_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/enum_options_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/error_response_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/event_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_add_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_add_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_add_supporting_work_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_gid_add_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_gid_remove_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_gid_set_metric_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_gid_set_metric_current_value_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_membership_base_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_membership_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_membership_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_metric_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_metric_current_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_base_supported_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_base_supporting_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationship_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_relationships_goal_relationship_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_remove_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_remove_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_likes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_time_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goal_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goals_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/goals_goal_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/inline_response412.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/inline_response412_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/job_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/job_base_new_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/job_base_new_project_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/job_base_new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/job_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/job_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/like.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/member_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_compact_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_compact_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_compact_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/memberships_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/modify_dependencies_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/modify_dependents_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/organization_export_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/organization_export_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/organization_export_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/organization_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/organization_export_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/organization_exports_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_add_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_gid_add_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_gid_remove_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_membership_base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_remove_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_response_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolio_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolios_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/portfolios_portfolio_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    19771 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_base_current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_base_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_brief_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_brief_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_brief_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_brief_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_brief_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_briefs_project_brief_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_duplicate_request_schedule_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_project_briefs_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_project_statuses_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_save_as_template_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_gid_sections_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_compact_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_normal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_normal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_membership_response_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    25790 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    32570 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response_created_from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response_project_brief.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_save_as_template_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_section_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_status_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_status_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_base_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_base_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_base_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_gid_instantiate_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_instantiate_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_instantiate_project_request_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_instantiate_project_request_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_template_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24102 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/project_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/projects_project_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/remove_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/remove_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/requested_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/rule_trigger_gid_run_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/rule_trigger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/rule_trigger_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/rule_trigger_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_gid_add_task_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/section_task_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/sections_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/sections_section_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_update_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_update_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_update_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_update_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_update_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/status_updates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/stories_story_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    48927 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_assignee.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_old_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_old_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_old_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_story.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/story_response_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tag_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tag_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tag_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_add_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_add_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_base_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_base_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_base_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_base_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_base_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_count_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_count_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_add_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_add_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_add_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_add_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_remove_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_remove_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_remove_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_remove_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_set_parent_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_stories_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_subtasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_gid_time_tracking_entries_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_remove_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_remove_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    43510 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    44565 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response_assignee_section.py
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/task_set_parent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/tasks_task_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/team_response_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/teams_team_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/template_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_period_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_period_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_period_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_period_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_period_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_tracking_entry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_tracking_entry_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_tracking_entry_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/time_tracking_entry_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/update_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_base_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_base_response_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_task_list_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_task_list_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_task_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_task_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/user_task_list_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_compact_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_request_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhook_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhooks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/webhooks_webhook_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_gid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_response_user_task_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_membership_response_vacation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspace_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-03 02:44:26.000000 asana-4.0.3/asana/models/workspaces_workspace_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-08-03 02:44:26.000000 asana-4.0.3/asana/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:38.000000 asana-4.0.3/asana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    62600 2023-08-03 02:44:38.000000 asana-4.0.3/asana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36288 2023-08-03 02:44:38.000000 asana-4.0.3/asana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 02:44:38.000000 asana-4.0.3/asana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 02:44:38.000000 asana-4.0.3/asana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 02:44:38.000000 asana-4.0.3/asana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 02:44:38.000000 asana-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-03 02:44:26.000000 asana-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:38.000000 asana-4.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 02:44:26.000000 asana-4.0.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_add_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_add_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_project_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_project_template_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_project_template_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_story_response_new_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_story_response_old_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_compact_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_compact_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_request_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_request_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_user_task_list_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_workspace_membership_response_user_task_list_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_all_of_workspace_membership_response_user_task_list_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_asana_named_resource_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachment_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachment_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachment_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachment_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachment_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_audit_log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_audit_log_event_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_audit_log_event_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_audit_log_event_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_audit_log_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_audit_log_event_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_request_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_batch_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_create_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_create_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_base_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_base_enum_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_base_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_gid_enum_options_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_response_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_response_people_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_setting_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_fields_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_custom_fields_custom_field_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_date_variable_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_date_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_empty_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_enum_option_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_enum_option_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_enum_option_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_enum_option_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_enum_options_enum_option_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_enum_options_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_error_response_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_event_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_add_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_add_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_add_supporting_work_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_gid_add_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_gid_remove_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_gid_set_metric_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_gid_set_metric_current_value_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_membership_base_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_membership_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_membership_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_metric_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_metric_current_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_base_supported_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_base_supporting_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationship_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_relationships_goal_relationship_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_remove_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_remove_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_likes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_time_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goal_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goals_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goals_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_goals_goal_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_inline_response412.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_inline_response412_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_job_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_job_base_new_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_job_base_new_project_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_job_base_new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_job_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_job_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_member_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_compact_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_compact_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_compact_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_memberships_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_modify_dependencies_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_modify_dependents_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_organization_export_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_organization_export_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_organization_export_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_organization_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_organization_export_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_organization_exports_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_add_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_gid_add_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_gid_remove_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_membership_base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_remove_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_response_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolio_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolios_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_portfolios_portfolio_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_base_current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_base_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_brief_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_brief_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_brief_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_brief_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_brief_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_briefs_project_brief_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_duplicate_request_schedule_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_project_briefs_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_project_statuses_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_save_as_template_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_gid_sections_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_compact_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_normal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_normal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_membership_response_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response_created_from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response_project_brief.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_save_as_template_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_section_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_status_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_status_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_base_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_base_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_base_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_gid_instantiate_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_instantiate_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_instantiate_project_request_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_instantiate_project_request_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_template_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_project_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_projects_project_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_remove_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_remove_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_requested_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_rule_trigger_gid_run_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_rule_trigger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_rule_trigger_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_rule_trigger_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_gid_add_task_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_section_task_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_sections_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_sections_section_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_update_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_update_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_update_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_update_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_update_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_status_updates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_stories_story_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_assignee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_old_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_old_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_old_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_story.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_story_response_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tag_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tag_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tag_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_add_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_add_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_base_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_base_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_base_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_base_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_base_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_count_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_count_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_add_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_add_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_add_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_add_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_remove_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_remove_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_remove_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_remove_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_set_parent_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_stories_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_subtasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_gid_time_tracking_entries_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_remove_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_remove_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response_assignee_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_task_set_parent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_tasks_task_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_team_response_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_teams_team_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_template_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_period_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_period_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_period_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_period_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_period_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_tracking_entries_time_tracking_entry_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_tracking_entry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_tracking_entry_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_tracking_entry_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_time_tracking_entry_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_update_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_base_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_base_response_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_task_list_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_task_list_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_task_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_task_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_task_list_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_compact_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_request_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhook_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhooks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_webhooks_webhook_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_gid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_response_user_task_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_membership_response_vacation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspace_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-03 02:44:26.000000 asana-4.0.3/test/test_workspaces_workspace_gid_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:19:08.000000 asana-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-04 17:18:56.000000 asana-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    62682 2023-08-04 17:19:08.000000 asana-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    62453 2023-08-04 17:18:56.000000 asana-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:19:08.000000 asana-4.0.4/asana/
+-rw-r--r--   0 runner    (1001) docker     (123)    33173 2023-08-04 17:18:56.000000 asana-4.0.4/asana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:19:08.000000 asana-4.0.4/asana/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45545 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28584 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52939 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63742 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106576 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26060 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163533 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29476 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api/workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25560 2023-08-04 17:18:56.000000 asana-4.0.4/asana/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-08-04 17:18:56.000000 asana-4.0.4/asana/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:19:08.000000 asana-4.0.4/asana/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    31204 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/attachment_response_parent_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_membership_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_membership_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_compact_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_compact_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_compact_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19771 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_compact_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_normal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_normal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25790 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32570 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24102 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/project_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48927 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44293 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45352 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/teams_team_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-04 17:18:56.000000 asana-4.0.4/asana/models/workspaces_workspace_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-08-04 17:18:56.000000 asana-4.0.4/asana/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:19:08.000000 asana-4.0.4/asana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    62682 2023-08-04 17:19:08.000000 asana-4.0.4/asana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36393 2023-08-04 17:19:08.000000 asana-4.0.4/asana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:19:08.000000 asana-4.0.4/asana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-04 17:19:08.000000 asana-4.0.4/asana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 17:19:08.000000 asana-4.0.4/asana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:19:08.000000 asana-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-04 17:18:56.000000 asana-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:19:08.000000 asana-4.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 17:18:56.000000 asana-4.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachment_response_parent_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_membership_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_membership_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_compact_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_compact_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_compact_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_compact_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_normal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_normal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_project_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_teams_team_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 17:18:56.000000 asana-4.0.4/test/test_workspaces_workspace_gid_body.py
```

### Comparing `asana-4.0.3/LICENSE` & `asana-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/PKG-INFO` & `asana-4.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1
-Name: asana
-Version: 4.0.3
-Summary: Asana
-Home-page: http://github.com/asana/python-asana
-Author: Asana, Inc
-License: MIT
-Keywords: asana,Asana
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # asana [![GitHub release][release-image]]() [![Build][github-actions-image]][github-actions-url] [![PyPi Version][pypi-image]][pypi-url]
 
 Python client library for Asana
 
 - API version: 1.0
-- Package version: 4.0.3
+- Package version: 4.0.4
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -424,14 +413,15 @@
  - [AttachmentBase](docs/AttachmentBase.md)
  - [AttachmentCompact](docs/AttachmentCompact.md)
  - [AttachmentRequest](docs/AttachmentRequest.md)
  - [AttachmentResponse](docs/AttachmentResponse.md)
  - [AttachmentResponseArray](docs/AttachmentResponseArray.md)
  - [AttachmentResponseData](docs/AttachmentResponseData.md)
  - [AttachmentResponseParent](docs/AttachmentResponseParent.md)
+ - [AttachmentResponseParentCreatedBy](docs/AttachmentResponseParentCreatedBy.md)
  - [AuditLogEvent](docs/AuditLogEvent.md)
  - [AuditLogEventActor](docs/AuditLogEventActor.md)
  - [AuditLogEventArray](docs/AuditLogEventArray.md)
  - [AuditLogEventContext](docs/AuditLogEventContext.md)
  - [AuditLogEventDetails](docs/AuditLogEventDetails.md)
  - [AuditLogEventResource](docs/AuditLogEventResource.md)
  - [BatchBody](docs/BatchBody.md)
```

### Comparing `asana-4.0.3/README.md` & `asana-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+Metadata-Version: 2.1
+Name: asana
+Version: 4.0.4
+Summary: Asana
+Home-page: http://github.com/asana/python-asana
+Author: Asana, Inc
+License: MIT
+Keywords: asana,Asana
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # asana [![GitHub release][release-image]]() [![Build][github-actions-image]][github-actions-url] [![PyPi Version][pypi-image]][pypi-url]
 
 Python client library for Asana
 
 - API version: 1.0
-- Package version: 4.0.3
+- Package version: 4.0.4
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -413,14 +424,15 @@
  - [AttachmentBase](docs/AttachmentBase.md)
  - [AttachmentCompact](docs/AttachmentCompact.md)
  - [AttachmentRequest](docs/AttachmentRequest.md)
  - [AttachmentResponse](docs/AttachmentResponse.md)
  - [AttachmentResponseArray](docs/AttachmentResponseArray.md)
  - [AttachmentResponseData](docs/AttachmentResponseData.md)
  - [AttachmentResponseParent](docs/AttachmentResponseParent.md)
+ - [AttachmentResponseParentCreatedBy](docs/AttachmentResponseParentCreatedBy.md)
  - [AuditLogEvent](docs/AuditLogEvent.md)
  - [AuditLogEventActor](docs/AuditLogEventActor.md)
  - [AuditLogEventArray](docs/AuditLogEventArray.md)
  - [AuditLogEventContext](docs/AuditLogEventContext.md)
  - [AuditLogEventDetails](docs/AuditLogEventDetails.md)
  - [AuditLogEventResource](docs/AuditLogEventResource.md)
  - [BatchBody](docs/BatchBody.md)
```

### Comparing `asana-4.0.3/asana/__init__.py` & `asana-4.0.4/asana/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 from asana.models.attachment_base import AttachmentBase
 from asana.models.attachment_compact import AttachmentCompact
 from asana.models.attachment_request import AttachmentRequest
 from asana.models.attachment_response import AttachmentResponse
 from asana.models.attachment_response_array import AttachmentResponseArray
 from asana.models.attachment_response_data import AttachmentResponseData
 from asana.models.attachment_response_parent import AttachmentResponseParent
+from asana.models.attachment_response_parent_created_by import AttachmentResponseParentCreatedBy
 from asana.models.audit_log_event import AuditLogEvent
 from asana.models.audit_log_event_actor import AuditLogEventActor
 from asana.models.audit_log_event_array import AuditLogEventArray
 from asana.models.audit_log_event_context import AuditLogEventContext
 from asana.models.audit_log_event_details import AuditLogEventDetails
 from asana.models.audit_log_event_resource import AuditLogEventResource
 from asana.models.batch_body import BatchBody
```

### Comparing `asana-4.0.3/asana/api/__init__.py` & `asana-4.0.4/asana/api/__init__.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/attachments_api.py` & `asana-4.0.4/asana/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/audit_log_api_api.py` & `asana-4.0.4/asana/api/audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/batch_api_api.py` & `asana-4.0.4/asana/api/batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/custom_field_settings_api.py` & `asana-4.0.4/asana/api/custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/custom_fields_api.py` & `asana-4.0.4/asana/api/custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/events_api.py` & `asana-4.0.4/asana/api/events_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/goal_relationships_api.py` & `asana-4.0.4/asana/api/goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/goals_api.py` & `asana-4.0.4/asana/api/goals_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/jobs_api.py` & `asana-4.0.4/asana/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/memberships_api.py` & `asana-4.0.4/asana/api/memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/organization_exports_api.py` & `asana-4.0.4/asana/api/organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/portfolio_memberships_api.py` & `asana-4.0.4/asana/api/portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/portfolios_api.py` & `asana-4.0.4/asana/api/portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/project_briefs_api.py` & `asana-4.0.4/asana/api/project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/project_memberships_api.py` & `asana-4.0.4/asana/api/project_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/project_statuses_api.py` & `asana-4.0.4/asana/api/project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/project_templates_api.py` & `asana-4.0.4/asana/api/project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/projects_api.py` & `asana-4.0.4/asana/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/rules_api.py` & `asana-4.0.4/asana/api/rules_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/sections_api.py` & `asana-4.0.4/asana/api/sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/status_updates_api.py` & `asana-4.0.4/asana/api/status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/stories_api.py` & `asana-4.0.4/asana/api/stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/tags_api.py` & `asana-4.0.4/asana/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/tasks_api.py` & `asana-4.0.4/asana/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/team_memberships_api.py` & `asana-4.0.4/asana/api/team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/teams_api.py` & `asana-4.0.4/asana/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/time_periods_api.py` & `asana-4.0.4/asana/api/time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/time_tracking_entries_api.py` & `asana-4.0.4/asana/api/time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/typeahead_api.py` & `asana-4.0.4/asana/api/typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/user_task_lists_api.py` & `asana-4.0.4/asana/api/user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/users_api.py` & `asana-4.0.4/asana/api/users_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/webhooks_api.py` & `asana-4.0.4/asana/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/workspace_memberships_api.py` & `asana-4.0.4/asana/api/workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api/workspaces_api.py` & `asana-4.0.4/asana/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/api_client.py` & `asana-4.0.4/asana/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/4.0.3/python'
+        self.user_agent = 'Swagger-Codegen/4.0.4/python'
         # Add custom header
         self.default_headers['X-Asana-Client-Lib'] = urlencode(
             {
                 'language': 'Python',
-                'version': '4.0.3',
+                'version': '4.0.4',
                 'language_version': platform.python_version(),
                 'os': platform.system(),
                 'os_version': platform.release()
             }
         )
 
     def __del__(self):
```

### Comparing `asana-4.0.3/asana/configuration.py` & `asana-4.0.4/asana/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,9 +245,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 4.0.3".\
+               "SDK Package Version: 4.0.4".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asana-4.0.3/asana/models/__init__.py` & `asana-4.0.4/asana/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from asana.models.attachment_base import AttachmentBase
 from asana.models.attachment_compact import AttachmentCompact
 from asana.models.attachment_request import AttachmentRequest
 from asana.models.attachment_response import AttachmentResponse
 from asana.models.attachment_response_array import AttachmentResponseArray
 from asana.models.attachment_response_data import AttachmentResponseData
 from asana.models.attachment_response_parent import AttachmentResponseParent
+from asana.models.attachment_response_parent_created_by import AttachmentResponseParentCreatedBy
 from asana.models.audit_log_event import AuditLogEvent
 from asana.models.audit_log_event_actor import AuditLogEventActor
 from asana.models.audit_log_event_array import AuditLogEventArray
 from asana.models.audit_log_event_context import AuditLogEventContext
 from asana.models.audit_log_event_details import AuditLogEventDetails
 from asana.models.audit_log_event_resource import AuditLogEventResource
 from asana.models.batch_body import BatchBody
```

### Comparing `asana-4.0.3/asana/models/add_custom_field_setting_request.py` & `asana-4.0.4/asana/models/add_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/add_followers_request.py` & `asana-4.0.4/asana/models/add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/add_members_request.py` & `asana-4.0.4/asana/models/add_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_project_response_owner.py` & `asana-4.0.4/asana/models/all_of_project_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_project_template_base_owner.py` & `asana-4.0.4/asana/models/all_of_project_template_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_project_template_response_owner.py` & `asana-4.0.4/asana/models/all_of_project_template_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_story_response_new_date_value.py` & `asana-4.0.4/asana/models/all_of_story_response_new_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_story_response_old_date_value.py` & `asana-4.0.4/asana/models/all_of_story_response_old_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_base_owner.py` & `asana-4.0.4/asana/models/all_of_user_task_list_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_base_workspace.py` & `asana-4.0.4/asana/models/all_of_user_task_list_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_compact_owner.py` & `asana-4.0.4/asana/models/all_of_user_task_list_compact_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_compact_workspace.py` & `asana-4.0.4/asana/models/all_of_user_task_list_compact_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_request_owner.py` & `asana-4.0.4/asana/models/all_of_user_task_list_request_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_request_workspace.py` & `asana-4.0.4/asana/models/all_of_user_task_list_request_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_response_owner.py` & `asana-4.0.4/asana/models/all_of_user_task_list_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_user_task_list_response_workspace.py` & `asana-4.0.4/asana/models/all_of_user_task_list_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_workspace_membership_response_user_task_list_owner.py` & `asana-4.0.4/asana/models/all_of_workspace_membership_response_user_task_list_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py` & `asana-4.0.4/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/asana_named_resource.py` & `asana-4.0.4/asana/models/asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/asana_named_resource_array.py` & `asana-4.0.4/asana/models/asana_named_resource_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/asana_resource.py` & `asana-4.0.4/asana/models/asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/attachment_base.py` & `asana-4.0.4/asana/models/attachment_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/attachment_compact.py` & `asana-4.0.4/asana/models/attachment_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/attachment_request.py` & `asana-4.0.4/asana/models/attachment_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/attachment_response.py` & `asana-4.0.4/asana/models/attachment_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/attachment_response_array.py` & `asana-4.0.4/asana/models/attachment_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/attachment_response_data.py` & `asana-4.0.4/asana/models/attachment_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/attachment_response_parent.py` & `asana-4.0.4/asana/models/attachment_response_parent.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
-        'resource_subtype': 'str'
+        'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
-        'resource_subtype': 'resource_subtype'
+        'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None):  # noqa: E501
         """AttachmentResponseParent - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
 
     @property
     def gid(self):
         """Gets the gid of this AttachmentResponseParent.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -145,14 +150,35 @@
 
         :param resource_subtype: The resource_subtype of this AttachmentResponseParent.  # noqa: E501
         :type: str
         """
 
         self._resource_subtype = resource_subtype
 
+    @property
+    def created_by(self):
+        """Gets the created_by of this AttachmentResponseParent.  # noqa: E501
+
+
+        :return: The created_by of this AttachmentResponseParent.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this AttachmentResponseParent.
+
+
+        :param created_by: The created_by of this AttachmentResponseParent.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asana-4.0.3/asana/models/audit_log_event.py` & `asana-4.0.4/asana/models/audit_log_event.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/audit_log_event_actor.py` & `asana-4.0.4/asana/models/audit_log_event_actor.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/audit_log_event_array.py` & `asana-4.0.4/asana/models/audit_log_event_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/audit_log_event_context.py` & `asana-4.0.4/asana/models/audit_log_event_context.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/audit_log_event_details.py` & `asana-4.0.4/asana/models/audit_log_event_details.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/audit_log_event_resource.py` & `asana-4.0.4/asana/models/audit_log_event_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/batch_body.py` & `asana-4.0.4/asana/models/batch_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/batch_request.py` & `asana-4.0.4/asana/models/batch_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/batch_request_action.py` & `asana-4.0.4/asana/models/batch_request_action.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/batch_request_actions.py` & `asana-4.0.4/asana/models/batch_request_actions.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/batch_request_options.py` & `asana-4.0.4/asana/models/batch_request_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/batch_response.py` & `asana-4.0.4/asana/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/batch_response_array.py` & `asana-4.0.4/asana/models/batch_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/create_membership_request.py` & `asana-4.0.4/asana/models/create_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/create_time_tracking_entry_request.py` & `asana-4.0.4/asana/models/create_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_base.py` & `asana-4.0.4/asana/models/custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_base_date_value.py` & `asana-4.0.4/asana/models/custom_field_base_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_base_enum_options.py` & `asana-4.0.4/asana/models/custom_field_base_enum_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_base_enum_value.py` & `asana-4.0.4/asana/models/custom_field_base_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_compact.py` & `asana-4.0.4/asana/models/custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_gid_enum_options_body.py` & `asana-4.0.4/asana/models/custom_field_gid_enum_options_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_request.py` & `asana-4.0.4/asana/models/custom_field_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_response.py` & `asana-4.0.4/asana/models/custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_response_array.py` & `asana-4.0.4/asana/models/custom_field_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_response_created_by.py` & `asana-4.0.4/asana/models/custom_field_response_created_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_response_data.py` & `asana-4.0.4/asana/models/custom_field_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_response_people_value.py` & `asana-4.0.4/asana/models/custom_field_response_people_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_base.py` & `asana-4.0.4/asana/models/custom_field_setting_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_compact.py` & `asana-4.0.4/asana/models/custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_response.py` & `asana-4.0.4/asana/models/custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_response_array.py` & `asana-4.0.4/asana/models/custom_field_setting_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_response_custom_field.py` & `asana-4.0.4/asana/models/custom_field_setting_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_response_data.py` & `asana-4.0.4/asana/models/custom_field_setting_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_response_parent.py` & `asana-4.0.4/asana/models/custom_field_setting_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_field_setting_response_project.py` & `asana-4.0.4/asana/models/custom_field_setting_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_fields_body.py` & `asana-4.0.4/asana/models/custom_fields_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/custom_fields_custom_field_gid_body.py` & `asana-4.0.4/asana/models/custom_fields_custom_field_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/date_variable_compact.py` & `asana-4.0.4/asana/models/date_variable_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/date_variable_request.py` & `asana-4.0.4/asana/models/date_variable_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/empty_response.py` & `asana-4.0.4/asana/models/empty_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/empty_response_data.py` & `asana-4.0.4/asana/models/empty_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/enum_option.py` & `asana-4.0.4/asana/models/enum_option.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/enum_option_base.py` & `asana-4.0.4/asana/models/enum_option_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/enum_option_data.py` & `asana-4.0.4/asana/models/enum_option_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/enum_option_insert_request.py` & `asana-4.0.4/asana/models/enum_option_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/enum_option_request.py` & `asana-4.0.4/asana/models/enum_option_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/enum_options_enum_option_gid_body.py` & `asana-4.0.4/asana/models/enum_options_enum_option_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/enum_options_insert_body.py` & `asana-4.0.4/asana/models/enum_options_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/error.py` & `asana-4.0.4/asana/models/error.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/error_response.py` & `asana-4.0.4/asana/models/error_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/error_response_errors.py` & `asana-4.0.4/asana/models/error_response_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/event_response.py` & `asana-4.0.4/asana/models/event_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/event_response_array.py` & `asana-4.0.4/asana/models/event_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/event_response_change.py` & `asana-4.0.4/asana/models/event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/event_response_parent.py` & `asana-4.0.4/asana/models/event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/event_response_resource.py` & `asana-4.0.4/asana/models/event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/event_response_user.py` & `asana-4.0.4/asana/models/event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_add_subgoal_request.py` & `asana-4.0.4/asana/models/goal_add_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_add_supporting_relationship_request.py` & `asana-4.0.4/asana/models/goal_add_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_add_supporting_work_request.py` & `asana-4.0.4/asana/models/goal_add_supporting_work_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_base.py` & `asana-4.0.4/asana/models/goal_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_compact.py` & `asana-4.0.4/asana/models/goal_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_gid_add_followers_body.py` & `asana-4.0.4/asana/models/goal_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_gid_add_supporting_relationship_body.py` & `asana-4.0.4/asana/models/goal_gid_add_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_gid_remove_followers_body.py` & `asana-4.0.4/asana/models/goal_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_gid_remove_supporting_relationship_body.py` & `asana-4.0.4/asana/models/goal_gid_remove_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_gid_set_metric_body.py` & `asana-4.0.4/asana/models/goal_gid_set_metric_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_gid_set_metric_current_value_body.py` & `asana-4.0.4/asana/models/goal_gid_set_metric_current_value_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_membership_base.py` & `asana-4.0.4/asana/models/goal_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_membership_base_goal.py` & `asana-4.0.4/asana/models/goal_membership_base_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_membership_compact.py` & `asana-4.0.4/asana/models/goal_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_membership_response.py` & `asana-4.0.4/asana/models/goal_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_membership_response_user.py` & `asana-4.0.4/asana/models/goal_membership_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_membership_response_workspace.py` & `asana-4.0.4/asana/models/goal_membership_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_metric_base.py` & `asana-4.0.4/asana/models/goal_metric_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_metric_current_value_request.py` & `asana-4.0.4/asana/models/goal_metric_current_value_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_metric_request.py` & `asana-4.0.4/asana/models/goal_metric_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_base.py` & `asana-4.0.4/asana/models/goal_relationship_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_base_supported_goal.py` & `asana-4.0.4/asana/models/goal_relationship_base_supported_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_base_supporting_resource.py` & `asana-4.0.4/asana/models/goal_relationship_base_supporting_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_compact.py` & `asana-4.0.4/asana/models/goal_relationship_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_request.py` & `asana-4.0.4/asana/models/goal_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_response.py` & `asana-4.0.4/asana/models/goal_relationship_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_response_array.py` & `asana-4.0.4/asana/models/goal_relationship_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationship_response_data.py` & `asana-4.0.4/asana/models/goal_relationship_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_relationships_goal_relationship_gid_body.py` & `asana-4.0.4/asana/models/goal_relationships_goal_relationship_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_remove_subgoal_request.py` & `asana-4.0.4/asana/models/goal_remove_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_remove_supporting_relationship_request.py` & `asana-4.0.4/asana/models/goal_remove_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_request.py` & `asana-4.0.4/asana/models/goal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_request_base.py` & `asana-4.0.4/asana/models/goal_request_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response.py` & `asana-4.0.4/asana/models/goal_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_array.py` & `asana-4.0.4/asana/models/goal_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_current_status_update.py` & `asana-4.0.4/asana/models/goal_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_data.py` & `asana-4.0.4/asana/models/goal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_likes.py` & `asana-4.0.4/asana/models/goal_response_likes.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_metric.py` & `asana-4.0.4/asana/models/goal_response_metric.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_team.py` & `asana-4.0.4/asana/models/goal_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_time_period.py` & `asana-4.0.4/asana/models/goal_response_time_period.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_response_workspace.py` & `asana-4.0.4/asana/models/goal_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goal_update_request.py` & `asana-4.0.4/asana/models/goal_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goals_body.py` & `asana-4.0.4/asana/models/goals_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/goals_goal_gid_body.py` & `asana-4.0.4/asana/models/goals_goal_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/inline_response412.py` & `asana-4.0.4/asana/models/inline_response412.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/inline_response412_errors.py` & `asana-4.0.4/asana/models/inline_response412_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/job_base.py` & `asana-4.0.4/asana/models/job_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/job_base_new_project.py` & `asana-4.0.4/asana/models/job_base_new_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/job_base_new_project_template.py` & `asana-4.0.4/asana/models/job_base_new_project_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/job_base_new_task.py` & `asana-4.0.4/asana/models/job_base_new_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
-        'resource_subtype': 'str'
+        'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
-        'resource_subtype': 'resource_subtype'
+        'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None):  # noqa: E501
         """JobBaseNewTask - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
 
     @property
     def gid(self):
         """Gets the gid of this JobBaseNewTask.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -151,14 +156,35 @@
             raise ValueError(
                 "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(resource_subtype, allowed_values)
             )
 
         self._resource_subtype = resource_subtype
 
+    @property
+    def created_by(self):
+        """Gets the created_by of this JobBaseNewTask.  # noqa: E501
+
+
+        :return: The created_by of this JobBaseNewTask.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this JobBaseNewTask.
+
+
+        :param created_by: The created_by of this JobBaseNewTask.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asana-4.0.3/asana/models/job_compact.py` & `asana-4.0.4/asana/models/job_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/job_response.py` & `asana-4.0.4/asana/models/job_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/job_response_data.py` & `asana-4.0.4/asana/models/job_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/like.py` & `asana-4.0.4/asana/models/like.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/member_compact.py` & `asana-4.0.4/asana/models/member_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_compact.py` & `asana-4.0.4/asana/models/membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_compact_goal.py` & `asana-4.0.4/asana/models/membership_compact_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_compact_member.py` & `asana-4.0.4/asana/models/membership_compact_member.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_compact_parent.py` & `asana-4.0.4/asana/models/membership_compact_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_request.py` & `asana-4.0.4/asana/models/membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_response.py` & `asana-4.0.4/asana/models/membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_response_array.py` & `asana-4.0.4/asana/models/membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/membership_response_data.py` & `asana-4.0.4/asana/models/membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/memberships_body.py` & `asana-4.0.4/asana/models/memberships_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/modify_dependencies_request.py` & `asana-4.0.4/asana/models/modify_dependencies_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/modify_dependents_request.py` & `asana-4.0.4/asana/models/modify_dependents_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/next_page.py` & `asana-4.0.4/asana/models/next_page.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/organization_export_base.py` & `asana-4.0.4/asana/models/organization_export_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/organization_export_compact.py` & `asana-4.0.4/asana/models/organization_export_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/organization_export_request.py` & `asana-4.0.4/asana/models/organization_export_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/organization_export_response.py` & `asana-4.0.4/asana/models/organization_export_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/organization_export_response_data.py` & `asana-4.0.4/asana/models/organization_export_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/organization_exports_body.py` & `asana-4.0.4/asana/models/organization_exports_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_add_item_request.py` & `asana-4.0.4/asana/models/portfolio_add_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_base.py` & `asana-4.0.4/asana/models/portfolio_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_compact.py` & `asana-4.0.4/asana/models/portfolio_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_gid_add_custom_field_setting_body.py` & `asana-4.0.4/asana/models/portfolio_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_gid_add_item_body.py` & `asana-4.0.4/asana/models/portfolio_gid_add_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_gid_add_members_body.py` & `asana-4.0.4/asana/models/portfolio_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_gid_remove_custom_field_setting_body.py` & `asana-4.0.4/asana/models/portfolio_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_gid_remove_item_body.py` & `asana-4.0.4/asana/models/portfolio_gid_remove_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_gid_remove_members_body.py` & `asana-4.0.4/asana/models/portfolio_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_membership_base.py` & `asana-4.0.4/asana/models/portfolio_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_membership_base_portfolio.py` & `asana-4.0.4/asana/models/portfolio_membership_base_portfolio.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_membership_compact.py` & `asana-4.0.4/asana/models/portfolio_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_membership_response.py` & `asana-4.0.4/asana/models/portfolio_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_membership_response_array.py` & `asana-4.0.4/asana/models/portfolio_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_membership_response_data.py` & `asana-4.0.4/asana/models/portfolio_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_remove_item_request.py` & `asana-4.0.4/asana/models/portfolio_remove_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_request.py` & `asana-4.0.4/asana/models/portfolio_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_response.py` & `asana-4.0.4/asana/models/portfolio_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_response_array.py` & `asana-4.0.4/asana/models/portfolio_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_response_current_status_update.py` & `asana-4.0.4/asana/models/portfolio_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_response_custom_field_settings.py` & `asana-4.0.4/asana/models/portfolio_response_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_response_custom_fields.py` & `asana-4.0.4/asana/models/portfolio_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_response_data.py` & `asana-4.0.4/asana/models/portfolio_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolio_response_workspace.py` & `asana-4.0.4/asana/models/portfolio_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolios_body.py` & `asana-4.0.4/asana/models/portfolios_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/portfolios_portfolio_gid_body.py` & `asana-4.0.4/asana/models/portfolios_portfolio_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/preview.py` & `asana-4.0.4/asana/models/preview.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_base.py` & `asana-4.0.4/asana/models/project_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_base_current_status.py` & `asana-4.0.4/asana/models/project_base_current_status.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_base_current_status_update.py` & `asana-4.0.4/asana/models/project_base_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_base_workspace.py` & `asana-4.0.4/asana/models/project_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_brief_base.py` & `asana-4.0.4/asana/models/project_brief_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_brief_compact.py` & `asana-4.0.4/asana/models/project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_brief_request.py` & `asana-4.0.4/asana/models/project_brief_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_brief_response.py` & `asana-4.0.4/asana/models/project_brief_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_brief_response_data.py` & `asana-4.0.4/asana/models/project_brief_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_brief_response_project.py` & `asana-4.0.4/asana/models/project_brief_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_briefs_project_brief_gid_body.py` & `asana-4.0.4/asana/models/project_briefs_project_brief_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_compact.py` & `asana-4.0.4/asana/models/project_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_duplicate_request.py` & `asana-4.0.4/asana/models/project_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_duplicate_request_schedule_dates.py` & `asana-4.0.4/asana/models/project_duplicate_request_schedule_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_add_custom_field_setting_body.py` & `asana-4.0.4/asana/models/project_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_add_followers_body.py` & `asana-4.0.4/asana/models/project_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_add_members_body.py` & `asana-4.0.4/asana/models/project_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_duplicate_body.py` & `asana-4.0.4/asana/models/project_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_project_briefs_body.py` & `asana-4.0.4/asana/models/project_gid_project_briefs_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_project_statuses_body.py` & `asana-4.0.4/asana/models/project_gid_project_statuses_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_remove_custom_field_setting_body.py` & `asana-4.0.4/asana/models/project_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_remove_followers_body.py` & `asana-4.0.4/asana/models/project_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_remove_members_body.py` & `asana-4.0.4/asana/models/project_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_save_as_template_body.py` & `asana-4.0.4/asana/models/project_gid_save_as_template_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_gid_sections_body.py` & `asana-4.0.4/asana/models/project_gid_sections_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_base.py` & `asana-4.0.4/asana/models/project_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_compact.py` & `asana-4.0.4/asana/models/project_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_compact_array.py` & `asana-4.0.4/asana/models/project_membership_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_compact_response.py` & `asana-4.0.4/asana/models/project_membership_compact_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_normal_response.py` & `asana-4.0.4/asana/models/project_membership_normal_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_normal_response_data.py` & `asana-4.0.4/asana/models/project_membership_normal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_response.py` & `asana-4.0.4/asana/models/project_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_response_array.py` & `asana-4.0.4/asana/models/project_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_response_data.py` & `asana-4.0.4/asana/models/project_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_membership_response_member.py` & `asana-4.0.4/asana/models/project_membership_response_member.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_request.py` & `asana-4.0.4/asana/models/project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response.py` & `asana-4.0.4/asana/models/project_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response_array.py` & `asana-4.0.4/asana/models/project_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response_completed_by.py` & `asana-4.0.4/asana/models/project_response_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response_created_from_template.py` & `asana-4.0.4/asana/models/project_response_created_from_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response_data.py` & `asana-4.0.4/asana/models/project_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response_project_brief.py` & `asana-4.0.4/asana/models/project_response_project_brief.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response_team.py` & `asana-4.0.4/asana/models/project_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_response_workspace.py` & `asana-4.0.4/asana/models/project_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_save_as_template_request.py` & `asana-4.0.4/asana/models/project_save_as_template_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_section_insert_request.py` & `asana-4.0.4/asana/models/project_section_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_status_base.py` & `asana-4.0.4/asana/models/project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_status_compact.py` & `asana-4.0.4/asana/models/project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_status_request.py` & `asana-4.0.4/asana/models/project_status_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_status_response.py` & `asana-4.0.4/asana/models/project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_status_response_array.py` & `asana-4.0.4/asana/models/project_status_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_status_response_data.py` & `asana-4.0.4/asana/models/project_status_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_base.py` & `asana-4.0.4/asana/models/project_template_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_base_requested_dates.py` & `asana-4.0.4/asana/models/project_template_base_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_base_requested_roles.py` & `asana-4.0.4/asana/models/project_template_base_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_base_team.py` & `asana-4.0.4/asana/models/project_template_base_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_compact.py` & `asana-4.0.4/asana/models/project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_gid_instantiate_project_body.py` & `asana-4.0.4/asana/models/project_template_gid_instantiate_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_instantiate_project_request.py` & `asana-4.0.4/asana/models/project_template_instantiate_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_instantiate_project_request_requested_dates.py` & `asana-4.0.4/asana/models/project_template_instantiate_project_request_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_instantiate_project_request_requested_roles.py` & `asana-4.0.4/asana/models/project_template_instantiate_project_request_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_response.py` & `asana-4.0.4/asana/models/project_template_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_response_array.py` & `asana-4.0.4/asana/models/project_template_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_template_response_data.py` & `asana-4.0.4/asana/models/project_template_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/project_update_request.py` & `asana-4.0.4/asana/models/project_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/projects_body.py` & `asana-4.0.4/asana/models/projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/projects_project_gid_body.py` & `asana-4.0.4/asana/models/projects_project_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/remove_custom_field_setting_request.py` & `asana-4.0.4/asana/models/remove_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/remove_followers_request.py` & `asana-4.0.4/asana/models/remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/remove_members_request.py` & `asana-4.0.4/asana/models/remove_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/requested_role_request.py` & `asana-4.0.4/asana/models/requested_role_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/rule_trigger_gid_run_body.py` & `asana-4.0.4/asana/models/rule_trigger_gid_run_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/rule_trigger_request.py` & `asana-4.0.4/asana/models/rule_trigger_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/rule_trigger_response.py` & `asana-4.0.4/asana/models/rule_trigger_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/rule_trigger_response_data.py` & `asana-4.0.4/asana/models/rule_trigger_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_base.py` & `asana-4.0.4/asana/models/section_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_compact.py` & `asana-4.0.4/asana/models/section_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_gid_add_task_body.py` & `asana-4.0.4/asana/models/section_gid_add_task_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_request.py` & `asana-4.0.4/asana/models/section_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_response.py` & `asana-4.0.4/asana/models/section_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_response_array.py` & `asana-4.0.4/asana/models/section_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_response_data.py` & `asana-4.0.4/asana/models/section_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/section_task_insert_request.py` & `asana-4.0.4/asana/models/section_task_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/sections_insert_body.py` & `asana-4.0.4/asana/models/sections_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/sections_section_gid_body.py` & `asana-4.0.4/asana/models/sections_section_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_update_base.py` & `asana-4.0.4/asana/models/status_update_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_update_compact.py` & `asana-4.0.4/asana/models/status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_update_request.py` & `asana-4.0.4/asana/models/status_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_update_response.py` & `asana-4.0.4/asana/models/status_update_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_update_response_array.py` & `asana-4.0.4/asana/models/status_update_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_update_response_data.py` & `asana-4.0.4/asana/models/status_update_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_update_response_parent.py` & `asana-4.0.4/asana/models/status_update_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/status_updates_body.py` & `asana-4.0.4/asana/models/status_updates_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/stories_story_gid_body.py` & `asana-4.0.4/asana/models/stories_story_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_base.py` & `asana-4.0.4/asana/models/story_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_compact.py` & `asana-4.0.4/asana/models/story_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_request.py` & `asana-4.0.4/asana/models/story_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response.py` & `asana-4.0.4/asana/models/story_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_array.py` & `asana-4.0.4/asana/models/story_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_assignee.py` & `asana-4.0.4/asana/models/story_response_assignee.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_custom_field.py` & `asana-4.0.4/asana/models/story_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_data.py` & `asana-4.0.4/asana/models/story_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_dates.py` & `asana-4.0.4/asana/models/story_response_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_old_dates.py` & `asana-4.0.4/asana/models/story_response_old_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_old_enum_value.py` & `asana-4.0.4/asana/models/story_response_old_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_old_section.py` & `asana-4.0.4/asana/models/story_response_old_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_previews.py` & `asana-4.0.4/asana/models/story_response_previews.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_project.py` & `asana-4.0.4/asana/models/story_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_story.py` & `asana-4.0.4/asana/models/story_response_story.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_tag.py` & `asana-4.0.4/asana/models/story_response_tag.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/story_response_target.py` & `asana-4.0.4/asana/models/webhook_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,153 +11,147 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class StoryResponseTarget(object):
+class WebhookFilter(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'gid': 'str',
         'resource_type': 'str',
-        'name': 'str',
-        'resource_subtype': 'str'
+        'resource_subtype': 'str',
+        'action': 'str',
+        'fields': 'list[str]'
     }
 
     attribute_map = {
-        'gid': 'gid',
         'resource_type': 'resource_type',
-        'name': 'name',
-        'resource_subtype': 'resource_subtype'
+        'resource_subtype': 'resource_subtype',
+        'action': 'action',
+        'fields': 'fields'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None):  # noqa: E501
-        """StoryResponseTarget - a model defined in Swagger"""  # noqa: E501
-        self._gid = None
+    def __init__(self, resource_type=None, resource_subtype=None, action=None, fields=None):  # noqa: E501
+        """WebhookFilter - a model defined in Swagger"""  # noqa: E501
         self._resource_type = None
-        self._name = None
         self._resource_subtype = None
+        self._action = None
+        self._fields = None
         self.discriminator = None
-        if gid is not None:
-            self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
-        if name is not None:
-            self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if action is not None:
+            self.action = action
+        if fields is not None:
+            self.fields = fields
 
     @property
-    def gid(self):
-        """Gets the gid of this StoryResponseTarget.  # noqa: E501
+    def resource_type(self):
+        """Gets the resource_type of this WebhookFilter.  # noqa: E501
 
-        Globally unique identifier of the resource, as a string.  # noqa: E501
+        The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :return: The gid of this StoryResponseTarget.  # noqa: E501
+        :return: The resource_type of this WebhookFilter.  # noqa: E501
         :rtype: str
         """
-        return self._gid
+        return self._resource_type
 
-    @gid.setter
-    def gid(self, gid):
-        """Sets the gid of this StoryResponseTarget.
+    @resource_type.setter
+    def resource_type(self, resource_type):
+        """Sets the resource_type of this WebhookFilter.
 
-        Globally unique identifier of the resource, as a string.  # noqa: E501
+        The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :param gid: The gid of this StoryResponseTarget.  # noqa: E501
+        :param resource_type: The resource_type of this WebhookFilter.  # noqa: E501
         :type: str
         """
 
-        self._gid = gid
+        self._resource_type = resource_type
 
     @property
-    def resource_type(self):
-        """Gets the resource_type of this StoryResponseTarget.  # noqa: E501
+    def resource_subtype(self):
+        """Gets the resource_subtype of this WebhookFilter.  # noqa: E501
 
-        The base type of this resource.  # noqa: E501
+        The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :return: The resource_type of this StoryResponseTarget.  # noqa: E501
+        :return: The resource_subtype of this WebhookFilter.  # noqa: E501
         :rtype: str
         """
-        return self._resource_type
+        return self._resource_subtype
 
-    @resource_type.setter
-    def resource_type(self, resource_type):
-        """Sets the resource_type of this StoryResponseTarget.
+    @resource_subtype.setter
+    def resource_subtype(self, resource_subtype):
+        """Sets the resource_subtype of this WebhookFilter.
 
-        The base type of this resource.  # noqa: E501
+        The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :param resource_type: The resource_type of this StoryResponseTarget.  # noqa: E501
+        :param resource_subtype: The resource_subtype of this WebhookFilter.  # noqa: E501
         :type: str
         """
 
-        self._resource_type = resource_type
+        self._resource_subtype = resource_subtype
 
     @property
-    def name(self):
-        """Gets the name of this StoryResponseTarget.  # noqa: E501
+    def action(self):
+        """Gets the action of this WebhookFilter.  # noqa: E501
 
-        The name of the task.  # noqa: E501
+        The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :return: The name of this StoryResponseTarget.  # noqa: E501
+        :return: The action of this WebhookFilter.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._action
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this StoryResponseTarget.
+    @action.setter
+    def action(self, action):
+        """Sets the action of this WebhookFilter.
 
-        The name of the task.  # noqa: E501
+        The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :param name: The name of this StoryResponseTarget.  # noqa: E501
+        :param action: The action of this WebhookFilter.  # noqa: E501
         :type: str
         """
 
-        self._name = name
+        self._action = action
 
     @property
-    def resource_subtype(self):
-        """Gets the resource_subtype of this StoryResponseTarget.  # noqa: E501
+    def fields(self):
+        """Gets the fields of this WebhookFilter.  # noqa: E501
 
-        The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.  # noqa: E501
+        *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :return: The resource_subtype of this StoryResponseTarget.  # noqa: E501
-        :rtype: str
+        :return: The fields of this WebhookFilter.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._resource_subtype
+        return self._fields
 
-    @resource_subtype.setter
-    def resource_subtype(self, resource_subtype):
-        """Sets the resource_subtype of this StoryResponseTarget.
+    @fields.setter
+    def fields(self, fields):
+        """Sets the fields of this WebhookFilter.
 
-        The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.  # noqa: E501
+        *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :param resource_subtype: The resource_subtype of this StoryResponseTarget.  # noqa: E501
-        :type: str
+        :param fields: The fields of this WebhookFilter.  # noqa: E501
+        :type: list[str]
         """
-        allowed_values = ["default_task", "milestone", "section", "approval"]  # noqa: E501
-        if resource_subtype not in allowed_values:
-            raise ValueError(
-                "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
-                .format(resource_subtype, allowed_values)
-            )
 
-        self._resource_subtype = resource_subtype
+        self._fields = fields
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -172,15 +166,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(StoryResponseTarget, dict):
+        if issubclass(WebhookFilter, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -188,15 +182,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StoryResponseTarget):
+        if not isinstance(other, WebhookFilter):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asana-4.0.3/asana/models/story_response_task.py` & `asana-4.0.4/asana/models/story_response_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
-        'resource_subtype': 'str'
+        'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
-        'resource_subtype': 'resource_subtype'
+        'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None):  # noqa: E501
         """StoryResponseTask - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
 
     @property
     def gid(self):
         """Gets the gid of this StoryResponseTask.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -151,14 +156,35 @@
             raise ValueError(
                 "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(resource_subtype, allowed_values)
             )
 
         self._resource_subtype = resource_subtype
 
+    @property
+    def created_by(self):
+        """Gets the created_by of this StoryResponseTask.  # noqa: E501
+
+
+        :return: The created_by of this StoryResponseTask.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this StoryResponseTask.
+
+
+        :param created_by: The created_by of this StoryResponseTask.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asana-4.0.3/asana/models/tag_base.py` & `asana-4.0.4/asana/models/tag_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tag_compact.py` & `asana-4.0.4/asana/models/tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tag_request.py` & `asana-4.0.4/asana/models/tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tag_response.py` & `asana-4.0.4/asana/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tag_response_array.py` & `asana-4.0.4/asana/models/tag_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tag_response_data.py` & `asana-4.0.4/asana/models/tag_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tags_body.py` & `asana-4.0.4/asana/models/tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_add_followers_request.py` & `asana-4.0.4/asana/models/task_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_add_project_request.py` & `asana-4.0.4/asana/models/task_add_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_add_tag_request.py` & `asana-4.0.4/asana/models/task_add_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_base.py` & `asana-4.0.4/asana/models/task_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
         'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy',
         'approval_status': 'str',
         'assignee_status': 'str',
         'completed': 'bool',
         'completed_at': 'datetime',
         'completed_by': 'TaskBaseCompletedBy',
         'created_at': 'datetime',
         'dependencies': 'list[TaskBaseDependencies]',
@@ -61,14 +62,15 @@
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
         'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by',
         'approval_status': 'approval_status',
         'assignee_status': 'assignee_status',
         'completed': 'completed',
         'completed_at': 'completed_at',
         'completed_by': 'completed_by',
         'created_at': 'created_at',
         'dependencies': 'dependencies',
@@ -89,20 +91,21 @@
         'num_likes': 'num_likes',
         'num_subtasks': 'num_subtasks',
         'start_at': 'start_at',
         'start_on': 'start_on',
         'actual_time_minutes': 'actual_time_minutes'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, approval_status=None, assignee_status=None, completed=None, completed_at=None, completed_by=None, created_at=None, dependencies=None, dependents=None, due_at=None, due_on=None, external=None, html_notes=None, hearted=None, hearts=None, is_rendered_as_separator=None, liked=None, likes=None, memberships=None, modified_at=None, notes=None, num_hearts=None, num_likes=None, num_subtasks=None, start_at=None, start_on=None, actual_time_minutes=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None, approval_status=None, assignee_status=None, completed=None, completed_at=None, completed_by=None, created_at=None, dependencies=None, dependents=None, due_at=None, due_on=None, external=None, html_notes=None, hearted=None, hearts=None, is_rendered_as_separator=None, liked=None, likes=None, memberships=None, modified_at=None, notes=None, num_hearts=None, num_likes=None, num_subtasks=None, start_at=None, start_on=None, actual_time_minutes=None):  # noqa: E501
         """TaskBase - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self._approval_status = None
         self._assignee_status = None
         self._completed = None
         self._completed_at = None
         self._completed_by = None
         self._created_at = None
         self._dependencies = None
@@ -130,14 +133,16 @@
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
         if approval_status is not None:
             self.approval_status = approval_status
         if assignee_status is not None:
             self.assignee_status = assignee_status
         if completed is not None:
             self.completed = completed
         if completed_at is not None:
@@ -282,14 +287,35 @@
                 "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(resource_subtype, allowed_values)
             )
 
         self._resource_subtype = resource_subtype
 
     @property
+    def created_by(self):
+        """Gets the created_by of this TaskBase.  # noqa: E501
+
+
+        :return: The created_by of this TaskBase.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this TaskBase.
+
+
+        :param created_by: The created_by of this TaskBase.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
+    @property
     def approval_status(self):
         """Gets the approval_status of this TaskBase.  # noqa: E501
 
         *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.  # noqa: E501
 
         :return: The approval_status of this TaskBase.  # noqa: E501
         :rtype: str
```

### Comparing `asana-4.0.3/asana/models/task_base_completed_by.py` & `asana-4.0.4/asana/models/task_base_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_base_dependencies.py` & `asana-4.0.4/asana/models/task_base_dependencies.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_base_external.py` & `asana-4.0.4/asana/models/task_base_external.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_base_memberships.py` & `asana-4.0.4/asana/models/task_base_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_base_section.py` & `asana-4.0.4/asana/models/task_base_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_compact.py` & `asana-4.0.4/asana/models/task_compact.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
-        'resource_subtype': 'str'
+        'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
-        'resource_subtype': 'resource_subtype'
+        'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None):  # noqa: E501
         """TaskCompact - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
 
     @property
     def gid(self):
         """Gets the gid of this TaskCompact.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -151,14 +156,35 @@
             raise ValueError(
                 "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(resource_subtype, allowed_values)
             )
 
         self._resource_subtype = resource_subtype
 
+    @property
+    def created_by(self):
+        """Gets the created_by of this TaskCompact.  # noqa: E501
+
+
+        :return: The created_by of this TaskCompact.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this TaskCompact.
+
+
+        :param created_by: The created_by of this TaskCompact.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asana-4.0.3/asana/models/task_count_response.py` & `asana-4.0.4/asana/models/task_count_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_count_response_data.py` & `asana-4.0.4/asana/models/task_count_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_duplicate_request.py` & `asana-4.0.4/asana/models/task_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_add_dependencies_body.py` & `asana-4.0.4/asana/models/task_gid_add_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_add_dependents_body.py` & `asana-4.0.4/asana/models/task_gid_add_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_add_followers_body.py` & `asana-4.0.4/asana/models/task_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_add_project_body.py` & `asana-4.0.4/asana/models/task_gid_add_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_add_tag_body.py` & `asana-4.0.4/asana/models/task_gid_add_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_duplicate_body.py` & `asana-4.0.4/asana/models/task_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_remove_dependencies_body.py` & `asana-4.0.4/asana/models/task_gid_remove_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_remove_dependents_body.py` & `asana-4.0.4/asana/models/task_gid_remove_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_remove_followers_body.py` & `asana-4.0.4/asana/models/task_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_remove_project_body.py` & `asana-4.0.4/asana/models/task_gid_remove_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_remove_tag_body.py` & `asana-4.0.4/asana/models/task_gid_remove_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_set_parent_body.py` & `asana-4.0.4/asana/models/task_gid_set_parent_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_stories_body.py` & `asana-4.0.4/asana/models/task_gid_stories_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_subtasks_body.py` & `asana-4.0.4/asana/models/task_gid_subtasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_gid_time_tracking_entries_body.py` & `asana-4.0.4/asana/models/task_gid_time_tracking_entries_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_remove_followers_request.py` & `asana-4.0.4/asana/models/task_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_remove_project_request.py` & `asana-4.0.4/asana/models/task_remove_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_remove_tag_request.py` & `asana-4.0.4/asana/models/task_remove_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_request.py` & `asana-4.0.4/asana/models/task_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
         'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy',
         'approval_status': 'str',
         'assignee_status': 'str',
         'completed': 'bool',
         'completed_at': 'datetime',
         'completed_by': 'TaskBaseCompletedBy',
         'created_at': 'datetime',
         'dependencies': 'list[TaskBaseDependencies]',
@@ -69,14 +70,15 @@
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
         'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by',
         'approval_status': 'approval_status',
         'assignee_status': 'assignee_status',
         'completed': 'completed',
         'completed_at': 'completed_at',
         'completed_by': 'completed_by',
         'created_at': 'created_at',
         'dependencies': 'dependencies',
@@ -105,20 +107,21 @@
         'followers': 'followers',
         'parent': 'parent',
         'projects': 'projects',
         'tags': 'tags',
         'workspace': 'workspace'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, approval_status=None, assignee_status=None, completed=None, completed_at=None, completed_by=None, created_at=None, dependencies=None, dependents=None, due_at=None, due_on=None, external=None, html_notes=None, hearted=None, hearts=None, is_rendered_as_separator=None, liked=None, likes=None, memberships=None, modified_at=None, notes=None, num_hearts=None, num_likes=None, num_subtasks=None, start_at=None, start_on=None, actual_time_minutes=None, assignee=None, assignee_section=None, custom_fields=None, followers=None, parent=None, projects=None, tags=None, workspace=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None, approval_status=None, assignee_status=None, completed=None, completed_at=None, completed_by=None, created_at=None, dependencies=None, dependents=None, due_at=None, due_on=None, external=None, html_notes=None, hearted=None, hearts=None, is_rendered_as_separator=None, liked=None, likes=None, memberships=None, modified_at=None, notes=None, num_hearts=None, num_likes=None, num_subtasks=None, start_at=None, start_on=None, actual_time_minutes=None, assignee=None, assignee_section=None, custom_fields=None, followers=None, parent=None, projects=None, tags=None, workspace=None):  # noqa: E501
         """TaskRequest - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self._approval_status = None
         self._assignee_status = None
         self._completed = None
         self._completed_at = None
         self._completed_by = None
         self._created_at = None
         self._dependencies = None
@@ -154,14 +157,16 @@
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
         if approval_status is not None:
             self.approval_status = approval_status
         if assignee_status is not None:
             self.assignee_status = assignee_status
         if completed is not None:
             self.completed = completed
         if completed_at is not None:
@@ -322,14 +327,35 @@
                 "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(resource_subtype, allowed_values)
             )
 
         self._resource_subtype = resource_subtype
 
     @property
+    def created_by(self):
+        """Gets the created_by of this TaskRequest.  # noqa: E501
+
+
+        :return: The created_by of this TaskRequest.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this TaskRequest.
+
+
+        :param created_by: The created_by of this TaskRequest.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
+    @property
     def approval_status(self):
         """Gets the approval_status of this TaskRequest.  # noqa: E501
 
         *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.  # noqa: E501
 
         :return: The approval_status of this TaskRequest.  # noqa: E501
         :rtype: str
```

### Comparing `asana-4.0.3/asana/models/task_response.py` & `asana-4.0.4/asana/models/task_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
         'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy',
         'approval_status': 'str',
         'assignee_status': 'str',
         'completed': 'bool',
         'completed_at': 'datetime',
         'completed_by': 'TaskBaseCompletedBy',
         'created_at': 'datetime',
         'dependencies': 'list[TaskBaseDependencies]',
@@ -70,14 +71,15 @@
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
         'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by',
         'approval_status': 'approval_status',
         'assignee_status': 'assignee_status',
         'completed': 'completed',
         'completed_at': 'completed_at',
         'completed_by': 'completed_by',
         'created_at': 'created_at',
         'dependencies': 'dependencies',
@@ -107,20 +109,21 @@
         'parent': 'parent',
         'projects': 'projects',
         'tags': 'tags',
         'workspace': 'workspace',
         'permalink_url': 'permalink_url'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, approval_status=None, assignee_status=None, completed=None, completed_at=None, completed_by=None, created_at=None, dependencies=None, dependents=None, due_at=None, due_on=None, external=None, html_notes=None, hearted=None, hearts=None, is_rendered_as_separator=None, liked=None, likes=None, memberships=None, modified_at=None, notes=None, num_hearts=None, num_likes=None, num_subtasks=None, start_at=None, start_on=None, actual_time_minutes=None, assignee=None, assignee_section=None, custom_fields=None, followers=None, parent=None, projects=None, tags=None, workspace=None, permalink_url=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None, approval_status=None, assignee_status=None, completed=None, completed_at=None, completed_by=None, created_at=None, dependencies=None, dependents=None, due_at=None, due_on=None, external=None, html_notes=None, hearted=None, hearts=None, is_rendered_as_separator=None, liked=None, likes=None, memberships=None, modified_at=None, notes=None, num_hearts=None, num_likes=None, num_subtasks=None, start_at=None, start_on=None, actual_time_minutes=None, assignee=None, assignee_section=None, custom_fields=None, followers=None, parent=None, projects=None, tags=None, workspace=None, permalink_url=None):  # noqa: E501
         """TaskResponse - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self._approval_status = None
         self._assignee_status = None
         self._completed = None
         self._completed_at = None
         self._completed_by = None
         self._created_at = None
         self._dependencies = None
@@ -157,14 +160,16 @@
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
         if approval_status is not None:
             self.approval_status = approval_status
         if assignee_status is not None:
             self.assignee_status = assignee_status
         if completed is not None:
             self.completed = completed
         if completed_at is not None:
@@ -327,14 +332,35 @@
                 "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(resource_subtype, allowed_values)
             )
 
         self._resource_subtype = resource_subtype
 
     @property
+    def created_by(self):
+        """Gets the created_by of this TaskResponse.  # noqa: E501
+
+
+        :return: The created_by of this TaskResponse.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this TaskResponse.
+
+
+        :param created_by: The created_by of this TaskResponse.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
+    @property
     def approval_status(self):
         """Gets the approval_status of this TaskResponse.  # noqa: E501
 
         *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.  # noqa: E501
 
         :return: The approval_status of this TaskResponse.  # noqa: E501
         :rtype: str
```

### Comparing `asana-4.0.3/asana/models/task_response_array.py` & `asana-4.0.4/asana/models/task_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_response_assignee_section.py` & `asana-4.0.4/asana/models/task_response_assignee_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_response_custom_fields.py` & `asana-4.0.4/asana/models/task_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_response_data.py` & `asana-4.0.4/asana/models/task_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_response_parent.py` & `asana-4.0.4/asana/models/task_response_parent.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
-        'resource_subtype': 'str'
+        'resource_subtype': 'str',
+        'created_by': 'AttachmentResponseParentCreatedBy'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
-        'resource_subtype': 'resource_subtype'
+        'resource_subtype': 'resource_subtype',
+        'created_by': 'created_by'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, resource_subtype=None, created_by=None):  # noqa: E501
         """TaskResponseParent - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._resource_subtype = None
+        self._created_by = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
         if resource_subtype is not None:
             self.resource_subtype = resource_subtype
+        if created_by is not None:
+            self.created_by = created_by
 
     @property
     def gid(self):
         """Gets the gid of this TaskResponseParent.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -151,14 +156,35 @@
             raise ValueError(
                 "Invalid value for `resource_subtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(resource_subtype, allowed_values)
             )
 
         self._resource_subtype = resource_subtype
 
+    @property
+    def created_by(self):
+        """Gets the created_by of this TaskResponseParent.  # noqa: E501
+
+
+        :return: The created_by of this TaskResponseParent.  # noqa: E501
+        :rtype: AttachmentResponseParentCreatedBy
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this TaskResponseParent.
+
+
+        :param created_by: The created_by of this TaskResponseParent.  # noqa: E501
+        :type: AttachmentResponseParentCreatedBy
+        """
+
+        self._created_by = created_by
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asana-4.0.3/asana/models/task_response_tags.py` & `asana-4.0.4/asana/models/task_response_tags.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_response_workspace.py` & `asana-4.0.4/asana/models/task_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/task_set_parent_request.py` & `asana-4.0.4/asana/models/task_set_parent_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tasks_body.py` & `asana-4.0.4/asana/models/tasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/tasks_task_gid_body.py` & `asana-4.0.4/asana/models/tasks_task_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_add_user_request.py` & `asana-4.0.4/asana/models/team_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_base.py` & `asana-4.0.4/asana/models/team_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_compact.py` & `asana-4.0.4/asana/models/team_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_gid_add_user_body.py` & `asana-4.0.4/asana/models/team_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_gid_projects_body.py` & `asana-4.0.4/asana/models/team_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_gid_remove_user_body.py` & `asana-4.0.4/asana/models/team_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_membership_base.py` & `asana-4.0.4/asana/models/team_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_membership_compact.py` & `asana-4.0.4/asana/models/team_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_membership_response.py` & `asana-4.0.4/asana/models/team_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_membership_response_array.py` & `asana-4.0.4/asana/models/team_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_membership_response_data.py` & `asana-4.0.4/asana/models/team_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_remove_user_request.py` & `asana-4.0.4/asana/models/team_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_request.py` & `asana-4.0.4/asana/models/team_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_response.py` & `asana-4.0.4/asana/models/team_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_response_array.py` & `asana-4.0.4/asana/models/team_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_response_data.py` & `asana-4.0.4/asana/models/team_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/team_response_organization.py` & `asana-4.0.4/asana/models/team_response_organization.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/teams_body.py` & `asana-4.0.4/asana/models/teams_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/teams_team_gid_body.py` & `asana-4.0.4/asana/models/teams_team_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/template_role.py` & `asana-4.0.4/asana/models/template_role.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_period_base.py` & `asana-4.0.4/asana/models/time_period_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_period_compact.py` & `asana-4.0.4/asana/models/time_period_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_period_response.py` & `asana-4.0.4/asana/models/time_period_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_period_response_array.py` & `asana-4.0.4/asana/models/time_period_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_period_response_data.py` & `asana-4.0.4/asana/models/time_period_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py` & `asana-4.0.4/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_tracking_entry_base.py` & `asana-4.0.4/asana/models/time_tracking_entry_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_tracking_entry_base_data.py` & `asana-4.0.4/asana/models/time_tracking_entry_base_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_tracking_entry_compact.py` & `asana-4.0.4/asana/models/time_tracking_entry_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/time_tracking_entry_compact_array.py` & `asana-4.0.4/asana/models/time_tracking_entry_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/update_time_tracking_entry_request.py` & `asana-4.0.4/asana/models/update_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_base.py` & `asana-4.0.4/asana/models/user_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_base_response.py` & `asana-4.0.4/asana/models/user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_base_response_data.py` & `asana-4.0.4/asana/models/user_base_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_base_response_photo.py` & `asana-4.0.4/asana/models/user_base_response_photo.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_compact.py` & `asana-4.0.4/asana/models/user_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_request.py` & `asana-4.0.4/asana/models/user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_response.py` & `asana-4.0.4/asana/models/user_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_response_array.py` & `asana-4.0.4/asana/models/user_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_response_data.py` & `asana-4.0.4/asana/models/user_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_task_list_base.py` & `asana-4.0.4/asana/models/user_task_list_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_task_list_compact.py` & `asana-4.0.4/asana/models/user_task_list_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_task_list_request.py` & `asana-4.0.4/asana/models/user_task_list_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_task_list_response.py` & `asana-4.0.4/asana/models/user_task_list_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/user_task_list_response_data.py` & `asana-4.0.4/asana/models/user_task_list_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhook_compact.py` & `asana-4.0.4/asana/models/webhook_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhook_compact_resource.py` & `asana-4.0.4/asana/models/webhook_compact_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhook_filter.py` & `asana-4.0.4/asana/models/webhook_request_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class WebhookFilter(object):
+class WebhookRequestFilters(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -38,15 +38,15 @@
         'resource_type': 'resource_type',
         'resource_subtype': 'resource_subtype',
         'action': 'action',
         'fields': 'fields'
     }
 
     def __init__(self, resource_type=None, resource_subtype=None, action=None, fields=None):  # noqa: E501
-        """WebhookFilter - a model defined in Swagger"""  # noqa: E501
+        """WebhookRequestFilters - a model defined in Swagger"""  # noqa: E501
         self._resource_type = None
         self._resource_subtype = None
         self._action = None
         self._fields = None
         self.discriminator = None
         if resource_type is not None:
             self.resource_type = resource_type
@@ -55,99 +55,99 @@
         if action is not None:
             self.action = action
         if fields is not None:
             self.fields = fields
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this WebhookFilter.  # noqa: E501
+        """Gets the resource_type of this WebhookRequestFilters.  # noqa: E501
 
         The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :return: The resource_type of this WebhookFilter.  # noqa: E501
+        :return: The resource_type of this WebhookRequestFilters.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this WebhookFilter.
+        """Sets the resource_type of this WebhookRequestFilters.
 
         The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :param resource_type: The resource_type of this WebhookFilter.  # noqa: E501
+        :param resource_type: The resource_type of this WebhookRequestFilters.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
     def resource_subtype(self):
-        """Gets the resource_subtype of this WebhookFilter.  # noqa: E501
+        """Gets the resource_subtype of this WebhookRequestFilters.  # noqa: E501
 
         The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :return: The resource_subtype of this WebhookFilter.  # noqa: E501
+        :return: The resource_subtype of this WebhookRequestFilters.  # noqa: E501
         :rtype: str
         """
         return self._resource_subtype
 
     @resource_subtype.setter
     def resource_subtype(self, resource_subtype):
-        """Sets the resource_subtype of this WebhookFilter.
+        """Sets the resource_subtype of this WebhookRequestFilters.
 
         The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :param resource_subtype: The resource_subtype of this WebhookFilter.  # noqa: E501
+        :param resource_subtype: The resource_subtype of this WebhookRequestFilters.  # noqa: E501
         :type: str
         """
 
         self._resource_subtype = resource_subtype
 
     @property
     def action(self):
-        """Gets the action of this WebhookFilter.  # noqa: E501
+        """Gets the action of this WebhookRequestFilters.  # noqa: E501
 
         The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :return: The action of this WebhookFilter.  # noqa: E501
+        :return: The action of this WebhookRequestFilters.  # noqa: E501
         :rtype: str
         """
         return self._action
 
     @action.setter
     def action(self, action):
-        """Sets the action of this WebhookFilter.
+        """Sets the action of this WebhookRequestFilters.
 
         The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :param action: The action of this WebhookFilter.  # noqa: E501
+        :param action: The action of this WebhookRequestFilters.  # noqa: E501
         :type: str
         """
 
         self._action = action
 
     @property
     def fields(self):
-        """Gets the fields of this WebhookFilter.  # noqa: E501
+        """Gets the fields of this WebhookRequestFilters.  # noqa: E501
 
         *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :return: The fields of this WebhookFilter.  # noqa: E501
+        :return: The fields of this WebhookRequestFilters.  # noqa: E501
         :rtype: list[str]
         """
         return self._fields
 
     @fields.setter
     def fields(self, fields):
-        """Sets the fields of this WebhookFilter.
+        """Sets the fields of this WebhookRequestFilters.
 
         *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :param fields: The fields of this WebhookFilter.  # noqa: E501
+        :param fields: The fields of this WebhookRequestFilters.  # noqa: E501
         :type: list[str]
         """
 
         self._fields = fields
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -166,15 +166,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WebhookFilter, dict):
+        if issubclass(WebhookRequestFilters, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -182,15 +182,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WebhookFilter):
+        if not isinstance(other, WebhookRequestFilters):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asana-4.0.3/asana/models/webhook_request.py` & `asana-4.0.4/asana/models/webhook_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhook_response.py` & `asana-4.0.4/asana/models/webhook_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhook_response_array.py` & `asana-4.0.4/asana/models/webhook_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhook_response_data.py` & `asana-4.0.4/asana/models/webhook_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhook_update_request.py` & `asana-4.0.4/asana/models/webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhooks_body.py` & `asana-4.0.4/asana/models/webhooks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/webhooks_webhook_gid_body.py` & `asana-4.0.4/asana/models/webhooks_webhook_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_add_user_request.py` & `asana-4.0.4/asana/models/workspace_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_base.py` & `asana-4.0.4/asana/models/workspace_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_compact.py` & `asana-4.0.4/asana/models/workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_gid_add_user_body.py` & `asana-4.0.4/asana/models/workspace_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_gid_projects_body.py` & `asana-4.0.4/asana/models/workspace_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_gid_remove_user_body.py` & `asana-4.0.4/asana/models/workspace_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_gid_tags_body.py` & `asana-4.0.4/asana/models/workspace_gid_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_base.py` & `asana-4.0.4/asana/models/workspace_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_compact.py` & `asana-4.0.4/asana/models/workspace_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_request.py` & `asana-4.0.4/asana/models/workspace_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_response.py` & `asana-4.0.4/asana/models/workspace_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_response_array.py` & `asana-4.0.4/asana/models/workspace_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_response_data.py` & `asana-4.0.4/asana/models/workspace_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_response_user_task_list.py` & `asana-4.0.4/asana/models/workspace_membership_response_user_task_list.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_membership_response_vacation_dates.py` & `asana-4.0.4/asana/models/workspace_membership_response_vacation_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_remove_user_request.py` & `asana-4.0.4/asana/models/workspace_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_request.py` & `asana-4.0.4/asana/models/workspace_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_response.py` & `asana-4.0.4/asana/models/workspace_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_response_array.py` & `asana-4.0.4/asana/models/workspace_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspace_response_data.py` & `asana-4.0.4/asana/models/workspace_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/models/workspaces_workspace_gid_body.py` & `asana-4.0.4/asana/models/workspaces_workspace_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana/rest.py` & `asana-4.0.4/asana/rest.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/asana.egg-info/PKG-INFO` & `asana-4.0.4/asana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: asana
-Version: 4.0.3
+Version: 4.0.4
 Summary: Asana
 Home-page: http://github.com/asana/python-asana
 Author: Asana, Inc
 License: MIT
 Keywords: asana,Asana
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # asana [![GitHub release][release-image]]() [![Build][github-actions-image]][github-actions-url] [![PyPi Version][pypi-image]][pypi-url]
 
 Python client library for Asana
 
 - API version: 1.0
-- Package version: 4.0.3
+- Package version: 4.0.4
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -424,14 +424,15 @@
  - [AttachmentBase](docs/AttachmentBase.md)
  - [AttachmentCompact](docs/AttachmentCompact.md)
  - [AttachmentRequest](docs/AttachmentRequest.md)
  - [AttachmentResponse](docs/AttachmentResponse.md)
  - [AttachmentResponseArray](docs/AttachmentResponseArray.md)
  - [AttachmentResponseData](docs/AttachmentResponseData.md)
  - [AttachmentResponseParent](docs/AttachmentResponseParent.md)
+ - [AttachmentResponseParentCreatedBy](docs/AttachmentResponseParentCreatedBy.md)
  - [AuditLogEvent](docs/AuditLogEvent.md)
  - [AuditLogEventActor](docs/AuditLogEventActor.md)
  - [AuditLogEventArray](docs/AuditLogEventArray.md)
  - [AuditLogEventContext](docs/AuditLogEventContext.md)
  - [AuditLogEventDetails](docs/AuditLogEventDetails.md)
  - [AuditLogEventResource](docs/AuditLogEventResource.md)
  - [BatchBody](docs/BatchBody.md)
```

### Comparing `asana-4.0.3/asana.egg-info/SOURCES.txt` & `asana-4.0.4/asana.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 asana/models/attachment_base.py
 asana/models/attachment_compact.py
 asana/models/attachment_request.py
 asana/models/attachment_response.py
 asana/models/attachment_response_array.py
 asana/models/attachment_response_data.py
 asana/models/attachment_response_parent.py
+asana/models/attachment_response_parent_created_by.py
 asana/models/audit_log_event.py
 asana/models/audit_log_event_actor.py
 asana/models/audit_log_event_array.py
 asana/models/audit_log_event_context.py
 asana/models/audit_log_event_details.py
 asana/models/audit_log_event_resource.py
 asana/models/batch_body.py
@@ -496,14 +497,15 @@
 test/test_attachment_base.py
 test/test_attachment_compact.py
 test/test_attachment_request.py
 test/test_attachment_response.py
 test/test_attachment_response_array.py
 test/test_attachment_response_data.py
 test/test_attachment_response_parent.py
+test/test_attachment_response_parent_created_by.py
 test/test_attachments_api.py
 test/test_audit_log_api_api.py
 test/test_audit_log_event.py
 test/test_audit_log_event_actor.py
 test/test_audit_log_event_array.py
 test/test_audit_log_event_context.py
 test/test_audit_log_event_details.py
```

### Comparing `asana-4.0.3/setup.py` & `asana-4.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import os
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "asana"
-VERSION = "4.0.3"
+VERSION = "4.0.4"
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     LONG_DESCRIPTION = readme.read()
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
```

### Comparing `asana-4.0.3/test/test_add_custom_field_setting_request.py` & `asana-4.0.4/test/test_add_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_add_followers_request.py` & `asana-4.0.4/test/test_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_add_members_request.py` & `asana-4.0.4/test/test_add_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_project_response_owner.py` & `asana-4.0.4/test/test_all_of_project_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_project_template_base_owner.py` & `asana-4.0.4/test/test_all_of_project_template_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_project_template_response_owner.py` & `asana-4.0.4/test/test_all_of_project_template_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_story_response_new_date_value.py` & `asana-4.0.4/test/test_all_of_story_response_new_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_story_response_old_date_value.py` & `asana-4.0.4/test/test_all_of_story_response_old_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_base_owner.py` & `asana-4.0.4/test/test_all_of_user_task_list_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_base_workspace.py` & `asana-4.0.4/test/test_all_of_user_task_list_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_compact_owner.py` & `asana-4.0.4/test/test_all_of_user_task_list_compact_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_compact_workspace.py` & `asana-4.0.4/test/test_all_of_user_task_list_compact_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_request_owner.py` & `asana-4.0.4/test/test_all_of_user_task_list_request_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_request_workspace.py` & `asana-4.0.4/test/test_all_of_user_task_list_request_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_response_owner.py` & `asana-4.0.4/test/test_all_of_user_task_list_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_user_task_list_response_workspace.py` & `asana-4.0.4/test/test_all_of_user_task_list_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_workspace_membership_response_user_task_list_owner.py` & `asana-4.0.4/test/test_all_of_workspace_membership_response_user_task_list_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_all_of_workspace_membership_response_user_task_list_workspace.py` & `asana-4.0.4/test/test_all_of_workspace_membership_response_user_task_list_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_asana_named_resource.py` & `asana-4.0.4/test/test_asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_asana_named_resource_array.py` & `asana-4.0.4/test/test_asana_named_resource_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_asana_resource.py` & `asana-4.0.4/test/test_asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachment_base.py` & `asana-4.0.4/test/test_attachment_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachment_compact.py` & `asana-4.0.4/test/test_attachment_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachment_request.py` & `asana-4.0.4/test/test_attachment_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachment_response.py` & `asana-4.0.4/test/test_attachment_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachment_response_array.py` & `asana-4.0.4/test/test_attachment_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachment_response_data.py` & `asana-4.0.4/test/test_attachment_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachment_response_parent.py` & `asana-4.0.4/test/test_attachment_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_attachments_api.py` & `asana-4.0.4/test/test_attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_audit_log_api_api.py` & `asana-4.0.4/test/test_audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_audit_log_event.py` & `asana-4.0.4/test/test_audit_log_event.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_audit_log_event_actor.py` & `asana-4.0.4/test/test_audit_log_event_actor.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_audit_log_event_array.py` & `asana-4.0.4/test/test_audit_log_event_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_audit_log_event_context.py` & `asana-4.0.4/test/test_audit_log_event_context.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_audit_log_event_details.py` & `asana-4.0.4/test/test_audit_log_event_details.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_audit_log_event_resource.py` & `asana-4.0.4/test/test_audit_log_event_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_api_api.py` & `asana-4.0.4/test/test_batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_body.py` & `asana-4.0.4/test/test_batch_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_request.py` & `asana-4.0.4/test/test_batch_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_request_action.py` & `asana-4.0.4/test/test_batch_request_action.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_request_actions.py` & `asana-4.0.4/test/test_batch_request_actions.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_request_options.py` & `asana-4.0.4/test/test_batch_request_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_response.py` & `asana-4.0.4/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_batch_response_array.py` & `asana-4.0.4/test/test_batch_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_create_membership_request.py` & `asana-4.0.4/test/test_create_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_create_time_tracking_entry_request.py` & `asana-4.0.4/test/test_create_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_base.py` & `asana-4.0.4/test/test_custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_base_date_value.py` & `asana-4.0.4/test/test_custom_field_base_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_base_enum_options.py` & `asana-4.0.4/test/test_custom_field_base_enum_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_base_enum_value.py` & `asana-4.0.4/test/test_custom_field_base_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_compact.py` & `asana-4.0.4/test/test_custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_gid_enum_options_body.py` & `asana-4.0.4/test/test_custom_field_gid_enum_options_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_request.py` & `asana-4.0.4/test/test_custom_field_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_response.py` & `asana-4.0.4/test/test_custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_response_array.py` & `asana-4.0.4/test/test_custom_field_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_response_created_by.py` & `asana-4.0.4/test/test_custom_field_response_created_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_response_data.py` & `asana-4.0.4/test/test_custom_field_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_response_people_value.py` & `asana-4.0.4/test/test_custom_field_response_people_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_base.py` & `asana-4.0.4/test/test_custom_field_setting_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_compact.py` & `asana-4.0.4/test/test_custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_response.py` & `asana-4.0.4/test/test_custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_response_array.py` & `asana-4.0.4/test/test_custom_field_setting_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_response_custom_field.py` & `asana-4.0.4/test/test_custom_field_setting_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_response_data.py` & `asana-4.0.4/test/test_custom_field_setting_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_response_parent.py` & `asana-4.0.4/test/test_custom_field_setting_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_setting_response_project.py` & `asana-4.0.4/test/test_custom_field_setting_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_field_settings_api.py` & `asana-4.0.4/test/test_custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_fields_api.py` & `asana-4.0.4/test/test_custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_fields_body.py` & `asana-4.0.4/test/test_custom_fields_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_custom_fields_custom_field_gid_body.py` & `asana-4.0.4/test/test_custom_fields_custom_field_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_date_variable_compact.py` & `asana-4.0.4/test/test_date_variable_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_date_variable_request.py` & `asana-4.0.4/test/test_date_variable_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_empty_response.py` & `asana-4.0.4/test/test_empty_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_empty_response_data.py` & `asana-4.0.4/test/test_empty_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_enum_option.py` & `asana-4.0.4/test/test_enum_option.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_enum_option_base.py` & `asana-4.0.4/test/test_enum_option_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_enum_option_data.py` & `asana-4.0.4/test/test_enum_option_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_enum_option_insert_request.py` & `asana-4.0.4/test/test_enum_option_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_enum_option_request.py` & `asana-4.0.4/test/test_enum_option_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_enum_options_enum_option_gid_body.py` & `asana-4.0.4/test/test_enum_options_enum_option_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_enum_options_insert_body.py` & `asana-4.0.4/test/test_enum_options_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_error.py` & `asana-4.0.4/test/test_error.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_error_response.py` & `asana-4.0.4/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_error_response_errors.py` & `asana-4.0.4/test/test_error_response_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_event_response.py` & `asana-4.0.4/test/test_event_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_event_response_array.py` & `asana-4.0.4/test/test_event_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_event_response_change.py` & `asana-4.0.4/test/test_event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_event_response_parent.py` & `asana-4.0.4/test/test_event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_event_response_resource.py` & `asana-4.0.4/test/test_event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_event_response_user.py` & `asana-4.0.4/test/test_event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_events_api.py` & `asana-4.0.4/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_add_subgoal_request.py` & `asana-4.0.4/test/test_goal_add_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_add_supporting_relationship_request.py` & `asana-4.0.4/test/test_goal_add_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_add_supporting_work_request.py` & `asana-4.0.4/test/test_goal_add_supporting_work_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_base.py` & `asana-4.0.4/test/test_goal_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_compact.py` & `asana-4.0.4/test/test_goal_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_gid_add_followers_body.py` & `asana-4.0.4/test/test_goal_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_gid_add_supporting_relationship_body.py` & `asana-4.0.4/test/test_goal_gid_add_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_gid_remove_followers_body.py` & `asana-4.0.4/test/test_goal_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_gid_remove_supporting_relationship_body.py` & `asana-4.0.4/test/test_goal_gid_remove_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_gid_set_metric_body.py` & `asana-4.0.4/test/test_goal_gid_set_metric_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_gid_set_metric_current_value_body.py` & `asana-4.0.4/test/test_goal_gid_set_metric_current_value_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_membership_base.py` & `asana-4.0.4/test/test_goal_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_membership_base_goal.py` & `asana-4.0.4/test/test_goal_membership_base_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_membership_compact.py` & `asana-4.0.4/test/test_goal_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_membership_response.py` & `asana-4.0.4/test/test_goal_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_membership_response_user.py` & `asana-4.0.4/test/test_goal_membership_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_membership_response_workspace.py` & `asana-4.0.4/test/test_goal_membership_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_metric_base.py` & `asana-4.0.4/test/test_goal_metric_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_metric_current_value_request.py` & `asana-4.0.4/test/test_goal_metric_current_value_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_metric_request.py` & `asana-4.0.4/test/test_goal_metric_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_base.py` & `asana-4.0.4/test/test_goal_relationship_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_base_supported_goal.py` & `asana-4.0.4/test/test_goal_relationship_base_supported_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_base_supporting_resource.py` & `asana-4.0.4/test/test_goal_relationship_base_supporting_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_compact.py` & `asana-4.0.4/test/test_goal_relationship_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_request.py` & `asana-4.0.4/test/test_goal_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_response.py` & `asana-4.0.4/test/test_goal_relationship_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_response_array.py` & `asana-4.0.4/test/test_goal_relationship_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationship_response_data.py` & `asana-4.0.4/test/test_goal_relationship_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationships_api.py` & `asana-4.0.4/test/test_goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_relationships_goal_relationship_gid_body.py` & `asana-4.0.4/test/test_goal_relationships_goal_relationship_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_remove_subgoal_request.py` & `asana-4.0.4/test/test_goal_remove_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_remove_supporting_relationship_request.py` & `asana-4.0.4/test/test_goal_remove_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_request.py` & `asana-4.0.4/test/test_goal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_request_base.py` & `asana-4.0.4/test/test_goal_request_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response.py` & `asana-4.0.4/test/test_goal_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_array.py` & `asana-4.0.4/test/test_goal_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_current_status_update.py` & `asana-4.0.4/test/test_goal_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_data.py` & `asana-4.0.4/test/test_goal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_likes.py` & `asana-4.0.4/test/test_goal_response_likes.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_metric.py` & `asana-4.0.4/test/test_goal_response_metric.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_team.py` & `asana-4.0.4/test/test_goal_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_time_period.py` & `asana-4.0.4/test/test_goal_response_time_period.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_response_workspace.py` & `asana-4.0.4/test/test_goal_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goal_update_request.py` & `asana-4.0.4/test/test_goal_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goals_api.py` & `asana-4.0.4/test/test_goals_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goals_body.py` & `asana-4.0.4/test/test_goals_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_goals_goal_gid_body.py` & `asana-4.0.4/test/test_goals_goal_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_inline_response412.py` & `asana-4.0.4/test/test_inline_response412.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_inline_response412_errors.py` & `asana-4.0.4/test/test_inline_response412_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_job_base.py` & `asana-4.0.4/test/test_job_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_job_base_new_project.py` & `asana-4.0.4/test/test_job_base_new_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_job_base_new_project_template.py` & `asana-4.0.4/test/test_job_base_new_project_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_job_base_new_task.py` & `asana-4.0.4/test/test_job_base_new_task.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_job_compact.py` & `asana-4.0.4/test/test_job_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_job_response.py` & `asana-4.0.4/test/test_job_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_job_response_data.py` & `asana-4.0.4/test/test_job_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_jobs_api.py` & `asana-4.0.4/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_like.py` & `asana-4.0.4/test/test_like.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_member_compact.py` & `asana-4.0.4/test/test_member_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_compact.py` & `asana-4.0.4/test/test_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_compact_goal.py` & `asana-4.0.4/test/test_membership_compact_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_compact_member.py` & `asana-4.0.4/test/test_membership_compact_member.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_compact_parent.py` & `asana-4.0.4/test/test_membership_compact_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_request.py` & `asana-4.0.4/test/test_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_response.py` & `asana-4.0.4/test/test_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_response_array.py` & `asana-4.0.4/test/test_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_membership_response_data.py` & `asana-4.0.4/test/test_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_memberships_api.py` & `asana-4.0.4/test/test_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_memberships_body.py` & `asana-4.0.4/test/test_memberships_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_modify_dependencies_request.py` & `asana-4.0.4/test/test_modify_dependencies_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_modify_dependents_request.py` & `asana-4.0.4/test/test_modify_dependents_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_next_page.py` & `asana-4.0.4/test/test_next_page.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_organization_export_base.py` & `asana-4.0.4/test/test_organization_export_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_organization_export_compact.py` & `asana-4.0.4/test/test_organization_export_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_organization_export_request.py` & `asana-4.0.4/test/test_organization_export_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_organization_export_response.py` & `asana-4.0.4/test/test_organization_export_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_organization_export_response_data.py` & `asana-4.0.4/test/test_organization_export_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_organization_exports_api.py` & `asana-4.0.4/test/test_organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_organization_exports_body.py` & `asana-4.0.4/test/test_organization_exports_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_add_item_request.py` & `asana-4.0.4/test/test_portfolio_add_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_base.py` & `asana-4.0.4/test/test_portfolio_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_compact.py` & `asana-4.0.4/test/test_portfolio_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_gid_add_custom_field_setting_body.py` & `asana-4.0.4/test/test_portfolio_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_gid_add_item_body.py` & `asana-4.0.4/test/test_portfolio_gid_add_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_gid_add_members_body.py` & `asana-4.0.4/test/test_portfolio_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_gid_remove_custom_field_setting_body.py` & `asana-4.0.4/test/test_portfolio_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_gid_remove_item_body.py` & `asana-4.0.4/test/test_portfolio_gid_remove_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_gid_remove_members_body.py` & `asana-4.0.4/test/test_portfolio_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_membership_base.py` & `asana-4.0.4/test/test_portfolio_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_membership_base_portfolio.py` & `asana-4.0.4/test/test_portfolio_membership_base_portfolio.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_membership_compact.py` & `asana-4.0.4/test/test_portfolio_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_membership_response.py` & `asana-4.0.4/test/test_portfolio_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_membership_response_array.py` & `asana-4.0.4/test/test_portfolio_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_membership_response_data.py` & `asana-4.0.4/test/test_portfolio_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_memberships_api.py` & `asana-4.0.4/test/test_portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_remove_item_request.py` & `asana-4.0.4/test/test_portfolio_remove_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_request.py` & `asana-4.0.4/test/test_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_response.py` & `asana-4.0.4/test/test_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_response_array.py` & `asana-4.0.4/test/test_portfolio_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_response_current_status_update.py` & `asana-4.0.4/test/test_portfolio_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_response_custom_field_settings.py` & `asana-4.0.4/test/test_portfolio_response_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_response_custom_fields.py` & `asana-4.0.4/test/test_portfolio_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_response_data.py` & `asana-4.0.4/test/test_portfolio_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolio_response_workspace.py` & `asana-4.0.4/test/test_portfolio_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolios_api.py` & `asana-4.0.4/test/test_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolios_body.py` & `asana-4.0.4/test/test_portfolios_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_portfolios_portfolio_gid_body.py` & `asana-4.0.4/test/test_portfolios_portfolio_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_preview.py` & `asana-4.0.4/test/test_preview.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_base.py` & `asana-4.0.4/test/test_project_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_base_current_status.py` & `asana-4.0.4/test/test_project_base_current_status.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_base_current_status_update.py` & `asana-4.0.4/test/test_project_base_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_base_workspace.py` & `asana-4.0.4/test/test_project_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_brief_base.py` & `asana-4.0.4/test/test_project_brief_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_brief_compact.py` & `asana-4.0.4/test/test_project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_brief_request.py` & `asana-4.0.4/test/test_project_brief_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_brief_response.py` & `asana-4.0.4/test/test_project_brief_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_brief_response_data.py` & `asana-4.0.4/test/test_project_brief_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_brief_response_project.py` & `asana-4.0.4/test/test_project_brief_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_briefs_api.py` & `asana-4.0.4/test/test_project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_briefs_project_brief_gid_body.py` & `asana-4.0.4/test/test_project_briefs_project_brief_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_compact.py` & `asana-4.0.4/test/test_project_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_duplicate_request.py` & `asana-4.0.4/test/test_project_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_duplicate_request_schedule_dates.py` & `asana-4.0.4/test/test_project_duplicate_request_schedule_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_add_custom_field_setting_body.py` & `asana-4.0.4/test/test_project_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_add_followers_body.py` & `asana-4.0.4/test/test_project_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_add_members_body.py` & `asana-4.0.4/test/test_project_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_duplicate_body.py` & `asana-4.0.4/test/test_project_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_project_briefs_body.py` & `asana-4.0.4/test/test_project_gid_project_briefs_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_project_statuses_body.py` & `asana-4.0.4/test/test_project_gid_project_statuses_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_remove_custom_field_setting_body.py` & `asana-4.0.4/test/test_project_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_remove_followers_body.py` & `asana-4.0.4/test/test_project_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_remove_members_body.py` & `asana-4.0.4/test/test_project_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_save_as_template_body.py` & `asana-4.0.4/test/test_project_gid_save_as_template_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_gid_sections_body.py` & `asana-4.0.4/test/test_project_gid_sections_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_base.py` & `asana-4.0.4/test/test_project_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_compact.py` & `asana-4.0.4/test/test_project_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_compact_array.py` & `asana-4.0.4/test/test_project_membership_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_compact_response.py` & `asana-4.0.4/test/test_project_membership_compact_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_normal_response.py` & `asana-4.0.4/test/test_project_membership_normal_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_normal_response_data.py` & `asana-4.0.4/test/test_project_membership_normal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_response.py` & `asana-4.0.4/test/test_project_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_response_array.py` & `asana-4.0.4/test/test_project_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_response_data.py` & `asana-4.0.4/test/test_project_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_membership_response_member.py` & `asana-4.0.4/test/test_project_membership_response_member.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_memberships_api.py` & `asana-4.0.4/test/test_project_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_request.py` & `asana-4.0.4/test/test_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response.py` & `asana-4.0.4/test/test_project_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response_array.py` & `asana-4.0.4/test/test_project_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response_completed_by.py` & `asana-4.0.4/test/test_project_response_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response_created_from_template.py` & `asana-4.0.4/test/test_project_response_created_from_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response_data.py` & `asana-4.0.4/test/test_project_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response_project_brief.py` & `asana-4.0.4/test/test_project_response_project_brief.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response_team.py` & `asana-4.0.4/test/test_project_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_response_workspace.py` & `asana-4.0.4/test/test_project_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_save_as_template_request.py` & `asana-4.0.4/test/test_project_save_as_template_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_section_insert_request.py` & `asana-4.0.4/test/test_project_section_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_status_base.py` & `asana-4.0.4/test/test_project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_status_compact.py` & `asana-4.0.4/test/test_project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_status_request.py` & `asana-4.0.4/test/test_project_status_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_status_response.py` & `asana-4.0.4/test/test_project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_status_response_array.py` & `asana-4.0.4/test/test_project_status_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_status_response_data.py` & `asana-4.0.4/test/test_project_status_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_statuses_api.py` & `asana-4.0.4/test/test_project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_base.py` & `asana-4.0.4/test/test_project_template_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_base_requested_dates.py` & `asana-4.0.4/test/test_project_template_base_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_base_requested_roles.py` & `asana-4.0.4/test/test_project_template_base_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_base_team.py` & `asana-4.0.4/test/test_project_template_base_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_compact.py` & `asana-4.0.4/test/test_project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_gid_instantiate_project_body.py` & `asana-4.0.4/test/test_project_template_gid_instantiate_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_instantiate_project_request.py` & `asana-4.0.4/test/test_project_template_instantiate_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_instantiate_project_request_requested_dates.py` & `asana-4.0.4/test/test_project_template_instantiate_project_request_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_instantiate_project_request_requested_roles.py` & `asana-4.0.4/test/test_project_template_instantiate_project_request_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_response.py` & `asana-4.0.4/test/test_project_template_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_response_array.py` & `asana-4.0.4/test/test_project_template_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_template_response_data.py` & `asana-4.0.4/test/test_project_template_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_templates_api.py` & `asana-4.0.4/test/test_project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_project_update_request.py` & `asana-4.0.4/test/test_project_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_projects_api.py` & `asana-4.0.4/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_projects_body.py` & `asana-4.0.4/test/test_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_projects_project_gid_body.py` & `asana-4.0.4/test/test_projects_project_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_remove_custom_field_setting_request.py` & `asana-4.0.4/test/test_remove_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_remove_followers_request.py` & `asana-4.0.4/test/test_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_remove_members_request.py` & `asana-4.0.4/test/test_remove_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_requested_role_request.py` & `asana-4.0.4/test/test_requested_role_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_rule_trigger_gid_run_body.py` & `asana-4.0.4/test/test_rule_trigger_gid_run_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_rule_trigger_request.py` & `asana-4.0.4/test/test_rule_trigger_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_rule_trigger_response.py` & `asana-4.0.4/test/test_rule_trigger_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_rule_trigger_response_data.py` & `asana-4.0.4/test/test_rule_trigger_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_rules_api.py` & `asana-4.0.4/test/test_rules_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_base.py` & `asana-4.0.4/test/test_section_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_compact.py` & `asana-4.0.4/test/test_section_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_gid_add_task_body.py` & `asana-4.0.4/test/test_section_gid_add_task_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_request.py` & `asana-4.0.4/test/test_section_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_response.py` & `asana-4.0.4/test/test_section_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_response_array.py` & `asana-4.0.4/test/test_section_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_response_data.py` & `asana-4.0.4/test/test_section_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_section_task_insert_request.py` & `asana-4.0.4/test/test_section_task_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_sections_api.py` & `asana-4.0.4/test/test_sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_sections_insert_body.py` & `asana-4.0.4/test/test_sections_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_sections_section_gid_body.py` & `asana-4.0.4/test/test_sections_section_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_update_base.py` & `asana-4.0.4/test/test_status_update_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_update_compact.py` & `asana-4.0.4/test/test_status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_update_request.py` & `asana-4.0.4/test/test_status_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_update_response.py` & `asana-4.0.4/test/test_status_update_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_update_response_array.py` & `asana-4.0.4/test/test_status_update_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_update_response_data.py` & `asana-4.0.4/test/test_status_update_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_update_response_parent.py` & `asana-4.0.4/test/test_status_update_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_updates_api.py` & `asana-4.0.4/test/test_status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_status_updates_body.py` & `asana-4.0.4/test/test_status_updates_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_stories_api.py` & `asana-4.0.4/test/test_stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_stories_story_gid_body.py` & `asana-4.0.4/test/test_stories_story_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_base.py` & `asana-4.0.4/test/test_story_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_compact.py` & `asana-4.0.4/test/test_story_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_request.py` & `asana-4.0.4/test/test_story_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response.py` & `asana-4.0.4/test/test_story_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_array.py` & `asana-4.0.4/test/test_story_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_assignee.py` & `asana-4.0.4/test/test_story_response_assignee.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_custom_field.py` & `asana-4.0.4/test/test_story_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_data.py` & `asana-4.0.4/test/test_story_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_dates.py` & `asana-4.0.4/test/test_story_response_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_old_dates.py` & `asana-4.0.4/test/test_story_response_old_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_old_enum_value.py` & `asana-4.0.4/test/test_story_response_old_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_old_section.py` & `asana-4.0.4/test/test_story_response_old_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_previews.py` & `asana-4.0.4/test/test_story_response_previews.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_project.py` & `asana-4.0.4/test/test_story_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_story.py` & `asana-4.0.4/test/test_story_response_story.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_tag.py` & `asana-4.0.4/test/test_story_response_tag.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_target.py` & `asana-4.0.4/test/test_story_response_target.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_story_response_task.py` & `asana-4.0.4/test/test_story_response_task.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tag_base.py` & `asana-4.0.4/test/test_tag_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tag_compact.py` & `asana-4.0.4/test/test_tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tag_request.py` & `asana-4.0.4/test/test_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tag_response.py` & `asana-4.0.4/test/test_tag_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tag_response_array.py` & `asana-4.0.4/test/test_tag_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tag_response_data.py` & `asana-4.0.4/test/test_tag_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tags_api.py` & `asana-4.0.4/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tags_body.py` & `asana-4.0.4/test/test_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_add_followers_request.py` & `asana-4.0.4/test/test_task_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_add_project_request.py` & `asana-4.0.4/test/test_task_add_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_add_tag_request.py` & `asana-4.0.4/test/test_task_add_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_base.py` & `asana-4.0.4/test/test_task_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_base_completed_by.py` & `asana-4.0.4/test/test_task_base_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_base_dependencies.py` & `asana-4.0.4/test/test_task_base_dependencies.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_base_external.py` & `asana-4.0.4/test/test_task_base_external.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_base_memberships.py` & `asana-4.0.4/test/test_task_base_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_base_section.py` & `asana-4.0.4/test/test_task_base_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_compact.py` & `asana-4.0.4/test/test_task_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_count_response.py` & `asana-4.0.4/test/test_task_count_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_count_response_data.py` & `asana-4.0.4/test/test_task_count_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_duplicate_request.py` & `asana-4.0.4/test/test_task_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_add_dependencies_body.py` & `asana-4.0.4/test/test_task_gid_add_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_add_dependents_body.py` & `asana-4.0.4/test/test_task_gid_add_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_add_followers_body.py` & `asana-4.0.4/test/test_task_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_add_project_body.py` & `asana-4.0.4/test/test_task_gid_add_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_add_tag_body.py` & `asana-4.0.4/test/test_task_gid_add_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_duplicate_body.py` & `asana-4.0.4/test/test_task_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_remove_dependencies_body.py` & `asana-4.0.4/test/test_task_gid_remove_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_remove_dependents_body.py` & `asana-4.0.4/test/test_task_gid_remove_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_remove_followers_body.py` & `asana-4.0.4/test/test_task_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_remove_project_body.py` & `asana-4.0.4/test/test_task_gid_remove_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_remove_tag_body.py` & `asana-4.0.4/test/test_task_gid_remove_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_set_parent_body.py` & `asana-4.0.4/test/test_task_gid_set_parent_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_stories_body.py` & `asana-4.0.4/test/test_task_gid_stories_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_subtasks_body.py` & `asana-4.0.4/test/test_task_gid_subtasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_gid_time_tracking_entries_body.py` & `asana-4.0.4/test/test_task_gid_time_tracking_entries_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_remove_followers_request.py` & `asana-4.0.4/test/test_task_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_remove_project_request.py` & `asana-4.0.4/test/test_task_remove_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_remove_tag_request.py` & `asana-4.0.4/test/test_task_remove_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_request.py` & `asana-4.0.4/test/test_task_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response.py` & `asana-4.0.4/test/test_task_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response_array.py` & `asana-4.0.4/test/test_task_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response_assignee_section.py` & `asana-4.0.4/test/test_task_response_assignee_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response_custom_fields.py` & `asana-4.0.4/test/test_task_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response_data.py` & `asana-4.0.4/test/test_task_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response_parent.py` & `asana-4.0.4/test/test_task_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response_tags.py` & `asana-4.0.4/test/test_task_response_tags.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_response_workspace.py` & `asana-4.0.4/test/test_task_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_task_set_parent_request.py` & `asana-4.0.4/test/test_task_set_parent_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tasks_api.py` & `asana-4.0.4/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tasks_body.py` & `asana-4.0.4/test/test_tasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_tasks_task_gid_body.py` & `asana-4.0.4/test/test_tasks_task_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_add_user_request.py` & `asana-4.0.4/test/test_team_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_base.py` & `asana-4.0.4/test/test_team_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_compact.py` & `asana-4.0.4/test/test_team_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_gid_add_user_body.py` & `asana-4.0.4/test/test_team_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_gid_projects_body.py` & `asana-4.0.4/test/test_team_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_gid_remove_user_body.py` & `asana-4.0.4/test/test_team_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_membership_base.py` & `asana-4.0.4/test/test_team_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_membership_compact.py` & `asana-4.0.4/test/test_team_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_membership_response.py` & `asana-4.0.4/test/test_team_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_membership_response_array.py` & `asana-4.0.4/test/test_team_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_membership_response_data.py` & `asana-4.0.4/test/test_team_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_memberships_api.py` & `asana-4.0.4/test/test_team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_remove_user_request.py` & `asana-4.0.4/test/test_team_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_request.py` & `asana-4.0.4/test/test_team_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_response.py` & `asana-4.0.4/test/test_team_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_response_array.py` & `asana-4.0.4/test/test_team_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_response_data.py` & `asana-4.0.4/test/test_team_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_team_response_organization.py` & `asana-4.0.4/test/test_team_response_organization.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_teams_api.py` & `asana-4.0.4/test/test_teams_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_teams_body.py` & `asana-4.0.4/test/test_teams_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_teams_team_gid_body.py` & `asana-4.0.4/test/test_teams_team_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_template_role.py` & `asana-4.0.4/test/test_template_role.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_period_base.py` & `asana-4.0.4/test/test_time_period_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_period_compact.py` & `asana-4.0.4/test/test_time_period_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_period_response.py` & `asana-4.0.4/test/test_time_period_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_period_response_array.py` & `asana-4.0.4/test/test_time_period_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_period_response_data.py` & `asana-4.0.4/test/test_time_period_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_periods_api.py` & `asana-4.0.4/test/test_time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_tracking_entries_api.py` & `asana-4.0.4/test/test_time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_tracking_entries_time_tracking_entry_gid_body.py` & `asana-4.0.4/test/test_time_tracking_entries_time_tracking_entry_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_tracking_entry_base.py` & `asana-4.0.4/test/test_time_tracking_entry_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_tracking_entry_base_data.py` & `asana-4.0.4/test/test_time_tracking_entry_base_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_tracking_entry_compact.py` & `asana-4.0.4/test/test_time_tracking_entry_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_time_tracking_entry_compact_array.py` & `asana-4.0.4/test/test_time_tracking_entry_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_typeahead_api.py` & `asana-4.0.4/test/test_typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_update_time_tracking_entry_request.py` & `asana-4.0.4/test/test_update_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_base.py` & `asana-4.0.4/test/test_user_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_base_response.py` & `asana-4.0.4/test/test_user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_base_response_data.py` & `asana-4.0.4/test/test_user_base_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_base_response_photo.py` & `asana-4.0.4/test/test_user_base_response_photo.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_compact.py` & `asana-4.0.4/test/test_user_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_request.py` & `asana-4.0.4/test/test_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_response.py` & `asana-4.0.4/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_response_array.py` & `asana-4.0.4/test/test_user_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_response_data.py` & `asana-4.0.4/test/test_user_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_task_list_base.py` & `asana-4.0.4/test/test_user_task_list_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_task_list_compact.py` & `asana-4.0.4/test/test_user_task_list_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_task_list_request.py` & `asana-4.0.4/test/test_user_task_list_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_task_list_response.py` & `asana-4.0.4/test/test_user_task_list_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_task_list_response_data.py` & `asana-4.0.4/test/test_user_task_list_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_user_task_lists_api.py` & `asana-4.0.4/test/test_user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_users_api.py` & `asana-4.0.4/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_compact.py` & `asana-4.0.4/test/test_webhook_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_compact_resource.py` & `asana-4.0.4/test/test_webhook_compact_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_filter.py` & `asana-4.0.4/test/test_webhook_filter.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_request.py` & `asana-4.0.4/test/test_webhook_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_request_filters.py` & `asana-4.0.4/test/test_webhook_request_filters.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_response.py` & `asana-4.0.4/test/test_webhook_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_response_array.py` & `asana-4.0.4/test/test_webhook_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_response_data.py` & `asana-4.0.4/test/test_webhook_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhook_update_request.py` & `asana-4.0.4/test/test_webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhooks_api.py` & `asana-4.0.4/test/test_webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhooks_body.py` & `asana-4.0.4/test/test_webhooks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_webhooks_webhook_gid_body.py` & `asana-4.0.4/test/test_webhooks_webhook_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_add_user_request.py` & `asana-4.0.4/test/test_workspace_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_base.py` & `asana-4.0.4/test/test_workspace_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_compact.py` & `asana-4.0.4/test/test_workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_gid_add_user_body.py` & `asana-4.0.4/test/test_workspace_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_gid_projects_body.py` & `asana-4.0.4/test/test_workspace_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_gid_remove_user_body.py` & `asana-4.0.4/test/test_workspace_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_gid_tags_body.py` & `asana-4.0.4/test/test_workspace_gid_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_base.py` & `asana-4.0.4/test/test_workspace_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_compact.py` & `asana-4.0.4/test/test_workspace_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_request.py` & `asana-4.0.4/test/test_workspace_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_response.py` & `asana-4.0.4/test/test_workspace_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_response_array.py` & `asana-4.0.4/test/test_workspace_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_response_data.py` & `asana-4.0.4/test/test_workspace_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_response_user_task_list.py` & `asana-4.0.4/test/test_workspace_membership_response_user_task_list.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_membership_response_vacation_dates.py` & `asana-4.0.4/test/test_workspace_membership_response_vacation_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_memberships_api.py` & `asana-4.0.4/test/test_workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_remove_user_request.py` & `asana-4.0.4/test/test_workspace_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_request.py` & `asana-4.0.4/test/test_workspace_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_response.py` & `asana-4.0.4/test/test_workspace_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_response_array.py` & `asana-4.0.4/test/test_workspace_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspace_response_data.py` & `asana-4.0.4/test/test_workspace_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspaces_api.py` & `asana-4.0.4/test/test_workspaces_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.3/test/test_workspaces_workspace_gid_body.py` & `asana-4.0.4/test/test_workspaces_workspace_gid_body.py`

 * *Files identical despite different names*

