# Comparing `tmp/spellbot-9.0.2.tar.gz` & `tmp/spellbot-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spellbot-9.0.2.tar", max compression
+gzip compressed data, was "spellbot-9.0.3.tar", max compression
```

## Comparing `spellbot-9.0.2.tar` & `spellbot-9.0.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-9.0.2/LICENSE.md
--rw-r--r--   0        0        0    10824 2023-04-18 21:36:17.595924 spellbot-9.0.2/README.md
--rw-r--r--   0        0        0     3561 2023-07-19 18:16:53.234473 spellbot-9.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-9.0.2/src/spellbot/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-25 03:19:31.669125 spellbot-9.0.2/src/spellbot/_version.py
--rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-9.0.2/src/spellbot/actions/__init__.py
--rw-r--r--   0        0        0    15152 2023-07-19 16:08:41.755106 spellbot-9.0.2/src/spellbot/actions/admin_action.py
--rw-r--r--   0        0        0     3577 2023-05-26 20:08:39.547131 spellbot-9.0.2/src/spellbot/actions/base_action.py
--rw-r--r--   0        0        0     1491 2023-04-18 21:36:17.604572 spellbot-9.0.2/src/spellbot/actions/block_action.py
--rw-r--r--   0        0        0     1719 2023-07-19 16:08:41.755436 spellbot-9.0.2/src/spellbot/actions/config_action.py
--rw-r--r--   0        0        0     4951 2023-07-19 16:08:41.755771 spellbot-9.0.2/src/spellbot/actions/leave_action.py
--rw-r--r--   0        0        0    19245 2023-07-19 16:08:41.756139 spellbot-9.0.2/src/spellbot/actions/lfg_action.py
--rw-r--r--   0        0        0     3238 2023-06-14 15:20:15.566402 spellbot-9.0.2/src/spellbot/actions/score_action.py
--rw-r--r--   0        0        0     7517 2023-07-19 16:08:41.756468 spellbot-9.0.2/src/spellbot/actions/tasks_action.py
--rw-r--r--   0        0        0      996 2023-06-14 15:20:15.566614 spellbot-9.0.2/src/spellbot/actions/verify_action.py
--rw-r--r--   0        0        0     4819 2023-07-19 16:08:41.756793 spellbot-9.0.2/src/spellbot/actions/watch_action.py
--rw-r--r--   0        0        0     3470 2023-07-19 16:08:41.757174 spellbot-9.0.2/src/spellbot/cli.py
--rw-r--r--   0        0        0     6714 2023-07-19 16:08:41.757474 spellbot-9.0.2/src/spellbot/client.py
--rw-r--r--   0        0        0     2082 2023-07-19 16:08:41.757681 spellbot-9.0.2/src/spellbot/cogs/__init__.py
--rw-r--r--   0        0        0     1987 2023-04-25 03:19:31.672344 spellbot-9.0.2/src/spellbot/cogs/about_cog.py
--rw-r--r--   0        0        0     9862 2023-07-19 16:08:41.757984 spellbot-9.0.2/src/spellbot/cogs/admin_cog.py
--rw-r--r--   0        0        0     1563 2023-04-25 03:19:31.672995 spellbot-9.0.2/src/spellbot/cogs/block_cog.py
--rw-r--r--   0        0        0     1708 2023-07-19 16:08:41.758282 spellbot-9.0.2/src/spellbot/cogs/config_cog.py
--rw-r--r--   0        0        0     1673 2023-05-19 17:20:13.374286 spellbot-9.0.2/src/spellbot/cogs/events_cog.py
--rw-r--r--   0        0        0     1576 2023-07-19 16:08:41.758545 spellbot-9.0.2/src/spellbot/cogs/leave_cog.py
--rw-r--r--   0        0        0     2000 2023-07-19 16:08:41.758724 spellbot-9.0.2/src/spellbot/cogs/lfg_cog.py
--rw-r--r--   0        0        0     3128 2023-04-25 03:19:31.674236 spellbot-9.0.2/src/spellbot/cogs/owner_cog.py
--rw-r--r--   0        0        0     2182 2023-04-25 03:19:31.674424 spellbot-9.0.2/src/spellbot/cogs/score_cog.py
--rw-r--r--   0        0        0     1130 2023-04-25 03:19:31.674692 spellbot-9.0.2/src/spellbot/cogs/sync_cog.py
--rw-r--r--   0        0        0     3485 2023-07-19 16:08:41.759001 spellbot-9.0.2/src/spellbot/cogs/tasks_cog.py
--rw-r--r--   0        0        0     1658 2023-04-25 03:19:31.675274 spellbot-9.0.2/src/spellbot/cogs/verify_cog.py
--rw-r--r--   0        0        0     2672 2023-07-19 16:08:41.759238 spellbot-9.0.2/src/spellbot/cogs/watch_cog.py
--rw-r--r--   0        0        0     4708 2023-05-26 20:08:39.548488 spellbot-9.0.2/src/spellbot/database.py
--rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-9.0.2/src/spellbot/environment.py
--rw-r--r--   0        0        0     1125 2023-04-25 03:19:31.676087 spellbot-9.0.2/src/spellbot/errors.py
--rw-r--r--   0        0        0      939 2023-04-25 03:19:31.676348 spellbot-9.0.2/src/spellbot/logs.py
--rw-r--r--   0        0        0     4845 2023-04-25 03:19:31.676603 spellbot-9.0.2/src/spellbot/metrics.py
--rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-9.0.2/src/spellbot/migrations/alembic.ini
--rw-r--r--   0        0        0     1638 2023-04-25 03:19:31.676886 spellbot-9.0.2/src/spellbot/migrations/env.py
--rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-9.0.2/src/spellbot/migrations/script.py.mako
--rw-r--r--   0        0        0     2924 2023-07-19 16:08:41.759508 spellbot-9.0.2/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py
--rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-9.0.2/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
--rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-9.0.2/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
--rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-9.0.2/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
--rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-9.0.2/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
--rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-9.0.2/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
--rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-9.0.2/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
--rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-9.0.2/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
--rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-9.0.2/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
--rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-9.0.2/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
--rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-9.0.2/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
--rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-9.0.2/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
--rw-r--r--   0        0        0     1466 2023-07-19 16:08:41.759802 spellbot-9.0.2/src/spellbot/models/__init__.py
--rw-r--r--   0        0        0     3372 2023-06-24 21:54:36.397629 spellbot-9.0.2/src/spellbot/models/award.py
--rw-r--r--   0        0        0     2670 2023-04-25 03:19:31.677412 spellbot-9.0.2/src/spellbot/models/base.py
--rw-r--r--   0        0        0      935 2023-04-18 21:36:17.607770 spellbot-9.0.2/src/spellbot/models/block.py
--rw-r--r--   0        0        0     4003 2023-04-18 21:36:17.607826 spellbot-9.0.2/src/spellbot/models/channel.py
--rw-r--r--   0        0        0     1059 2023-06-24 21:54:36.397930 spellbot-9.0.2/src/spellbot/models/config.py
--rw-r--r--   0        0        0    11386 2023-07-19 16:08:41.760123 spellbot-9.0.2/src/spellbot/models/game.py
--rw-r--r--   0        0        0     2625 2023-04-18 22:53:49.516268 spellbot-9.0.2/src/spellbot/models/guild.py
--rw-r--r--   0        0        0     1081 2023-06-24 21:54:36.398222 spellbot-9.0.2/src/spellbot/models/play.py
--rw-r--r--   0        0        0      855 2023-07-19 16:08:41.760351 spellbot-9.0.2/src/spellbot/models/queue.py
--rw-r--r--   0        0        0     4341 2023-07-19 16:08:41.760636 spellbot-9.0.2/src/spellbot/models/user.py
--rw-r--r--   0        0        0      952 2023-06-24 21:54:36.398413 spellbot-9.0.2/src/spellbot/models/verify.py
--rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-9.0.2/src/spellbot/models/watch.py
--rw-r--r--   0        0        0    18796 2023-07-19 16:08:41.760996 spellbot-9.0.2/src/spellbot/operations.py
--rw-r--r--   0        0        0     1059 2023-04-25 03:19:31.678344 spellbot-9.0.2/src/spellbot/services/__init__.py
--rw-r--r--   0        0        0     3202 2023-05-26 20:08:39.548754 spellbot-9.0.2/src/spellbot/services/awards.py
--rw-r--r--   0        0        0     5038 2023-06-14 15:20:15.567285 spellbot-9.0.2/src/spellbot/services/channels.py
--rw-r--r--   0        0        0     1555 2023-05-26 20:08:39.549976 spellbot-9.0.2/src/spellbot/services/configs.py
--rw-r--r--   0        0        0    15479 2023-07-19 18:16:27.660096 spellbot-9.0.2/src/spellbot/services/games.py
--rw-r--r--   0        0        0     4841 2023-05-26 20:08:39.550465 spellbot-9.0.2/src/spellbot/services/guilds.py
--rw-r--r--   0        0        0     7539 2023-05-26 20:08:39.550699 spellbot-9.0.2/src/spellbot/services/plays.py
--rw-r--r--   0        0        0     7036 2023-07-19 16:08:41.761644 spellbot-9.0.2/src/spellbot/services/users.py
--rw-r--r--   0        0        0     1631 2023-05-26 20:08:39.551170 spellbot-9.0.2/src/spellbot/services/verifies.py
--rw-r--r--   0        0        0      504 2023-05-26 20:08:39.552173 spellbot-9.0.2/src/spellbot/services/watches.py
--rw-r--r--   0        0        0     3856 2023-07-19 16:08:41.761930 spellbot-9.0.2/src/spellbot/settings.py
--rw-r--r--   0        0        0     2377 2023-07-04 17:01:13.493720 spellbot-9.0.2/src/spellbot/spelltable.py
--rw-r--r--   0        0        0    10934 2023-07-07 01:58:15.645427 spellbot-9.0.2/src/spellbot/utils.py
--rw-r--r--   0        0        0      295 2023-04-26 18:55:38.771824 spellbot-9.0.2/src/spellbot/views/__init__.py
--rw-r--r--   0        0        0      302 2023-04-25 03:19:31.680995 spellbot-9.0.2/src/spellbot/views/base_view.py
--rw-r--r--   0        0        0     4076 2023-07-19 16:08:41.762229 spellbot-9.0.2/src/spellbot/views/lfg_view.py
--rw-r--r--   0        0        0     2482 2023-05-19 17:20:13.375617 spellbot-9.0.2/src/spellbot/views/setup_view.py
--rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-9.0.2/src/spellbot/web/__init__.py
--rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-9.0.2/src/spellbot/web/api/__init__.py
--rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-9.0.2/src/spellbot/web/api/ping.py
--rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-9.0.2/src/spellbot/web/api/record.py
--rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-9.0.2/src/spellbot/web/builder.py
--rw-r--r--   0        0        0      689 2023-04-25 03:19:31.681447 spellbot-9.0.2/src/spellbot/web/server.py
--rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-9.0.2/src/spellbot/web/templates/channel_record.html.j2
--rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-9.0.2/src/spellbot/web/templates/record.css
--rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-9.0.2/src/spellbot/web/templates/record_base.html.j2
--rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-9.0.2/src/spellbot/web/templates/table2CSV.js
--rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-9.0.2/src/spellbot/web/templates/user_record.html.j2
--rw-r--r--   0        0        0    12908 1970-01-01 00:00:00.000000 spellbot-9.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-9.0.3/LICENSE.md
+-rw-r--r--   0        0        0    10824 2023-04-18 21:36:17.595924 spellbot-9.0.3/README.md
+-rw-r--r--   0        0        0     3561 2023-08-03 22:42:38.471840 spellbot-9.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-9.0.3/src/spellbot/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-25 03:19:31.669125 spellbot-9.0.3/src/spellbot/_version.py
+-rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-9.0.3/src/spellbot/actions/__init__.py
+-rw-r--r--   0        0        0    15152 2023-07-19 16:08:41.755106 spellbot-9.0.3/src/spellbot/actions/admin_action.py
+-rw-r--r--   0        0        0     3577 2023-05-26 20:08:39.547131 spellbot-9.0.3/src/spellbot/actions/base_action.py
+-rw-r--r--   0        0        0     1491 2023-04-18 21:36:17.604572 spellbot-9.0.3/src/spellbot/actions/block_action.py
+-rw-r--r--   0        0        0     1719 2023-07-19 16:08:41.755436 spellbot-9.0.3/src/spellbot/actions/config_action.py
+-rw-r--r--   0        0        0     4951 2023-07-19 16:08:41.755771 spellbot-9.0.3/src/spellbot/actions/leave_action.py
+-rw-r--r--   0        0        0    19245 2023-07-19 16:08:41.756139 spellbot-9.0.3/src/spellbot/actions/lfg_action.py
+-rw-r--r--   0        0        0     3238 2023-06-14 15:20:15.566402 spellbot-9.0.3/src/spellbot/actions/score_action.py
+-rw-r--r--   0        0        0     7517 2023-07-19 16:08:41.756468 spellbot-9.0.3/src/spellbot/actions/tasks_action.py
+-rw-r--r--   0        0        0      996 2023-06-14 15:20:15.566614 spellbot-9.0.3/src/spellbot/actions/verify_action.py
+-rw-r--r--   0        0        0     4819 2023-07-19 16:08:41.756793 spellbot-9.0.3/src/spellbot/actions/watch_action.py
+-rw-r--r--   0        0        0     3470 2023-07-19 16:08:41.757174 spellbot-9.0.3/src/spellbot/cli.py
+-rw-r--r--   0        0        0     6714 2023-07-23 05:04:54.812283 spellbot-9.0.3/src/spellbot/client.py
+-rw-r--r--   0        0        0     2082 2023-07-19 16:08:41.757681 spellbot-9.0.3/src/spellbot/cogs/__init__.py
+-rw-r--r--   0        0        0     1987 2023-04-25 03:19:31.672344 spellbot-9.0.3/src/spellbot/cogs/about_cog.py
+-rw-r--r--   0        0        0     9862 2023-07-19 16:08:41.757984 spellbot-9.0.3/src/spellbot/cogs/admin_cog.py
+-rw-r--r--   0        0        0     1563 2023-04-25 03:19:31.672995 spellbot-9.0.3/src/spellbot/cogs/block_cog.py
+-rw-r--r--   0        0        0     1708 2023-07-19 16:08:41.758282 spellbot-9.0.3/src/spellbot/cogs/config_cog.py
+-rw-r--r--   0        0        0     1673 2023-05-19 17:20:13.374286 spellbot-9.0.3/src/spellbot/cogs/events_cog.py
+-rw-r--r--   0        0        0     1576 2023-07-19 16:08:41.758545 spellbot-9.0.3/src/spellbot/cogs/leave_cog.py
+-rw-r--r--   0        0        0     2000 2023-07-19 16:08:41.758724 spellbot-9.0.3/src/spellbot/cogs/lfg_cog.py
+-rw-r--r--   0        0        0     3128 2023-04-25 03:19:31.674236 spellbot-9.0.3/src/spellbot/cogs/owner_cog.py
+-rw-r--r--   0        0        0     2182 2023-04-25 03:19:31.674424 spellbot-9.0.3/src/spellbot/cogs/score_cog.py
+-rw-r--r--   0        0        0     1130 2023-04-25 03:19:31.674692 spellbot-9.0.3/src/spellbot/cogs/sync_cog.py
+-rw-r--r--   0        0        0     3485 2023-07-19 16:08:41.759001 spellbot-9.0.3/src/spellbot/cogs/tasks_cog.py
+-rw-r--r--   0        0        0     1658 2023-04-25 03:19:31.675274 spellbot-9.0.3/src/spellbot/cogs/verify_cog.py
+-rw-r--r--   0        0        0     2672 2023-07-19 16:08:41.759238 spellbot-9.0.3/src/spellbot/cogs/watch_cog.py
+-rw-r--r--   0        0        0     4708 2023-05-26 20:08:39.548488 spellbot-9.0.3/src/spellbot/database.py
+-rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-9.0.3/src/spellbot/environment.py
+-rw-r--r--   0        0        0     1125 2023-04-25 03:19:31.676087 spellbot-9.0.3/src/spellbot/errors.py
+-rw-r--r--   0        0        0      939 2023-04-25 03:19:31.676348 spellbot-9.0.3/src/spellbot/logs.py
+-rw-r--r--   0        0        0     4845 2023-04-25 03:19:31.676603 spellbot-9.0.3/src/spellbot/metrics.py
+-rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-9.0.3/src/spellbot/migrations/alembic.ini
+-rw-r--r--   0        0        0     1638 2023-04-25 03:19:31.676886 spellbot-9.0.3/src/spellbot/migrations/env.py
+-rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-9.0.3/src/spellbot/migrations/script.py.mako
+-rw-r--r--   0        0        0     2924 2023-07-19 16:08:41.759508 spellbot-9.0.3/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py
+-rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-9.0.3/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
+-rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-9.0.3/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
+-rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-9.0.3/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
+-rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-9.0.3/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
+-rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-9.0.3/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
+-rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-9.0.3/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
+-rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-9.0.3/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
+-rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-9.0.3/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
+-rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-9.0.3/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
+-rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-9.0.3/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
+-rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-9.0.3/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
+-rw-r--r--   0        0        0     1466 2023-07-19 16:08:41.759802 spellbot-9.0.3/src/spellbot/models/__init__.py
+-rw-r--r--   0        0        0     3372 2023-06-24 21:54:36.397629 spellbot-9.0.3/src/spellbot/models/award.py
+-rw-r--r--   0        0        0     2670 2023-04-25 03:19:31.677412 spellbot-9.0.3/src/spellbot/models/base.py
+-rw-r--r--   0        0        0      935 2023-04-18 21:36:17.607770 spellbot-9.0.3/src/spellbot/models/block.py
+-rw-r--r--   0        0        0     4003 2023-04-18 21:36:17.607826 spellbot-9.0.3/src/spellbot/models/channel.py
+-rw-r--r--   0        0        0     1059 2023-06-24 21:54:36.397930 spellbot-9.0.3/src/spellbot/models/config.py
+-rw-r--r--   0        0        0    11386 2023-07-19 16:08:41.760123 spellbot-9.0.3/src/spellbot/models/game.py
+-rw-r--r--   0        0        0     2625 2023-04-18 22:53:49.516268 spellbot-9.0.3/src/spellbot/models/guild.py
+-rw-r--r--   0        0        0     1081 2023-06-24 21:54:36.398222 spellbot-9.0.3/src/spellbot/models/play.py
+-rw-r--r--   0        0        0      855 2023-07-19 16:08:41.760351 spellbot-9.0.3/src/spellbot/models/queue.py
+-rw-r--r--   0        0        0     4341 2023-07-19 16:08:41.760636 spellbot-9.0.3/src/spellbot/models/user.py
+-rw-r--r--   0        0        0      952 2023-06-24 21:54:36.398413 spellbot-9.0.3/src/spellbot/models/verify.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-9.0.3/src/spellbot/models/watch.py
+-rw-r--r--   0        0        0    18796 2023-07-19 16:08:41.760996 spellbot-9.0.3/src/spellbot/operations.py
+-rw-r--r--   0        0        0     1059 2023-04-25 03:19:31.678344 spellbot-9.0.3/src/spellbot/services/__init__.py
+-rw-r--r--   0        0        0     3202 2023-05-26 20:08:39.548754 spellbot-9.0.3/src/spellbot/services/awards.py
+-rw-r--r--   0        0        0     5038 2023-06-14 15:20:15.567285 spellbot-9.0.3/src/spellbot/services/channels.py
+-rw-r--r--   0        0        0     1555 2023-05-26 20:08:39.549976 spellbot-9.0.3/src/spellbot/services/configs.py
+-rw-r--r--   0        0        0    15479 2023-07-19 18:16:27.660096 spellbot-9.0.3/src/spellbot/services/games.py
+-rw-r--r--   0        0        0     4841 2023-05-26 20:08:39.550465 spellbot-9.0.3/src/spellbot/services/guilds.py
+-rw-r--r--   0        0        0     7539 2023-05-26 20:08:39.550699 spellbot-9.0.3/src/spellbot/services/plays.py
+-rw-r--r--   0        0        0     6779 2023-08-03 22:42:30.886621 spellbot-9.0.3/src/spellbot/services/users.py
+-rw-r--r--   0        0        0     1631 2023-05-26 20:08:39.551170 spellbot-9.0.3/src/spellbot/services/verifies.py
+-rw-r--r--   0        0        0      504 2023-05-26 20:08:39.552173 spellbot-9.0.3/src/spellbot/services/watches.py
+-rw-r--r--   0        0        0     3856 2023-07-19 16:08:41.761930 spellbot-9.0.3/src/spellbot/settings.py
+-rw-r--r--   0        0        0     2377 2023-07-04 17:01:13.493720 spellbot-9.0.3/src/spellbot/spelltable.py
+-rw-r--r--   0        0        0    10934 2023-07-07 01:58:15.645427 spellbot-9.0.3/src/spellbot/utils.py
+-rw-r--r--   0        0        0      295 2023-04-26 18:55:38.771824 spellbot-9.0.3/src/spellbot/views/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-25 03:19:31.680995 spellbot-9.0.3/src/spellbot/views/base_view.py
+-rw-r--r--   0        0        0     4076 2023-07-19 16:08:41.762229 spellbot-9.0.3/src/spellbot/views/lfg_view.py
+-rw-r--r--   0        0        0     2482 2023-05-19 17:20:13.375617 spellbot-9.0.3/src/spellbot/views/setup_view.py
+-rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-9.0.3/src/spellbot/web/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-9.0.3/src/spellbot/web/api/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-9.0.3/src/spellbot/web/api/ping.py
+-rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-9.0.3/src/spellbot/web/api/record.py
+-rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-9.0.3/src/spellbot/web/builder.py
+-rw-r--r--   0        0        0      689 2023-04-25 03:19:31.681447 spellbot-9.0.3/src/spellbot/web/server.py
+-rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-9.0.3/src/spellbot/web/templates/channel_record.html.j2
+-rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-9.0.3/src/spellbot/web/templates/record.css
+-rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-9.0.3/src/spellbot/web/templates/record_base.html.j2
+-rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-9.0.3/src/spellbot/web/templates/table2CSV.js
+-rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-9.0.3/src/spellbot/web/templates/user_record.html.j2
+-rw-r--r--   0        0        0    12908 1970-01-01 00:00:00.000000 spellbot-9.0.3/PKG-INFO
```

### Comparing `spellbot-9.0.2/LICENSE.md` & `spellbot-9.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/README.md` & `spellbot-9.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/pyproject.toml` & `spellbot-9.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 license = 'MIT'
 name = 'spellbot'
 packages = [
   {include = "spellbot", from = "src"},
 ]
 readme = 'README.md'
 repository = 'https://github.com/lexicalunit/spellbot'
-version = "9.0.2"
+version = "9.0.3"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.4"
 aiohttp-jinja2 = "^1.5.1"
 aiohttp-retry = "^2.8.3"
 alembic = "^1.10.3"
 asgiref = "^3.7.1"
@@ -149,15 +149,15 @@
 exceptiongroup = "^1"
 factory-boy = "^3"
 faker = ">=18,<20"
 gitpython = "^3"
 pexpect = "^4"
 ptyprocess = "^0"
 pylic = "^3.5.0"
-pylint = "2.17.4"
+pylint = "2.17.5"
 pyright = "^1"
 pytest = "^7"
 pytest-aiohttp = "^1"
 pytest-asyncio = "^0"
 pytest-cov = "^4"
 pytest-freezegun = "^0"
 pytest-mock = "^3"
```

### Comparing `spellbot-9.0.2/src/spellbot/_version.py` & `spellbot-9.0.3/src/spellbot/_version.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/__init__.py` & `spellbot-9.0.3/src/spellbot/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/admin_action.py` & `spellbot-9.0.3/src/spellbot/actions/admin_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/base_action.py` & `spellbot-9.0.3/src/spellbot/actions/base_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/block_action.py` & `spellbot-9.0.3/src/spellbot/actions/block_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/config_action.py` & `spellbot-9.0.3/src/spellbot/actions/config_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/leave_action.py` & `spellbot-9.0.3/src/spellbot/actions/leave_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/lfg_action.py` & `spellbot-9.0.3/src/spellbot/actions/lfg_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/score_action.py` & `spellbot-9.0.3/src/spellbot/actions/score_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/tasks_action.py` & `spellbot-9.0.3/src/spellbot/actions/tasks_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/verify_action.py` & `spellbot-9.0.3/src/spellbot/actions/verify_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/actions/watch_action.py` & `spellbot-9.0.3/src/spellbot/actions/watch_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cli.py` & `spellbot-9.0.3/src/spellbot/cli.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/client.py` & `spellbot-9.0.3/src/spellbot/client.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/__init__.py` & `spellbot-9.0.3/src/spellbot/cogs/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/about_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/about_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/admin_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/admin_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/block_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/block_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/config_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/config_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/events_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/events_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/leave_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/leave_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/lfg_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/lfg_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/owner_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/owner_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/score_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/score_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/sync_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/sync_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/tasks_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/tasks_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/verify_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/verify_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/cogs/watch_cog.py` & `spellbot-9.0.3/src/spellbot/cogs/watch_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/database.py` & `spellbot-9.0.3/src/spellbot/database.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/errors.py` & `spellbot-9.0.3/src/spellbot/errors.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/logs.py` & `spellbot-9.0.3/src/spellbot/logs.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/metrics.py` & `spellbot-9.0.3/src/spellbot/metrics.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/alembic.ini` & `spellbot-9.0.3/src/spellbot/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/env.py` & `spellbot-9.0.3/src/spellbot/migrations/env.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py` & `spellbot-9.0.3/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/__init__.py` & `spellbot-9.0.3/src/spellbot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/award.py` & `spellbot-9.0.3/src/spellbot/models/award.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/base.py` & `spellbot-9.0.3/src/spellbot/models/base.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/block.py` & `spellbot-9.0.3/src/spellbot/models/block.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/channel.py` & `spellbot-9.0.3/src/spellbot/models/channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/config.py` & `spellbot-9.0.3/src/spellbot/models/config.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/game.py` & `spellbot-9.0.3/src/spellbot/models/game.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/guild.py` & `spellbot-9.0.3/src/spellbot/models/guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/play.py` & `spellbot-9.0.3/src/spellbot/models/play.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/queue.py` & `spellbot-9.0.3/src/spellbot/models/queue.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/user.py` & `spellbot-9.0.3/src/spellbot/models/user.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/verify.py` & `spellbot-9.0.3/src/spellbot/models/verify.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/models/watch.py` & `spellbot-9.0.3/src/spellbot/models/watch.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/operations.py` & `spellbot-9.0.3/src/spellbot/operations.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/__init__.py` & `spellbot-9.0.3/src/spellbot/services/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/awards.py` & `spellbot-9.0.3/src/spellbot/services/awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/channels.py` & `spellbot-9.0.3/src/spellbot/services/channels.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/configs.py` & `spellbot-9.0.3/src/spellbot/services/configs.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/games.py` & `spellbot-9.0.3/src/spellbot/services/games.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/guilds.py` & `spellbot-9.0.3/src/spellbot/services/guilds.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/plays.py` & `spellbot-9.0.3/src/spellbot/services/plays.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/services/users.py` & `spellbot-9.0.3/src/spellbot/services/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import datetime
 from typing import Any, Optional, Union
 
 import discord
 import pytz
 from asgiref.sync import sync_to_async
-from sqlalchemy import select, update
+from sqlalchemy import update
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.sql.expression import and_
 
 from ..database import DatabaseSession
 from ..models import Block, Game, Queue, User, Watch
 
 
@@ -79,50 +79,44 @@
                 ),
             )
             .first()
         )
         return queue.game_id if queue else None
 
     @sync_to_async()
-    def leave_game(self, channel_xid: int) -> Optional[int]:
+    def leave_game(self, channel_xid: int) -> None:
         assert self.user
-        game = self.user.game(channel_xid)
-        left_game_id = game.id if game else None
-
-        if left_game_id is not None:
-            inner = (
-                select(Game.id)  # type: ignore
-                .join(Queue)
-                .filter(  # type: ignore
-                    and_(
-                        Queue.user_xid == self.user.xid,
-                        Game.channel_xid == channel_xid,
-                    ),
-                )
-            )
-            DatabaseSession.query(Queue).filter(
+        pending_games = (
+            DatabaseSession.query(Queue)
+            .join(Game)
+            .filter(
                 and_(
                     Queue.user_xid == self.user.xid,
-                    Queue.game_id.in_(inner),
+                    Game.channel_xid == channel_xid,
                 ),
-            ).delete()
-            DatabaseSession.commit()
-
-            # This operation should "dirty" the Game, so
-            # we need to update its updated_at field now.
-            query = (
-                update(Game)
-                .where(Game.id == left_game_id)
-                .values(updated_at=datetime.now(tz=pytz.utc))
-                .execution_options(synchronize_session=False)
             )
-            DatabaseSession.execute(query)
-            DatabaseSession.commit()
+        )
+        left_game_ids = [game.game_id for game in pending_games]
+
+        DatabaseSession.query(Queue).filter(
+            Queue.user_xid == self.user.xid,
+            Queue.game_id.in_(left_game_ids),
+        ).delete()
+        DatabaseSession.commit()
 
-        return left_game_id
+        # This operation should "dirty" the Games, so
+        # we need to update their updated_at field now.
+        query = (
+            update(Game)
+            .where(Game.id.in_(left_game_ids))
+            .values(updated_at=datetime.now(tz=pytz.utc))
+            .execution_options(synchronize_session=False)
+        )
+        DatabaseSession.execute(query)
+        DatabaseSession.commit()
 
     @sync_to_async()
     def is_waiting(self, channel_xid: int) -> bool:
         assert self.user
         return self.user.waiting(channel_xid)
 
     @sync_to_async()
```

### Comparing `spellbot-9.0.2/src/spellbot/services/verifies.py` & `spellbot-9.0.3/src/spellbot/services/verifies.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/settings.py` & `spellbot-9.0.3/src/spellbot/settings.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/spelltable.py` & `spellbot-9.0.3/src/spellbot/spelltable.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/utils.py` & `spellbot-9.0.3/src/spellbot/utils.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/views/lfg_view.py` & `spellbot-9.0.3/src/spellbot/views/lfg_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/views/setup_view.py` & `spellbot-9.0.3/src/spellbot/views/setup_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/api/record.py` & `spellbot-9.0.3/src/spellbot/web/api/record.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/builder.py` & `spellbot-9.0.3/src/spellbot/web/builder.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/server.py` & `spellbot-9.0.3/src/spellbot/web/server.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/templates/channel_record.html.j2` & `spellbot-9.0.3/src/spellbot/web/templates/channel_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/templates/record.css` & `spellbot-9.0.3/src/spellbot/web/templates/record.css`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/templates/record_base.html.j2` & `spellbot-9.0.3/src/spellbot/web/templates/record_base.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/templates/table2CSV.js` & `spellbot-9.0.3/src/spellbot/web/templates/table2CSV.js`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/src/spellbot/web/templates/user_record.html.j2` & `spellbot-9.0.3/src/spellbot/web/templates/user_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-9.0.2/PKG-INFO` & `spellbot-9.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spellbot
-Version: 9.0.2
+Version: 9.0.3
 Summary: The Discord bot for SpellTable
 Home-page: http://spellbot.io/
 License: MIT
 Keywords: discord,magic,bot,mtg,SpellTable
 Author: Amy Troschinetz
 Author-email: spellbot@lexicalunit.com
 Requires-Python: >=3.10,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spellbot Version: 9.0.2 Summary: The Discord bot
+Metadata-Version: 2.1 Name: spellbot Version: 9.0.3 Summary: The Discord bot
 for SpellTable Home-page: http://spellbot.io/ License: MIT Keywords:
 discord,magic,bot,mtg,SpellTable Author: Amy Troschinetz Author-email:
 spellbot@lexicalunit.com Requires-Python: >=3.10,<4 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

